# Comparing `tmp/odxtools-4.0.4.tar.gz` & `tmp/odxtools-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odxtools-4.0.4.tar", last modified: Fri Jul  7 06:40:11 2023, max compression
+gzip compressed data, was "odxtools-4.0.5.tar", last modified: Tue Jul 11 10:04:37 2023, max compression
```

## Comparing `odxtools-4.0.4.tar` & `odxtools-4.0.5.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-07-07 06:40:11.101345 odxtools-4.0.4/
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1069 2022-03-09 15:55:44.000000 odxtools-4.0.4/LICENSE
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    23581 2023-07-07 06:40:11.097345 odxtools-4.0.4/PKG-INFO
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    22767 2022-12-12 08:24:18.000000 odxtools-4.0.4/README.md
-drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-07-07 06:40:11.053344 odxtools-4.0.4/examples/
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)       65 2023-01-27 13:39:15.000000 odxtools-4.0.4/examples/__init__.py
--rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)     1686 2023-06-21 06:52:15.000000 odxtools-4.0.4/examples/isotp_send.py
--rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)      811 2023-01-27 13:39:15.000000 odxtools-4.0.4/examples/mksomersaultpdx.py
--rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)     1612 2023-01-27 13:39:15.000000 odxtools-4.0.4/examples/pdxcopy.py
--rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)    81924 2023-07-02 11:28:36.000000 odxtools-4.0.4/examples/somersaultecu.py
--rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)    19444 2023-01-27 13:39:15.000000 odxtools-4.0.4/examples/somersaultlazy.py
-drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-07-07 06:40:11.073345 odxtools-4.0.4/odxtools/
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2925 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/__init__.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      153 2023-01-13 13:17:58.000000 odxtools-4.0.4/odxtools/__main__.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7853 2023-06-21 06:52:15.000000 odxtools-4.0.4/odxtools/admindata.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4267 2023-06-21 06:52:15.000000 odxtools-4.0.4/odxtools/audience.py
-drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-07-07 06:40:11.077345 odxtools-4.0.4/odxtools/cli/
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      140 2023-01-13 13:17:58.000000 odxtools-4.0.4/odxtools/cli/__init__.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      549 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/cli/_parser_utils.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3287 2023-06-21 06:52:15.000000 odxtools-4.0.4/odxtools/cli/_print_utils.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    14094 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/cli/browse.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1171 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/cli/dummy_sub_parser.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5974 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/cli/find.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7337 2023-07-04 15:58:15.000000 odxtools-4.0.4/odxtools/cli/list.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1809 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/cli/main.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7471 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/cli/snoop.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5302 2023-06-21 06:52:15.000000 odxtools-4.0.4/odxtools/communicationparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     8581 2023-06-28 12:35:57.000000 odxtools-4.0.4/odxtools/companydata.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    11567 2023-06-21 06:52:15.000000 odxtools-4.0.4/odxtools/comparam_subset.py
-drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-07-07 06:40:11.085345 odxtools-4.0.4/odxtools/compumethods/
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      840 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/compumethods/__init__.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      894 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/compumethods/compumethodbase.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      210 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/compumethods/compurationalcoeffs.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1489 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/compumethods/compuscale.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7662 2023-07-02 11:28:36.000000 odxtools-4.0.4/odxtools/compumethods/createanycompumethod.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      843 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/compumethods/identicalcompumethod.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2531 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/compumethods/limit.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     8228 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/compumethods/linearcompumethod.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1692 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/compumethods/scalelinearcompumethod.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     6252 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/compumethods/tabintpcompumethod.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2502 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/compumethods/texttablecompumethod.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5667 2023-06-21 06:52:15.000000 odxtools-4.0.4/odxtools/database.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    15371 2023-06-21 06:52:15.000000 odxtools-4.0.4/odxtools/dataobjectproperty.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      699 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/decodestate.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    27425 2023-06-21 06:52:15.000000 odxtools-4.0.4/odxtools/diagcodedtypes.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     6643 2023-06-21 06:52:15.000000 odxtools-4.0.4/odxtools/diagdatadictionaryspec.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    39660 2023-06-28 12:35:57.000000 odxtools-4.0.4/odxtools/diaglayer.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5957 2023-06-21 06:52:15.000000 odxtools-4.0.4/odxtools/diaglayercontainer.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    11411 2023-06-21 06:52:15.000000 odxtools-4.0.4/odxtools/diaglayerraw.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      908 2023-06-21 06:52:15.000000 odxtools-4.0.4/odxtools/diaglayertype.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     6969 2023-06-28 12:35:57.000000 odxtools-4.0.4/odxtools/ecu_variant_matcher.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3427 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/ecu_variant_patterns.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1190 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/encodestate.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7307 2023-07-07 06:40:10.000000 odxtools-4.0.4/odxtools/endofpdufield.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2429 2023-06-21 06:52:15.000000 odxtools-4.0.4/odxtools/envdata.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5382 2023-06-21 06:52:15.000000 odxtools-4.0.4/odxtools/envdatadesc.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      549 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/exceptions.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1249 2023-06-21 06:52:15.000000 odxtools-4.0.4/odxtools/functionalclass.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      173 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/globals.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    12104 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/isotp_state_machine.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      452 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/load_file.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      310 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/load_odx_d_file.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      334 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/load_pdx_file.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      963 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/message.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    12896 2023-06-21 06:52:15.000000 odxtools-4.0.4/odxtools/multiplexer.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4185 2023-06-21 06:52:15.000000 odxtools-4.0.4/odxtools/nameditemlist.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1209 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/obd.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     8438 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/odxlink.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3469 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/odxtypes.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3467 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/parameter_info.py
-drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-07-07 06:40:11.093345 odxtools-4.0.4/odxtools/parameters/
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      832 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/parameters/__init__.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4330 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/parameters/codedconstparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     9282 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/parameters/createanyparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1566 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/parameters/dynamicparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1387 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/parameters/lengthkeyparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3011 2023-06-28 12:35:57.000000 odxtools-4.0.4/odxtools/parameters/matchingrequestparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4851 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/parameters/nrcconstparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7208 2023-06-21 06:52:15.000000 odxtools-4.0.4/odxtools/parameters/parameterbase.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4108 2023-06-28 12:35:57.000000 odxtools-4.0.4/odxtools/parameters/parameterwithdop.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3263 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/parameters/physicalconstantparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2787 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/parameters/reservedparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1805 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/parameters/systemparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1090 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/parameters/tableentryparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2484 2023-07-02 11:28:36.000000 odxtools-4.0.4/odxtools/parameters/tablekeyparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1230 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/parameters/tablestructparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3130 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/parameters/valueparameter.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3304 2023-06-21 06:52:15.000000 odxtools-4.0.4/odxtools/parentref.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2372 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/physicaltype.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    13655 2023-06-28 12:35:57.000000 odxtools-4.0.4/odxtools/service.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    16374 2023-06-21 06:52:15.000000 odxtools-4.0.4/odxtools/singleecujob.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5290 2023-06-21 06:52:15.000000 odxtools-4.0.4/odxtools/specialdata.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1234 2023-06-21 06:52:15.000000 odxtools-4.0.4/odxtools/state.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3495 2023-06-21 06:52:15.000000 odxtools-4.0.4/odxtools/statechart.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2553 2023-06-21 06:52:15.000000 odxtools-4.0.4/odxtools/statetransition.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    24316 2023-06-21 06:52:15.000000 odxtools-4.0.4/odxtools/structures.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     8058 2023-06-21 06:52:15.000000 odxtools-4.0.4/odxtools/table.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4409 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/uds.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    11672 2023-06-21 06:52:15.000000 odxtools-4.0.4/odxtools/units.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1885 2023-01-27 13:39:15.000000 odxtools-4.0.4/odxtools/utils.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)       87 2023-07-07 06:40:10.000000 odxtools-4.0.4/odxtools/version.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5907 2023-06-21 06:52:15.000000 odxtools-4.0.4/odxtools/write_pdx_file.py
-drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-07-07 06:40:11.077345 odxtools-4.0.4/odxtools.egg-info/
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    23581 2023-07-07 06:40:10.000000 odxtools-4.0.4/odxtools.egg-info/PKG-INFO
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3342 2023-07-07 06:40:10.000000 odxtools-4.0.4/odxtools.egg-info/SOURCES.txt
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)        1 2023-07-07 06:40:10.000000 odxtools-4.0.4/odxtools.egg-info/dependency_links.txt
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)       53 2023-07-07 06:40:10.000000 odxtools-4.0.4/odxtools.egg-info/entry_points.txt
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      100 2023-07-07 06:40:10.000000 odxtools-4.0.4/odxtools.egg-info/requires.txt
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)       18 2023-07-07 06:40:10.000000 odxtools-4.0.4/odxtools.egg-info/top_level.txt
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      382 2023-01-27 13:39:15.000000 odxtools-4.0.4/pyproject.toml
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)       38 2023-07-07 06:40:11.101345 odxtools-4.0.4/setup.cfg
--rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)     2005 2023-01-27 13:39:15.000000 odxtools-4.0.4/setup.py
-drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-07-07 06:40:11.097345 odxtools-4.0.4/tests/
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    14195 2023-07-02 11:28:36.000000 odxtools-4.0.4/tests/test_compu_methods.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    51695 2023-06-28 12:35:57.000000 odxtools-4.0.4/tests/test_decoding.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    36363 2023-06-21 06:52:15.000000 odxtools-4.0.4/tests/test_diag_coded_types.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     9192 2023-06-21 06:52:15.000000 odxtools-4.0.4/tests/test_diag_data_dictionary_spec.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    14065 2023-06-21 06:52:15.000000 odxtools-4.0.4/tests/test_ecu_variant_matching.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2499 2023-01-13 13:17:58.000000 odxtools-4.0.4/tests/test_ecu_variant_patterns.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    10314 2023-06-21 06:52:15.000000 odxtools-4.0.4/tests/test_encoding.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3827 2023-01-27 13:39:15.000000 odxtools-4.0.4/tests/test_odxtools.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1962 2023-01-27 13:39:15.000000 odxtools-4.0.4/tests/test_odxtypes.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1639 2023-01-27 13:39:15.000000 odxtools-4.0.4/tests/test_readparameters.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    17020 2023-06-21 06:52:15.000000 odxtools-4.0.4/tests/test_singleecujob.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)    11866 2023-06-28 12:35:57.000000 odxtools-4.0.4/tests/test_somersault.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)     8220 2023-06-21 06:52:15.000000 odxtools-4.0.4/tests/test_unit_spec.py
--rw-r--r--   0 odxtools  (1002) odxtools  (1002)      745 2023-01-13 13:17:58.000000 odxtools-4.0.4/tests/test_utils.py
+drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-07-11 10:04:37.840000 odxtools-4.0.5/
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1069 2022-03-09 15:55:44.000000 odxtools-4.0.5/LICENSE
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    23581 2023-07-11 10:04:37.836000 odxtools-4.0.5/PKG-INFO
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    22767 2022-12-12 08:24:18.000000 odxtools-4.0.5/README.md
+drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-07-11 10:04:37.795999 odxtools-4.0.5/examples/
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)       65 2023-01-27 13:39:15.000000 odxtools-4.0.5/examples/__init__.py
+-rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)     1686 2023-06-21 06:52:15.000000 odxtools-4.0.5/examples/isotp_send.py
+-rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)      811 2023-01-27 13:39:15.000000 odxtools-4.0.5/examples/mksomersaultpdx.py
+-rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)     1612 2023-01-27 13:39:15.000000 odxtools-4.0.5/examples/pdxcopy.py
+-rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)    81924 2023-07-02 11:28:36.000000 odxtools-4.0.5/examples/somersaultecu.py
+-rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)    19444 2023-01-27 13:39:15.000000 odxtools-4.0.5/examples/somersaultlazy.py
+drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-07-11 10:04:37.815999 odxtools-4.0.5/odxtools/
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2925 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/__init__.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      153 2023-01-13 13:17:58.000000 odxtools-4.0.5/odxtools/__main__.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7853 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/admindata.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4267 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/audience.py
+drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-07-11 10:04:37.820000 odxtools-4.0.5/odxtools/cli/
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      140 2023-01-13 13:17:58.000000 odxtools-4.0.5/odxtools/cli/__init__.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      549 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/cli/_parser_utils.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3287 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/cli/_print_utils.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    14094 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/cli/browse.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1171 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/cli/dummy_sub_parser.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5974 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/cli/find.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7337 2023-07-04 15:58:15.000000 odxtools-4.0.5/odxtools/cli/list.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1809 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/cli/main.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7471 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/cli/snoop.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5302 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/communicationparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     8581 2023-06-28 12:35:57.000000 odxtools-4.0.5/odxtools/companydata.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    11567 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/comparam_subset.py
+drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-07-11 10:04:37.824000 odxtools-4.0.5/odxtools/compumethods/
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      840 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/compumethods/__init__.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      894 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/compumethods/compumethodbase.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      210 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/compumethods/compurationalcoeffs.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1489 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/compumethods/compuscale.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7662 2023-07-02 11:28:36.000000 odxtools-4.0.5/odxtools/compumethods/createanycompumethod.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      843 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/compumethods/identicalcompumethod.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2531 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/compumethods/limit.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     8228 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/compumethods/linearcompumethod.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1692 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/compumethods/scalelinearcompumethod.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     6252 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/compumethods/tabintpcompumethod.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2502 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/compumethods/texttablecompumethod.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5667 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/database.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    15371 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/dataobjectproperty.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      699 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/decodestate.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    27425 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/diagcodedtypes.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     6643 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/diagdatadictionaryspec.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    39660 2023-06-28 12:35:57.000000 odxtools-4.0.5/odxtools/diaglayer.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5957 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/diaglayercontainer.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    11412 2023-07-11 10:04:37.000000 odxtools-4.0.5/odxtools/diaglayerraw.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      908 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/diaglayertype.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     6969 2023-06-28 12:35:57.000000 odxtools-4.0.5/odxtools/ecu_variant_matcher.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3427 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/ecu_variant_patterns.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1190 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/encodestate.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7307 2023-07-07 06:40:10.000000 odxtools-4.0.5/odxtools/endofpdufield.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2429 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/envdata.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5382 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/envdatadesc.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      549 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/exceptions.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1249 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/functionalclass.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      173 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/globals.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    12104 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/isotp_state_machine.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      452 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/load_file.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      310 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/load_odx_d_file.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      334 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/load_pdx_file.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      963 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/message.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    12896 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/multiplexer.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4185 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/nameditemlist.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1209 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/obd.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     8438 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/odxlink.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3469 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/odxtypes.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3467 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/parameter_info.py
+drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-07-11 10:04:37.832000 odxtools-4.0.5/odxtools/parameters/
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      832 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/parameters/__init__.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4330 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/parameters/codedconstparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     9282 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/parameters/createanyparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1566 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/parameters/dynamicparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1387 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/parameters/lengthkeyparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3011 2023-06-28 12:35:57.000000 odxtools-4.0.5/odxtools/parameters/matchingrequestparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4851 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/parameters/nrcconstparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     7208 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/parameters/parameterbase.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4108 2023-06-28 12:35:57.000000 odxtools-4.0.5/odxtools/parameters/parameterwithdop.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3263 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/parameters/physicalconstantparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2787 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/parameters/reservedparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1805 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/parameters/systemparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1090 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/parameters/tableentryparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2484 2023-07-02 11:28:36.000000 odxtools-4.0.5/odxtools/parameters/tablekeyparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1230 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/parameters/tablestructparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3130 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/parameters/valueparameter.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3304 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/parentref.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2372 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/physicaltype.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    13655 2023-06-28 12:35:57.000000 odxtools-4.0.5/odxtools/service.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    16374 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/singleecujob.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5290 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/specialdata.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1234 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/state.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3495 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/statechart.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2553 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/statetransition.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    24316 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/structures.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     8058 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/table.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     4409 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/uds.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    11672 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/units.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1885 2023-01-27 13:39:15.000000 odxtools-4.0.5/odxtools/utils.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)       87 2023-07-11 10:04:37.000000 odxtools-4.0.5/odxtools/version.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     5907 2023-06-21 06:52:15.000000 odxtools-4.0.5/odxtools/write_pdx_file.py
+drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-07-11 10:04:37.815999 odxtools-4.0.5/odxtools.egg-info/
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    23581 2023-07-11 10:04:37.000000 odxtools-4.0.5/odxtools.egg-info/PKG-INFO
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3342 2023-07-11 10:04:37.000000 odxtools-4.0.5/odxtools.egg-info/SOURCES.txt
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)        1 2023-07-11 10:04:37.000000 odxtools-4.0.5/odxtools.egg-info/dependency_links.txt
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)       53 2023-07-11 10:04:37.000000 odxtools-4.0.5/odxtools.egg-info/entry_points.txt
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      100 2023-07-11 10:04:37.000000 odxtools-4.0.5/odxtools.egg-info/requires.txt
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)       18 2023-07-11 10:04:37.000000 odxtools-4.0.5/odxtools.egg-info/top_level.txt
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      382 2023-01-27 13:39:15.000000 odxtools-4.0.5/pyproject.toml
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)       38 2023-07-11 10:04:37.840000 odxtools-4.0.5/setup.cfg
+-rwxr-xr-x   0 odxtools  (1002) odxtools  (1002)     2005 2023-01-27 13:39:15.000000 odxtools-4.0.5/setup.py
+drwxr-xr-x   0 odxtools  (1002) odxtools  (1002)        0 2023-07-11 10:04:37.836000 odxtools-4.0.5/tests/
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    14195 2023-07-02 11:28:36.000000 odxtools-4.0.5/tests/test_compu_methods.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    51695 2023-06-28 12:35:57.000000 odxtools-4.0.5/tests/test_decoding.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    36363 2023-06-21 06:52:15.000000 odxtools-4.0.5/tests/test_diag_coded_types.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     9192 2023-06-21 06:52:15.000000 odxtools-4.0.5/tests/test_diag_data_dictionary_spec.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    14065 2023-06-21 06:52:15.000000 odxtools-4.0.5/tests/test_ecu_variant_matching.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     2499 2023-01-13 13:17:58.000000 odxtools-4.0.5/tests/test_ecu_variant_patterns.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    10314 2023-06-21 06:52:15.000000 odxtools-4.0.5/tests/test_encoding.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     3827 2023-01-27 13:39:15.000000 odxtools-4.0.5/tests/test_odxtools.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1962 2023-01-27 13:39:15.000000 odxtools-4.0.5/tests/test_odxtypes.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     1639 2023-01-27 13:39:15.000000 odxtools-4.0.5/tests/test_readparameters.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    17020 2023-06-21 06:52:15.000000 odxtools-4.0.5/tests/test_singleecujob.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)    11866 2023-06-28 12:35:57.000000 odxtools-4.0.5/tests/test_somersault.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)     8220 2023-06-21 06:52:15.000000 odxtools-4.0.5/tests/test_unit_spec.py
+-rw-r--r--   0 odxtools  (1002) odxtools  (1002)      745 2023-01-13 13:17:58.000000 odxtools-4.0.5/tests/test_utils.py
```

### Comparing `odxtools-4.0.4/LICENSE` & `odxtools-4.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/PKG-INFO` & `odxtools-4.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odxtools
-Version: 4.0.4
+Version: 4.0.5
 Summary: Utilities to work with the automotive diagnostics standard ODX.
 Home-page: https://github.com/Daimler/odxtools
 Author: Katrin Bauer, Andreas Lauser
 Author-email: katrin.b.bauer@mbition.io, andreas.lauser@mbition.io
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Daimler/odxtools/issues
 Keywords: can,can bus,odx,pdx,obd,uds,automotive,diagnostics
```

### Comparing `odxtools-4.0.4/README.md` & `odxtools-4.0.5/README.md`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/examples/isotp_send.py` & `odxtools-4.0.5/examples/isotp_send.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/examples/mksomersaultpdx.py` & `odxtools-4.0.5/examples/mksomersaultpdx.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/examples/pdxcopy.py` & `odxtools-4.0.5/examples/pdxcopy.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/examples/somersaultecu.py` & `odxtools-4.0.5/examples/somersaultecu.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/examples/somersaultlazy.py` & `odxtools-4.0.5/examples/somersaultlazy.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/__init__.py` & `odxtools-4.0.5/odxtools/__init__.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/admindata.py` & `odxtools-4.0.5/odxtools/admindata.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/audience.py` & `odxtools-4.0.5/odxtools/audience.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/cli/_parser_utils.py` & `odxtools-4.0.5/odxtools/cli/_parser_utils.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/cli/_print_utils.py` & `odxtools-4.0.5/odxtools/cli/_print_utils.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/cli/browse.py` & `odxtools-4.0.5/odxtools/cli/browse.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/cli/dummy_sub_parser.py` & `odxtools-4.0.5/odxtools/cli/dummy_sub_parser.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/cli/find.py` & `odxtools-4.0.5/odxtools/cli/find.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/cli/list.py` & `odxtools-4.0.5/odxtools/cli/list.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/cli/main.py` & `odxtools-4.0.5/odxtools/cli/main.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/cli/snoop.py` & `odxtools-4.0.5/odxtools/cli/snoop.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/communicationparameter.py` & `odxtools-4.0.5/odxtools/communicationparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/companydata.py` & `odxtools-4.0.5/odxtools/companydata.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/comparam_subset.py` & `odxtools-4.0.5/odxtools/comparam_subset.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/compumethods/__init__.py` & `odxtools-4.0.5/odxtools/compumethods/__init__.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/compumethods/compumethodbase.py` & `odxtools-4.0.5/odxtools/compumethods/compumethodbase.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/compumethods/compuscale.py` & `odxtools-4.0.5/odxtools/compumethods/compuscale.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/compumethods/createanycompumethod.py` & `odxtools-4.0.5/odxtools/compumethods/createanycompumethod.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/compumethods/identicalcompumethod.py` & `odxtools-4.0.5/odxtools/compumethods/identicalcompumethod.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/compumethods/limit.py` & `odxtools-4.0.5/odxtools/compumethods/limit.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/compumethods/linearcompumethod.py` & `odxtools-4.0.5/odxtools/compumethods/linearcompumethod.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/compumethods/scalelinearcompumethod.py` & `odxtools-4.0.5/odxtools/compumethods/scalelinearcompumethod.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/compumethods/tabintpcompumethod.py` & `odxtools-4.0.5/odxtools/compumethods/tabintpcompumethod.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/compumethods/texttablecompumethod.py` & `odxtools-4.0.5/odxtools/compumethods/texttablecompumethod.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/database.py` & `odxtools-4.0.5/odxtools/database.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/dataobjectproperty.py` & `odxtools-4.0.5/odxtools/dataobjectproperty.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/decodestate.py` & `odxtools-4.0.5/odxtools/decodestate.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/diagcodedtypes.py` & `odxtools-4.0.5/odxtools/diagcodedtypes.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/diagdatadictionaryspec.py` & `odxtools-4.0.5/odxtools/diagdatadictionaryspec.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/diaglayer.py` & `odxtools-4.0.5/odxtools/diaglayer.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/diaglayercontainer.py` & `odxtools-4.0.5/odxtools/diaglayercontainer.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/diaglayerraw.py` & `odxtools-4.0.5/odxtools/diaglayerraw.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,15 @@
         communication_parameters = [
             CommunicationParameterRef.from_et(el, doc_frags, variant_type)
             for el in et_element.iterfind("COMPARAM-REFS/COMPARAM-REF")
         ]
 
         ecu_variant_patterns = [
             EcuVariantPattern.from_et(el, doc_frags)
-            for el in et_element.iterfind("ECU-VARIANT-PATTERN/ECU-VARIANT-PATTERN")
+            for el in et_element.iterfind("ECU-VARIANT-PATTERNS/ECU-VARIANT-PATTERN")
         ]
         if variant_type is not DiagLayerType.ECU_VARIANT:
             assert (
                 len(ecu_variant_patterns) == 0
             ), "DiagLayer of type other than 'ECU-VARIANT' must not define a ECU-VARIANT-PATTERN"
 
         # Create DiagLayer
```

### Comparing `odxtools-4.0.4/odxtools/diaglayertype.py` & `odxtools-4.0.5/odxtools/diaglayertype.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/ecu_variant_matcher.py` & `odxtools-4.0.5/odxtools/ecu_variant_matcher.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/ecu_variant_patterns.py` & `odxtools-4.0.5/odxtools/ecu_variant_patterns.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/encodestate.py` & `odxtools-4.0.5/odxtools/encodestate.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/endofpdufield.py` & `odxtools-4.0.5/odxtools/endofpdufield.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/envdata.py` & `odxtools-4.0.5/odxtools/envdata.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/envdatadesc.py` & `odxtools-4.0.5/odxtools/envdatadesc.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/exceptions.py` & `odxtools-4.0.5/odxtools/exceptions.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/functionalclass.py` & `odxtools-4.0.5/odxtools/functionalclass.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/isotp_state_machine.py` & `odxtools-4.0.5/odxtools/isotp_state_machine.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/message.py` & `odxtools-4.0.5/odxtools/message.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/multiplexer.py` & `odxtools-4.0.5/odxtools/multiplexer.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/nameditemlist.py` & `odxtools-4.0.5/odxtools/nameditemlist.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/obd.py` & `odxtools-4.0.5/odxtools/obd.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/odxlink.py` & `odxtools-4.0.5/odxtools/odxlink.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/odxtypes.py` & `odxtools-4.0.5/odxtools/odxtypes.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/parameter_info.py` & `odxtools-4.0.5/odxtools/parameter_info.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/parameters/__init__.py` & `odxtools-4.0.5/odxtools/parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/parameters/codedconstparameter.py` & `odxtools-4.0.5/odxtools/parameters/codedconstparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/parameters/createanyparameter.py` & `odxtools-4.0.5/odxtools/parameters/createanyparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/parameters/dynamicparameter.py` & `odxtools-4.0.5/odxtools/parameters/dynamicparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/parameters/lengthkeyparameter.py` & `odxtools-4.0.5/odxtools/parameters/lengthkeyparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/parameters/matchingrequestparameter.py` & `odxtools-4.0.5/odxtools/parameters/matchingrequestparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/parameters/nrcconstparameter.py` & `odxtools-4.0.5/odxtools/parameters/nrcconstparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/parameters/parameterbase.py` & `odxtools-4.0.5/odxtools/parameters/parameterbase.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/parameters/parameterwithdop.py` & `odxtools-4.0.5/odxtools/parameters/parameterwithdop.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/parameters/physicalconstantparameter.py` & `odxtools-4.0.5/odxtools/parameters/physicalconstantparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/parameters/reservedparameter.py` & `odxtools-4.0.5/odxtools/parameters/reservedparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/parameters/systemparameter.py` & `odxtools-4.0.5/odxtools/parameters/systemparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/parameters/tableentryparameter.py` & `odxtools-4.0.5/odxtools/parameters/tableentryparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/parameters/tablekeyparameter.py` & `odxtools-4.0.5/odxtools/parameters/tablekeyparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/parameters/tablestructparameter.py` & `odxtools-4.0.5/odxtools/parameters/tablestructparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/parameters/valueparameter.py` & `odxtools-4.0.5/odxtools/parameters/valueparameter.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/parentref.py` & `odxtools-4.0.5/odxtools/parentref.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/physicaltype.py` & `odxtools-4.0.5/odxtools/physicaltype.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/service.py` & `odxtools-4.0.5/odxtools/service.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/singleecujob.py` & `odxtools-4.0.5/odxtools/singleecujob.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/specialdata.py` & `odxtools-4.0.5/odxtools/specialdata.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/state.py` & `odxtools-4.0.5/odxtools/state.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/statechart.py` & `odxtools-4.0.5/odxtools/statechart.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/statetransition.py` & `odxtools-4.0.5/odxtools/statetransition.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/structures.py` & `odxtools-4.0.5/odxtools/structures.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/table.py` & `odxtools-4.0.5/odxtools/table.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/uds.py` & `odxtools-4.0.5/odxtools/uds.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/units.py` & `odxtools-4.0.5/odxtools/units.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/utils.py` & `odxtools-4.0.5/odxtools/utils.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools/write_pdx_file.py` & `odxtools-4.0.5/odxtools/write_pdx_file.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/odxtools.egg-info/PKG-INFO` & `odxtools-4.0.5/odxtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odxtools
-Version: 4.0.4
+Version: 4.0.5
 Summary: Utilities to work with the automotive diagnostics standard ODX.
 Home-page: https://github.com/Daimler/odxtools
 Author: Katrin Bauer, Andreas Lauser
 Author-email: katrin.b.bauer@mbition.io, andreas.lauser@mbition.io
 License: MIT
 Project-URL: Bug Tracker, https://github.com/Daimler/odxtools/issues
 Keywords: can,can bus,odx,pdx,obd,uds,automotive,diagnostics
```

### Comparing `odxtools-4.0.4/odxtools.egg-info/SOURCES.txt` & `odxtools-4.0.5/odxtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/setup.py` & `odxtools-4.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/tests/test_compu_methods.py` & `odxtools-4.0.5/tests/test_compu_methods.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/tests/test_decoding.py` & `odxtools-4.0.5/tests/test_decoding.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/tests/test_diag_coded_types.py` & `odxtools-4.0.5/tests/test_diag_coded_types.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/tests/test_diag_data_dictionary_spec.py` & `odxtools-4.0.5/tests/test_diag_data_dictionary_spec.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/tests/test_ecu_variant_matching.py` & `odxtools-4.0.5/tests/test_ecu_variant_matching.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/tests/test_ecu_variant_patterns.py` & `odxtools-4.0.5/tests/test_ecu_variant_patterns.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/tests/test_encoding.py` & `odxtools-4.0.5/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/tests/test_odxtools.py` & `odxtools-4.0.5/tests/test_odxtools.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/tests/test_odxtypes.py` & `odxtools-4.0.5/tests/test_odxtypes.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/tests/test_readparameters.py` & `odxtools-4.0.5/tests/test_readparameters.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/tests/test_singleecujob.py` & `odxtools-4.0.5/tests/test_singleecujob.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/tests/test_somersault.py` & `odxtools-4.0.5/tests/test_somersault.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/tests/test_unit_spec.py` & `odxtools-4.0.5/tests/test_unit_spec.py`

 * *Files identical despite different names*

### Comparing `odxtools-4.0.4/tests/test_utils.py` & `odxtools-4.0.5/tests/test_utils.py`

 * *Files identical despite different names*

