# Comparing `tmp/hdl21-3.0.dev3.tar.gz` & `tmp/hdl21-4.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdl21-3.0.dev3.tar", last modified: Tue Jan 17 23:17:33 2023, max compression
+gzip compressed data, was "hdl21-4.0.0rc0.tar", last modified: Tue Jul 11 16:53:02 2023, max compression
```

## Comparing `hdl21-3.0.dev3.tar` & `hdl21-4.0.0rc0.tar`

### file list

```diff
@@ -1,135 +1,139 @@
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:33.540001 hdl21-3.0.dev3/
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:33.511565 hdl21-3.0.dev3/.github/
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:33.515461 hdl21-3.0.dev3/.github/workflows/
--rw-r--r--   0 dan        (501) staff       (20)     1877 2022-12-15 01:51:40.000000 hdl21-3.0.dev3/.github/workflows/test.yaml
--rw-r--r--   0 dan        (501) staff       (20)     2541 2022-05-03 17:59:57.000000 hdl21-3.0.dev3/.gitignore
--rw-r--r--   0 dan        (501) staff       (20)      129 2023-01-09 00:49:23.000000 hdl21-3.0.dev3/.pre-commit-config.yaml
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:33.515845 hdl21-3.0.dev3/.vscode/
--rw-r--r--   0 dan        (501) staff       (20)      233 2021-08-24 00:04:32.000000 hdl21-3.0.dev3/.vscode/settings.json
--rw-r--r--   0 dan        (501) staff       (20)      513 2021-04-16 16:11:28.000000 hdl21-3.0.dev3/Cargo.toml
--rw-r--r--   0 dan        (501) staff       (20)     1521 2021-04-16 16:18:38.000000 hdl21-3.0.dev3/LICENSE
--rw-r--r--   0 dan        (501) staff       (20)    41620 2023-01-17 23:17:33.539662 hdl21-3.0.dev3/PKG-INFO
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:33.516543 hdl21-3.0.dev3/SampleSitePdks/
--rw-r--r--   0 dan        (501) staff       (20)     1121 2022-06-13 20:52:07.000000 hdl21-3.0.dev3/SampleSitePdks/readme.md
--rw-r--r--   0 dan        (501) staff       (20)      987 2023-01-17 23:14:01.000000 hdl21-3.0.dev3/SampleSitePdks/setup.py
--rw-r--r--   0 dan        (501) staff       (20)     1174 2022-08-12 23:32:38.000000 hdl21-3.0.dev3/SampleSitePdks/sitepdks.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:33.518348 hdl21-3.0.dev3/examples/
--rw-r--r--   0 dan        (501) staff       (20)      634 2022-11-29 06:32:17.000000 hdl21-3.0.dev3/examples/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)     4494 2022-11-29 06:32:17.000000 hdl21-3.0.dev3/examples/encoder.py
--rw-r--r--   0 dan        (501) staff       (20)     1415 2022-12-15 00:46:13.000000 hdl21-3.0.dev3/examples/mos_iv_sim.py
--rw-r--r--   0 dan        (501) staff       (20)     7408 2022-12-01 18:46:32.000000 hdl21-3.0.dev3/examples/rdac.py
--rw-r--r--   0 dan        (501) staff       (20)     3768 2022-11-29 06:32:17.000000 hdl21-3.0.dev3/examples/ro.py
--rw-r--r--   0 dan        (501) staff       (20)      516 2022-12-15 00:46:13.000000 hdl21-3.0.dev3/examples/test_examples.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:33.524305 hdl21-3.0.dev3/hdl21/
--rw-r--r--   0 dan        (501) staff       (20)     1391 2022-12-15 01:51:40.000000 hdl21-3.0.dev3/hdl21/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)     2077 2023-01-09 00:49:33.000000 hdl21-3.0.dev3/hdl21/attrmagic.py
--rw-r--r--   0 dan        (501) staff       (20)    13154 2022-11-01 16:11:00.000000 hdl21-3.0.dev3/hdl21/bundle.py
--rw-r--r--   0 dan        (501) staff       (20)     2400 2022-11-01 16:11:00.000000 hdl21-3.0.dev3/hdl21/call.py
--rw-r--r--   0 dan        (501) staff       (20)     1529 2022-11-01 16:11:00.000000 hdl21-3.0.dev3/hdl21/concat.py
--rw-r--r--   0 dan        (501) staff       (20)      566 2023-01-09 00:49:33.000000 hdl21-3.0.dev3/hdl21/concatable.py
--rw-r--r--   0 dan        (501) staff       (20)      773 2023-01-09 00:49:33.000000 hdl21-3.0.dev3/hdl21/connect.py
--rw-r--r--   0 dan        (501) staff       (20)     1688 2023-01-09 00:49:33.000000 hdl21-3.0.dev3/hdl21/datatype.py
--rw-r--r--   0 dan        (501) staff       (20)      572 2022-11-01 00:28:38.000000 hdl21-3.0.dev3/hdl21/default.py
--rw-r--r--   0 dan        (501) staff       (20)     1584 2022-08-12 23:32:38.000000 hdl21-3.0.dev3/hdl21/diff_pair.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:33.526699 hdl21-3.0.dev3/hdl21/elab/
--rw-r--r--   0 dan        (501) staff       (20)      159 2022-11-26 00:08:30.000000 hdl21-3.0.dev3/hdl21/elab/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)     3450 2022-11-01 16:11:00.000000 hdl21-3.0.dev3/hdl21/elab/context.py
--rw-r--r--   0 dan        (501) staff       (20)     1626 2023-01-09 00:49:33.000000 hdl21-3.0.dev3/hdl21/elab/elab.py
--rw-r--r--   0 dan        (501) staff       (20)      481 2022-11-01 16:11:00.000000 hdl21-3.0.dev3/hdl21/elab/elaboratable.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:33.530014 hdl21-3.0.dev3/hdl21/elab/elaborators/
--rw-r--r--   0 dan        (501) staff       (20)      465 2022-12-15 00:46:13.000000 hdl21-3.0.dev3/hdl21/elab/elaborators/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)     4003 2022-10-17 20:35:07.000000 hdl21-3.0.dev3/hdl21/elab/elaborators/arrays.py
--rw-r--r--   0 dan        (501) staff       (20)     9479 2022-12-15 00:46:13.000000 hdl21-3.0.dev3/hdl21/elab/elaborators/base.py
--rw-r--r--   0 dan        (501) staff       (20)     9281 2023-01-09 00:49:30.000000 hdl21-3.0.dev3/hdl21/elab/elaborators/conntypes.py
--rw-r--r--   0 dan        (501) staff       (20)    16872 2023-01-09 00:49:23.000000 hdl21-3.0.dev3/hdl21/elab/elaborators/flatten_bundles.py
--rw-r--r--   0 dan        (501) staff       (20)     5934 2023-01-09 00:49:23.000000 hdl21-3.0.dev3/hdl21/elab/elaborators/generators.py
--rw-r--r--   0 dan        (501) staff       (20)     3465 2022-08-12 23:32:38.000000 hdl21-3.0.dev3/hdl21/elab/elaborators/inst_bundles.py
--rw-r--r--   0 dan        (501) staff       (20)      427 2022-12-15 00:46:13.000000 hdl21-3.0.dev3/hdl21/elab/elaborators/mark_modules.py
--rw-r--r--   0 dan        (501) staff       (20)     4955 2022-08-12 23:32:38.000000 hdl21-3.0.dev3/hdl21/elab/elaborators/orphanage.py
--rw-r--r--   0 dan        (501) staff       (20)    13331 2023-01-09 00:49:30.000000 hdl21-3.0.dev3/hdl21/elab/elaborators/portrefs.py
--rw-r--r--   0 dan        (501) staff       (20)     3739 2022-10-17 20:35:07.000000 hdl21-3.0.dev3/hdl21/elab/elaborators/resolve_ref_types.py
--rw-r--r--   0 dan        (501) staff       (20)     7338 2022-08-12 23:32:38.000000 hdl21-3.0.dev3/hdl21/elab/elaborators/slices.py
--rw-r--r--   0 dan        (501) staff       (20)     2961 2022-10-17 20:35:07.000000 hdl21-3.0.dev3/hdl21/elab/elaborators/width.py
--rw-r--r--   0 dan        (501) staff       (20)     1427 2022-12-15 00:46:13.000000 hdl21-3.0.dev3/hdl21/elab/elabpass.py
--rw-r--r--   0 dan        (501) staff       (20)     3784 2022-11-01 16:11:00.000000 hdl21-3.0.dev3/hdl21/external_module.py
--rw-r--r--   0 dan        (501) staff       (20)     5178 2023-01-09 00:49:23.000000 hdl21-3.0.dev3/hdl21/generator.py
--rw-r--r--   0 dan        (501) staff       (20)     6676 2023-01-17 23:14:01.000000 hdl21-3.0.dev3/hdl21/generators.py
--rw-r--r--   0 dan        (501) staff       (20)    12899 2023-01-09 00:49:33.000000 hdl21-3.0.dev3/hdl21/instance.py
--rw-r--r--   0 dan        (501) staff       (20)     1859 2023-01-17 23:14:01.000000 hdl21-3.0.dev3/hdl21/instantiable.py
--rw-r--r--   0 dan        (501) staff       (20)      336 2022-12-15 01:51:40.000000 hdl21-3.0.dev3/hdl21/literal.py
--rw-r--r--   0 dan        (501) staff       (20)    14637 2023-01-09 00:49:23.000000 hdl21-3.0.dev3/hdl21/module.py
--rw-r--r--   0 dan        (501) staff       (20)     1312 2022-08-12 23:32:38.000000 hdl21-3.0.dev3/hdl21/netlist.py
--rw-r--r--   0 dan        (501) staff       (20)     1273 2022-11-01 16:11:00.000000 hdl21-3.0.dev3/hdl21/noconn.py
--rw-r--r--   0 dan        (501) staff       (20)      191 2023-01-09 00:49:23.000000 hdl21-3.0.dev3/hdl21/one_or_more.py
--rw-r--r--   0 dan        (501) staff       (20)     8981 2022-10-27 22:36:09.000000 hdl21-3.0.dev3/hdl21/params.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:33.531080 hdl21-3.0.dev3/hdl21/pdk/
--rw-r--r--   0 dan        (501) staff       (20)       83 2023-01-09 00:49:23.000000 hdl21-3.0.dev3/hdl21/pdk/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)     1649 2022-08-12 23:32:38.000000 hdl21-3.0.dev3/hdl21/pdk/corner.py
--rw-r--r--   0 dan        (501) staff       (20)     3224 2022-11-04 21:00:31.000000 hdl21-3.0.dev3/hdl21/pdk/installation.py
--rw-r--r--   0 dan        (501) staff       (20)     6198 2023-01-09 00:49:23.000000 hdl21-3.0.dev3/hdl21/pdk/pdk.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:33.531790 hdl21-3.0.dev3/hdl21/pdk/sample_pdk/
--rw-r--r--   0 dan        (501) staff       (20)      861 2022-12-15 00:46:13.000000 hdl21-3.0.dev3/hdl21/pdk/sample_pdk/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)     3501 2022-12-15 00:46:13.000000 hdl21-3.0.dev3/hdl21/pdk/sample_pdk/pdk.py
--rw-r--r--   0 dan        (501) staff       (20)     1470 2022-12-15 00:46:13.000000 hdl21-3.0.dev3/hdl21/pdk/sample_pdk/test_sample_pdk.py
--rw-r--r--   0 dan        (501) staff       (20)      703 2022-08-12 23:32:38.000000 hdl21-3.0.dev3/hdl21/pdk/test_pdk.py
--rw-r--r--   0 dan        (501) staff       (20)     1296 2022-11-01 16:11:00.000000 hdl21-3.0.dev3/hdl21/portref.py
--rw-r--r--   0 dan        (501) staff       (20)    15760 2023-01-09 00:49:23.000000 hdl21-3.0.dev3/hdl21/prefix.py
--rw-r--r--   0 dan        (501) staff       (20)    21241 2022-12-15 01:51:40.000000 hdl21-3.0.dev3/hdl21/primitives.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:33.532588 hdl21-3.0.dev3/hdl21/proto/
--rw-r--r--   0 dan        (501) staff       (20)      213 2022-05-03 17:59:57.000000 hdl21-3.0.dev3/hdl21/proto/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)    15224 2022-12-15 01:51:40.000000 hdl21-3.0.dev3/hdl21/proto/from_proto.py
--rw-r--r--   0 dan        (501) staff       (20)    17838 2023-01-09 00:49:23.000000 hdl21-3.0.dev3/hdl21/proto/to_proto.py
--rw-r--r--   0 dan        (501) staff       (20)     2127 2023-01-09 00:49:33.000000 hdl21-3.0.dev3/hdl21/qualname.py
--rw-r--r--   0 dan        (501) staff       (20)     6043 2023-01-09 00:49:23.000000 hdl21-3.0.dev3/hdl21/scalar.py
--rw-r--r--   0 dan        (501) staff       (20)     6357 2022-11-29 06:32:17.000000 hdl21-3.0.dev3/hdl21/signal.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:33.533657 hdl21-3.0.dev3/hdl21/sim/
--rw-r--r--   0 dan        (501) staff       (20)       72 2022-06-13 20:51:56.000000 hdl21-3.0.dev3/hdl21/sim/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)    14337 2023-01-09 00:49:23.000000 hdl21-3.0.dev3/hdl21/sim/data.py
--rw-r--r--   0 dan        (501) staff       (20)     8328 2022-10-17 22:32:24.000000 hdl21-3.0.dev3/hdl21/sim/delay.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:33.533904 hdl21-3.0.dev3/hdl21/sim/tests/
--rw-r--r--   0 dan        (501) staff       (20)     8874 2022-12-15 01:51:40.000000 hdl21-3.0.dev3/hdl21/sim/tests/test_sim.py
--rw-r--r--   0 dan        (501) staff       (20)    13788 2023-01-09 00:49:23.000000 hdl21-3.0.dev3/hdl21/sim/to_proto.py
--rw-r--r--   0 dan        (501) staff       (20)     5347 2022-11-04 21:00:31.000000 hdl21-3.0.dev3/hdl21/slice.py
--rw-r--r--   0 dan        (501) staff       (20)     2123 2023-01-09 00:49:33.000000 hdl21-3.0.dev3/hdl21/sliceable.py
--rw-r--r--   0 dan        (501) staff       (20)     3844 2022-11-01 16:11:00.000000 hdl21-3.0.dev3/hdl21/source_info.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:33.537281 hdl21-3.0.dev3/hdl21/tests/
--rw-r--r--   0 dan        (501) staff       (20)        0 2021-04-16 16:15:12.000000 hdl21-3.0.dev3/hdl21/tests/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)     1091 2022-11-26 00:08:30.000000 hdl21-3.0.dev3/hdl21/tests/content.py
--rw-r--r--   0 dan        (501) staff       (20)     3134 2023-01-09 00:49:23.000000 hdl21-3.0.dev3/hdl21/tests/test_builtin_generators.py
--rw-r--r--   0 dan        (501) staff       (20)    19347 2023-01-09 00:49:30.000000 hdl21-3.0.dev3/hdl21/tests/test_bundles.py
--rw-r--r--   0 dan        (501) staff       (20)     5491 2022-10-17 20:35:07.000000 hdl21-3.0.dev3/hdl21/tests/test_conns.py
--rw-r--r--   0 dan        (501) staff       (20)     5505 2022-11-04 21:00:31.000000 hdl21-3.0.dev3/hdl21/tests/test_doc_examples.py
--rw-r--r--   0 dan        (501) staff       (20)    15250 2022-11-26 00:08:30.000000 hdl21-3.0.dev3/hdl21/tests/test_exports.py
--rw-r--r--   0 dan        (501) staff       (20)    33801 2023-01-09 00:53:34.000000 hdl21-3.0.dev3/hdl21/tests/test_hdl21.py
--rw-r--r--   0 dan        (501) staff       (20)     5349 2022-08-12 23:32:38.000000 hdl21-3.0.dev3/hdl21/tests/test_params.py
--rw-r--r--   0 dan        (501) staff       (20)    13267 2022-12-15 01:51:40.000000 hdl21-3.0.dev3/hdl21/tests/test_prefix.py
--rw-r--r--   0 dan        (501) staff       (20)      741 2022-10-17 20:35:07.000000 hdl21-3.0.dev3/hdl21/tests/test_source_info.py
--rw-r--r--   0 dan        (501) staff       (20)     4122 2022-11-26 00:08:30.000000 hdl21-3.0.dev3/hdl21/walker.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:33.525682 hdl21-3.0.dev3/hdl21.egg-info/
--rw-r--r--   0 dan        (501) staff       (20)    41620 2023-01-17 23:17:33.000000 hdl21-3.0.dev3/hdl21.egg-info/PKG-INFO
--rw-r--r--   0 dan        (501) staff       (20)     2564 2023-01-17 23:17:33.000000 hdl21-3.0.dev3/hdl21.egg-info/SOURCES.txt
--rw-r--r--   0 dan        (501) staff       (20)        1 2023-01-17 23:17:33.000000 hdl21-3.0.dev3/hdl21.egg-info/dependency_links.txt
--rw-r--r--   0 dan        (501) staff       (20)      127 2023-01-17 23:17:33.000000 hdl21-3.0.dev3/hdl21.egg-info/requires.txt
--rw-r--r--   0 dan        (501) staff       (20)       15 2023-01-17 23:17:33.000000 hdl21-3.0.dev3/hdl21.egg-info/top_level.txt
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:33.537457 hdl21-3.0.dev3/pdks/
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:33.537834 hdl21-3.0.dev3/pdks/Asap7/
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:33.537960 hdl21-3.0.dev3/pdks/Asap7/asap7/
--rw-r--r--   0 dan        (501) staff       (20)      315 2022-11-26 00:08:30.000000 hdl21-3.0.dev3/pdks/Asap7/asap7/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)        0 2022-05-03 17:59:57.000000 hdl21-3.0.dev3/pdks/Asap7/readme.md
--rw-r--r--   0 dan        (501) staff       (20)      895 2023-01-17 23:14:01.000000 hdl21-3.0.dev3/pdks/Asap7/setup.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:33.538201 hdl21-3.0.dev3/pdks/Sky130/
--rw-r--r--   0 dan        (501) staff       (20)        0 2022-05-03 17:59:57.000000 hdl21-3.0.dev3/pdks/Sky130/readme.md
--rw-r--r--   0 dan        (501) staff       (20)      905 2023-01-17 23:14:01.000000 hdl21-3.0.dev3/pdks/Sky130/setup.py
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:33.538326 hdl21-3.0.dev3/pdks/Sky130/sky130/
--rw-r--r--   0 dan        (501) staff       (20)      315 2022-11-26 00:08:30.000000 hdl21-3.0.dev3/pdks/Sky130/sky130/__init__.py
--rw-r--r--   0 dan        (501) staff       (20)      541 2022-06-13 20:51:56.000000 hdl21-3.0.dev3/pdks/readme.md
--rw-r--r--   0 dan        (501) staff       (20)    41320 2022-12-15 00:46:13.000000 hdl21-3.0.dev3/readme.md
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:33.538481 hdl21-3.0.dev3/scratch/
--rw-r--r--   0 dan        (501) staff       (20)        0 2021-09-08 00:13:15.000000 hdl21-3.0.dev3/scratch/empty
-drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-01-17 23:17:33.539212 hdl21-3.0.dev3/scripts/
--rw-r--r--   0 dan        (501) staff       (20)        0 2022-10-27 22:36:09.000000 hdl21-3.0.dev3/scripts/empty
--rwxr-xr-x   0 dan        (501) staff       (20)      263 2022-10-27 22:36:09.000000 hdl21-3.0.dev3/scripts/install-dev.sh
--rwxr-xr-x   0 dan        (501) staff       (20)      158 2022-12-15 01:51:40.000000 hdl21-3.0.dev3/scripts/install-pypi.sh
--rw-r--r--   0 dan        (501) staff       (20)     2357 2022-10-27 22:36:09.000000 hdl21-3.0.dev3/scripts/primtable.py
--rw-r--r--   0 dan        (501) staff       (20)       38 2023-01-17 23:17:33.540072 hdl21-3.0.dev3/setup.cfg
--rw-r--r--   0 dan        (501) staff       (20)     1139 2023-01-17 23:14:01.000000 hdl21-3.0.dev3/setup.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:53:02.183929 hdl21-4.0.0rc0/
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:53:02.144698 hdl21-4.0.0rc0/.github/
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:53:02.148916 hdl21-4.0.0rc0/.github/workflows/
+-rw-r--r--   0 dan        (501) staff       (20)     3458 2023-07-11 14:50:48.000000 hdl21-4.0.0rc0/.github/workflows/test.yaml
+-rw-r--r--   0 dan        (501) staff       (20)     2559 2023-06-07 23:06:22.000000 hdl21-4.0.0rc0/.gitignore
+-rw-r--r--   0 dan        (501) staff       (20)      164 2023-03-17 23:05:04.000000 hdl21-4.0.0rc0/.pre-commit-config.yaml
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:53:02.149430 hdl21-4.0.0rc0/.vscode/
+-rw-r--r--   0 dan        (501) staff       (20)      280 2023-06-07 23:06:22.000000 hdl21-4.0.0rc0/.vscode/settings.json
+-rw-r--r--   0 dan        (501) staff       (20)      513 2021-04-16 16:11:28.000000 hdl21-4.0.0rc0/Cargo.toml
+-rw-r--r--   0 dan        (501) staff       (20)     1521 2021-04-16 16:18:38.000000 hdl21-4.0.0rc0/LICENSE
+-rw-r--r--   0 dan        (501) staff       (20)    52019 2023-07-11 16:53:02.183669 hdl21-4.0.0rc0/PKG-INFO
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:53:02.150460 hdl21-4.0.0rc0/SampleSitePdks/
+-rw-r--r--   0 dan        (501) staff       (20)     1121 2022-06-13 20:52:07.000000 hdl21-4.0.0rc0/SampleSitePdks/readme.md
+-rw-r--r--   0 dan        (501) staff       (20)      984 2023-07-11 16:31:14.000000 hdl21-4.0.0rc0/SampleSitePdks/setup.py
+-rw-r--r--   0 dan        (501) staff       (20)     1521 2023-07-11 14:50:48.000000 hdl21-4.0.0rc0/SampleSitePdks/sitepdks.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:53:02.153753 hdl21-4.0.0rc0/examples/
+-rw-r--r--   0 dan        (501) staff       (20)      634 2022-11-29 06:32:17.000000 hdl21-4.0.0rc0/examples/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)     2310 2023-07-11 16:27:41.000000 hdl21-4.0.0rc0/examples/bundles.py
+-rw-r--r--   0 dan        (501) staff       (20)     2675 2023-06-23 19:51:39.000000 hdl21-4.0.0rc0/examples/diff_ota.py
+-rw-r--r--   0 dan        (501) staff       (20)     4494 2022-11-29 06:32:17.000000 hdl21-4.0.0rc0/examples/encoder.py
+-rw-r--r--   0 dan        (501) staff       (20)     3596 2023-06-26 21:03:45.000000 hdl21-4.0.0rc0/examples/idac.py
+-rw-r--r--   0 dan        (501) staff       (20)     1727 2023-06-23 19:51:39.000000 hdl21-4.0.0rc0/examples/mos_sim.py
+-rw-r--r--   0 dan        (501) staff       (20)     7408 2022-12-01 18:46:32.000000 hdl21-4.0.0rc0/examples/rdac.py
+-rw-r--r--   0 dan        (501) staff       (20)     3768 2022-11-29 06:32:17.000000 hdl21-4.0.0rc0/examples/ro.py
+-rw-r--r--   0 dan        (501) staff       (20)      566 2023-07-11 16:27:41.000000 hdl21-4.0.0rc0/examples/test_examples.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:53:02.164476 hdl21-4.0.0rc0/hdl21/
+-rw-r--r--   0 dan        (501) staff       (20)     1640 2023-07-11 16:47:02.000000 hdl21-4.0.0rc0/hdl21/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)     4721 2023-06-26 21:03:45.000000 hdl21-4.0.0rc0/hdl21/attrmagic.py
+-rw-r--r--   0 dan        (501) staff       (20)    19042 2023-06-26 21:03:45.000000 hdl21-4.0.0rc0/hdl21/bundle.py
+-rw-r--r--   0 dan        (501) staff       (20)     2400 2022-11-01 16:11:00.000000 hdl21-4.0.0rc0/hdl21/call.py
+-rw-r--r--   0 dan        (501) staff       (20)     1654 2023-06-26 21:03:45.000000 hdl21-4.0.0rc0/hdl21/concat.py
+-rw-r--r--   0 dan        (501) staff       (20)      566 2023-01-09 00:49:33.000000 hdl21-4.0.0rc0/hdl21/concatable.py
+-rw-r--r--   0 dan        (501) staff       (20)      773 2023-01-09 00:49:33.000000 hdl21-4.0.0rc0/hdl21/connect.py
+-rw-r--r--   0 dan        (501) staff       (20)     1807 2023-06-26 21:03:45.000000 hdl21-4.0.0rc0/hdl21/datatype.py
+-rw-r--r--   0 dan        (501) staff       (20)      538 2023-06-26 21:03:45.000000 hdl21-4.0.0rc0/hdl21/default.py
+-rw-r--r--   0 dan        (501) staff       (20)     1674 2023-06-23 17:09:45.000000 hdl21-4.0.0rc0/hdl21/diff_pair.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:53:02.166859 hdl21-4.0.0rc0/hdl21/elab/
+-rw-r--r--   0 dan        (501) staff       (20)      159 2022-11-26 00:08:30.000000 hdl21-4.0.0rc0/hdl21/elab/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)     3450 2022-11-01 16:11:00.000000 hdl21-4.0.0rc0/hdl21/elab/context.py
+-rw-r--r--   0 dan        (501) staff       (20)     1626 2023-01-09 00:49:33.000000 hdl21-4.0.0rc0/hdl21/elab/elab.py
+-rw-r--r--   0 dan        (501) staff       (20)      481 2022-11-01 16:11:00.000000 hdl21-4.0.0rc0/hdl21/elab/elaboratable.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:53:02.171814 hdl21-4.0.0rc0/hdl21/elab/elaborators/
+-rw-r--r--   0 dan        (501) staff       (20)      465 2022-12-15 00:46:13.000000 hdl21-4.0.0rc0/hdl21/elab/elaborators/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)     4003 2022-10-17 20:35:07.000000 hdl21-4.0.0rc0/hdl21/elab/elaborators/arrays.py
+-rw-r--r--   0 dan        (501) staff       (20)     9433 2023-06-09 23:37:53.000000 hdl21-4.0.0rc0/hdl21/elab/elaborators/base.py
+-rw-r--r--   0 dan        (501) staff       (20)     9281 2023-01-09 00:49:30.000000 hdl21-4.0.0rc0/hdl21/elab/elaborators/conntypes.py
+-rw-r--r--   0 dan        (501) staff       (20)    18422 2023-03-17 23:05:04.000000 hdl21-4.0.0rc0/hdl21/elab/elaborators/flatten_bundles.py
+-rw-r--r--   0 dan        (501) staff       (20)     6025 2023-02-17 18:07:59.000000 hdl21-4.0.0rc0/hdl21/elab/elaborators/generators.py
+-rw-r--r--   0 dan        (501) staff       (20)     3465 2022-08-12 23:32:38.000000 hdl21-4.0.0rc0/hdl21/elab/elaborators/inst_bundles.py
+-rw-r--r--   0 dan        (501) staff       (20)      593 2023-06-09 23:37:53.000000 hdl21-4.0.0rc0/hdl21/elab/elaborators/mark_modules.py
+-rw-r--r--   0 dan        (501) staff       (20)     4955 2022-08-12 23:32:38.000000 hdl21-4.0.0rc0/hdl21/elab/elaborators/orphanage.py
+-rw-r--r--   0 dan        (501) staff       (20)    13331 2023-01-09 00:49:30.000000 hdl21-4.0.0rc0/hdl21/elab/elaborators/portrefs.py
+-rw-r--r--   0 dan        (501) staff       (20)     3739 2022-10-17 20:35:07.000000 hdl21-4.0.0rc0/hdl21/elab/elaborators/resolve_ref_types.py
+-rw-r--r--   0 dan        (501) staff       (20)     7338 2022-08-12 23:32:38.000000 hdl21-4.0.0rc0/hdl21/elab/elaborators/slices.py
+-rw-r--r--   0 dan        (501) staff       (20)     2961 2022-10-17 20:35:07.000000 hdl21-4.0.0rc0/hdl21/elab/elaborators/width.py
+-rw-r--r--   0 dan        (501) staff       (20)     1427 2022-12-15 00:46:13.000000 hdl21-4.0.0rc0/hdl21/elab/elabpass.py
+-rw-r--r--   0 dan        (501) staff       (20)     4662 2023-06-26 21:03:45.000000 hdl21-4.0.0rc0/hdl21/external_module.py
+-rw-r--r--   0 dan        (501) staff       (20)     4867 2023-03-17 23:05:04.000000 hdl21-4.0.0rc0/hdl21/generator.py
+-rw-r--r--   0 dan        (501) staff       (20)     6706 2023-06-23 19:51:39.000000 hdl21-4.0.0rc0/hdl21/generators.py
+-rw-r--r--   0 dan        (501) staff       (20)    12976 2023-03-17 23:05:04.000000 hdl21-4.0.0rc0/hdl21/instance.py
+-rw-r--r--   0 dan        (501) staff       (20)     1893 2023-07-11 16:27:41.000000 hdl21-4.0.0rc0/hdl21/instantiable.py
+-rw-r--r--   0 dan        (501) staff       (20)      294 2023-06-26 21:03:45.000000 hdl21-4.0.0rc0/hdl21/literal.py
+-rw-r--r--   0 dan        (501) staff       (20)    15194 2023-06-26 21:03:45.000000 hdl21-4.0.0rc0/hdl21/module.py
+-rw-r--r--   0 dan        (501) staff       (20)     1312 2022-08-12 23:32:38.000000 hdl21-4.0.0rc0/hdl21/netlist.py
+-rw-r--r--   0 dan        (501) staff       (20)     1273 2022-11-01 16:11:00.000000 hdl21-4.0.0rc0/hdl21/noconn.py
+-rw-r--r--   0 dan        (501) staff       (20)      191 2023-01-09 00:49:23.000000 hdl21-4.0.0rc0/hdl21/one_or_more.py
+-rw-r--r--   0 dan        (501) staff       (20)    11280 2023-06-26 21:03:45.000000 hdl21-4.0.0rc0/hdl21/params.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:53:02.173650 hdl21-4.0.0rc0/hdl21/pdk/
+-rw-r--r--   0 dan        (501) staff       (20)       83 2023-06-09 23:37:53.000000 hdl21-4.0.0rc0/hdl21/pdk/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)     1649 2022-08-12 23:32:38.000000 hdl21-4.0.0rc0/hdl21/pdk/corner.py
+-rw-r--r--   0 dan        (501) staff       (20)     3224 2022-11-04 21:00:31.000000 hdl21-4.0.0rc0/hdl21/pdk/installation.py
+-rw-r--r--   0 dan        (501) staff       (20)     6198 2023-01-09 00:49:23.000000 hdl21-4.0.0rc0/hdl21/pdk/pdk.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:53:02.174715 hdl21-4.0.0rc0/hdl21/pdk/sample_pdk/
+-rw-r--r--   0 dan        (501) staff       (20)      861 2022-12-15 00:46:13.000000 hdl21-4.0.0rc0/hdl21/pdk/sample_pdk/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)     5318 2023-06-23 19:51:39.000000 hdl21-4.0.0rc0/hdl21/pdk/sample_pdk/pdk.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:53:02.175017 hdl21-4.0.0rc0/hdl21/pdk/sample_pdk/resources/
+-rw-r--r--   0 dan        (501) staff       (20)      639 2023-06-23 19:51:39.000000 hdl21-4.0.0rc0/hdl21/pdk/sample_pdk/resources/models.sp
+-rw-r--r--   0 dan        (501) staff       (20)     1470 2022-12-15 00:46:13.000000 hdl21-4.0.0rc0/hdl21/pdk/sample_pdk/test_sample_pdk.py
+-rw-r--r--   0 dan        (501) staff       (20)      703 2022-08-12 23:32:38.000000 hdl21-4.0.0rc0/hdl21/pdk/test_pdk.py
+-rw-r--r--   0 dan        (501) staff       (20)     1296 2022-11-01 16:11:00.000000 hdl21-4.0.0rc0/hdl21/portref.py
+-rw-r--r--   0 dan        (501) staff       (20)    16266 2023-07-11 16:27:41.000000 hdl21-4.0.0rc0/hdl21/prefix.py
+-rw-r--r--   0 dan        (501) staff       (20)    23597 2023-06-26 21:03:45.000000 hdl21-4.0.0rc0/hdl21/primitives.py
+-rw-r--r--   0 dan        (501) staff       (20)     2300 2023-03-17 23:05:04.000000 hdl21-4.0.0rc0/hdl21/props.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:53:02.176006 hdl21-4.0.0rc0/hdl21/proto/
+-rw-r--r--   0 dan        (501) staff       (20)      213 2022-05-03 17:59:57.000000 hdl21-4.0.0rc0/hdl21/proto/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)    15343 2023-07-11 16:27:41.000000 hdl21-4.0.0rc0/hdl21/proto/from_proto.py
+-rw-r--r--   0 dan        (501) staff       (20)    18032 2023-07-11 16:27:41.000000 hdl21-4.0.0rc0/hdl21/proto/to_proto.py
+-rw-r--r--   0 dan        (501) staff       (20)     1711 2023-07-11 16:27:41.000000 hdl21-4.0.0rc0/hdl21/qualname.py
+-rw-r--r--   0 dan        (501) staff       (20)     2442 2023-07-11 16:27:41.000000 hdl21-4.0.0rc0/hdl21/role.py
+-rw-r--r--   0 dan        (501) staff       (20)     4043 2023-06-26 21:03:45.000000 hdl21-4.0.0rc0/hdl21/scalar.py
+-rw-r--r--   0 dan        (501) staff       (20)     8544 2023-03-17 23:05:04.000000 hdl21-4.0.0rc0/hdl21/signal.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:53:02.177263 hdl21-4.0.0rc0/hdl21/sim/
+-rw-r--r--   0 dan        (501) staff       (20)       72 2022-06-13 20:51:56.000000 hdl21-4.0.0rc0/hdl21/sim/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)    15154 2023-06-25 17:33:23.000000 hdl21-4.0.0rc0/hdl21/sim/data.py
+-rw-r--r--   0 dan        (501) staff       (20)     8328 2022-10-17 22:32:24.000000 hdl21-4.0.0rc0/hdl21/sim/delay.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:53:02.177640 hdl21-4.0.0rc0/hdl21/sim/tests/
+-rw-r--r--   0 dan        (501) staff       (20)     9850 2023-06-26 21:03:45.000000 hdl21-4.0.0rc0/hdl21/sim/tests/test_sim.py
+-rw-r--r--   0 dan        (501) staff       (20)    13689 2023-06-26 21:03:45.000000 hdl21-4.0.0rc0/hdl21/sim/to_proto.py
+-rw-r--r--   0 dan        (501) staff       (20)     5339 2023-03-17 23:05:04.000000 hdl21-4.0.0rc0/hdl21/slice.py
+-rw-r--r--   0 dan        (501) staff       (20)     2123 2023-01-09 00:49:33.000000 hdl21-4.0.0rc0/hdl21/sliceable.py
+-rw-r--r--   0 dan        (501) staff       (20)     3844 2022-11-01 16:11:00.000000 hdl21-4.0.0rc0/hdl21/source_info.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:53:02.180513 hdl21-4.0.0rc0/hdl21/tests/
+-rw-r--r--   0 dan        (501) staff       (20)        0 2021-04-16 16:15:12.000000 hdl21-4.0.0rc0/hdl21/tests/__init__.py
+-rw-r--r--   0 dan        (501) staff       (20)     1091 2022-11-26 00:08:30.000000 hdl21-4.0.0rc0/hdl21/tests/content.py
+-rw-r--r--   0 dan        (501) staff       (20)     3134 2023-01-09 00:49:23.000000 hdl21-4.0.0rc0/hdl21/tests/test_builtin_generators.py
+-rw-r--r--   0 dan        (501) staff       (20)    23228 2023-07-11 16:27:41.000000 hdl21-4.0.0rc0/hdl21/tests/test_bundles.py
+-rw-r--r--   0 dan        (501) staff       (20)     5491 2022-10-17 20:35:07.000000 hdl21-4.0.0rc0/hdl21/tests/test_conns.py
+-rw-r--r--   0 dan        (501) staff       (20)     7227 2023-07-11 16:27:41.000000 hdl21-4.0.0rc0/hdl21/tests/test_doc_examples.py
+-rw-r--r--   0 dan        (501) staff       (20)    18007 2023-07-11 16:27:41.000000 hdl21-4.0.0rc0/hdl21/tests/test_exports.py
+-rw-r--r--   0 dan        (501) staff       (20)    39004 2023-07-11 16:52:24.000000 hdl21-4.0.0rc0/hdl21/tests/test_hdl21.py
+-rw-r--r--   0 dan        (501) staff       (20)     5267 2023-06-26 21:03:45.000000 hdl21-4.0.0rc0/hdl21/tests/test_params.py
+-rw-r--r--   0 dan        (501) staff       (20)    13224 2023-06-26 21:03:45.000000 hdl21-4.0.0rc0/hdl21/tests/test_prefix.py
+-rw-r--r--   0 dan        (501) staff       (20)      741 2022-10-17 20:35:07.000000 hdl21-4.0.0rc0/hdl21/tests/test_source_info.py
+-rw-r--r--   0 dan        (501) staff       (20)      372 2023-03-17 23:05:04.000000 hdl21-4.0.0rc0/hdl21/visibility.py
+-rw-r--r--   0 dan        (501) staff       (20)     4122 2022-11-26 00:08:30.000000 hdl21-4.0.0rc0/hdl21/walker.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:53:02.165519 hdl21-4.0.0rc0/hdl21.egg-info/
+-rw-r--r--   0 dan        (501) staff       (20)    52019 2023-07-11 16:53:02.000000 hdl21-4.0.0rc0/hdl21.egg-info/PKG-INFO
+-rw-r--r--   0 dan        (501) staff       (20)     2649 2023-07-11 16:53:02.000000 hdl21-4.0.0rc0/hdl21.egg-info/SOURCES.txt
+-rw-r--r--   0 dan        (501) staff       (20)        1 2023-07-11 16:53:02.000000 hdl21-4.0.0rc0/hdl21.egg-info/dependency_links.txt
+-rw-r--r--   0 dan        (501) staff       (20)      139 2023-07-11 16:53:02.000000 hdl21-4.0.0rc0/hdl21.egg-info/requires.txt
+-rw-r--r--   0 dan        (501) staff       (20)       15 2023-07-11 16:53:02.000000 hdl21-4.0.0rc0/hdl21.egg-info/top_level.txt
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:53:02.180780 hdl21-4.0.0rc0/pdks/
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:53:02.181277 hdl21-4.0.0rc0/pdks/Asap7/
+-rw-r--r--   0 dan        (501) staff       (20)        0 2022-05-03 17:59:57.000000 hdl21-4.0.0rc0/pdks/Asap7/readme.md
+-rw-r--r--   0 dan        (501) staff       (20)      890 2023-07-11 16:31:14.000000 hdl21-4.0.0rc0/pdks/Asap7/setup.py
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:53:02.182072 hdl21-4.0.0rc0/pdks/Sky130/
+-rw-r--r--   0 dan        (501) staff       (20)    20433 2023-07-11 14:50:48.000000 hdl21-4.0.0rc0/pdks/Sky130/readme.md
+-rw-r--r--   0 dan        (501) staff       (20)      915 2023-07-11 16:52:30.000000 hdl21-4.0.0rc0/pdks/Sky130/setup.py
+-rw-r--r--   0 dan        (501) staff       (20)      643 2023-07-11 14:50:48.000000 hdl21-4.0.0rc0/pdks/readme.md
+-rw-r--r--   0 dan        (501) staff       (20)    51716 2023-07-11 16:27:41.000000 hdl21-4.0.0rc0/readme.md
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:53:02.182228 hdl21-4.0.0rc0/scratch/
+-rw-r--r--   0 dan        (501) staff       (20)        0 2021-09-08 00:13:15.000000 hdl21-4.0.0rc0/scratch/empty
+drwxr-xr-x   0 dan        (501) staff       (20)        0 2023-07-11 16:53:02.183206 hdl21-4.0.0rc0/scripts/
+-rw-r--r--   0 dan        (501) staff       (20)        0 2022-10-27 22:36:09.000000 hdl21-4.0.0rc0/scripts/empty
+-rwxr-xr-x   0 dan        (501) staff       (20)      279 2023-06-07 23:06:22.000000 hdl21-4.0.0rc0/scripts/install-dev.sh
+-rwxr-xr-x   0 dan        (501) staff       (20)      160 2023-06-07 23:06:22.000000 hdl21-4.0.0rc0/scripts/install-pypi.sh
+-rw-r--r--   0 dan        (501) staff       (20)     2350 2023-03-17 23:05:04.000000 hdl21-4.0.0rc0/scripts/primtable.py
+-rw-r--r--   0 dan        (501) staff       (20)       38 2023-07-11 16:53:02.183984 hdl21-4.0.0rc0/setup.cfg
+-rw-r--r--   0 dan        (501) staff       (20)     1396 2023-07-11 16:52:09.000000 hdl21-4.0.0rc0/setup.py
```

### Comparing `hdl21-3.0.dev3/.gitignore` & `hdl21-4.0.0rc0/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -64,28 +64,29 @@
 *.manifest
 *.spec
 
 # Installer logs
 pip-log.txt
 pip-delete-this-directory.txt
 
-# Unit test / coverage reports
+# Unit test / coverage / profiling reports
 htmlcov/
 .tox/
 .nox/
 .coverage
 .coverage.*
 .cache
 nosetests.xml
 coverage.xml
 *.cover
 *.py,cover
 .hypothesis/
 .pytest_cache/
 cover/
+prof/
 
 # Translations
 *.mo
 *.pot
 
 # Django stuff:
 *.log
```

### Comparing `hdl21-3.0.dev3/Cargo.toml` & `hdl21-4.0.0rc0/Cargo.toml`

 * *Files identical despite different names*

### Comparing `hdl21-3.0.dev3/LICENSE` & `hdl21-4.0.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `hdl21-3.0.dev3/PKG-INFO` & `hdl21-4.0.0rc0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,51 @@
 Metadata-Version: 2.1
 Name: hdl21
-Version: 3.0.dev3
+Version: 4.0.0rc0
 Summary: Hardware Description Library
 Home-page: https://github.com/dan-fritchman/Hdl21
 Author: Dan Fritchman
 Author-email: dan@fritch.mn
-Requires-Python: >=3.7, <4
+Requires-Python: >=3.7, <3.12
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # HDL21
 
 ## Analog Hardware Description Library in Python
 
+[![pypi](https://img.shields.io/badge/pypi-hdl21-blue)](https://pypi.org/project/hdl21/)
+[![python-versions](https://img.shields.io/badge/python-3.7_3.8_3.9_3.10_3.11-blue)](https://codecov.io/gh/dan-fritchman/Hdl21)
 [![test](https://github.com/dan-fritchman/Hdl21/actions/workflows/test.yaml/badge.svg)](https://github.com/dan-fritchman/Hdl21/actions/workflows/test.yaml)
 [![codecov](https://codecov.io/gh/dan-fritchman/Hdl21/branch/main/graph/badge.svg?token=f8LKUqEPdq)](https://codecov.io/gh/dan-fritchman/Hdl21)
 
-Hdl21 is a [hardware description library](https://en.wikipedia.org/wiki/Hardware_description_language) embedded in Python. It is targeted and optimized for analog and custom integrated circuits, and for maximum productivity with minimum fancy-programming skill.
-
-Hdl21 generates hardware databases in the [VLSIR](https://github.com/Vlsir/Vlsir) interchange formats, defined through [Google Protocol Buffers](https://developers.google.com/protocol-buffers/). Through [VLSIR's Python tools](https://pypi.org/project/vlsirtools/) Hdl21 also includes drivers for popular industry-standard data formats and popular spice-class simulation engines.
+Hdl21 is a [hardware description library](https://en.wikipedia.org/wiki/Hardware_description_language) embedded in Python.  
+It is targeted for analog and custom integrated circuits, and for maximum productivity with minimum fancy-programming skill.
 
 ## Contents
 
+- [Installation](#installation)
 - [Modules](#modules)
 - [Signals](#signals), [Ports](#signals), and [Connections](#connections)
 - [Generators](#generators) and [Parameters](#parameters)
+- [Primitive Elements and External Modules](#primitives-and-external-modules)
 - [Spice-Class Simulation](#spice-class-simulation)
-- [Primitive Elements](#primitives-and-external-modules)
-- [Process Technology (PDK) Packages](#process-technologies)
-- Coming Soon: Structured Connections with `Bundle`s
-- Coming Soon: [Schematics](https://github.com/Vlsir/Hdl21Schematics)
-- [Examples Library](#examples-library)
+- [Process Technologies (PDKs)](#process-technologies)
+- [Bundles](#bundles)
+- [Examples](#examples)
+- [Related Projects](#related-projects)
+
+## Installation
+
+```
+pip install hdl21
+```
+
+That's it. No crazy build step, no crazy dependencies, no crazy EDA stuff, no "clone and _just_ modify these 300 things", no `source`ing, none of that. Hdl21 is pure Python, and is designed to be as easy to install as any other Python package.
 
 ## Modules
 
 Hdl21's primary unit of hardware reuse is the `Module`. Think of it as Verilog's `module`, or VHDL's `entity`, or SPICE's `subckt`. Better yet if you are used to graphical schematics, think of it as the content of a schematic. Hdl21 `Modules` are containers of a handful of `hdl21` types. Think of them as including:
 
 - Instances of other `Modules`
 - Connections between them, defined by `Signals` and `Ports`
@@ -276,21 +286,46 @@
 o = Outer(**d1)
 # Convert back to another dictionary
 d2 = asdict(o)
 # And check they line up
 assert d1 == d2
 ```
 
+Generators include the capability to construct their param-classes inline, if provided a set of compatible keyword arguments. For example, defining a generator using the `MyParams` parameters above:
+
+```python
+@h.generator
+def MyGen(params: MyParams) -> h.Module:
+    ... # Create a `Module` & return it
+```
+
+This typical invocation:
+
+```python
+p = MyParams(width=8, text="My Favorite Module")
+MyGen(p)
+```
+
+is the same as calling:
+
+```python
+MyParams(width=8, text="My Favorite Module")
+```
+
+Parameters may be provided as keywords, or as a single positional argument which is an instance of the generator's param-class. Combinations of the two are not supported.
+
 ## A Note on Parametrization
 
 Hdl21 `Generators` have parameters. `Modules` do not.
 
 This is a deliberate decision, which in this sense makes `hdl21.Module` less feature-rich than the analogous `module` concepts in existing HDLs (Verilog, VHDL, and even SPICE). These languages support what might be called "static parameters" - relatively simple relationships between parent and child-module parameterization. Setting, for example, the width of a signal or number of instances in an array is straightforward. But more elaborate parametrization-cases are either highly cumbersome or altogether impossible to create. (As an example, try using Verilog parametrization to make a programmable-depth binary tree.) Hdl21, in contrast, exposes all parametrization to the full Python-power of its generators.
 
-## `Prefixed` Numeric Parameters
+## Numeric Parameters
+
+### `Prefixed` Numbers
 
 Hdl21 provides an [SI prefixed](https://www.nist.gov/pml/owm/metric-si-prefixes) numeric type `Prefixed`, which is especially common for physical generator parameters. Each `Prefixed` value is a combination of the Python standard library's `Decimal` and an enumerated SI `Prefix`:
 
 ```python
 @dataclass
 class Prefixed:
     number: Decimal  # Numeric Portion
@@ -301,15 +336,15 @@
 
 `Prefixed` values rarely need to be instantiated directly. Instead Hdl21 exposes a set of common prefixes via their typical single-character names:
 
 ```python
 f = FEMTO = Prefix.FEMTO
 p = PICO = Prefix.PICO
 n = NANO = Prefix.NANO
-µ = MICRO = Prefix.MICRO
+µ = u = MICRO = Prefix.MICRO # Note both `u` and `µ` are valid
 m = MILLI = Prefix.MILLI
 K = KILO = Prefix.KILO
 M = MEGA = Prefix.MEGA
 G = GIGA = Prefix.GIGA
 T = TERA = Prefix.TERA
 P = PETA = Prefix.PETA
 UNIT = Prefix.UNIT
@@ -340,17 +375,165 @@
 
 11 * e(-6) == 11 * µ  # True
 ```
 
 These `e()` values are also most common in multiplication expressions,
 to create `Prefixed` values in "floating point" style such as `11 * e(-9)`.
 
+### `Scalar`
+
+Many Hdl21 primitive parameters can be either numbers or string-literals.  
+The combination is so common that Hdl21 defines a `Scalar` type which is (roughly):
+
+```python
+Scalar = Union[Prefixed, Literal]
+```
+
+With automatic conversions from each of `str`, `int`, `float`, and `Decimal`.
+
+`Scalar` is particularly designed for parameter-values of `Primitive`s and of simulations.
+Most such parameters "want" to be the `Prefixed` type, for reasons outlined [above](#prefixed-numeric-parameters). They often also need a string-valued escape hatch, e.g. when referring to out-of-Hdl21 quantities
+such as parameters in external netlists or simulation decks.
+These out-of-Hdl21 expressions are represented by the `Literal` type, a simple wrapper around `str`.
+
+Where possible `Scalar` prefers to use the `Prefixed` variant.
+Built-in numbers `(int, float, Decimal)` are converted to `Prefixed` inline.
+Strings are attempted to be converted to `Prefixed`, and fall back to `Literal` if unsuccessful.
+This conversion process is also available as the free-standing `to_scalar()` function.
+
+Example:
+
+```python
+import hdl21 as h
+from hdl21.prefix import NANO, µ
+from decimal import Decimal
+
+@h.paramclass
+class MyMosParams:
+    w = h.Param(dtype=h.Scalar, desc="Width", default=1e-6) # Default `float` converts to a `Prefixed`
+    l = h.Param(dtype=h.Scalar, desc="Length", default="w/5") # Default `str` converts to a `Literal`
+
+# Example instantiations
+MyMosParams() # Default values
+MyMosParams(w=Decimal(1e-6), l=3*µ)
+MyMosParams(w=h.Literal("sim_param_width"), l=h.Prefixed.new(20, NANO))
+MyMosParams(w="11*l", l=11)
+```
+
+When defining "primitive level" parameters - e.g. those that will be used in PDK-level devices - `Scalar` is generally the best datatype to use.
+
+## Primitives and External Modules
+
+The leaf-nodes of each hierarchical Hdl21 circuit are generally defined in one of two places:
+
+- `Primitive` elements, defined in the `hdl21.primitives` package. Each is designed to be a technology-independent representation of an irreducible component.
+- `ExternalModules`, defined outside Hdl21. Such "module wrappers", which might alternately be called "black boxes", are common for including circuits from other HDLs.
+
+### `Primitives`
+
+Hdl21's library of generic primitive elements is defined in the `hdl21.primitives` package. Its content is roughly equivalent to that built into a typical SPICE simulator.
+
+A summary of `hdl21.primitives`:
+
+| Name                           | Description                       | Type     | Aliases                               | Ports        |
+| ------------------------------ | --------------------------------- | -------- | ------------------------------------- | ------------ |
+| Mos                            | Mos Transistor                    | PHYSICAL | MOS                                   | d, g, s, b   |
+| IdealResistor                  | Ideal Resistor                    | IDEAL    | R, Res, Resistor, IdealR, IdealRes    | p, n         |
+| PhysicalResistor               | Physical Resistor                 | PHYSICAL | PhyR, PhyRes, ResPhy, PhyResistor     | p, n         |
+| ThreeTerminalResistor          | Three Terminal Resistor           | PHYSICAL | Res3, PhyRes3, ResPhy3, PhyResistor3  | p, n, b      |
+| IdealCapacitor                 | Ideal Capacitor                   | IDEAL    | C, Cap, Capacitor, IdealC, IdealCap   | p, n         |
+| PhysicalCapacitor              | Physical Capacitor                | PHYSICAL | PhyC, PhyCap, CapPhy, PhyCapacitor    | p, n         |
+| ThreeTerminalCapacitor         | Three Terminal Capacitor          | PHYSICAL | Cap3, PhyCap3, CapPhy3, PhyCapacitor3 | p, n, b      |
+| IdealInductor                  | Ideal Inductor                    | IDEAL    | L, Ind, Inductor, IdealL, IdealInd    | p, n         |
+| PhysicalInductor               | Physical Inductor                 | PHYSICAL | PhyL, PhyInd, IndPhy, PhyInductor     | p, n         |
+| ThreeTerminalInductor          | Three Terminal Inductor           | PHYSICAL | Ind3, PhyInd3, IndPhy3, PhyInductor3  | p, n, b      |
+| PhysicalShort                  | Short-Circuit/ Net-Tie            | PHYSICAL | Short                                 | p, n         |
+| DcVoltageSource                | DC Voltage Source                 | IDEAL    | V, Vdc, Vsrc                          | p, n         |
+| PulseVoltageSource             | Pulse Voltage Source              | IDEAL    | Vpu, Vpulse                           | p, n         |
+| CurrentSource                  | Ideal DC Current Source           | IDEAL    | I, Idc, Isrc                          | p, n         |
+| VoltageControlledVoltageSource | Voltage Controlled Voltage Source | IDEAL    | Vcvs, VCVS                            | p, n, cp, cn |
+| CurrentControlledVoltageSource | Current Controlled Voltage Source | IDEAL    | Ccvs, CCVS                            | p, n, cp, cn |
+| VoltageControlledCurrentSource | Voltage Controlled Current Source | IDEAL    | Vccs, VCCS                            | p, n, cp, cn |
+| CurrentControlledCurrentSource | Current Controlled Current Source | IDEAL    | Cccs, CCCS                            | p, n, cp, cn |
+| Bipolar                        | Bipolar Transistor                | PHYSICAL | Bjt, BJT                              | c, b, e      |
+| Diode                          | Diode                             | PHYSICAL | D                                     | p, n         |
+
+Each primitive is available in the `hdl21.primitives` namespace, either through its full name or any of its aliases. Most primitives have fairly verbose names (e.g. `VoltageControlledCurrentSource`, `IdealResistor`), but also expose short-form aliases (e.g. `Vcvs`, `R`). Each of the aliases in Table 1 above refer to _the same_ Python object, i.e.
+
+```python
+from hdl21.primitives import R, Res, IdealResistor
+
+R is Res            # evaluates to True
+R is IdealResistor  # also evaluates to True
+```
+
+Hdl21 `Primitives` come in _ideal_ and _physical_ flavors. The difference is most frequently relevant for passive elements, which can for example represent either
+
+- (a) technology-specific passives, e.g. a MIM or MOS capacitor, or
+- (b) an _ideal_ capacitor
+
+Some element-types have solely physical implementations, some are solely ideal, and others include both.
+
+### `ExternalModules`
+
+Alternately Hdl21 includes an `ExternalModule` type which defines the interface to a module-implementation outside Hdl21. These external definitions are common for instantiating technology-specific modules and libraries. Think of them as a module "function header"; other popular modern HDLs refer to them as module _black boxes_.
+
+An example `ExternalModule`:
+
+```python
+import hdl21 as h
+from hdl21.prefix import µ
+from hdl21.primitives import Diode
+
+@h.paramclass
+class BandGapParams:
+    self_destruct = h.Param(
+        dtype=bool,
+        desc="Whether to include the self-destruction feature",
+        default=True,
+    )
+
+BandGap = h.ExternalModule(
+    name="BandGap",
+    desc="Example ExternalModule, defined outside Hdl21",
+    port_list=[h.Port(name="vref"), h.Port(name="enable")],
+    paramtype=BandGapParams,
+)
+```
+
+Both `Primitives` and `ExternalModules` have names, ordered `Ports`, and a few other pieces of metadata, but no internal implementation: no internal signals, and no instances of other modules. Unlike `Modules`, both _do_ have parameters. `Primitives` each have an associated `paramclass`, while `ExternalModules` can optionally declare one via their `paramtype` attribute. Their parameter-types are limited to a small subset of those possible for `Generators` - generally "scalar" types such as numbers, strings, and `Scalar` - primarily limited by the need to need to provide them to legacy HDLs. Parameters are applied in the same style as for `Generators`, by calling the `Primitive` or `ExternalModule`. Parameter-applications can either be an instance of the module's `paramtype` or a set of keyword arguments which validly contruct one inline.
+
+```python
+# Continuing from the snippet above:
+params = BandGapParams(self_destruct=False)  # Watch out there!
+```
+
+`Primitives` and `ExternalModules` can be instantiated and connected in all the same styles as `Modules`:
+
+```python
+@h.module
+class BandGapPlus:
+    vref, enable = h.Signals(2)
+    # Instantiate the `ExternalModule` defined above
+    bg = BandGap(params)(vref=vref, enable=enable)
+    # ...Anything else...
+
+@h.module
+class DiodePlus:
+    p, n = h.Signals(2)
+    # Parameterize, instantiate, and connect a `primitives.Diode`
+    d = Diode(w=1 * µ, l=1 * µ)(p=p, n=n)
+    # ... Everything else ...
+```
+
 ## Exporting and Importing
 
-Hdl21's primary import/ export format is [VLSIR](https://github.com/Vlsir/Vlsir). VLSIR is a binary ProtoBuf-based format with support for a variety of industry-standard formats and tools. The `hdl21.to_proto()` function converts an Hdl21 `Module` or group of `Modules` into VLSIR `Package`. The `hdl21.from_proto()` function similarly imports a VLSIR `Package` into a namespace of Hdl21 `Modules`.
+Hdl21 generates hardware databases in the [VLSIR](https://github.com/Vlsir/Vlsir) interchange formats, defined through [Google Protocol Buffers](https://developers.google.com/protocol-buffers/). Through [VLSIR's Python tools](https://pypi.org/project/vlsirtools/) Hdl21 also includes drivers for popular industry-standard data formats and popular spice-class simulation engines.
+
+The `hdl21.to_proto()` function converts an Hdl21 `Module` or group of `Modules` into a VLSIR `Package`. The `hdl21.from_proto()` function similarly imports a VLSIR `Package` into a Python namespace of Hdl21 `Modules`.
 
 Exporting to industry-standard netlist formats is a particularly common operation for Hdl21 users. The `hdl21.netlist()` function uses VLSIR to export any of its supported netlist formats.
 
 ```python
 import sys
 import hdl21 as h
 
@@ -362,28 +545,45 @@
     cap = h.Cap(c=1e3)(p=p, n=n)
     ind = h.Ind(l=1e-9)(p=p, n=n)
 
 # Write a spice-format netlist to stdout
 h.netlist(Rlc, sys.stdout, fmt="spice")
 ```
 
-`hdl21.netlist` takes a second destination argument `dest`, which is commonly either an open file-handle or `sys.stdout`. All its remaining arguments are passed to `vlsirtools.netlist`.
+`hdl21.netlist` takes a second destination argument `dest`, which is commonly either an open file-handle or `sys.stdout`.
+
+Each `Module` includes a list of `Literal` contents, designed to be included directly in exported netlists. These are commonly used to refer to out-of-Hdl21 quantities, or to include netlist-language features not first-class supported by Hdl21. Example:
+
+```python
+@h.module
+class HasLiterals:
+    a, b, c = h.Ports(3)
+
+# Add some literal content
+HasLiterals.literals.extend([
+    h.Literal("generate some_verilog_code"),
+    h.Literal(".some_spice_attribute what=ever"),
+    h.Literal("PRAGMA: some_pragma"),
+])
+```
+
+`Module.literals` is a Python built-in list and can be manipulated with any of its typical methods (`append`, `extend`, etc.). Literals are written to netlists in the order they appear in the list. Order between Literals and other Module content is not preserved.
 
 ## Spice-Class Simulation
 
 Hdl21 includes drivers for popular spice-class simulation engines commonly used to evaluate analog circuits.
 The `hdl21.sim` package includes a wide variety of spice-class simulation constructs, including:
 
 - DC, AC, Transient, Operating-Point, Noise, Monte-Carlo, Parameter-Sweep and Custom (per netlist language) Analyses
 - Control elements for saving signals (`Save`), simulation options (`Options`), including external files and contents (`Include`, `Lib`), measurements (`Meas`), simulation parameters (`Param`), and literal netlist commands (`Literal`)
 
 The entrypoint to Hdl21-driven simulation is the simulation-input type `hdl21.sim.Sim`. Each `Sim` includes:
 
 - A testbench Module `tb`, and
-- A list of unordered simulation attributes (`attrs`), including any and all of the analyses, controls, and related elements listed above.
+- A list of simulation attributes (`attrs`), including any and all of the analyses, controls, and related elements listed above.
 
 Example:
 
 ```python
 import hdl21 as h
 from hdl21.sim import *
 
@@ -418,23 +618,26 @@
     ],
 )
 
 # And run it!
 sim.run()
 ```
 
-`Sim` also includes a class-based syntax similar to `Module` and `Bundle`, in which simulation attributes are named based on their class attribute name:
+`Sim` also includes a class-based syntax similar to `Module` and `Bundle`. This also allows for inline definition of a testbench module, which can be named either `tb` or `Tb`:
 
 ```python
 import hdl21 as h
 from hdl21.sim import *
 
 @sim
 class MySim:
-    tb = MyModulesTestbench
+
+    @h.module
+    class Tb:
+        # ... Testbench content ...
 
     x = Param(5)
     y = Param(6)
     mydc = Dc(var=x, sweep=PointSweep([1]))
     myac = Ac(sweep=LogSweep(1e1, 1e10, 10))
     mytran = Tran(tstop=11 * h.prefix.PICO)
     mysweep = SweepAnalysis(
@@ -454,15 +657,15 @@
 MySim.run()
 ```
 
 Note that in these class-based definitions, attributes whose names don't really matter such as `save_all` above can be _named_ anything, but must be _assigned_ into the class, not just constructed.
 
 Class-based `Sim` definitions retain all class members which are `SimAttr`s and drop all others. Non-`SimAttr`-valued fields can nonetheless be handy for defining intermediate values upon which the ultimate SimAttrs depend, such as the `a_path` field in the example above.
 
-Classes decoratated by `sim` a single special required field: a `tb` attribute which sets the simulation testbench. A handful of names are disallowed in `sim` class-definitions, generally corresponding to the names of the `Sim` class's fields and methods such as `attrs` and `run`.
+Classes decorated by `@sim` have a single special required field: a testbench attribute, named either `tb` or `Tb`, which sets the simulation testbench. A handful of names are disallowed in `sim` class-definitions, generally corresponding to the names of the `Sim` class's fields and methods such as `attrs` and `run`.
 
 Each `sim` also includes a set of methods to add simulation attributes from their keyword constructor arguments. These methods use the same names as the simulation attributes (`Dc`, `Meas`, etc.) but incorporating the python language convention that functions and methods be lowercase (`dc`, `meas`, etc.). Example:
 
 ```python
 # Create a `Sim`
 s = Sim(tb=MyTb)
 
@@ -487,137 +690,52 @@
 s.lib(path="/home/models", section="fast")
 s.options(reltol=1e-9)
 
 # And run it!
 s.run()
 ```
 
-## Primitives and External Modules
-
-The leaf-nodes of each hierarchical Hdl21 circuit are generally defined in one of two places:
-
-- `Primitive` elements, defined in the `hdl21.primitives` package. These include transistors, resistors, capacitors, and other irreducible components. Simulation-level behavior of these elements is typically defined _inside of_ simulation tools and other EDA software.
-- `ExternalModules`, defined outside Hdl21. Such "module wrappers", which might alternately be called "black boxes", are common for including circuits from other HDLs.
-
-### `Primitives`
-
-Hdl21 `Primitives` come in _ideal_ and _physical_ flavors. The difference is most frequently relevant for passive elements, which can for example represent either (a) technology-specific passives, e.g. a MIM or MOS capacitor, or (b) an _ideal_ capacitor. Some element-types have solely physical implementations, some are solely ideal, and others include both.
-
-### The `hdl21.primitives` Library
-
-The `Primitive` type and all its valid values are defined by the `hdl21.primitives` package. A summary of the `hdl21.primitives` library content:
-
-| Name                           | Description                       | Type     | Aliases                               | Ports        |
-| ------------------------------ | --------------------------------- | -------- | ------------------------------------- | ------------ |
-| Mos                            | Mos Transistor                    | PHYSICAL | MOS                                   | d, g, s, b   |
-| IdealResistor                  | Ideal Resistor                    | IDEAL    | R, Res, Resistor, IdealR, IdealRes    | p, n         |
-| PhysicalResistor               | Physical Resistor                 | PHYSICAL | PhyR, PhyRes, ResPhy, PhyResistor     | p, n         |
-| ThreeTerminalResistor          | Three Terminal Resistor           | PHYSICAL | Res3, PhyRes3, ResPhy3, PhyResistor3  | p, n, b      |
-| IdealCapacitor                 | Ideal Capacitor                   | IDEAL    | C, Cap, Capacitor, IdealC, IdealCap   | p, n         |
-| PhysicalCapacitor              | Physical Capacitor                | PHYSICAL | PhyC, PhyCap, CapPhy, PhyCapacitor    | p, n         |
-| ThreeTerminalCapacitor         | Three Terminal Capacitor          | PHYSICAL | Cap3, PhyCap3, CapPhy3, PhyCapacitor3 | p, n, b      |
-| IdealInductor                  | Ideal Inductor                    | IDEAL    | L, Ind, Inductor, IdealL, IdealInd    | p, n         |
-| PhysicalInductor               | Physical Inductor                 | PHYSICAL | PhyL, PhyInd, IndPhy, PhyInductor     | p, n         |
-| ThreeTerminalInductor          | Three Terminal Inductor           | PHYSICAL | Ind3, PhyInd3, IndPhy3, PhyInductor3  | p, n, b      |
-| PhysicalShort                  | Short-Circuit/ Net-Tie            | PHYSICAL | Short                                 | p, n         |
-| DcVoltageSource                | DC Voltage Source                 | IDEAL    | V, Vdc, Vsrc                          | p, n         |
-| PulseVoltageSource             | Pulse Voltage Source              | IDEAL    | Vpu, Vpulse                           | p, n         |
-| CurrentSource                  | Ideal DC Current Source           | IDEAL    | I, Idc, Isrc                          | p, n         |
-| VoltageControlledVoltageSource | Voltage Controlled Voltage Source | IDEAL    | Vcvs, VCVS                            | p, n, cp, cn |
-| CurrentControlledVoltageSource | Current Controlled Voltage Source | IDEAL    | Ccvs, CCVS                            | p, n, cp, cn |
-| VoltageControlledCurrentSource | Voltage Controlled Current Source | IDEAL    | Vccs, VCCS                            | p, n, cp, cn |
-| CurrentControlledCurrentSource | Current Controlled Current Source | IDEAL    | Cccs, CCCS                            | p, n, cp, cn |
-| Bipolar                        | Bipolar Transistor                | PHYSICAL | Bjt, BJT                              | c, b, e      |
-| Diode                          | Diode                             | PHYSICAL | D                                     | p, n         |
-
-Each primitive is available in the `hdl21.primitives` namespace, either through its full name or any of its aliases. Most primitives have fairly verbose names (e.g. `VoltageControlledCurrentSource`, `IdealResistor`), but also expose short-form aliases (e.g. `Vcvs`, `R`). Each of the aliases in Table 1 above refer to _the same_ Python object, i.e.
-
-```python
-from hdl21.primitives import R, Res, IdealResistor
-
-R is Res            # evaluates to True
-R is IdealResistor  # also evaluates to True
-```
-
-### `ExternalModules`
-
-Alternately Hdl21 includes an `ExternalModule` type which defines the interface to a module-implementation outside Hdl21. These external definitions are common for instantiating technology-specific modules and libraries. Other popular modern HDLs refer to these as module _black boxes_. An example `ExternalModule`:
-
-```python
-import hdl21 as h
-from hdl21.prefix import µ
-from hdl21.primitives import Diode
-
-@h.paramclass
-class BandGapParams:
-    self_destruct = h.Param(
-        dtype=bool,
-        desc="Whether to include the self-destruction feature",
-        default=True,
-    )
-
-BandGap = h.ExternalModule(
-    name="BandGap",
-    desc="Example ExternalModule, defined outside Hdl21",
-    port_list=[h.Port(name="vref"), h.Port(name="enable")],
-    paramtype=BandGapParams,
-)
-```
-
-Both `Primitives` and `ExternalModules` have names, ordered `Ports`, and a few other pieces of metadata, but no internal implementation: no internal signals, and no instances of other modules. Unlike `Modules`, both _do_ have parameters. `Primitives` each have an associated `paramclass`, while `ExternalModules` can optionally declare one via their `paramtype` attribute. Their parameter-types are limited to a small subset of those possible for `Generators` - scalar numeric types (`int`, `float`) and `str` - primarily limited by the need to need to provide them to legacy HDLs.
-
-`Primitives` and `ExternalModules` can be instantiated and connected in all the same styles as `Modules`:
-
-```python
-# Continuing from the snippet above:
-params = BandGapParams(self_destruct=False)  # Watch out there!
-
-@h.module
-class BandGapPlus:
-    vref, enable = h.Signals(2)
-    # Instantiate the `ExternalModule` defined above
-    bg = BandGap(params)(vref=vref, enable=enable)
-    # ...Anything else...
-
-@h.module
-class DiodePlus:
-    p, n = h.Signals(2)
-    # Parameterize, instantiate, and connect a `primitives.Diode`
-    d = Diode(w=1 * µ, l=1 * µ)(p=p, n=n)
-    # ... Everything else ...
-```
-
 ## Process Technologies
 
 Designing for a specific implementation technology (or "process development kit", or PDK) with Hdl21 can use either of (or a combination of) two routes:
 
 - Instantiate `ExternalModules` corresponding to the target technology. These would commonly include its process-specific transistor and passive modules, and potentially larger cells, for example from a cell library. Such external modules are frequently defined as part of a PDK (python) package, but can also be defined anywhere else, including inline among Hdl21 generator code.
-- Use `hdl21.Primitives`, each of which is designed to be a technology-independent representation of a primitive component. Moving to a particular technology then generally requires passing the design through an `hdl21.pdk` converter.
+- Use `hdl21.Primitives`, each of which is designed to be a technology-independent representation of a primitive component. Moving to a particular technology then generally requires passing the design through an `hdl21.pdk`'s `compile` function.
 
 Hdl21 PDKs are Python packages which generally include two primary elements:
 
 - (a) A library `ExternalModules` describing the technology's cells, and
 - (b) A `compile` conversion-method which transforms a hierarchical Hdl21 tree, mapping generic `hdl21.Primitives` into the tech-specific `ExternalModules`.
 
-Since PDKs are python packages, using them is as simple as importing them. Hdl21 includes two built-in PDKs: the academic predicitive [ASAP7](https://pypi.org/project/asap7-hdl21/) technology, and the open-source [SkyWater 130nm](https://pypi.org/project/sky130-hdl21/) technology.
+Since PDKs are python packages, using them is as simple as importing them. Hdl21 includes a built-in sample PDK available via `hdl21.pdk.sample_pdk` which includes simulatable NMOS and PMOS transistors. Hdl21's source tree includes three additional PDK packages:
+
+|                                       | PyPi                                   | Source        |
+| ------------------------------------- | -------------------------------------- | ------------- |
+| ASAP7 Predictive/ Academic PDK        | https://pypi.org/project/asap7-hdl21/  | [pdks/Asap7](./pdks/Asap7)  |
+| SkyWater 130nm Open-Source PDK        | https://pypi.org/project/sky130-hdl21/ | [pdks/Sky130](./pdks/Sky130) |
+| GlobalFoundries 180nm Open-Source PDK | https://pypi.org/project/gf180-hdl21   | [pdks/Gf180](./pdks/Gf180)  |
+
+Each contain much more detail documentation on their specific installation and use.
 
 ```python
 import hdl21 as h
-import sky130
+import sky130_hdl21
 
 @h.module
 class SkyInv:
     """ An inverter, demonstrating using PDK modules """
 
     # Create some IO
     i, o, VDD, VSS = h.Ports(4)
 
+    p = sky130_hdl21.Sky130MosParams(w=1,l=1)
+
     # And create some transistors!
-    ps = sky130.modules.sky130_fd_pr__pfet_01v8(w=1, l=1)(d=o, g=i, s=VDD, b=VDD)
-    ns = sky130.modules.sky130_fd_pr__nfet_01v8(w=1, l=1)(d=o, g=i, s=VSS, b=VSS)
+    ps = sky130_hdl21.primtives.PMOS_1p8V_STD(p)(d=o, g=i, s=VDD, b=VDD)
+    ns = sky130_hdl21.primtives.NMOS_1p8V_STD(p)(d=o, g=i, s=VSS, b=VSS)
 ```
 
 Process-portable modules instead use Hdl21 `Primitives`, which can be compiled to a target technology:
 
 ```python
 import hdl21 as h
 from hdl21.prefix import µ
@@ -635,17 +753,17 @@
     ns = Nmos(w=1*µ, l=1*µ, vth=MosVth.STD)(d=o, g=i, s=VSS, b=VSS)
 ```
 
 Compiling the generic devices to a target PDK then just requires a pass through the PDK's `compile()` method:
 
 ```python
 import hdl21 as h
-import sky130
+import sky130_hdl21
 
-sky130.compile(Inv) # Produces the same content as `SkyInv` above
+sky130_hdl21.compile(Inv) # Produces the same content as `SkyInv` above
 ```
 
 Hdl21 includes an `hdl21.pdk` subpackage which tracks the available in-memory PDKs. If there is a single PDK available, it need not be explicitly imported: `hdl21.pdk.compile()` will use it by default.
 
 ```python
 import hdl21 as h
 import sky130  # Note this import can be elsewhere in the program, i.e. in a configuration layer.
@@ -682,15 +800,15 @@
 CmosCorner = TT | FF | SS | SF | FS
 ```
 
 Hdl21 exposes each of these corner-types as Python enumerations and combinations thereof. Each PDK package then defines its mapping from these `Corner` types to the content they include, typically in the form of external files.
 
 ### PDK Installations and Sites
 
-Much of the content of a typical process technology - even the subset that Hdl21 cares about - is not defined in Python. Transistor models and SPICE "library" files, such as those defining the `_nfet` and `_pfet` above, are common examples pertinent to Hdl21. Tech-files, layout libraries, and the like are similarly necessary for related pieces of EDA software. These PDK contents are commonly stored in a technology-specific arrangement of interdependent files. Hdl21 PDK packages structure this external content as a `PdkInstallation` type.
+Much of the content of a typical process technology - even the subset that Hdl21 cares about - is not defined in Python. Transistor models and SPICE "library" files, such as those defining the `PMOS` and `NMOS` above, are common examples pertinent to Hdl21. Tech-files, layout libraries, and the like are similarly necessary for related pieces of EDA software. These PDK contents are commonly stored in a technology-specific arrangement of interdependent files. Hdl21 PDK packages structure this external content as a `PdkInstallation` type.
 
 Each `PdkInstallation` is a runtime type-checked Python `dataclass` which extends the base `hdl21.pdk.PdkInstallation` type. Installations are free to define arbitrary fields and methods, which will be type-validated for each `Install` instance. Example:
 
 ```python
 """ A sample PDK package with an `Install` type """
 
 from pydantic.dataclasses import dataclass
@@ -738,19 +856,19 @@
 
 These "site packages" are named `sitepdks` by convention. They can often be shared among several PDKs on a given filesystem. Hdl21 includes one built-in example such site-package, [SampleSitePdks](./SampleSitePdks/), which demonstrates setting up both built-in PDKs, Sky130 and ASAP7:
 
 ```python
 # The built-in sample `sitepdks` package
 from pathlib import Path
 
-import sky130
-sky130.install = sky130.Install(model_lib=Path("pdks") / "sky130" / ... / "sky130.lib.spice")
+import sky130_hdl21
+sky130_hdl21.install = sky130_hdl21.Install(model_lib=Path("pdks") / "sky130" / ... / "sky130.lib.spice")
 
-import asap7
-asap7.install = asap7.Install(model_lib=Path("pdks") / "asap7" / ... / "TT.pm")
+import asap7_hdl21
+asap7_hdl21.install = asap7_hdl21.Install(model_lib=Path("pdks") / "asap7" / ... / "TT.pm")
 ```
 
 "Site-portable" code requiring external PDK content can then refer to the PDK package's `install`, without being directly aware of its contents.
 An example simulation using `mypdk`'s models with the `sitepdk`s defined above:
 
 ```python
 # sim_my_pdk.py
@@ -770,25 +888,218 @@
 
 # And run it!
 SimMyPdk.run()
 ```
 
 Note that `sim_my_pdk.py` need not necessarily import or directly depend upon `sitepdks` itself. So long as `sitepdks` is imported and configures the PDK installation anywhere in the Python program, further code will be able to refer to the PDK's `install` fields.
 
-## Examples Library
+### Creating PDK Packages
+
+Hdl21's source tree includes a [cookiecutter template](https://github.com/cookiecutter/cookiecutter) for creating a new PDK package, available at [pdks/PdkTemplate](./pdks/PdkTemplate).
+
+## Bundles
+
+Hdl21 `Bundle`s are _structured connection types_ which can include `Signal`s and instances of other `Bundle`s.
+Think of them as "connection structs". Similar ideas are implemented by Chisel's `Bundle`s and SystemVerilog's `interface`s.
+
+```python
+@h.bundle
+class Diff:
+    p = h.Signal()
+    n = h.Signal()
+
+@h.bundle
+class Quadrature:
+    i = Diff()
+    q = Diff()
+```
+
+Like `Module`s, `Bundle`s can be defined either procedurally or as a class decorated by the `hdl21.bundle` function.
+
+```python
+# This creates the same stuff as the class-based definitions above:
+
+Diff = h.Bundle(name="Diff")
+Diff.add(h.Signal(name="p"))
+Diff.add(h.Signal(name="n"))
+
+Quadrature = h.Bundle(name="Quadrature")
+Quadrature.add(Diff(name="i"))
+Quadrature.add(Diff(name="q"))
+```
+
+Calling a `Bundle` as in the calls to `Diff()` and `Diff(name=q)` creates an instance of that `Bundle`.
+
+## Bundle Ports
+
+Bundles are commonly most valuable for shipping collections of related `Signal`s between `Module`s.
+Modules can accordingly have Bundle-valued ports. To create a Bundle-port, set the `port` argument to either the boolean `True`
+or the `hdl21.Visibility.PORT` value.
+
+```python
+@h.module
+class HasDiffs:
+    d1 = Diff(port=True)
+    d2 = Diff(port=h.Visbility.PORT)
+```
+
+Port directions on bundle-ports can be set by either of two methods.
+The first is to set the directions directly on the Bundle's constituent `Signal`s.
+To swap directions, pass the bundle-instances through the `hdl21.flipped` function,
+or set the `flipped` argument to the instance-constructor.
+
+```python
+@h.bundle
+class Inner:
+    i = h.Input()
+    o = h.Output()
+
+@h.bundle
+class Outer:
+    b1 = Inner()
+    b2 = h.flipped(Inner())
+    b3 = Inner(flipped=True)
+```
+
+Here:
+
+- An `Inner` bundle defines an `Input` and an `Output`
+- An `Outer` bundle instantiates three of them
+  - Instance `b1` is not flipped; its `i` is an input, and its `o` is an output
+  - Instance `b2` is flipped; its `i` is an _output_, and its `o` is an _input_
+  - Instance `b3` is also flipped, via its constructor argument
+
+These "flipping based" bundles require that all constituent signals, including nested ones, have port-visibility.
+The rules for flipping port directions are:
+
+- Inputs become Outputs
+- Outputs become Inputs
+- Inouts and undirected ports (`direction=NONE`) retain their directions
+
+```python
+@h.bundle
+class B:
+    clk = h.Output()
+    data = h.Input()
+
+@h.module
+class X: # Module with a `clk` output and `data` input
+    b = B(port=True)
+
+@h.module
+class Y: # Module with a `clk` input and `data` output
+    b = B(flipped=True, port=True)
+
+@h.module
+class Z:
+    b = B() # Internal instance of the `B` bundle
+    x = X(b=b)
+    y = Y(b=b)
+```
+
+The second method for setting bundle-port directions is with `Role`s.
+Each Hdl21 bundle either explicitly or implictly defines a set of `Role`s, which might alternately be called "endpoints".
+These are the expected "end users" of the Bundle.
+Signal directions are then defined on each signal's `src` (source) and `dest` (destination) arguments, which can be set to any of the bundle's roles.
+
+```python
+@h.roles
+class HostDevice(Enum):
+    HOST = auto()
+    DEVICE = auto()
+
+@h.bundle
+class Jtag:
+    roles = HostDevice # Set the bundle's roles
+    # Note each signal sets one of the roles as `src` and another as `dest`
+    tck, tdi, tms = h.Signals(3, src=roles.HOST, dest=roles.DEVICE)
+    tdo = h.Signal(src=roles.DEVICE, dest=roles.HOST)
+```
+
+Bundle-valued ports are then assigned a role and associated signal-port directions via their `role` constructor argument.
+
+```python
+@h.module
+class Widget: # with a Jtag Device port
+    jtag = Jtag(port=True, role=Jtag.roles.DEVICE)
+
+@h.module
+class Debugger: # with a Jtag Host port
+    jtag = Jtag(port=True, role=Jtag.roles.HOST)
+
+@h.module
+class System: # combining the two
+    widget = Widget()
+    debugger = Debugger(jtag=widget.jtag)
+```
+
+The rules for port-directions of role-based bundles are:
+
+- If the bundle's role is the signal's source, the signal is an `Output`
+- If the bundle's role is the signal's destination, the signal is an `Input`
+- Otherwise the signal is assigned no direction, i.e. `direction=NONE`
+
+## Collecting Bundles
+
+It is often helpful or necessary to collect existing signals into a bundle, or to "re-arrange" signals from one bundle into another.
+The primary mechanism for doing so is the `hdl21.bundlize` function which creates them.
+Each call to `bundlize` creates an "anonymous" bundle which lacks a backing bundle-definition type.
+
+```python
+@h.bundle
+class Uart:
+    tx = h.Output()
+    rx = h.Input()
+
+@h.module
+class HasUart:
+    # Module with a `Uart` port
+    uart = Uart(port=True)
+
+@h.module
+class ConnectTwo:
+    # Connect two `HasUart`s, swapping `tx` and `rx`.
+    uart = Uart()
+    m1 = HasUart(uart=uart)
+    m2 = HasUart(uart=h.bundlize(tx=uart.rx, rx=uart.tx))
+```
+
+## Examples
+
+### Built-In Examples Library
 
 Hdl21's source tree includes a built-in [examples](./examples/) library. Each is designed to be a straightforward but realistic use-case, and is a self-contained Python program which can be run directly, e.g. with:
 
 ```bash
 python examples/rdac.py
 ```
 
+The built-in examples include:
+
+- [Current DAC](./examples/idac.py)
+- [MOS Transistor Simulation](./examples/mos_sim.py)
+- [Ring Oscillator Generator](./examples/ro.py)
+- [Resistor-Ladder DAC](./examples/rdac.py)
+- [Recursive Binary to One-Hot Encoders](./examples/encoder.py)
+
 Reading, copying, or cloning these example programs is generally among the best ways to get started.  
 And adding an example is a **highly** encouraged form of [pull request](https://github.com/dan-fritchman/Hdl21/pulls)!
 
+### Featured Community Examples
+
+- [Continuous-Time Delta-Sigma ADC Generators](https://github.com/aviralpandey/CT-DS-ADC_generator)
+- [USB 2.0 PHY](https://github.com/Vlsir/Usb2Phy/tree/main/Usb2PhyAna)
+- [VCO-Based ADC Generators](https://github.com/aviralpandey) (Coming soon!)
+
+## Related Projects
+
+- [VLSIR](https://github.com/vlsir/vlsir)
+- [Hdl21 Schematics](https://github.com/vlsir/hdl21schematics)
+- [Layout21](https://github.com/dan-fritchman/Layout21)
+
 ## Why Use Python?
 
 Custom IC design is a complicated field. Its practitioners have to know
 [a](https://people.eecs.berkeley.edu/~boser/courses/240B/lectures/M07%20OTA%20II.pdf) |
 [lot](http://rfic.eecs.berkeley.edu/~niknejad/ee142_fa05lects/pdf/lect24.pdf) |
 [of](https://www.delroy.com/PLL_dir/ISSCC2004/PLLTutorialISSCC2004.pdf) |
 [stuff](https://inst.eecs.berkeley.edu/~ee247/fa10/files07/lectures/L25_2_f10.pdf),
```

### Comparing `hdl21-3.0.dev3/SampleSitePdks/readme.md` & `hdl21-4.0.0rc0/SampleSitePdks/readme.md`

 * *Files identical despite different names*

### Comparing `hdl21-3.0.dev3/SampleSitePdks/setup.py` & `hdl21-4.0.0rc0/SampleSitePdks/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,28 +11,28 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "readme.md").read_text(encoding="utf-8")
 
-_VLSIR_VERSION = "3.0.dev3"
+_VLSIR_VERSION = "4.0.rc0"
 
 setup(
     name="sitepdks",
     version=_VLSIR_VERSION,
     description="PDK Installations on THIS Machine",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="Dan Fritchman",
     author_email="dan@fritch.mn",
     packages=find_packages(),
-    python_requires=">=3.8, <4",
+    python_requires=">=3.7",
     install_requires=[
         f"sky130-hdl21=={_VLSIR_VERSION}",
-        f"asap7-hdl21=={_VLSIR_VERSION}",
+        # f"asap7-hdl21=={_VLSIR_VERSION}",
     ],
     extras_require={
         "dev": ["pytest==7.1", "coverage", "pytest-cov", "black==22.6", "twine"]
     },
 )
```

### Comparing `hdl21-3.0.dev3/SampleSitePdks/sitepdks.py` & `hdl21-4.0.0rc0/SampleSitePdks/sitepdks.py`

 * *Files 21% similar despite different names*

```diff
@@ -19,19 +19,30 @@
 
 The two examples used here are PDK packages built into the Hdl21 source tree: 
 the ASAP7 academic predictive kit, and the Skywater 130nm open-source PDK. 
 
 """
 
 from pathlib import Path
+import os
 
 # Sky 130
-import sky130
+import sky130_hdl21
 
-sky130.install = sky130.Install(
-    model_lib=Path("pdks") / "sky130" / ... / "sky130.lib.spice"
+sky130_hdl21.install = sky130_hdl21.Install(
+    pdk_path=Path(os.environ["PDK_ROOT"] + "/" + os.environ["PDK"]),
+    lib_path=Path("libs.tech/ngspice/sky130.lib.spice"),
+    model_ref=Path("libs.ref/sky130_fd_pr/spice"),
 )
 
 # ASAP7
-import asap7
+import asap7_hdl21
 
-asap7.install = asap7.Install(model_lib=Path("pdks") / "asap7" / ... / "7nm_TT.pm")
+# FIXME: Complete implementation
+# asap7_hdl21.install = asap7_hdl21.Install(Path("pdks") / "asap7" / "..." / "7nm_TT.pm")
+
+# GF180
+import gf180_hdl21
+
+gf180_hdl21.install = gf180_hdl21.Install(
+    model_lib=Path("/usr/local/share/pdk/gf180mcuC/libs.tech/ngspice/sm141064.ngspice")
+)
```

### Comparing `hdl21-3.0.dev3/examples/__init__.py` & `hdl21-4.0.0rc0/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `hdl21-3.0.dev3/examples/encoder.py` & `hdl21-4.0.0rc0/examples/encoder.py`

 * *Files identical despite different names*

### Comparing `hdl21-3.0.dev3/examples/rdac.py` & `hdl21-4.0.0rc0/examples/rdac.py`

 * *Files identical despite different names*

### Comparing `hdl21-3.0.dev3/examples/ro.py` & `hdl21-4.0.0rc0/examples/ro.py`

 * *Files identical despite different names*

### Comparing `hdl21-3.0.dev3/hdl21/__init__.py` & `hdl21-4.0.0rc0/hdl21/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,62 @@
 """ 
 # Hdl21 Hardware Description Library 
 """
 
-__version__ = "2.0.dev0"
+__version__ = "4.0.0rc0" # NOTE: VLSIR_VERSION
 
 
 # Before any real importing, ensure we can instantiate non-pydantic types in type-checked dataclasses.
 # This `Config` seems to be shared for *all* pydantic types, even when not applied to `BaseModel`.
 from pydantic import BaseModel
 
 BaseModel.Config.arbitrary_types_allowed = True
 
 # Internal (python) module aliases, overridden by names such as the `module` decorator function.
 from . import module as _module_module
+from . import bundle as _bundle_module
 from . import external_module as _external_module_module
 from . import instance as _instance_module
 from . import generator as _generator_module
 
+from . import params
 from .params import *
+
 from .instance import *
 from .signal import *
 from .slice import *
 from .concat import *
 from .noconn import *
 from .external_module import *
 from .module import *
 from .generator import *
-from .generators import *
-from .primitives import *
 from .bundle import *
+from .role import *
 from .netlist import *
-from .elab import *
-from .walker import HierarchyWalker
 from .instantiable import *
 from .diff_pair import *
-from . import prefix
-from .prefix import Prefix, Prefixed
+from .props import Properties
 from .scalar import Scalar
 from .literal import Literal
+
+from . import primitives
+from .primitives import *
+
+from . import prefix
+from .prefix import Prefix, Prefixed
+
+# Import these as modules, but not their contents
+from . import generators
 from . import sim
+from . import pdk
 from . import proto
 from .proto import to_proto, from_proto
 
+from .walker import HierarchyWalker
+
+from . import elab
+from .elab import *
+
 # Update all the forward type-references throughout our many `@datatype`s
 from .datatype import _update_forward_refs
 
 _update_forward_refs()
```

### Comparing `hdl21-3.0.dev3/hdl21/bundle.py` & `hdl21-4.0.0rc0/hdl21/bundle.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 """ 
 # `hdl21.Bundle` and Related Classes 
 
 Structured connection objects, instances thereof, and associated utilities.
 """
 
+# Std-Lib Imports
+import warnings
+from copy import copy
 from enum import Enum, EnumMeta
 from typing import Optional, Union, Any, Dict, Set, List, ClassVar
 
 # Local Imports
-from .attrmagic import init
+from . import attrmagic
+from .role import Role, RoleSet
 from .connect import connectable, is_connectable
 from .sliceable import sliceable
 from .concat import concatable
 from .signal import Signal
+from .visibility import Visibility
+from .props import Properties
 
 
 def getattr_bundle_refs(cls: type) -> type:
     """Decorator to add the "__getattr__ generates BundleRefs" functionality to `cls`.
     Adds the `_bundle_ref` method and `__getattr__` access to it."""
 
     # First check and fail if any of the methods to be defined here are already defined elsewhere
@@ -56,159 +62,261 @@
 def has_getattr_bundle_refs(obj: Any) -> bool:
     """Boolean indication of "getattr bundle refs" functionality"""
     return getattr(obj, "__getattr_bundle_refs__", False)
 
 
 @getattr_bundle_refs
 @connectable
-@init
+@attrmagic.only_set_known_attrs
+@attrmagic.init
 class BundleInstance:
     """# Instance of a `Bundle`
     Generally in a `Module` or another `Bundle`"""
 
     _specialcases = [
         "name",
         "of",
         "port",
         "role",
         "src",
         "dest",
         "desc",
+        "props",
         "refs_to_me",
     ]
 
     def __init__(
         self,
         *,
         name: Optional[str] = None,
         of: "Bundle",
         port: bool = False,
-        role: Optional[Enum] = None,
-        src: Optional[Enum] = None,
-        dest: Optional[Enum] = None,
+        flipped: bool = False,
+        role: Union[Role, Enum, None] = None,
+        src: Union[Role, Enum, None] = None,
+        dest: Union[Role, Enum, None] = None,
         desc: Optional[str] = None,
     ):
         self.name = name
         self.of = of
-        self.port = port
+        self.port = port  # FIXME: make this a `Visibility`
+        self.flipped = flipped
         self.role = role
         self.src = src
         self.dest = dest
         self.desc = desc
         # References handed out to our children
         self.refs_to_me: Dict[str, "BundleRef"] = dict()
+        self.props: Properties = Properties()
         # Connected port references
         self._connected_ports: Set["PortRef"] = set()
         self._parent_module: Optional["Module"] = None
         self._elaborated = False
         self._initialized = True
 
     @property
     def _resolved(self) -> "Bundle":
         return self.of
 
+    """ Special Methods """
+
     def __repr__(self):
         return f"{self.__class__.__name__}(name={self.name} of={self.of})"
 
+    def __rmul__(self, num: int) -> List["Self"]:
+        """# Right multiplication. Creates `num` copies of ourselves."""
+        if not isinstance(num, int):
+            return NotImplemented
+        return [copy(self) for _ in range(num)]
+
 
 # Type-alias for HDL objects storable as `Module` attributes
 BundleAttr = Union[Signal, BundleInstance]
 
 
 def is_bundle_attr(val: Any) -> bool:
     """Boolean indication of whether `val` is a valid `hdl21.Bundle` attribute."""
     return isinstance(val, BundleAttr.__args__)
 
 
-@init
+def assert_bundle_attr(b: "Bundle", val: Any) -> None:
+    """Raise a TypeError if `val` is not a valid attribute."""
+    if not is_bundle_attr(val):
+        msg = f"Invalid attribute {val} added to {b}"
+        raise TypeError(msg)
+
+
+_banned = ["signals", "bundles", "namespace"]
+
+
+@attrmagic.init
 class Bundle:
     """
     # hdl21 Bundle
 
     Bundles are structured hierarchical connection objects which include Signals and other Bundles.
     """
 
-    def __init__(self, *, name=None):
-        self.name = name
-        self.roles = None
-        self.signals = dict()
-        self.bundles = dict()
-        self.namespace = dict()  # Combination of all these
-        self._elaborated = False
-        self._initialized = True
+    def __init__(self, *, name: Optional[str] = None):
+        self.name: Optional[str] = name
+        self.roles: Optional[RoleSet] = None
+        self.signals: Dict[str, "Signal"] = dict()
+        self.bundles: Dict[str, "BundleInstance"] = dict()
+        self.namespace: Dict[str, "BundleAttr"] = dict()  # Combination of all these
+        self.props: Properties = Properties()
+        self._elaborated = (
+            False  # FIXME: unify whether these are boolean, or Optional objects
+        )
+        self._initialized = True  # Done running __init__, enable some magic
+
+    """
+    The public `Bundle` API. Just `add` and `get`. 
+    To keep the space of valid names for post-fix dot access as large as possible, 
+    the `Bundle` class namespace is kept *as small* as possible. 
+    """
+
+    def add(self, val: BundleAttr, *, name: Optional[str] = None) -> BundleAttr:
+        """Add a Bundle attribute.
+
+        `Bundle.add` allows for programmatic insertion of attributes whose names are not legal Python identifiers,
+        such as keywords ('in', 'from') and those including invalid characters.
+
+        The added object `val` is also provided as the return value, enabling chaining-style usages such as
+        ```python
+        instance.inp = MyBundle.add(h.Input(name="in", width=5))
+        ```
+        and similar.
+
+        Attribute naming comes from one of either:
+        * `val`'s `name` attribute, if it has one, or
+        * The optional `name` argument.
+        Only one of the two name-sources is allowed per call.
+        """
+
+        # Check it's a valid attribute-type
+        assert_bundle_attr(self, val)
+
+        # Now sort out naming. We get two name-sources:
+        # (a) the function-argument `name` and (b) the value's `name` attribute.
+        # One or the other (and not both) must be set.
+        if name is None and val.name is None:  # Neither set, fail.
+            msg = f"Anonymous attribute {val} cannot be added to Bundle {self.name}"
+            raise RuntimeError(msg)
+        if name is not None and val.name is not None:  # Both set, fail.
+            msg = f"{val} with conflicting names {name} and {val.name} cannot be added to Bundle {self.name}"
+            raise RuntimeError(msg)
+        if name is not None:  # One or the other set - great.
+            val.name = name
+
+        # Now `val.name` is set appropriately.
+        # Add it to our type-based containers, and return it.
+        return _add(bundle=self, val=val)
+
+    def get(self, name: str) -> Optional[BundleAttr]:
+        """Get attribute `name`. Returns `None` if not present.
+        Note unlike Python built-ins such as `getattr`, `get` returns solely
+        from the HDL namespace-worth of `BundleAttr`s."""
+        ns = self.__getattribute__("namespace")
+        return ns.get(name, None)
+
+    @property
+    def Roles(self):
+        """# Roles Accessor Property"""
+        # Roles often look like a class, so they have a class-style name-accessor
+        return self.roles
 
-    def __setattr__(self, key: str, val: object):
+    """
+    Special Methods
+    """
+
+    def __setattr__(self, key: str, val: Any) -> None:
         """Set-attribute over-ride, organizing into type-based containers"""
-        from .signal import Signal
 
-        if not getattr(self, "_initialized", False) or key.startswith("_"):
+        if key.startswith("_") or not getattr(self, "_initialized", False):
+            # Bootstrapping phase. Pass along to "regular" setattr.
             return super().__setattr__(key, val)
 
-        # Protected attrs - the internal dicts
-        banned = ["signals", "bundles", "namespace"]
-        if key in banned:
-            msg = f"Error attempting to over-write protected attribute {key} of Bundle {self}"
+        if key in _banned:
+            msg = f"Error attempting to over-write protected attribute {key} of Module {self}"
             raise RuntimeError(msg)
         # Special case(s)
         if key == "name":
             return super().__setattr__(key, val)
         if key == "roles":
-            if not isinstance(val, EnumMeta):
-                raise TypeError(f"Bundle roles must be an `enum.Enum`")
+            if isinstance(val, EnumMeta):
+                # FIXME: deprecation warning and inline conversion here for now!
+                msg = f"Bundle roles should be a `RoleSet`. Use `RoleSet.from_enum` to convert an `Enum` class!"
+                warnings.warn(DeprecationWarning(msg))
+                val = RoleSet.from_enum(val)
+            if not isinstance(val, RoleSet):
+                raise TypeError(f"Bundle roles must be an `RoleSet`, not {val}")
+
             return super().__setattr__(key, val)
 
-        # Type-based organization
-        if isinstance(val, Signal):
-            val.name = key
-            self.namespace[key] = val
-            self.signals[key] = val
-        elif isinstance(val, BundleInstance):
-            val.name = key
-            self.bundles[key] = val
-            self.namespace[key] = val
-        else:
-            raise TypeError(f"Invalid Bundle attribute {val} for {self}")
+        # Check it's a valid attribute-type
+        assert_bundle_attr(self, val)
+
+        # Checks out! Name `val` and add it to our type-based containers.
+        val.name = key
+        _add(bundle=self, val=val)
+        return None
 
     def __getattr__(self, key):
         ns = self.__getattribute__("namespace")
         if key in ns:
             return ns[key]
         return object.__getattribute__(self, key)
 
     def __call__(self, **kwargs):
         """Calls to Bundles return Bundle Instances"""
         return BundleInstance(of=self, **kwargs)
 
-    def __init_subclass__(cls, *_args, **_kwargs):
+    def __init_subclass__(cls, *_, **__):
         """Sub-Classing Disable-ization"""
         msg = f"Error attempting to create {cls.__name__}. Sub-Typing hdl21.Bundle is not supported."
         raise RuntimeError(msg)
 
-    def add(self, val: BundleAttr, *, name: Optional[str] = None) -> BundleAttr:
-        raise NotImplementedError  # FIXME!
-
-    def get(self, name: str) -> Optional[BundleAttr]:
-        """Get module-attribute `name`. Returns `None` if not present.
-        Note unlike Python built-ins such as `getattr`, `get` returns solely
-        from the HDL namespace-worth of `BundleAttr`s."""
-        ns = self.__getattribute__("namespace")
-        return ns.get(name, None)
-
-    @property
-    def Roles(self):
-        """Roles-Enumeration Accessor Property"""
-        # Roles often look like a class, so they have a class-style name-accessor
-        return self.roles
-
     def __repr__(self) -> str:
         if self.name:
             return f"Bundle(name={self.name})"
         return f"Bundle(_anon_)"
 
 
+def _add(bundle: Bundle, val: BundleAttr) -> BundleAttr:
+    """Internal `Module.add` and `Module.__setattr__` implementation.
+    Primarily sort `val` into one of our type-based containers.
+    Layers above `_add` must ensure that `val` has its `name` attribute before calling this method."""
+
+    if bundle._elaborated:  ## FIXME: is not None:
+        raise RuntimeError(f"Cannot add {val} to {bundle} after elaboration.")
+
+    # Sort out which of our type-based containers to add `val` to.
+    if isinstance(val, Signal):
+        type_ctr = bundle.signals
+    elif isinstance(val, BundleInstance):
+        type_ctr = bundle.bundles
+    elif isinstance(val, Role):
+        type_ctr = bundle.roles.inner
+    else:
+        # The next line *should* never be reached, as outer layers should have checked `_is_bundle_attr`.
+        # Nonetheless gotta raise an error if we get here, somehow.
+        msg = f"Invalid Bundle attribute {val} for {bundle}"
+        raise TypeError(msg)
+
+    # Add it to the bundle namespace, and the type-specific container
+    type_ctr[val.name] = val
+    bundle.namespace[val.name] = val
+
+    # Give it a reference to us
+    val._parent_bundle = bundle
+
+    # And return our newly-added attribute
+    return val
+
+
 def bundle(cls: type) -> Bundle:
     """# Bundle Definition Decorator
 
     Converts a class-body full of Bundle-storable attributes (Signals, other Bundles) to an `hdl21.Bundle`.
     Example Usage:
 
     ```python
@@ -253,31 +361,46 @@
     # Create the Bundle object
     bundle = Bundle(name=cls.__name__)
 
     protected_names = ["signals", "bundles"]
     # Any class-body content that isn't a `ModuleAttr` will be "forgotten" from the `Module` definition.
     # This can nonetheless be handy for defining intermediate values upon which the ultimate Module attributes depend.
     forgetme: List[Any] = list()
+    # Collect a list of all declared `Role`s
+    roles_dict: Dict[str, Role] = dict()
 
     # Take a lap through the class dictionary, type-check everything and assign relevant attributes to the bundle
     for key, val in cls.__dict__.items():
         if key in protected_names:
             raise RuntimeError(f"Invalid field name {key} in bundle {cls}")
         elif key == "roles" or key == "Roles":
             # Special-case the upper-cased `Roles`, as it'll often be a class-def
             setattr(bundle, "roles", val)
+        elif isinstance(val, Role):
+            roles_dict[key] = val
         elif is_bundle_attr(val):
             setattr(bundle, key, val)
         else:  # Add to the forget-list
             forgetme.append(val)
 
+    # Sort out the role definitions.
+    # This can come either from a single `roles`/`Roles` attribute, or from a list of `Role`s, but not both.
+    if roles_dict:
+        if bundle.roles is not None:
+            msg = f"Error attempting to define roles for {bundle} when it already has roles {bundle.roles}"
+            raise RuntimeError(msg)
+        # Defined via list. Convert to a `RoleSet`.
+        bundle.roles = RoleSet.from_dict(roles_dict)
+
     # And return the bundle
     return bundle
 
 
+@attrmagic.no_setattr
+@attrmagic.init
 @connectable
 class AnonymousBundle:
     """# Anonymous Connection Bundle
     Commonly used for "collecting" Signals into `h.Bundle`s,
     or for re-jiggering connections between `h.Bundle`s."""
 
     def __init__(self, **kwargs: Dict[str, "Connectable"]):
@@ -287,14 +410,16 @@
         # Connected port references
         self._connected_ports: Set["PortRef"] = set()
 
         # And add each keyword-arg
         for key, val in kwargs.items():
             self.add(key, val)
 
+        self._initialized = True
+
     def add(self, name: str, val: BundleAttr) -> BundleAttr:
         """Add attribute `val` to our namespace."""
 
         if name in self._namespace:
             raise RuntimeError(f"Duplicate attribute {name} in {self}")
         if not is_connectable(val):
             raise TypeError(f"Invalid Bundle attribute {val} for {self}")
@@ -314,15 +439,16 @@
     return AnonymousBundle(**kwargs)
 
 
 @getattr_bundle_refs
 @concatable
 @sliceable
 @connectable
-@init
+@attrmagic.only_set_known_attrs
+@attrmagic.init
 class BundleRef:
     """Reference into a Bundle Instance"""
 
     _specialcases: ClassVar[List[str]] = [
         "parent",
         "attrname",
         "path",
@@ -361,23 +487,23 @@
 
     def path(self) -> List[str]:
         """Get the path to this potentially nested reference."""
         if isinstance(self.parent, BundleRef):
             return self.parent.path() + [self.attrname]
         if isinstance(self.parent, BundleInstance):
             return [self.attrname]
-        raise TypeError
+        raise TypeError(f"Invalid parent {self.parent} for {self}")
 
     def root(self) -> "BundleInstance":
         """Get the root `BundleInstance` of this potentially nested reference."""
         if isinstance(self.parent, BundleRef):
             return self.parent.root()
         if isinstance(self.parent, BundleInstance):
             return self.parent
-        raise TypeError
+        raise TypeError(f"Invalid parent {self.parent} for {self}")
 
     def __repr__(self):
         return f"{self.__class__.__name__}(root={self.root()} path={self.path()})"
 
 
 def _bundle_ref(self: Union[BundleRef, BundleInstance], key: str) -> BundleRef:
     """Return a reference to name `key`, creating it if necessary."""
@@ -387,7 +513,36 @@
     if key in bundle_refs:
         return bundle_refs[key]
 
     # New reference; create, add, and return it
     bundle_ref = BundleRef(parent=self, attrname=key)
     bundle_refs[key] = bundle_ref
     return bundle_ref
+
+
+def flippable(b: Bundle) -> bool:
+    """
+    # Boolean indication of whether a Bundle is flippable.
+    Requires that all Signals in the Bundle,
+    and all Signals in all its sub-bundles, have port-visibility.
+    """
+    return all([s.vis == Visibility.PORT for s in b.signals.values()]) and all(
+        [flippable(bi.of) for bi in b.bundles.values()]
+    )
+
+
+def flipped(bi: BundleInstance) -> BundleInstance:
+    """# Create a flipped copy of a BundleInstance"""
+    cp = copy(bi)
+    cp.flipped = not cp.flipped
+    return cp
+
+
+__all__ = [
+    "Bundle",
+    "bundle",
+    "BundleInstance",
+    "AnonymousBundle",
+    "bundlize",
+    "flipped",
+    "BundleRef",  # FIXME: remove
+]
```

### Comparing `hdl21-3.0.dev3/hdl21/call.py` & `hdl21-4.0.0rc0/hdl21/call.py`

 * *Files identical despite different names*

### Comparing `hdl21-3.0.dev3/hdl21/concat.py` & `hdl21-4.0.0rc0/hdl21/concat.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-"""
-# Hdl21 Concatenations 
-"Sequences" of Signals and other Connectable objects. 
-"""
-
+# Std-Lib Imports
 from typing import Optional, Set
 
 # Local imports
+from . import attrmagic
 from .connect import connectable
 from .sliceable import sliceable
 from .concatable import concatable, is_concatable
 
 
+@attrmagic.only_set_known_attrs
+@attrmagic.init
 @sliceable
 @concatable
 @connectable
 class Concat:
-    """Signal Concatenation
-    Uses *Python-convention* ordering, in which "LSBs", i.e. index 0, are specified first."""
+    """
+    # Signal Concat(enations)
+    "Sequences" of Signals and other Connectable objects.
+    Uses *Python-convention* ordering, in which "LSBs", i.e. index 0, are specified first.
+    """
 
     def __init__(self, *parts):
         invalid_parts = [p for p in parts if not is_concatable(p)]
         if invalid_parts:
             raise TypeError(f"Invalid `Concat` of {invalid_parts}")
 
         for part in parts:
@@ -30,18 +32,19 @@
         self.parts = tuple(parts)
 
         # Inner management data
         self._connected_ports: Set["PortRef"] = set()
         self._width: Optional[int] = None
         self._slices: Set["Slice"] = set()
         self._concats: Set["Concat"] = set()
+        self._initialized = True
 
     def __eq__(self, other) -> bool:
         # Identity is equality
-        return id(self) == id(other)
+        return other is self
 
     def __hash__(self) -> bool:
         # Identity is equality
         return hash(id(self))
 
     def __repr__(self):
         return f"Concat(parts={len(self.parts)})"
@@ -51,8 +54,9 @@
         # FIXME: whether to keep me around as a property
         # As is the elaboration mechanics do not use this property, but users may.
         from .elab.elaborators.width import width
 
         return width(self)
 
 
+__doc__ = Concat.__doc__
 __all__ = ["Concat"]
```

### Comparing `hdl21-3.0.dev3/hdl21/concatable.py` & `hdl21-4.0.0rc0/hdl21/concatable.py`

 * *Files identical despite different names*

### Comparing `hdl21-3.0.dev3/hdl21/connect.py` & `hdl21-4.0.0rc0/hdl21/connect.py`

 * *Files identical despite different names*

### Comparing `hdl21-3.0.dev3/hdl21/datatype.py` & `hdl21-4.0.0rc0/hdl21/datatype.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,29 +23,34 @@
   * Importing this function into other packages is therefore highly discouraged. (Copying it is quite easy though.) 
 * `@datatype` only works on modules which are imported before `_update_forward_refs()` is run. 
   * Generally this means modules which are imported as part of `__init__.py`
 * `@datatype` is designed solely to work on `pydantic.dataclasses.dataclass`es. 
   * Notable exceptions include *union types* thereof, which do not have the necessary fields/ methods. 
 """
 
+from pydantic import Extra
 from pydantic.dataclasses import dataclass
-from typing import TypeVar, Type
+from typing import TypeVar, Type, Any
 
 # The list of defined datatypes
 datatypes = []
 
 T = TypeVar("T")
 
 
+class Config:  # Pydantic Model Config
+    allow_extra = Extra.forbid
+
+
 def datatype(cls: Type[T]) -> Type[T]:
     """Register a class as a datatype."""
 
     # Convert `cls` to a `pydantic.dataclasses.dataclass`,
     # and add it to the list of datatypes
-    cls = dataclass(cls)
+    cls = dataclass(cls, config=Config)
     datatypes.append(cls)
     return cls
 
 
 def _update_forward_refs():
     """Update all the forward type-references"""
     for tp in datatypes:
```

### Comparing `hdl21-3.0.dev3/hdl21/default.py` & `hdl21-4.0.0rc0/hdl21/default.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,12 +13,10 @@
     """
     # Default Value Sentinel
 
     Used by a number of Hdl21 types to indicate a default value,
     where all other "public" values could be valid non-default data.
     """
 
-    ...  # Empty contents
-
-    def __new__(cls, *args, **kwargs):
+    def __new__(cls, *_, **__):
         # And we're a singleton. Call away, you get the same class-object back.
         return Default
```

### Comparing `hdl21-3.0.dev3/hdl21/diff_pair.py` & `hdl21-4.0.0rc0/hdl21/diff_pair.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,24 +5,30 @@
 # Std-Lib Imports
 from enum import Enum, auto
 
 # Local imports
 from .signal import Signals
 from .instance import InstanceBundleType
 from .bundle import bundle, AnonymousBundle
+from .role import RoleSet
+
+
+class SourceSink(Enum):
+    SOURCE = auto()
+    SINK = auto()
+
+
+SourceSink = RoleSet.from_enum(SourceSink)
 
 
 @bundle
 class Diff:
-    """Differential Bundle"""
-
-    class Roles(Enum):
-        SOURCE = auto()
-        SINK = auto()
+    """# Differential Bundle"""
 
+    Roles = SourceSink
     p, n = Signals(2, src=Roles.SOURCE, dest=Roles.SINK)
 
 
 def inverse(d: Diff) -> AnonymousBundle:
     """Create a Bundle with the same signals as `d`, but with `p` and `n` reversed."""
     return AnonymousBundle(p=d.n, n=d.p)
```

### Comparing `hdl21-3.0.dev3/hdl21/elab/context.py` & `hdl21-4.0.0rc0/hdl21/elab/context.py`

 * *Files identical despite different names*

### Comparing `hdl21-3.0.dev3/hdl21/elab/elab.py` & `hdl21-4.0.0rc0/hdl21/elab/elab.py`

 * *Files identical despite different names*

### Comparing `hdl21-3.0.dev3/hdl21/elab/elaborators/arrays.py` & `hdl21-4.0.0rc0/hdl21/elab/elaborators/arrays.py`

 * *Files identical despite different names*

### Comparing `hdl21-3.0.dev3/hdl21/elab/elaborators/base.py` & `hdl21-4.0.0rc0/hdl21/elab/elaborators/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,18 +88,14 @@
         `elaborate_module_base` instead.
         """
 
         # Check if this has already been elaborated
         if module._elaborated is not None:
             return module._elaborated
 
-        if not module.name:
-            msg = f"Anonymous Module {module} cannot be elaborated (did you forget to name it?)"
-            self.fail(msg)
-
         self.stack.append(module)
 
         # Depth-first traverse instances, ensuring their targets are defined
         for inst in module.instances.values():
             self.elaborate_instance_base(inst)
         for arr in module.instarrays.values():
             self.elaborate_instance_base(arr)
@@ -192,15 +188,17 @@
     def format_hier_path(self) -> List[str]:
         """Create a list of lines describing the current hierarchy path
         Generally intended for debug use, especially in error messages."""
 
         lines = []
         for s in self.stack:
             # Format: `  Module          MyModule      `
-            line = "  " + type(s).__name__.ljust(14) + str(s.name).ljust(28)
+            s_name = s.name or ""
+            # Filter out None-valued names, common during elaboration errors.
+            line = "  " + type(s).__name__.ljust(14) + s_name.ljust(28)
 
             source_info = getattr(s, "_source_info", None)
             if source_info is not None:
                 # The entry has source/line info. Add it to the error line.
 
                 # For source-paths in the run-directory, print the (presumably shorter) relative-path only
                 filepath = source_info.filepath
```

### Comparing `hdl21-3.0.dev3/hdl21/elab/elaborators/conntypes.py` & `hdl21-4.0.0rc0/hdl21/elab/elaborators/conntypes.py`

 * *Files identical despite different names*

### Comparing `hdl21-3.0.dev3/hdl21/elab/elaborators/flatten_bundles.py` & `hdl21-4.0.0rc0/hdl21/elab/elaborators/flatten_bundles.py`

 * *Files 3% similar despite different names*

```diff
@@ -182,31 +182,14 @@
         # Add each flattened Signal. Note flattened Signals are modified in-place.
         for pathstr, sig in flat.signals.items():
             # Rename the signal, prepending the bundle-instance's name
             sig.name = self.flatname(
                 segments=[bundle_inst.name, pathstr.to_name()],
                 avoid=module.namespace,
             )
-            # Sort out the new Signal's visibility and direction
-            if bundle_inst.port:
-                vis_ = Visibility.PORT
-                if bundle_inst.role is None:
-                    dir_ = PortDir.NONE
-                elif bundle_inst.role == sig.src:
-                    dir_ = PortDir.OUTPUT
-                elif bundle_inst.role == sig.dest:
-                    dir_ = PortDir.INPUT
-                else:
-                    dir_ = PortDir.NONE
-            else:
-                vis_ = Visibility.INTERNAL
-                dir_ = PortDir.NONE
-            # Apply all these attributes to our new Signal
-            sig.vis = vis_
-            sig.direction = dir_
             # And add it to the Module namespace
             module.add(sig)
 
         # Store the result in our caches
         THE_CACHE.bundle_insts[id(bundle_inst)] = flat
         if bundle_inst.port:
             entry = BundlePortEntry(module, bundle_inst.name)
@@ -299,31 +282,87 @@
                 msg += f"but no `{path}`."
                 self.fail(msg)
             inst.connect(flat_port.name, flat.signals[path])
 
     def flatten_bundle_inst(
         self, bundle_inst: BundleInstance, path: Path
     ) -> BundleScope:
+        """# Flatten a bundle instance"""
+        # Kick off recursive flattening
+        return self.flatten_bundle_inst_helper(
+            bundle_inst=bundle_inst,
+            path=path,
+            is_this_top_level=True,
+            is_port=bundle_inst.port,
+            flip_state=bundle_inst.flipped,
+        )
+
+    def flatten_bundle_inst_helper(
+        self,
+        bundle_inst: BundleInstance,
+        path: Path,
+        is_this_top_level: bool,
+        is_port: bool,
+        flip_state: bool,
+    ) -> BundleScope:
+        """Recursive inner implementation of `flatten_bundle_inst`."""
 
         bundle_def = bundle_inst.of
         scope = BundleScope(src=bundle_inst)
 
         # Copy each scalar signal, retaining its original name as the key in `scope.signals`
         for sig in bundle_def.signals.values():
             signal_path = Path([sig.name])
             if signal_path in scope.signals:
                 self.fail(f"Doubly defined Signal {sig} in {bundle_inst}")
             newsig = copy.deepcopy(sig)
             newsig.name = signal_path.to_name()
+
+            # Sort out the new Signal's visibility and direction
+            if is_port:  # "Port-ness" applies to the entire top-level bundle instance
+                vis_ = Visibility.PORT
+
+                # If the Signal is declared as a port, look at its direction and our flip state
+                if newsig.vis == Visibility.PORT:
+                    if flip_state:  # Flip direction
+                        dir_ = newsig.direction.flipped()
+                    else:  # Not flipped; leave unchanged
+                        dir_ = newsig.direction
+
+                # If the Signal is not a port, look at its source and dest roles.
+                elif bundle_inst.role is None:
+                    dir_ = PortDir.NONE
+                elif bundle_inst.role == newsig.src:
+                    dir_ = PortDir.OUTPUT
+                elif bundle_inst.role == newsig.dest:
+                    dir_ = PortDir.INPUT
+                else:  # Some other Role
+                    dir_ = PortDir.NONE
+            else:
+                vis_ = Visibility.INTERNAL
+                dir_ = PortDir.NONE
+
+            # Apply all these attributes to our new Signal
+            newsig.vis = vis_
+            newsig.direction = dir_
             scope.signals[signal_path] = newsig
 
         # And recursively do this to all sub-bundle instances, adding them to `scopes` along the way.
         for sub_bundle_inst in bundle_def.bundles.values():
             subpath = path.append(Path([sub_bundle_inst.name]))
-            subscope = self.flatten_bundle_inst(sub_bundle_inst, subpath)
+            sub_flip_state = (
+                flip_state if not sub_bundle_inst.flipped else not flip_state
+            )
+            subscope = self.flatten_bundle_inst_helper(
+                bundle_inst=sub_bundle_inst,
+                path=subpath,
+                is_this_top_level=False,
+                is_port=is_port,  # Port-ness is defined from the top-level BundleInstance
+                flip_state=sub_flip_state,  # Flip-state can be inverted at each level
+            )
             scope.add_subscope(name=sub_bundle_inst.name, scope=subscope)
 
         return scope
 
     def replace_anon_bundle_conn(
         self, inst: Instance, portname: str, anon: AnonymousBundle
     ):
```

### Comparing `hdl21-3.0.dev3/hdl21/elab/elaborators/generators.py` & `hdl21-4.0.0rc0/hdl21/elab/elaborators/generators.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,29 +85,30 @@
             if call.gen.usecontext:
                 m = call.gen.func(call.params, self.ctx)
             else:
                 m = call.gen.func(call.params)
         except Exception as e:
             self.fail(f"{call.gen} raised an exception: \n{e}")
 
-        # Give the result a reference bay to the generating `Call`
         if isinstance(m, Module):
+            # Give the result a reference back to the generating `Call`
             m._generated_by = call
 
+            # And elaborate the module
+            m = self.elaborate_module_base(m)  # Note the `_base` here!
+
             # If the Module that comes back is anonymous, start by giving it a name equal to the Generator's
             if m.name is None:
                 m.name = call.gen.func.__name__
 
             # Then add a unique suffix per its parameter-values
+            # Note this part may require that `m` has been through elaboration above!
             if not isinstance(call.params, HasNoParams):
                 m.name += "(" + _unique_name(call.params) + ")"
 
-            # And elaborate the module
-            m = self.elaborate_module_base(m)  # Note the `_base` here!
-
         # Generators may return other (potentially nested) generator-calls; recursively unwind any of them
         # Note this should hit Python's recursive stack-check if it doesn't terminate
         elif isinstance(m, GeneratorCall):
             m._generated_by = call
             m: Module = self.elaborate_generator_call(m)
 
         # Type-check the result.
```

### Comparing `hdl21-3.0.dev3/hdl21/elab/elaborators/inst_bundles.py` & `hdl21-4.0.0rc0/hdl21/elab/elaborators/inst_bundles.py`

 * *Files identical despite different names*

### Comparing `hdl21-3.0.dev3/hdl21/elab/elaborators/orphanage.py` & `hdl21-4.0.0rc0/hdl21/elab/elaborators/orphanage.py`

 * *Files identical despite different names*

### Comparing `hdl21-3.0.dev3/hdl21/elab/elaborators/portrefs.py` & `hdl21-4.0.0rc0/hdl21/elab/elaborators/portrefs.py`

 * *Files identical despite different names*

### Comparing `hdl21-3.0.dev3/hdl21/elab/elaborators/resolve_ref_types.py` & `hdl21-4.0.0rc0/hdl21/elab/elaborators/resolve_ref_types.py`

 * *Files identical despite different names*

### Comparing `hdl21-3.0.dev3/hdl21/elab/elaborators/slices.py` & `hdl21-4.0.0rc0/hdl21/elab/elaborators/slices.py`

 * *Files identical despite different names*

### Comparing `hdl21-3.0.dev3/hdl21/elab/elaborators/width.py` & `hdl21-4.0.0rc0/hdl21/elab/elaborators/width.py`

 * *Files identical despite different names*

### Comparing `hdl21-3.0.dev3/hdl21/elab/elabpass.py` & `hdl21-4.0.0rc0/hdl21/elab/elabpass.py`

 * *Files identical despite different names*

### Comparing `hdl21-3.0.dev3/hdl21/external_module.py` & `hdl21-4.0.0rc0/hdl21/external_module.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 
 Wrapper for circuits defined outside Hdl21. 
 """
 
 from typing import Any, Optional, List, Type, Dict
 from pydantic.dataclasses import dataclass
 
+# VLSIR Imports
+from vlsirtools import SpiceType
+
 # Local imports
+from .datatype import datatype
 from .default import Default
 from .call import param_call
 from .source_info import source_info, SourceInfo
-from .params import HasNoParams, isparamclass
+from .params import HasNoParams, isparamclass, _unique_name
 from .signal import Signal, Visibility
 from .instance import calls_instantiate
-from .qualname import qualname_magic_methods
 
 
-@dataclass
-@qualname_magic_methods
+@datatype
 class ExternalModule:
     """
     # External Module
 
     Wrapper for circuits defined outside Hdl21, such as:
     * Inclusion of existing SPICE or Verilog netlists
     * Foundry or technology-specific primitives
@@ -32,17 +34,18 @@
     Each `ExternalModule` stores a parameter-type field `paramtype`.
     Parameter types may be either `hdl21.paramclass`es or the built-in `dict`.
     Parameter-values are checked to be instances of `paramtype` at creation time.
     """
 
     name: str  # Module name. Used *directly* when exporting.
     port_list: List[Signal]  # Ordered Ports
-    paramtype: Type = HasNoParams  # Parameter-type `paramclass`
+    paramtype: Type[object] = HasNoParams  # Parameter-type `paramclass`
     desc: Optional[str] = None  # Description
     domain: Optional[str] = None  # Domain name, for references upon export
+    spicetype: SpiceType = SpiceType.SUBCKT  # Spice type, for SPICE export
 
     @property
     def ports(self) -> dict:
         """Port dictionary, from name to `Signal`."""
         return {p.name: p for p in self.port_list}
 
     @property
@@ -68,37 +71,60 @@
                 raise ValueError(f"Unnamed Primitive Port {p} for {self.name}")
             if p.vis != Visibility.PORT:
                 msg = f"Invalid Primitive Port {p.name} on {self.name}; must have PORT visibility"
                 raise ValueError(msg)
 
     def __call__(self, arg: Any = Default, **kwargs) -> "ExternalModuleCall":
         """Call to set an `ExternalModule`'s parameters.
-        Returns an `ExternalModuleCall` combining the `ExternalModule` and parameter values."""
+        Returns an `ExternalModuleCall` combining the `ExternalModule` and parameter values.
+        """
         params = param_call(callee=self, arg=arg, **kwargs)
         return ExternalModuleCall(module=self, params=params)
 
+    def __eq__(self, other) -> bool:
+        # Identity is equality
+        return other is self
+
+    def __hash__(self) -> bool:
+        # Identity is equality
+        return hash(id(self))
+
 
 @calls_instantiate
 @dataclass
 class ExternalModuleCall:
     """# External Module Call
-    A combination of an `ExternalModule` and its Parameter-values, typically generated by calling the `ExternalModule`."""
+    A combination of an `ExternalModule` and its Parameter-values, typically generated by calling the `ExternalModule`.
+    """
 
     module: ExternalModule
     params: Any
 
     def __post_init_post_parse__(self):
         # Type-validate our parameters
         if not isinstance(self.params, self.module.paramtype):
             msg = f"Invalid parameter type {type(self.params)} for ExternalModule {self.module.name}. Must be {self.module.paramtype}"
             raise TypeError(msg)
 
     @property
-    def name(self) -> Optional[str]:
-        return self.module.name
+    def name(self) -> str:
+        return self.module.name + "(" + _unique_name(self.params) + ")"
 
     @property
     def ports(self) -> Dict[str, Signal]:
         return self.module.ports
 
+    def __eq__(self, other) -> bool:
+        """Call equality requires:
+        * *Identity* between modules, and
+        * *Equality* between parameter-values."""
+        return self.module is other.module and self.params == other.params
+
+    def __hash__(self):
+        """Generator-Call hashing, consistent with `__eq__` above, uses:
+        * *Identity* of its module, and
+        * *Value* of its parameters.
+        The two are joined for hashing as a two-element tuple."""
+        return hash((id(self.module), self.params))
+
 
 __all__ = ["ExternalModule", "ExternalModuleCall"]
```

### Comparing `hdl21-3.0.dev3/hdl21/generator.py` & `hdl21-4.0.0rc0/hdl21/generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 """
 # hdl21 Generators
 """
 
 import inspect
-import pickle
-from textwrap import dedent
 from typing import Callable, Any, Optional, Dict
 
 # Local imports
 from .default import Default
 from .call import param_call
-from .params import HasNoParams, _unique_name
+from .params import _unique_name
 from .source_info import SourceInfo, source_info
 from .module import Module
 from .instance import calls_instantiate
 
 
 class Generator:
     """
@@ -24,36 +22,44 @@
     Stores a function-object and parameters-type, along with some auxiliary data.
     """
 
     def __init__(self, func: Callable, paramtype: type, usecontext: bool):
         self.func = func
         self.paramtype = paramtype
         self.usecontext = usecontext
-        self._source_info: Optional[SourceInfo] = source_info(get_pymodule=False)
+        self._source_info: Optional[SourceInfo] = source_info(get_pymodule=True)
 
     def __call__(self, arg: Any = Default, **kwargs: Dict) -> "GeneratorCall":
         """Calls to Generators create GeneratorCall-objects
         to be expanded during elaboration."""
         params = param_call(callee=self, arg=arg, **kwargs)
         return GeneratorCall(gen=self, params=params)
 
+    def __repr__(self) -> str:
+        return f"Generator(name={self.name})"
+
+    def __eq__(self, other) -> bool:
+        # Identity is equality
+        return other is self
+
+    def __hash__(self) -> bool:
+        # Identity is equality
+        return hash(id(self))
+
     @property
     def name(self) -> str:
         """Generator Name
         Equal to its callable-function's name."""
         return self.func.__name__
 
     @property
     def Params(self) -> type:
-        """Parameter-Type Property"""
+        """Type-style alias for the parameter-type."""
         return self.paramtype
 
-    def __repr__(self) -> str:
-        return f"Generator(name={self.name})"
-
 
 @calls_instantiate
 class GeneratorCall:
     """Generator 'Bare Calls'
     Stored for expansion during elaboration.
     Only single-argument calls with `Params` are supported.
     Any application of a `Context` is done during elaboration."""
@@ -73,31 +79,22 @@
         return self.gen is other.gen and self.params == other.params
 
     def __hash__(self):
         """Generator-Call hashing, consistent with `__eq__` above, uses:
         * *Identity* of its generator, and
         * *Value* of its parameters.
         The two are joined for hashing as a two-element tuple."""
-        return hash((id(self.gen), pickle.dumps(self.params)))
+        return hash((id(self.gen), self.params))
 
     def __repr__(self) -> str:
         return f"GeneratorCall(gen={self.gen.name})"
 
     @property
     def name(self) -> str:
-        """GeneratorCall Naming
-        Once elaborated, returns the name of the generated Module.
-        If not elaborated, raises a `RuntimeError`."""
-        if self.result is None:
-            name = self.gen.name
-            if not isinstance(self.params, HasNoParams):
-                name += "(" + _unique_name(self.params) + ")"
-            return name
-        return self.result.name  # FIXME: do we need this case?
-        # They are probably always the same already, but can be made 110% the same for sure.
+        return self.gen.name + "(" + _unique_name(self.params) + ")"
 
 
 def generator(f: Callable) -> Generator:
     """Decorator for Generator Functions"""
     from .params import isparamclass
     from .elab import Context
```

### Comparing `hdl21-3.0.dev3/hdl21/generators.py` & `hdl21-4.0.0rc0/hdl21/generators.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,26 +25,24 @@
     nser = Param(dtype=int, desc="Number of series fingers", default=1)
     npar = Param(dtype=int, desc="Number of parallel fingers", default=1)
     tp = Param(dtype=MosType, desc="MosType (PMOS/NMOS)", default=MosType.NMOS)
     vth = Param(dtype=MosVth, desc="Threshold voltage specifier", default=MosVth.STD)
 
     def __post_init_post_parse__(self):
         """Value Checks"""
-        if self.w <= 0:
+        if self.w is not None and self.w <= 0:
             raise ValueError(f"MosParams with invalid width {self.w}")
-        if self.l <= 0:
+        if self.l is not None and self.l <= 0:
             raise ValueError(f"MosParams with invalid length {self.l}")
         if self.npar <= 0:
-            raise ValueError(
-                f"MosParams with invalid number parallel fingers {self.npar}"
-            )
+            msg = f"MosParams with invalid number parallel fingers {self.npar}"
+            raise ValueError(msg)
         if self.nser <= 0:
-            raise ValueError(
-                f"MosParams with invalid number series fingers {self.nser}"
-            )
+            msg = f"MosParams with invalid number series fingers {self.nser}"
+            raise ValueError(msg)
 
 
 @generator
 def Mos(params: MosParams) -> Module:
     """Mos Series-Stack Generator
     Generates a `Module` including `nser` identical series instances of unit-Mos `primitives.Mos`.
     Unit-Mos gate and bulk ports are connected in parallel."""
```

### Comparing `hdl21-3.0.dev3/hdl21/instance.py` & `hdl21-4.0.0rc0/hdl21/instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from dataclasses import dataclass, field
 from textwrap import dedent
 
 # Local imports
 from .source_info import source_info, SourceInfo
 from .attrmagic import init
 from .connect import Connectable, is_connectable
+from .props import Properties
 
 T = TypeVar("T")
 
 
 @init
 class _Instance:
     """Shared base class for Instance-like types (Instance, InstanceArray)"""
@@ -31,14 +32,15 @@
 
         if not is_instantiable(of):
             raise RuntimeError(f"Invalid Instance of {of}")
 
         self.name: Optional[str] = name
         self.of: "Instantiable" = of
         self.conns: Dict[str, "Connectable"] = dict()
+        self.props: Properties = Properties()
 
         # References we give out, either for refering to ports or entries in out own `conns`
         self._refs = Refs()
 
         self._parent_module: Optional["Module"] = None  # Instantiating module
         self._elaborated: bool = False
         self._source_info: Optional[SourceInfo] = source_info(get_pymodule=False)
@@ -365,14 +367,15 @@
     return cls
 
 
 """
 Selected star-exports 
 Notably excludes the base class, and module-level functions
 """
+
 __all__ = [
     "Instance",
     "InstanceArray",
     "InstanceBundle",
     "InstanceBundleType",
     "calls_instantiate",
 ]
```

### Comparing `hdl21-3.0.dev3/hdl21/instantiable.py` & `hdl21-4.0.0rc0/hdl21/instantiable.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,20 +32,21 @@
     # The other variants can have a path-qualifier
     if isinstance(i, Module):
         return module_qualname(i)
     if isinstance(i, ExternalModuleCall):
         return module_qualname(i.module)
     if isinstance(i, GeneratorCall):
         return module_qualname(i.result)
-    raise TypeError
+    raise TypeError(f"Invalid Instantiable {i}")
 
 
 def io(i: Instantiable) -> Dict[str, "Connectable"]:
     """Get a complete dictionary of IO ports for `i`, including all types: Signals and Bundles.
-    Copies the Instantiable's top-level dictionary so that it is not modified by consumers."""
+    Copies the Instantiable's top-level dictionary so that it is not modified by consumers.
+    """
 
     if isinstance(i, GeneratorCall):
         if i.result is None:
             raise RuntimeError(f"Cannot get IO of unelaborated Generator {i}")
         # Take the result of the generator call
         i = i.result
```

### Comparing `hdl21-3.0.dev3/hdl21/module.py` & `hdl21-4.0.0rc0/hdl21/module.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,21 +17,23 @@
 from .instance import (
     calls_instantiate,
     Instance,
     InstanceArray,
     InstanceBundle,
 )
 from .bundle import BundleInstance
-from .qualname import qualname_magic_methods
+from .props import Properties
+from .literal import Literal
 
 # Type-alias for HDL objects storable as `Module` attributes
 ModuleAttr = Union[Signal, Instance, InstanceArray, InstanceBundle, BundleInstance]
+# And "other things" that are also storable as `Module` attributes
+ModuleOther = Union[Literal, Properties]
 
 
-@qualname_magic_methods
 @calls_instantiate
 @init
 class Module:
     """# Module
 
     The central element of hardware re-use.
     Hdl21 `Module`s are static combinations of HDL objects such as `Signal`s, `Instance`s of other `Module`s, and `Bundle`s.
@@ -64,21 +66,24 @@
             if isclass(name):
                 msg = f"Module name {name} is a class. Did you mean to use the `module` decorator?"
             else:
                 msg = f"Invalid Module name {name}, must be a string"
             raise TypeError(msg)
         self.name = name
 
-        self.ports = dict()
-        self.signals = dict()
-        self.instances = dict()
-        self.instarrays = dict()
-        self.instbundles = dict()
-        self.bundles = dict()
-        self.namespace = dict()  # Combination of all these
+        self.ports: Dict[str, Signal] = dict()
+        self.signals: Dict[str, Signal] = dict()
+        self.instances: Dict[str, Instance] = dict()
+        self.instarrays: Dict[str, InstanceArray] = dict()
+        self.instbundles: Dict[str, InstanceBundle] = dict()
+        self.bundles: Dict[str, BundleInstance] = dict()
+        self.namespace: Dict[str, ModuleAttr] = dict()  # Combination of all these
+
+        self.literals: List[Literal] = list()
+        self.props: Properties = Properties()
 
         # Elaborated version of this module.
         # Set at the end of elaboration.
         # For most modules this will be `self`.
         self._elaborated: Optional[Module] = None
 
         # IOs as captured before bundle-flattening.
@@ -190,28 +195,37 @@
         ns = self.__getattribute__("namespace")
         if key in ns:
             return ns[key]
         return object.__getattribute__(self, key)
 
     def __delattr__(self, __name: str) -> None:
         """Disable attribute deletion.
-        This may be enabled some day, but until unwinding any dependencies is not allowed."""
+        This may be enabled some day, but until unwinding any dependencies is not allowed.
+        """
         msg = f"Cannot delete Module attribute {__name} of {self}"
         raise RuntimeError(msg)
 
     def __init_subclass__(cls, *_, **__):
         """Sub-Classing Disable-ization"""
         msg = f"Error attempting to create {cls.__name__}. Sub-Typing {cls} is not supported."
         raise RuntimeError(msg)
 
     def __repr__(self) -> str:
         if self.name:
             return f"Module(name={self.name})"
         return f"Module(_anon_)"
 
+    def __eq__(self, other) -> bool:
+        # Identity is equality
+        return other is self
+
+    def __hash__(self) -> bool:
+        # Identity is equality
+        return hash(id(self))
+
 
 def module(cls: type) -> Module:
     """
     # Module Definition Decorator
 
     Converts a class-body full of Module-storable attributes to an `hdl21.Module`.
     Example Usage:
@@ -283,51 +297,54 @@
 _banned = [
     "ports",
     "signals",
     "instances",
     "instarrays",
     "instbundles",
     "bundles",
+    "literals",
+    "props",
     "namespace",
     "add",
     "get",
 ]
 
 
 def _add(module: Module, val: ModuleAttr) -> ModuleAttr:
     """Internal `Module.add` and `Module.__setattr__` implementation.
     Primarily sort `val` into one of our type-based containers.
-    Layers above `_add` must ensure that `val` has its `name` attribute before calling this method."""
+    Layers above `_add` must ensure that `val` has its `name` attribute before calling this method.
+    """
 
     if module._elaborated is not None:
         raise RuntimeError(f"Cannot add {val} to {module} after elaboration.")
 
+    # Sort out which of our type-based containers to add `val` to.
     if isinstance(val, Signal):
-        module.namespace[val.name] = val
         if val.vis == Visibility.PORT:
-            module.ports[val.name] = val
+            type_ctr = module.ports
         else:
-            module.signals[val.name] = val
+            type_ctr = module.signals
     elif isinstance(val, Instance):
-        module.instances[val.name] = val
-        module.namespace[val.name] = val
+        type_ctr = module.instances
     elif isinstance(val, InstanceArray):
-        module.instarrays[val.name] = val
-        module.namespace[val.name] = val
+        type_ctr = module.instarrays
     elif isinstance(val, InstanceBundle):
-        module.instbundles[val.name] = val
-        module.namespace[val.name] = val
+        type_ctr = module.instbundles
     elif isinstance(val, BundleInstance):
-        module.bundles[val.name] = val
-        module.namespace[val.name] = val
+        type_ctr = module.bundles
     else:
         # The next line *should* never be reached, as outer layers should have checked `_is_module_attr`.
         # Nonetheless gotta raise an error if we get here, somehow.
         _attr_type_error(val)
 
+    # Add it to the module namespace, and the type-specific container
+    type_ctr[val.name] = val
+    module.namespace[val.name] = val
+
     # Give it a reference to us.
     #
     # ## Note:
     # Parent-testing *can* be done here instead of at elaboration time.
     # It's not clear that this would be a good idea though.
     # Attributes which are *copied* (for example) keep the `_parent_module` member, which is often helpful to just over-write.
     # Nonetheless if "setattr-time" failure is desired, this is where it will go:
```

### Comparing `hdl21-3.0.dev3/hdl21/netlist.py` & `hdl21-4.0.0rc0/hdl21/netlist.py`

 * *Files identical despite different names*

### Comparing `hdl21-3.0.dev3/hdl21/noconn.py` & `hdl21-4.0.0rc0/hdl21/noconn.py`

 * *Files identical despite different names*

### Comparing `hdl21-3.0.dev3/hdl21/params.py` & `hdl21-4.0.0rc0/hdl21/params.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 """
 Hdl21 Parameters and Param-Classes 
 """
 
-from typing import Optional, Union, Any, Dict
-import dataclasses
-import json
-import pickle
-import hashlib
+# Std-Lib Imports
+import dataclasses, inspect, json, hashlib
+from typing import Optional, Any, Type, TypeVar, Dict
+
+# PyPi Imports
 import pydantic
 
 # Local Imports
 from .default import Default
 
+T = TypeVar("T")
+
 
-def paramclass(cls: type) -> type:
-    """Parameter-Class Creation Decorator
+def paramclass(cls: Type[T]) -> Type[T]:
+    """# Parameter-Class Creation Decorator
 
     Transforms a class-definition full of Params into a type-validated dataclass,
     with methods for default value and description-dictionary retrieval.
 
     Hdl21's `paramclass`es are immutable, strongly-typed data-storage structures.
     They are defined through a syntax similar to `@dataclass`, but using the `Param`
     constructor, and assignment rather than type annotation.
 
+    ```python
     @paramclass
     class C:
         reqd = Param(dtype=int, desc="A Required Parameter")
         optn = Param(dtype=int, desc="An Optional Parameter", default=11)
+    ```
 
     `Param`s each have required datatype (`dtype`) and description (`desc`) fields,
     and optional default values.
     Each `paramclass` constructor can be called with ordered arguments,
     in the order defined in the `paramclass`, or with named arguments.
     Named arguments are highly recommended for more than a single parameter.
     Note Python's function-argument ordering requirements also dictate
@@ -42,20 +46,23 @@
     names to default values (for those with defaults), respectively.
 
     Requirements of the input `cls`:
     * *All* non-Python-internal fields must be of type `Param`
     * Inheritance is not supported
     """
 
+    if not inspect.isclass(cls):
+        msg = f"Invalid @hdl21.paramclass `{cls}`. Apply the `@apramclass` decorator to classes."
+        raise RuntimeError(msg)
     if cls.__bases__ != (object,):
         raise RuntimeError(f"Invalid @hdl21.paramclass inheriting from {cls.__bases__}")
 
     protected_names = ["descriptions", "defaults"]
-    dunders = dict()
-    params = dict()
+    dunders = dict()  # Double-under attributes; ignored
+    params = dict()  # Parameters; used to create dataclass fields
 
     # Take a lap through the class dictionary, type-check everything and grab Params
     # FIXME: look for, and alert users about, the error writing type annotations rather than equality.
     # (Or, we could move to type annotations...)
     for key, val in cls.__dict__.items():
         if key in protected_names:
             raise RuntimeError(f"Invalid field name {key} in paramclass {cls}")
@@ -63,61 +70,102 @@
             dunders[key] = val
         elif isinstance(val, Param):
             params[key] = val
         else:
             msg = f"Invalid class-attribute {key} in paramclass {cls}. All attributes should be `hdl21.Param`s."
             raise RuntimeError(msg)
 
-    # Translate the Params into dataclass.field-compatible tuples
-    fields = list()
-    for name, par in params.items():
-        field = [name, par.dtype]
-        if par.default is not Default:
-            field.append(dataclasses.field(default=par.default))
-        elif par.default_factory is not Default:
-            raise NotImplementedError(f"Param.default_factory for {cls}")
-            field.append(dataclasses.field(default_factory=par.default_factory))
-        fields.append(tuple(field))
+    # Set up type annotations for the dataclass-to-be
+    # There is quite a bit of invaluable content on this here:
+    # https://docs.python.org/3/howto/annotations.html
+    # Especially for Python versions before 3.10.
+    # Some of our constraints - notably the lack of inheritance, checked above -
+    # make that advice somewhat easier to follow;
+    # nonetheless we are definitely not following it in full.
+
+    # Notably, this weird bit right here is the "howto/annotations" recommendation -
+    # Look only in the class `__dict__`, and be prepared for `__annotations__` to be missing.
+    annotations = cls.__dict__.get("__annotations__", None)
+    if annotations is None:
+        annotations = cls.__annotations__ = dict()
+
+    # Translate the Params into dataclass-compatible annotations
+    for name, param in params.items():
+        # Set the type-annotation
+        annotations[name] = param.dtype
+
+        # Handle the default value, which is the class-attribute-value on dataclasses
+        if param.default is not Default and param.default_factory is not Default:
+            msg = f"Invalid Param {param} in paramclass {cls}. Only one of `default` or `default_factory` may be specified."
+            raise RuntimeError(msg)
+
+        elif param.default is not Default:
+            setattr(cls, name, param.default)
+
+        elif param.default_factory is not Default:
+            field = dataclasses.field(default_factory=param.default_factory)
+            setattr(cls, name, field)
+
+        else:  # Otherwise there is no default value, this is a required parameter.
+            # Remove the `Param` object from the class namespace
+            delattr(cls, name)
+
     # Add a few helpers to the class namespace
-    ns = dict(
-        __params__=params,
-        __paramclass__=True,
-        descriptions=classmethod(
-            lambda cls: {k: v.desc for k, v in cls.__params__.items()}
-        ),
-        defaults=classmethod(
-            lambda cls: {
-                k: v.default
-                for k, v in cls.__params__.items()
-                if v.default is not Default
-            }
-        ),
-    )
-    # Create ourselves a (std-lib) dataclass
-    cls = dataclasses.make_dataclass(cls.__name__, fields, namespace=ns, frozen=True)
+    cls.__params__ = params
+    cls.__paramclass__ = True
+    cls.descriptions = classmethod(descriptions)
+    cls.defaults = classmethod(defaults)
+
     # Pass this through the pydantic dataclass-decorator-function
-    cls = pydantic.dataclasses.dataclass(cls, frozen=True)
+    cls = pydantic.dataclasses.dataclass(cls, config=Config, frozen=True)
+
     # Pydantic seems to want to add this one *after* class-creation
     def _brick_subclassing_(cls, *_, **__):
         msg = f"Error: attempt to sub-class `hdl21.paramclass` {cls} is not supported"
         raise RuntimeError(msg)
 
     cls.__init_subclass__ = classmethod(_brick_subclassing_)
     # And don't forget to return it!
     return cls
 
 
+def descriptions(cls: Type) -> Dict[str, str]:
+    """# Get a dictionary of parameter names to descriptions for `cls`
+    Available both as a free function and as a `classmethod` of each `paramclass`.
+    Raises a `RuntimeError` if `cls` is not a param-class."""
+
+    if not isparamclass(cls):
+        raise RuntimeError(f"Invalid @hdl21.paramclass {cls}")
+
+    return {k: v.desc for k, v in cls.__params__.items()}
+
+
+def defaults(cls: Type) -> Dict[str, Any]:
+    """# Get a dictionary of parameter names to default values for param-class `cls`.
+    Available both as a free function and as a `classmethod` of each `paramclass`.
+    Raises a `RuntimeError` if `cls` is not a param-class."""
+
+    if not isparamclass(cls):
+        raise RuntimeError(f"Invalid @hdl21.paramclass {cls}")
+
+    return {k: v.default for k, v in cls.__params__.items() if v.default is not Default}
+
+
 def isparamclass(cls: type) -> bool:
     """Boolean indication of whether `cls` has been `@paramclass`-decorated"""
     return getattr(cls, "__paramclass__", False)
 
 
-@pydantic.dataclasses.dataclass
+class Config:  # Pydantic Model Config
+    allow_extra = pydantic.Extra.forbid
+
+
+@pydantic.dataclasses.dataclass(config=Config, frozen=True)
 class Param:
-    """Parameter Declaration"""
+    """# Parameter Declaration"""
 
     dtype: Any  # Datatype. Required
     desc: str  # Description. Required
     default: Optional[Any] = Default  # Default Value. Optional
     default_factory: Optional[Any] = Default  # Default Call-Factory. Optional
 
 
@@ -175,34 +223,42 @@
 
     "Extends" `pydantic.json.pydantic_encoder` by first checking for
     each of the non-serializable Hdl21 types (`Module`, `Instance`, `Generator`, etc.),
     then hands everything else off to `pydantic.json.pydantic_encoder`.
 
     Note this *does not fully serialize `Module`s and the like -
     see `hdl21.to_proto` for this. This JSON-ization is just good enough
-    to enable unique naming of Hdl-object-value parameters."""
+    to enable unique naming of Hdl-object-valued parameters."""
 
     from .module import Module
     from .qualname import qualname as module_qualname
     from .external_module import ExternalModule, ExternalModuleCall
     from .instance import Instance
     from .generator import Generator, GeneratorCall
+    from .primitives import Primitive, PrimitiveCall
 
-    if isinstance(obj, (Instance, Generator)):
+    if isinstance(obj, (Instance,)):
         # Not supported as parameters
         raise RuntimeError(f"Invalid `hdl21.paramclass` field {obj}")
-    if isinstance(obj, (Module, ExternalModule)):
-        # Modules use their qualified class names/paths
+
+    if isinstance(obj, (Module, ExternalModule, Generator)):
+        # Use qualified class names/paths
         return module_qualname(obj)
+
+    if isinstance(obj, (Primitive, PrimitiveCall)):
+        # Primitives use their `name` attribute/ property directly
+        return obj.name
+
+    # Mix the qualified class names/paths with the parameters
+    if isinstance(obj, GeneratorCall):
+        return module_qualname(obj.gen) + _unique_name(obj.params)
+
     if isinstance(obj, ExternalModuleCall):
         # Mix the qualified class names/paths with the parameters
         return module_qualname(obj.module) + _unique_name(obj.params)
-    if isinstance(obj, GeneratorCall):
-        # Most other Hdl21 objects as parameters are pending, maybe, maybe not, support as parameter-values.
-        raise NotImplementedError
 
     # Dataclasses also require custom handling, as the default encoder deep-copies them,
     # often invoking methods not supported on several Hdl21 types.
     # Convert to (shallow) dictionaries instead.
     if dataclasses.is_dataclass(obj):
         return {f.name: getattr(obj, f.name) for f in dataclasses.fields(obj)}
```

### Comparing `hdl21-3.0.dev3/hdl21/pdk/corner.py` & `hdl21-4.0.0rc0/hdl21/pdk/corner.py`

 * *Files identical despite different names*

### Comparing `hdl21-3.0.dev3/hdl21/pdk/installation.py` & `hdl21-4.0.0rc0/hdl21/pdk/installation.py`

 * *Files identical despite different names*

### Comparing `hdl21-3.0.dev3/hdl21/pdk/pdk.py` & `hdl21-4.0.0rc0/hdl21/pdk/pdk.py`

 * *Files identical despite different names*

### Comparing `hdl21-3.0.dev3/hdl21/pdk/sample_pdk/__init__.py` & `hdl21-4.0.0rc0/hdl21/pdk/sample_pdk/__init__.py`

 * *Files identical despite different names*

### Comparing `hdl21-3.0.dev3/hdl21/pdk/sample_pdk/test_sample_pdk.py` & `hdl21-4.0.0rc0/hdl21/pdk/sample_pdk/test_sample_pdk.py`

 * *Files identical despite different names*

### Comparing `hdl21-3.0.dev3/hdl21/pdk/test_pdk.py` & `hdl21-4.0.0rc0/hdl21/pdk/test_pdk.py`

 * *Files identical despite different names*

### Comparing `hdl21-3.0.dev3/hdl21/portref.py` & `hdl21-4.0.0rc0/hdl21/portref.py`

 * *Files identical despite different names*

### Comparing `hdl21-3.0.dev3/hdl21/prefix.py` & `hdl21-4.0.0rc0/hdl21/prefix.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 typical floating-point value generation. This is again most commonly useful in conjunction 
 with the multiplication operator, to construct values such as `11 * e(-21)`. 
 
 """
 
 from enum import Enum
 from decimal import Decimal
-from typing import Optional, Any, Union
+from typing import Optional, Any, Union, Tuple
 from pydantic import BaseModel, ValidationError, Field
 from pydantic.dataclasses import dataclass
 
 
 EPSILON = 20
 
 
@@ -173,25 +173,15 @@
 
     @classmethod
     def validate(cls, v: Union["Prefixed", "ToPrefixed"]) -> "Prefixed":
         """Validate `v` as a `Prefixed` number, or convert to `Prefixed` if applicable.
         While usable elsewhere, `validate` is primarily intended for use in type-validated
         dataclass trees, such as those generated in `paramclass`es."""
 
-        if isinstance(v, Prefixed):
-            return v  # Valid as-is, return it.
-        if isinstance(v, Decimal):
-            return Prefixed(number=v)  # Also pretty much done
-        # Convert the remaining convertible types to `Decimal` inline
-        if isinstance(v, (int, float)):
-            # Note that, like `pydantic`, we convert numeric types to `str` before passing to `Decimal`.
-            return Prefixed(number=Decimal(str(v)))
-        if isinstance(v, str):
-            return Prefixed(number=Decimal(v))
-        raise ValidationError(f"Cannot convert {v} to Prefixed number")
+        return to_prefixed(v)
 
     @classmethod
     def __get_validators__(cls):
         yield cls.validate
 
     def __hash__(self):
         return hash((self.number, self.prefix))
@@ -289,14 +279,31 @@
         return round(lhs.number, EPSILON) >= round(rhs.number, EPSILON)
 
 
 # Union of the types which can be converted to `Prefixed`
 ToPrefixed = Union[int, float, str, Decimal]
 
 
+def to_prefixed(v: Union[Prefixed, "ToPrefixed"]) -> Prefixed:
+    """Convert any convertible type to a `Prefixed` number."""
+
+    if isinstance(v, Prefixed):
+        return v  # Valid as-is, return it.
+    if isinstance(v, Decimal):
+        return Prefixed(number=v)  # Also pretty much done
+    # Convert the remaining convertible types to `Decimal` inline
+    if isinstance(v, (int, float)):
+        # Note that, like `pydantic`, we convert numeric types to `str` before passing to `Decimal`.
+        return Prefixed(number=Decimal(str(v)))
+    if isinstance(v, str):
+        return Prefixed(number=Decimal(v))
+
+    raise RuntimeError(f"Cannot convert {v} to Prefixed number")
+
+
 def _add(lhs: Prefixed, rhs: Prefixed) -> Prefixed:
     """`Prefixed` Addition"""
     if lhs.prefix == rhs.prefix:
         return Prefixed.new(lhs.number + rhs.number, lhs.prefix)
 
     # Different prefix values. Scale to the smaller of the two
     smaller = lhs.prefix if lhs.prefix.value < rhs.prefix.value else rhs.prefix
@@ -311,27 +318,35 @@
 
     # Different prefix values. Scale to the smaller of the two
     smaller = lhs.prefix if lhs.prefix.value < rhs.prefix.value else rhs.prefix
     newnum = lhs.scale(smaller).number - rhs.scale(smaller).number
     return Prefixed.new(newnum, smaller)
 
 
-def _scale_to_smaller(lhs: Prefixed, rhs: Prefixed):
-    smaller = lhs.prefix if lhs.prefix.value < rhs.prefix.value else rhs.prefix
-    return lhs.scale(smaller), rhs.scale(smaller)
+def _scale_to_smaller(
+    me: Prefixed, other: Union[Prefixed, ToPrefixed]
+) -> Tuple[Prefixed, Prefixed]:
+    """# Scale two `Prefixed` numbers to the smaller of the two prefixes.
+    The `me` argument is always a `Prefixed`, generally due to being the `self` in a `Prefixed` mthod.
+    The `other` argument is commonly another compatible/ convertible type,
+    and is converted before scaling."""
+
+    other = to_prefixed(other)
+    smaller = me.prefix if me.prefix.value < other.prefix.value else other.prefix
+    return me.scale(smaller), other.scale(smaller)
 
 
 # Common prefixes as single-character identifiers, and exposed in the module namespace.
 y = YOCTO = Prefix.YOCTO
 z = ZEPTO = Prefix.ZEPTO
 a = ATTO = Prefix.ATTO
 f = FEMTO = Prefix.FEMTO
 p = PICO = Prefix.PICO
 n = NANO = Prefix.NANO
-µ = MICRO = Prefix.MICRO
+µ = u = MICRO = Prefix.MICRO
 m = MILLI = Prefix.MILLI
 c = CENTI = Prefix.CENTI
 d = DECI = Prefix.DECI
 D = DECA = Prefix.DECA
 K = KILO = Prefix.KILO
 M = MEGA = Prefix.MEGA
 G = GIGA = Prefix.GIGA
```

### Comparing `hdl21-3.0.dev3/hdl21/primitives.py` & `hdl21-4.0.0rc0/hdl21/primitives.py`

 * *Files 10% similar despite different names*

```diff
@@ -59,23 +59,23 @@
 # which imports the contents of this module and prints a line per primitive.
 # On changes to this module, re-run the script, paste the table here and anywhere else it is used.
 
 # Std-Lib Imports
 import copy
 from enum import Enum
 from dataclasses import replace
-from typing import Optional, Any, List, Type, Dict, Union
+from typing import Optional, Any, List, Type, Dict
 
 # PyPi Imports
 from pydantic.dataclasses import dataclass
 
 # Local imports
 from .default import Default
 from .call import param_call
-from .params import paramclass, Param, isparamclass, NoParams
+from .params import paramclass, Param, isparamclass, NoParams, _unique_name
 from .signal import Port, Signal, Visibility
 from .instance import calls_instantiate
 from .scalar import Scalar
 
 
 class PrimitiveType(Enum):
     """Enumerated Primitive-Types"""
@@ -92,15 +92,15 @@
     but by simulation tools or device fabricators.
     Prominent examples include MOS transistors, diodes, resistors, and capacitors.
     """
 
     name: str  # Primitive Name
     desc: str  # String Description
     port_list: List[Signal]  # Ordered Port List
-    paramtype: Type  # Class/ Type of valid Parameters
+    paramtype: Type[object]  # Class/ Type of valid Parameters
     primtype: PrimitiveType  # Ideal vs Physical Primitive-Type
 
     def __post_init_post_parse__(self):
         """After type-checking, do plenty more checks on values"""
         if not isparamclass(self.paramtype):
             msg = f"Invalid Primitive param-type {self.paramtype} for {self.name}, must be an `hdl21.paramclass`"
             raise TypeError(msg)
@@ -113,20 +113,29 @@
 
     def __call__(self, arg: Any = Default, **kwargs) -> "PrimitiveCall":
         params = param_call(callee=self, arg=arg, **kwargs)
         return PrimitiveCall(prim=self, params=params)
 
     @property
     def Params(self) -> Type:
+        """Type-style alias for the parameter-type."""
         return self.paramtype
 
     @property
     def ports(self) -> Dict[str, Signal]:
         return {p.name: p for p in self.port_list}
 
+    def __eq__(self, other) -> bool:
+        # Identity is equality
+        return other is self
+
+    def __hash__(self) -> bool:
+        # Identity is equality
+        return hash(id(self))
+
 
 @calls_instantiate
 @dataclass
 class PrimitiveCall:
     """Primitive Call
     A combination of a Primitive and its Parameter-values,
     typically generated by calling the Primitive."""
@@ -137,20 +146,39 @@
     def __post_init_post_parse__(self):
         # Type-validate our parameters
         if not isinstance(self.params, self.prim.paramtype):
             msg = f"Invalid parameters {self.params} for Primitive {self.prim}. Must be {self.prim.paramtype}"
             raise TypeError(msg)
 
     @property
+    def name(self) -> str:
+        return self.prim.name + "(" + _unique_name(self.params) + ")"
+
+    @property
     def ports(self) -> dict:
         return self.prim.ports
 
+    def __eq__(self, other) -> bool:
+        """Call equality requires:
+        * *Identity* between prims, and
+        * *Equality* between parameter-values."""
+        return self.prim is other.prim and self.params == other.params
+
+    def __hash__(self):
+        """Generator-Call hashing, consistent with `__eq__` above, uses:
+        * *Identity* of its prim, and
+        * *Value* of its parameters.
+        The two are joined for hashing as a two-element tuple."""
+        return hash((id(self.prim), self.params))
+
 
 @dataclass
 class PrimLibEntry:
+    """# Entry in the Primitive Library"""
+
     prim: Primitive
     aliases: List[str]
 
 
 # Dictionary storing all primitives, keyed by their primary name.
 # Stores aliases on the side.
 _primitives: Dict[str, PrimLibEntry] = dict()
@@ -179,49 +207,67 @@
 
 """ 
 Mos Transistor Section 
 """
 
 
 class MosType(Enum):
-    """NMOS/PMOS Type Enumeration"""
+    """# MOS Type (NMOS/ PMOS) Enumeration"""
 
     NMOS = "NMOS"
     PMOS = "PMOS"
 
 
 class MosVth(Enum):
-    """MOS Threshold Enumeration"""
+    """# MOS Threshold Enumeration"""
 
     STD = "STD"
     LOW = "LOW"
     HIGH = "HIGH"
+    ULTRA_LOW = "ULTRA_LOW"
+    ZERO = "ZERO"
+    NATIVE = "NATIVE"
+
+
+class MosFamily(Enum):
+    """# MOS Family Enumeration"""
+
+    NONE = "NONE"
+    CORE = "CORE"
+    IO = "IO"
+    LP = "LP"
+    HP = "HP"
 
 
 @paramclass
 class MosParams:
-    """MOS Transistor Parameters"""
+    """# MOS Transistor Parameters"""
 
     w = Param(dtype=Optional[Scalar], desc="Width in resolution units", default=None)
     l = Param(dtype=Optional[Scalar], desc="Length in resolution units", default=None)
-    npar = Param(dtype=int, desc="Number of parallel fingers", default=1)
+    npar = Param(
+        dtype=Scalar, desc="Number of parallel fingers", default=1
+    )  # FIXME: rename
+    mult = Param(dtype=Scalar, desc="Multiplier", default=1)
+
     tp = Param(dtype=MosType, desc="MosType (Nmos/ Pmos)", default=MosType.NMOS)
     vth = Param(dtype=MosVth, desc="Threshold voltage specifier", default=MosVth.STD)
+    family = Param(dtype=MosFamily, desc="Device family", default=MosFamily.NONE)
     model = Param(dtype=Optional[str], desc="Model (Name)", default=None)
-    # FIXME: whether to include `model`
 
-    def __post_init_post_parse__(self):
-        """Value Checks"""
-        if self.w <= 0:
-            raise ValueError(f"MosParams with invalid width {self.w}")
-        if self.l <= 0:
-            raise ValueError(f"MosParams with invalid length {self.l}")
-        if self.npar <= 0:
-            msg = f"MosParams with invalid number parallel fingers {self.npar}"
-            raise ValueError(msg)
+    # def __post_init_post_parse__(self):
+    #     """Value Checks"""
+    #     # FIXME: re-introduce these, for the case in which the parameters are `Prefixed` and not `Literal` values.
+    #     if self.w <= 0:
+    #         raise ValueError(f"MosParams with invalid width {self.w}")
+    #     if self.l <= 0:
+    #         raise ValueError(f"MosParams with invalid length {self.l}")
+    #     if self.npar <= 0:
+    #         msg = f"MosParams with invalid number parallel fingers {self.npar}"
+    #         raise ValueError(msg)
 
 
 # Mos Transistor Ports, in SPICE Conventional Order
 MosPorts = [
     Port(name="d", desc="Drain"),
     Port(name="g", desc="Gate"),
     Port(name="s", desc="Source"),
@@ -265,15 +311,15 @@
 
 
 @paramclass
 class ResistorParams:
     r = Param(dtype=Scalar, desc="Resistance (ohms)")
 
 
-_add(
+IdealResistor = _add(
     prim=Primitive(
         name="IdealResistor",
         desc="Ideal Resistor",
         port_list=copy.deepcopy(PassivePorts),
         paramtype=ResistorParams,
         primtype=PrimitiveType.IDEAL,
     ),
@@ -284,27 +330,27 @@
 @paramclass
 class PhysicalResistorParams:
     w = Param(dtype=Optional[Scalar], desc="Width in resolution units", default=None)
     l = Param(dtype=Optional[Scalar], desc="Length in resolution units", default=None)
     model = Param(dtype=Optional[str], desc="Model (Name)", default=None)
 
 
-_add(
+PhysicalResistor = _add(
     prim=Primitive(
         name="PhysicalResistor",
         desc="Physical Resistor",
         port_list=copy.deepcopy(PassivePorts),
         paramtype=PhysicalResistorParams,
         primtype=PrimitiveType.PHYSICAL,
     ),
     aliases=["PhyR", "PhyRes", "ResPhy", "PhyResistor"],
 )
 
 
-_add(
+ThreeTerminalResistor = _add(
     prim=Primitive(
         name="ThreeTerminalResistor",
         desc="Three Terminal Resistor",
         port_list=copy.deepcopy(ThreeTerminalPorts),
         paramtype=PhysicalResistorParams,
         primtype=PrimitiveType.PHYSICAL,
     ),
@@ -313,44 +359,48 @@
 
 
 @paramclass
 class IdealCapacitorParams:
     c = Param(dtype=Scalar, desc="Capacitance (F)")
 
 
-_add(
+IdealCapacitor = _add(
     prim=Primitive(
         name="IdealCapacitor",
         desc="Ideal Capacitor",
         port_list=copy.deepcopy(PassivePorts),
         paramtype=IdealCapacitorParams,
         primtype=PrimitiveType.IDEAL,
     ),
     aliases=["C", "Cap", "Capacitor", "IdealC", "IdealCap"],
 )
 
 
 @paramclass
 class PhysicalCapacitorParams:
-    c = Param(dtype=Scalar, desc="Capacitance (F)")
+    c = Param(dtype=Scalar, desc="Capacitance (F)", default=None)
+    w = Param(dtype=Scalar, desc="Width in resolution units", default=None)
+    l = Param(dtype=Scalar, desc="Length in resolution units", default=None)
+    model = Param(dtype=Optional[str], desc="Model (Name)", default=None)
+    mult = Param(dtype=Optional[str], desc="Multiplier", default=None)
 
 
-_add(
+PhysicalCapacitor = _add(
     prim=Primitive(
         name="PhysicalCapacitor",
         desc="Physical Capacitor",
         port_list=copy.deepcopy(PassivePorts),
         paramtype=PhysicalCapacitorParams,
         primtype=PrimitiveType.PHYSICAL,
     ),
     aliases=["PhyC", "PhyCap", "CapPhy", "PhyCapacitor"],
 )
 
 
-_add(
+ThreeTerminalCapacitor = _add(
     prim=Primitive(
         name="ThreeTerminalCapacitor",
         desc="Three Terminal Capacitor",
         port_list=copy.deepcopy(ThreeTerminalPorts),
         paramtype=PhysicalCapacitorParams,
         primtype=PrimitiveType.PHYSICAL,
     ),
@@ -359,15 +409,15 @@
 
 
 @paramclass
 class IdealInductorParams:
     l = Param(dtype=Scalar, desc="Inductance (H)")
 
 
-_add(
+IdealInductor = _add(
     prim=Primitive(
         name="IdealInductor",
         desc="Ideal Inductor",
         port_list=copy.deepcopy(PassivePorts),
         paramtype=IdealInductorParams,
         primtype=PrimitiveType.IDEAL,
     ),
@@ -376,46 +426,46 @@
 
 
 @paramclass
 class PhysicalInductorParams:
     l = Param(dtype=Scalar, desc="Inductance (H)")
 
 
-_add(
+PhysicalInductor = _add(
     Primitive(
         name="PhysicalInductor",
         desc="Physical Inductor",
         port_list=copy.deepcopy(PassivePorts),
         paramtype=PhysicalInductorParams,
         primtype=PrimitiveType.PHYSICAL,
     ),
     aliases=["PhyL", "PhyInd", "IndPhy", "PhyInductor"],
 )
 
 
-_add(
+ThreeTerminalInductor = _add(
     prim=Primitive(
         name="ThreeTerminalInductor",
         desc="Three Terminal Inductor",
         port_list=copy.deepcopy(ThreeTerminalPorts),
         paramtype=PhysicalInductorParams,
         primtype=PrimitiveType.PHYSICAL,
     ),
     aliases=["Ind3", "PhyInd3", "IndPhy3", "PhyInductor3"],
 )
 
 
 @paramclass
 class PhysicalShortParams:
-    layer = Param(dtype=Optional[Union[int, str]], desc="Metal layer", default=None)
+    layer = Param(dtype=Optional[Scalar], desc="Metal layer", default=None)
     w = Param(dtype=Optional[Scalar], desc="Width in resolution units", default=None)
     l = Param(dtype=Optional[Scalar], desc="Length in resolution units", default=None)
 
 
-_add(
+PhysicalShort = _add(
     prim=Primitive(
         name="PhysicalShort",
         desc="Short-Circuit/ Net-Tie",
         port_list=copy.deepcopy(PassivePorts),
         paramtype=PhysicalShortParams,
         primtype=PrimitiveType.PHYSICAL,
     ),
@@ -432,15 +482,15 @@
 class DcVoltageSourceParams:
     """`DcVoltageSource` Parameters"""
 
     dc = Param(dtype=Optional[Scalar], default=0, desc="DC Value (V)")
     ac = Param(dtype=Optional[Scalar], default=None, desc="AC Amplitude (V)")
 
 
-_add(
+DcVoltageSource = _add(
     prim=Primitive(
         name="DcVoltageSource",
         desc="DC Voltage Source",
         port_list=copy.deepcopy(PassivePorts),
         paramtype=DcVoltageSourceParams,
         primtype=PrimitiveType.IDEAL,
     ),
@@ -461,38 +511,41 @@
     v2 = Param(dtype=Optional[Scalar], default=None, desc="Zero Value (V)")
     period = Param(dtype=Optional[Scalar], default=None, desc="Period (s)")
     rise = Param(dtype=Optional[Scalar], default=None, desc="Rise time (s)")
     fall = Param(dtype=Optional[Scalar], default=None, desc="Fall time (s)")
     width = Param(dtype=Optional[Scalar], default=None, desc="Pulse width (s)")
 
 
-_add(
+PulseVoltageSource = _add(
     prim=Primitive(
         name="PulseVoltageSource",
         desc="Pulse Voltage Source",
         port_list=copy.deepcopy(PassivePorts),
         paramtype=PulseVoltageSourceParams,
         primtype=PrimitiveType.IDEAL,
     ),
     aliases=["Vpu", "Vpulse"],
 )
 
+Vpu = PulseVoltageSource
+Vpulse = PulseVoltageSource
+
 
 @paramclass
 class SineVoltageSourceParams:
     """`SineVoltageSource` Parameters"""
 
     voff = Param(dtype=Optional[Scalar], default=None, desc="Offset (V)")
     vamp = Param(dtype=Optional[Scalar], default=None, desc="Amplitude (V)")
     freq = Param(dtype=Optional[Scalar], default=None, desc="Frequency (Hz)")
     td = Param(dtype=Optional[Scalar], default=None, desc="Delay (s)")
     phase = Param(dtype=Optional[Scalar], default=None, desc="Phase at td (degrees)")
 
 
-_add(
+SineVoltageSource = _add(
     prim=Primitive(
         name="SineVoltageSource",
         desc="Sine Voltage Source",
         port_list=copy.deepcopy(PassivePorts),
         paramtype=SineVoltageSourceParams,
         primtype=PrimitiveType.IDEAL,
     ),
@@ -501,15 +554,15 @@
 
 
 @paramclass
 class CurrentSourceParams:
     dc = Param(dtype=Optional[Scalar], default=0, desc="DC Value (A)")
 
 
-_add(
+CurrentSource = _add(
     Primitive(
         name="CurrentSource",
         desc="Ideal DC Current Source",
         port_list=copy.deepcopy(PassivePorts),
         paramtype=CurrentSourceParams,
         primtype=PrimitiveType.IDEAL,
     ),
@@ -531,45 +584,45 @@
 ControlledSourcePorts = [
     Port(name="p", desc="Output, Positive"),
     Port(name="n", desc="Output, Negative"),
     Port(name="cp", desc="Control, Positive"),
     Port(name="cn", desc="Control, Negative"),
 ]
 
-_add(
+VoltageControlledVoltageSource = _add(
     prim=Primitive(
         name="VoltageControlledVoltageSource",
         desc="Voltage Controlled Voltage Source",
         port_list=copy.deepcopy(ControlledSourcePorts),
         paramtype=ControlledSourceParams,
         primtype=PrimitiveType.IDEAL,
     ),
     aliases=["Vcvs", "VCVS"],
 )
-_add(
+CurrentControlledVoltageSource = _add(
     prim=Primitive(
         name="CurrentControlledVoltageSource",
         desc="Current Controlled Voltage Source",
         port_list=copy.deepcopy(ControlledSourcePorts),
         paramtype=ControlledSourceParams,
         primtype=PrimitiveType.IDEAL,
     ),
     aliases=["Ccvs", "CCVS"],
 )
-_add(
+VoltageControlledCurrentSource = _add(
     prim=Primitive(
         name="VoltageControlledCurrentSource",
         desc="Voltage Controlled Current Source",
         port_list=copy.deepcopy(ControlledSourcePorts),
         paramtype=ControlledSourceParams,
         primtype=PrimitiveType.IDEAL,
     ),
     aliases=["Vccs", "VCCS"],
 )
-_add(
+CurrentControlledCurrentSource = _add(
     prim=Primitive(
         name="CurrentControlledCurrentSource",
         desc="Current Controlled Current Source",
         port_list=copy.deepcopy(ControlledSourcePorts),
         paramtype=ControlledSourceParams,
         primtype=PrimitiveType.IDEAL,
     ),
@@ -593,20 +646,22 @@
     """Bipolar Transistor Parameters"""
 
     w = Param(dtype=Optional[Scalar], desc="Width in resolution units", default=None)
     l = Param(dtype=Optional[Scalar], desc="Length in resolution units", default=None)
     tp = Param(
         dtype=BipolarType, desc="Bipolar Type (NPN/ PNP)", default=BipolarType.NPN
     )
+    model = Param(dtype=Optional[str], desc="Model (Name)", default=None)
+    mult = Param(dtype=Optional[Scalar], desc="Multiplier", default=None)
 
     def __post_init_post_parse__(self):
         """Value Checks"""
-        if self.w <= 0:
+        if self.w is not None and self.w <= 0:
             raise ValueError(f"BipolarParams with invalid width {self.w}")
-        if self.l <= 0:
+        if self.l is not None and self.l <= 0:
             raise ValueError(f"BipolarParams with invalid length {self.l}")
 
 
 BipolarPorts = [Port(name="c"), Port(name="b"), Port(name="e")]
 
 Bipolar = _add(
     prim=Primitive(
@@ -640,18 +695,17 @@
 
 
 @paramclass
 class DiodeParams:
     w = Param(dtype=Optional[Scalar], desc="Width in resolution units", default=None)
     l = Param(dtype=Optional[Scalar], desc="Length in resolution units", default=None)
     model = Param(dtype=Optional[str], desc="Model (Name)", default=None)
-    # FIXME: whether to include `model`
 
 
-_add(
+Diode = _add(
     prim=Primitive(
         name="Diode",
         desc="Diode",
         # Despite not really being "passive", Diode does use the same `PassivePorts` list.
         port_list=copy.deepcopy(PassivePorts),
         paramtype=DiodeParams,
         primtype=PrimitiveType.PHYSICAL,
```

### Comparing `hdl21-3.0.dev3/hdl21/proto/from_proto.py` & `hdl21-4.0.0rc0/hdl21/proto/from_proto.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,27 +13,29 @@
 from ..prefix import Prefix, Prefixed
 from ..module import Module
 from ..external_module import ExternalModule
 from ..instance import Instance
 from ..signal import Signal, PortDir, Visibility
 from ..slice import Slice
 from ..concat import Concat
+from ..literal import Literal
 from .. import primitives
 from ..primitives import Primitive, Vpulse
 
 
 def from_proto(pkg: vckt.Package) -> SimpleNamespace:
     """Convert Proto-defined Package `pkg` to a namespace-full of Modules."""
     importer = ProtoImporter(pkg)
     return importer.import_()
 
 
 class ProtoImporter:
     """Protobuf Package Importer.
-    Collects all `Modules` defined in Protobuf-sourced primary-argument `pkg` into a Python `types.SimpleNamespace`."""
+    Collects all `Modules` defined in Protobuf-sourced primary-argument `pkg` into a Python `types.SimpleNamespace`.
+    """
 
     def __init__(self, pkg: vckt.Package):
         self.pkg = pkg
         self.modules = dict()  # Dict of names to Modules
         self.ext_modules = dict()  # Dict of qual-names to ExternalModules
         self.ns = SimpleNamespace()
         self.ns.name = pkg.domain
@@ -106,29 +108,33 @@
         module._importpath = path[:-1]
         module.name = path[-1]
 
         # Import its signals and ports
         for sig in import_ports_and_signals(pmod):
             module.add(sig)
 
-        # Lap through instances, connecting them, creating internal Signals if necessary (bleh)
+        # Lap through instances & connect them
         for pinst in pmod.instances:
             inst = self.import_instance(pinst)
             module.add(inst)
 
             # Make the instance's connections
             for pconn in pinst.connections:
                 if pconn.portname not in inst._resolved.ports:
                     msg = f"Invalid Port {pconn.portname} on {inst} in Module {module.name}"
                     raise RuntimeError(msg)
                 # Import the Signal-object
                 conn = import_connection_target(pconn.target, module)
                 # And connect it to the Instance
                 inst.connect(pconn.portname, conn)
 
+        # Import any literal content
+        for plit in pmod.literals:
+            module.literals.append(Literal(text=plit))
+
         # Add the Module to our cache and return-namespace, and return it
         self.modules[pmod.name] = module
         setattr(ns, module.name, module)
         return module
 
     def import_instance(self, pinst: vckt.Instance) -> Instance:
         """Convert Proto-Instance `pinst` to an `hdl21.Instance`.
@@ -183,15 +189,16 @@
         return Instance(name=pinst.name, of=target)
 
 
 def import_ports_and_signals(
     pmod: Union[vckt.Module, vckt.ExternalModule]
 ) -> List[Signal]:
     """Import all Ports and Signals from Proto-Module `pmod`.
-    Returns them as a single list, which can serve as arguments to `Module.add` or `ExternalModule.port_list`."""
+    Returns them as a single list, which can serve as arguments to `Module.add` or `ExternalModule.port_list`.
+    """
 
     # Keep a dictionary from name: Signal imported
     signals: Dict[str, Signal] = {}
     for psig in pmod.signals:
         signals[psig.name] = Signal(name=psig.name, width=psig.width)
 
     # Convert the entries of `signals` that are ports
```

### Comparing `hdl21-3.0.dev3/hdl21/proto/to_proto.py` & `hdl21-4.0.0rc0/hdl21/proto/to_proto.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 which particularly handles hierarchically-referential types such as `Module`, `Instance`, and `ExternalModule`. 
 
 Exports of simpler "scalar"(-ish) types such as `Signal`s and `Param`s are provided as 
 free-standing functions to enable use elsewhere. 
 """
 
 from decimal import Decimal
-from textwrap import dedent
 from dataclasses import fields
 from enum import Enum
 from typing import Optional, List, Union, Dict, Any
 
 from pydantic.dataclasses import dataclass
 
 # Local imports
@@ -98,30 +97,29 @@
         return self.pkg
 
     def export_module_name(self, module: Module) -> vlsir.utils.QualifiedName:
         """Create and return a unique `QualifiedName` for Module `module`.
         Raises a `RuntimeError` if unique name is taken."""
 
         mname = module_qualname(module)
-        if "Mos(7271d1c5009776529f754c575eb55012)" in mname:
-            print(5)
+
         if mname in self.modules_by_name:
             conflict = self.modules_by_name[mname].hmod
             msg = f"Cannot serialize Module {module} due to conflicting name with {conflict}. \n"
             msg += "(Was this a generator that didn't get decorated with `@hdl21.generator`?) "
             raise RuntimeError(msg)
         return mname
 
     def export_module(self, module: Module) -> vckt.Module:
         """Export a Module `module` and all its dependencies."""
 
         if id(module) in self.modules_by_id:  # Already done
             return self.modules_by_id[id(module)].pmod
 
-        if module.bundles:  # Can't handle these, at least for now
+        if module.bundles:  # Invalid, should have been elaborated out.
             msg = f"Invalid attribute for Proto export: Module {module.name} with Bundles {list(module.bundles.keys())}"
             raise RuntimeError(msg)
 
         # Create the Proto-Module
         pmod = vckt.Module()
 
         # Create its serialized name
@@ -140,29 +138,33 @@
         for inst in module.instances.values():
             if not inst._resolved:
                 msg = f"Invalid Instance {inst.name} of unresolved Module in Module {module.name}"
                 raise RuntimeError(msg)
             pinst = self.export_instance(inst)
             pmod.instances.append(pinst)
 
+        # Create the Module's `literal`s
+        for literal in module.literals:
+            pmod.literals.append(export_literal(literal))
+
         # Store references to the result, and return it
         mapping = ModuleMapping(module, pmod)
         self.modules_by_id[id(module)] = mapping
         self.modules_by_name[pmod.name] = mapping
         self.pkg.modules.append(pmod)
         return pmod
 
     def export_external_module(self, emod: ExternalModule) -> vckt.ExternalModule:
         """Export an `ExternalModule`"""
         if id(emod) in self.ext_modules:  # Already done
             return self.ext_modules[id(emod)]
 
         # Create the Proto-ExternalModule
         qname = vlsir.utils.QualifiedName(name=emod.name, domain=emod.domain)
-        pmod = vckt.ExternalModule(name=qname)
+        pmod = vckt.ExternalModule(name=qname, spicetype=emod.spicetype.to_schema())
 
         # Create its Port-objects, which also require Vlsir Signal objects
         for port in emod.port_list:
             psig = vckt.Signal(name=port.name, width=port.width)
             pmod.signals.append(psig)
             pmod.ports.append(export_port(port))
 
@@ -377,15 +379,15 @@
         return vlsir.ParamValue(literal=val.value)
 
     # Internal numeric (and number-like) types
     if isinstance(val, Scalar):
         # `Scalar` will either have an internal `Literal` or `Prefixed` value.
         val = val.inner
     if isinstance(val, Literal):  # String/ expression literals
-        return vlsir.ParamValue(literal=val.txt)
+        return vlsir.ParamValue(literal=val.text)
     if isinstance(val, Prefixed):
         return vlsir.ParamValue(prefixed=export_prefixed(val))
 
     # Standard-Lib Numbers
     if isinstance(val, Decimal):
         return vlsir.ParamValue(literal=str(val))
     if isinstance(val, int):
@@ -458,7 +460,12 @@
 #
 #     # Create its Port-objects
 #     for port in prim.port_list:
 #         pmod.ports.append(cls.export_port(port))
 #
 #     # And return it
 #     return pmod
+
+
+def export_literal(literal: Literal) -> str:
+    """Export a `Literal`, as its text value"""
+    return literal.text
```

### Comparing `hdl21-3.0.dev3/hdl21/qualname.py` & `hdl21-4.0.0rc0/hdl21/qualname.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,62 +2,47 @@
 # Qualified Names 
 
 Helpers for uniquely identifying a Module or ExternalModule, 
 given their native language (Python) has hierarchical namespaces, 
 and many of their import/ export languages (e.g. Verilog, netlists) do not.
 """
 
+from typing import Optional, Union, List
 
-from typing import Any, Optional, Union, TypeVar, Type
+# Type alias of the types that have a qualified path.
+HasQualPath = Union["Module", "ExternalModule", "Generator"]
 
 
-def qualname(mod: Union["Module", "ExternalModule"]) -> Optional[str]:
-    """# Qualified Name
-    Helper for exporting. Returns a module's path-qualified name.
+def qualpath(mod: HasQualPath) -> Optional[List[str]]:
+    """# Qualified Path
+    Helper for exporting. Returns a module's definition path.
     This is generally one of a few things:
     * If "normally" defined via Python code, it's the Python module path plus the module name.
     * If *imported*, it's the path inferred during import."""
 
-    if mod._importpath is not None:
+    if getattr(mod, "_importpath", None) is not None:
         # Imported. Return the period-separated import path.
-        return ".".join(mod._importpath)
+        return mod._importpath
 
     if mod.name is None:
         # Unnamed. Return None.
         return None
 
     if mod._source_info.pymodule is None:
-        # Defined in a non-Python context. Return the Module's name, without any path qualifiers.
-        return mod.name
+        # Defined outside a Python module, e.g. in a call to `exec`, a notebook cell, or a `python -c` string.
+        # Return its name without any path qualifiers.
+        return [mod.name]
 
     # Defined the old fashioned way. Use the Python module name.
-    return mod._source_info.pymodule.__name__ + "." + mod.name
-
-
-T = TypeVar("T")
-
+    return mod._source_info.pymodule.__name__.split(".") + [mod.name]
 
-def qualname_magic_methods(cls: Type[T]) -> Type[T]:
-    """Decorator to add the 'use qualname for equality, hashing, and pickling'
-    magic methods to a class."""
 
-    def __eq__(self, other: "Self") -> bool:
-        if not isinstance(other, type(self)):
-            return NotImplemented
-        if self.name is None or other.name is None:
-            raise RuntimeError(f"Cannot invoke equality on unnamed {type(self)} {self}")
-        return qualname(self) == qualname(other)
-
-    def __hash__(self):
-        if self.name is None:
-            raise RuntimeError(f"Cannot invoke hashing on unnamed {type(self)} {self}")
-        return hash(qualname(self))
-
-    def __getstate__(self):
-        if self.name is None:
-            raise RuntimeError(f"Cannot invoke pickling on unnamed {type(self)} {self}")
-        return qualname(self)
+def qualname(mod: HasQualPath) -> Optional[str]:
+    """# Qualified Name
+    Helper for exporting. Returns a module's path-qualified name.
+    If `mod` has a qualified path as determined by `qualpath`, returns it
+    joined together by the Python-conventional path-separator "."."""
 
-    cls.__eq__ = __eq__
-    cls.__hash__ = __hash__
-    cls.__getstate__ = __getstate__
-    return cls
+    qpath = qualpath(mod)
+    if qpath is None:
+        return None
+    return ".".join(qpath)
```

### Comparing `hdl21-3.0.dev3/hdl21/signal.py` & `hdl21-4.0.0rc0/hdl21/signal.py`

 * *Files 26% similar despite different names*

```diff
@@ -22,65 +22,119 @@
 
 from copy import copy
 from enum import Enum
 from dataclasses import field
 from typing import Callable, Optional, List, Set
 
 # Local imports
+from .role import Role
 from .datatype import datatype
+from .visibility import Visibility
 from .connect import connectable
 from .sliceable import sliceable
 from .concat import concatable
+from .props import Properties
 
 
 class PortDir(Enum):
-    """Port-Direction Enumeration"""
+    """# Port Direction Enumeration"""
 
-    INPUT = 0
-    OUTPUT = 1
-    INOUT = 2
-    NONE = 3
-
-
-class Visibility(Enum):
-    """Port-Visibility Enumeration"""
-
-    INTERNAL = 0  # Internal, Module-private Signal
-    PORT = 1  # Exposed as a Port
+    INPUT = "INPUT"
+    OUTPUT = "OUTPUT"
+    INOUT = "INOUT"
+    NONE = "NONE"  # No direction or unspecified
+
+    def flipped(self) -> "PortDir":
+        """# Flip the direction of a port"""
+        if self == PortDir.INPUT:
+            return PortDir.OUTPUT
+        if self == PortDir.OUTPUT:
+            return PortDir.INPUT
+        return self  # INOUT or NONE
+
+
+class Usage(Enum):
+    """# Signal Usage"""
+
+    SIGNAL = "SIGNAL"
+    POWER = "POWER"
+    GROUND = "GROUND"
+    CLOCK = "CLOCK"
 
 
 @sliceable
 @concatable
 @connectable
 @datatype
 class Signal:
     """
-    # hdl21 Signal
-    The base-level unit of hardware connectivity
+    # Signal
+
+    Signals are Hdl21's base-level unit of hardware connectivity.
+
+    Each `Signal` is analogous in content to a *bus* or (single-dimensional) *array* in many legacy HDLs.
+    (Most similar to Verilog's packed single-dimensional arrays.)
+    The `Signal.width` field indicates the bit-width of said bus.
+    It defaults to one for scalar Signals.
+    Widths of zero or less generate errors, both at construction-time and later.
+
+    Hdl21 `Signals` are *untyped*.
+    They represent a connection, not the type or value of data it carries.
+    In this sense they are more similar to analog-style environments than to most legacy HDLs.
+
+    `Ports`, `Inputs`, `Outputs`, and `Inouts` are not dedicated Hdl21 types,
+    but thin convenience function-wrappers around `Signal`.
+    Each `Signal` includes enumerated fields for its visibility (internal vs port)
+    and direction. For internal `Signals`, the `direction` field is globally expected to be ignored.
+
     """
 
-    name: Optional[str] = None
-    width: int = 1
-    vis: Visibility = Visibility.INTERNAL
-    direction: PortDir = PortDir.NONE
+    name: Optional[str] = None  # Signal name
+    width: int = 1  # Bit-width
+    vis: Visibility = field(repr=False, default=Visibility.INTERNAL)  # Port visibility
+    direction: PortDir = field(repr=False, default=PortDir.NONE)  # Port direction
+    usage: Usage = field(repr=False, default=Usage.SIGNAL)  # Signal usage
+    props: Properties = field(repr=False, default_factory=Properties)  # Properties
     desc: Optional[str] = None  # Description
-    src: Optional[Enum] = field(repr=False, default=None)
-    dest: Optional[Enum] = field(repr=False, default=None)
+    src: Optional[Role] = field(repr=False, default=None)  # Source Role
+    dest: Optional[Role] = field(repr=False, default=None)  # Destination Role
+
+    # Related signals
+    related_clk: Optional["Signal"] = field(repr=False, default=None)
+    # Related clock signal
+    related_pwr: Optional["Signal"] = field(repr=False, default=None)
+    # Related power signal
+    related_gnd: Optional["Signal"] = field(repr=False, default=None)
+    # Related ground signal
 
     def __post_init_post_parse__(self):
         if self.width < 1:
             raise ValueError(f"Signal {self.name} width must be positive")
         self._parent_module: Optional["Module"] = None
         self._slices: Set["Slice"] = set()
         self._concats: Set["Concat"] = set()
         self._connected_ports: Set["PortRef"] = set()
 
+        # Back-references to related signals
+        self._related_clk_of: Set["Signal"] = set()
+        self._related_pwr_of: Set["Signal"] = set()
+        self._related_gnd_of: Set["Signal"] = set()
+
+        # Add those back-references to signals *we* relate to.
+        # Note this only happens at construction-time.
+        if self.related_clk is not None:
+            self.related_clk._related_clk_of.add(self)
+        if self.related_pwr is not None:
+            self.related_pwr._related_pwr_of.add(self)
+        if self.related_gnd is not None:
+            self.related_gnd._related_gnd_of.add(self)
+
     def __eq__(self, other) -> bool:
         # Identity is equality
-        return id(self) == id(other)
+        return other is self
 
     def __hash__(self) -> bool:
         # Identity is equality
         return hash(id(self))
 
     def __copy__(self) -> "Signal":
         """Signal copying implementation
@@ -99,115 +153,103 @@
         )
 
     def __deepcopy__(self, _memo) -> "Signal":
         """Signal "deep" copies"""
         # The same as shallow ones; there is no "deep" data being copied.
         return self.__copy__()
 
-
-def _copy_to_internal(sig: Signal) -> Signal:
-    """Make a copy of `sig`, replacing its visibility and port-direction to be internal."""
-    sig = copy(sig)
-    sig.vis = Visibility.INTERNAL
-    sig.direction = PortDir.NONE
-    sig._parent_module = None
-    return sig
+    def __rmul__(self, num: int) -> List["Signal"]:
+        """# Right multiplication. Creates `num` copies of this Signal."""
+        if not isinstance(num, int):
+            return NotImplemented
+        return [copy(self) for _ in range(num)]
 
 
-def Signals(num: int, **kwargs) -> List[Signal]:
-    """
-    Create `num` new Signals.
-    Typical usage:
-    ```python
-    @h.module
-    class UsesSignals:
-        bias, fold, mirror = h.Signals(3)
-    ```
-    Note the `num` value is required to support the tuple-destructuring use-case shown above.
-    """
-    return _plural(fn=Signal, num=num, **kwargs)
+"""
+# Constructor Helpers 
+
+Thin wrappers around the `Signal` constructor which set common fields, 
+e.g. `Port()` replacing `Signal(vis=Visibility.PORT)`.
+"""
 
 
 def Input(**kwargs) -> Signal:
-    """Input Port Constructor. Thin wrapper around `hdl21.Signal`"""
+    """# Input Port Constructor
+    Thin wrapper around `hdl21.Signal`"""
     return Signal(vis=Visibility.PORT, direction=PortDir.INPUT, **kwargs)
 
 
-def Inputs(num: int, **kwargs) -> List[Signal]:
-    """
-    Create `num` new Input Ports.
-    Typical usage:
-    ```python
-    @h.module
-    class UsesInputs:
-        a, b, c, VDD, VSS = h.Inputs(5)
-    ```
-    Note the `num` value is required to support the tuple-destructuring use-case shown above.
-    """
-    return _plural(fn=Input, num=num, **kwargs)
-
-
 def Output(**kwargs) -> Signal:
-    """Output Port Constructor. Thin wrapper around `hdl21.Signal`"""
+    """# Output Port Constructor
+    Thin wrapper around `hdl21.Signal`"""
     return Signal(vis=Visibility.PORT, direction=PortDir.OUTPUT, **kwargs)
 
 
-def Outputs(num: int, **kwargs) -> List[Signal]:
-    """
-    Create `num` new Output Ports.
-    Typical usage:
-    ```python
-    @h.module
-    class UsesOutputs:
-        tdo, tms, tck = h.Outputs(3)
-    ```
-    Note the `num` value is required to support the tuple-destructuring use-case shown above.
-    """
-    return _plural(fn=Output, num=num, **kwargs)
-
-
 def Inout(**kwargs) -> Signal:
-    """Inout Port Constructor. Thin wrapper around `hdl21.Signal`"""
+    """# Inout Port Constructor
+    Thin wrapper around `hdl21.Signal`"""
     return Signal(vis=Visibility.PORT, direction=PortDir.INOUT, **kwargs)
 
 
-def Inouts(num: int, **kwargs) -> List[Signal]:
-    """
-    Create `num` new Inout Ports.
-    Typical usage:
-    ```python
-    @h.module
-    class UsesInouts:
-        gpio1, gpio2 = h.Inouts(2)
-    ```
-    Note the `num` value is required to support the tuple-destructuring use-case shown above.
-    """
-    return _plural(fn=Inout, num=num, **kwargs)
-
-
 def Port(direction=PortDir.NONE, **kwargs) -> Signal:
-    """Port Constructor. Thin wrapper around `hdl21.Signal`.
+    """# Port Constructor
+    Thin wrapper around `hdl21.Signal`.
     The `direction` argument sets the Port's direction,
     and defaults to the unknown direction `PortDir.NONE`."""
     return Signal(direction=direction, vis=Visibility.PORT, **kwargs)
 
 
-def Ports(num: int, **kwargs) -> List[Signal]:
-    """
-    Create `num` new Ports.
-    Typical usage:
-    ```python
-    @h.module
-    class UsesPorts:
-        inp, out = h.Ports(2)
-    ```
-    Note the `num` value is required to support the tuple-destructuring use-case shown above.
-    """
-    return _plural(fn=Port, num=num, **kwargs)
+def Power(**kwargs) -> Signal:
+    """# Power Signal Constructor
+    Thin wrapper around `hdl21.Signal`"""
+    return Signal(usage=Usage.POWER, **kwargs)
+
+
+def Ground(**kwargs) -> Signal:
+    """# Ground Signal Constructor
+    Thin wrapper around `hdl21.Signal`"""
+    return Signal(usage=Usage.GROUND, **kwargs)
+
+
+def Clock(**kwargs) -> Signal:
+    """# Clock Signal Constructor
+    Thin wrapper around `hdl21.Signal`"""
+    return Signal(usage=Usage.CLOCK, **kwargs)
+
+
+"""
+# Plural Constructors
+
+Wrappers that generate the functions named `Signals`, `Ports`, and the like. 
+"""
+
 
+def _pluralize(fn: Callable):
+    """Inner helper method for creating "plural" versions of `Signal` constructors."""
 
-def _plural(*, fn: Callable, num: int, **kwargs) -> List[Signal]:
-    """Internal helper method for creating `num` identical `Signal` objects via callable `fn`."""
-    rv = list()
-    for _ in range(num):
-        rv.append(fn(**kwargs))
-    return rv
+    def _plural(num: int, **kwargs) -> List[Signal]:
+        return [fn(**kwargs) for _ in range(num)]
+
+    # Give the wrapper a plural name, e.g. "Signals" or "Clocks"
+    _plural.__name__ = fn.__name__ + "s"
+    # And a basic doc string
+    _plural.__doc__ = f"Create `num` new {fn.__name__}s."
+    # Add the wrapper to this module's namespace
+    globals()[_plural.__name__] = _plural
+
+
+# Create all those plural versions
+[_pluralize(fn) for fn in [Signal, Port, Input, Output, Inout, Power, Ground, Clock]]
+
+
+"""
+# Non-public (well, at least in intent) Methods
+"""
+
+
+def _copy_to_internal(sig: Signal) -> Signal:
+    """Make a copy of `sig`, replacing its visibility and port-direction to be internal."""
+    sig = copy(sig)
+    sig.vis = Visibility.INTERNAL
+    sig.direction = PortDir.NONE
+    sig._parent_module = None
+    return sig
```

### Comparing `hdl21-3.0.dev3/hdl21/sim/data.py` & `hdl21-4.0.0rc0/hdl21/sim/data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Spice-Class Simulation Interface 
 """
 
-from decimal import Decimal
+from textwrap import dedent
+from warnings import warn
 from enum import Enum
-from typing import Union, Any, Optional, List, Sequence, Awaitable
+from typing import Union, Any, Optional, List, Awaitable, Dict
 from pathlib import Path
 from dataclasses import field
 
 import vlsirtools.spice as vsp
 
 # Create a few aliases to the VLSIR sim-results types
 from vlsirtools.spice import SimResultUnion
@@ -35,15 +36,15 @@
     a single, scalar, undirected Port named "VSS"."""
     tb = Module(name=name)
     tb.VSS = Port(width=1)
     return tb
 
 
 def is_tb(i: Instantiable) -> bool:
-    """Boolean indication of whether Module `m` meets the test-bench interface."""
+    """Boolean indication of whether Instantiable `m` meets the test-bench interface."""
     if isinstance(i, (Module, ExternalModuleCall)):
         m = i
     elif isinstance(i, GeneratorCall):
         m = i.result
     else:
         raise TypeError(f"Invalid un-instantiable argument {i} to `is_tb`")
 
@@ -328,27 +329,30 @@
 Control = Union[Include, Lib, Save, Meas, Param, Literal]
 
 
 def is_control(val: Any) -> bool:
     return isinstance(val, Control.__args__)
 
 
+# Define all available option types below
+OptionTypes = Union[
+    bool,
+    Scalar,
+    str,
+    Literal,
+]
+
+
 @simattr
 @datatype
 class Options:
     """Simulation Options"""
 
-    temper: Optional[int] = None  # Temperature
-    tnom: Optional[int] = None  # Nominal temperature
-    # FIXME NOTE: these three will in short order become `Scalar`s!
-    gmin: Optional[float] = None
-    reltol: Optional[float] = None
-    iabstol: Optional[float] = None
-
-    name: Optional[str] = None  # Name, used in class-based `Sim` definitions
+    value: OptionTypes
+    name: str
 
 
 # Spice-Sim Attribute-Union
 SimAttr = Union[Analysis, Control, Options]
 
 
 def is_simattr(val: Any) -> bool:
@@ -373,48 +377,63 @@
     name: Optional[str] = None
 
     def add(self, *attrs: List[SimAttr]) -> OneOrMore[SimAttr]:
         """Add one or more `SimAttr`s to the simulation.
         Returns the inserted attributes, either as a list or a single `SimAttr`."""
         for attr in attrs:
             if not is_simattr(attr):
-                raise TypeError
+                raise TypeError(f"Invalid Sim attribute: {attr} being added to {self}")
             self.attrs.append(attr)
         if len(attrs) == 1:
             return attrs[0]
         return list(attrs)
 
     def run(self, opts: Optional[vsp.SimOptions] = None) -> vsp.SimResultUnion:
         """Invoke simulation via `vlsirtools.spice`."""
         return run(self, opts=opts)
 
-    async def run_async(
-        self, opts: Optional[vsp.SimOptions] = None
-    ) -> Awaitable[vsp.SimResultUnion]:
-        """Invoke simulation via `vlsirtools.spice`."""
-        return run_async(self, opts=opts)
+    @property
+    def Tb(self) -> "Module":
+        """Get our testbench Module, with a class-style accessor name."""
+        # Many testbenches "look like" classes, so we provide a class-name-style accessor
+        return self.tb
 
 
 def run(
     inp: OneOrMore[Sim], opts: Optional[vsp.SimOptions] = None
 ) -> OneOrMore[vsp.SimResultUnion]:
     """Invoke one or more `Sim`s via `vlsirtools.spice`."""
 
     from .to_proto import to_proto
 
+    # FIXME: I don't see anything that relied on this, but whatever it was, has gotta go
+    # inp.Tb.props.set("simulator", opts.simulator.value)
+
     return vsp.sim(inp=to_proto(inp), opts=opts)
 
 
-async def run_async(
+def run_async(
     inp: OneOrMore[Sim], opts: Optional[vsp.SimOptions] = None
-) -> OneOrMore[Awaitable[vsp.SimResultUnion]]:
+) -> OneOrMore[vsp.SimResultUnion]:
     """Invoke simulation via `vlsirtools.spice`."""
     from .to_proto import to_proto
 
-    return await vsp.sim_async(inp=to_proto(inp), opts=opts)
+    # FIXME: go through with deprecation
+    warn(
+        PendingDeprecationWarning(
+            dedent(
+                """\
+        Async `hdl21.Sim` invocation will be deprecated and `run_async` will be removed with the next major version.
+        Use `run` instead, which now parallelizes across simulation processes internally.
+    """
+            )
+        )
+    )
+
+    return vsp.sim(inp=to_proto(inp), opts=opts)
 
 
 def _add_attr_func(name: str, cls: type):
     # Create the internal "construct + add" closure
     def _method(self, *args, **kwargs):
         inst = cls(*args, **kwargs)
         self.add(inst)
@@ -474,16 +493,19 @@
         fast_lib = Lib(path=a_path, section="fast")
     ```
 
     Class-based `Sim` definitions retain all class members which are `SimAttr`s and drop all others.
     Non-`SimAttr`-valued fields can nonetheless be handy for defining intermediate values upon which the ultimate SimAttrs depend,
     such as the `a_path` field in the example aboe.
 
-    Classes decoratated by `sim` a single special required field:
-    a `tb` attribute which sets the simulation testbench.
+    Classes decoratated by `sim` a single special required field,
+    named either `tb` or `Tb`, which sets the simulation testbench.
+    Valid testbenches must adhere to "the testbench IO interface":
+    a single, width-one port, nominally named "VSS", and expected to be connected from "simulator ground" to the DUT's ground.
+    Testbench attributes which fail to adhere to this interface will cause a `RuntimeError`.
 
     Several other names are disallowed in `sim` class-definitions,
     generally corresponding to the names of the `Sim` class's fields and methods.
     Disallowed names include: `["attrs", "add", "run", "namespace"]`.
     """
 
     if cls.__bases__ != (object,):
@@ -502,30 +524,33 @@
     # This can nonetheless be handy for defining intermediate values upon which the ultimate SimAttrs depend.
     forgetme: List[Any] = list()
 
     # Take a lap through the class dictionary, type-check everything and assign relevant attributes to the sim
     for key, val in cls.__dict__.items():
         if key in protected_names:
             raise RuntimeError(f"Invalid field name {key} in Sim {cls}")
-        elif key == "tb":  # Set the test-bench attribute
+        elif key in ("tb", "Tb"):  # Set the test-bench attribute
             tb = val
         elif key == "name":  # Set the sim-name attribute
             name = val
         elif is_simattr(val):
             # Add to the sim-attributes list
             # Special case Python's conventional "ignored" name, the underscore.
             # Leave attributes named "_"'s `name` field set to `None`.
             if key != "_":
                 val.name = key
             attrs.append(val)
         else:  # Add to the forget-list
             forgetme.append(val)
 
+    # Validate the testbench module
     if tb is None:
         raise RuntimeError(f"No `tb` defined in Sim {cls}")
+    if not is_tb(tb):
+        raise RuntimeError(f"Invalid testbench {tb} in Sim {cls}")
 
     # Create the `Sim` object
     name = name or cls.__name__
     sim = Sim(name=name, tb=tb, attrs=attrs)
 
     # And return the `Sim`
     return sim
```

### Comparing `hdl21-3.0.dev3/hdl21/sim/delay.py` & `hdl21-4.0.0rc0/hdl21/sim/delay.py`

 * *Files identical despite different names*

### Comparing `hdl21-3.0.dev3/hdl21/sim/tests/test_sim.py` & `hdl21-4.0.0rc0/hdl21/sim/tests/test_sim.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,20 @@
+"""
+# `hdl21.sim` Unit Tests
+"""
+
+import pytest
+
 import hdl21 as h
 from hdl21.sim import *
-from hdl21.primitives import Vdc
 from hdl21.prefix import m
+from hdl21.primitives import Vdc
+import vlsir.spice_pb2 as vsp
 import vlsirtools
-import pytest
+from vlsirtools.spice import sim, SimOptions, ResultFormat, sim_data as sd
 
 
 def test_sim1():
     """Test minimal `Sim` creation"""
     s = Sim(tb=tb("empty"), attrs=[])
     assert isinstance(s, Sim)
     assert s.tb.name == "empty"
@@ -52,15 +59,15 @@
                 npts=11,
                 name="mymc",
             ),
             Save(SaveMode.ALL),
             Meas(analysis="mytr", name="a_delay", expr="trig_targ_something"),
             Include("/home/models"),
             Lib(path="/home/models", section="fast"),
-            Options(reltol=1e-9),
+            Options(1e-9, name="reltol"),
         ],
     )
     to_proto(s)
 
 
 def test_simattrs():
     """Test the "sim attrs" feature, which adds methods to `Sim` for each `SimAttr`"""
@@ -73,28 +80,28 @@
     tr = s.tran(tstop=11 * h.prefix.p, name="mytran")
     noise = s.noise(
         output=MyTb.p,
         input_source=MyTb.v,
         sweep=LogSweep(1e1, 1e10, 10),
         name="mynoise",
     )
-    assert tr.tstop == h.Scalar.new(11 * h.prefix.p)
+    assert tr.tstop == 11 * h.prefix.p
     sw = s.sweepanalysis(inner=[tr], var=p, sweep=LinearSweep(0, 1, 2), name="mysweep")
     mc = s.montecarlo(
         inner=[
             Dc(var="y", sweep=PointSweep([1]), name="swpdc"),
         ],
         npts=11,
         name="mymc",
     )
     s.save(SaveMode.ALL)
     s.meas(analysis=tr, name="a_delay", expr="trig_targ_something")
     s.include("/home/models")
     s.lib(path="/home/models", section="fast")
-    s.options(reltol=1e-9)
+    s.options(1e-9, name="reltol")
 
     to_proto(s)
 
 
 def test_sim_decorator():
     """Test creating the same Sim, via the class decorator"""
 
@@ -120,15 +127,15 @@
         mymc = MonteCarlo(
             inner=[
                 Dc(var="y", sweep=PointSweep([1]), name="swpdc"),
             ],
             npts=11,
         )
         a_delay = Meas(analysis=mytran, expr="trig_targ_something")
-        opts = Options(reltol=1e-9)
+        opts = Options(1e-9, name="reltol")
 
         # Attributes whose names don't really matter can be called anything,
         # but must be *assigned* into the class, not just constructed.
         _ = Save(SaveMode.ALL)
 
         # The `a_path` field will be dropped from the `Sim` definition,
         # but can be referred to by the following attributes.
@@ -179,15 +186,15 @@
                 npts=11,
                 name="mymc",
             ),
             Save(SaveMode.ALL),
             Meas(analysis="mytr", name="a_delay", expr="trig_targ_something"),
             Include("/home/models"),
             Lib(path="/home/models", section="fast"),
-            Options(reltol=1e-9),
+            Options(1e-9, name="reltol"),
         ],
     )
 
     p = to_proto(s)
 
     import vlsir.circuit_pb2 as vckt
     import vlsir.spice_pb2 as vsp
@@ -254,15 +261,15 @@
         pathsep=":",
     )
     delay_sim = delay.create_sim(p)
     h.sim.to_proto(delay_sim)
     # FIXME! some real checks plz
 
 
-def empty_tb() -> h.Module:
+def empty_tb(num=0) -> h.Module:
     from hdl21.prefix import K
     from hdl21.primitives import R
 
     ri = R(R.Params(r=1 * K))
 
     @h.module
     class EmptyTb:
@@ -270,29 +277,25 @@
         or as close as we can get to one without some simulators failing.
         AKA, a resistor to ground."""
 
         VSS = h.Port()
         s = h.Signal()
         r = ri(p=s, n=VSS)
 
-    EmptyTb.name = "EmptyTb"
+    EmptyTb.name = f"EmptyTb{num}"
     return EmptyTb
 
 
 @pytest.mark.skipif(
     vlsirtools.spice.default() is None,
     reason="No simulator available",
 )
 def test_empty_sim1():
     """Create and run an empty `Sim`, returning a VLSIR_PROTO"""
 
-    from hdl21.sim import Sim, to_proto
-    import vlsir.spice_pb2 as vsp
-    from vlsirtools.spice import sim, SimOptions, ResultFormat, sim_data as sd
-
     s = Sim(tb=empty_tb(), attrs=[])
     r = sim(to_proto(s), SimOptions(fmt=ResultFormat.VLSIR_PROTO))
     assert isinstance(r, vsp.SimResult)
     assert not len(r.an)  # No analysis inputs, no analysis results
 
 
 @pytest.mark.skipif(
@@ -302,15 +305,46 @@
 @pytest.mark.skipif(
     vlsirtools.spice.default() == vlsirtools.spice.SupportedSimulators.XYCE,
     reason="No support for `Xyce` + `SimData` python types",
 )
 def test_empty_sim2():
     """Create and run an empty `Sim`, returning SIM_DATA"""
 
-    from hdl21.sim import Sim, to_proto
-    import vlsir.spice_pb2 as vsp
-    from vlsirtools.spice import sim, SimOptions, ResultFormat, sim_data as sd
-
     s = Sim(tb=empty_tb(), attrs=[])
     r = sim(to_proto(s), SimOptions(fmt=ResultFormat.SIM_DATA))
     assert isinstance(r, sd.SimResult)
     assert not len(r.an)  # No analysis inputs, no analysis results
+
+
+@pytest.mark.xfail(reason="VLSIR #71 https://github.com/Vlsir/Vlsir/issues/71")
+def test_multi_sim():
+    """Test multiple Sims in parallel"""
+    s1 = Sim(tb=empty_tb(1), attrs=[])
+    s2 = Sim(tb=empty_tb(2), attrs=[])
+    s3 = Sim(tb=empty_tb(3), attrs=[])
+    s4 = Sim(tb=empty_tb(4), attrs=[])
+
+    r = sim(to_proto([s1, s2, s3, s4]), SimOptions(fmt=ResultFormat.VLSIR_PROTO))
+
+    for a in r:
+        assert isinstance(a, vsp.SimResult)
+        assert not len(a.an)
+
+
+def really_empty_tb() -> h.Module:
+    @h.module
+    class ReallyEmptyTb:
+        """An Empty TestBench, this time REALLY empty.
+        For inducing an error in a multi-sim below."""
+
+    return ReallyEmptyTb
+
+
+def test_multi_sim_error():
+    """Test that a failure in multiple concurrent sims fails, unlike in erdewit/nest_asyncio#57"""
+    with pytest.raises(Exception):
+        s1 = Sim(tb=empty_tb(1), attrs=[])
+        s2 = Sim(tb=really_empty_tb(), attrs=[])
+        s3 = Sim(tb=empty_tb(3), attrs=[])
+        s4 = Sim(tb=empty_tb(4), attrs=[])
+
+        r = sim(to_proto([s1, s2, s3, s4]), SimOptions(fmt=ResultFormat.VLSIR_PROTO))
```

### Comparing `hdl21-3.0.dev3/hdl21/sim/to_proto.py` & `hdl21-4.0.0rc0/hdl21/sim/to_proto.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import vlsir
 import vlsir.circuit_pb2 as vckt
 import vlsir.spice_pb2 as vsp
 
 # Local Imports
 from ..one_or_more import OneOrMore
 from . import data
+from ..literal import Literal
 from ..prefix import Prefixed
 from ..scalar import Scalar
 from ..signal import Signal
 from ..connect import is_connectable
 
 
 def to_proto(inp: OneOrMore[data.Sim]) -> OneOrMore[vsp.SimInput]:
@@ -270,36 +271,34 @@
             )
         else:
             raise TypeError(f"Invalid Sweep value {sweep}")
 
 
 def export_options(options: data.Options) -> vsp.SimOptions:
     """Export simulation options"""
-    return vsp.SimOptions(
-        temp=options.temper,
-        tnom=options.tnom,
-        gmin=options.gmin,
-        iabstol=options.iabstol,
-        reltol=options.reltol,
-    )
+    from ..proto.to_proto import export_param_value
+
+    return vsp.SimOptions(name=options.name, value=export_param_value(options.value))
 
 
 def export_control(ctrl: data.Control) -> vsp.Control:
     """Export a `Control` element"""
+    from ..proto.to_proto import export_literal
+
     if isinstance(ctrl, data.Include):
         return vsp.Control(include=export_include(ctrl))
     if isinstance(ctrl, data.Lib):
         return vsp.Control(lib=export_lib(ctrl))
     if isinstance(ctrl, data.Save):
         return vsp.Control(save=export_save(ctrl))
     if isinstance(ctrl, data.Meas):
         return vsp.Control(meas=export_meas(ctrl))
     if isinstance(ctrl, data.Param):
         return vsp.Control(param=export_param(ctrl))
-    if isinstance(ctrl, data.Literal):
+    if isinstance(ctrl, Literal):
         return vsp.Control(literal=export_literal(ctrl))
     raise TypeError(f"Invalid Sim Control {ctrl}")
 
 
 def export_include(inc: data.Include) -> vsp.Include:
     return vsp.Include(path=str(inc.path))
 
@@ -351,19 +350,14 @@
 def export_param(param: data.Param) -> vlsir.Param:
     """Export a parameter declaration"""
     from ..proto.to_proto import export_param_value
 
     return vlsir.Param(name=param.name, value=export_param_value(param.val))
 
 
-def export_literal(literal: data.Literal) -> str:
-    """Export a simulation literal, as its text value"""
-    return literal.txt
-
-
 def export_float(num: Union[float, int, Decimal, Prefixed, Scalar]) -> float:
     """Export a `Number` union-type to a float, or protobuf float/double."""
     if num is None:
         # FIXME: this is the protobuf default, but we really wanna make fields that use it optional
         return 0.0
     if isinstance(num, float):
         return num
```

### Comparing `hdl21-3.0.dev3/hdl21/slice.py` & `hdl21-4.0.0rc0/hdl21/slice.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         return _get_inner(self).width
 
     def __repr__(self):
         return f"Slice(parent={self.parent}, index={self.index})"
 
     def __eq__(self, other) -> bool:
         # Identity is equality
-        return id(self) == id(other)
+        return other is self
 
     def __hash__(self) -> bool:
         # Identity is equality
         return hash(id(self))
 
 
 @datatype
```

### Comparing `hdl21-3.0.dev3/hdl21/sliceable.py` & `hdl21-4.0.0rc0/hdl21/sliceable.py`

 * *Files identical despite different names*

### Comparing `hdl21-3.0.dev3/hdl21/source_info.py` & `hdl21-4.0.0rc0/hdl21/source_info.py`

 * *Files identical despite different names*

### Comparing `hdl21-3.0.dev3/hdl21/tests/content.py` & `hdl21-4.0.0rc0/hdl21/tests/content.py`

 * *Files identical despite different names*

### Comparing `hdl21-3.0.dev3/hdl21/tests/test_builtin_generators.py` & `hdl21-4.0.0rc0/hdl21/tests/test_builtin_generators.py`

 * *Files identical despite different names*

### Comparing `hdl21-3.0.dev3/hdl21/tests/test_bundles.py` & `hdl21-4.0.0rc0/hdl21/tests/test_bundles.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 # Hdl21 Unit Tests
 
 Not necessarily exclusive to `Bundle`s, but focusing on them.
 """
 import copy, pytest
-from enum import Enum, EnumMeta, auto
+from enum import Enum, auto
 
 import hdl21 as h
 
 
 def test_bundle1():
     # Create an bundle
 
@@ -112,26 +112,28 @@
 
     @h.bundle
     class HasRoles:  # An Bundle with Roles
         class Roles(Enum):  # USB-Style Role Nomenclature
             HOST = auto()
             DEVICE = auto()
 
+        Roles = h.RoleSet.from_enum(Roles)
+
         # Create signals going in either direction
         tx = h.Signal(src=Roles.HOST, dest=Roles.DEVICE)
         rx = h.Signal(src=Roles.DEVICE, dest=Roles.HOST)
 
         # And create differential versions thereof
         txd = Diff(src=Roles.HOST, dest=Roles.DEVICE)
         rxd = Diff(src=Roles.DEVICE, dest=Roles.HOST)
 
     hr = HasRoles()
     assert isinstance(HasRoles, h.Bundle)
-    assert isinstance(HasRoles.roles, EnumMeta)
-    assert isinstance(HasRoles.Roles, EnumMeta)
+    assert isinstance(HasRoles.roles, h.RoleSet)
+    assert isinstance(HasRoles.Roles, h.RoleSet)
     assert isinstance(hr, h.BundleInstance)
     assert isinstance(HasRoles.tx, h.Signal)
     assert isinstance(HasRoles.rx, h.Signal)
     assert isinstance(HasRoles.txd, h.BundleInstance)
     assert isinstance(HasRoles.rxd, h.BundleInstance)
 
     @h.module
@@ -172,85 +174,77 @@
     assert "host_hr_rxd_p" in sys.namespace
     assert "host_hr_rxd_n" in sys.namespace
 
 
 def test_bigger_bundles():
     """Test a slightly more elaborate Bundle-based system"""
 
+    @h.roleset
     class HostDevice(Enum):
+        # A pair of roles `Host` and `Device`, as commonly used by USB, JTAG, and similar buses.
         HOST = auto()
         DEVICE = auto()
 
     @h.bundle
     class Jtag:
         # Jtag Bundle
-
         roles = HostDevice
         tck, tdi, tms = h.Signals(3, src=roles.HOST, dest=roles.DEVICE)
         tdo = h.Signal(src=roles.DEVICE, dest=roles.HOST)
 
     @h.bundle
     class Uart:
         # Uart Bundle
-        class Roles(Enum):
-            # Uart roles are essentially peers, here named `ME` and `YOU`.
-            # Essentially everything will use the role `ME`,
-            # except for interconnect which swaps between the two.
-            ME = auto()
-            YOU = auto()
-
-        tx = h.Signal(src=Roles.ME, dest=Roles.YOU)
-        rx = h.Signal(src=Roles.YOU, dest=Roles.ME)
+        # Note the UART bundle is not role-based; `tx` is always output, `rx` is always input.
+        tx = h.Output()
+        rx = h.Input()
 
     @h.bundle
     class Spi:
         # Spi Bundle
         roles = HostDevice
         sck, cs = h.Signals(2, src=roles.HOST, dest=roles.DEVICE)
         dq = h.Signal(src=roles.DEVICE, dest=roles.HOST, width=4)
 
     @h.module
     class Chip:
         spi = Spi(role=HostDevice.HOST, port=True)
         jtag = Jtag(role=HostDevice.DEVICE, port=True)
-        uart = Uart(role=Uart.Roles.ME, port=True)
+        uart = Uart(port=True)
         ...  # Actual internal content, which likely connects these down *many* levels of hierarchy
 
     @h.module
     class SpiFlash:
         # A typical flash memory with a SPI port
         spi = Spi(role=HostDevice.DEVICE, port=True)
 
     @h.module
     class Board:
         # A typical embedded board, featuring a custom chip, SPI-connected flash, and JTAG port
         jtag = Jtag(role=HostDevice.DEVICE, port=True)
-        uart = Uart(role=Uart.Roles.ME, port=True)
+        uart = Uart(port=True)
 
         chip = Chip(jtag=jtag, uart=uart)
         flash = SpiFlash(spi=chip.spi)
 
     @h.module
     class Tester:
         # A typical test-widget with a JTAG port
         jtag = Jtag(role=HostDevice.HOST, port=True)
-        uart = Uart(role=Uart.Roles.ME, port=True)
+        uart = Uart(port=True)
 
     @h.module
     class TestSystem:
         # A system in which `Tester` can test `Board`
         jtag = Jtag()
-
-        tester = Tester(jtag=jtag)
-        board = Board(jtag=jtag)
-
-        # Connect UART, swapping `rx` and `tx`
         u0, u1 = h.Signals(2)
-        board.uart = h.AnonymousBundle(tx=u0, rx=u1)
-        tester.uart = h.AnonymousBundle(rx=u0, tx=u1)
+
+        # Connect the two, swapping UART `rx` and `tx`
+        board = Board(jtag=jtag, uart=h.bundlize(tx=u0, rx=u1))
+        tester = Tester(jtag=jtag, uart=h.bundlize(tx=u1, rx=u0))
 
     assert isinstance(TestSystem.jtag, h.BundleInstance)
     assert isinstance(TestSystem.tester, h.Instance)
     assert isinstance(TestSystem.board, h.Instance)
 
     assert isinstance(TestSystem.tester.uart, h.PortRef)
     assert isinstance(TestSystem.board.uart, h.PortRef)
@@ -686,7 +680,168 @@
     assert Top.bot1.conns["c_s2"] is Top.bot1_c_s2
     assert Top.bot1.conns["c_s3"] is Top.bot1_c_s3
 
     assert Top.bot2.conns["b_s1"] is Top.bot2_b_s1
     assert Top.bot2.conns["c_s1"] is Top.bot2_c_s1
     assert Top.bot2.conns["c_s2"] is Top.bot2_c_s2
     assert Top.bot2.conns["c_s3"] is Top.bot2_c_s3
+
+
+def test_structured_roles():
+    """Test creating structured Bundle Roles"""
+
+    @h.bundle
+    class MyBundle:
+        Host, Device = 2 * h.Role()
+
+    class HostDeviceEnum(Enum):
+        Host = auto()
+        Device = auto()
+
+    HostDevice = h.RoleSet.from_enum(HostDeviceEnum)
+
+    @h.module
+    class HostModule:
+        mb = MyBundle(role=HostDevice.Host, port=True)
+        # FIXME: not this part, at least not yet
+        # mb = MyBundle.Host()
+
+    @h.module
+    class DeviceModule:
+        mb = MyBundle(role=HostDevice.Device, port=True)
+        # FIXME: not this part, at least not yet
+        # mb = MyBundle.Host()
+
+    @h.module
+    class Top:
+        host = HostModule()
+        device = DeviceModule(mb=host.mb)
+
+    h.elaborate(Top)
+
+    @h.bundle
+    class AnotherBundle:
+        roles = HostDevice
+
+    @h.bundle
+    class YetAnotherBundle:
+        Roles = HostDevice  # Capital R also works
+
+    assert AnotherBundle.roles is HostDevice
+    assert AnotherBundle.Roles is HostDevice
+    assert YetAnotherBundle.roles is HostDevice
+    assert YetAnotherBundle.Roles is HostDevice
+
+
+def test_flipped():
+    """Test bundles with directed ports, and direction-flips thereof"""
+
+    from hdl21.bundle import flippable
+
+    @h.bundle
+    class Empty:
+        ...  # like it says, empty
+
+    assert flippable(Empty)
+
+    @h.bundle
+    class NoFlip:
+        s = h.Signal()
+
+    assert not flippable(NoFlip)
+
+    @h.bundle
+    class B:
+        i = h.Input()
+        o = h.Output()
+        io = h.Inout()
+        p = h.Port()
+
+    assert flippable(B)
+
+    @h.module
+    class M:
+        b = B(port=True)
+
+    @h.module
+    class F:
+        b = B(port=True, flipped=True)
+
+    @h.module
+    class Top:
+        m = M()
+        f = F(b=m.b)
+
+    h.elaborate(Top)
+
+    assert M.b_i.vis == h.Visibility.PORT
+    assert M.b_i.direction == h.PortDir.INPUT
+    assert M.b_o.vis == h.Visibility.PORT
+    assert M.b_o.direction == h.PortDir.OUTPUT
+    assert M.b_io.vis == h.Visibility.PORT
+    assert M.b_io.direction == h.PortDir.INOUT
+    assert M.b_p.vis == h.Visibility.PORT
+    assert M.b_p.direction == h.PortDir.NONE
+
+    assert F.b_i.vis == h.Visibility.PORT
+    assert F.b_i.direction == h.PortDir.OUTPUT
+    assert F.b_o.vis == h.Visibility.PORT
+    assert F.b_o.direction == h.PortDir.INPUT
+    assert F.b_io.vis == h.Visibility.PORT
+    assert F.b_io.direction == h.PortDir.INOUT
+    assert F.b_p.vis == h.Visibility.PORT
+    assert F.b_p.direction == h.PortDir.NONE
+
+    assert Top.m_b_i.vis == h.Visibility.INTERNAL
+    assert Top.m_b_i.direction == h.PortDir.NONE
+    assert Top.m_b_o.vis == h.Visibility.INTERNAL
+    assert Top.m_b_o.direction == h.PortDir.NONE
+    assert Top.m_b_io.vis == h.Visibility.INTERNAL
+    assert Top.m_b_io.direction == h.PortDir.NONE
+    assert Top.m_b_p.vis == h.Visibility.INTERNAL
+    assert Top.m_b_p.direction == h.PortDir.NONE
+
+
+def test_nested_flipping():
+    """# Test nesting the `flipped` attribute"""
+
+    @h.bundle
+    class Base:
+        i = h.Input()
+        o = h.Output()
+
+    @h.bundle
+    class Nested:
+        b = h.flipped(Base())
+        ni = h.Input()
+        no = h.Output()
+
+    @h.bundle
+    class NestedSquared:
+        n = h.flipped(Nested())
+        n2i = h.Input()
+        n2o = h.Output()
+
+    @h.module
+    class M:
+        n = h.flipped(NestedSquared(port=True))
+
+    h.elaborate(M)
+
+    # Some of these are a mouthful!
+    # (That's the point of having nested Bundles really;
+    # the flattened versions look pretty bad.)
+
+    assert M.n_n2i.vis == h.Visibility.PORT
+    assert M.n_n2i.direction == h.PortDir.OUTPUT
+    assert M.n_n2o.vis == h.Visibility.PORT
+    assert M.n_n2o.direction == h.PortDir.INPUT
+
+    assert M.n_n_ni.vis == h.Visibility.PORT
+    assert M.n_n_ni.direction == h.PortDir.INPUT
+    assert M.n_n_no.vis == h.Visibility.PORT
+    assert M.n_n_no.direction == h.PortDir.OUTPUT
+
+    assert M.n_n_b_i.vis == h.Visibility.PORT
+    assert M.n_n_b_i.direction == h.PortDir.OUTPUT
+    assert M.n_n_b_o.vis == h.Visibility.PORT
+    assert M.n_n_b_o.direction == h.PortDir.INPUT
```

### Comparing `hdl21-3.0.dev3/hdl21/tests/test_conns.py` & `hdl21-4.0.0rc0/hdl21/tests/test_conns.py`

 * *Files identical despite different names*

### Comparing `hdl21-3.0.dev3/hdl21/tests/test_exports.py` & `hdl21-4.0.0rc0/hdl21/tests/test_exports.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 # Hdl21 Unit Tests
 
 * Exporting to VLSIR 
   * Ultimately to EDA formats 
 * Importing back from VLSIR
 """
 
-import sys, pytest
+import pytest
 from io import StringIO
 from types import SimpleNamespace
-from textwrap import dedent
+from copy import deepcopy
 
 # Import the PUT (package under test)
 import hdl21 as h
 import vlsir
 
 
 @pytest.mark.xfail(reason="#1 https://github.com/dan-fritchman/Hdl21/issues/1")
@@ -23,15 +23,15 @@
     c = h.Module(name="c")
     c.p = h.Input(width=2)
 
     p = h.Module(name="p")
     p.s = h.Signal(width=20)
     p.c = c(p=p.s[::10])  # Connect two of the 20 bits, with stride 10
 
-    h.netlist(h.to_proto(p), sys.stdout, fmt="verilog")
+    h.netlist(h.to_proto(p), StringIO(), fmt="verilog")
 
 
 def test_prim_proto1():
     # Test round-tripping primitives through proto
 
     @h.module
     class HasPrims:
@@ -288,15 +288,14 @@
     assert isinstance(ns.M1, h.Module)
     assert len(ns.M1.signals) == 0
     assert len(ns.M1.ports) == 0
     assert len(ns.M1.instances) == 0
 
 
 def test_proto_roundtrip2():
-
     # Create a child/leaf Module
     M1 = h.Module(name="M1")
     M1.i = h.Input()
     M1.o = h.Output()
     M1.p = h.Port()
 
     # Create an instantiating parent-module
@@ -396,17 +395,21 @@
     assert ".s(s)" in nl
     assert ".p(p)" in nl
     assert "endmodule // Top" in nl
 
     nl = StringIO()
     h.netlist(ppkg, nl, fmt="spice")
     nl = nl.getvalue()
-    assert ".SUBCKT Bot \n+ s_2 s_1 s_0 p" in nl
-    assert ".SUBCKT Top \n+ p" in nl
-    assert "xb \n+ s_2 s_1 s_0 p \n+ Bot" in nl
+    assert ".SUBCKT Bot" in nl
+    assert "+ s_2 s_1 s_0 p" in nl
+    assert ".SUBCKT Top" in nl
+    assert "+ p" in nl
+    assert "xb" in nl
+    assert "+ s_2 s_1 s_0 p" in nl
+    assert "+ Bot" in nl
 
 
 def test_spice_netlister():
     from hdl21.prefix import e
 
     @h.module
     class DUT:
@@ -497,15 +500,15 @@
     # Round-trip back from Proto to Modules
     rt = h.from_proto(ppkg)
     ns = rt.hdl21.tests.test_exports
     assert isinstance(ns.Caller, h.Module)
     assert isinstance(getattr(ns, "CallMeTwice"), h.Module)
 
 
-def test_rountrip_external_module():
+def test_roundtrip_external_module():
     """Test round-tripping `ExternalModule`s between Hdl21 and VLSIR Proto"""
 
     @h.paramclass
     class P:  # Our ExternalModule's parameter-type
         a = h.Param(dtype=int, desc="a", default=1)
         b = h.Param(dtype=str, desc="b", default="two")
 
@@ -519,7 +522,97 @@
     imported = h.from_proto(exported)
     h.to_proto(imported.hdl21.tests.test_exports.HasE)
 
 
 def test_module_with_no_python_module():
     # Issue #48 https://github.com/dan-fritchman/Hdl21/issues/48
     exec("import hdl21 as h; h.to_proto(h.Module(name='not_in_a_pymodule'))")
+
+
+def test_netlist_spicetypes():
+    """# Test netlisting `ExternalModule`s with `SpiceType`s"""
+    from hdl21.external_module import SpiceType
+    from vlsirtools.netlist import NetlistFormat
+
+    NmosModel = h.ExternalModule(
+        name="nmos_model",
+        port_list=deepcopy(h.Mos.port_list),
+        paramtype=h.HasNoParams,
+        spicetype=SpiceType.MOS,
+    )
+
+    @h.module
+    class HasSpiceTypes:
+        VSS = h.Signal()
+        the_model_inst = NmosModel()(d=VSS, g=VSS, s=VSS, b=VSS)
+
+    # Test netlisting in a handful of formats
+    # Do some basic checking - mostly against exceptions.
+    # But make sure the model-name got in there at least somewhere.
+
+    sio = StringIO()
+    h.netlist(HasSpiceTypes, sio, fmt=NetlistFormat.SPICE)
+    nl = sio.getvalue()
+    assert "nmos_model" in nl
+
+    sio = StringIO()
+    h.netlist(HasSpiceTypes, sio, fmt=NetlistFormat.XYCE)
+    nl = sio.getvalue()
+    assert "nmos_model" in nl
+
+    sio = StringIO()
+    h.netlist(HasSpiceTypes, sio, fmt=NetlistFormat.NGSPICE)
+    nl = sio.getvalue()
+    assert "nmos_model" in nl
+
+    sio = StringIO()
+    h.netlist(HasSpiceTypes, sio, fmt=NetlistFormat.SPECTRE)
+    nl = sio.getvalue()
+    assert "nmos_model" in nl
+
+
+def test_module_with_literals():
+    """# Test exporting modules with literals"""
+
+    @h.module
+    class HasLit:
+        a, b, c = h.Ports(3)
+
+    # Add the literals
+    HasLit.literals.extend(
+        [
+            h.Literal("generate some_terrible_verilog_code"),
+            h.Literal(".some_spice_attribute what=ever"),
+            h.Literal("PRAGMA: some_pragma"),
+        ]
+    )
+
+    # Test converting to proto
+    pkg = h.to_proto(HasLit)
+    pmod = pkg.modules[0]
+    assert isinstance(pmod, vlsir.circuit.Module)
+    assert pmod.name == "hdl21.tests.test_exports.HasLit"
+    assert len(pmod.ports) == 3
+    assert len(pmod.signals) == 3
+
+    assert pmod.literals == [l.text for l in HasLit.literals]
+    assert pmod.literals == [
+        "generate some_terrible_verilog_code",
+        ".some_spice_attribute what=ever",
+        "PRAGMA: some_pragma",
+    ]
+
+    dest = StringIO()
+    h.netlist(HasLit, dest)
+    assert "generate some_terrible_verilog_code" in dest.getvalue()
+    assert ".some_spice_attribute what=ever" in dest.getvalue()
+    assert "PRAGMA: some_pragma" in dest.getvalue()
+
+    # Test round-tripping
+    ns = h.from_proto(pkg)
+    assert isinstance(ns, SimpleNamespace)
+    ns = ns.hdl21.tests.test_exports
+    assert isinstance(ns, SimpleNamespace)
+    HasLitRoundTripped = ns.HasLit
+    assert isinstance(HasLitRoundTripped, h.Module)
+    assert len(HasLitRoundTripped.literals) == 3
+    assert HasLitRoundTripped.literals == HasLit.literals
```

### Comparing `hdl21-3.0.dev3/hdl21/tests/test_hdl21.py` & `hdl21-4.0.0rc0/hdl21/tests/test_hdl21.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import copy, pytest
 from enum import Enum, EnumMeta, auto
 
 import hdl21 as h
 
 
 def test_version():
-    assert h.__version__ == "2.0.dev0"
+    assert h.__version__ == "4.0.0rc0" # NOTE: VLSIR_VERSION
 
 
 def test_module1():
     """Initial Module Test"""
 
     @h.module
     class M1:
@@ -409,34 +409,69 @@
     P.s4 = h.Signal(width=4)
     P.s2 = h.Signal(width=2)
     P.ic = C(p1=P.s4[0], p4=P.s4, p7=h.Concat(P.s4, P.s2, P.s2[0]))
 
     h.elaborate(P)
 
 
-def test_module_as_param():
-    """Test using a `Module` as a parameter-value"""
+def test_instantiable_as_param():
+    """Test using each Instantiable type as a parameter-value."""
 
     @h.paramclass
-    class HasModuleParam:
-        m = h.Param(dtype=h.Module, desc="A `Module` provided as a parameter")
-        e = h.Param(
-            dtype=h.ExternalModule, desc="An `ExternalModule` provided as a parameter"
-        )
+    class Params:
+        m = h.Param(dtype=h.Module, desc="A `Module`")
+        e = h.Param(dtype=h.ExternalModule, desc="An `ExternalModule`")
+        ec = h.Param(dtype=h.ExternalModuleCall, desc="An `ExternalModuleCall`")
+        # FIXME: `Generator` is the one exception here. Maybe it can work, some day.
+        # g = h.Param(dtype=h.Generator, desc="An `Generator`")
+        gc = h.Param(dtype=h.GeneratorCall, desc="An `GeneratorCall`")
+        p = h.Param(dtype=h.Primitive, desc="An `Primitive`")
+        pc = h.Param(dtype=h.PrimitiveCall, desc="An `PrimitiveCall`")
+        i = h.Param(dtype=h.Instantiable, desc="An `Instantiable`")
 
     @h.generator
-    def UsesModuleParam(params: HasModuleParam) -> h.Module:
-        return params.m  # Returns the Module unmodified
+    def UsesThemParams(params: Params) -> h.Module:
+        @h.module
+        class M:
+            x = h.Signal()
+
+            m = params.m(x=x)
+            e = params.e()(x=x)
+            ec = params.ec(x=x)
+            # g = params.g()(x=x)
+            gc = params.gc(x=x)
+            p = params.p()(d=x, g=x, s=x, b=x)
+            pc = params.pc(d=x, g=x, s=x, b=x)
+            i = params.i(x=x)
+
+        return M
 
     Mod = h.Module(name="Mod")
-    Emod = h.ExternalModule(name="Emod", port_list=[])
-    p = HasModuleParam(m=Mod, e=Emod)
-    m = UsesModuleParam(p)
+    Mod.x = h.Port()
+    Emod = h.ExternalModule(name="Emod", port_list=[h.Port(name="x")])
+
+    @h.generator
+    def Gen(_: h.HasNoParams) -> h.Module:
+        m = h.Module()
+        m.x = h.Port()
+        return m
+
+    p = Params(
+        m=Mod,
+        e=Emod,
+        ec=Emod(),
+        # g=Gen,
+        gc=Gen(),
+        p=h.Mos,
+        pc=h.Mos(),
+        i=Mod,
+    )
+    m = UsesThemParams(p)
     m = h.elaborate(m)
-    assert m == Mod
+    # assert m == Mod
 
 
 def test_instance_mult():
     """Initial tests of instance-array-generation by multiplication"""
 
     Child = h.Module(name="Child")
     Parent = h.Module(name="Parent")
@@ -711,15 +746,14 @@
         @h.Module  # Bad!
         class M:
             ...
 
     assert "Did you mean to use the `module` decorator?" in str(e)
 
     with pytest.raises(TypeError) as e:
-
         h.Module(2)  # Bad!
 
     assert "Invalid Module name" in str(e)
 
     with pytest.raises(TypeError) as e:
         ok = h.Module("ok")  # OK
         h.Module(ok)  # Bad!
@@ -1280,7 +1314,184 @@
     O.i1.b = O.i2.b = O.i3.b
 
     h.elaborate(O)
 
     assert list(O.signals.keys()) == ["i3_a", "i3_b"]
     assert O.i1.conns["a"] is O.i2.conns["a"] is O.i3.conns["a"] is O.i3_a
     assert O.i1.conns["b"] is O.i2.conns["b"] is O.i3.conns["b"] is O.i3_b
+
+
+def test_signal_usage():
+    """Test that the `usage` property of `Signal`s is set correctly."""
+
+    s = h.Signal()
+    assert s.usage == h.Usage.SIGNAL
+    p = h.Power()
+    assert p.usage == h.Usage.POWER
+    g = h.Ground()
+    assert g.usage == h.Usage.GROUND
+    c = h.Clock()
+    assert c.usage == h.Usage.CLOCK
+
+    s = h.Signals(2)
+    assert all(s.usage == h.Usage.SIGNAL for s in s)
+    p = h.Powers(3)
+    assert all(p.usage == h.Usage.POWER for p in p)
+    g = h.Grounds(4)
+    assert all(g.usage == h.Usage.GROUND for g in g)
+    c = h.Clocks(5)
+    assert all(c.usage == h.Usage.CLOCK for c in c)
+
+
+def test_properties():
+    """Test adding `Properties` to signals, modules, instances, and the like."""
+
+    s = h.Signal()
+
+    s.props.set("foo", "bar")
+    assert s.props.get("foo") == "bar"
+    assert s.props["foo"] == "bar"
+
+    s.props.set("foo", 4)
+    assert s.props.get("foo") == 4
+    assert s.props["foo"] == 4
+
+    with pytest.raises(TypeError):
+        s.props[3] = 4
+
+    with pytest.raises(TypeError):
+        s.props[TabError] = 11
+
+    with pytest.raises(TypeError):
+        s.props.set(key=None, val=5)
+
+    with pytest.raises(TypeError):
+        s.props.set(None, None)
+
+    with pytest.raises(TypeError):
+        s.props.get(None)
+
+    m = h.Module(name="m")
+    m.props["my_favorite_number"] = 42
+    assert m.props["my_favorite_number"] == 42
+
+    @h.module
+    class M:
+        ...
+
+    M.props["your_favorite_number"] = 11
+    assert M.props["your_favorite_number"] == 11
+
+    mi = M()
+    mi.props["abc"] = 123
+    assert mi.props["abc"] == 123
+
+    @h.bundle
+    class B:
+        ...
+
+    B.props["their_favorite_number"] = 3
+    assert B.props["their_favorite_number"] == 3
+
+    bi = B()
+    bi.props["xyz"] = None
+    assert bi.props["xyz"] is None
+
+
+def test_module_literals():
+    """Test adding `Literal`s to modules."""
+
+    @h.module
+    class HasLit:
+        x, y, z = 3 * h.Signal()
+
+    HasLit.literals.append(h.Literal("mother"))
+    HasLit.literals.append(h.Literal("father"))
+    HasLit.literals.extend(
+        [h.Literal("child"), h.Literal("uncle"), h.Literal("nephew")]
+    )
+
+    assert len(HasLit.signals) == 3
+    assert HasLit.literals == [
+        h.Literal(t) for t in ["mother", "father", "child", "uncle", "nephew"]
+    ]
+
+
+def test_signal_mult():
+    """# Test using the multiplication operator to create multiple `Signal`s."""
+
+    @h.module
+    class M:
+        a, b, c = 3 * h.Signal()
+        i1, i2 = 2 * h.Input()
+        o1, o2 = 2 * h.Output()
+        io1, io2 = 2 * h.Inout()
+        p1, p2, p3 = 3 * h.Port()
+
+    assert M.a is not M.b
+    assert M.a is not M.c
+    assert M.b is not M.c
+    assert M.i1 is not M.i2
+    assert M.o1 is not M.o2
+    assert M.io1 is not M.io2
+    assert M.p1 is not M.p2
+
+    assert len(M.ports) == 9
+    assert len(M.signals) == 3
+
+
+def test_bundle_mult():
+    """# Test using the multiplication operator to create multiple `BundleInstance`s."""
+
+    @h.bundle
+    class B:
+        i, q = 2 * h.Signal()
+
+    @h.module
+    class M:
+        b1, b2 = 2 * B()  # <= here's the test!
+
+    assert isinstance(M.b1, h.BundleInstance)
+    assert isinstance(M.b2, h.BundleInstance)
+    assert M.b1 is not M.b2
+
+    h.elaborate(M)
+
+    assert len(M.signals) == 4
+    assert M.b1_i is not M.b2_i
+    assert M.b1_q is not M.b2_q
+
+
+def test_set_bad_attrs():
+    """Test the "only allow setting known attributes" feature of a few types."""
+
+    @h.bundle
+    class B:
+        s = h.Signal()
+
+    # Create a `BundleInstance`
+    b = B()
+
+    # And assert we can't assign stuff to it
+    with pytest.raises(RuntimeError):
+        b.q = 5
+
+    # Create a `BundleRef` into that instance
+    ref = b.some_signal
+
+    # And assert we can't assign stuff to it
+    with pytest.raises(RuntimeError):
+        ref.whatever = 6
+
+    # Create an `AnonymousBundle`
+    bu = h.bundlize(a=h.Signal())
+
+    # And assert we can't assign stuff to it
+    with pytest.raises(RuntimeError):
+        bu.q = 5
+
+    # Create a `Concat`
+    c = h.Concat(h.Signal(), h.Signal())
+
+    # And assert we can't assign stuff to it
+    with pytest.raises(RuntimeError):
+        c.xyz = TabError
```

### Comparing `hdl21-3.0.dev3/hdl21/tests/test_params.py` & `hdl21-4.0.0rc0/hdl21/tests/test_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,15 +166,14 @@
             something = 11
 
     with pytest.raises(RuntimeError):
         # Test a bad argument type
         h.params._unique_name(33)
 
 
-@pytest.mark.xfail(reason="#30 https://github.com/dan-fritchman/Hdl21/issues/30")
 def test_param_default_factory():
     """Test the `default_factory` feature of `Param`"""
 
     # Test the pydantic versions without `paramclass` first
 
     @dataclass
     class NoFactory:
```

### Comparing `hdl21-3.0.dev3/hdl21/tests/test_prefix.py` & `hdl21-4.0.0rc0/hdl21/tests/test_prefix.py`

 * *Files 1% similar despite different names*

```diff
@@ -389,29 +389,29 @@
     class P:
         x: h.Prefixed
         y: h.Scalar
 
     # Test with int for each
     p = P(x=1, y=1)
     assert p.x == h.Prefixed(number=Decimal(1))
-    assert p.y.inner == h.Prefixed(number=Decimal(1))
+    assert p.y == h.Prefixed(number=Decimal(1))
 
     # Test with float for each
     p = P(x=3.0, y=3.0)
     assert p.x == h.Prefixed(number=Decimal(3.0))
-    assert p.y.inner == h.Prefixed(number=Decimal(3.0))
+    assert p.y == h.Prefixed(number=Decimal(3.0))
 
     # Test with str for each
     p = P(x="2e-9", y="2e-9")
     assert p.x == h.Prefixed(number=Decimal("2e-9"))
-    assert p.y == h.Scalar(inner=h.Prefixed(number=Decimal("2e-9")))
+    assert p.y == h.Prefixed(number=Decimal("2e-9"))
 
     # Test with an expression-literal for the `Scalar`
     p = P(x=11.11, y="m*x+b")
     assert p.x == h.Prefixed(number=11.11)
-    assert p.y == h.Scalar(inner=h.Literal(txt="m*x+b"))
+    assert p.y == h.Literal(text="m*x+b")
 
     # Test some invalid types
     with pt.raises(ValidationError):
         p = P(x=None, y=2)
     with pt.raises(ValidationError):
         p = P(x=3, y=None)
```

### Comparing `hdl21-3.0.dev3/hdl21/tests/test_source_info.py` & `hdl21-4.0.0rc0/hdl21/tests/test_source_info.py`

 * *Files identical despite different names*

### Comparing `hdl21-3.0.dev3/hdl21/walker.py` & `hdl21-4.0.0rc0/hdl21/walker.py`

 * *Files identical despite different names*

### Comparing `hdl21-3.0.dev3/hdl21.egg-info/PKG-INFO` & `hdl21-4.0.0rc0/hdl21.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,51 @@
 Metadata-Version: 2.1
 Name: hdl21
-Version: 3.0.dev3
+Version: 4.0.0rc0
 Summary: Hardware Description Library
 Home-page: https://github.com/dan-fritchman/Hdl21
 Author: Dan Fritchman
 Author-email: dan@fritch.mn
-Requires-Python: >=3.7, <4
+Requires-Python: >=3.7, <3.12
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # HDL21
 
 ## Analog Hardware Description Library in Python
 
+[![pypi](https://img.shields.io/badge/pypi-hdl21-blue)](https://pypi.org/project/hdl21/)
+[![python-versions](https://img.shields.io/badge/python-3.7_3.8_3.9_3.10_3.11-blue)](https://codecov.io/gh/dan-fritchman/Hdl21)
 [![test](https://github.com/dan-fritchman/Hdl21/actions/workflows/test.yaml/badge.svg)](https://github.com/dan-fritchman/Hdl21/actions/workflows/test.yaml)
 [![codecov](https://codecov.io/gh/dan-fritchman/Hdl21/branch/main/graph/badge.svg?token=f8LKUqEPdq)](https://codecov.io/gh/dan-fritchman/Hdl21)
 
-Hdl21 is a [hardware description library](https://en.wikipedia.org/wiki/Hardware_description_language) embedded in Python. It is targeted and optimized for analog and custom integrated circuits, and for maximum productivity with minimum fancy-programming skill.
-
-Hdl21 generates hardware databases in the [VLSIR](https://github.com/Vlsir/Vlsir) interchange formats, defined through [Google Protocol Buffers](https://developers.google.com/protocol-buffers/). Through [VLSIR's Python tools](https://pypi.org/project/vlsirtools/) Hdl21 also includes drivers for popular industry-standard data formats and popular spice-class simulation engines.
+Hdl21 is a [hardware description library](https://en.wikipedia.org/wiki/Hardware_description_language) embedded in Python.  
+It is targeted for analog and custom integrated circuits, and for maximum productivity with minimum fancy-programming skill.
 
 ## Contents
 
+- [Installation](#installation)
 - [Modules](#modules)
 - [Signals](#signals), [Ports](#signals), and [Connections](#connections)
 - [Generators](#generators) and [Parameters](#parameters)
+- [Primitive Elements and External Modules](#primitives-and-external-modules)
 - [Spice-Class Simulation](#spice-class-simulation)
-- [Primitive Elements](#primitives-and-external-modules)
-- [Process Technology (PDK) Packages](#process-technologies)
-- Coming Soon: Structured Connections with `Bundle`s
-- Coming Soon: [Schematics](https://github.com/Vlsir/Hdl21Schematics)
-- [Examples Library](#examples-library)
+- [Process Technologies (PDKs)](#process-technologies)
+- [Bundles](#bundles)
+- [Examples](#examples)
+- [Related Projects](#related-projects)
+
+## Installation
+
+```
+pip install hdl21
+```
+
+That's it. No crazy build step, no crazy dependencies, no crazy EDA stuff, no "clone and _just_ modify these 300 things", no `source`ing, none of that. Hdl21 is pure Python, and is designed to be as easy to install as any other Python package.
 
 ## Modules
 
 Hdl21's primary unit of hardware reuse is the `Module`. Think of it as Verilog's `module`, or VHDL's `entity`, or SPICE's `subckt`. Better yet if you are used to graphical schematics, think of it as the content of a schematic. Hdl21 `Modules` are containers of a handful of `hdl21` types. Think of them as including:
 
 - Instances of other `Modules`
 - Connections between them, defined by `Signals` and `Ports`
@@ -276,21 +286,46 @@
 o = Outer(**d1)
 # Convert back to another dictionary
 d2 = asdict(o)
 # And check they line up
 assert d1 == d2
 ```
 
+Generators include the capability to construct their param-classes inline, if provided a set of compatible keyword arguments. For example, defining a generator using the `MyParams` parameters above:
+
+```python
+@h.generator
+def MyGen(params: MyParams) -> h.Module:
+    ... # Create a `Module` & return it
+```
+
+This typical invocation:
+
+```python
+p = MyParams(width=8, text="My Favorite Module")
+MyGen(p)
+```
+
+is the same as calling:
+
+```python
+MyParams(width=8, text="My Favorite Module")
+```
+
+Parameters may be provided as keywords, or as a single positional argument which is an instance of the generator's param-class. Combinations of the two are not supported.
+
 ## A Note on Parametrization
 
 Hdl21 `Generators` have parameters. `Modules` do not.
 
 This is a deliberate decision, which in this sense makes `hdl21.Module` less feature-rich than the analogous `module` concepts in existing HDLs (Verilog, VHDL, and even SPICE). These languages support what might be called "static parameters" - relatively simple relationships between parent and child-module parameterization. Setting, for example, the width of a signal or number of instances in an array is straightforward. But more elaborate parametrization-cases are either highly cumbersome or altogether impossible to create. (As an example, try using Verilog parametrization to make a programmable-depth binary tree.) Hdl21, in contrast, exposes all parametrization to the full Python-power of its generators.
 
-## `Prefixed` Numeric Parameters
+## Numeric Parameters
+
+### `Prefixed` Numbers
 
 Hdl21 provides an [SI prefixed](https://www.nist.gov/pml/owm/metric-si-prefixes) numeric type `Prefixed`, which is especially common for physical generator parameters. Each `Prefixed` value is a combination of the Python standard library's `Decimal` and an enumerated SI `Prefix`:
 
 ```python
 @dataclass
 class Prefixed:
     number: Decimal  # Numeric Portion
@@ -301,15 +336,15 @@
 
 `Prefixed` values rarely need to be instantiated directly. Instead Hdl21 exposes a set of common prefixes via their typical single-character names:
 
 ```python
 f = FEMTO = Prefix.FEMTO
 p = PICO = Prefix.PICO
 n = NANO = Prefix.NANO
-µ = MICRO = Prefix.MICRO
+µ = u = MICRO = Prefix.MICRO # Note both `u` and `µ` are valid
 m = MILLI = Prefix.MILLI
 K = KILO = Prefix.KILO
 M = MEGA = Prefix.MEGA
 G = GIGA = Prefix.GIGA
 T = TERA = Prefix.TERA
 P = PETA = Prefix.PETA
 UNIT = Prefix.UNIT
@@ -340,17 +375,165 @@
 
 11 * e(-6) == 11 * µ  # True
 ```
 
 These `e()` values are also most common in multiplication expressions,
 to create `Prefixed` values in "floating point" style such as `11 * e(-9)`.
 
+### `Scalar`
+
+Many Hdl21 primitive parameters can be either numbers or string-literals.  
+The combination is so common that Hdl21 defines a `Scalar` type which is (roughly):
+
+```python
+Scalar = Union[Prefixed, Literal]
+```
+
+With automatic conversions from each of `str`, `int`, `float`, and `Decimal`.
+
+`Scalar` is particularly designed for parameter-values of `Primitive`s and of simulations.
+Most such parameters "want" to be the `Prefixed` type, for reasons outlined [above](#prefixed-numeric-parameters). They often also need a string-valued escape hatch, e.g. when referring to out-of-Hdl21 quantities
+such as parameters in external netlists or simulation decks.
+These out-of-Hdl21 expressions are represented by the `Literal` type, a simple wrapper around `str`.
+
+Where possible `Scalar` prefers to use the `Prefixed` variant.
+Built-in numbers `(int, float, Decimal)` are converted to `Prefixed` inline.
+Strings are attempted to be converted to `Prefixed`, and fall back to `Literal` if unsuccessful.
+This conversion process is also available as the free-standing `to_scalar()` function.
+
+Example:
+
+```python
+import hdl21 as h
+from hdl21.prefix import NANO, µ
+from decimal import Decimal
+
+@h.paramclass
+class MyMosParams:
+    w = h.Param(dtype=h.Scalar, desc="Width", default=1e-6) # Default `float` converts to a `Prefixed`
+    l = h.Param(dtype=h.Scalar, desc="Length", default="w/5") # Default `str` converts to a `Literal`
+
+# Example instantiations
+MyMosParams() # Default values
+MyMosParams(w=Decimal(1e-6), l=3*µ)
+MyMosParams(w=h.Literal("sim_param_width"), l=h.Prefixed.new(20, NANO))
+MyMosParams(w="11*l", l=11)
+```
+
+When defining "primitive level" parameters - e.g. those that will be used in PDK-level devices - `Scalar` is generally the best datatype to use.
+
+## Primitives and External Modules
+
+The leaf-nodes of each hierarchical Hdl21 circuit are generally defined in one of two places:
+
+- `Primitive` elements, defined in the `hdl21.primitives` package. Each is designed to be a technology-independent representation of an irreducible component.
+- `ExternalModules`, defined outside Hdl21. Such "module wrappers", which might alternately be called "black boxes", are common for including circuits from other HDLs.
+
+### `Primitives`
+
+Hdl21's library of generic primitive elements is defined in the `hdl21.primitives` package. Its content is roughly equivalent to that built into a typical SPICE simulator.
+
+A summary of `hdl21.primitives`:
+
+| Name                           | Description                       | Type     | Aliases                               | Ports        |
+| ------------------------------ | --------------------------------- | -------- | ------------------------------------- | ------------ |
+| Mos                            | Mos Transistor                    | PHYSICAL | MOS                                   | d, g, s, b   |
+| IdealResistor                  | Ideal Resistor                    | IDEAL    | R, Res, Resistor, IdealR, IdealRes    | p, n         |
+| PhysicalResistor               | Physical Resistor                 | PHYSICAL | PhyR, PhyRes, ResPhy, PhyResistor     | p, n         |
+| ThreeTerminalResistor          | Three Terminal Resistor           | PHYSICAL | Res3, PhyRes3, ResPhy3, PhyResistor3  | p, n, b      |
+| IdealCapacitor                 | Ideal Capacitor                   | IDEAL    | C, Cap, Capacitor, IdealC, IdealCap   | p, n         |
+| PhysicalCapacitor              | Physical Capacitor                | PHYSICAL | PhyC, PhyCap, CapPhy, PhyCapacitor    | p, n         |
+| ThreeTerminalCapacitor         | Three Terminal Capacitor          | PHYSICAL | Cap3, PhyCap3, CapPhy3, PhyCapacitor3 | p, n, b      |
+| IdealInductor                  | Ideal Inductor                    | IDEAL    | L, Ind, Inductor, IdealL, IdealInd    | p, n         |
+| PhysicalInductor               | Physical Inductor                 | PHYSICAL | PhyL, PhyInd, IndPhy, PhyInductor     | p, n         |
+| ThreeTerminalInductor          | Three Terminal Inductor           | PHYSICAL | Ind3, PhyInd3, IndPhy3, PhyInductor3  | p, n, b      |
+| PhysicalShort                  | Short-Circuit/ Net-Tie            | PHYSICAL | Short                                 | p, n         |
+| DcVoltageSource                | DC Voltage Source                 | IDEAL    | V, Vdc, Vsrc                          | p, n         |
+| PulseVoltageSource             | Pulse Voltage Source              | IDEAL    | Vpu, Vpulse                           | p, n         |
+| CurrentSource                  | Ideal DC Current Source           | IDEAL    | I, Idc, Isrc                          | p, n         |
+| VoltageControlledVoltageSource | Voltage Controlled Voltage Source | IDEAL    | Vcvs, VCVS                            | p, n, cp, cn |
+| CurrentControlledVoltageSource | Current Controlled Voltage Source | IDEAL    | Ccvs, CCVS                            | p, n, cp, cn |
+| VoltageControlledCurrentSource | Voltage Controlled Current Source | IDEAL    | Vccs, VCCS                            | p, n, cp, cn |
+| CurrentControlledCurrentSource | Current Controlled Current Source | IDEAL    | Cccs, CCCS                            | p, n, cp, cn |
+| Bipolar                        | Bipolar Transistor                | PHYSICAL | Bjt, BJT                              | c, b, e      |
+| Diode                          | Diode                             | PHYSICAL | D                                     | p, n         |
+
+Each primitive is available in the `hdl21.primitives` namespace, either through its full name or any of its aliases. Most primitives have fairly verbose names (e.g. `VoltageControlledCurrentSource`, `IdealResistor`), but also expose short-form aliases (e.g. `Vcvs`, `R`). Each of the aliases in Table 1 above refer to _the same_ Python object, i.e.
+
+```python
+from hdl21.primitives import R, Res, IdealResistor
+
+R is Res            # evaluates to True
+R is IdealResistor  # also evaluates to True
+```
+
+Hdl21 `Primitives` come in _ideal_ and _physical_ flavors. The difference is most frequently relevant for passive elements, which can for example represent either
+
+- (a) technology-specific passives, e.g. a MIM or MOS capacitor, or
+- (b) an _ideal_ capacitor
+
+Some element-types have solely physical implementations, some are solely ideal, and others include both.
+
+### `ExternalModules`
+
+Alternately Hdl21 includes an `ExternalModule` type which defines the interface to a module-implementation outside Hdl21. These external definitions are common for instantiating technology-specific modules and libraries. Think of them as a module "function header"; other popular modern HDLs refer to them as module _black boxes_.
+
+An example `ExternalModule`:
+
+```python
+import hdl21 as h
+from hdl21.prefix import µ
+from hdl21.primitives import Diode
+
+@h.paramclass
+class BandGapParams:
+    self_destruct = h.Param(
+        dtype=bool,
+        desc="Whether to include the self-destruction feature",
+        default=True,
+    )
+
+BandGap = h.ExternalModule(
+    name="BandGap",
+    desc="Example ExternalModule, defined outside Hdl21",
+    port_list=[h.Port(name="vref"), h.Port(name="enable")],
+    paramtype=BandGapParams,
+)
+```
+
+Both `Primitives` and `ExternalModules` have names, ordered `Ports`, and a few other pieces of metadata, but no internal implementation: no internal signals, and no instances of other modules. Unlike `Modules`, both _do_ have parameters. `Primitives` each have an associated `paramclass`, while `ExternalModules` can optionally declare one via their `paramtype` attribute. Their parameter-types are limited to a small subset of those possible for `Generators` - generally "scalar" types such as numbers, strings, and `Scalar` - primarily limited by the need to need to provide them to legacy HDLs. Parameters are applied in the same style as for `Generators`, by calling the `Primitive` or `ExternalModule`. Parameter-applications can either be an instance of the module's `paramtype` or a set of keyword arguments which validly contruct one inline.
+
+```python
+# Continuing from the snippet above:
+params = BandGapParams(self_destruct=False)  # Watch out there!
+```
+
+`Primitives` and `ExternalModules` can be instantiated and connected in all the same styles as `Modules`:
+
+```python
+@h.module
+class BandGapPlus:
+    vref, enable = h.Signals(2)
+    # Instantiate the `ExternalModule` defined above
+    bg = BandGap(params)(vref=vref, enable=enable)
+    # ...Anything else...
+
+@h.module
+class DiodePlus:
+    p, n = h.Signals(2)
+    # Parameterize, instantiate, and connect a `primitives.Diode`
+    d = Diode(w=1 * µ, l=1 * µ)(p=p, n=n)
+    # ... Everything else ...
+```
+
 ## Exporting and Importing
 
-Hdl21's primary import/ export format is [VLSIR](https://github.com/Vlsir/Vlsir). VLSIR is a binary ProtoBuf-based format with support for a variety of industry-standard formats and tools. The `hdl21.to_proto()` function converts an Hdl21 `Module` or group of `Modules` into VLSIR `Package`. The `hdl21.from_proto()` function similarly imports a VLSIR `Package` into a namespace of Hdl21 `Modules`.
+Hdl21 generates hardware databases in the [VLSIR](https://github.com/Vlsir/Vlsir) interchange formats, defined through [Google Protocol Buffers](https://developers.google.com/protocol-buffers/). Through [VLSIR's Python tools](https://pypi.org/project/vlsirtools/) Hdl21 also includes drivers for popular industry-standard data formats and popular spice-class simulation engines.
+
+The `hdl21.to_proto()` function converts an Hdl21 `Module` or group of `Modules` into a VLSIR `Package`. The `hdl21.from_proto()` function similarly imports a VLSIR `Package` into a Python namespace of Hdl21 `Modules`.
 
 Exporting to industry-standard netlist formats is a particularly common operation for Hdl21 users. The `hdl21.netlist()` function uses VLSIR to export any of its supported netlist formats.
 
 ```python
 import sys
 import hdl21 as h
 
@@ -362,28 +545,45 @@
     cap = h.Cap(c=1e3)(p=p, n=n)
     ind = h.Ind(l=1e-9)(p=p, n=n)
 
 # Write a spice-format netlist to stdout
 h.netlist(Rlc, sys.stdout, fmt="spice")
 ```
 
-`hdl21.netlist` takes a second destination argument `dest`, which is commonly either an open file-handle or `sys.stdout`. All its remaining arguments are passed to `vlsirtools.netlist`.
+`hdl21.netlist` takes a second destination argument `dest`, which is commonly either an open file-handle or `sys.stdout`.
+
+Each `Module` includes a list of `Literal` contents, designed to be included directly in exported netlists. These are commonly used to refer to out-of-Hdl21 quantities, or to include netlist-language features not first-class supported by Hdl21. Example:
+
+```python
+@h.module
+class HasLiterals:
+    a, b, c = h.Ports(3)
+
+# Add some literal content
+HasLiterals.literals.extend([
+    h.Literal("generate some_verilog_code"),
+    h.Literal(".some_spice_attribute what=ever"),
+    h.Literal("PRAGMA: some_pragma"),
+])
+```
+
+`Module.literals` is a Python built-in list and can be manipulated with any of its typical methods (`append`, `extend`, etc.). Literals are written to netlists in the order they appear in the list. Order between Literals and other Module content is not preserved.
 
 ## Spice-Class Simulation
 
 Hdl21 includes drivers for popular spice-class simulation engines commonly used to evaluate analog circuits.
 The `hdl21.sim` package includes a wide variety of spice-class simulation constructs, including:
 
 - DC, AC, Transient, Operating-Point, Noise, Monte-Carlo, Parameter-Sweep and Custom (per netlist language) Analyses
 - Control elements for saving signals (`Save`), simulation options (`Options`), including external files and contents (`Include`, `Lib`), measurements (`Meas`), simulation parameters (`Param`), and literal netlist commands (`Literal`)
 
 The entrypoint to Hdl21-driven simulation is the simulation-input type `hdl21.sim.Sim`. Each `Sim` includes:
 
 - A testbench Module `tb`, and
-- A list of unordered simulation attributes (`attrs`), including any and all of the analyses, controls, and related elements listed above.
+- A list of simulation attributes (`attrs`), including any and all of the analyses, controls, and related elements listed above.
 
 Example:
 
 ```python
 import hdl21 as h
 from hdl21.sim import *
 
@@ -418,23 +618,26 @@
     ],
 )
 
 # And run it!
 sim.run()
 ```
 
-`Sim` also includes a class-based syntax similar to `Module` and `Bundle`, in which simulation attributes are named based on their class attribute name:
+`Sim` also includes a class-based syntax similar to `Module` and `Bundle`. This also allows for inline definition of a testbench module, which can be named either `tb` or `Tb`:
 
 ```python
 import hdl21 as h
 from hdl21.sim import *
 
 @sim
 class MySim:
-    tb = MyModulesTestbench
+
+    @h.module
+    class Tb:
+        # ... Testbench content ...
 
     x = Param(5)
     y = Param(6)
     mydc = Dc(var=x, sweep=PointSweep([1]))
     myac = Ac(sweep=LogSweep(1e1, 1e10, 10))
     mytran = Tran(tstop=11 * h.prefix.PICO)
     mysweep = SweepAnalysis(
@@ -454,15 +657,15 @@
 MySim.run()
 ```
 
 Note that in these class-based definitions, attributes whose names don't really matter such as `save_all` above can be _named_ anything, but must be _assigned_ into the class, not just constructed.
 
 Class-based `Sim` definitions retain all class members which are `SimAttr`s and drop all others. Non-`SimAttr`-valued fields can nonetheless be handy for defining intermediate values upon which the ultimate SimAttrs depend, such as the `a_path` field in the example above.
 
-Classes decoratated by `sim` a single special required field: a `tb` attribute which sets the simulation testbench. A handful of names are disallowed in `sim` class-definitions, generally corresponding to the names of the `Sim` class's fields and methods such as `attrs` and `run`.
+Classes decorated by `@sim` have a single special required field: a testbench attribute, named either `tb` or `Tb`, which sets the simulation testbench. A handful of names are disallowed in `sim` class-definitions, generally corresponding to the names of the `Sim` class's fields and methods such as `attrs` and `run`.
 
 Each `sim` also includes a set of methods to add simulation attributes from their keyword constructor arguments. These methods use the same names as the simulation attributes (`Dc`, `Meas`, etc.) but incorporating the python language convention that functions and methods be lowercase (`dc`, `meas`, etc.). Example:
 
 ```python
 # Create a `Sim`
 s = Sim(tb=MyTb)
 
@@ -487,137 +690,52 @@
 s.lib(path="/home/models", section="fast")
 s.options(reltol=1e-9)
 
 # And run it!
 s.run()
 ```
 
-## Primitives and External Modules
-
-The leaf-nodes of each hierarchical Hdl21 circuit are generally defined in one of two places:
-
-- `Primitive` elements, defined in the `hdl21.primitives` package. These include transistors, resistors, capacitors, and other irreducible components. Simulation-level behavior of these elements is typically defined _inside of_ simulation tools and other EDA software.
-- `ExternalModules`, defined outside Hdl21. Such "module wrappers", which might alternately be called "black boxes", are common for including circuits from other HDLs.
-
-### `Primitives`
-
-Hdl21 `Primitives` come in _ideal_ and _physical_ flavors. The difference is most frequently relevant for passive elements, which can for example represent either (a) technology-specific passives, e.g. a MIM or MOS capacitor, or (b) an _ideal_ capacitor. Some element-types have solely physical implementations, some are solely ideal, and others include both.
-
-### The `hdl21.primitives` Library
-
-The `Primitive` type and all its valid values are defined by the `hdl21.primitives` package. A summary of the `hdl21.primitives` library content:
-
-| Name                           | Description                       | Type     | Aliases                               | Ports        |
-| ------------------------------ | --------------------------------- | -------- | ------------------------------------- | ------------ |
-| Mos                            | Mos Transistor                    | PHYSICAL | MOS                                   | d, g, s, b   |
-| IdealResistor                  | Ideal Resistor                    | IDEAL    | R, Res, Resistor, IdealR, IdealRes    | p, n         |
-| PhysicalResistor               | Physical Resistor                 | PHYSICAL | PhyR, PhyRes, ResPhy, PhyResistor     | p, n         |
-| ThreeTerminalResistor          | Three Terminal Resistor           | PHYSICAL | Res3, PhyRes3, ResPhy3, PhyResistor3  | p, n, b      |
-| IdealCapacitor                 | Ideal Capacitor                   | IDEAL    | C, Cap, Capacitor, IdealC, IdealCap   | p, n         |
-| PhysicalCapacitor              | Physical Capacitor                | PHYSICAL | PhyC, PhyCap, CapPhy, PhyCapacitor    | p, n         |
-| ThreeTerminalCapacitor         | Three Terminal Capacitor          | PHYSICAL | Cap3, PhyCap3, CapPhy3, PhyCapacitor3 | p, n, b      |
-| IdealInductor                  | Ideal Inductor                    | IDEAL    | L, Ind, Inductor, IdealL, IdealInd    | p, n         |
-| PhysicalInductor               | Physical Inductor                 | PHYSICAL | PhyL, PhyInd, IndPhy, PhyInductor     | p, n         |
-| ThreeTerminalInductor          | Three Terminal Inductor           | PHYSICAL | Ind3, PhyInd3, IndPhy3, PhyInductor3  | p, n, b      |
-| PhysicalShort                  | Short-Circuit/ Net-Tie            | PHYSICAL | Short                                 | p, n         |
-| DcVoltageSource                | DC Voltage Source                 | IDEAL    | V, Vdc, Vsrc                          | p, n         |
-| PulseVoltageSource             | Pulse Voltage Source              | IDEAL    | Vpu, Vpulse                           | p, n         |
-| CurrentSource                  | Ideal DC Current Source           | IDEAL    | I, Idc, Isrc                          | p, n         |
-| VoltageControlledVoltageSource | Voltage Controlled Voltage Source | IDEAL    | Vcvs, VCVS                            | p, n, cp, cn |
-| CurrentControlledVoltageSource | Current Controlled Voltage Source | IDEAL    | Ccvs, CCVS                            | p, n, cp, cn |
-| VoltageControlledCurrentSource | Voltage Controlled Current Source | IDEAL    | Vccs, VCCS                            | p, n, cp, cn |
-| CurrentControlledCurrentSource | Current Controlled Current Source | IDEAL    | Cccs, CCCS                            | p, n, cp, cn |
-| Bipolar                        | Bipolar Transistor                | PHYSICAL | Bjt, BJT                              | c, b, e      |
-| Diode                          | Diode                             | PHYSICAL | D                                     | p, n         |
-
-Each primitive is available in the `hdl21.primitives` namespace, either through its full name or any of its aliases. Most primitives have fairly verbose names (e.g. `VoltageControlledCurrentSource`, `IdealResistor`), but also expose short-form aliases (e.g. `Vcvs`, `R`). Each of the aliases in Table 1 above refer to _the same_ Python object, i.e.
-
-```python
-from hdl21.primitives import R, Res, IdealResistor
-
-R is Res            # evaluates to True
-R is IdealResistor  # also evaluates to True
-```
-
-### `ExternalModules`
-
-Alternately Hdl21 includes an `ExternalModule` type which defines the interface to a module-implementation outside Hdl21. These external definitions are common for instantiating technology-specific modules and libraries. Other popular modern HDLs refer to these as module _black boxes_. An example `ExternalModule`:
-
-```python
-import hdl21 as h
-from hdl21.prefix import µ
-from hdl21.primitives import Diode
-
-@h.paramclass
-class BandGapParams:
-    self_destruct = h.Param(
-        dtype=bool,
-        desc="Whether to include the self-destruction feature",
-        default=True,
-    )
-
-BandGap = h.ExternalModule(
-    name="BandGap",
-    desc="Example ExternalModule, defined outside Hdl21",
-    port_list=[h.Port(name="vref"), h.Port(name="enable")],
-    paramtype=BandGapParams,
-)
-```
-
-Both `Primitives` and `ExternalModules` have names, ordered `Ports`, and a few other pieces of metadata, but no internal implementation: no internal signals, and no instances of other modules. Unlike `Modules`, both _do_ have parameters. `Primitives` each have an associated `paramclass`, while `ExternalModules` can optionally declare one via their `paramtype` attribute. Their parameter-types are limited to a small subset of those possible for `Generators` - scalar numeric types (`int`, `float`) and `str` - primarily limited by the need to need to provide them to legacy HDLs.
-
-`Primitives` and `ExternalModules` can be instantiated and connected in all the same styles as `Modules`:
-
-```python
-# Continuing from the snippet above:
-params = BandGapParams(self_destruct=False)  # Watch out there!
-
-@h.module
-class BandGapPlus:
-    vref, enable = h.Signals(2)
-    # Instantiate the `ExternalModule` defined above
-    bg = BandGap(params)(vref=vref, enable=enable)
-    # ...Anything else...
-
-@h.module
-class DiodePlus:
-    p, n = h.Signals(2)
-    # Parameterize, instantiate, and connect a `primitives.Diode`
-    d = Diode(w=1 * µ, l=1 * µ)(p=p, n=n)
-    # ... Everything else ...
-```
-
 ## Process Technologies
 
 Designing for a specific implementation technology (or "process development kit", or PDK) with Hdl21 can use either of (or a combination of) two routes:
 
 - Instantiate `ExternalModules` corresponding to the target technology. These would commonly include its process-specific transistor and passive modules, and potentially larger cells, for example from a cell library. Such external modules are frequently defined as part of a PDK (python) package, but can also be defined anywhere else, including inline among Hdl21 generator code.
-- Use `hdl21.Primitives`, each of which is designed to be a technology-independent representation of a primitive component. Moving to a particular technology then generally requires passing the design through an `hdl21.pdk` converter.
+- Use `hdl21.Primitives`, each of which is designed to be a technology-independent representation of a primitive component. Moving to a particular technology then generally requires passing the design through an `hdl21.pdk`'s `compile` function.
 
 Hdl21 PDKs are Python packages which generally include two primary elements:
 
 - (a) A library `ExternalModules` describing the technology's cells, and
 - (b) A `compile` conversion-method which transforms a hierarchical Hdl21 tree, mapping generic `hdl21.Primitives` into the tech-specific `ExternalModules`.
 
-Since PDKs are python packages, using them is as simple as importing them. Hdl21 includes two built-in PDKs: the academic predicitive [ASAP7](https://pypi.org/project/asap7-hdl21/) technology, and the open-source [SkyWater 130nm](https://pypi.org/project/sky130-hdl21/) technology.
+Since PDKs are python packages, using them is as simple as importing them. Hdl21 includes a built-in sample PDK available via `hdl21.pdk.sample_pdk` which includes simulatable NMOS and PMOS transistors. Hdl21's source tree includes three additional PDK packages:
+
+|                                       | PyPi                                   | Source        |
+| ------------------------------------- | -------------------------------------- | ------------- |
+| ASAP7 Predictive/ Academic PDK        | https://pypi.org/project/asap7-hdl21/  | [pdks/Asap7](./pdks/Asap7)  |
+| SkyWater 130nm Open-Source PDK        | https://pypi.org/project/sky130-hdl21/ | [pdks/Sky130](./pdks/Sky130) |
+| GlobalFoundries 180nm Open-Source PDK | https://pypi.org/project/gf180-hdl21   | [pdks/Gf180](./pdks/Gf180)  |
+
+Each contain much more detail documentation on their specific installation and use.
 
 ```python
 import hdl21 as h
-import sky130
+import sky130_hdl21
 
 @h.module
 class SkyInv:
     """ An inverter, demonstrating using PDK modules """
 
     # Create some IO
     i, o, VDD, VSS = h.Ports(4)
 
+    p = sky130_hdl21.Sky130MosParams(w=1,l=1)
+
     # And create some transistors!
-    ps = sky130.modules.sky130_fd_pr__pfet_01v8(w=1, l=1)(d=o, g=i, s=VDD, b=VDD)
-    ns = sky130.modules.sky130_fd_pr__nfet_01v8(w=1, l=1)(d=o, g=i, s=VSS, b=VSS)
+    ps = sky130_hdl21.primtives.PMOS_1p8V_STD(p)(d=o, g=i, s=VDD, b=VDD)
+    ns = sky130_hdl21.primtives.NMOS_1p8V_STD(p)(d=o, g=i, s=VSS, b=VSS)
 ```
 
 Process-portable modules instead use Hdl21 `Primitives`, which can be compiled to a target technology:
 
 ```python
 import hdl21 as h
 from hdl21.prefix import µ
@@ -635,17 +753,17 @@
     ns = Nmos(w=1*µ, l=1*µ, vth=MosVth.STD)(d=o, g=i, s=VSS, b=VSS)
 ```
 
 Compiling the generic devices to a target PDK then just requires a pass through the PDK's `compile()` method:
 
 ```python
 import hdl21 as h
-import sky130
+import sky130_hdl21
 
-sky130.compile(Inv) # Produces the same content as `SkyInv` above
+sky130_hdl21.compile(Inv) # Produces the same content as `SkyInv` above
 ```
 
 Hdl21 includes an `hdl21.pdk` subpackage which tracks the available in-memory PDKs. If there is a single PDK available, it need not be explicitly imported: `hdl21.pdk.compile()` will use it by default.
 
 ```python
 import hdl21 as h
 import sky130  # Note this import can be elsewhere in the program, i.e. in a configuration layer.
@@ -682,15 +800,15 @@
 CmosCorner = TT | FF | SS | SF | FS
 ```
 
 Hdl21 exposes each of these corner-types as Python enumerations and combinations thereof. Each PDK package then defines its mapping from these `Corner` types to the content they include, typically in the form of external files.
 
 ### PDK Installations and Sites
 
-Much of the content of a typical process technology - even the subset that Hdl21 cares about - is not defined in Python. Transistor models and SPICE "library" files, such as those defining the `_nfet` and `_pfet` above, are common examples pertinent to Hdl21. Tech-files, layout libraries, and the like are similarly necessary for related pieces of EDA software. These PDK contents are commonly stored in a technology-specific arrangement of interdependent files. Hdl21 PDK packages structure this external content as a `PdkInstallation` type.
+Much of the content of a typical process technology - even the subset that Hdl21 cares about - is not defined in Python. Transistor models and SPICE "library" files, such as those defining the `PMOS` and `NMOS` above, are common examples pertinent to Hdl21. Tech-files, layout libraries, and the like are similarly necessary for related pieces of EDA software. These PDK contents are commonly stored in a technology-specific arrangement of interdependent files. Hdl21 PDK packages structure this external content as a `PdkInstallation` type.
 
 Each `PdkInstallation` is a runtime type-checked Python `dataclass` which extends the base `hdl21.pdk.PdkInstallation` type. Installations are free to define arbitrary fields and methods, which will be type-validated for each `Install` instance. Example:
 
 ```python
 """ A sample PDK package with an `Install` type """
 
 from pydantic.dataclasses import dataclass
@@ -738,19 +856,19 @@
 
 These "site packages" are named `sitepdks` by convention. They can often be shared among several PDKs on a given filesystem. Hdl21 includes one built-in example such site-package, [SampleSitePdks](./SampleSitePdks/), which demonstrates setting up both built-in PDKs, Sky130 and ASAP7:
 
 ```python
 # The built-in sample `sitepdks` package
 from pathlib import Path
 
-import sky130
-sky130.install = sky130.Install(model_lib=Path("pdks") / "sky130" / ... / "sky130.lib.spice")
+import sky130_hdl21
+sky130_hdl21.install = sky130_hdl21.Install(model_lib=Path("pdks") / "sky130" / ... / "sky130.lib.spice")
 
-import asap7
-asap7.install = asap7.Install(model_lib=Path("pdks") / "asap7" / ... / "TT.pm")
+import asap7_hdl21
+asap7_hdl21.install = asap7_hdl21.Install(model_lib=Path("pdks") / "asap7" / ... / "TT.pm")
 ```
 
 "Site-portable" code requiring external PDK content can then refer to the PDK package's `install`, without being directly aware of its contents.
 An example simulation using `mypdk`'s models with the `sitepdk`s defined above:
 
 ```python
 # sim_my_pdk.py
@@ -770,25 +888,218 @@
 
 # And run it!
 SimMyPdk.run()
 ```
 
 Note that `sim_my_pdk.py` need not necessarily import or directly depend upon `sitepdks` itself. So long as `sitepdks` is imported and configures the PDK installation anywhere in the Python program, further code will be able to refer to the PDK's `install` fields.
 
-## Examples Library
+### Creating PDK Packages
+
+Hdl21's source tree includes a [cookiecutter template](https://github.com/cookiecutter/cookiecutter) for creating a new PDK package, available at [pdks/PdkTemplate](./pdks/PdkTemplate).
+
+## Bundles
+
+Hdl21 `Bundle`s are _structured connection types_ which can include `Signal`s and instances of other `Bundle`s.
+Think of them as "connection structs". Similar ideas are implemented by Chisel's `Bundle`s and SystemVerilog's `interface`s.
+
+```python
+@h.bundle
+class Diff:
+    p = h.Signal()
+    n = h.Signal()
+
+@h.bundle
+class Quadrature:
+    i = Diff()
+    q = Diff()
+```
+
+Like `Module`s, `Bundle`s can be defined either procedurally or as a class decorated by the `hdl21.bundle` function.
+
+```python
+# This creates the same stuff as the class-based definitions above:
+
+Diff = h.Bundle(name="Diff")
+Diff.add(h.Signal(name="p"))
+Diff.add(h.Signal(name="n"))
+
+Quadrature = h.Bundle(name="Quadrature")
+Quadrature.add(Diff(name="i"))
+Quadrature.add(Diff(name="q"))
+```
+
+Calling a `Bundle` as in the calls to `Diff()` and `Diff(name=q)` creates an instance of that `Bundle`.
+
+## Bundle Ports
+
+Bundles are commonly most valuable for shipping collections of related `Signal`s between `Module`s.
+Modules can accordingly have Bundle-valued ports. To create a Bundle-port, set the `port` argument to either the boolean `True`
+or the `hdl21.Visibility.PORT` value.
+
+```python
+@h.module
+class HasDiffs:
+    d1 = Diff(port=True)
+    d2 = Diff(port=h.Visbility.PORT)
+```
+
+Port directions on bundle-ports can be set by either of two methods.
+The first is to set the directions directly on the Bundle's constituent `Signal`s.
+To swap directions, pass the bundle-instances through the `hdl21.flipped` function,
+or set the `flipped` argument to the instance-constructor.
+
+```python
+@h.bundle
+class Inner:
+    i = h.Input()
+    o = h.Output()
+
+@h.bundle
+class Outer:
+    b1 = Inner()
+    b2 = h.flipped(Inner())
+    b3 = Inner(flipped=True)
+```
+
+Here:
+
+- An `Inner` bundle defines an `Input` and an `Output`
+- An `Outer` bundle instantiates three of them
+  - Instance `b1` is not flipped; its `i` is an input, and its `o` is an output
+  - Instance `b2` is flipped; its `i` is an _output_, and its `o` is an _input_
+  - Instance `b3` is also flipped, via its constructor argument
+
+These "flipping based" bundles require that all constituent signals, including nested ones, have port-visibility.
+The rules for flipping port directions are:
+
+- Inputs become Outputs
+- Outputs become Inputs
+- Inouts and undirected ports (`direction=NONE`) retain their directions
+
+```python
+@h.bundle
+class B:
+    clk = h.Output()
+    data = h.Input()
+
+@h.module
+class X: # Module with a `clk` output and `data` input
+    b = B(port=True)
+
+@h.module
+class Y: # Module with a `clk` input and `data` output
+    b = B(flipped=True, port=True)
+
+@h.module
+class Z:
+    b = B() # Internal instance of the `B` bundle
+    x = X(b=b)
+    y = Y(b=b)
+```
+
+The second method for setting bundle-port directions is with `Role`s.
+Each Hdl21 bundle either explicitly or implictly defines a set of `Role`s, which might alternately be called "endpoints".
+These are the expected "end users" of the Bundle.
+Signal directions are then defined on each signal's `src` (source) and `dest` (destination) arguments, which can be set to any of the bundle's roles.
+
+```python
+@h.roles
+class HostDevice(Enum):
+    HOST = auto()
+    DEVICE = auto()
+
+@h.bundle
+class Jtag:
+    roles = HostDevice # Set the bundle's roles
+    # Note each signal sets one of the roles as `src` and another as `dest`
+    tck, tdi, tms = h.Signals(3, src=roles.HOST, dest=roles.DEVICE)
+    tdo = h.Signal(src=roles.DEVICE, dest=roles.HOST)
+```
+
+Bundle-valued ports are then assigned a role and associated signal-port directions via their `role` constructor argument.
+
+```python
+@h.module
+class Widget: # with a Jtag Device port
+    jtag = Jtag(port=True, role=Jtag.roles.DEVICE)
+
+@h.module
+class Debugger: # with a Jtag Host port
+    jtag = Jtag(port=True, role=Jtag.roles.HOST)
+
+@h.module
+class System: # combining the two
+    widget = Widget()
+    debugger = Debugger(jtag=widget.jtag)
+```
+
+The rules for port-directions of role-based bundles are:
+
+- If the bundle's role is the signal's source, the signal is an `Output`
+- If the bundle's role is the signal's destination, the signal is an `Input`
+- Otherwise the signal is assigned no direction, i.e. `direction=NONE`
+
+## Collecting Bundles
+
+It is often helpful or necessary to collect existing signals into a bundle, or to "re-arrange" signals from one bundle into another.
+The primary mechanism for doing so is the `hdl21.bundlize` function which creates them.
+Each call to `bundlize` creates an "anonymous" bundle which lacks a backing bundle-definition type.
+
+```python
+@h.bundle
+class Uart:
+    tx = h.Output()
+    rx = h.Input()
+
+@h.module
+class HasUart:
+    # Module with a `Uart` port
+    uart = Uart(port=True)
+
+@h.module
+class ConnectTwo:
+    # Connect two `HasUart`s, swapping `tx` and `rx`.
+    uart = Uart()
+    m1 = HasUart(uart=uart)
+    m2 = HasUart(uart=h.bundlize(tx=uart.rx, rx=uart.tx))
+```
+
+## Examples
+
+### Built-In Examples Library
 
 Hdl21's source tree includes a built-in [examples](./examples/) library. Each is designed to be a straightforward but realistic use-case, and is a self-contained Python program which can be run directly, e.g. with:
 
 ```bash
 python examples/rdac.py
 ```
 
+The built-in examples include:
+
+- [Current DAC](./examples/idac.py)
+- [MOS Transistor Simulation](./examples/mos_sim.py)
+- [Ring Oscillator Generator](./examples/ro.py)
+- [Resistor-Ladder DAC](./examples/rdac.py)
+- [Recursive Binary to One-Hot Encoders](./examples/encoder.py)
+
 Reading, copying, or cloning these example programs is generally among the best ways to get started.  
 And adding an example is a **highly** encouraged form of [pull request](https://github.com/dan-fritchman/Hdl21/pulls)!
 
+### Featured Community Examples
+
+- [Continuous-Time Delta-Sigma ADC Generators](https://github.com/aviralpandey/CT-DS-ADC_generator)
+- [USB 2.0 PHY](https://github.com/Vlsir/Usb2Phy/tree/main/Usb2PhyAna)
+- [VCO-Based ADC Generators](https://github.com/aviralpandey) (Coming soon!)
+
+## Related Projects
+
+- [VLSIR](https://github.com/vlsir/vlsir)
+- [Hdl21 Schematics](https://github.com/vlsir/hdl21schematics)
+- [Layout21](https://github.com/dan-fritchman/Layout21)
+
 ## Why Use Python?
 
 Custom IC design is a complicated field. Its practitioners have to know
 [a](https://people.eecs.berkeley.edu/~boser/courses/240B/lectures/M07%20OTA%20II.pdf) |
 [lot](http://rfic.eecs.berkeley.edu/~niknejad/ee142_fa05lects/pdf/lect24.pdf) |
 [of](https://www.delroy.com/PLL_dir/ISSCC2004/PLLTutorialISSCC2004.pdf) |
 [stuff](https://inst.eecs.berkeley.edu/~ee247/fa10/files07/lectures/L25_2_f10.pdf),
```

### Comparing `hdl21-3.0.dev3/hdl21.egg-info/SOURCES.txt` & `hdl21-4.0.0rc0/hdl21.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,19 @@
 setup.py
 .github/workflows/test.yaml
 .vscode/settings.json
 SampleSitePdks/readme.md
 SampleSitePdks/setup.py
 SampleSitePdks/sitepdks.py
 examples/__init__.py
+examples/bundles.py
+examples/diff_ota.py
 examples/encoder.py
-examples/mos_iv_sim.py
+examples/idac.py
+examples/mos_sim.py
 examples/rdac.py
 examples/ro.py
 examples/test_examples.py
 hdl21/__init__.py
 hdl21/attrmagic.py
 hdl21/bundle.py
 hdl21/call.py
@@ -35,20 +38,23 @@
 hdl21/netlist.py
 hdl21/noconn.py
 hdl21/one_or_more.py
 hdl21/params.py
 hdl21/portref.py
 hdl21/prefix.py
 hdl21/primitives.py
+hdl21/props.py
 hdl21/qualname.py
+hdl21/role.py
 hdl21/scalar.py
 hdl21/signal.py
 hdl21/slice.py
 hdl21/sliceable.py
 hdl21/source_info.py
+hdl21/visibility.py
 hdl21/walker.py
 hdl21.egg-info/PKG-INFO
 hdl21.egg-info/SOURCES.txt
 hdl21.egg-info/dependency_links.txt
 hdl21.egg-info/requires.txt
 hdl21.egg-info/top_level.txt
 hdl21/elab/__init__.py
@@ -73,14 +79,15 @@
 hdl21/pdk/corner.py
 hdl21/pdk/installation.py
 hdl21/pdk/pdk.py
 hdl21/pdk/test_pdk.py
 hdl21/pdk/sample_pdk/__init__.py
 hdl21/pdk/sample_pdk/pdk.py
 hdl21/pdk/sample_pdk/test_sample_pdk.py
+hdl21/pdk/sample_pdk/resources/models.sp
 hdl21/proto/__init__.py
 hdl21/proto/from_proto.py
 hdl21/proto/to_proto.py
 hdl21/sim/__init__.py
 hdl21/sim/data.py
 hdl21/sim/delay.py
 hdl21/sim/to_proto.py
@@ -95,16 +102,14 @@
 hdl21/tests/test_hdl21.py
 hdl21/tests/test_params.py
 hdl21/tests/test_prefix.py
 hdl21/tests/test_source_info.py
 pdks/readme.md
 pdks/Asap7/readme.md
 pdks/Asap7/setup.py
-pdks/Asap7/asap7/__init__.py
 pdks/Sky130/readme.md
 pdks/Sky130/setup.py
-pdks/Sky130/sky130/__init__.py
 scratch/empty
 scripts/empty
 scripts/install-dev.sh
 scripts/install-pypi.sh
 scripts/primtable.py
```

### Comparing `hdl21-3.0.dev3/pdks/Asap7/setup.py` & `hdl21-4.0.0rc0/pdks/Asap7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "readme.md").read_text(encoding="utf-8")
 
-_VLSIR_VERSION = "3.0.dev3"
+_VLSIR_VERSION = "4.0.rc0"
 
 setup(
     name="asap7-hdl21",
     version=_VLSIR_VERSION,
     description="ASAP7 PDK Package for Hdl21",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dan-fritchman/Hdl21",
     author="Dan Fritchman",
     packages=find_packages(),
-    python_requires=">=3.8, <4",
+    python_requires=">=3.7",
     install_requires=[f"hdl21=={_VLSIR_VERSION}"],
     extras_require={"dev": ["pytest==7.1", "coverage", "pytest-cov", "twine"]},
 )
```

### Comparing `hdl21-3.0.dev3/pdks/Sky130/setup.py` & `hdl21-4.0.0rc0/pdks/Sky130/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "readme.md").read_text(encoding="utf-8")
 
-_VLSIR_VERSION = "3.0.dev3"
+_VLSIR_VERSION = "4.0.0rc0"
 
 setup(
     name="sky130-hdl21",
     version=_VLSIR_VERSION,
     description="SkyWater 130nm PDK Package for Hdl21",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dan-fritchman/Hdl21",
-    author="Dan Fritchman",
+    author="Dan Fritchman, Thomas Pluck",
     packages=find_packages(),
-    python_requires=">=3.8, <4",
+    python_requires=">=3.7",
     install_requires=[f"hdl21=={_VLSIR_VERSION}"],
     extras_require={"dev": ["pytest==7.1", "coverage", "pytest-cov", "twine"]},
 )
```

### Comparing `hdl21-3.0.dev3/pdks/readme.md` & `hdl21-4.0.0rc0/pdks/readme.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 # Hdl21 PDKs
 
 Built-in `hdl21.pdk` plug-ins.
 
 - [Sky130](./Sky130) serves the [SkyWater 130nm](https://github.com/google/skywater-pdk) technology
+- [Gf180](./Gf180/) serves the [Global Foundries 180nm MCU](https://github.com/gf180mcu-pdk) technology
 - [Asap7](./Asap7) serves the [ASAP7](https://github.com/The-OpenROAD-Project/asap7/) predictive/ academic technology
 
 While source-controlled in the Hdl21 codebase, each are stand-alone packages distributed through PyPi. 
 
-An additional fully-fictitious `sample_pdk`, available in the `hdl21` namespace at `hdl21.pdk.sample_pdk`, 
-makes an even lighter-weight demonstration of a PDK plug-in. 
+An additional fully-fictitious `sample_pdk`, available in the `hdl21` namespace at `hdl21.pdk.sample_pdk`, makes an even lighter-weight demonstration of a PDK plug-in.
```

### Comparing `hdl21-3.0.dev3/readme.md` & `hdl21-4.0.0rc0/readme.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 # HDL21
 
 ## Analog Hardware Description Library in Python
 
+[![pypi](https://img.shields.io/badge/pypi-hdl21-blue)](https://pypi.org/project/hdl21/)
+[![python-versions](https://img.shields.io/badge/python-3.7_3.8_3.9_3.10_3.11-blue)](https://codecov.io/gh/dan-fritchman/Hdl21)
 [![test](https://github.com/dan-fritchman/Hdl21/actions/workflows/test.yaml/badge.svg)](https://github.com/dan-fritchman/Hdl21/actions/workflows/test.yaml)
 [![codecov](https://codecov.io/gh/dan-fritchman/Hdl21/branch/main/graph/badge.svg?token=f8LKUqEPdq)](https://codecov.io/gh/dan-fritchman/Hdl21)
 
-Hdl21 is a [hardware description library](https://en.wikipedia.org/wiki/Hardware_description_language) embedded in Python. It is targeted and optimized for analog and custom integrated circuits, and for maximum productivity with minimum fancy-programming skill.
-
-Hdl21 generates hardware databases in the [VLSIR](https://github.com/Vlsir/Vlsir) interchange formats, defined through [Google Protocol Buffers](https://developers.google.com/protocol-buffers/). Through [VLSIR's Python tools](https://pypi.org/project/vlsirtools/) Hdl21 also includes drivers for popular industry-standard data formats and popular spice-class simulation engines.
+Hdl21 is a [hardware description library](https://en.wikipedia.org/wiki/Hardware_description_language) embedded in Python.  
+It is targeted for analog and custom integrated circuits, and for maximum productivity with minimum fancy-programming skill.
 
 ## Contents
 
+- [Installation](#installation)
 - [Modules](#modules)
 - [Signals](#signals), [Ports](#signals), and [Connections](#connections)
 - [Generators](#generators) and [Parameters](#parameters)
+- [Primitive Elements and External Modules](#primitives-and-external-modules)
 - [Spice-Class Simulation](#spice-class-simulation)
-- [Primitive Elements](#primitives-and-external-modules)
-- [Process Technology (PDK) Packages](#process-technologies)
-- Coming Soon: Structured Connections with `Bundle`s
-- Coming Soon: [Schematics](https://github.com/Vlsir/Hdl21Schematics)
-- [Examples Library](#examples-library)
+- [Process Technologies (PDKs)](#process-technologies)
+- [Bundles](#bundles)
+- [Examples](#examples)
+- [Related Projects](#related-projects)
+
+## Installation
+
+```
+pip install hdl21
+```
+
+That's it. No crazy build step, no crazy dependencies, no crazy EDA stuff, no "clone and _just_ modify these 300 things", no `source`ing, none of that. Hdl21 is pure Python, and is designed to be as easy to install as any other Python package.
 
 ## Modules
 
 Hdl21's primary unit of hardware reuse is the `Module`. Think of it as Verilog's `module`, or VHDL's `entity`, or SPICE's `subckt`. Better yet if you are used to graphical schematics, think of it as the content of a schematic. Hdl21 `Modules` are containers of a handful of `hdl21` types. Think of them as including:
 
 - Instances of other `Modules`
 - Connections between them, defined by `Signals` and `Ports`
@@ -264,21 +274,46 @@
 o = Outer(**d1)
 # Convert back to another dictionary
 d2 = asdict(o)
 # And check they line up
 assert d1 == d2
 ```
 
+Generators include the capability to construct their param-classes inline, if provided a set of compatible keyword arguments. For example, defining a generator using the `MyParams` parameters above:
+
+```python
+@h.generator
+def MyGen(params: MyParams) -> h.Module:
+    ... # Create a `Module` & return it
+```
+
+This typical invocation:
+
+```python
+p = MyParams(width=8, text="My Favorite Module")
+MyGen(p)
+```
+
+is the same as calling:
+
+```python
+MyParams(width=8, text="My Favorite Module")
+```
+
+Parameters may be provided as keywords, or as a single positional argument which is an instance of the generator's param-class. Combinations of the two are not supported.
+
 ## A Note on Parametrization
 
 Hdl21 `Generators` have parameters. `Modules` do not.
 
 This is a deliberate decision, which in this sense makes `hdl21.Module` less feature-rich than the analogous `module` concepts in existing HDLs (Verilog, VHDL, and even SPICE). These languages support what might be called "static parameters" - relatively simple relationships between parent and child-module parameterization. Setting, for example, the width of a signal or number of instances in an array is straightforward. But more elaborate parametrization-cases are either highly cumbersome or altogether impossible to create. (As an example, try using Verilog parametrization to make a programmable-depth binary tree.) Hdl21, in contrast, exposes all parametrization to the full Python-power of its generators.
 
-## `Prefixed` Numeric Parameters
+## Numeric Parameters
+
+### `Prefixed` Numbers
 
 Hdl21 provides an [SI prefixed](https://www.nist.gov/pml/owm/metric-si-prefixes) numeric type `Prefixed`, which is especially common for physical generator parameters. Each `Prefixed` value is a combination of the Python standard library's `Decimal` and an enumerated SI `Prefix`:
 
 ```python
 @dataclass
 class Prefixed:
     number: Decimal  # Numeric Portion
@@ -289,15 +324,15 @@
 
 `Prefixed` values rarely need to be instantiated directly. Instead Hdl21 exposes a set of common prefixes via their typical single-character names:
 
 ```python
 f = FEMTO = Prefix.FEMTO
 p = PICO = Prefix.PICO
 n = NANO = Prefix.NANO
-µ = MICRO = Prefix.MICRO
+µ = u = MICRO = Prefix.MICRO # Note both `u` and `µ` are valid
 m = MILLI = Prefix.MILLI
 K = KILO = Prefix.KILO
 M = MEGA = Prefix.MEGA
 G = GIGA = Prefix.GIGA
 T = TERA = Prefix.TERA
 P = PETA = Prefix.PETA
 UNIT = Prefix.UNIT
@@ -328,17 +363,165 @@
 
 11 * e(-6) == 11 * µ  # True
 ```
 
 These `e()` values are also most common in multiplication expressions,
 to create `Prefixed` values in "floating point" style such as `11 * e(-9)`.
 
+### `Scalar`
+
+Many Hdl21 primitive parameters can be either numbers or string-literals.  
+The combination is so common that Hdl21 defines a `Scalar` type which is (roughly):
+
+```python
+Scalar = Union[Prefixed, Literal]
+```
+
+With automatic conversions from each of `str`, `int`, `float`, and `Decimal`.
+
+`Scalar` is particularly designed for parameter-values of `Primitive`s and of simulations.
+Most such parameters "want" to be the `Prefixed` type, for reasons outlined [above](#prefixed-numeric-parameters). They often also need a string-valued escape hatch, e.g. when referring to out-of-Hdl21 quantities
+such as parameters in external netlists or simulation decks.
+These out-of-Hdl21 expressions are represented by the `Literal` type, a simple wrapper around `str`.
+
+Where possible `Scalar` prefers to use the `Prefixed` variant.
+Built-in numbers `(int, float, Decimal)` are converted to `Prefixed` inline.
+Strings are attempted to be converted to `Prefixed`, and fall back to `Literal` if unsuccessful.
+This conversion process is also available as the free-standing `to_scalar()` function.
+
+Example:
+
+```python
+import hdl21 as h
+from hdl21.prefix import NANO, µ
+from decimal import Decimal
+
+@h.paramclass
+class MyMosParams:
+    w = h.Param(dtype=h.Scalar, desc="Width", default=1e-6) # Default `float` converts to a `Prefixed`
+    l = h.Param(dtype=h.Scalar, desc="Length", default="w/5") # Default `str` converts to a `Literal`
+
+# Example instantiations
+MyMosParams() # Default values
+MyMosParams(w=Decimal(1e-6), l=3*µ)
+MyMosParams(w=h.Literal("sim_param_width"), l=h.Prefixed.new(20, NANO))
+MyMosParams(w="11*l", l=11)
+```
+
+When defining "primitive level" parameters - e.g. those that will be used in PDK-level devices - `Scalar` is generally the best datatype to use.
+
+## Primitives and External Modules
+
+The leaf-nodes of each hierarchical Hdl21 circuit are generally defined in one of two places:
+
+- `Primitive` elements, defined in the `hdl21.primitives` package. Each is designed to be a technology-independent representation of an irreducible component.
+- `ExternalModules`, defined outside Hdl21. Such "module wrappers", which might alternately be called "black boxes", are common for including circuits from other HDLs.
+
+### `Primitives`
+
+Hdl21's library of generic primitive elements is defined in the `hdl21.primitives` package. Its content is roughly equivalent to that built into a typical SPICE simulator.
+
+A summary of `hdl21.primitives`:
+
+| Name                           | Description                       | Type     | Aliases                               | Ports        |
+| ------------------------------ | --------------------------------- | -------- | ------------------------------------- | ------------ |
+| Mos                            | Mos Transistor                    | PHYSICAL | MOS                                   | d, g, s, b   |
+| IdealResistor                  | Ideal Resistor                    | IDEAL    | R, Res, Resistor, IdealR, IdealRes    | p, n         |
+| PhysicalResistor               | Physical Resistor                 | PHYSICAL | PhyR, PhyRes, ResPhy, PhyResistor     | p, n         |
+| ThreeTerminalResistor          | Three Terminal Resistor           | PHYSICAL | Res3, PhyRes3, ResPhy3, PhyResistor3  | p, n, b      |
+| IdealCapacitor                 | Ideal Capacitor                   | IDEAL    | C, Cap, Capacitor, IdealC, IdealCap   | p, n         |
+| PhysicalCapacitor              | Physical Capacitor                | PHYSICAL | PhyC, PhyCap, CapPhy, PhyCapacitor    | p, n         |
+| ThreeTerminalCapacitor         | Three Terminal Capacitor          | PHYSICAL | Cap3, PhyCap3, CapPhy3, PhyCapacitor3 | p, n, b      |
+| IdealInductor                  | Ideal Inductor                    | IDEAL    | L, Ind, Inductor, IdealL, IdealInd    | p, n         |
+| PhysicalInductor               | Physical Inductor                 | PHYSICAL | PhyL, PhyInd, IndPhy, PhyInductor     | p, n         |
+| ThreeTerminalInductor          | Three Terminal Inductor           | PHYSICAL | Ind3, PhyInd3, IndPhy3, PhyInductor3  | p, n, b      |
+| PhysicalShort                  | Short-Circuit/ Net-Tie            | PHYSICAL | Short                                 | p, n         |
+| DcVoltageSource                | DC Voltage Source                 | IDEAL    | V, Vdc, Vsrc                          | p, n         |
+| PulseVoltageSource             | Pulse Voltage Source              | IDEAL    | Vpu, Vpulse                           | p, n         |
+| CurrentSource                  | Ideal DC Current Source           | IDEAL    | I, Idc, Isrc                          | p, n         |
+| VoltageControlledVoltageSource | Voltage Controlled Voltage Source | IDEAL    | Vcvs, VCVS                            | p, n, cp, cn |
+| CurrentControlledVoltageSource | Current Controlled Voltage Source | IDEAL    | Ccvs, CCVS                            | p, n, cp, cn |
+| VoltageControlledCurrentSource | Voltage Controlled Current Source | IDEAL    | Vccs, VCCS                            | p, n, cp, cn |
+| CurrentControlledCurrentSource | Current Controlled Current Source | IDEAL    | Cccs, CCCS                            | p, n, cp, cn |
+| Bipolar                        | Bipolar Transistor                | PHYSICAL | Bjt, BJT                              | c, b, e      |
+| Diode                          | Diode                             | PHYSICAL | D                                     | p, n         |
+
+Each primitive is available in the `hdl21.primitives` namespace, either through its full name or any of its aliases. Most primitives have fairly verbose names (e.g. `VoltageControlledCurrentSource`, `IdealResistor`), but also expose short-form aliases (e.g. `Vcvs`, `R`). Each of the aliases in Table 1 above refer to _the same_ Python object, i.e.
+
+```python
+from hdl21.primitives import R, Res, IdealResistor
+
+R is Res            # evaluates to True
+R is IdealResistor  # also evaluates to True
+```
+
+Hdl21 `Primitives` come in _ideal_ and _physical_ flavors. The difference is most frequently relevant for passive elements, which can for example represent either
+
+- (a) technology-specific passives, e.g. a MIM or MOS capacitor, or
+- (b) an _ideal_ capacitor
+
+Some element-types have solely physical implementations, some are solely ideal, and others include both.
+
+### `ExternalModules`
+
+Alternately Hdl21 includes an `ExternalModule` type which defines the interface to a module-implementation outside Hdl21. These external definitions are common for instantiating technology-specific modules and libraries. Think of them as a module "function header"; other popular modern HDLs refer to them as module _black boxes_.
+
+An example `ExternalModule`:
+
+```python
+import hdl21 as h
+from hdl21.prefix import µ
+from hdl21.primitives import Diode
+
+@h.paramclass
+class BandGapParams:
+    self_destruct = h.Param(
+        dtype=bool,
+        desc="Whether to include the self-destruction feature",
+        default=True,
+    )
+
+BandGap = h.ExternalModule(
+    name="BandGap",
+    desc="Example ExternalModule, defined outside Hdl21",
+    port_list=[h.Port(name="vref"), h.Port(name="enable")],
+    paramtype=BandGapParams,
+)
+```
+
+Both `Primitives` and `ExternalModules` have names, ordered `Ports`, and a few other pieces of metadata, but no internal implementation: no internal signals, and no instances of other modules. Unlike `Modules`, both _do_ have parameters. `Primitives` each have an associated `paramclass`, while `ExternalModules` can optionally declare one via their `paramtype` attribute. Their parameter-types are limited to a small subset of those possible for `Generators` - generally "scalar" types such as numbers, strings, and `Scalar` - primarily limited by the need to need to provide them to legacy HDLs. Parameters are applied in the same style as for `Generators`, by calling the `Primitive` or `ExternalModule`. Parameter-applications can either be an instance of the module's `paramtype` or a set of keyword arguments which validly contruct one inline.
+
+```python
+# Continuing from the snippet above:
+params = BandGapParams(self_destruct=False)  # Watch out there!
+```
+
+`Primitives` and `ExternalModules` can be instantiated and connected in all the same styles as `Modules`:
+
+```python
+@h.module
+class BandGapPlus:
+    vref, enable = h.Signals(2)
+    # Instantiate the `ExternalModule` defined above
+    bg = BandGap(params)(vref=vref, enable=enable)
+    # ...Anything else...
+
+@h.module
+class DiodePlus:
+    p, n = h.Signals(2)
+    # Parameterize, instantiate, and connect a `primitives.Diode`
+    d = Diode(w=1 * µ, l=1 * µ)(p=p, n=n)
+    # ... Everything else ...
+```
+
 ## Exporting and Importing
 
-Hdl21's primary import/ export format is [VLSIR](https://github.com/Vlsir/Vlsir). VLSIR is a binary ProtoBuf-based format with support for a variety of industry-standard formats and tools. The `hdl21.to_proto()` function converts an Hdl21 `Module` or group of `Modules` into VLSIR `Package`. The `hdl21.from_proto()` function similarly imports a VLSIR `Package` into a namespace of Hdl21 `Modules`.
+Hdl21 generates hardware databases in the [VLSIR](https://github.com/Vlsir/Vlsir) interchange formats, defined through [Google Protocol Buffers](https://developers.google.com/protocol-buffers/). Through [VLSIR's Python tools](https://pypi.org/project/vlsirtools/) Hdl21 also includes drivers for popular industry-standard data formats and popular spice-class simulation engines.
+
+The `hdl21.to_proto()` function converts an Hdl21 `Module` or group of `Modules` into a VLSIR `Package`. The `hdl21.from_proto()` function similarly imports a VLSIR `Package` into a Python namespace of Hdl21 `Modules`.
 
 Exporting to industry-standard netlist formats is a particularly common operation for Hdl21 users. The `hdl21.netlist()` function uses VLSIR to export any of its supported netlist formats.
 
 ```python
 import sys
 import hdl21 as h
 
@@ -350,28 +533,45 @@
     cap = h.Cap(c=1e3)(p=p, n=n)
     ind = h.Ind(l=1e-9)(p=p, n=n)
 
 # Write a spice-format netlist to stdout
 h.netlist(Rlc, sys.stdout, fmt="spice")
 ```
 
-`hdl21.netlist` takes a second destination argument `dest`, which is commonly either an open file-handle or `sys.stdout`. All its remaining arguments are passed to `vlsirtools.netlist`.
+`hdl21.netlist` takes a second destination argument `dest`, which is commonly either an open file-handle or `sys.stdout`.
+
+Each `Module` includes a list of `Literal` contents, designed to be included directly in exported netlists. These are commonly used to refer to out-of-Hdl21 quantities, or to include netlist-language features not first-class supported by Hdl21. Example:
+
+```python
+@h.module
+class HasLiterals:
+    a, b, c = h.Ports(3)
+
+# Add some literal content
+HasLiterals.literals.extend([
+    h.Literal("generate some_verilog_code"),
+    h.Literal(".some_spice_attribute what=ever"),
+    h.Literal("PRAGMA: some_pragma"),
+])
+```
+
+`Module.literals` is a Python built-in list and can be manipulated with any of its typical methods (`append`, `extend`, etc.). Literals are written to netlists in the order they appear in the list. Order between Literals and other Module content is not preserved.
 
 ## Spice-Class Simulation
 
 Hdl21 includes drivers for popular spice-class simulation engines commonly used to evaluate analog circuits.
 The `hdl21.sim` package includes a wide variety of spice-class simulation constructs, including:
 
 - DC, AC, Transient, Operating-Point, Noise, Monte-Carlo, Parameter-Sweep and Custom (per netlist language) Analyses
 - Control elements for saving signals (`Save`), simulation options (`Options`), including external files and contents (`Include`, `Lib`), measurements (`Meas`), simulation parameters (`Param`), and literal netlist commands (`Literal`)
 
 The entrypoint to Hdl21-driven simulation is the simulation-input type `hdl21.sim.Sim`. Each `Sim` includes:
 
 - A testbench Module `tb`, and
-- A list of unordered simulation attributes (`attrs`), including any and all of the analyses, controls, and related elements listed above.
+- A list of simulation attributes (`attrs`), including any and all of the analyses, controls, and related elements listed above.
 
 Example:
 
 ```python
 import hdl21 as h
 from hdl21.sim import *
 
@@ -406,23 +606,26 @@
     ],
 )
 
 # And run it!
 sim.run()
 ```
 
-`Sim` also includes a class-based syntax similar to `Module` and `Bundle`, in which simulation attributes are named based on their class attribute name:
+`Sim` also includes a class-based syntax similar to `Module` and `Bundle`. This also allows for inline definition of a testbench module, which can be named either `tb` or `Tb`:
 
 ```python
 import hdl21 as h
 from hdl21.sim import *
 
 @sim
 class MySim:
-    tb = MyModulesTestbench
+
+    @h.module
+    class Tb:
+        # ... Testbench content ...
 
     x = Param(5)
     y = Param(6)
     mydc = Dc(var=x, sweep=PointSweep([1]))
     myac = Ac(sweep=LogSweep(1e1, 1e10, 10))
     mytran = Tran(tstop=11 * h.prefix.PICO)
     mysweep = SweepAnalysis(
@@ -442,15 +645,15 @@
 MySim.run()
 ```
 
 Note that in these class-based definitions, attributes whose names don't really matter such as `save_all` above can be _named_ anything, but must be _assigned_ into the class, not just constructed.
 
 Class-based `Sim` definitions retain all class members which are `SimAttr`s and drop all others. Non-`SimAttr`-valued fields can nonetheless be handy for defining intermediate values upon which the ultimate SimAttrs depend, such as the `a_path` field in the example above.
 
-Classes decoratated by `sim` a single special required field: a `tb` attribute which sets the simulation testbench. A handful of names are disallowed in `sim` class-definitions, generally corresponding to the names of the `Sim` class's fields and methods such as `attrs` and `run`.
+Classes decorated by `@sim` have a single special required field: a testbench attribute, named either `tb` or `Tb`, which sets the simulation testbench. A handful of names are disallowed in `sim` class-definitions, generally corresponding to the names of the `Sim` class's fields and methods such as `attrs` and `run`.
 
 Each `sim` also includes a set of methods to add simulation attributes from their keyword constructor arguments. These methods use the same names as the simulation attributes (`Dc`, `Meas`, etc.) but incorporating the python language convention that functions and methods be lowercase (`dc`, `meas`, etc.). Example:
 
 ```python
 # Create a `Sim`
 s = Sim(tb=MyTb)
 
@@ -475,137 +678,52 @@
 s.lib(path="/home/models", section="fast")
 s.options(reltol=1e-9)
 
 # And run it!
 s.run()
 ```
 
-## Primitives and External Modules
-
-The leaf-nodes of each hierarchical Hdl21 circuit are generally defined in one of two places:
-
-- `Primitive` elements, defined in the `hdl21.primitives` package. These include transistors, resistors, capacitors, and other irreducible components. Simulation-level behavior of these elements is typically defined _inside of_ simulation tools and other EDA software.
-- `ExternalModules`, defined outside Hdl21. Such "module wrappers", which might alternately be called "black boxes", are common for including circuits from other HDLs.
-
-### `Primitives`
-
-Hdl21 `Primitives` come in _ideal_ and _physical_ flavors. The difference is most frequently relevant for passive elements, which can for example represent either (a) technology-specific passives, e.g. a MIM or MOS capacitor, or (b) an _ideal_ capacitor. Some element-types have solely physical implementations, some are solely ideal, and others include both.
-
-### The `hdl21.primitives` Library
-
-The `Primitive` type and all its valid values are defined by the `hdl21.primitives` package. A summary of the `hdl21.primitives` library content:
-
-| Name                           | Description                       | Type     | Aliases                               | Ports        |
-| ------------------------------ | --------------------------------- | -------- | ------------------------------------- | ------------ |
-| Mos                            | Mos Transistor                    | PHYSICAL | MOS                                   | d, g, s, b   |
-| IdealResistor                  | Ideal Resistor                    | IDEAL    | R, Res, Resistor, IdealR, IdealRes    | p, n         |
-| PhysicalResistor               | Physical Resistor                 | PHYSICAL | PhyR, PhyRes, ResPhy, PhyResistor     | p, n         |
-| ThreeTerminalResistor          | Three Terminal Resistor           | PHYSICAL | Res3, PhyRes3, ResPhy3, PhyResistor3  | p, n, b      |
-| IdealCapacitor                 | Ideal Capacitor                   | IDEAL    | C, Cap, Capacitor, IdealC, IdealCap   | p, n         |
-| PhysicalCapacitor              | Physical Capacitor                | PHYSICAL | PhyC, PhyCap, CapPhy, PhyCapacitor    | p, n         |
-| ThreeTerminalCapacitor         | Three Terminal Capacitor          | PHYSICAL | Cap3, PhyCap3, CapPhy3, PhyCapacitor3 | p, n, b      |
-| IdealInductor                  | Ideal Inductor                    | IDEAL    | L, Ind, Inductor, IdealL, IdealInd    | p, n         |
-| PhysicalInductor               | Physical Inductor                 | PHYSICAL | PhyL, PhyInd, IndPhy, PhyInductor     | p, n         |
-| ThreeTerminalInductor          | Three Terminal Inductor           | PHYSICAL | Ind3, PhyInd3, IndPhy3, PhyInductor3  | p, n, b      |
-| PhysicalShort                  | Short-Circuit/ Net-Tie            | PHYSICAL | Short                                 | p, n         |
-| DcVoltageSource                | DC Voltage Source                 | IDEAL    | V, Vdc, Vsrc                          | p, n         |
-| PulseVoltageSource             | Pulse Voltage Source              | IDEAL    | Vpu, Vpulse                           | p, n         |
-| CurrentSource                  | Ideal DC Current Source           | IDEAL    | I, Idc, Isrc                          | p, n         |
-| VoltageControlledVoltageSource | Voltage Controlled Voltage Source | IDEAL    | Vcvs, VCVS                            | p, n, cp, cn |
-| CurrentControlledVoltageSource | Current Controlled Voltage Source | IDEAL    | Ccvs, CCVS                            | p, n, cp, cn |
-| VoltageControlledCurrentSource | Voltage Controlled Current Source | IDEAL    | Vccs, VCCS                            | p, n, cp, cn |
-| CurrentControlledCurrentSource | Current Controlled Current Source | IDEAL    | Cccs, CCCS                            | p, n, cp, cn |
-| Bipolar                        | Bipolar Transistor                | PHYSICAL | Bjt, BJT                              | c, b, e      |
-| Diode                          | Diode                             | PHYSICAL | D                                     | p, n         |
-
-Each primitive is available in the `hdl21.primitives` namespace, either through its full name or any of its aliases. Most primitives have fairly verbose names (e.g. `VoltageControlledCurrentSource`, `IdealResistor`), but also expose short-form aliases (e.g. `Vcvs`, `R`). Each of the aliases in Table 1 above refer to _the same_ Python object, i.e.
-
-```python
-from hdl21.primitives import R, Res, IdealResistor
-
-R is Res            # evaluates to True
-R is IdealResistor  # also evaluates to True
-```
-
-### `ExternalModules`
-
-Alternately Hdl21 includes an `ExternalModule` type which defines the interface to a module-implementation outside Hdl21. These external definitions are common for instantiating technology-specific modules and libraries. Other popular modern HDLs refer to these as module _black boxes_. An example `ExternalModule`:
-
-```python
-import hdl21 as h
-from hdl21.prefix import µ
-from hdl21.primitives import Diode
-
-@h.paramclass
-class BandGapParams:
-    self_destruct = h.Param(
-        dtype=bool,
-        desc="Whether to include the self-destruction feature",
-        default=True,
-    )
-
-BandGap = h.ExternalModule(
-    name="BandGap",
-    desc="Example ExternalModule, defined outside Hdl21",
-    port_list=[h.Port(name="vref"), h.Port(name="enable")],
-    paramtype=BandGapParams,
-)
-```
-
-Both `Primitives` and `ExternalModules` have names, ordered `Ports`, and a few other pieces of metadata, but no internal implementation: no internal signals, and no instances of other modules. Unlike `Modules`, both _do_ have parameters. `Primitives` each have an associated `paramclass`, while `ExternalModules` can optionally declare one via their `paramtype` attribute. Their parameter-types are limited to a small subset of those possible for `Generators` - scalar numeric types (`int`, `float`) and `str` - primarily limited by the need to need to provide them to legacy HDLs.
-
-`Primitives` and `ExternalModules` can be instantiated and connected in all the same styles as `Modules`:
-
-```python
-# Continuing from the snippet above:
-params = BandGapParams(self_destruct=False)  # Watch out there!
-
-@h.module
-class BandGapPlus:
-    vref, enable = h.Signals(2)
-    # Instantiate the `ExternalModule` defined above
-    bg = BandGap(params)(vref=vref, enable=enable)
-    # ...Anything else...
-
-@h.module
-class DiodePlus:
-    p, n = h.Signals(2)
-    # Parameterize, instantiate, and connect a `primitives.Diode`
-    d = Diode(w=1 * µ, l=1 * µ)(p=p, n=n)
-    # ... Everything else ...
-```
-
 ## Process Technologies
 
 Designing for a specific implementation technology (or "process development kit", or PDK) with Hdl21 can use either of (or a combination of) two routes:
 
 - Instantiate `ExternalModules` corresponding to the target technology. These would commonly include its process-specific transistor and passive modules, and potentially larger cells, for example from a cell library. Such external modules are frequently defined as part of a PDK (python) package, but can also be defined anywhere else, including inline among Hdl21 generator code.
-- Use `hdl21.Primitives`, each of which is designed to be a technology-independent representation of a primitive component. Moving to a particular technology then generally requires passing the design through an `hdl21.pdk` converter.
+- Use `hdl21.Primitives`, each of which is designed to be a technology-independent representation of a primitive component. Moving to a particular technology then generally requires passing the design through an `hdl21.pdk`'s `compile` function.
 
 Hdl21 PDKs are Python packages which generally include two primary elements:
 
 - (a) A library `ExternalModules` describing the technology's cells, and
 - (b) A `compile` conversion-method which transforms a hierarchical Hdl21 tree, mapping generic `hdl21.Primitives` into the tech-specific `ExternalModules`.
 
-Since PDKs are python packages, using them is as simple as importing them. Hdl21 includes two built-in PDKs: the academic predicitive [ASAP7](https://pypi.org/project/asap7-hdl21/) technology, and the open-source [SkyWater 130nm](https://pypi.org/project/sky130-hdl21/) technology.
+Since PDKs are python packages, using them is as simple as importing them. Hdl21 includes a built-in sample PDK available via `hdl21.pdk.sample_pdk` which includes simulatable NMOS and PMOS transistors. Hdl21's source tree includes three additional PDK packages:
+
+|                                       | PyPi                                   | Source        |
+| ------------------------------------- | -------------------------------------- | ------------- |
+| ASAP7 Predictive/ Academic PDK        | https://pypi.org/project/asap7-hdl21/  | [pdks/Asap7](./pdks/Asap7)  |
+| SkyWater 130nm Open-Source PDK        | https://pypi.org/project/sky130-hdl21/ | [pdks/Sky130](./pdks/Sky130) |
+| GlobalFoundries 180nm Open-Source PDK | https://pypi.org/project/gf180-hdl21   | [pdks/Gf180](./pdks/Gf180)  |
+
+Each contain much more detail documentation on their specific installation and use.
 
 ```python
 import hdl21 as h
-import sky130
+import sky130_hdl21
 
 @h.module
 class SkyInv:
     """ An inverter, demonstrating using PDK modules """
 
     # Create some IO
     i, o, VDD, VSS = h.Ports(4)
 
+    p = sky130_hdl21.Sky130MosParams(w=1,l=1)
+
     # And create some transistors!
-    ps = sky130.modules.sky130_fd_pr__pfet_01v8(w=1, l=1)(d=o, g=i, s=VDD, b=VDD)
-    ns = sky130.modules.sky130_fd_pr__nfet_01v8(w=1, l=1)(d=o, g=i, s=VSS, b=VSS)
+    ps = sky130_hdl21.primtives.PMOS_1p8V_STD(p)(d=o, g=i, s=VDD, b=VDD)
+    ns = sky130_hdl21.primtives.NMOS_1p8V_STD(p)(d=o, g=i, s=VSS, b=VSS)
 ```
 
 Process-portable modules instead use Hdl21 `Primitives`, which can be compiled to a target technology:
 
 ```python
 import hdl21 as h
 from hdl21.prefix import µ
@@ -623,17 +741,17 @@
     ns = Nmos(w=1*µ, l=1*µ, vth=MosVth.STD)(d=o, g=i, s=VSS, b=VSS)
 ```
 
 Compiling the generic devices to a target PDK then just requires a pass through the PDK's `compile()` method:
 
 ```python
 import hdl21 as h
-import sky130
+import sky130_hdl21
 
-sky130.compile(Inv) # Produces the same content as `SkyInv` above
+sky130_hdl21.compile(Inv) # Produces the same content as `SkyInv` above
 ```
 
 Hdl21 includes an `hdl21.pdk` subpackage which tracks the available in-memory PDKs. If there is a single PDK available, it need not be explicitly imported: `hdl21.pdk.compile()` will use it by default.
 
 ```python
 import hdl21 as h
 import sky130  # Note this import can be elsewhere in the program, i.e. in a configuration layer.
@@ -670,15 +788,15 @@
 CmosCorner = TT | FF | SS | SF | FS
 ```
 
 Hdl21 exposes each of these corner-types as Python enumerations and combinations thereof. Each PDK package then defines its mapping from these `Corner` types to the content they include, typically in the form of external files.
 
 ### PDK Installations and Sites
 
-Much of the content of a typical process technology - even the subset that Hdl21 cares about - is not defined in Python. Transistor models and SPICE "library" files, such as those defining the `_nfet` and `_pfet` above, are common examples pertinent to Hdl21. Tech-files, layout libraries, and the like are similarly necessary for related pieces of EDA software. These PDK contents are commonly stored in a technology-specific arrangement of interdependent files. Hdl21 PDK packages structure this external content as a `PdkInstallation` type.
+Much of the content of a typical process technology - even the subset that Hdl21 cares about - is not defined in Python. Transistor models and SPICE "library" files, such as those defining the `PMOS` and `NMOS` above, are common examples pertinent to Hdl21. Tech-files, layout libraries, and the like are similarly necessary for related pieces of EDA software. These PDK contents are commonly stored in a technology-specific arrangement of interdependent files. Hdl21 PDK packages structure this external content as a `PdkInstallation` type.
 
 Each `PdkInstallation` is a runtime type-checked Python `dataclass` which extends the base `hdl21.pdk.PdkInstallation` type. Installations are free to define arbitrary fields and methods, which will be type-validated for each `Install` instance. Example:
 
 ```python
 """ A sample PDK package with an `Install` type """
 
 from pydantic.dataclasses import dataclass
@@ -726,19 +844,19 @@
 
 These "site packages" are named `sitepdks` by convention. They can often be shared among several PDKs on a given filesystem. Hdl21 includes one built-in example such site-package, [SampleSitePdks](./SampleSitePdks/), which demonstrates setting up both built-in PDKs, Sky130 and ASAP7:
 
 ```python
 # The built-in sample `sitepdks` package
 from pathlib import Path
 
-import sky130
-sky130.install = sky130.Install(model_lib=Path("pdks") / "sky130" / ... / "sky130.lib.spice")
+import sky130_hdl21
+sky130_hdl21.install = sky130_hdl21.Install(model_lib=Path("pdks") / "sky130" / ... / "sky130.lib.spice")
 
-import asap7
-asap7.install = asap7.Install(model_lib=Path("pdks") / "asap7" / ... / "TT.pm")
+import asap7_hdl21
+asap7_hdl21.install = asap7_hdl21.Install(model_lib=Path("pdks") / "asap7" / ... / "TT.pm")
 ```
 
 "Site-portable" code requiring external PDK content can then refer to the PDK package's `install`, without being directly aware of its contents.
 An example simulation using `mypdk`'s models with the `sitepdk`s defined above:
 
 ```python
 # sim_my_pdk.py
@@ -758,25 +876,218 @@
 
 # And run it!
 SimMyPdk.run()
 ```
 
 Note that `sim_my_pdk.py` need not necessarily import or directly depend upon `sitepdks` itself. So long as `sitepdks` is imported and configures the PDK installation anywhere in the Python program, further code will be able to refer to the PDK's `install` fields.
 
-## Examples Library
+### Creating PDK Packages
+
+Hdl21's source tree includes a [cookiecutter template](https://github.com/cookiecutter/cookiecutter) for creating a new PDK package, available at [pdks/PdkTemplate](./pdks/PdkTemplate).
+
+## Bundles
+
+Hdl21 `Bundle`s are _structured connection types_ which can include `Signal`s and instances of other `Bundle`s.
+Think of them as "connection structs". Similar ideas are implemented by Chisel's `Bundle`s and SystemVerilog's `interface`s.
+
+```python
+@h.bundle
+class Diff:
+    p = h.Signal()
+    n = h.Signal()
+
+@h.bundle
+class Quadrature:
+    i = Diff()
+    q = Diff()
+```
+
+Like `Module`s, `Bundle`s can be defined either procedurally or as a class decorated by the `hdl21.bundle` function.
+
+```python
+# This creates the same stuff as the class-based definitions above:
+
+Diff = h.Bundle(name="Diff")
+Diff.add(h.Signal(name="p"))
+Diff.add(h.Signal(name="n"))
+
+Quadrature = h.Bundle(name="Quadrature")
+Quadrature.add(Diff(name="i"))
+Quadrature.add(Diff(name="q"))
+```
+
+Calling a `Bundle` as in the calls to `Diff()` and `Diff(name=q)` creates an instance of that `Bundle`.
+
+## Bundle Ports
+
+Bundles are commonly most valuable for shipping collections of related `Signal`s between `Module`s.
+Modules can accordingly have Bundle-valued ports. To create a Bundle-port, set the `port` argument to either the boolean `True`
+or the `hdl21.Visibility.PORT` value.
+
+```python
+@h.module
+class HasDiffs:
+    d1 = Diff(port=True)
+    d2 = Diff(port=h.Visbility.PORT)
+```
+
+Port directions on bundle-ports can be set by either of two methods.
+The first is to set the directions directly on the Bundle's constituent `Signal`s.
+To swap directions, pass the bundle-instances through the `hdl21.flipped` function,
+or set the `flipped` argument to the instance-constructor.
+
+```python
+@h.bundle
+class Inner:
+    i = h.Input()
+    o = h.Output()
+
+@h.bundle
+class Outer:
+    b1 = Inner()
+    b2 = h.flipped(Inner())
+    b3 = Inner(flipped=True)
+```
+
+Here:
+
+- An `Inner` bundle defines an `Input` and an `Output`
+- An `Outer` bundle instantiates three of them
+  - Instance `b1` is not flipped; its `i` is an input, and its `o` is an output
+  - Instance `b2` is flipped; its `i` is an _output_, and its `o` is an _input_
+  - Instance `b3` is also flipped, via its constructor argument
+
+These "flipping based" bundles require that all constituent signals, including nested ones, have port-visibility.
+The rules for flipping port directions are:
+
+- Inputs become Outputs
+- Outputs become Inputs
+- Inouts and undirected ports (`direction=NONE`) retain their directions
+
+```python
+@h.bundle
+class B:
+    clk = h.Output()
+    data = h.Input()
+
+@h.module
+class X: # Module with a `clk` output and `data` input
+    b = B(port=True)
+
+@h.module
+class Y: # Module with a `clk` input and `data` output
+    b = B(flipped=True, port=True)
+
+@h.module
+class Z:
+    b = B() # Internal instance of the `B` bundle
+    x = X(b=b)
+    y = Y(b=b)
+```
+
+The second method for setting bundle-port directions is with `Role`s.
+Each Hdl21 bundle either explicitly or implictly defines a set of `Role`s, which might alternately be called "endpoints".
+These are the expected "end users" of the Bundle.
+Signal directions are then defined on each signal's `src` (source) and `dest` (destination) arguments, which can be set to any of the bundle's roles.
+
+```python
+@h.roles
+class HostDevice(Enum):
+    HOST = auto()
+    DEVICE = auto()
+
+@h.bundle
+class Jtag:
+    roles = HostDevice # Set the bundle's roles
+    # Note each signal sets one of the roles as `src` and another as `dest`
+    tck, tdi, tms = h.Signals(3, src=roles.HOST, dest=roles.DEVICE)
+    tdo = h.Signal(src=roles.DEVICE, dest=roles.HOST)
+```
+
+Bundle-valued ports are then assigned a role and associated signal-port directions via their `role` constructor argument.
+
+```python
+@h.module
+class Widget: # with a Jtag Device port
+    jtag = Jtag(port=True, role=Jtag.roles.DEVICE)
+
+@h.module
+class Debugger: # with a Jtag Host port
+    jtag = Jtag(port=True, role=Jtag.roles.HOST)
+
+@h.module
+class System: # combining the two
+    widget = Widget()
+    debugger = Debugger(jtag=widget.jtag)
+```
+
+The rules for port-directions of role-based bundles are:
+
+- If the bundle's role is the signal's source, the signal is an `Output`
+- If the bundle's role is the signal's destination, the signal is an `Input`
+- Otherwise the signal is assigned no direction, i.e. `direction=NONE`
+
+## Collecting Bundles
+
+It is often helpful or necessary to collect existing signals into a bundle, or to "re-arrange" signals from one bundle into another.
+The primary mechanism for doing so is the `hdl21.bundlize` function which creates them.
+Each call to `bundlize` creates an "anonymous" bundle which lacks a backing bundle-definition type.
+
+```python
+@h.bundle
+class Uart:
+    tx = h.Output()
+    rx = h.Input()
+
+@h.module
+class HasUart:
+    # Module with a `Uart` port
+    uart = Uart(port=True)
+
+@h.module
+class ConnectTwo:
+    # Connect two `HasUart`s, swapping `tx` and `rx`.
+    uart = Uart()
+    m1 = HasUart(uart=uart)
+    m2 = HasUart(uart=h.bundlize(tx=uart.rx, rx=uart.tx))
+```
+
+## Examples
+
+### Built-In Examples Library
 
 Hdl21's source tree includes a built-in [examples](./examples/) library. Each is designed to be a straightforward but realistic use-case, and is a self-contained Python program which can be run directly, e.g. with:
 
 ```bash
 python examples/rdac.py
 ```
 
+The built-in examples include:
+
+- [Current DAC](./examples/idac.py)
+- [MOS Transistor Simulation](./examples/mos_sim.py)
+- [Ring Oscillator Generator](./examples/ro.py)
+- [Resistor-Ladder DAC](./examples/rdac.py)
+- [Recursive Binary to One-Hot Encoders](./examples/encoder.py)
+
 Reading, copying, or cloning these example programs is generally among the best ways to get started.  
 And adding an example is a **highly** encouraged form of [pull request](https://github.com/dan-fritchman/Hdl21/pulls)!
 
+### Featured Community Examples
+
+- [Continuous-Time Delta-Sigma ADC Generators](https://github.com/aviralpandey/CT-DS-ADC_generator)
+- [USB 2.0 PHY](https://github.com/Vlsir/Usb2Phy/tree/main/Usb2PhyAna)
+- [VCO-Based ADC Generators](https://github.com/aviralpandey) (Coming soon!)
+
+## Related Projects
+
+- [VLSIR](https://github.com/vlsir/vlsir)
+- [Hdl21 Schematics](https://github.com/vlsir/hdl21schematics)
+- [Layout21](https://github.com/dan-fritchman/Layout21)
+
 ## Why Use Python?
 
 Custom IC design is a complicated field. Its practitioners have to know
 [a](https://people.eecs.berkeley.edu/~boser/courses/240B/lectures/M07%20OTA%20II.pdf) |
 [lot](http://rfic.eecs.berkeley.edu/~niknejad/ee142_fa05lects/pdf/lect24.pdf) |
 [of](https://www.delroy.com/PLL_dir/ISSCC2004/PLLTutorialISSCC2004.pdf) |
 [stuff](https://inst.eecs.berkeley.edu/~ee247/fa10/files07/lectures/L25_2_f10.pdf),
```

### Comparing `hdl21-3.0.dev3/scripts/primtable.py` & `hdl21-4.0.0rc0/scripts/primtable.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 # Primitive Table Generation 
 
 Writes the markdown-format table of primitives used in documentation.
 """
 
-import sys
-from typing import IO
+# import sys
+# from typing import IO
 from pydantic.dataclasses import dataclass
-from hdl21.primitives import _primitives, Primitive, PrimLibEntry
+from hdl21.primitives import _primitives, PrimLibEntry
 
 
 @dataclass
 class Widths:
     name: int
     desc: int
     prim_type: int
```

### Comparing `hdl21-3.0.dev3/setup.py` & `hdl21-4.0.0rc0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,41 +6,45 @@
 
 """
 
 # Always prefer setuptools over distutils
 from setuptools import setup, find_packages
 import pathlib
 
-here = pathlib.Path(__file__).parent.resolve()
-
 # Get the long description from the README file
-long_description = (here / "readme.md").read_text(encoding="utf-8")
+here = pathlib.Path(__file__).parent.resolve()
+readme = here / "readme.md"
+long_description = "" if not readme.exists() else readme.read_text(encoding="utf-8")
 
-_VLSIR_VERSION = "3.0.dev3"
+_VLSIR_VERSION = "4.0.0rc0"
 
 setup(
     name="hdl21",
     version=_VLSIR_VERSION,
     description="Hardware Description Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dan-fritchman/Hdl21",
     author="Dan Fritchman",
     author_email="dan@fritch.mn",
     packages=find_packages(),
-    python_requires=">=3.7, <4",
+    package_data={"hdl21": ["**/*.sp"]},  # Include built-in PDK models
+    python_requires=">=3.7, <3.12",
     install_requires=[
         f"vlsir=={_VLSIR_VERSION}",
         f"vlsirtools=={_VLSIR_VERSION}",
-        "pydantic==1.9.1",
+        # Our primary external dependency is pydantic.
+        # Tested with everything in the 1.9-1.10 range.
+        "pydantic>=1.9.0,<1.11",
     ],
     extras_require={
         "dev": [
             "pytest==7.1",
             "coverage",
             "pytest-cov",
             "pre-commit==2.20",
             "black==22.6",
             "twine",
+            "build",
         ]
     },
 )
```

