# Comparing `tmp/icpp_free-2.8.1-py3-none-any.whl.zip` & `tmp/icpp_free-2.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,160 +1,39 @@
-Zip file size: 220698 bytes, number of entries: 233
+Zip file size: 48410 bytes, number of entries: 80
 -rw-rw-r--  2.0 unx      747 b- defN 23-Apr-29 11:50 icpp/__init__.py
 -rw-rw-r--  2.0 unx     1086 b- defN 23-May-19 20:47 icpp/__main__.py
--rw-rw-r--  2.0 unx     1053 b- defN 23-Jul-08 01:15 icpp/commands_build_native.py
+-rw-rw-r--  2.0 unx     1053 b- defN 23-Jul-10 14:38 icpp/commands_build_native.py
 -rw-rw-r--  2.0 unx     5433 b- defN 23-May-19 20:47 icpp/commands_build_wasm.py
 -rw-rw-r--  2.0 unx     1122 b- defN 23-Apr-29 11:50 icpp/commands_get.py
 -rw-rw-r--  2.0 unx      753 b- defN 23-Apr-29 11:50 icpp/commands_init.py
 -rw-rw-r--  2.0 unx     4724 b- defN 23-Jul-08 00:43 icpp/commands_install_wasi_sdk.py
--rw-rw-r--  2.0 unx     5894 b- defN 23-Jul-08 00:43 icpp/config_default.py
--rw-rw-r--  2.0 unx     2565 b- defN 23-Jul-08 01:15 icpp/conftest_base.py
+-rw-rw-r--  2.0 unx     6070 b- defN 23-Jul-10 14:41 icpp/config_default.py
+-rw-rw-r--  2.0 unx     2565 b- defN 23-Jul-10 14:38 icpp/conftest_base.py
 -rw-rw-r--  2.0 unx     2944 b- defN 23-May-19 20:47 icpp/decorators.py
 -rw-rw-r--  2.0 unx     3776 b- defN 23-May-12 19:56 icpp/icpp_toml.py
 -rw-rw-r--  2.0 unx      670 b- defN 23-May-19 20:47 icpp/options_build.py
--rw-rw-r--  2.0 unx      925 b- defN 23-Jul-08 01:15 icpp/options_main.py
--rw-rw-r--  2.0 unx      879 b- defN 23-Jul-08 01:15 icpp/pro.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Jul-10 14:38 icpp/options_main.py
+-rw-rw-r--  2.0 unx      879 b- defN 23-Jul-10 14:38 icpp/pro.py
 -rw-rw-r--  2.0 unx       98 b- defN 23-Apr-29 11:50 icpp/py.typed
 -rw-rw-r--  2.0 unx     5280 b- defN 23-May-10 21:24 icpp/run_shell_cmd.py
--rw-rw-r--  2.0 unx     1506 b- defN 23-Jul-08 01:15 icpp/smoketest.py
--rw-rw-r--  2.0 unx      322 b- defN 23-Jul-08 01:14 icpp/version.py
+-rw-rw-r--  2.0 unx     1506 b- defN 23-Jul-10 14:38 icpp/smoketest.py
+-rw-rw-r--  2.0 unx      322 b- defN 23-Jul-10 14:41 icpp/version.py
 -rw-rw-r--  2.0 unx      231 b- defN 23-Jul-08 00:43 icpp/version_wasi_sdk.py
 -rw-r--r--  2.0 unx       92 b- defN 23-Apr-29 11:50 icpp/canisters/greet/README.md
 -rwxr-xr-x  2.0 unx      774 b- defN 23-May-30 20:59 icpp/canisters/greet/demo.sh
 -rw-r--r--  2.0 unx      283 b- defN 23-Jun-08 12:04 icpp/canisters/greet/dfx.json
 -rw-r--r--  2.0 unx      474 b- defN 23-Apr-29 11:50 icpp/canisters/greet/icpp.toml
 -rw-rw-r--  2.0 unx     2061 b- defN 23-May-19 20:47 icpp/canisters/greet/native/main.cpp
 -rw-rw-r--  2.0 unx      137 b- defN 23-May-19 20:47 icpp/canisters/greet/native/main.h
 -rw-rw-r--  2.0 unx     3125 b- defN 23-Jun-14 01:34 icpp/canisters/greet/src/greet.cpp
 -rw-r--r--  2.0 unx      469 b- defN 23-May-19 20:47 icpp/canisters/greet/src/greet.did
 -rw-r--r--  2.0 unx      354 b- defN 23-May-19 20:47 icpp/canisters/greet/src/greet.h
 -rw-rw-r--  2.0 unx        0 b- defN 23-Apr-29 11:50 icpp/canisters/greet/test/__init__.py
 -rw-rw-r--  2.0 unx      298 b- defN 23-Apr-29 11:50 icpp/canisters/greet/test/conftest.py
 -rw-rw-r--  2.0 unx     2500 b- defN 23-May-10 21:24 icpp/canisters/greet/test/test_apis.py
--rw-rw-r--  2.0 unx     6153 b- defN 23-May-10 21:33 icpp/ic/candid/candid.h
--rw-rw-r--  2.0 unx      986 b- defN 23-May-10 21:33 icpp/ic/candid/candid_assert.cpp
--rw-rw-r--  2.0 unx      335 b- defN 23-May-10 21:33 icpp/ic/candid/candid_assert.h
--rw-rw-r--  2.0 unx    13930 b- defN 23-May-19 20:47 icpp/ic/candid/candid_deserialize.cpp
--rw-rw-r--  2.0 unx     1392 b- defN 23-May-10 21:33 icpp/ic/candid/candid_deserialize.h
--rw-rw-r--  2.0 unx     7021 b- defN 23-May-10 21:33 icpp/ic/candid/candid_opcode.cpp
--rw-rw-r--  2.0 unx     2878 b- defN 23-May-10 21:33 icpp/ic/candid/candid_opcode.h
--rw-r--r--  2.0 unx     4328 b- defN 23-May-10 21:33 icpp/ic/candid/candid_serialize.cpp
--rw-r--r--  2.0 unx     1000 b- defN 23-May-10 21:33 icpp/ic/candid/candid_serialize.h
--rw-rw-r--  2.0 unx     1761 b- defN 23-Jun-11 11:30 icpp/ic/candid/candid_type_base.cpp
--rw-rw-r--  2.0 unx     1976 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_base.h
--rw-rw-r--  2.0 unx     2048 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_bool.cpp
--rw-rw-r--  2.0 unx      626 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_bool.h
--rw-rw-r--  2.0 unx     1120 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_empty.cpp
--rw-rw-r--  2.0 unx      420 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_empty.h
--rw-rw-r--  2.0 unx     2187 b- defN 23-May-10 22:24 icpp/ic/candid/candid_type_float32.cpp
--rw-rw-r--  2.0 unx      657 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_float32.h
--rw-rw-r--  2.0 unx     2195 b- defN 23-May-10 22:24 icpp/ic/candid/candid_type_float64.cpp
--rw-rw-r--  2.0 unx      664 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_float64.h
--rw-r--r--  2.0 unx     1966 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_int.cpp
--rw-r--r--  2.0 unx      661 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_int.h
--rw-rw-r--  2.0 unx     2016 b- defN 23-May-10 22:24 icpp/ic/candid/candid_type_int16.cpp
--rw-rw-r--  2.0 unx      655 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_int16.h
--rw-rw-r--  2.0 unx     2016 b- defN 23-May-10 22:24 icpp/ic/candid/candid_type_int32.cpp
--rw-rw-r--  2.0 unx      655 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_int32.h
--rw-rw-r--  2.0 unx     2016 b- defN 23-May-10 22:24 icpp/ic/candid/candid_type_int64.cpp
--rw-rw-r--  2.0 unx      655 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_int64.h
--rw-rw-r--  2.0 unx     1990 b- defN 23-May-10 22:24 icpp/ic/candid/candid_type_int8.cpp
--rw-rw-r--  2.0 unx      640 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_int8.h
--rw-rw-r--  2.0 unx     1988 b- defN 23-May-10 22:24 icpp/ic/candid/candid_type_nat.cpp
--rw-rw-r--  2.0 unx      667 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_nat.h
--rw-rw-r--  2.0 unx     2008 b- defN 23-May-10 22:24 icpp/ic/candid/candid_type_nat16.cpp
--rw-rw-r--  2.0 unx      662 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_nat16.h
--rw-rw-r--  2.0 unx     2008 b- defN 23-May-10 22:24 icpp/ic/candid/candid_type_nat32.cpp
--rw-rw-r--  2.0 unx      662 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_nat32.h
--rw-rw-r--  2.0 unx     2008 b- defN 23-May-10 22:24 icpp/ic/candid/candid_type_nat64.cpp
--rw-rw-r--  2.0 unx      662 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_nat64.h
--rw-rw-r--  2.0 unx     1982 b- defN 23-May-10 22:24 icpp/ic/candid/candid_type_nat8.cpp
--rw-rw-r--  2.0 unx      647 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_nat8.h
--rw-rw-r--  2.0 unx      786 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_null.cpp
--rw-rw-r--  2.0 unx      339 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_null.h
--rw-rw-r--  2.0 unx     1819 b- defN 23-May-10 22:24 icpp/ic/candid/candid_type_opt_base.cpp
--rw-rw-r--  2.0 unx      412 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_opt_base.h
--rw-rw-r--  2.0 unx     2679 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_opt_bool.cpp
--rw-rw-r--  2.0 unx      804 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_opt_bool.h
--rw-rw-r--  2.0 unx     2696 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_opt_float32.cpp
--rw-rw-r--  2.0 unx      826 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_opt_float32.h
--rw-rw-r--  2.0 unx     2702 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_opt_float64.cpp
--rw-rw-r--  2.0 unx      833 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_opt_float64.h
--rw-rw-r--  2.0 unx     2688 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_opt_int.cpp
--rw-rw-r--  2.0 unx      841 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_opt_int.h
--rw-rw-r--  2.0 unx     2678 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_opt_int16.cpp
--rw-rw-r--  2.0 unx      830 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_opt_int16.h
--rw-rw-r--  2.0 unx     2678 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_opt_int32.cpp
--rw-rw-r--  2.0 unx      832 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_opt_int32.h
--rw-rw-r--  2.0 unx     2678 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_opt_int64.cpp
--rw-rw-r--  2.0 unx      830 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_opt_int64.h
--rw-rw-r--  2.0 unx     2655 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_opt_int8.cpp
--rw-rw-r--  2.0 unx      818 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_opt_int8.h
--rw-rw-r--  2.0 unx     2694 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_opt_nat.cpp
--rw-rw-r--  2.0 unx      848 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_opt_nat.h
--rw-rw-r--  2.0 unx     2684 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_opt_nat16.cpp
--rw-rw-r--  2.0 unx      837 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_opt_nat16.h
--rw-rw-r--  2.0 unx     2684 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_opt_nat32.cpp
--rw-rw-r--  2.0 unx      837 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_opt_nat32.h
--rw-rw-r--  2.0 unx     2684 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_opt_nat64.cpp
--rw-rw-r--  2.0 unx      837 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_opt_nat64.h
--rw-rw-r--  2.0 unx     2661 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_opt_nat8.cpp
--rw-rw-r--  2.0 unx      825 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_opt_nat8.h
--rw-rw-r--  2.0 unx     2926 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_opt_principal.cpp
--rw-rw-r--  2.0 unx      880 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_opt_principal.h
--rw-rw-r--  2.0 unx     2925 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_opt_text.cpp
--rw-rw-r--  2.0 unx      853 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_opt_text.h
--rw-rw-r--  2.0 unx      148 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_prim.cpp
--rw-rw-r--  2.0 unx      484 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_prim.h
--rw-r--r--  2.0 unx     9795 b- defN 23-Jun-08 12:04 icpp/ic/candid/candid_type_principal.cpp
--rw-rw-r--  2.0 unx     1842 b- defN 23-Jun-08 12:04 icpp/ic/candid/candid_type_principal.h
--rw-rw-r--  2.0 unx    10646 b- defN 23-May-10 22:24 icpp/ic/candid/candid_type_record.cpp
--rw-rw-r--  2.0 unx     1206 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_record.h
--rw-rw-r--  2.0 unx     1045 b- defN 23-May-10 22:24 icpp/ic/candid/candid_type_reserved.cpp
--rw-rw-r--  2.0 unx      434 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_reserved.h
--rw-rw-r--  2.0 unx     2579 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_table.cpp
--rw-rw-r--  2.0 unx      676 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_table.h
--rw-rw-r--  2.0 unx     2861 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_text.cpp
--rw-rw-r--  2.0 unx      728 b- defN 23-May-19 20:47 icpp/ic/candid/candid_type_text.h
--rw-rw-r--  2.0 unx    12406 b- defN 23-Jun-08 12:04 icpp/ic/candid/candid_type_variant.cpp
--rw-rw-r--  2.0 unx     1673 b- defN 23-Jun-08 12:04 icpp/ic/candid/candid_type_variant.h
--rw-rw-r--  2.0 unx     1819 b- defN 23-May-10 22:24 icpp/ic/candid/candid_type_vec_base.cpp
--rw-r--r--  2.0 unx      412 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_vec_base.h
--rw-r--r--  2.0 unx     2485 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_vec_bool.cpp
--rw-r--r--  2.0 unx      678 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_vec_bool.h
--rw-r--r--  2.0 unx     2485 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_vec_float32.cpp
--rw-r--r--  2.0 unx      700 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_vec_float32.h
--rw-r--r--  2.0 unx     2492 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_vec_float64.cpp
--rw-r--r--  2.0 unx      707 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_vec_float64.h
--rw-r--r--  2.0 unx     2457 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_vec_int.cpp
--rw-r--r--  2.0 unx      715 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_vec_int.h
--rw-r--r--  2.0 unx     2502 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_vec_int16.cpp
--rw-r--r--  2.0 unx      704 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_vec_int16.h
--rw-r--r--  2.0 unx     2502 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_vec_int32.cpp
--rw-r--r--  2.0 unx      704 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_vec_int32.h
--rw-r--r--  2.0 unx     2502 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_vec_int64.cpp
--rw-r--r--  2.0 unx      704 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_vec_int64.h
--rw-r--r--  2.0 unx     2479 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_vec_int8.cpp
--rw-r--r--  2.0 unx      692 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_vec_int8.h
--rw-r--r--  2.0 unx     2504 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_vec_nat.cpp
--rw-r--r--  2.0 unx      722 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_vec_nat.h
--rw-r--r--  2.0 unx     2517 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_vec_nat16.cpp
--rw-r--r--  2.0 unx      711 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_vec_nat16.h
--rw-r--r--  2.0 unx     2517 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_vec_nat32.cpp
--rw-r--r--  2.0 unx      711 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_vec_nat32.h
--rw-r--r--  2.0 unx     2517 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_vec_nat64.cpp
--rw-r--r--  2.0 unx      711 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_vec_nat64.h
--rw-r--r--  2.0 unx     2493 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_vec_nat8.cpp
--rw-r--r--  2.0 unx      699 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_vec_nat8.h
--rw-r--r--  2.0 unx     2661 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_vec_principal.cpp
--rw-r--r--  2.0 unx      752 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_vec_principal.h
--rw-r--r--  2.0 unx     2724 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_vec_text.cpp
--rw-r--r--  2.0 unx      727 b- defN 23-May-10 21:33 icpp/ic/candid/candid_type_vec_text.h
--rw-rw-r--  2.0 unx    15454 b- defN 23-May-19 20:47 icpp/ic/candid/vec_bytes.cpp
--rw-rw-r--  2.0 unx     7790 b- defN 23-Jul-08 00:43 icpp/ic/candid/vec_bytes.h
 -rw-r--r--  2.0 unx     1916 b- defN 23-Jun-14 01:34 icpp/ic/canister/canister.h
 -rw-r--r--  2.0 unx      262 b- defN 23-Jun-14 01:34 icpp/ic/canister/canister_base.cpp
 -rw-r--r--  2.0 unx      295 b- defN 23-Jun-14 01:34 icpp/ic/canister/canister_base.h
 -rw-r--r--  2.0 unx      269 b- defN 23-Jun-14 01:34 icpp/ic/canister/canister_cleanup_callback.cpp
 -rw-r--r--  2.0 unx      240 b- defN 23-Jun-14 01:34 icpp/ic/canister/canister_cleanup_callback.h
 -rw-r--r--  2.0 unx      245 b- defN 23-Jun-14 01:34 icpp/ic/canister/canister_global_timer.cpp
 -rw-r--r--  2.0 unx      224 b- defN 23-Jun-14 01:34 icpp/ic/canister/canister_global_timer.h
@@ -176,60 +55,28 @@
 -rw-r--r--  2.0 unx      232 b- defN 23-Jun-14 01:34 icpp/ic/canister/canister_reply_callback.h
 -rw-r--r--  2.0 unx      209 b- defN 23-Jun-14 01:34 icpp/ic/canister/canister_start.cpp
 -rw-r--r--  2.0 unx      200 b- defN 23-Jun-14 01:34 icpp/ic/canister/canister_start.h
 -rw-r--r--  2.0 unx      215 b- defN 23-Jun-14 01:34 icpp/ic/canister/canister_update.cpp
 -rw-r--r--  2.0 unx      204 b- defN 23-Jun-14 01:34 icpp/ic/canister/canister_update.h
 -rw-rw-r--  2.0 unx     3407 b- defN 23-Apr-29 11:50 icpp/ic/ic0/ic0.h
 -rw-r--r--  2.0 unx      110 b- defN 23-Apr-29 11:50 icpp/ic/ic0mock/global.h
--rw-r--r--  2.0 unx     3288 b- defN 23-Jul-08 01:15 icpp/ic/ic0mock/ic0.cpp
+-rw-r--r--  2.0 unx     3288 b- defN 23-Jul-10 14:38 icpp/ic/ic0mock/ic0.cpp
 -rw-rw-r--  2.0 unx     2091 b- defN 23-Apr-29 11:50 icpp/ic/ic0mock/ic0.h
--rw-r--r--  2.0 unx     1372 b- defN 23-Jul-08 01:15 icpp/ic/ic0mock/mock_ic.cpp
+-rw-r--r--  2.0 unx     1372 b- defN 23-Jul-10 14:38 icpp/ic/ic0mock/mock_ic.cpp
 -rw-rw-r--  2.0 unx     1495 b- defN 23-May-01 15:09 icpp/ic/ic0mock/mock_ic.h
 -rw-rw-r--  2.0 unx     6636 b- defN 23-Jun-14 01:34 icpp/ic/icapi/ic_api.cpp
 -rw-rw-r--  2.0 unx     9710 b- defN 23-Jul-08 00:43 icpp/ic/icapi/ic_api.h
 -rw-r--r--  2.0 unx      463 b- defN 23-Apr-29 11:50 icpp/ic/icapi/wasm_symbol.h
--rw-r--r--  2.0 unx      754 b- defN 23-Jul-08 01:15 icpp/ic/pro/pro.cpp
+-rw-r--r--  2.0 unx      754 b- defN 23-Jul-10 14:38 icpp/ic/pro/pro.cpp
 -rw-r--r--  2.0 unx      393 b- defN 23-Apr-29 17:59 icpp/ic/pro/pro.h
--rw-rw-r--  2.0 unx     1155 b- defN 23-Apr-29 11:50 icpp/ic/vendors/cppcodec/LICENSE
--rw-rw-r--  2.0 unx     3933 b- defN 23-Apr-29 11:50 icpp/ic/vendors/cppcodec/base32_crockford.hpp
--rw-rw-r--  2.0 unx     1366 b- defN 23-Apr-29 11:50 icpp/ic/vendors/cppcodec/base32_default_crockford.hpp
--rw-rw-r--  2.0 unx     1342 b- defN 23-Apr-29 11:50 icpp/ic/vendors/cppcodec/base32_default_hex.hpp
--rw-rw-r--  2.0 unx     1356 b- defN 23-Apr-29 11:50 icpp/ic/vendors/cppcodec/base32_default_rfc4648.hpp
--rw-rw-r--  2.0 unx     3090 b- defN 23-Apr-29 11:50 icpp/ic/vendors/cppcodec/base32_hex.hpp
--rw-rw-r--  2.0 unx     3143 b- defN 23-Apr-29 11:50 icpp/ic/vendors/cppcodec/base32_rfc4648.hpp
--rw-rw-r--  2.0 unx     1356 b- defN 23-Apr-29 11:50 icpp/ic/vendors/cppcodec/base64_default_rfc4648.hpp
--rw-rw-r--  2.0 unx     1336 b- defN 23-Apr-29 11:50 icpp/ic/vendors/cppcodec/base64_default_url.hpp
--rw-rw-r--  2.0 unx     1381 b- defN 23-Apr-29 11:50 icpp/ic/vendors/cppcodec/base64_default_url_unpadded.hpp
--rw-rw-r--  2.0 unx     3070 b- defN 23-Apr-29 11:50 icpp/ic/vendors/cppcodec/base64_rfc4648.hpp
--rw-rw-r--  2.0 unx     3201 b- defN 23-Apr-29 11:50 icpp/ic/vendors/cppcodec/base64_url.hpp
--rw-rw-r--  2.0 unx     1805 b- defN 23-Apr-29 11:50 icpp/ic/vendors/cppcodec/base64_url_unpadded.hpp
--rw-rw-r--  2.0 unx     1328 b- defN 23-Apr-29 11:50 icpp/ic/vendors/cppcodec/hex_default_lower.hpp
--rw-rw-r--  2.0 unx     1328 b- defN 23-Apr-29 11:50 icpp/ic/vendors/cppcodec/hex_default_upper.hpp
--rw-rw-r--  2.0 unx     3009 b- defN 23-Apr-29 11:50 icpp/ic/vendors/cppcodec/hex_lower.hpp
--rw-rw-r--  2.0 unx     2994 b- defN 23-Apr-29 11:50 icpp/ic/vendors/cppcodec/hex_upper.hpp
--rw-rw-r--  2.0 unx     3283 b- defN 23-Apr-29 11:50 icpp/ic/vendors/cppcodec/parse_error.hpp
--rw-rw-r--  2.0 unx    12087 b- defN 23-Apr-29 11:50 icpp/ic/vendors/cppcodec/data/access.hpp
--rw-rw-r--  2.0 unx     2352 b- defN 23-Apr-29 11:50 icpp/ic/vendors/cppcodec/data/raw_result_buffer.hpp
--rw-rw-r--  2.0 unx     7970 b- defN 23-Apr-29 11:50 icpp/ic/vendors/cppcodec/detail/base32.hpp
--rw-rw-r--  2.0 unx     5676 b- defN 23-Apr-29 11:50 icpp/ic/vendors/cppcodec/detail/base64.hpp
--rw-rw-r--  2.0 unx    11905 b- defN 23-Apr-29 11:50 icpp/ic/vendors/cppcodec/detail/codec.hpp
--rw-rw-r--  2.0 unx     1606 b- defN 23-Apr-29 11:50 icpp/ic/vendors/cppcodec/detail/config.hpp
--rw-rw-r--  2.0 unx     4533 b- defN 23-Apr-29 11:50 icpp/ic/vendors/cppcodec/detail/hex.hpp
--rw-rw-r--  2.0 unx    19640 b- defN 23-Apr-29 11:50 icpp/ic/vendors/cppcodec/detail/stream_codec.hpp
--rw-r--r--  2.0 unx      861 b- defN 23-Apr-29 11:50 icpp/ic/vendors/hash-library/LICENSE
--rw-r--r--  2.0 unx    31026 b- defN 23-Jun-08 12:04 icpp/ic/vendors/hash-library/crc32.cpp
--rw-r--r--  2.0 unx     1736 b- defN 23-Apr-29 11:50 icpp/ic/vendors/hash-library/crc32.h
--rw-r--r--  2.0 unx     1758 b- defN 23-Apr-29 11:50 icpp/ic/vendors/hash-library/readme.md
--rw-r--r--  2.0 unx    15133 b- defN 23-Jun-08 12:04 icpp/ic/vendors/hash-library/sha256.cpp
--rw-r--r--  2.0 unx     1968 b- defN 23-Jun-08 12:04 icpp/ic/vendors/hash-library/sha256.h
 -rw-rw-r--  2.0 unx     1370 b- defN 23-Apr-29 11:50 icpp/ic/wasi_sdk_traps/__wasilibc_initialize_environ.c
 -rw-rw-r--  2.0 unx      327 b- defN 23-Apr-29 11:50 icpp/ic/wasi_sdk_traps/ic_trap.c
 -rw-rw-r--  2.0 unx       70 b- defN 23-Apr-29 11:50 icpp/ic/wasi_sdk_traps/ic_trap.h
 -rw-rw-r--  2.0 unx     4743 b- defN 23-May-19 20:47 icpp/ic/wasi_sdk_traps/posix.c
 -rw-r--r--  2.0 unx    10198 b- defN 23-May-19 20:47 icpp/ic/wasi_sdk_traps/unreachable.c
--rw-r--r--  2.0 unx     1066 b- defN 23-Jul-08 01:18 icpp_free-2.8.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1735 b- defN 23-Jul-08 01:18 icpp_free-2.8.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-08 01:18 icpp_free-2.8.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       44 b- defN 23-Jul-08 01:18 icpp_free-2.8.1.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        5 b- defN 23-Jul-08 01:18 icpp_free-2.8.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    21399 b- defN 23-Jul-08 01:19 icpp_free-2.8.1.dist-info/RECORD
-233 files, 542333 bytes uncompressed, 186410 bytes compressed:  65.6%
+-rw-r--r--  2.0 unx     1066 b- defN 23-Jul-10 14:47 icpp_free-2.9.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1772 b- defN 23-Jul-10 14:47 icpp_free-2.9.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-10 14:47 icpp_free-2.9.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       44 b- defN 23-Jul-10 14:47 icpp_free-2.9.0.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        5 b- defN 23-Jul-10 14:47 icpp_free-2.9.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     6905 b- defN 23-Jul-10 14:47 icpp_free-2.9.0.dist-info/RECORD
+80 files, 115013 bytes uncompressed, 37390 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -87,377 +87,14 @@
 
 Filename: icpp/canisters/greet/test/conftest.py
 Comment: 
 
 Filename: icpp/canisters/greet/test/test_apis.py
 Comment: 
 
-Filename: icpp/ic/candid/candid.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_assert.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_assert.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_deserialize.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_deserialize.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_opcode.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_opcode.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_serialize.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_serialize.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_base.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_base.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_bool.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_bool.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_empty.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_empty.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_float32.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_float32.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_float64.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_float64.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_int.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_int.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_int16.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_int16.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_int32.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_int32.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_int64.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_int64.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_int8.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_int8.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_nat.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_nat.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_nat16.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_nat16.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_nat32.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_nat32.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_nat64.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_nat64.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_nat8.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_nat8.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_null.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_null.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_opt_base.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_opt_base.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_opt_bool.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_opt_bool.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_opt_float32.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_opt_float32.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_opt_float64.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_opt_float64.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_opt_int.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_opt_int.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_opt_int16.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_opt_int16.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_opt_int32.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_opt_int32.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_opt_int64.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_opt_int64.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_opt_int8.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_opt_int8.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_opt_nat.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_opt_nat.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_opt_nat16.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_opt_nat16.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_opt_nat32.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_opt_nat32.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_opt_nat64.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_opt_nat64.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_opt_nat8.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_opt_nat8.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_opt_principal.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_opt_principal.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_opt_text.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_opt_text.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_prim.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_prim.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_principal.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_principal.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_record.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_record.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_reserved.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_reserved.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_table.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_table.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_text.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_text.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_variant.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_variant.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_vec_base.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_vec_base.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_vec_bool.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_vec_bool.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_vec_float32.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_vec_float32.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_vec_float64.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_vec_float64.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_vec_int.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_vec_int.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_vec_int16.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_vec_int16.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_vec_int32.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_vec_int32.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_vec_int64.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_vec_int64.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_vec_int8.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_vec_int8.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_vec_nat.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_vec_nat.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_vec_nat16.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_vec_nat16.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_vec_nat32.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_vec_nat32.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_vec_nat64.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_vec_nat64.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_vec_nat8.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_vec_nat8.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_vec_principal.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_vec_principal.h
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_vec_text.cpp
-Comment: 
-
-Filename: icpp/ic/candid/candid_type_vec_text.h
-Comment: 
-
-Filename: icpp/ic/candid/vec_bytes.cpp
-Comment: 
-
-Filename: icpp/ic/candid/vec_bytes.h
-Comment: 
-
 Filename: icpp/ic/canister/canister.h
 Comment: 
 
 Filename: icpp/ic/canister/canister_base.cpp
 Comment: 
 
 Filename: icpp/ic/canister/canister_base.h
@@ -564,110 +201,14 @@
 
 Filename: icpp/ic/pro/pro.cpp
 Comment: 
 
 Filename: icpp/ic/pro/pro.h
 Comment: 
 
-Filename: icpp/ic/vendors/cppcodec/LICENSE
-Comment: 
-
-Filename: icpp/ic/vendors/cppcodec/base32_crockford.hpp
-Comment: 
-
-Filename: icpp/ic/vendors/cppcodec/base32_default_crockford.hpp
-Comment: 
-
-Filename: icpp/ic/vendors/cppcodec/base32_default_hex.hpp
-Comment: 
-
-Filename: icpp/ic/vendors/cppcodec/base32_default_rfc4648.hpp
-Comment: 
-
-Filename: icpp/ic/vendors/cppcodec/base32_hex.hpp
-Comment: 
-
-Filename: icpp/ic/vendors/cppcodec/base32_rfc4648.hpp
-Comment: 
-
-Filename: icpp/ic/vendors/cppcodec/base64_default_rfc4648.hpp
-Comment: 
-
-Filename: icpp/ic/vendors/cppcodec/base64_default_url.hpp
-Comment: 
-
-Filename: icpp/ic/vendors/cppcodec/base64_default_url_unpadded.hpp
-Comment: 
-
-Filename: icpp/ic/vendors/cppcodec/base64_rfc4648.hpp
-Comment: 
-
-Filename: icpp/ic/vendors/cppcodec/base64_url.hpp
-Comment: 
-
-Filename: icpp/ic/vendors/cppcodec/base64_url_unpadded.hpp
-Comment: 
-
-Filename: icpp/ic/vendors/cppcodec/hex_default_lower.hpp
-Comment: 
-
-Filename: icpp/ic/vendors/cppcodec/hex_default_upper.hpp
-Comment: 
-
-Filename: icpp/ic/vendors/cppcodec/hex_lower.hpp
-Comment: 
-
-Filename: icpp/ic/vendors/cppcodec/hex_upper.hpp
-Comment: 
-
-Filename: icpp/ic/vendors/cppcodec/parse_error.hpp
-Comment: 
-
-Filename: icpp/ic/vendors/cppcodec/data/access.hpp
-Comment: 
-
-Filename: icpp/ic/vendors/cppcodec/data/raw_result_buffer.hpp
-Comment: 
-
-Filename: icpp/ic/vendors/cppcodec/detail/base32.hpp
-Comment: 
-
-Filename: icpp/ic/vendors/cppcodec/detail/base64.hpp
-Comment: 
-
-Filename: icpp/ic/vendors/cppcodec/detail/codec.hpp
-Comment: 
-
-Filename: icpp/ic/vendors/cppcodec/detail/config.hpp
-Comment: 
-
-Filename: icpp/ic/vendors/cppcodec/detail/hex.hpp
-Comment: 
-
-Filename: icpp/ic/vendors/cppcodec/detail/stream_codec.hpp
-Comment: 
-
-Filename: icpp/ic/vendors/hash-library/LICENSE
-Comment: 
-
-Filename: icpp/ic/vendors/hash-library/crc32.cpp
-Comment: 
-
-Filename: icpp/ic/vendors/hash-library/crc32.h
-Comment: 
-
-Filename: icpp/ic/vendors/hash-library/readme.md
-Comment: 
-
-Filename: icpp/ic/vendors/hash-library/sha256.cpp
-Comment: 
-
-Filename: icpp/ic/vendors/hash-library/sha256.h
-Comment: 
-
 Filename: icpp/ic/wasi_sdk_traps/__wasilibc_initialize_environ.c
 Comment: 
 
 Filename: icpp/ic/wasi_sdk_traps/ic_trap.c
 Comment: 
 
 Filename: icpp/ic/wasi_sdk_traps/ic_trap.h
@@ -675,26 +216,26 @@
 
 Filename: icpp/ic/wasi_sdk_traps/posix.c
 Comment: 
 
 Filename: icpp/ic/wasi_sdk_traps/unreachable.c
 Comment: 
 
-Filename: icpp_free-2.8.1.dist-info/LICENSE
+Filename: icpp_free-2.9.0.dist-info/LICENSE
 Comment: 
 
-Filename: icpp_free-2.8.1.dist-info/METADATA
+Filename: icpp_free-2.9.0.dist-info/METADATA
 Comment: 
 
-Filename: icpp_free-2.8.1.dist-info/WHEEL
+Filename: icpp_free-2.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: icpp_free-2.8.1.dist-info/entry_points.txt
+Filename: icpp_free-2.9.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: icpp_free-2.8.1.dist-info/top_level.txt
+Filename: icpp_free-2.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: icpp_free-2.8.1.dist-info/RECORD
+Filename: icpp_free-2.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## icpp/config_default.py

```diff
@@ -1,14 +1,15 @@
 """
 Set the default config variables
 """
 import sys
 import platform
 from pathlib import Path
 import getpass
+import icpp_candid  # pylint: disable = unused-import
 from icpp import __version_wasi_sdk__
 
 # The OS we're running on - https://stackoverflow.com/a/1857/5480536
 
 OS_SYSTEM = platform.system()
 OS_PROCESSOR = platform.processor()
 
@@ -58,81 +59,85 @@
 )
 
 ICPP_ROOT = Path.home() / ".icpp"
 ICPP_ROOT_UNTAR_DIR = ICPP_ROOT / f"{get_wasi_sdk_untar_dir_name()}"
 ICPP_ROOT_COMPILER = ICPP_ROOT / f"{__version_wasi_sdk__}"
 
 USER = getpass.getuser()
+
 ICPP_PATH = Path(sys.modules["icpp"].__path__[0])
 ICPP_DIR = str(ICPP_PATH)
 
+ICPP_CANDID_PATH = Path(sys.modules["icpp_candid"].__path__[0])
+ICPP_CANDID_DIR = str(ICPP_CANDID_PATH)
+
 ########################################################################
-# init
+# The greet canister created by `icpp init`
 #
 ICPP_INIT_PATH = ICPP_PATH / "canisters/greet"
 LOCAL_INIT_PATH = Path("./greet")
 
 ########################################################################
 # build-wasm
 #
 IC_C_FILES = (
     " ".join(
         [
             str(x)
             for x in list(ICPP_PATH.glob("ic/ic0/*.c"))
             + list(ICPP_PATH.glob("ic/wasi_sdk_traps/*.c"))
-            + list(ICPP_PATH.glob("ic/candid/*.c"))
             + list(ICPP_PATH.glob("ic/canister/*.c"))
             + list(ICPP_PATH.glob("ic/icapi/*.c"))
-            # + list(ICPP_PATH.glob("ic/vendors/*.c"))
+            + list(ICPP_CANDID_PATH.glob("candid/*.c"))
+            # + list(ICPP_CANDID_PATH.glob("vendors/*.c"))
         ]
     )
     + " "
 )
 IC_CPP_FILES = (
     " ".join(
         [
             str(x)
             for x in list(ICPP_PATH.glob("ic/ic0/*.cpp"))
-            + list(ICPP_PATH.glob("ic/candid/*.cpp"))
             + list(ICPP_PATH.glob("ic/canister/*.cpp"))
             + list(ICPP_PATH.glob("ic/icapi/*.cpp"))
             + list(ICPP_PATH.glob("ic/pro/*.cpp"))
-            + list(ICPP_PATH.glob("ic/vendors/hash-library/*.cpp"))
-            # + list(ICPP_PATH.glob("ic/vendors/*.cpp"))
+            + list(ICPP_CANDID_PATH.glob("candid/*.cpp"))
+            + list(ICPP_CANDID_PATH.glob("vendors/hash-library/*.cpp"))
         ]
     )
     + " "
 )
 IC_HEADER_FILES = (
     " ".join(
         [
             str(x)
             for x in list(ICPP_PATH.glob("ic/ic0/*.h"))
             + list(ICPP_PATH.glob("ic/wasi_sdk_traps/*.h"))
-            + list(ICPP_PATH.glob("ic/candid/*.h"))
             + list(ICPP_PATH.glob("ic/canister/*.h"))
             + list(ICPP_PATH.glob("ic/icapi/*.h"))
             + list(ICPP_PATH.glob("ic/pro/*.h"))
-            # + list(ICPP_PATH.glob("ic/vendors/*.h"))
-            # + list(ICPP_PATH.glob("ic/vendors/*.hpp"))
+            + list(ICPP_CANDID_PATH.glob("candid/*.h"))
+            # + list(ICPP_CANDID_PATH.glob("vendors/*.h"))
+            # + list(ICPP_CANDID_PATH.glob("vendors/*.hpp"))
         ]
     )
     + " "
 )
 
 SYSROOT = ICPP_ROOT_COMPILER / "share/wasi-sysroot"
 
 WASM_C = ICPP_ROOT_COMPILER / "bin/clang"
 WASM_CPP = ICPP_ROOT_COMPILER / "bin/clang++"
 WASM_CFLAGS = (
     f" --target=wasm32-wasi -O3 -flto -fno-exceptions -fvisibility=hidden "
     f" --sysroot {SYSROOT} "
-    f" -I {ICPP_DIR}/ic/candid -I {ICPP_DIR}/ic/canister -I {ICPP_DIR}/ic/icapi "
-    f" -I {ICPP_DIR}/ic/pro -I {ICPP_DIR}/ic/ic0 -I {ICPP_DIR}/ic/vendors "
+    f" -I {ICPP_DIR}/ic/canister -I {ICPP_DIR}/ic/icapi "
+    f" -I {ICPP_DIR}/ic/pro -I {ICPP_DIR}/ic/ic0 "
+    f" -I {ICPP_CANDID_PATH}/candid -I {ICPP_CANDID_PATH}/vendors "
     f" -D NDEBUG -D ICPP_VERBOSE=0 "
 )
 WASM_CPPFLAGS = WASM_CFLAGS + " -std=c++20 "
 WASM_LDFLAGS = (
     " -nostartfiles -Wl,--no-entry -Wl,--lto-O3 -Wl,--strip-all "
     " -Wl,--strip-debug -Wl,--stack-first -Wl,--export-dynamic "
 )
@@ -145,56 +150,56 @@
 # build-native
 #
 MOCKIC_C_FILES = (
     " ".join(
         [
             str(x)
             for x in list(ICPP_PATH.glob("ic/ic0mock/*.c"))
-            + list(ICPP_PATH.glob("ic/candid/*.c"))
             + list(ICPP_PATH.glob("ic/canister/*.c"))
             + list(ICPP_PATH.glob("ic/icapi/*.c"))
-            # + list(ICPP_PATH.glob("ic/vendors/*.c"))
+            + list(ICPP_CANDID_PATH.glob("candid/*.c"))
+            # + list(ICPP_CANDID_PATH.glob("vendors/*.c"))
         ]
     )
     + " "
 )
 MOCKIC_CPP_FILES = (
     " ".join(
         [
             str(x)
             for x in list(ICPP_PATH.glob("ic/ic0mock/*.cpp"))
-            + list(ICPP_PATH.glob("ic/candid/*.cpp"))
             + list(ICPP_PATH.glob("ic/canister/*.cpp"))
             + list(ICPP_PATH.glob("ic/icapi/*.cpp"))
             + list(ICPP_PATH.glob("ic/pro/*.cpp"))
-            + list(ICPP_PATH.glob("ic/vendors/hash-library/*.cpp"))
-            # + list(ICPP_PATH.glob("ic/vendors/*.cpp"))
+            + list(ICPP_CANDID_PATH.glob("candid/*.cpp"))
+            + list(ICPP_CANDID_PATH.glob("vendors/hash-library/*.cpp"))
         ]
     )
     + " "
 )
 MOCKIC_HEADER_FILES = (
     " ".join(
         [
             str(x)
             for x in list(ICPP_PATH.glob("ic/ic0mock/*.h"))
-            + list(ICPP_PATH.glob("ic/candid/*.h"))
             + list(ICPP_PATH.glob("ic/canister/*.h"))
             + list(ICPP_PATH.glob("ic/icapi/*.h"))
             + list(ICPP_PATH.glob("ic/pro/*.h"))
-            # + list(ICPP_PATH.glob("ic/vendors/*.h"))
-            # + list(ICPP_PATH.glob("ic/vendors/*.hpp"))
+            + list(ICPP_CANDID_PATH.glob("candid/*.h"))
+            # + list(ICPP_CANDID_PATH.glob("vendors/*.h"))
+            # + list(ICPP_CANDID_PATH.glob("vendors/*.hpp"))
         ]
     )
     + " "
 )
 
 NATIVE_COMPILER = "Clang"
 NATIVE_C = "clang"
 NATIVE_CPP = "clang++"
 NATIVE_CFLAGS = (
-    f" -g  -I {ICPP_DIR}/ic/candid -I {ICPP_DIR}/ic/canister -I {ICPP_DIR}/ic/icapi "
-    f" -I {ICPP_DIR}/ic/pro -I {ICPP_DIR}/ic/ic0mock -I {ICPP_DIR}/ic/vendors "
+    f" -g -I {ICPP_DIR}/ic/canister -I {ICPP_DIR}/ic/icapi "
+    f" -I {ICPP_DIR}/ic/pro -I {ICPP_DIR}/ic/ic0mock "
+    f" -I {ICPP_CANDID_PATH}/candid -I {ICPP_CANDID_PATH}/vendors "
     f" -D ICPP_VERBOSE=0 "
 )
 NATIVE_CPPFLAGS = NATIVE_CFLAGS + " -std=c++20 "
 NATIVE_LDFLAGS = " "
```

## icpp/version.py

```diff
@@ -5,8 +5,8 @@
 (-) do not add anything but the version number here!
 
 We do it this way, so both __init__.py and setup.py can use it.
 
 see:
 https://packaging.python.org/guides/single-sourcing-package-version/
 """
-__version__ = "2.8.1"
+__version__ = "2.9.0"
```

## Comparing `icpp/ic/vendors/cppcodec/LICENSE` & `icpp_free-2.9.0.dist-info/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Copyright (c) 2015 Topology Inc.
-Copyright (c) 2018 Jakob Petsovits
-Copyright (c) various other contributors, see individual files
+MIT License
+
+Copyright (c) 2023 icppWorld
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

## Comparing `icpp_free-2.8.1.dist-info/METADATA` & `icpp_free-2.9.0.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icpp-free
-Version: 2.8.1
+Version: 2.9.0
 Summary: C++ Canister Development Kit (CDK) for the Internet Computer
 Home-page: https://docs.icpp.world/
 Author: icppWorld
 Author-email: icpp@icpp.world
 License: MIT
 Keywords: Internet Computer,C++,Canister Development Kit,CDK,Smart Contracts,blockchain
 Classifier: Development Status :: 4 - Beta
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: icpp-candid (==2.9.0)
 Requires-Dist: typer[all] (>=0.9.0)
 Requires-Dist: tomli
 Requires-Dist: requests
 Requires-Dist: enlighten
 Requires-Dist: pytest
 Provides-Extra: dev
 Requires-Dist: black ; extra == 'dev'
```

