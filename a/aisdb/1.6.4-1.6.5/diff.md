# Comparing `tmp/aisdb-1.6.4-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl.zip` & `tmp/aisdb-1.6.5-cp39-cp39-macosx_11_0_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,199 +1,237 @@
-Zip file size: 4307569 bytes, number of entries: 197
--rw-r--r--  4.6 unx     4949 b- defN 23-Jun-08 15:24 aisdb-1.6.4.dist-info/METADATA
--rw-r--r--  4.6 unx      129 b- defN 23-Jun-08 15:24 aisdb-1.6.4.dist-info/WHEEL
--rw-r--r--  4.6 unx     1605 b- defN 23-Jun-08 15:24 aisdb/__init__.py
--rw-r--r--  4.6 unx     4924 b- defN 23-Jun-08 15:24 aisdb/aisdb_sql/coarsetype.sql
--rw-r--r--  4.6 unx      358 b- defN 23-Jun-08 15:24 aisdb/aisdb_sql/createtable_dynamic_clustered.sql
--rw-r--r--  4.6 unx      108 b- defN 23-Jun-08 15:24 aisdb/aisdb_sql/createtable_griddata.sql
--rw-r--r--  4.6 unx      539 b- defN 23-Jun-08 15:24 aisdb/aisdb_sql/createtable_static.sql
--rw-r--r--  4.6 unx      258 b- defN 23-Jun-08 15:24 aisdb/aisdb_sql/createtable_static_aggregate.sql
--rw-r--r--  4.6 unx      369 b- defN 23-Jun-08 15:24 aisdb/aisdb_sql/createtable_webdata_marinetraffic.sql
--rw-r--r--  4.6 unx       43 b- defN 23-Jun-08 15:24 aisdb/aisdb_sql/cte_aliases.sql
--rw-r--r--  4.6 unx       91 b- defN 23-Jun-08 15:24 aisdb/aisdb_sql/cte_coarsetype.sql
--rw-r--r--  4.6 unx      125 b- defN 23-Jun-08 15:24 aisdb/aisdb_sql/cte_dynamic_clusteredidx.sql
--rw-r--r--  4.6 unx      185 b- defN 23-Jun-08 15:24 aisdb/aisdb_sql/cte_static.sql
--rw-r--r--  4.6 unx      210 b- defN 23-Jun-08 15:24 aisdb/aisdb_sql/cte_static_aggregate.sql
--rw-r--r--  4.6 unx      230 b- defN 23-Jun-08 15:24 aisdb/aisdb_sql/insert_dynamic_clusteredidx.sql
--rw-r--r--  4.6 unx      400 b- defN 23-Jun-08 15:24 aisdb/aisdb_sql/insert_static.sql
--rw-r--r--  4.6 unx      763 b- defN 23-Jun-08 15:24 aisdb/aisdb_sql/insert_webdata_marinetraffic.sql
--rw-r--r--  4.6 unx      312 b- defN 23-Jun-08 15:24 aisdb/aisdb_sql/select_columns_static.sql
--rw-r--r--  4.6 unx      493 b- defN 23-Jun-08 15:24 aisdb/aisdb_sql/select_join_dynamic_static_clusteredidx.sql
--rw-r--r--  4.6 unx      881 b- defN 23-Jun-08 15:24 aisdb/aisdb_sql/select_merged_all.sql
--rw-r--r--  4.6 unx      658 b- defN 23-Jun-08 15:24 aisdb/aisdb_sql/select_static_join_webdata.sql
--rw-r--r--  4.6 unx        1 b- defN 23-Jun-08 15:24 aisdb/database/__init__.py
--rw-r--r--  4.6 unx     4900 b- defN 23-Jun-08 15:24 aisdb/database/create_tables.py
--rw-r--r--  4.6 unx     6358 b- defN 23-Jun-08 15:24 aisdb/database/dbconn.py
--rw-r--r--  4.6 unx    11962 b- defN 23-Jun-08 15:24 aisdb/database/dbqry.py
--rw-r--r--  4.6 unx     9816 b- defN 23-Jun-08 15:24 aisdb/database/decoder.py
--rw-r--r--  4.6 unx     4170 b- defN 23-Jun-08 15:24 aisdb/database/sql_query_strings.py
--rw-r--r--  4.6 unx     3188 b- defN 23-Jun-08 15:24 aisdb/database/sqlfcn.py
--rw-r--r--  4.6 unx     1739 b- defN 23-Jun-08 15:24 aisdb/database/sqlfcn_callbacks.py
--rw-r--r--  4.6 unx     7783 b- defN 23-Jun-08 15:24 aisdb/denoising_encoder.py
--rw-r--r--  4.6 unx    18568 b- defN 23-Jun-08 15:24 aisdb/gis.py
--rw-r--r--  4.6 unx     1599 b- defN 23-Jun-08 15:24 aisdb/interp.py
--rw-r--r--  4.6 unx    18893 b- defN 23-Jun-08 15:24 aisdb/network_graph.py
--rw-r--r--  4.6 unx     8060 b- defN 23-Jun-08 15:24 aisdb/proc_util.py
--rw-r--r--  4.6 unx     2470 b- defN 23-Jun-08 15:24 aisdb/receiver.py
--rw-r--r--  4.6 unx        0 b- defN 23-Jun-08 15:24 aisdb/tests/__init__.py
--rw-r--r--  4.6 unx     3139 b- defN 23-Jun-08 15:24 aisdb/tests/create_testing_data.py
--rw-r--r--  4.6 unx     1420 b- defN 23-Jun-08 15:24 aisdb/tests/test_00_decode.py
--rw-r--r--  4.6 unx     2738 b- defN 23-Jun-08 15:24 aisdb/tests/test_01_createtables.py
--rw-r--r--  4.6 unx     2803 b- defN 23-Jun-08 15:24 aisdb/tests/test_02_dbqry.py
--rw-r--r--  4.6 unx     2956 b- defN 23-Jun-08 15:24 aisdb/tests/test_02_sqlfcn.py
--rw-r--r--  4.6 unx     2956 b- defN 23-Jun-08 15:24 aisdb/tests/test_03_gis.py
--rw-r--r--  4.6 unx     2332 b- defN 23-Jun-08 15:24 aisdb/tests/test_04_trackgen.py
--rw-r--r--  4.6 unx     4385 b- defN 23-Jun-08 15:24 aisdb/tests/test_05_proc_util.py
--rw-r--r--  4.6 unx     1090 b- defN 23-Jun-08 15:24 aisdb/tests/test_06_interp.py
--rw-r--r--  4.6 unx     1256 b- defN 23-Jun-08 15:24 aisdb/tests/test_07_bathymetry.py
--rw-r--r--  4.6 unx     1131 b- defN 23-Jun-08 15:24 aisdb/tests/test_07_shore_dist.py
--rw-r--r--  4.6 unx     2580 b- defN 23-Jun-08 15:24 aisdb/tests/test_08_marinetraffic.py
--rw-r--r--  4.6 unx     1679 b- defN 23-Jun-08 15:24 aisdb/tests/test_08_wsa.py
--rw-r--r--  4.6 unx     3596 b- defN 23-Jun-08 15:24 aisdb/tests/test_09_network_graph.py
--rw-r--r--  4.6 unx      778 b- defN 23-Jun-08 15:24 aisdb/tests/test_11_postgres.py
--rw-r--r--  4.6 unx       74 b- defN 23-Jun-08 15:24 aisdb/tests/test_rx.py
--rw-r--r--  4.6 unx    84630 b- defN 23-Jun-08 15:24 aisdb/tests/testdata/test_data_20211101.nm4
--rw-r--r--  4.6 unx    23613 b- defN 23-Jun-08 15:24 aisdb/tests/testdata/test_data_20211101.nm4.gz
--rw-r--r--  4.6 unx     7650 b- defN 23-Jun-08 15:24 aisdb/track_gen.py
--rw-r--r--  4.6 unx     6994 b- defN 23-Jun-08 15:24 aisdb/web_interface.py
--rw-r--r--  4.6 unx        0 b- defN 23-Jun-08 15:24 aisdb/webdata/__init__.py
--rw-r--r--  4.6 unx     2505 b- defN 23-Jun-08 15:24 aisdb/webdata/_scraper.py
--rw-r--r--  4.6 unx     5440 b- defN 23-Jun-08 15:24 aisdb/webdata/bathymetry.py
--rw-r--r--  4.6 unx     2448 b- defN 23-Jun-08 15:24 aisdb/webdata/load_raster.py
--rw-r--r--  4.6 unx    11002 b- defN 23-Jun-08 15:24 aisdb/webdata/marinetraffic.py
--rw-r--r--  4.6 unx     2690 b- defN 23-Jun-08 15:24 aisdb/webdata/shore_dist.py
--rw-r--r--  4.6 unx     3845 b- defN 23-Jun-08 15:24 aisdb/wsa.py
--rw-r--r--  4.6 unx     1605 b- defN 23-Jun-08 15:24 aisdb/__init__.py
--rw-r--r--  4.6 unx     7783 b- defN 23-Jun-08 15:24 aisdb/denoising_encoder.py
--rw-r--r--  4.6 unx    18568 b- defN 23-Jun-08 15:24 aisdb/gis.py
--rw-r--r--  4.6 unx     1599 b- defN 23-Jun-08 15:24 aisdb/interp.py
--rw-r--r--  4.6 unx    18893 b- defN 23-Jun-08 15:24 aisdb/network_graph.py
--rw-r--r--  4.6 unx     8060 b- defN 23-Jun-08 15:24 aisdb/proc_util.py
--rw-r--r--  4.6 unx     2470 b- defN 23-Jun-08 15:24 aisdb/receiver.py
--rw-r--r--  4.6 unx     7650 b- defN 23-Jun-08 15:24 aisdb/track_gen.py
--rw-r--r--  4.6 unx     6994 b- defN 23-Jun-08 15:24 aisdb/web_interface.py
--rw-r--r--  4.6 unx     3845 b- defN 23-Jun-08 15:24 aisdb/wsa.py
--rw-r--r--  4.6 unx     4924 b- defN 23-Jun-08 15:24 aisdb/aisdb_sql/coarsetype.sql
--rw-r--r--  4.6 unx      358 b- defN 23-Jun-08 15:24 aisdb/aisdb_sql/createtable_dynamic_clustered.sql
--rw-r--r--  4.6 unx      108 b- defN 23-Jun-08 15:24 aisdb/aisdb_sql/createtable_griddata.sql
--rw-r--r--  4.6 unx      539 b- defN 23-Jun-08 15:24 aisdb/aisdb_sql/createtable_static.sql
--rw-r--r--  4.6 unx      258 b- defN 23-Jun-08 15:24 aisdb/aisdb_sql/createtable_static_aggregate.sql
--rw-r--r--  4.6 unx      369 b- defN 23-Jun-08 15:24 aisdb/aisdb_sql/createtable_webdata_marinetraffic.sql
--rw-r--r--  4.6 unx       43 b- defN 23-Jun-08 15:24 aisdb/aisdb_sql/cte_aliases.sql
--rw-r--r--  4.6 unx       91 b- defN 23-Jun-08 15:24 aisdb/aisdb_sql/cte_coarsetype.sql
--rw-r--r--  4.6 unx      125 b- defN 23-Jun-08 15:24 aisdb/aisdb_sql/cte_dynamic_clusteredidx.sql
--rw-r--r--  4.6 unx      185 b- defN 23-Jun-08 15:24 aisdb/aisdb_sql/cte_static.sql
--rw-r--r--  4.6 unx      210 b- defN 23-Jun-08 15:24 aisdb/aisdb_sql/cte_static_aggregate.sql
--rw-r--r--  4.6 unx      230 b- defN 23-Jun-08 15:24 aisdb/aisdb_sql/insert_dynamic_clusteredidx.sql
--rw-r--r--  4.6 unx      400 b- defN 23-Jun-08 15:24 aisdb/aisdb_sql/insert_static.sql
--rw-r--r--  4.6 unx      763 b- defN 23-Jun-08 15:24 aisdb/aisdb_sql/insert_webdata_marinetraffic.sql
--rw-r--r--  4.6 unx      312 b- defN 23-Jun-08 15:24 aisdb/aisdb_sql/select_columns_static.sql
--rw-r--r--  4.6 unx      493 b- defN 23-Jun-08 15:24 aisdb/aisdb_sql/select_join_dynamic_static_clusteredidx.sql
--rw-r--r--  4.6 unx      881 b- defN 23-Jun-08 15:24 aisdb/aisdb_sql/select_merged_all.sql
--rw-r--r--  4.6 unx      658 b- defN 23-Jun-08 15:24 aisdb/aisdb_sql/select_static_join_webdata.sql
--rw-r--r--  4.6 unx        1 b- defN 23-Jun-08 15:24 aisdb/database/__init__.py
--rw-r--r--  4.6 unx     4900 b- defN 23-Jun-08 15:24 aisdb/database/create_tables.py
--rw-r--r--  4.6 unx     6358 b- defN 23-Jun-08 15:24 aisdb/database/dbconn.py
--rw-r--r--  4.6 unx    11962 b- defN 23-Jun-08 15:24 aisdb/database/dbqry.py
--rw-r--r--  4.6 unx     9816 b- defN 23-Jun-08 15:24 aisdb/database/decoder.py
--rw-r--r--  4.6 unx     4170 b- defN 23-Jun-08 15:24 aisdb/database/sql_query_strings.py
--rw-r--r--  4.6 unx     3188 b- defN 23-Jun-08 15:24 aisdb/database/sqlfcn.py
--rw-r--r--  4.6 unx     1739 b- defN 23-Jun-08 15:24 aisdb/database/sqlfcn_callbacks.py
--rw-r--r--  4.6 unx        0 b- defN 23-Jun-08 15:24 aisdb/tests/__init__.py
--rw-r--r--  4.6 unx     3139 b- defN 23-Jun-08 15:24 aisdb/tests/create_testing_data.py
--rw-r--r--  4.6 unx     1420 b- defN 23-Jun-08 15:24 aisdb/tests/test_00_decode.py
--rw-r--r--  4.6 unx     2738 b- defN 23-Jun-08 15:24 aisdb/tests/test_01_createtables.py
--rw-r--r--  4.6 unx     2803 b- defN 23-Jun-08 15:24 aisdb/tests/test_02_dbqry.py
--rw-r--r--  4.6 unx     2956 b- defN 23-Jun-08 15:24 aisdb/tests/test_02_sqlfcn.py
--rw-r--r--  4.6 unx     2956 b- defN 23-Jun-08 15:24 aisdb/tests/test_03_gis.py
--rw-r--r--  4.6 unx     2332 b- defN 23-Jun-08 15:24 aisdb/tests/test_04_trackgen.py
--rw-r--r--  4.6 unx     4385 b- defN 23-Jun-08 15:24 aisdb/tests/test_05_proc_util.py
--rw-r--r--  4.6 unx     1090 b- defN 23-Jun-08 15:24 aisdb/tests/test_06_interp.py
--rw-r--r--  4.6 unx     1256 b- defN 23-Jun-08 15:24 aisdb/tests/test_07_bathymetry.py
--rw-r--r--  4.6 unx     1131 b- defN 23-Jun-08 15:24 aisdb/tests/test_07_shore_dist.py
--rw-r--r--  4.6 unx     2580 b- defN 23-Jun-08 15:24 aisdb/tests/test_08_marinetraffic.py
--rw-r--r--  4.6 unx     1679 b- defN 23-Jun-08 15:24 aisdb/tests/test_08_wsa.py
--rw-r--r--  4.6 unx     3596 b- defN 23-Jun-08 15:24 aisdb/tests/test_09_network_graph.py
--rw-r--r--  4.6 unx      778 b- defN 23-Jun-08 15:24 aisdb/tests/test_11_postgres.py
--rw-r--r--  4.6 unx       74 b- defN 23-Jun-08 15:24 aisdb/tests/test_rx.py
--rw-r--r--  4.6 unx  1258678 b- defN 23-Jun-08 15:24 aisdb/tests/testdata/test_data_20210701.csv
--rwxr-xr-x  4.6 unx    84630 b- defN 23-Jun-08 15:24 aisdb/tests/testdata/test_data_20211101.nm4
--rw-r--r--  4.6 unx        0 b- defN 23-Jun-08 15:24 aisdb/webdata/__init__.py
--rw-r--r--  4.6 unx     2505 b- defN 23-Jun-08 15:24 aisdb/webdata/_scraper.py
--rw-r--r--  4.6 unx     5440 b- defN 23-Jun-08 15:24 aisdb/webdata/bathymetry.py
--rw-r--r--  4.6 unx     2448 b- defN 23-Jun-08 15:24 aisdb/webdata/load_raster.py
--rw-r--r--  4.6 unx    11002 b- defN 23-Jun-08 15:24 aisdb/webdata/marinetraffic.py
--rw-r--r--  4.6 unx     2690 b- defN 23-Jun-08 15:24 aisdb/webdata/shore_dist.py
--rw-r--r--  4.6 unx    36655 b- defN 23-Jun-08 15:24 aisdb_lib/Cargo.lock
--rw-r--r--  4.6 unx      946 b- defN 23-Jun-08 15:24 aisdb_lib/Cargo.toml
--rw-r--r--  4.6 unx      135 b- defN 23-Jun-08 15:24 aisdb_lib/build.rs
--rw-r--r--  4.6 unx     1672 b- defN 23-Jun-08 15:24 aisdb_web/dist_map/assets/OSM-18e3061c.js
--rw-r--r--  4.6 unx     1672 b- defN 23-Jun-08 15:24 aisdb_web/dist_map/assets/OSM-3d3b8c7a.js
--rw-r--r--  4.6 unx     1672 b- defN 23-Jun-08 15:24 aisdb_web/dist_map/assets/OSM-a7270865.js
--rw-r--r--  4.6 unx    17519 b- defN 23-Jun-08 15:24 aisdb_web/dist_map/assets/TileImage-865fdc14.js
--rw-r--r--  4.6 unx    17519 b- defN 23-Jun-08 15:24 aisdb_web/dist_map/assets/TileImage-e0a2bc65.js
--rw-r--r--  4.6 unx    17519 b- defN 23-Jun-08 15:24 aisdb_web/dist_map/assets/TileImage-e2e53f79.js
--rw-r--r--  4.6 unx   173279 b- defN 23-Jun-08 15:24 aisdb_web/dist_map/assets/client_bg-05f4a55d.wasm
--rw-r--r--  4.6 unx   173279 b- defN 23-Jun-08 15:24 aisdb_web/dist_map/assets/client_bg-6a509824.wasm
--rw-r--r--  4.6 unx   173278 b- defN 23-Jun-08 15:24 aisdb_web/dist_map/assets/client_bg-916ba2c4.wasm
--rw-r--r--  4.6 unx      723 b- defN 23-Jun-08 15:24 aisdb_web/dist_map/assets/constants-a418eeb2.js
--rw-r--r--  4.6 unx     8224 b- defN 23-Jun-08 15:24 aisdb_web/dist_map/assets/index-f2c4f58e.css
--rw-r--r--  4.6 unx     1185 b- defN 23-Jun-08 15:24 aisdb_web/dist_map/assets/livestream-04f2da24.js
--rw-r--r--  4.6 unx     1185 b- defN 23-Jun-08 15:24 aisdb_web/dist_map/assets/livestream-7a84f2e5.js
--rw-r--r--  4.6 unx     1185 b- defN 23-Jun-08 15:24 aisdb_web/dist_map/assets/livestream-7c48cb34.js
--rw-r--r--  4.6 unx     2662 b- defN 23-Jun-08 15:24 aisdb_web/dist_map/assets/main-12a41ab2.js
--rw-r--r--  4.6 unx     2662 b- defN 23-Jun-08 15:24 aisdb_web/dist_map/assets/main-b42e8f3c.js
--rw-r--r--  4.6 unx     2662 b- defN 23-Jun-08 15:24 aisdb_web/dist_map/assets/main-c046974e.js
--rw-r--r--  4.6 unx   405869 b- defN 23-Jun-08 15:24 aisdb_web/dist_map/assets/map-0df0429f.js
--rw-r--r--  4.6 unx   405869 b- defN 23-Jun-08 15:24 aisdb_web/dist_map/assets/map-abddb635.js
--rw-r--r--  4.6 unx   405869 b- defN 23-Jun-08 15:24 aisdb_web/dist_map/assets/map-b057f40e.js
--rw-r--r--  4.6 unx    15782 b- defN 23-Jun-08 15:24 aisdb_web/dist_map/assets/map-c04ede37.css
--rw-r--r--  4.6 unx    16622 b- defN 23-Jun-08 15:24 aisdb_web/dist_map/assets/proj-3e4e3ac0.js
--rw-r--r--  4.6 unx   203253 b- defN 23-Jun-08 15:24 aisdb_web/dist_map/assets/render-15f8910a.js
--rw-r--r--  4.6 unx   203253 b- defN 23-Jun-08 15:24 aisdb_web/dist_map/assets/render-29aaa5e2.js
--rw-r--r--  4.6 unx   203253 b- defN 23-Jun-08 15:24 aisdb_web/dist_map/assets/render-9978d19f.js
--rw-r--r--  4.6 unx     3092 b- defN 23-Jun-08 15:24 aisdb_web/dist_map/assets/tileserver-24a57af3.js
--rw-r--r--  4.6 unx     3092 b- defN 23-Jun-08 15:24 aisdb_web/dist_map/assets/tileserver-8260d47b.js
--rw-r--r--  4.6 unx     3092 b- defN 23-Jun-08 15:24 aisdb_web/dist_map/assets/tileserver-b56401ad.js
--rw-r--r--  4.6 unx     3114 b- defN 23-Jun-08 15:24 aisdb_web/dist_map/assets/url-3f93404c.js
--rw-r--r--  4.6 unx     3114 b- defN 23-Jun-08 15:24 aisdb_web/dist_map/assets/url-7cac731b.js
--rw-r--r--  4.6 unx     3114 b- defN 23-Jun-08 15:24 aisdb_web/dist_map/assets/url-b43e4d73.js
--rw-r--r--  4.6 unx     1203 b- defN 23-Jun-08 15:24 aisdb_web/dist_map/assets/vessel_metadata-52b84ad7.js
--rw-r--r--  4.6 unx     1203 b- defN 23-Jun-08 15:24 aisdb_web/dist_map/assets/vessel_metadata-a539ebc6.js
--rw-r--r--  4.6 unx     1203 b- defN 23-Jun-08 15:24 aisdb_web/dist_map/assets/vessel_metadata-d682b0f2.js
--rw-rw-rw-  4.6 unx    26223 b- defN 23-Jun-08 15:24 aisdb_web/dist_map/favicon.png
--rw-rw-rw-  4.6 unx    21560 b- defN 23-Jun-08 15:24 aisdb_web/dist_map/favicon.svg
--rw-r--r--  4.6 unx     2615 b- defN 23-Jun-08 15:24 aisdb_web/dist_map/index.html
--rw-r--r--  4.6 unx   173279 b- defN 23-Jun-08 15:24 aisdb_web/dist_map_bingmaps/assets/client_bg-05f4a55d.wasm
--rw-r--r--  4.6 unx   173279 b- defN 23-Jun-08 15:24 aisdb_web/dist_map_bingmaps/assets/client_bg-6a509824.wasm
--rw-r--r--  4.6 unx   173278 b- defN 23-Jun-08 15:24 aisdb_web/dist_map_bingmaps/assets/client_bg-916ba2c4.wasm
--rw-r--r--  4.6 unx      616 b- defN 23-Jun-08 15:24 aisdb_web/dist_map_bingmaps/assets/constants-870f4956.js
--rw-r--r--  4.6 unx     8224 b- defN 23-Jun-08 15:24 aisdb_web/dist_map_bingmaps/assets/index-f2c4f58e.css
--rw-r--r--  4.6 unx     1185 b- defN 23-Jun-08 15:24 aisdb_web/dist_map_bingmaps/assets/livestream-3a02edee.js
--rw-r--r--  4.6 unx     1185 b- defN 23-Jun-08 15:24 aisdb_web/dist_map_bingmaps/assets/livestream-6755c91e.js
--rw-r--r--  4.6 unx     1185 b- defN 23-Jun-08 15:24 aisdb_web/dist_map_bingmaps/assets/livestream-73586b67.js
--rw-r--r--  4.6 unx     2662 b- defN 23-Jun-08 15:24 aisdb_web/dist_map_bingmaps/assets/main-7f6e0eb2.js
--rw-r--r--  4.6 unx     2662 b- defN 23-Jun-08 15:24 aisdb_web/dist_map_bingmaps/assets/main-8b0e81cf.js
--rw-r--r--  4.6 unx     2662 b- defN 23-Jun-08 15:24 aisdb_web/dist_map_bingmaps/assets/main-feaa3a7b.js
--rw-r--r--  4.6 unx   405469 b- defN 23-Jun-08 15:24 aisdb_web/dist_map_bingmaps/assets/map-64a6868c.js
--rw-r--r--  4.6 unx   405469 b- defN 23-Jun-08 15:24 aisdb_web/dist_map_bingmaps/assets/map-967b67d1.js
--rw-r--r--  4.6 unx    15782 b- defN 23-Jun-08 15:24 aisdb_web/dist_map_bingmaps/assets/map-c04ede37.css
--rw-r--r--  4.6 unx   405469 b- defN 23-Jun-08 15:24 aisdb_web/dist_map_bingmaps/assets/map-c0ca9a66.js
--rw-r--r--  4.6 unx    16622 b- defN 23-Jun-08 15:24 aisdb_web/dist_map_bingmaps/assets/proj-04f64360.js
--rw-r--r--  4.6 unx   203253 b- defN 23-Jun-08 15:24 aisdb_web/dist_map_bingmaps/assets/render-75680345.js
--rw-r--r--  4.6 unx   203253 b- defN 23-Jun-08 15:24 aisdb_web/dist_map_bingmaps/assets/render-c2851da9.js
--rw-r--r--  4.6 unx   203253 b- defN 23-Jun-08 15:24 aisdb_web/dist_map_bingmaps/assets/render-c61cd003.js
--rw-r--r--  4.6 unx    20179 b- defN 23-Jun-08 15:24 aisdb_web/dist_map_bingmaps/assets/tileserver-0d479a70.js
--rw-r--r--  4.6 unx    20179 b- defN 23-Jun-08 15:24 aisdb_web/dist_map_bingmaps/assets/tileserver-1d4ceaca.js
--rw-r--r--  4.6 unx    20179 b- defN 23-Jun-08 15:24 aisdb_web/dist_map_bingmaps/assets/tileserver-2ce22ad4.js
--rw-r--r--  4.6 unx     3114 b- defN 23-Jun-08 15:24 aisdb_web/dist_map_bingmaps/assets/url-3542f36d.js
--rw-r--r--  4.6 unx     3114 b- defN 23-Jun-08 15:24 aisdb_web/dist_map_bingmaps/assets/url-43e87897.js
--rw-r--r--  4.6 unx     3114 b- defN 23-Jun-08 15:24 aisdb_web/dist_map_bingmaps/assets/url-be1cb54a.js
--rw-r--r--  4.6 unx     1203 b- defN 23-Jun-08 15:24 aisdb_web/dist_map_bingmaps/assets/vessel_metadata-a3d1e26e.js
--rw-r--r--  4.6 unx     1203 b- defN 23-Jun-08 15:24 aisdb_web/dist_map_bingmaps/assets/vessel_metadata-b8bf0fe9.js
--rw-r--r--  4.6 unx     1203 b- defN 23-Jun-08 15:24 aisdb_web/dist_map_bingmaps/assets/vessel_metadata-df772244.js
--rw-rw-rw-  4.6 unx    26223 b- defN 23-Jun-08 15:24 aisdb_web/dist_map_bingmaps/favicon.png
--rw-rw-rw-  4.6 unx    21560 b- defN 23-Jun-08 15:24 aisdb_web/dist_map_bingmaps/favicon.svg
--rw-r--r--  4.6 unx     2615 b- defN 23-Jun-08 15:24 aisdb_web/dist_map_bingmaps/index.html
--rwxr-xr-x  4.6 unx  4800368 b- defN 23-Jun-08 15:24 aisdb/aisdb.cpython-39-aarch64-linux-gnu.so
--rw-r--r--  4.6 unx    18452 b- defN 23-Jun-08 15:24 aisdb-1.6.4.dist-info/RECORD
-197 files, 11745242 bytes uncompressed, 4278023 bytes compressed:  63.6%
+Zip file size: 5051217 bytes, number of entries: 235
+-rw-r--r--  4.6 unx     4949 b- defN 23-Jul-11 20:07 aisdb-1.6.5.dist-info/METADATA
+-rw-r--r--  4.6 unx      102 b- defN 23-Jul-11 20:07 aisdb-1.6.5.dist-info/WHEEL
+-rw-r--r--  4.6 unx     9816 b- defN 23-Jul-11 20:07 aisdb/database/decoder.py
+-rw-r--r--  4.6 unx     1739 b- defN 23-Jul-11 20:07 aisdb/database/sqlfcn_callbacks.py
+-rw-r--r--  4.6 unx        1 b- defN 23-Jul-11 20:07 aisdb/database/__init__.py
+-rw-r--r--  4.6 unx    11962 b- defN 23-Jul-11 20:07 aisdb/database/dbqry.py
+-rw-r--r--  4.6 unx     4900 b- defN 23-Jul-11 20:07 aisdb/database/create_tables.py
+-rw-r--r--  4.6 unx     6358 b- defN 23-Jul-11 20:07 aisdb/database/dbconn.py
+-rw-r--r--  4.6 unx     3188 b- defN 23-Jul-11 20:07 aisdb/database/sqlfcn.py
+-rw-r--r--  4.6 unx     4170 b- defN 23-Jul-11 20:07 aisdb/database/sql_query_strings.py
+-rw-r--r--  4.6 unx     7650 b- defN 23-Jul-11 20:07 aisdb/track_gen.py
+-rw-r--r--  4.6 unx     2505 b- defN 23-Jul-11 20:07 aisdb/webdata/_scraper.py
+-rw-r--r--  4.6 unx        0 b- defN 23-Jul-11 20:07 aisdb/webdata/__init__.py
+-rw-r--r--  4.6 unx     2448 b- defN 23-Jul-11 20:07 aisdb/webdata/load_raster.py
+-rw-r--r--  4.6 unx    11002 b- defN 23-Jul-11 20:07 aisdb/webdata/marinetraffic.py
+-rw-r--r--  4.6 unx     5440 b- defN 23-Jul-11 20:07 aisdb/webdata/bathymetry.py
+-rw-r--r--  4.6 unx     2690 b- defN 23-Jul-11 20:07 aisdb/webdata/shore_dist.py
+-rw-r--r--  4.6 unx    18893 b- defN 23-Jul-11 20:07 aisdb/network_graph.py
+-rw-r--r--  4.6 unx    23613 b- defN 23-Jul-11 20:07 aisdb/tests/testdata/test_data_20211101.nm4.gz
+-rw-r--r--  4.6 unx    84630 b- defN 23-Jul-11 20:07 aisdb/tests/testdata/test_data_20211101.nm4
+-rw-r--r--  4.6 unx     2738 b- defN 23-Jul-11 20:07 aisdb/tests/test_01_createtables.py
+-rw-r--r--  4.6 unx     1420 b- defN 23-Jul-11 20:07 aisdb/tests/test_00_decode.py
+-rw-r--r--  4.6 unx     2803 b- defN 23-Jul-11 20:07 aisdb/tests/test_02_dbqry.py
+-rw-r--r--  4.6 unx     2580 b- defN 23-Jul-11 20:07 aisdb/tests/test_08_marinetraffic.py
+-rw-r--r--  4.6 unx     1131 b- defN 23-Jul-11 20:07 aisdb/tests/test_07_shore_dist.py
+-rw-r--r--  4.6 unx     1256 b- defN 23-Jul-11 20:07 aisdb/tests/test_07_bathymetry.py
+-rw-r--r--  4.6 unx        0 b- defN 23-Jul-11 20:07 aisdb/tests/__init__.py
+-rw-r--r--  4.6 unx     1679 b- defN 23-Jul-11 20:07 aisdb/tests/test_08_wsa.py
+-rw-r--r--  4.6 unx     2332 b- defN 23-Jul-11 20:07 aisdb/tests/test_04_trackgen.py
+-rw-r--r--  4.6 unx     1090 b- defN 23-Jul-11 20:07 aisdb/tests/test_06_interp.py
+-rw-r--r--  4.6 unx     4385 b- defN 23-Jul-11 20:07 aisdb/tests/test_05_proc_util.py
+-rw-r--r--  4.6 unx     2956 b- defN 23-Jul-11 20:07 aisdb/tests/test_03_gis.py
+-rw-r--r--  4.6 unx      778 b- defN 23-Jul-11 20:07 aisdb/tests/test_11_postgres.py
+-rw-r--r--  4.6 unx     3139 b- defN 23-Jul-11 20:07 aisdb/tests/create_testing_data.py
+-rw-r--r--  4.6 unx     3596 b- defN 23-Jul-11 20:07 aisdb/tests/test_09_network_graph.py
+-rw-r--r--  4.6 unx       74 b- defN 23-Jul-11 20:07 aisdb/tests/test_rx.py
+-rw-r--r--  4.6 unx     2956 b- defN 23-Jul-11 20:07 aisdb/tests/test_02_sqlfcn.py
+-rw-r--r--  4.6 unx     2470 b- defN 23-Jul-11 20:07 aisdb/receiver.py
+-rw-r--r--  4.6 unx     1605 b- defN 23-Jul-11 20:07 aisdb/__init__.py
+-rw-r--r--  4.6 unx     7783 b- defN 23-Jul-11 20:07 aisdb/denoising_encoder.py
+-rw-r--r--  4.6 unx      369 b- defN 23-Jul-11 20:07 aisdb/aisdb_sql/createtable_webdata_marinetraffic.sql
+-rw-r--r--  4.6 unx      258 b- defN 23-Jul-11 20:07 aisdb/aisdb_sql/createtable_static_aggregate.sql
+-rw-r--r--  4.6 unx      763 b- defN 23-Jul-11 20:07 aisdb/aisdb_sql/insert_webdata_marinetraffic.sql
+-rw-r--r--  4.6 unx      125 b- defN 23-Jul-11 20:07 aisdb/aisdb_sql/cte_dynamic_clusteredidx.sql
+-rw-r--r--  4.6 unx      108 b- defN 23-Jul-11 20:07 aisdb/aisdb_sql/createtable_griddata.sql
+-rw-r--r--  4.6 unx     4924 b- defN 23-Jul-11 20:07 aisdb/aisdb_sql/coarsetype.sql
+-rw-r--r--  4.6 unx      881 b- defN 23-Jul-11 20:07 aisdb/aisdb_sql/select_merged_all.sql
+-rw-r--r--  4.6 unx       91 b- defN 23-Jul-11 20:07 aisdb/aisdb_sql/cte_coarsetype.sql
+-rw-r--r--  4.6 unx      185 b- defN 23-Jul-11 20:07 aisdb/aisdb_sql/cte_static.sql
+-rw-r--r--  4.6 unx      539 b- defN 23-Jul-11 20:07 aisdb/aisdb_sql/createtable_static.sql
+-rw-r--r--  4.6 unx      210 b- defN 23-Jul-11 20:07 aisdb/aisdb_sql/cte_static_aggregate.sql
+-rw-r--r--  4.6 unx      493 b- defN 23-Jul-11 20:07 aisdb/aisdb_sql/select_join_dynamic_static_clusteredidx.sql
+-rw-r--r--  4.6 unx      400 b- defN 23-Jul-11 20:07 aisdb/aisdb_sql/insert_static.sql
+-rw-r--r--  4.6 unx      658 b- defN 23-Jul-11 20:07 aisdb/aisdb_sql/select_static_join_webdata.sql
+-rw-r--r--  4.6 unx      312 b- defN 23-Jul-11 20:07 aisdb/aisdb_sql/select_columns_static.sql
+-rw-r--r--  4.6 unx      230 b- defN 23-Jul-11 20:07 aisdb/aisdb_sql/insert_dynamic_clusteredidx.sql
+-rw-r--r--  4.6 unx      358 b- defN 23-Jul-11 20:07 aisdb/aisdb_sql/createtable_dynamic_clustered.sql
+-rw-r--r--  4.6 unx       43 b- defN 23-Jul-11 20:07 aisdb/aisdb_sql/cte_aliases.sql
+-rw-r--r--  4.6 unx     8060 b- defN 23-Jul-11 20:07 aisdb/proc_util.py
+-rw-r--r--  4.6 unx     7421 b- defN 23-Jul-11 20:07 aisdb/web_interface.py
+-rw-r--r--  4.6 unx     1599 b- defN 23-Jul-11 20:07 aisdb/interp.py
+-rw-r--r--  4.6 unx    18568 b- defN 23-Jul-11 20:07 aisdb/gis.py
+-rw-r--r--  4.6 unx     3845 b- defN 23-Jul-11 20:07 aisdb/wsa.py
+-rw-r--r--  4.6 unx     1605 b- defN 23-Jul-11 20:07 aisdb/__init__.py
+-rw-r--r--  4.6 unx     7783 b- defN 23-Jul-11 20:07 aisdb/denoising_encoder.py
+-rw-r--r--  4.6 unx    18568 b- defN 23-Jul-11 20:07 aisdb/gis.py
+-rw-r--r--  4.6 unx     1599 b- defN 23-Jul-11 20:07 aisdb/interp.py
+-rw-r--r--  4.6 unx    18893 b- defN 23-Jul-11 20:07 aisdb/network_graph.py
+-rw-r--r--  4.6 unx     8060 b- defN 23-Jul-11 20:07 aisdb/proc_util.py
+-rw-r--r--  4.6 unx     2470 b- defN 23-Jul-11 20:07 aisdb/receiver.py
+-rw-r--r--  4.6 unx     7650 b- defN 23-Jul-11 20:07 aisdb/track_gen.py
+-rw-r--r--  4.6 unx     7421 b- defN 23-Jul-11 20:07 aisdb/web_interface.py
+-rw-r--r--  4.6 unx     3845 b- defN 23-Jul-11 20:07 aisdb/wsa.py
+-rw-r--r--  4.6 unx     4924 b- defN 23-Jul-11 20:07 aisdb/aisdb_sql/coarsetype.sql
+-rw-r--r--  4.6 unx      358 b- defN 23-Jul-11 20:07 aisdb/aisdb_sql/createtable_dynamic_clustered.sql
+-rw-r--r--  4.6 unx      108 b- defN 23-Jul-11 20:07 aisdb/aisdb_sql/createtable_griddata.sql
+-rw-r--r--  4.6 unx      539 b- defN 23-Jul-11 20:07 aisdb/aisdb_sql/createtable_static.sql
+-rw-r--r--  4.6 unx      258 b- defN 23-Jul-11 20:07 aisdb/aisdb_sql/createtable_static_aggregate.sql
+-rw-r--r--  4.6 unx      369 b- defN 23-Jul-11 20:07 aisdb/aisdb_sql/createtable_webdata_marinetraffic.sql
+-rw-r--r--  4.6 unx       43 b- defN 23-Jul-11 20:07 aisdb/aisdb_sql/cte_aliases.sql
+-rw-r--r--  4.6 unx       91 b- defN 23-Jul-11 20:07 aisdb/aisdb_sql/cte_coarsetype.sql
+-rw-r--r--  4.6 unx      125 b- defN 23-Jul-11 20:07 aisdb/aisdb_sql/cte_dynamic_clusteredidx.sql
+-rw-r--r--  4.6 unx      185 b- defN 23-Jul-11 20:07 aisdb/aisdb_sql/cte_static.sql
+-rw-r--r--  4.6 unx      210 b- defN 23-Jul-11 20:07 aisdb/aisdb_sql/cte_static_aggregate.sql
+-rw-r--r--  4.6 unx      230 b- defN 23-Jul-11 20:07 aisdb/aisdb_sql/insert_dynamic_clusteredidx.sql
+-rw-r--r--  4.6 unx      400 b- defN 23-Jul-11 20:07 aisdb/aisdb_sql/insert_static.sql
+-rw-r--r--  4.6 unx      763 b- defN 23-Jul-11 20:07 aisdb/aisdb_sql/insert_webdata_marinetraffic.sql
+-rw-r--r--  4.6 unx      312 b- defN 23-Jul-11 20:07 aisdb/aisdb_sql/select_columns_static.sql
+-rw-r--r--  4.6 unx      493 b- defN 23-Jul-11 20:07 aisdb/aisdb_sql/select_join_dynamic_static_clusteredidx.sql
+-rw-r--r--  4.6 unx      881 b- defN 23-Jul-11 20:07 aisdb/aisdb_sql/select_merged_all.sql
+-rw-r--r--  4.6 unx      658 b- defN 23-Jul-11 20:07 aisdb/aisdb_sql/select_static_join_webdata.sql
+-rw-r--r--  4.6 unx        1 b- defN 23-Jul-11 20:07 aisdb/database/__init__.py
+-rw-r--r--  4.6 unx     4900 b- defN 23-Jul-11 20:07 aisdb/database/create_tables.py
+-rw-r--r--  4.6 unx     6358 b- defN 23-Jul-11 20:07 aisdb/database/dbconn.py
+-rw-r--r--  4.6 unx    11962 b- defN 23-Jul-11 20:07 aisdb/database/dbqry.py
+-rw-r--r--  4.6 unx     9816 b- defN 23-Jul-11 20:07 aisdb/database/decoder.py
+-rw-r--r--  4.6 unx     4170 b- defN 23-Jul-11 20:07 aisdb/database/sql_query_strings.py
+-rw-r--r--  4.6 unx     3188 b- defN 23-Jul-11 20:07 aisdb/database/sqlfcn.py
+-rw-r--r--  4.6 unx     1739 b- defN 23-Jul-11 20:07 aisdb/database/sqlfcn_callbacks.py
+-rw-r--r--  4.6 unx        0 b- defN 23-Jul-11 20:07 aisdb/tests/__init__.py
+-rw-r--r--  4.6 unx     3139 b- defN 23-Jul-11 20:07 aisdb/tests/create_testing_data.py
+-rw-r--r--  4.6 unx     1420 b- defN 23-Jul-11 20:07 aisdb/tests/test_00_decode.py
+-rw-r--r--  4.6 unx     2738 b- defN 23-Jul-11 20:07 aisdb/tests/test_01_createtables.py
+-rw-r--r--  4.6 unx     2803 b- defN 23-Jul-11 20:07 aisdb/tests/test_02_dbqry.py
+-rw-r--r--  4.6 unx     2956 b- defN 23-Jul-11 20:07 aisdb/tests/test_02_sqlfcn.py
+-rw-r--r--  4.6 unx     2956 b- defN 23-Jul-11 20:07 aisdb/tests/test_03_gis.py
+-rw-r--r--  4.6 unx     2332 b- defN 23-Jul-11 20:07 aisdb/tests/test_04_trackgen.py
+-rw-r--r--  4.6 unx     4385 b- defN 23-Jul-11 20:07 aisdb/tests/test_05_proc_util.py
+-rw-r--r--  4.6 unx     1090 b- defN 23-Jul-11 20:07 aisdb/tests/test_06_interp.py
+-rw-r--r--  4.6 unx     1256 b- defN 23-Jul-11 20:07 aisdb/tests/test_07_bathymetry.py
+-rw-r--r--  4.6 unx     1131 b- defN 23-Jul-11 20:07 aisdb/tests/test_07_shore_dist.py
+-rw-r--r--  4.6 unx     2580 b- defN 23-Jul-11 20:07 aisdb/tests/test_08_marinetraffic.py
+-rw-r--r--  4.6 unx     1679 b- defN 23-Jul-11 20:07 aisdb/tests/test_08_wsa.py
+-rw-r--r--  4.6 unx     3596 b- defN 23-Jul-11 20:07 aisdb/tests/test_09_network_graph.py
+-rw-r--r--  4.6 unx      778 b- defN 23-Jul-11 20:07 aisdb/tests/test_11_postgres.py
+-rw-r--r--  4.6 unx       74 b- defN 23-Jul-11 20:07 aisdb/tests/test_rx.py
+-rw-r--r--  4.6 unx  1258678 b- defN 23-Jul-11 20:07 aisdb/tests/testdata/test_data_20210701.csv
+-rwxr-xr-x  4.6 unx    84630 b- defN 23-Jul-11 20:07 aisdb/tests/testdata/test_data_20211101.nm4
+-rw-r--r--  4.6 unx        0 b- defN 23-Jul-11 20:07 aisdb/webdata/__init__.py
+-rw-r--r--  4.6 unx     2505 b- defN 23-Jul-11 20:07 aisdb/webdata/_scraper.py
+-rw-r--r--  4.6 unx     5440 b- defN 23-Jul-11 20:07 aisdb/webdata/bathymetry.py
+-rw-r--r--  4.6 unx     2448 b- defN 23-Jul-11 20:07 aisdb/webdata/load_raster.py
+-rw-r--r--  4.6 unx    11002 b- defN 23-Jul-11 20:07 aisdb/webdata/marinetraffic.py
+-rw-r--r--  4.6 unx     2690 b- defN 23-Jul-11 20:07 aisdb/webdata/shore_dist.py
+-rw-r--r--  4.6 unx    32701 b- defN 23-Jul-11 20:07 aisdb_lib/Cargo.lock
+-rw-r--r--  4.6 unx      946 b- defN 23-Jul-11 20:07 aisdb_lib/Cargo.toml
+-rw-r--r--  4.6 unx      135 b- defN 23-Jul-11 20:07 aisdb_lib/build.rs
+-rw-r--r--  4.6 unx     1672 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/OSM-18e3061c.js
+-rw-r--r--  4.6 unx     1672 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/OSM-3d3b8c7a.js
+-rw-r--r--  4.6 unx     1672 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/OSM-a7270865.js
+-rw-r--r--  4.6 unx     1672 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/OSM-f12b1a18.js
+-rw-r--r--  4.6 unx     1672 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/OSM-fff71e55.js
+-rw-r--r--  4.6 unx    17519 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/TileImage-809400bf.js
+-rw-r--r--  4.6 unx    17519 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/TileImage-865fdc14.js
+-rw-r--r--  4.6 unx    17292 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/TileImage-b8366ddc.js
+-rw-r--r--  4.6 unx    17519 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/TileImage-e0a2bc65.js
+-rw-r--r--  4.6 unx    17519 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/TileImage-e2e53f79.js
+-rw-r--r--  4.6 unx   173279 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/client_bg-05f4a55d.wasm
+-rw-r--r--  4.6 unx   173403 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/client_bg-505558bc.wasm
+-rw-r--r--  4.6 unx   173279 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/client_bg-6a509824.wasm
+-rw-r--r--  4.6 unx   173278 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/client_bg-916ba2c4.wasm
+-rw-r--r--  4.6 unx      760 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/constants-36dce06f.js
+-rw-r--r--  4.6 unx      723 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/constants-a418eeb2.js
+-rw-r--r--  4.6 unx     8224 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/index-f2c4f58e.css
+-rw-r--r--  4.6 unx     1185 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/livestream-04f2da24.js
+-rw-r--r--  4.6 unx     1185 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/livestream-7a84f2e5.js
+-rw-r--r--  4.6 unx     1185 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/livestream-7c48cb34.js
+-rw-r--r--  4.6 unx     1185 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/livestream-86d0ab65.js
+-rw-r--r--  4.6 unx     1185 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/livestream-87738d04.js
+-rw-r--r--  4.6 unx     2662 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/main-12a41ab2.js
+-rw-r--r--  4.6 unx     2662 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/main-4986f97e.js
+-rw-r--r--  4.6 unx     2662 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/main-4e7182f2.js
+-rw-r--r--  4.6 unx     2662 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/main-b42e8f3c.js
+-rw-r--r--  4.6 unx     2662 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/main-c046974e.js
+-rw-r--r--  4.6 unx   405869 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/map-0df0429f.js
+-rw-r--r--  4.6 unx   406688 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/map-0f7724e3.js
+-rw-r--r--  4.6 unx   405998 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/map-8b360aef.js
+-rw-r--r--  4.6 unx   405869 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/map-abddb635.js
+-rw-r--r--  4.6 unx   405869 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/map-b057f40e.js
+-rw-r--r--  4.6 unx    15782 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/map-c04ede37.css
+-rw-r--r--  4.6 unx    16617 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/proj-20c50701.js
+-rw-r--r--  4.6 unx    16622 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/proj-3e4e3ac0.js
+-rw-r--r--  4.6 unx   203253 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/render-15f8910a.js
+-rw-r--r--  4.6 unx   203253 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/render-29aaa5e2.js
+-rw-r--r--  4.6 unx   203229 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/render-3e217d1c.js
+-rw-r--r--  4.6 unx   203253 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/render-9978d19f.js
+-rw-r--r--  4.6 unx   203253 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/render-9ee6ddf6.js
+-rw-r--r--  4.6 unx     3092 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/tileserver-24a57af3.js
+-rw-r--r--  4.6 unx     3092 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/tileserver-8260d47b.js
+-rw-r--r--  4.6 unx     3092 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/tileserver-b56401ad.js
+-rw-r--r--  4.6 unx     3092 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/tileserver-f7324a05.js
+-rw-r--r--  4.6 unx     3092 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/tileserver-f89aaf92.js
+-rw-r--r--  4.6 unx     3114 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/url-3f93404c.js
+-rw-r--r--  4.6 unx     3114 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/url-7cac731b.js
+-rw-r--r--  4.6 unx     3114 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/url-89988760.js
+-rw-r--r--  4.6 unx     3114 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/url-b43e4d73.js
+-rw-r--r--  4.6 unx     3114 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/url-daaf27e9.js
+-rw-r--r--  4.6 unx     1203 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/vessel_metadata-52b84ad7.js
+-rw-r--r--  4.6 unx     1203 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/vessel_metadata-a539ebc6.js
+-rw-r--r--  4.6 unx     1203 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/vessel_metadata-b3364c5a.js
+-rw-r--r--  4.6 unx     1084 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/vessel_metadata-c128d07d.js
+-rw-r--r--  4.6 unx     1203 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/assets/vessel_metadata-d682b0f2.js
+-rw-rw-rw-  4.6 unx    26223 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/favicon.png
+-rw-rw-rw-  4.6 unx    21560 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/favicon.svg
+-rw-r--r--  4.6 unx     2615 b- defN 23-Jul-11 20:07 aisdb_web/dist_map/index.html
+-rw-r--r--  4.6 unx   173279 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/client_bg-05f4a55d.wasm
+-rw-r--r--  4.6 unx   173403 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/client_bg-505558bc.wasm
+-rw-r--r--  4.6 unx   173279 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/client_bg-6a509824.wasm
+-rw-r--r--  4.6 unx   173278 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/client_bg-916ba2c4.wasm
+-rw-r--r--  4.6 unx      616 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/constants-870f4956.js
+-rw-r--r--  4.6 unx      653 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/constants-b9e7c6db.js
+-rw-r--r--  4.6 unx     8224 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/index-f2c4f58e.css
+-rw-r--r--  4.6 unx     1185 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/livestream-3a02edee.js
+-rw-r--r--  4.6 unx     1185 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/livestream-6755c91e.js
+-rw-r--r--  4.6 unx     1185 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/livestream-73586b67.js
+-rw-r--r--  4.6 unx     1185 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/livestream-e1be7db5.js
+-rw-r--r--  4.6 unx     1185 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/livestream-ffcfc7b5.js
+-rw-r--r--  4.6 unx     2662 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/main-49cea758.js
+-rw-r--r--  4.6 unx     2662 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/main-7f6e0eb2.js
+-rw-r--r--  4.6 unx     2662 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/main-8b0e81cf.js
+-rw-r--r--  4.6 unx     2662 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/main-f2134a8e.js
+-rw-r--r--  4.6 unx     2662 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/main-feaa3a7b.js
+-rw-r--r--  4.6 unx   406288 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/map-17890f38.js
+-rw-r--r--  4.6 unx   405598 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/map-54e8d9a1.js
+-rw-r--r--  4.6 unx   405469 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/map-64a6868c.js
+-rw-r--r--  4.6 unx   405469 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/map-967b67d1.js
+-rw-r--r--  4.6 unx    15782 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/map-c04ede37.css
+-rw-r--r--  4.6 unx   405469 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/map-c0ca9a66.js
+-rw-r--r--  4.6 unx    16622 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/proj-04f64360.js
+-rw-r--r--  4.6 unx    16617 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/proj-cfc8763a.js
+-rw-r--r--  4.6 unx   203253 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/render-002f1925.js
+-rw-r--r--  4.6 unx   203253 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/render-75680345.js
+-rw-r--r--  4.6 unx   203229 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/render-9dc74427.js
+-rw-r--r--  4.6 unx   203253 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/render-c2851da9.js
+-rw-r--r--  4.6 unx   203253 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/render-c61cd003.js
+-rw-r--r--  4.6 unx    20179 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/tileserver-0d479a70.js
+-rw-r--r--  4.6 unx    20179 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/tileserver-1d4ceaca.js
+-rw-r--r--  4.6 unx    20179 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/tileserver-2ce22ad4.js
+-rw-r--r--  4.6 unx    19952 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/tileserver-a213d9f6.js
+-rw-r--r--  4.6 unx    20179 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/tileserver-ce29a4c1.js
+-rw-r--r--  4.6 unx     3114 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/url-3542f36d.js
+-rw-r--r--  4.6 unx     3114 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/url-43e87897.js
+-rw-r--r--  4.6 unx     3114 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/url-447c8bef.js
+-rw-r--r--  4.6 unx     3114 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/url-be1cb54a.js
+-rw-r--r--  4.6 unx     3114 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/url-decb3532.js
+-rw-r--r--  4.6 unx     1084 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/vessel_metadata-a1e91a33.js
+-rw-r--r--  4.6 unx     1203 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/vessel_metadata-a3d1e26e.js
+-rw-r--r--  4.6 unx     1203 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/vessel_metadata-b8bf0fe9.js
+-rw-r--r--  4.6 unx     1203 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/vessel_metadata-df772244.js
+-rw-r--r--  4.6 unx     1203 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/assets/vessel_metadata-fe112f38.js
+-rw-rw-rw-  4.6 unx    26223 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/favicon.png
+-rw-rw-rw-  4.6 unx    21560 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/favicon.svg
+-rw-r--r--  4.6 unx     2615 b- defN 23-Jul-11 20:07 aisdb_web/dist_map_bingmaps/index.html
+-rwxr-xr-x  4.6 unx  4624391 b- defN 23-Jul-11 20:07 aisdb/aisdb.cpython-39-darwin.so
+-rw-r--r--  4.6 unx    22504 b- defN 23-Jul-11 20:07 aisdb-1.6.5.dist-info/RECORD
+235 files, 14506067 bytes uncompressed, 5015059 bytes compressed:  65.4%
```

## zipnote {}

```diff
@@ -1,191 +1,191 @@
-Filename: aisdb-1.6.4.dist-info/METADATA
+Filename: aisdb-1.6.5.dist-info/METADATA
 Comment: 
 
-Filename: aisdb-1.6.4.dist-info/WHEEL
+Filename: aisdb-1.6.5.dist-info/WHEEL
 Comment: 
 
-Filename: aisdb/__init__.py
+Filename: aisdb/database/decoder.py
 Comment: 
 
-Filename: aisdb/aisdb_sql/coarsetype.sql
+Filename: aisdb/database/sqlfcn_callbacks.py
 Comment: 
 
-Filename: aisdb/aisdb_sql/createtable_dynamic_clustered.sql
+Filename: aisdb/database/__init__.py
 Comment: 
 
-Filename: aisdb/aisdb_sql/createtable_griddata.sql
+Filename: aisdb/database/dbqry.py
 Comment: 
 
-Filename: aisdb/aisdb_sql/createtable_static.sql
+Filename: aisdb/database/create_tables.py
 Comment: 
 
-Filename: aisdb/aisdb_sql/createtable_static_aggregate.sql
+Filename: aisdb/database/dbconn.py
 Comment: 
 
-Filename: aisdb/aisdb_sql/createtable_webdata_marinetraffic.sql
+Filename: aisdb/database/sqlfcn.py
 Comment: 
 
-Filename: aisdb/aisdb_sql/cte_aliases.sql
+Filename: aisdb/database/sql_query_strings.py
 Comment: 
 
-Filename: aisdb/aisdb_sql/cte_coarsetype.sql
+Filename: aisdb/track_gen.py
 Comment: 
 
-Filename: aisdb/aisdb_sql/cte_dynamic_clusteredidx.sql
+Filename: aisdb/webdata/_scraper.py
 Comment: 
 
-Filename: aisdb/aisdb_sql/cte_static.sql
+Filename: aisdb/webdata/__init__.py
 Comment: 
 
-Filename: aisdb/aisdb_sql/cte_static_aggregate.sql
+Filename: aisdb/webdata/load_raster.py
 Comment: 
 
-Filename: aisdb/aisdb_sql/insert_dynamic_clusteredidx.sql
+Filename: aisdb/webdata/marinetraffic.py
 Comment: 
 
-Filename: aisdb/aisdb_sql/insert_static.sql
+Filename: aisdb/webdata/bathymetry.py
 Comment: 
 
-Filename: aisdb/aisdb_sql/insert_webdata_marinetraffic.sql
+Filename: aisdb/webdata/shore_dist.py
 Comment: 
 
-Filename: aisdb/aisdb_sql/select_columns_static.sql
+Filename: aisdb/network_graph.py
 Comment: 
 
-Filename: aisdb/aisdb_sql/select_join_dynamic_static_clusteredidx.sql
+Filename: aisdb/tests/testdata/test_data_20211101.nm4.gz
 Comment: 
 
-Filename: aisdb/aisdb_sql/select_merged_all.sql
+Filename: aisdb/tests/testdata/test_data_20211101.nm4
 Comment: 
 
-Filename: aisdb/aisdb_sql/select_static_join_webdata.sql
+Filename: aisdb/tests/test_01_createtables.py
 Comment: 
 
-Filename: aisdb/database/__init__.py
+Filename: aisdb/tests/test_00_decode.py
 Comment: 
 
-Filename: aisdb/database/create_tables.py
+Filename: aisdb/tests/test_02_dbqry.py
 Comment: 
 
-Filename: aisdb/database/dbconn.py
+Filename: aisdb/tests/test_08_marinetraffic.py
 Comment: 
 
-Filename: aisdb/database/dbqry.py
+Filename: aisdb/tests/test_07_shore_dist.py
 Comment: 
 
-Filename: aisdb/database/decoder.py
+Filename: aisdb/tests/test_07_bathymetry.py
 Comment: 
 
-Filename: aisdb/database/sql_query_strings.py
+Filename: aisdb/tests/__init__.py
 Comment: 
 
-Filename: aisdb/database/sqlfcn.py
+Filename: aisdb/tests/test_08_wsa.py
 Comment: 
 
-Filename: aisdb/database/sqlfcn_callbacks.py
+Filename: aisdb/tests/test_04_trackgen.py
 Comment: 
 
-Filename: aisdb/denoising_encoder.py
+Filename: aisdb/tests/test_06_interp.py
 Comment: 
 
-Filename: aisdb/gis.py
+Filename: aisdb/tests/test_05_proc_util.py
 Comment: 
 
-Filename: aisdb/interp.py
+Filename: aisdb/tests/test_03_gis.py
 Comment: 
 
-Filename: aisdb/network_graph.py
+Filename: aisdb/tests/test_11_postgres.py
 Comment: 
 
-Filename: aisdb/proc_util.py
+Filename: aisdb/tests/create_testing_data.py
 Comment: 
 
-Filename: aisdb/receiver.py
+Filename: aisdb/tests/test_09_network_graph.py
 Comment: 
 
-Filename: aisdb/tests/__init__.py
+Filename: aisdb/tests/test_rx.py
 Comment: 
 
-Filename: aisdb/tests/create_testing_data.py
+Filename: aisdb/tests/test_02_sqlfcn.py
 Comment: 
 
-Filename: aisdb/tests/test_00_decode.py
+Filename: aisdb/receiver.py
 Comment: 
 
-Filename: aisdb/tests/test_01_createtables.py
+Filename: aisdb/__init__.py
 Comment: 
 
-Filename: aisdb/tests/test_02_dbqry.py
+Filename: aisdb/denoising_encoder.py
 Comment: 
 
-Filename: aisdb/tests/test_02_sqlfcn.py
+Filename: aisdb/aisdb_sql/createtable_webdata_marinetraffic.sql
 Comment: 
 
-Filename: aisdb/tests/test_03_gis.py
+Filename: aisdb/aisdb_sql/createtable_static_aggregate.sql
 Comment: 
 
-Filename: aisdb/tests/test_04_trackgen.py
+Filename: aisdb/aisdb_sql/insert_webdata_marinetraffic.sql
 Comment: 
 
-Filename: aisdb/tests/test_05_proc_util.py
+Filename: aisdb/aisdb_sql/cte_dynamic_clusteredidx.sql
 Comment: 
 
-Filename: aisdb/tests/test_06_interp.py
+Filename: aisdb/aisdb_sql/createtable_griddata.sql
 Comment: 
 
-Filename: aisdb/tests/test_07_bathymetry.py
+Filename: aisdb/aisdb_sql/coarsetype.sql
 Comment: 
 
-Filename: aisdb/tests/test_07_shore_dist.py
+Filename: aisdb/aisdb_sql/select_merged_all.sql
 Comment: 
 
-Filename: aisdb/tests/test_08_marinetraffic.py
+Filename: aisdb/aisdb_sql/cte_coarsetype.sql
 Comment: 
 
-Filename: aisdb/tests/test_08_wsa.py
+Filename: aisdb/aisdb_sql/cte_static.sql
 Comment: 
 
-Filename: aisdb/tests/test_09_network_graph.py
+Filename: aisdb/aisdb_sql/createtable_static.sql
 Comment: 
 
-Filename: aisdb/tests/test_11_postgres.py
+Filename: aisdb/aisdb_sql/cte_static_aggregate.sql
 Comment: 
 
-Filename: aisdb/tests/test_rx.py
+Filename: aisdb/aisdb_sql/select_join_dynamic_static_clusteredidx.sql
 Comment: 
 
-Filename: aisdb/tests/testdata/test_data_20211101.nm4
+Filename: aisdb/aisdb_sql/insert_static.sql
 Comment: 
 
-Filename: aisdb/tests/testdata/test_data_20211101.nm4.gz
+Filename: aisdb/aisdb_sql/select_static_join_webdata.sql
 Comment: 
 
-Filename: aisdb/track_gen.py
+Filename: aisdb/aisdb_sql/select_columns_static.sql
 Comment: 
 
-Filename: aisdb/web_interface.py
+Filename: aisdb/aisdb_sql/insert_dynamic_clusteredidx.sql
 Comment: 
 
-Filename: aisdb/webdata/__init__.py
+Filename: aisdb/aisdb_sql/createtable_dynamic_clustered.sql
 Comment: 
 
-Filename: aisdb/webdata/_scraper.py
+Filename: aisdb/aisdb_sql/cte_aliases.sql
 Comment: 
 
-Filename: aisdb/webdata/bathymetry.py
+Filename: aisdb/proc_util.py
 Comment: 
 
-Filename: aisdb/webdata/load_raster.py
+Filename: aisdb/web_interface.py
 Comment: 
 
-Filename: aisdb/webdata/marinetraffic.py
+Filename: aisdb/interp.py
 Comment: 
 
-Filename: aisdb/webdata/shore_dist.py
+Filename: aisdb/gis.py
 Comment: 
 
 Filename: aisdb/wsa.py
 Comment: 
 
 Filename: aisdb/__init__.py
 Comment: 
@@ -384,32 +384,50 @@
 
 Filename: aisdb_web/dist_map/assets/OSM-3d3b8c7a.js
 Comment: 
 
 Filename: aisdb_web/dist_map/assets/OSM-a7270865.js
 Comment: 
 
+Filename: aisdb_web/dist_map/assets/OSM-f12b1a18.js
+Comment: 
+
+Filename: aisdb_web/dist_map/assets/OSM-fff71e55.js
+Comment: 
+
+Filename: aisdb_web/dist_map/assets/TileImage-809400bf.js
+Comment: 
+
 Filename: aisdb_web/dist_map/assets/TileImage-865fdc14.js
 Comment: 
 
+Filename: aisdb_web/dist_map/assets/TileImage-b8366ddc.js
+Comment: 
+
 Filename: aisdb_web/dist_map/assets/TileImage-e0a2bc65.js
 Comment: 
 
 Filename: aisdb_web/dist_map/assets/TileImage-e2e53f79.js
 Comment: 
 
 Filename: aisdb_web/dist_map/assets/client_bg-05f4a55d.wasm
 Comment: 
 
+Filename: aisdb_web/dist_map/assets/client_bg-505558bc.wasm
+Comment: 
+
 Filename: aisdb_web/dist_map/assets/client_bg-6a509824.wasm
 Comment: 
 
 Filename: aisdb_web/dist_map/assets/client_bg-916ba2c4.wasm
 Comment: 
 
+Filename: aisdb_web/dist_map/assets/constants-36dce06f.js
+Comment: 
+
 Filename: aisdb_web/dist_map/assets/constants-a418eeb2.js
 Comment: 
 
 Filename: aisdb_web/dist_map/assets/index-f2c4f58e.css
 Comment: 
 
 Filename: aisdb_web/dist_map/assets/livestream-04f2da24.js
@@ -417,71 +435,116 @@
 
 Filename: aisdb_web/dist_map/assets/livestream-7a84f2e5.js
 Comment: 
 
 Filename: aisdb_web/dist_map/assets/livestream-7c48cb34.js
 Comment: 
 
+Filename: aisdb_web/dist_map/assets/livestream-86d0ab65.js
+Comment: 
+
+Filename: aisdb_web/dist_map/assets/livestream-87738d04.js
+Comment: 
+
 Filename: aisdb_web/dist_map/assets/main-12a41ab2.js
 Comment: 
 
+Filename: aisdb_web/dist_map/assets/main-4986f97e.js
+Comment: 
+
+Filename: aisdb_web/dist_map/assets/main-4e7182f2.js
+Comment: 
+
 Filename: aisdb_web/dist_map/assets/main-b42e8f3c.js
 Comment: 
 
 Filename: aisdb_web/dist_map/assets/main-c046974e.js
 Comment: 
 
 Filename: aisdb_web/dist_map/assets/map-0df0429f.js
 Comment: 
 
+Filename: aisdb_web/dist_map/assets/map-0f7724e3.js
+Comment: 
+
+Filename: aisdb_web/dist_map/assets/map-8b360aef.js
+Comment: 
+
 Filename: aisdb_web/dist_map/assets/map-abddb635.js
 Comment: 
 
 Filename: aisdb_web/dist_map/assets/map-b057f40e.js
 Comment: 
 
 Filename: aisdb_web/dist_map/assets/map-c04ede37.css
 Comment: 
 
+Filename: aisdb_web/dist_map/assets/proj-20c50701.js
+Comment: 
+
 Filename: aisdb_web/dist_map/assets/proj-3e4e3ac0.js
 Comment: 
 
 Filename: aisdb_web/dist_map/assets/render-15f8910a.js
 Comment: 
 
 Filename: aisdb_web/dist_map/assets/render-29aaa5e2.js
 Comment: 
 
+Filename: aisdb_web/dist_map/assets/render-3e217d1c.js
+Comment: 
+
 Filename: aisdb_web/dist_map/assets/render-9978d19f.js
 Comment: 
 
+Filename: aisdb_web/dist_map/assets/render-9ee6ddf6.js
+Comment: 
+
 Filename: aisdb_web/dist_map/assets/tileserver-24a57af3.js
 Comment: 
 
 Filename: aisdb_web/dist_map/assets/tileserver-8260d47b.js
 Comment: 
 
 Filename: aisdb_web/dist_map/assets/tileserver-b56401ad.js
 Comment: 
 
+Filename: aisdb_web/dist_map/assets/tileserver-f7324a05.js
+Comment: 
+
+Filename: aisdb_web/dist_map/assets/tileserver-f89aaf92.js
+Comment: 
+
 Filename: aisdb_web/dist_map/assets/url-3f93404c.js
 Comment: 
 
 Filename: aisdb_web/dist_map/assets/url-7cac731b.js
 Comment: 
 
+Filename: aisdb_web/dist_map/assets/url-89988760.js
+Comment: 
+
 Filename: aisdb_web/dist_map/assets/url-b43e4d73.js
 Comment: 
 
+Filename: aisdb_web/dist_map/assets/url-daaf27e9.js
+Comment: 
+
 Filename: aisdb_web/dist_map/assets/vessel_metadata-52b84ad7.js
 Comment: 
 
 Filename: aisdb_web/dist_map/assets/vessel_metadata-a539ebc6.js
 Comment: 
 
+Filename: aisdb_web/dist_map/assets/vessel_metadata-b3364c5a.js
+Comment: 
+
+Filename: aisdb_web/dist_map/assets/vessel_metadata-c128d07d.js
+Comment: 
+
 Filename: aisdb_web/dist_map/assets/vessel_metadata-d682b0f2.js
 Comment: 
 
 Filename: aisdb_web/dist_map/favicon.png
 Comment: 
 
 Filename: aisdb_web/dist_map/favicon.svg
@@ -489,44 +552,68 @@
 
 Filename: aisdb_web/dist_map/index.html
 Comment: 
 
 Filename: aisdb_web/dist_map_bingmaps/assets/client_bg-05f4a55d.wasm
 Comment: 
 
+Filename: aisdb_web/dist_map_bingmaps/assets/client_bg-505558bc.wasm
+Comment: 
+
 Filename: aisdb_web/dist_map_bingmaps/assets/client_bg-6a509824.wasm
 Comment: 
 
 Filename: aisdb_web/dist_map_bingmaps/assets/client_bg-916ba2c4.wasm
 Comment: 
 
 Filename: aisdb_web/dist_map_bingmaps/assets/constants-870f4956.js
 Comment: 
 
+Filename: aisdb_web/dist_map_bingmaps/assets/constants-b9e7c6db.js
+Comment: 
+
 Filename: aisdb_web/dist_map_bingmaps/assets/index-f2c4f58e.css
 Comment: 
 
 Filename: aisdb_web/dist_map_bingmaps/assets/livestream-3a02edee.js
 Comment: 
 
 Filename: aisdb_web/dist_map_bingmaps/assets/livestream-6755c91e.js
 Comment: 
 
 Filename: aisdb_web/dist_map_bingmaps/assets/livestream-73586b67.js
 Comment: 
 
+Filename: aisdb_web/dist_map_bingmaps/assets/livestream-e1be7db5.js
+Comment: 
+
+Filename: aisdb_web/dist_map_bingmaps/assets/livestream-ffcfc7b5.js
+Comment: 
+
+Filename: aisdb_web/dist_map_bingmaps/assets/main-49cea758.js
+Comment: 
+
 Filename: aisdb_web/dist_map_bingmaps/assets/main-7f6e0eb2.js
 Comment: 
 
 Filename: aisdb_web/dist_map_bingmaps/assets/main-8b0e81cf.js
 Comment: 
 
+Filename: aisdb_web/dist_map_bingmaps/assets/main-f2134a8e.js
+Comment: 
+
 Filename: aisdb_web/dist_map_bingmaps/assets/main-feaa3a7b.js
 Comment: 
 
+Filename: aisdb_web/dist_map_bingmaps/assets/map-17890f38.js
+Comment: 
+
+Filename: aisdb_web/dist_map_bingmaps/assets/map-54e8d9a1.js
+Comment: 
+
 Filename: aisdb_web/dist_map_bingmaps/assets/map-64a6868c.js
 Comment: 
 
 Filename: aisdb_web/dist_map_bingmaps/assets/map-967b67d1.js
 Comment: 
 
 Filename: aisdb_web/dist_map_bingmaps/assets/map-c04ede37.css
@@ -534,17 +621,26 @@
 
 Filename: aisdb_web/dist_map_bingmaps/assets/map-c0ca9a66.js
 Comment: 
 
 Filename: aisdb_web/dist_map_bingmaps/assets/proj-04f64360.js
 Comment: 
 
+Filename: aisdb_web/dist_map_bingmaps/assets/proj-cfc8763a.js
+Comment: 
+
+Filename: aisdb_web/dist_map_bingmaps/assets/render-002f1925.js
+Comment: 
+
 Filename: aisdb_web/dist_map_bingmaps/assets/render-75680345.js
 Comment: 
 
+Filename: aisdb_web/dist_map_bingmaps/assets/render-9dc74427.js
+Comment: 
+
 Filename: aisdb_web/dist_map_bingmaps/assets/render-c2851da9.js
 Comment: 
 
 Filename: aisdb_web/dist_map_bingmaps/assets/render-c61cd003.js
 Comment: 
 
 Filename: aisdb_web/dist_map_bingmaps/assets/tileserver-0d479a70.js
@@ -552,41 +648,59 @@
 
 Filename: aisdb_web/dist_map_bingmaps/assets/tileserver-1d4ceaca.js
 Comment: 
 
 Filename: aisdb_web/dist_map_bingmaps/assets/tileserver-2ce22ad4.js
 Comment: 
 
+Filename: aisdb_web/dist_map_bingmaps/assets/tileserver-a213d9f6.js
+Comment: 
+
+Filename: aisdb_web/dist_map_bingmaps/assets/tileserver-ce29a4c1.js
+Comment: 
+
 Filename: aisdb_web/dist_map_bingmaps/assets/url-3542f36d.js
 Comment: 
 
 Filename: aisdb_web/dist_map_bingmaps/assets/url-43e87897.js
 Comment: 
 
+Filename: aisdb_web/dist_map_bingmaps/assets/url-447c8bef.js
+Comment: 
+
 Filename: aisdb_web/dist_map_bingmaps/assets/url-be1cb54a.js
 Comment: 
 
+Filename: aisdb_web/dist_map_bingmaps/assets/url-decb3532.js
+Comment: 
+
+Filename: aisdb_web/dist_map_bingmaps/assets/vessel_metadata-a1e91a33.js
+Comment: 
+
 Filename: aisdb_web/dist_map_bingmaps/assets/vessel_metadata-a3d1e26e.js
 Comment: 
 
 Filename: aisdb_web/dist_map_bingmaps/assets/vessel_metadata-b8bf0fe9.js
 Comment: 
 
 Filename: aisdb_web/dist_map_bingmaps/assets/vessel_metadata-df772244.js
 Comment: 
 
+Filename: aisdb_web/dist_map_bingmaps/assets/vessel_metadata-fe112f38.js
+Comment: 
+
 Filename: aisdb_web/dist_map_bingmaps/favicon.png
 Comment: 
 
 Filename: aisdb_web/dist_map_bingmaps/favicon.svg
 Comment: 
 
 Filename: aisdb_web/dist_map_bingmaps/index.html
 Comment: 
 
-Filename: aisdb/aisdb.cpython-39-aarch64-linux-gnu.so
+Filename: aisdb/aisdb.cpython-39-darwin.so
 Comment: 
 
-Filename: aisdb-1.6.4.dist-info/RECORD
+Filename: aisdb-1.6.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aisdb/web_interface.py

```diff
@@ -84,14 +84,18 @@
         },
         't': track['time'],
         'x': track['lon'],
         'y': track['lat'],
     }
 
     meta = {k: track[k] for k in track['static'] if k != 'marinetraffic_info'}
+
+    if 'color' in track.keys():
+        meta['color'] = track['color']
+
     meta['msgtype'] = 'vesselinfo'
 
     if 'marinetraffic_info' in track.keys():
         meta.update({
             k: track['marinetraffic_info'][k]
             for k in track['marinetraffic_info'].keys()
         })
@@ -187,14 +191,24 @@
         from domain zone geometries.
 
         If visualearth is True, microsoft visual earth map tiles will be used
         for the map background.
 
         If open_browser is True, python will attempt to open the web application
         in a new tab using the default browser.
+
+        To customize the color of each vessel track, set the 'color' value to
+        a color string or RGB value string:
+
+        >>> def color_tracks(tracks):
+        ...     for track in tracks:
+        ...         track['color'] = 'red' or 'rgb(255,0,0)'
+        ...         yield track
+        ...
+        ... tracks_colored = color_tracks(tracks)
     '''
     proc = multiprocessing.Process(target=_start_webclient, args=[visualearth])
     proc.start()
     try:
         asyncio.run(_start_webserver(tracks, domain, visualearth,
                                      open_browser))
         proc.join()
```

## aisdb_lib/Cargo.lock

```diff
@@ -10,28 +10,51 @@
 dependencies = [
  "getrandom",
  "once_cell",
  "version_check",
 ]
 
 [[package]]
+name = "ahash"
+version = "0.8.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2c99f64d1e06488f620f932677e24bc6e2897582980441ae90a671415bd7ec2f"
+dependencies = [
+ "cfg-if",
+ "once_cell",
+ "version_check",
+]
+
+[[package]]
 name = "aisdb-lib"
-version = "1.5.9"
+version = "1.6.4"
 dependencies = [
  "chrono",
  "csv",
  "geo",
  "geo-types",
  "include_dir",
  "nmea-parser",
  "postgres",
  "rusqlite",
 ]
 
 [[package]]
+name = "allocator-api2"
+version = "0.2.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "56fc6cf8dc8c4158eed8649f9b8b0ea1518eb62b544fe9490d66fa0b349eafe9"
+
+[[package]]
+name = "android-tzdata"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
+
+[[package]]
 name = "android_system_properties"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
@@ -49,15 +72,15 @@
 name = "async-trait"
 version = "0.1.68"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b9ccdd8f2a161be9bd5c023df56f1b2a0bd1d83872ae53b71a84a12c9bf6e842"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.13",
+ "syn",
 ]
 
 [[package]]
 name = "atomic-polyfill"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3ff7eb3f316534d83a8a2c3d1674ace8a5a71198eba31e2e2b597833f699b28"
@@ -69,17 +92,17 @@
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "base64"
-version = "0.21.0"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a4a4ddaa51a5bc52a6948f74c06d20aaaddb71924eab79b8c97a8c556e942d6a"
+checksum = "604178f6c5c21f02dc555784810edfb88d34ac2c73b2eae109655649ee73ce3d"
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
@@ -102,17 +125,17 @@
 checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.12.0"
+version = "3.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d261e256854913907f67ed06efbc3338dfe6179796deefc1ff763fc1aee5535"
+checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
 
 [[package]]
 name = "byteorder"
 version = "1.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
 
@@ -132,48 +155,38 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.24"
+version = "0.4.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4e3c5919066adf22df73762e50cffcde3a758f2a848b113b586d1f86728b673b"
+checksum = "ec837a71355b28f6556dbd569b37b3f363091c0bd4b2e735674521b4c5fd9bc5"
 dependencies = [
+ "android-tzdata",
  "iana-time-zone",
  "js-sys",
- "num-integer",
  "num-traits",
  "time",
  "wasm-bindgen",
  "winapi",
 ]
 
 [[package]]
-name = "codespan-reporting"
-version = "0.11.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3538270d33cc669650c4b093848450d380def10c331d38c768e34cac80576e6e"
-dependencies = [
- "termcolor",
- "unicode-width",
-]
-
-[[package]]
 name = "core-foundation-sys"
 version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.6"
+version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "280a9f2d8b3a38871a3c8a46fb80db65e5e5ed97da80c4d08bf27fb63e35e181"
+checksum = "03e69e28e9f7f77debdedbaafa2866e1de9ba56df55a8bd7cfc724c25a09987c"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "critical-section"
 version = "1.1.1"
@@ -188,17 +201,17 @@
 dependencies = [
  "generic-array",
  "typenum",
 ]
 
 [[package]]
 name = "csv"
-version = "1.2.1"
+version = "1.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b015497079b9a9d69c02ad25de6c0a6edef051ea6360a327d0bd05802ef64ad"
+checksum = "626ae34994d3d8d668f4269922248239db4ae42d538b14c398b74a52208e8086"
 dependencies = [
  "csv-core",
  "itoa",
  "ryu",
  "serde",
 ]
 
@@ -208,62 +221,18 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b2466559f260f48ad25fe6317b3c8dac77b5bdb5763ac7d9d6103530663bc90"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
-name = "cxx"
-version = "1.0.94"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f61f1b6389c3fe1c316bf8a4dccc90a38208354b330925bce1f74a6c4756eb93"
-dependencies = [
- "cc",
- "cxxbridge-flags",
- "cxxbridge-macro",
- "link-cplusplus",
-]
-
-[[package]]
-name = "cxx-build"
-version = "1.0.94"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12cee708e8962df2aeb38f594aae5d827c022b6460ac71a7a3e2c3c2aae5a07b"
-dependencies = [
- "cc",
- "codespan-reporting",
- "once_cell",
- "proc-macro2",
- "quote",
- "scratch",
- "syn 2.0.13",
-]
-
-[[package]]
-name = "cxxbridge-flags"
-version = "1.0.94"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7944172ae7e4068c533afbb984114a56c46e9ccddda550499caa222902c7f7bb"
-
-[[package]]
-name = "cxxbridge-macro"
-version = "1.0.94"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2345488264226bf682893e25de0769f3360aac9957980ec49361b083ddaa5bc5"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn 2.0.13",
-]
-
-[[package]]
 name = "digest"
-version = "0.10.6"
+version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8168378f4e5023e7218c89c891c0fd8ecdb5e5e4f18cb78f38cf245dd021e76f"
+checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
 dependencies = [
  "block-buffer",
  "crypto-common",
  "subtle",
 ]
 
 [[package]]
@@ -310,15 +279,15 @@
 name = "futures-macro"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.13",
+ "syn",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
@@ -352,17 +321,17 @@
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "geo"
-version = "0.24.1"
+version = "0.25.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c7d640a4dd1d1c98b45f4653c841a8ec15f461a71b86bc30533ae64c6f20f268"
+checksum = "c07ac450e9e7d8c08e58d2723d46bd0328bb6cc1d7b18f4f37a1e15a311098b0"
 dependencies = [
  "float_next_after",
  "geo-types",
  "geographiclib-rs",
  "log",
  "num-traits",
  "robust",
@@ -388,17 +357,17 @@
 checksum = "8ea804e7bd3c6a4ca6a01edfa35231557a8a81d4d3f3e1e2b650d028c42592be"
 dependencies = [
  "lazy_static",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.9"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
+checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi 0.11.0+wasi-snapshot-preview1",
 ]
 
 [[package]]
@@ -412,24 +381,34 @@
 
 [[package]]
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 dependencies = [
- "ahash",
+ "ahash 0.7.6",
+]
+
+[[package]]
+name = "hashbrown"
+version = "0.14.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2c6201b9ff9fd90a5a3bac2e56a830d0caa509576f0e503818ee82c181b3437a"
+dependencies = [
+ "ahash 0.8.3",
+ "allocator-api2",
 ]
 
 [[package]]
 name = "hashlink"
-version = "0.8.1"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69fe1fcf8b4278d860ad0548329f892a3631fb63f82574df68275f34cdbe0ffa"
+checksum = "312f66718a2d7789ffef4f4b7b213138ed9f1eb3aa1d0d82fc99f88fb3ffd26f"
 dependencies = [
- "hashbrown",
+ "hashbrown 0.14.0",
 ]
 
 [[package]]
 name = "heapless"
 version = "0.7.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "db04bc24a18b9ea980628ecf00e6c0264f3c1426dac36c00cb49b6fbad8b0743"
@@ -448,34 +427,33 @@
 checksum = "6c49c37c09c17a53d937dfbb742eb3a961d65a994e6bcdcf37e7399d0cc8ab5e"
 dependencies = [
  "digest",
 ]
 
 [[package]]
 name = "iana-time-zone"
-version = "0.1.56"
+version = "0.1.57"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0722cd7114b7de04316e7ea5456a0bbb20e4adb46fd27a3697adb812cff0f37c"
+checksum = "2fad5b825842d2b38bd206f3e81d6957625fd7f0a361e345c30e01a0ae2dd613"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
  "iana-time-zone-haiku",
  "js-sys",
  "wasm-bindgen",
  "windows",
 ]
 
 [[package]]
 name = "iana-time-zone-haiku"
-version = "0.1.1"
+version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0703ae284fc167426161c2e3f1da3ea71d94b21bedbcc9494e92b28e334e3dca"
+checksum = "f31827a206f56af32e590ba56d5d2d085f558508192593743f16b2306495269f"
 dependencies = [
- "cxx",
- "cxx-build",
+ "cc",
 ]
 
 [[package]]
 name = "include_dir"
 version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "18762faeff7122e89e0857b02f7ce6fcc0d101d5e9ad2ad7846cc01d61b7f19e"
@@ -497,77 +475,65 @@
 name = "itoa"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
 
 [[package]]
 name = "js-sys"
-version = "0.3.61"
+version = "0.3.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "445dde2150c55e483f3d8416706b97ec8e8237c307e5b7b4b8dd15e6af2a0730"
+checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.141"
+version = "0.2.146"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3304a64d199bb964be99741b7a14d26972741915b3649639149b2479bb46f4b5"
+checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
 
 [[package]]
 name = "libm"
-version = "0.2.6"
+version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "348108ab3fba42ec82ff6e9564fc4ca0247bdccdc68dd8af9764bbc79c3c8ffb"
+checksum = "f7012b1bbb0719e1097c47611d3898568c546d597c2e74d66f6087edd5233ff4"
 
 [[package]]
 name = "libsqlite3-sys"
 version = "0.25.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "29f835d03d717946d28b1d1ed632eb6f0e24a299388ee623d0c23118d3e8a7fa"
 dependencies = [
  "cc",
  "pkg-config",
  "vcpkg",
 ]
 
 [[package]]
-name = "link-cplusplus"
-version = "1.0.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ecd207c9c713c34f95a097a5b029ac2ce6010530c7b49d7fea24d977dede04f5"
-dependencies = [
- "cc",
-]
-
-[[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.17"
+version = "0.4.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
-dependencies = [
- "cfg-if",
-]
+checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
 
 [[package]]
 name = "md-5"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6365506850d44bff6e2fbcb5176cf63650e48bd45ef2fe2665ae1570e0f4b9ca"
 dependencies = [
@@ -578,91 +544,80 @@
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
 name = "mio"
-version = "0.8.6"
+version = "0.8.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b9d9a46eff5b4ff64b45a9e316a6d1e0bc719ef429cbec4dc630684212bfdf9"
+checksum = "927a765cd3fc26206e66b296465fa9d3e5ab003e651c1b3c060e7956d96b19d2"
 dependencies = [
  "libc",
- "log",
  "wasi 0.11.0+wasi-snapshot-preview1",
  "windows-sys",
 ]
 
 [[package]]
 name = "nmea-parser"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "954fcc71bfed9cd60532365696db908fd7e0261e17fd13d15b39a66a5a860261"
 dependencies = [
  "bitvec",
  "chrono",
- "hashbrown",
+ "hashbrown 0.12.3",
  "log",
  "num-traits",
 ]
 
 [[package]]
-name = "num-integer"
-version = "0.1.45"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
-dependencies = [
- "autocfg",
- "num-traits",
-]
-
-[[package]]
 name = "num-traits"
 version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
 dependencies = [
  "autocfg",
  "libm",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.1"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.7"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys",
+ "windows-targets",
 ]
 
 [[package]]
 name = "percent-encoding"
-version = "2.2.0"
+version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "478c572c3d73181ff3c2539045f6eb99e5491218eae919370993b890cdbdd98e"
+checksum = "9b2a4787296e9989611394c33f193f676704af1686e70b8f8033ab5ba9a35a94"
 
 [[package]]
 name = "phf"
 version = "0.11.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "928c6535de93548188ef63bb7c4036bd415cd8f36ad25af44b9789b2ee72a48c"
 dependencies = [
@@ -688,17 +643,17 @@
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
 [[package]]
 name = "pkg-config"
-version = "0.3.26"
+version = "0.3.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ac9a59f73473f1b8d852421e59e64809f025994837ef743615c6d0c5b305160"
+checksum = "26072860ba924cbfa98ea39c8c19b4dd6a4a25423dbdf219c1eca91aa0cf6964"
 
 [[package]]
 name = "postgres"
 version = "0.19.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0bed5017bc2ff49649c0075d0d7a9d676933c1292480c1d137776fb205b5cd18"
 dependencies = [
@@ -743,26 +698,26 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.56"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
+checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.26"
+version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
+checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "radium"
 version = "0.7.0"
@@ -797,17 +752,17 @@
 checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "robust"
 version = "0.2.3"
@@ -857,50 +812,44 @@
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
-name = "scratch"
-version = "1.0.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1792db035ce95be60c3f8853017b3999209281c24e2ba5bc8e59bf97a0c590c1"
-
-[[package]]
 name = "semver"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
 
 [[package]]
 name = "serde"
-version = "1.0.159"
+version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c04e8343c3daeec41f58990b9d77068df31209f2af111e059e9fe9646693065"
+checksum = "9e8c8cf938e98f769bc164923b06dce91cea1751522f46f8466461af04c9027d"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.159"
+version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c614d17805b093df4b147b51339e7e44bf05ef59fba1e45d83500bcfb4d8585"
+checksum = "d9735b638ccc51c28bf6914d90a2e9725b377144fc612c49a611fddd1b631d68"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.13",
+ "syn",
 ]
 
 [[package]]
 name = "sha2"
-version = "0.10.6"
+version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "82e6b795fe2e3b1e845bafcb27aa35405c4d47cdfc92af5fc8d3002f76cebdc0"
+checksum = "479fb9d862239e610720565ca91403019f2f00410f1864c5aa7479b950a76ed8"
 dependencies = [
  "cfg-if",
  "cpufeatures",
  "digest",
 ]
 
 [[package]]
@@ -932,17 +881,17 @@
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "socket2"
-version = "0.5.1"
+version = "0.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bc8d618c6641ae355025c449427f9e96b98abf99a772be3cef6708d15c77147a"
+checksum = "2538b18701741680e0322a2302176d3253a35388e2e62f172f64f4f16605f877"
 dependencies = [
  "libc",
  "windows-sys",
 ]
 
 [[package]]
 name = "spin"
@@ -967,56 +916,36 @@
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
 name = "subtle"
-version = "2.4.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6bdef32e8150c2a081110b42772ffe7d7c9032b606bc226c8260fd97e0976601"
-
-[[package]]
-name = "syn"
-version = "1.0.109"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
-dependencies = [
- "proc-macro2",
- "quote",
- "unicode-ident",
-]
+checksum = "81cdd64d312baedb58e21336b31bc043b77e01cc99033ce76ef539f78e965ebc"
 
 [[package]]
 name = "syn"
-version = "2.0.13"
+version = "2.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c9da457c5285ac1f936ebd076af6dac17a61cfe7826f2076b4d015cf47bc8ec"
+checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "tap"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "55937e1799185b12863d447f42597ed69d9928686b8d88a1df17376a097d8369"
 
 [[package]]
-name = "termcolor"
-version = "1.2.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
-dependencies = [
- "winapi-util",
-]
-
-[[package]]
 name = "time"
 version = "0.1.45"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1b797afad3f312d1c66a56d11d0316f916356d11bd158fbc6ca6389ff6bf805a"
 dependencies = [
  "libc",
  "wasi 0.10.0+wasi-snapshot-preview1",
@@ -1036,17 +965,17 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.27.0"
+version = "1.28.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d0de47a4eecbe11f498978a9b29d792f0d2692d1dd003650c24c76510e3bc001"
+checksum = "94d7b1cfd2aa4011f2de74c2c4c63665e27a71006b0a192dcd2710272e73dfa2"
 dependencies = [
  "autocfg",
  "bytes",
  "libc",
  "mio",
  "pin-project-lite",
  "socket2 0.4.9",
@@ -1068,24 +997,24 @@
  "log",
  "parking_lot",
  "percent-encoding",
  "phf",
  "pin-project-lite",
  "postgres-protocol",
  "postgres-types",
- "socket2 0.5.1",
+ "socket2 0.5.3",
  "tokio",
  "tokio-util",
 ]
 
 [[package]]
 name = "tokio-util"
-version = "0.7.7"
+version = "0.7.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5427d89453009325de0d8f342c9490009f76e999cb7672d77e46267448f7e6b2"
+checksum = "806fe8c2c87eccc8b3267cbae29ed3ab2d0bd37fca70ab622e46aaa9375ddb7d"
 dependencies = [
  "bytes",
  "futures-core",
  "futures-sink",
  "pin-project-lite",
  "tokio",
  "tracing",
@@ -1100,17 +1029,17 @@
  "cfg-if",
  "pin-project-lite",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-core"
-version = "0.1.30"
+version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "24eb03ba0eab1fd845050058ce5e616558e8f8d8fca633e6b163fe25c797213a"
+checksum = "0955b8137a1df6f1a2e9a37d8a6656291ff0297c1a97c24e0d8425fe2312f79a"
 dependencies = [
  "once_cell",
 ]
 
 [[package]]
 name = "typenum"
 version = "1.16.0"
@@ -1121,34 +1050,28 @@
 name = "unicode-bidi"
 version = "0.3.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.8"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
+checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
 name = "unicode-normalization"
 version = "0.1.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
 dependencies = [
  "tinyvec",
 ]
 
 [[package]]
-name = "unicode-width"
-version = "0.1.10"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c0edd1e5b14653f783770bce4a4dabb4a5108a5370a5f5d8cfe8710c361f6c8b"
-
-[[package]]
 name = "vcpkg"
 version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "accd4ea62f7bb7a82fe23066fb0957d48ef677f6eeb8215f372f52e48bb32426"
 
 [[package]]
 name = "version_check"
@@ -1166,65 +1089,65 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.84"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "31f8dcbc21f30d9b8f2ea926ecb58f6b91192c17e9d33594b3df58b2007ca53b"
+checksum = "7706a72ab36d8cb1f80ffbf0e071533974a60d0a308d01a5d0375bf60499a342"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.84"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "95ce90fd5bcc06af55a641a86428ee4229e44e07033963a2290a8e241607ccb9"
+checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.84"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c21f77c0bedc37fd5dc21f897894a5ca01e7bb159884559461862ae90c0b4c5"
+checksum = "dee495e55982a3bd48105a7b947fd2a9b4a8ae3010041b9e0faab3f9cd028f1d"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.84"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2aff81306fcac3c7515ad4e177f521b5c9a15f2b08f4e32d823066102f35a5f6"
+checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.84"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0046fef7e28c3804e5e38bfa31ea2a0f73905319b677e57ebe37e49358989b5d"
+checksum = "ca6ad05a4870b2bf5fe995117d3728437bd27d7cd5f06f13c17443ef369775a1"
 
 [[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
 dependencies = [
@@ -1235,156 +1158,90 @@
 [[package]]
 name = "winapi-i686-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
 
 [[package]]
-name = "winapi-util"
-version = "0.1.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "70ec6ce85bb158151cae5e5c87f95a8e97d2c0c4b001223f33a334e3ce5de178"
-dependencies = [
- "winapi",
-]
-
-[[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
 name = "windows"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
 dependencies = [
- "windows-targets 0.48.0",
+ "windows-targets",
 ]
 
 [[package]]
 name = "windows-sys"
-version = "0.45.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
-dependencies = [
- "windows-targets 0.42.2",
-]
-
-[[package]]
-name = "windows-targets"
-version = "0.42.2"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
- "windows_aarch64_gnullvm 0.42.2",
- "windows_aarch64_msvc 0.42.2",
- "windows_i686_gnu 0.42.2",
- "windows_i686_msvc 0.42.2",
- "windows_x86_64_gnu 0.42.2",
- "windows_x86_64_gnullvm 0.42.2",
- "windows_x86_64_msvc 0.42.2",
+ "windows-targets",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
 dependencies = [
- "windows_aarch64_gnullvm 0.48.0",
- "windows_aarch64_msvc 0.48.0",
- "windows_i686_gnu 0.48.0",
- "windows_i686_msvc 0.48.0",
- "windows_x86_64_gnu 0.48.0",
- "windows_x86_64_gnullvm 0.48.0",
- "windows_x86_64_msvc 0.48.0",
+ "windows_aarch64_gnullvm",
+ "windows_aarch64_msvc",
+ "windows_i686_gnu",
+ "windows_i686_msvc",
+ "windows_x86_64_gnu",
+ "windows_x86_64_gnullvm",
+ "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
-
-[[package]]
-name = "windows_aarch64_gnullvm"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
-
-[[package]]
-name = "windows_aarch64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
-
-[[package]]
-name = "windows_i686_gnu"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
-
-[[package]]
-name = "windows_i686_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
-
-[[package]]
-name = "windows_x86_64_gnu"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
-
-[[package]]
-name = "windows_x86_64_gnullvm"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
-
-[[package]]
-name = "windows_x86_64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
 name = "wyz"
 version = "0.5.1"
```

## aisdb_lib/Cargo.toml

```diff
@@ -1,9 +1,9 @@
 [package]
-version = "1.6.4"
+version = "1.6.5"
 name = "aisdb-lib"
 authors = [ "MERIDIAN // Matt Smith matthew.smith@dal.ca",]
 edition = "2021"
 include = [ "../aisdb/aisdb_sql", "/src/*",]
 build = "build.rs"
 readme = "readme.rst"
 description = "AIS Database and Processing Utils"
```

## aisdb_web/dist_map/index.html

```diff
@@ -12,15 +12,15 @@
       File:Antu tag-places.svg, CC BY 3.0, https://commons.wikimedia.org/w/index.php?curid=53807735 
     -->
     <link rel="icon" href="/favicon.svg" type="image/svg+xml">
     <link rel="mask-icon" href="/favicon.svg" type="image/svg+xml">
     <link rel="alternate icon" href="/favicon.png" type="image/png">
     <link rel="apple-touch-icon" href="/favicon.png" type="image/png">
     
-    <script type="module" crossorigin src="/assets/main-b42e8f3c.js"></script>
+    <script type="module" crossorigin src="/assets/main-4e7182f2.js"></script>
     <link rel="stylesheet" href="/assets/index-f2c4f58e.css">
   </head>
 
   <body>
     <div id="application">
       <div id="mapDiv" class="map"></div>
       <div id="overlay" class="overlay-popup">
```

## aisdb_web/dist_map_bingmaps/index.html

```diff
@@ -12,15 +12,15 @@
       File:Antu tag-places.svg, CC BY 3.0, https://commons.wikimedia.org/w/index.php?curid=53807735 
     -->
     <link rel="icon" href="/favicon.svg" type="image/svg+xml">
     <link rel="mask-icon" href="/favicon.svg" type="image/svg+xml">
     <link rel="alternate icon" href="/favicon.png" type="image/png">
     <link rel="apple-touch-icon" href="/favicon.png" type="image/png">
     
-    <script type="module" crossorigin src="/assets/main-8b0e81cf.js"></script>
+    <script type="module" crossorigin src="/assets/main-f2134a8e.js"></script>
     <link rel="stylesheet" href="/assets/index-f2c4f58e.css">
   </head>
 
   <body>
     <div id="application">
       <div id="mapDiv" class="map"></div>
       <div id="overlay" class="overlay-popup">
```

## Comparing `aisdb-1.6.4.dist-info/METADATA` & `aisdb-1.6.5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aisdb
-Version: 1.6.4
+Version: 1.6.5
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

## Comparing `aisdb/aisdb.cpython-39-aarch64-linux-gnu.so` & `aisdb/aisdb.cpython-39-darwin.so`

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

 * *Files 22% similar despite different names*

### strings --all --bytes=8 {}

```diff
@@ -1,219 +1,52 @@
-__gmon_start__
-_ITM_deregisterTMCloneTable
-_ITM_registerTMCloneTable
-__cxa_finalize
-PyInit_aisdb
-_Unwind_Resume
-PyErr_Restore
-PyErr_CheckSignals
-PyExc_TypeError
-PyExc_SystemError
-PyList_New
-PyUnicode_Type
-PyUnicode_AsUTF8AndSize
-PySequence_Check
-PySequence_Size
-__errno_location
-getauxval
-__stack_chk_guard
-__stack_chk_fail
-pthread_mutex_unlock
-pthread_mutex_trylock
-pthread_mutex_lock
-getpagesize
-gettimeofday
-pthread_join
-pthread_create
-pthread_mutex_destroy
-pthread_mutexattr_init
-pthread_mutexattr_settype
-pthread_mutex_init
-pthread_mutexattr_destroy
-localtime_r
-ftruncate64
-readlink
-getsockname
-getpeername
-getsockopt
-shutdown
-recvfrom
-setsockopt
-epoll_create1
-epoll_create
-epoll_wait
-epoll_ctl
-PyUnicode_FromStringAndSize
-PyTuple_New
-PyTuple_SetItem
-PyNumber_Index
-_Py_Dealloc
-PyObject_Repr
-PyObject_Str
-PyObject_GetIter
-PyIter_Next
-PyLong_FromLong
-PyLong_AsLong
-PyLong_FromUnsignedLongLong
-PyLong_AsUnsignedLongLong
-PyObject_IsInstance
-PyObject_GetAttr
-PyBytes_AsString
-PyBytes_Size
-Py_IsInitialized
-PyGILState_Ensure
-PyGILState_Release
-PyErr_Fetch
-PyErr_PrintEx
-PyErr_NewExceptionWithDoc
-PyException_GetCause
-PyException_SetCause
-PyErr_NormalizeException
-PyErr_Print
-_Py_NoneStruct
-PyFloat_FromDouble
-PyUnicode_InternInPlace
-PyUnicode_AsEncodedString
-PyObject_SetAttr
-PyFloat_AsDouble
-PyBool_Type
-_Py_TrueStruct
-PyList_Append
-PyExc_BaseException
-PyExc_AttributeError
-PyErr_GivenExceptionMatches
-PyModule_GetName
-PyModule_Create2
-PyCMethod_New
-PyExc_ValueError
-PyExc_ImportError
-PyExc_OverflowError
-__xpg_strerror_r
-_Unwind_GetTextRelBase
-_Unwind_GetDataRelBase
-freeaddrinfo
-pthread_self
-pthread_getattr_np
-pthread_attr_getstack
-pthread_attr_destroy
-sched_yield
-nanosleep
-_Unwind_GetIP
-_Unwind_Backtrace
-posix_memalign
-realpath
-pthread_getspecific
-pthread_setspecific
-gnu_get_libc_version
-getrandom
-sigaltstack
-mprotect
-pthread_attr_init
-pthread_attr_setstacksize
-pthread_setname_np
-pthread_detach
-pthread_attr_getguardsize
-__cxa_thread_atexit_impl
-clock_gettime
-pthread_key_create
-pthread_key_delete
-getaddrinfo
-__res_init
-gai_strerror
-_Unwind_GetLanguageSpecificData
-_Unwind_GetIPInfo
-_Unwind_GetRegionStart
-_Unwind_SetGR
-_Unwind_SetIP
-dl_iterate_phdr
-_Unwind_DeleteException
-_Unwind_RaiseException
-__register_atfork
-__xstat64
-__fxstat64
-__lxstat64
-libgcc_s.so.1
-libpthread.so.0
-libm.so.6
-libdl.so.2
-libc.so.6
-ld-linux-aarch64.so.1
-GLIBC_2.17
-GCC_4.2.0
-9	!@9*#@9)#
-9	%@9*'@9)'
-9	)@9*+@9)+
-9	-@9*/@9)/
-9	1@9*3@9)3
-9	5@9*7@9)7
-9	9@9*;@9);
-9	=@9*?@9)?
-9	A@9*C@9)C
-9	E@9*G@9)G
-9	I@9*K@9)K
-9	M@9*O@9)O
-9	Q@9*S@9)S
-9	U@9*W@9)W
-9	Y@9*[@9)[
-9	]@9*_@9)_
-9	a@9*c@9)c
-9	e@9*g@9)g
-9	i@9*k@9)k
-9	m@9*o@9)o
-9	q@9*s@9)s
-9	u@9*w@9)w
-9	y@9*{@9){
-9	!@9*#@9)#
-9	%@9*'@9)'
-9	)@9*+@9)+
-9	-@9*/@9)/
-9	1@9*3@9)3
-9	5@9*7@9)7
-9	9@9*;@9);
-9	=@9*?@9)?
-9	A@9*C@9)C
-9	E@9*G@9)G
-9	I@9*K@9)K
-9	M@9*O@9)O
-9	Q@9*S@9)S
-9	U@9*W@9)W
-9	Y@9*[@9)[
-9	]@9*_@9)_
-9	a@9*c@9)c
-9	e@9*g@9)g
-9	i@9*k@9)k
-9	m@9*o@9)o
-9	q@9*s@9)s
-9	u@9*w@9)w
-9	y@9*{@9){
-;jh88ji8H
-jYjxkyhx(
-hb@9jj@9
-;@9*	@9H
-(oBT(OrQ
-<	TCO*TCO
-<	TCO*TCO
-<	TCO*TCO
-Kik8+i(8
-ja8"j`8C
-	hi8Lii8
-+=@y(1@y
-(@@y)D@y
-(Q@yJS@y
-]3@yS7@yw
-H9)!KJJAKJ)
-H9)!JJkAJJ)
-<u@9=1@y45@y
+__stub_helper
+__gcc_except_tab__TEXT
+__cstring
+__unwind_info
+__eh_frame
+__DATA_CONST
+__DATA_CONST
+__DATA_CONST
+__la_symbol_ptr
+__thread_vars
+__thread_data
+__thread_bss
+__common
+__LINKEDIT
+@rpath/aisdb.cpython-39-darwin.so
+/System/Library/Frameworks/Security.framework/Versions/A/Security
+/System/Library/Frameworks/SystemConfiguration.framework/Versions/A/SystemConfiguration
+/System/Library/Frameworks/CoreFoundation.framework/Versions/A/CoreFoundation
+/usr/lib/libiconv.2.dylib
+/usr/lib/libSystem.B.dylib
+x@9	8@y A
+T*	@9HAHJ(	
+TCOxTCOYTCO9
+TCOxTCOYTCO9
+TCOxTCOYTCO9
+Oih8Pin81
+Oih8Pin81
+ja8#jb8d
+	hh8ihi8
+jh8+ik8Ki(8
+hi8Kik8k
+Rj&L)l.@
+(!@y* @y
+S3@y[7@yW
+@y	A	*(	
 h0@yi4@y
-R@y	Q@y?
-w2@yx6@y
-H9.T@9+ @y!
-LC@yJG@y
-Rl.I)n"@
- N%4%n&4&n
+h0@yi4@y
+45@y79@y
+@y	A	*(	
+vb@9w6@yx:@yH
++@@9,D@9-$@y.(@y6
+vb@9w6@yx:@y
+(@@y)D@y
+ N'4'n040n141n242n
+ N'4'n040n141n242n
 hh8Mhh8Nih8
 H(NBh(N@x
 q"H(NBh(NAx
 H(NBh(N@x@L"H(NB
 X(NBx(N@x
 q"X(NBx(NAx
 X(NBx(N@x@L"X(NB
@@ -223,144 +56,288 @@
 h(N!J(N!h(N
 J(N!h(N J(N
 h(N!J(N!h(N
 J(N!h(NB
 J(N!h(Nc
 0NcTAORB
 GHASH for ARMv8, CRYPTOGAMS by <appro@openssl.org>
-LH}@Li}@L
 Montgomery Multiplication for ARMv8, CRYPTOGAMS by <appro@openssl.org>
 ECP_NISTZ256 for ARMv8, CRYPTOGAMS by <appro@openssl.org>
-0NcTAORB
-hc8!hc8A
-@)h*A)l.B)i
-C)e>D)nFE)pJF)
-h*A)l.B)e"@
-"H@9#D@9J
-5hA)6xB)
-5hA)6xB)
-i!@yJ=@9
-hb8$hb8B
-Dic8%ic8c
-TDic8%ic8c
-l@y#l@y h@yF
-hb8#hb8B
-hb8$hb8B
-ja8%hc8!
-jb8Dha8B
-#ib8Dib8B
-T#ib8Dib8B
-$ic8Ehc8c
-T$ic8Ehc8c
-Ch`8Di`8
-Ch`8Di`8
-4`Z@9aB@9
-bF@9`P@y
-5@UA9F!L)
-h7b*@yBp
-TdIj8`A*
-n4`b=3@_=2 \=1
-n$`I=#@F=! C=
-86C	@9`8
-bb@9af@9
-ha8bk!8!
-hb8 hb8c
-%id8fhd8
-a&@9b*@9
-(@y (@yb
-r@ybj@y_
-B@9`B@9v
-Bhs8!hs8_
-R s@9c+@
-@y!AH6@h`
-ha8Bka8!
-ha8bka8!
-bha8`ka8!
-bha8`ka8!
-bha8@ka8!
- TC9(PC9
-ak`8Bi`8
-Tak`8Bi`8
-n4`b=3@_=2 \=1
-n$`I="@F=! C=
-9aB@9`&@9a^
-aW@9`h@y!
-y2@yz&@9{*@
-9a&@9`2@y!
-S$7@y#/@9!
-5 3@y"+@
-S$5@y#	@9
- @9!xzxZ
-T`&@9b*@
-`h@y`:(6d
-bh@yb!(6d
-ah@ya/(6d
-ahvx`h{x
-Kb'@9`3@
-*$0@9!$@9
-jkb8aka8
-Ta2@9`*@
-5a2@9y2@
-bha8dja8!
-jb8$hb8B
-ha8(hc8!
-ha8(hc8!
-#$@y"X@9c
-i`8bi`8?
-&@yd&@y!
-in@y`2@y
-*@?@y&xw
-ha8'hf8_
-k`8ah`8?
-xsxakax{
-Al@y@p@y!
-TCO@TCO!
-&n7`(@yZc
-  @9"0@y
-@@9`@@9_
-hha8	ka8!
-ha8Cka8!
-@xaNbxaN!
-@@9`@@9_
-0A9 ?G9_
-ha8Dha8!
-Bi`8ah`8?
-ah`8Bi`8?
-h`8Ch`8?
-h`8Ch`8?
-&@9`'@9?
-gif8Hif8
-gif8Hif8
-Ehd8fjd8
-5iRA))E	J
-(oBT(OrQ
-F93hl8Ijs8)A/
-)hl8Sji8
-)5	J)EIJ 
-6MJ8KMJ8
-B9iS@x	=
-ij8mij8J
-hj8mij8J
-Tii`8dh`8
-Tii`8dh`8
-h @9j$@9i(@9
-Qj,@9i4@9
-j,@9i4@9
-hj8Thj8J
-@8ii*8		
-BN!(aN!(!
-jYjxkyixi
-?receiveralready mutably borrowed/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/pyo3-0.18.3/src/gil.rsuncaught panic at ffi boundaryhaversinex1y1x2y2unknown file type! src/lib.rsdecoding NM4decoding CSVdecoderdbpathpsql_conn_stringtcp_connect_addrfilessourceverbosesimplify_linestring_idxxyprecisionencoder_score_fcnt1t2speed_threshdist_threshbinarysearch_vectorarrsearchexiting...
-sqlite_dbpathpostgres_connection_stringtcp_listen_addrudp_listen_addrmulticast_addr_parsedmulticast_addr_rawtcp_output_addrudp_output_addrdynamic_msg_bufsizestatic_msg_bufsizetee
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/geo-0.25.0/src/algorithm/simplify_vw.rscalled `Option::unwrap()` on a `None` value
-fatal runtime error: 
-thread result panicked on dropCouldn't compare valuessrc/lib.rs
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/pyo3-0.18.3/src/conversions/std/vec.rsout of range integral type conversion attempted on `elements.len()`Attempted to create PyList but `elements` was larger than reported by its `ExactSizeIterator` implementation.Attempted to create PyList but `elements` was smaller than reported by its `ExactSizeIterator` implementation.Can't extract `str` to `Vec`
-%attempted to fetch exception but none was set/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/pyo3-0.18.3/src/impl_/extract_argument.rsPyString
-attempted to fetch exception but none was setSequencehaversine
+n!TAOBTAOcTAO
+m:@)oBA)sB
+1i(8?i.8
+T/i(8?i-8
+T1i(8?i.8
+/i(8oin8o
+T1i(8?i.8
+T/i(8/in8/
+T1i(8?i.8
+T/i(8/in8o
+T1i(8?i.8
+T/i(8/in8o
+T/i(8/in8
+1i(8?i.8
+T/i(8?i-8
+T1i(8?i.8
+/i(8oin8o
+T1i(8?i.8
+T/i(8/in8/
+T1i(8?i.8
+T/i(8/in8o
+T1i(8?i.8
+T/i(8/in8o
+T/i(8/in8
+%8@):DA)<
+C)/lD)"xE)$
+%8@):DA)<
+C)/lD)"xE)$
+N#H(Nch(N$
+H(N!h(Nk
+H(NBh(NaH(N!h(N@H(N
+H(N!h(NAH(N!h(N(
+N"H(NBh(N
+H(NBh(NH
+N"H(NBh(N
+H(NBh(NH
+X(NBx(N@
+NCH(Nch(N
+H(N!h(Nk
+H(NBh(NJ
+H(N!h(NbH(NBh(N H(N
+mkm8nkn8
+Tmkm8nkn8
+Tmkm8nkn8
+Tmkm8nkn8
+Tmkm8nkn8
+mkm8nkn8
+mkm8nkn8
+mkm8nkn8
+mkm8nkn8
+*is8*k38j
+,kl8,k+8J
+@9Lih8mih8
+Nim8Li-8Ni(8
+Mil8Mi)8Ki,8Iii8)
+(ih8*ij8
+Mim8Nin8
+Lil8Mim8
+bjt8"ib8!
+nin8oio8
+nin8oio8
+Mkm8Nkn8
+Kkk8Lkl8
+Mim8Nin8
+/io80ip8
+T*ij8+ik8_
+0ip81iq8
+T,il8-im8
+T+ik8,il8
+T-im8.in8
+T-im8.in8
+T,il8-im8
+T+ik8,il8
+/io80ip8
++@y	'@y*
+Oc0pNB0p
+Ti"@9t.@
+0@y	 @9?
+6m{lxM{m
+5i2@9v2@
+Ri2@9v2@
+NAx)\#6	
+))@yIbh7
+.in8/io8
+	(@y((@y
+$@9	L@9?
+/io80ip8
+	X@9A @9?
+(@y+(@yl
+Ty&@9h2@yH
+.!@9-%@9+)@9,-@9
+i&@9j*@9)
+K3@yL3@9
+?k(8)kh8
+*ij8+ik8_
+jh8+hh8_
+3(	@9Lih8L
+3(!@9Hih8	
+	hh8Kii8
++ih8Kik8
+Hk8)ik8)
+Pip8Qiq8
+nin8oio8
+Aia8Cic8?
+Tqiq8`i`8?
+Tqiq8`i`8?
+Toio8pip8
+Tqiq8`i`8?
+Tqiq8`i`8?
+Toio8pip8
+TAia8Cic8?
+TOio8Pip8
+Mim8Nin8
+Lil8Mim8
+R	y6x(2Fx
+R	Y*x("@
+/io80ip8
+Mim8Nin8
+Mim8Nin8
+nkn8oko8
+Tkkk8lkl8
+Tkkk8lkl8
+kkk8lkl8
+Mim8Nin8
+Cic8Did8
+ip8`ip8?
+TQiq8@i`8?
+T@i`8Aia8
+@i`8Aia8
+Jkh8+ih8_
+hh8+ih8_
+mil8.kl8
+Mim8Nin8
+Mim8Nin8
+kkk8lkl8
+,il8-im8
+nin8oio8
+mim8nin8
+T*ij8+ik8_
+T*ij8+ik8_
+b@yjb@y?
+mkm8nkn8
+Kik8Lil8
+Kik8Lil8
+Mim8Nin8
+Mim8Nin8
+ i`8!ia8
+,il8-im8
+@yN1@yOa@y
+/io80ip8
+)kh8jih8?
+Mim8Nin8
+/io80ip8
+/io80ip8
+T,il8-im8
++ik8,il8
+`@ykb@y_
+X$@yN @y
+V(h7#((7
+W3@y[o@y
+,il8-im8
+-im8.in8
+-im8.in8
+yjY@9H#)
+T,il8-im8
+Kik8Lil8k
+h'@yi&@y(
+?7h+@yi*@y
+jkj8kkk8_
+F@9jF@9?
+O6mi@yom@y
+Knj@ypn@y
+t2@yun@ya
+Kik8Lil8
+/io80ip8
+pip8qiq8
+Tqjq8`j`8?
+Tpkp8qkq8
+/io80ip8
+jjj8kjk8_
+ii8Khi8_
+njn8ojo8
+/io80ip8
++ik8,il8
+T`i`8aia8
+T`i`8aia8
+nG:QNqIA
+ij@y?!(k
+/io80ip8
+-km8.kn8
+,il8-im8
+(ih8,il8
+jj8kkk8J
+Nin8Oio8
+Nin8Oio8
+4ir@9J)	
+hf@9ib@9(
+Mkm8Nkn8
+mil8.kl8
+Mkm8Nkn8
+mil8.kl8
+nin8oio8
+lil8mim8
+lil8mim8
+nin8oio8
+pip8qiq8
+nin8oio8
+Kik8Lil8
+Jkj8Kkk8_
+Jkj8Kkk8_
+Jkj8Kkk8_
+Lkl8Mkm8
+Hkh8Kkk8
+TJkj8Kkk8_
+TJkj8Kkk8_
+Iki8Jkj8?
+q@	@z 	@z@
+@9,il8L,
+6l	@9,il8
+@9+ik8++
+Ka8)kh8!
+T+ki8+k(8)
+T+kh8+k*8
+(3A9 =G9
+ix8kkx8_
+i{8Kk{8_
+Lii8Mki8
+,il8-im8
+Kik8Lil8
++ih8,hh8
+,il8-im8
+,il8-im8
+ikh8jih8?
+Nin8Oio8
+Mim8Nin8
+R-il8Nil8
+R-il8Nil8
+TKkk8Lkl8
+TKkk8Lkl8
+TKkk8Lkl8
+Jkj8Kkk8_
+jkxKhkxL
+jlxLhlxm
+Tqiq8`i`8?
+pip8qiq8
+kki8Lii8
+kki8Lii8
+kki8Lii8
+nin8oio8
+nin8oio8
+?#A9(3C9
+?#A9(3C9
+)A@9jjh8I
+JA@9+kh8j
+@9kh(8H	
+hjw8hj88
+|E95hl8	ju8)A/
+4	}	SjF@
+QI$@9J,@9
+I$@9J,@9)
+Tdi`8Iii8
+CX n$X n
+N"H(NBh(N
+H(NBh(NJ
+N"H(NBh(N
+H(NBh(NH
+j"8dh"8B
+already mutably borrowed/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/pyo3-0.18.3/src/gil.rsuncaught panic at ffi boundaryhaversinex1y1x2y2unknown file type! src/lib.rsdecoding NM4
+decoding CSVdecoderdbpathfilessourceverbosesimplify_linestring_idxxyprecisionencoder_score_fcnt1t2speed_threshdist_threshbinarysearch_vectorarrsearchexiting...
+sqlite_dbpathpostgres_connection_stringtcp_listen_addrudp_listen_addrmulticast_addr_parsedmulticast_addr_rawtcp_output_addrudp_output_addrdynamic_msg_bufsizestatic_msg_bufsizeteepsql_conn_stringtcp_connect_addrreceiveralready mutably borrowed/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/pyo3-0.18.3/src/gil.rsuncaught panic at ffi boundaryaisdb
+Functions imported from Rust
+haversine
 haversine(x1, y1, x2, y2)
 fast great circle distance
     x1 (float64)
         longitude of coordinate pair 1
     y1 (float64)
         latitude of coordinate pair 1
     x2 (float64)
@@ -461,120 +438,185 @@
         Number of positional messages to keep before inserting into the database.
         Defaults to 256 if none is given
     static_msg_bufsize (Option<usize>)
         Number of static messages to keep before inserting into database.
         Defaults to 64
     tee (bool)
         If True, raw input will be copied to stdout
-/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/std/src/io/mod.rsfailed to write whole bufferformatter erroralready mutably borrowed/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/pyo3-0.18.3/src/gil.rsuncaught panic at ffi boundaryaisdb
-Functions imported from Rust
-already borrowedfield identifiertcp_connect_addr[
- UDP -> dim_portdim_star}
-/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/core/src/str/pattern.rscalled `Result::unwrap()` on an `Err` value/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/alloc/src/slice.rsError while closing SQLite connection: 
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/inner_connection.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/cache.rsreceiver/src/receiver.rs0.0.0.0:9921
+!#%')+-/13579;=?ACEGIKMOQSUWY[]_/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/std/src/io/mod.rsfailed to write whole bufferformatter errorPyString
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/pyo3-0.18.3/src/conversions/std/vec.rsout of range integral type conversion attempted on `elements.len()`Attempted to create PyList but `elements` was larger than reported by its `ExactSizeIterator` implementation.Attempted to create PyList but `elements` was smaller than reported by its `ExactSizeIterator` implementation.Can't extract `str` to `Vec`
+(attempted to fetch exception but none was set/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/pyo3-0.18.3/src/impl_/extract_argument.rs
+(attempted to fetch exception but none was set
+Sequence
+fatal runtime error: thread result panicked on drop
+Couldn't compare valuessrc/lib.rs
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/geo-0.25.0/src/algorithm/simplify_vw.rscalled `Option::unwrap()` on a `None` value)
+ "$&(*,.02468:<>@BDFHJLNPRTVXZ\^
+ffffffffWf
+iwriting frame tungstenite::protocol::frame/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tungstenite-0.19.0/src/protocol/frame/mod.rsBug: can't write to vectorConnection reset while sendingfailed to write the buffered data
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/bytes-1.4.0/src/buf/buf_impl.rsoverflowassertion failed: pos <= self.get_ref().as_ref().len()
+88888888+8
+i/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tungstenite-0.19.0/src/buffer.rscould not resolve to any addresses
+called `Result::unwrap()` on an `Err` valuePoisonErrorError while closing SQLite connection: 
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/inner_connection.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/cache.rsSpawning receiver. Dynamic msgs buffer: 	 Static msgs buffer: receiver/src/receiver.rsdecode_multicast: got an error: sending to UDP listener via multicastsending to websocket via UDP multicast socketwriting to output bufferbinding socketforwarding:  WEBSOCKET
+accepting websocket connection from downstreamstream_server upstream: got an error: dropping client:  spawning websocket listener on /tcp
+ "$&(*,.02468:<>@BDFHJLNPRTVXZ\^`bdfhDoing handshake round.
+tungstenite::handshake::machine/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tungstenite-0.19.0/src/handshake/machine.rsassertion failed: buf.has_remaining()assertion failed: size > 0/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/http-0.2.9/src/header/map.rs
+internal error: entered unreachable code/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/serde_json-1.0.97/src/ser.rs\t\r\n\f\b\\\"00010203040506070809101112131415161718192021222324252627282930313233343536373839404142434445464748495051525354555657585960616263646566676869707172737475767778798081828384858687888990919293949596979899
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/futures-channel-0.3.28/src/mpsc/mod.rs
+called `Result::unwrap()` on an `Err` valuecalled `Option::unwrap()` on a `None` value
+llIMQlllX
+/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/core/src/str/pattern.rscalled `Result::unwrap()` on an `Err` valueError while closing SQLite connection: 
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/inner_connection.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/cache.rsreceiver/src/receiver.rs0.0.0.0:9921
 Inserting  static messages ...
 rxError inserting vessel static data:  dynamic messages ...
 Error inserting vessel dynamic data: Decoding messages incoming on copying raw input:  UDP
-copying parsed output to binding socket interfacegetting sqlite db connectiongetting postgres db connectionmmsitimelonlatrotsogheadingimovessel_nameship_typedim_bowdim_sterndraught
-/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/std/src/thread/mod.rsfailed to spawn threadthread name may not contain interior null bytes
-fatal runtime error: 
-thread result panicked on dropError while closing SQLite connection: /root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/inner_connection.rsalready borrowed/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/cache.rscalled `Option::unwrap()` on a `None` value/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/alloc/src/collections/btree/navigate.rsPoisonError
-aaaaaaaaQa
-writing frame tungstenite::protocol::frame/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tungstenite-0.19.0/src/protocol/frame/mod.rsBug: can't write to vectorConnection reset while sendingfailed to write the buffered data
-88888888+8
-binternal error: entered unreachable code/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/serde_json-1.0.96/src/ser.rs\t\r\n\f\b\\\"could not resolve to any addresses
-called `Result::unwrap()` on an `Err` valueError while closing SQLite connection: 
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/inner_connection.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/cache.rsSpawning receiver. Dynamic msgs buffer: 	 Static msgs buffer: receiver/src/receiver.rsdecode_multicast: got an error: sending to UDP listener via multicastsending to websocket via UDP multicast socketwriting to output bufferbinding socketforwarding:  UDP ->  WEBSOCKET
-accepting websocket connection from downstreamstream_server upstream: got an error: dropping client:  spawning websocket listener on /tcp
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/futures-channel-0.3.28/src/mpsc/mod.rscalled `Result::unwrap()` on an `Err` valuecalled `Option::unwrap()` on a `None` valueG,G
-bformatter error/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/alloc/src/slice.rs/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/alloc/src/vec/mod.rs
-called `Option::unwrap()` on a `None` value/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/alloc/src/collections/btree/navigate.rsSomeNone/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/bytes-1.4.0/src/buf/buf_impl.rsoverflowassertion failed: pos <= self.get_ref().as_ref().len()Error while closing SQLite connection: 
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/inner_connection.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/cache.rs
+copying parsed output to binding socket interfacegetting sqlite db connectiongetting postgres db connectionmmsilonlattimerotsogheading
+imovessel_nameship_typedim_bowdim_sterndim_portdim_stardraught
+already borrowed 
+ UDP -> 
 Sending pong reply
-tungstenite::protocol/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tungstenite-0.19.0/src/protocol/mod.rsFrames still in queue: Sending frame: assertion failed: (*tail).value.is_none()/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/futures-channel-0.3.28/src/mpsc/queue.rsassertion failed: (*next).value.is_some()
-b/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/std/src/io/mod.rsfailed to write whole bufferformatter errorno addresses to send data to/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/http-0.2.9/src/header/map.rs
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tungstenite-0.19.0/src/buffer.rs
-00010203040506070809101112131415161718192021222324252627282930313233343536373839404142434445464748495051525354555657585960616263646566676869707172737475767778798081828384858687888990919293949596979899HandshakeError::Failure()HandshakeError::Interrupted(...)Server handshake done.
-tungstenite::handshake::server/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tungstenite-0.19.0/src/handshake/server.rsServer handshake failed.called `Option::unwrap()` on a `None` value 
-: Server handshake initiated.Doing handshake round.
-tungstenite::handshake::machine/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tungstenite-0.19.0/src/handshake/machine.rsassertion failed: buf.has_remaining()assertion failed: size > 0
-$*06<BHNT`lx
-TEXTPONGPINGDataTextPongPingIanaSizeAwayRESERVED_DATA_BINARYCONTINUEReservedContinueAbnormalProtocolRESERVED_CONTROL_CLOSEControlBinaryCloseBadLibraryTlsAgainRestartErrorExtensionPolicyInvalidStatusUnsupportedNormal
-overflow
-final: is_final
+tungstenite::protocol/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tungstenite-0.19.0/src/protocol/mod.rsFrames still in queue: Sending frame: assertion failed: (*tail).value.is_none()/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/futures-channel-0.3.28/src/mpsc/queue.rsassertion failed: (*next).value.is_some()
+!#%')+-/13579;=?ACEGIKMOQSUWY[]_/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/std/src/io/mod.rsfailed to write whole bufferformatter error
+called `Option::unwrap()` on a `None` value/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/alloc/src/collections/btree/navigate.rsHandshakeError::Failure()HandshakeError::Interrupted(...)
+Server handshake done.
+tungstenite::handshake::server/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tungstenite-0.19.0/src/handshake/server.rsServer handshake failed.called `Option::unwrap()` on a `None` value 
+: Server handshake initiated.
+formatter error/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/alloc/src/vec/mod.rs
+/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/std/src/thread/mod.rsfailed to spawn threadthread name may not contain interior null bytes
+fatal runtime error: thread result panicked on drop
+Error while closing SQLite connection: 
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/inner_connection.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/cache.rsno addresses to send data to
+statusversionheadersBug: no HTTP versionBug: no method in headerBug: no path in header/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tungstenite-0.19.0/src/handshake/server.rsResponsebody
+ "$&(*,.02468:<>@BDFHJLNPRTVXZ\^`bd
+#(+05<FPZ
+RESERVED_DATA_BINARYRESERVED_CONTROL_CLOSEControlBinaryCloseBadLibraryTlsAgainRestartErrorExtensionPolicyInvalidStatusUnsupportedNormalTEXTPONGPINGPongPingIanaSizeAwayCONTINUEReservedContinueAbnormalProtocol
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/http-0.2.9/src/header/map.rsheader map at capacityConnectionUpgradewebsocketSec-WebSocket-VersionSec-WebSocket-KeySec-WebSocket-Accept13
+$'0369<?BENWZcfs
+ %,/6;>CFKPU_inx}
+HTTP format error: HTTP error: URL error: UTF-8 encoding errorSend queue is fullWebSocket protocol error: Space limit exceeded: TLS error: IO error: Trying to work with closed connectionConnection closed normallyHttpFormatUrlSendQueueFullTlsIoAlreadyClosedMessage too long:  > MessageTooLongTooManyHeadersInvalid close sequenceEncountered invalid opcode: Connection reset without closing handshakeWhile waiting for more fragments received: Continue frame but nothing to continueUnknown data frame type: Unknown control frame type: Control frame too big (payload must be 125 bytes or less)Fragmented control frameReceived a masked frame from serverReceived an unmasked frame from clientReserved bits are non-zeroRemote sent after having closedSending after closing is not allowedHandshake not finishedMissing, duplicated or incorrect header Custom response must not be successfulJunk after client requestKey mismatch in "Sec-WebSocket-Accept" headerNo "Sec-WebSocket-Key" headerNo "Sec-WebSocket-Version: 13" headerNo "Upgrade: websocket" headerNo "Connection: upgrade" headerHTTP version must be 1.1 or higherUnsupported HTTP method used - only GET is allowedInvalidCloseSequenceInvalidOpcodeResetWithoutClosingHandshakeUnexpectedContinueFrameUnknownDataFrameTypeUnknownControlFrameTypeControlFrameTooBigFragmentedControlFrameMaskedFrameFromServerUnmaskedFrameFromClientNonZeroReservedBitsReceivedAfterClosingHttparseErrorHandshakeIncompleteInvalidHeaderCustomResponseSuccessfulSecWebSocketAcceptKeyMismatchMissingSecWebSocketKeyMissingSecWebSocketVersionHeaderMissingUpgradeWebSocketHeaderMissingConnectionUpgradeHeaderWrongHttpMethodNo path/query in URLURL contains empty host nameURL scheme not supportedUnable to connect to No host name in the URLTLS support not compiled inNoPathOrQueryEmptyHostNameUnsupportedUrlSchemeUnableToConnectNoHostNameTlsFeatureNotEnabledwebpki error: rustls error: InvalidDnsNameWebpkiRustlsHttpCapacitymax_size
+ConnectionClosedToo many headershttparse error: ExpectedFragmentSendAfterClosingJunkAfterRequestWrongHttpVersionInvalid DNS name
 reserved:  
 opcode: 
 length: 
 payload length: 
 payload: 0x
-            CloseFramecodersv1rsv2rsv3maskreasonopcodeFrameHeaderFrameheaderpayload
-"%,/258;>AHORY\o
-$*06<BHNTZ`flr~
-HTTP format error: HTTP error: URL error: UTF-8 encoding errorSend queue is fullWebSocket protocol error: Space limit exceeded: TLS error: IO error: Trying to work with closed connectionConnection closed normallyHttpFormatHttpUtf8sizeUrlSendQueueFullCapacitymax_sizeTlsIoAlreadyClosedConnectionClosedToo many headershttparse error: ExpectedFragmentSendAfterClosingJunkAfterRequestWrongHttpVersionInvalid DNS nameMessage too long:  > MessageTooLongTooManyHeadersInvalid close sequenceEncountered invalid opcode: Connection reset without closing handshakeWhile waiting for more fragments received: Continue frame but nothing to continueUnknown data frame type: Unknown control frame type: Control frame too big (payload must be 125 bytes or less)Fragmented control frameReceived a masked frame from serverReceived an unmasked frame from clientReserved bits are non-zeroRemote sent after having closedSending after closing is not allowedHandshake not finishedMissing, duplicated or incorrect header Custom response must not be successfulJunk after client requestKey mismatch in "Sec-WebSocket-Accept" headerNo "Sec-WebSocket-Key" headerNo "Sec-WebSocket-Version: 13" headerNo "Upgrade: websocket" headerNo "Connection: upgrade" headerHTTP version must be 1.1 or higherUnsupported HTTP method used - only GET is allowedInvalidCloseSequenceInvalidOpcodeResetWithoutClosingHandshakeUnexpectedContinueFrameUnknownDataFrameTypeUnknownControlFrameTypeControlFrameTooBigFragmentedControlFrameMaskedFrameFromServerUnmaskedFrameFromClientNonZeroReservedBitsReceivedAfterClosingHttparseErrorHandshakeIncompleteInvalidHeaderCustomResponseSuccessfulSecWebSocketAcceptKeyMismatchMissingSecWebSocketKeyMissingSecWebSocketVersionHeaderMissingUpgradeWebSocketHeaderMissingConnectionUpgradeHeaderWrongHttpMethodNo path/query in URLURL contains empty host nameURL scheme not supportedUnable to connect to No host name in the URLTLS support not compiled inNoPathOrQueryEmptyHostNameUnsupportedUrlSchemeUnableToConnectNoHostNameTlsFeatureNotEnabledwebpki error: rustls error: InvalidDnsNameWebpkiRustls
-ConnectionUpgradeSec-WebSocket-VersionSec-WebSocket-KeywebsocketSec-WebSocket-Accept13Bug: no method in headerBug: no HTTP versionBug: no path in header/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tungstenite-0.19.0/src/handshake/server.rs258EAFA5-E914-47DA-95CA-C5AB0DC85B11ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/
+            CloseFramereasonopcodeFrameHeaderFrameheaderpayload
+final: is_finalrsv1rsv2rsv3mask
+!#%')+-/13579;=?ACEGIKMOQSUWY[]_
+!#%')+-/13579;=?ACEGIKMOQSUWY[]_aceg
+BinaryFrameClose
+258EAFA5-E914-47DA-95CA-C5AB0DC85B11ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/
 ?456789:;<=
  !"#$%&'()*+,-./0123
-Responsehttpbody at statusversionheaders
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/http-0.2.9/src/header/map.rs
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/http-0.2.9/src/header/map.rsheader map at capacityrequested capacity too large
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/http-0.2.9/src/header/map.rs
 0123456789
 abcdefghijklmnopqrstuvwxyz
 ^_`abcdefghijklmnopqrstuvwxyz
-BinaryFrameClose
-uespemosarenegylmodnarodsetybdet/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/http-0.2.9/src/header/map.rsheader map at capacityrequested capacity too large
-called `Result::unwrap()` on an `Err` value/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/data-encoding-2.4.0/src/lib.rsattempt to divide by zeroexplicit panic
-$*06<BHNTZ`flrx~
-$*06<BHNTZ`flr
-AlertDescriptionUnrecognisedNameMissingExtensionIllegalParameterHandshakeFailureDecryptionFailedNewSessionTicketChangeCipherSpecRSA_PKCS1_SHA512RSA_PKCS1_SHA384RSA_PKCS1_SHA256UnknownNoApplicationProtocolCertificateRequiredUnknownPSKIdentityBadCertificateHashValueBadCertificateStatusResponseCertificateUnobtainableUnsupportedExtensionNoRenegotiationUserCanceledInappropriateFallbackInternalErrorInsufficientSecurityProtocolVersionExportRestrictionDecryptErrorDecodeErrorAccessDeniedUnknownCACertificateUnknownCertificateExpiredCertificateRevokedUnsupportedCertificateBadCertificateNoCertificateDecompressionFailureRecordOverflowBadRecordMacUnexpectedMessageCloseNotifyMessageHashKeyUpdateCertificateStatusCertificateURLFinishedDTLSv1_3DTLSv1_2DTLSv1_0ClientKeyExchangeCertificateVerifyServerHelloDoneCertificateRequestServerKeyExchangeCertificateEncryptedExtensionsHelloRetryRequestEndOfEarlyDataHelloVerifyRequestServerHelloClientHelloHelloRequestHeartbeatApplicationDataHandshakeAlert
-HostNameidentityKeyShareBulkOnlylifetimeFinishedOCSPcertextsECDHECDHERSADHEDH
-attempt to join into collection with len > usize::MAXassertion failed: mid <= self.len()/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/alloc/src/str.rs
-R '*ru-x4
-,36>FN\jx
-$*06<BNTZfrx~
- or spkithe supplied max_fragment_size was too small or largepeer doesn't support any known protocolpeer sent excess record sizehandshake not completefailed to get random bytesfailed to get current timeunexpected error: invalid certificate timestamp: invalid peer certificate: received fatal alert: peer misbehaved: peer is incompatible: cannot encrypt messagecannot decrypt peer's messagepresented server name type wasn't supportedpeer sent no certificatesreceived corrupt message of type received unexpected handshake message: got  when expecting OwnedTrustAnchorname_constraintsPeerIncompatibleInvalidKeyUpdatereceived unexpected message: got client authentication not set upServerNameMustContainOneHostNameResumptionAttemptedWithVariedEmsRefusedToFollowHelloRetryRequestIllegalMiddleboxChangeCipherSpecBadMaxFragmentSizeNoApplicationProtocolPeerSentOversizedRecordHandshakeNotCompleteFailedToGetRandomBytesFailedToGetCurrentTimeGeneralInvalidSctInvalidCertificateAlertReceivedPeerMisbehavedEncryptErrorDecryptErrorUnsupportedNameTypeNoCertificatesPresentedInvalidMessageInappropriateHandshakeMessageexpect_typesgot_typeInappropriateMessageUnsupportedKeyExchangeAlgorithmUnsupportedCurveTypeUnsupportedCompressionUnknownProtocolVersionUnexpectedMessageTrailingDataNoSignatureSchemesMissingKeyExchangeMissingDataMessageTooShortMessageTooLargeInvalidServerNameInvalidEmptyPayloadInvalidDhParamsInvalidCertRequestInvalidCertificateStatusTypeInvalidContentTypeInvalidCcsHandshakePayloadTooLargeWrongGroupForKeyShareUnsolicitedServerHelloExtensionUnsolicitedSctListUnsolicitedEncryptedExtensionUnsolicitedCertExtensionUnexpectedCleartextExtensionTooMuchEarlyDataReceivedSignedHandshakeWithUnadvertisedSigSchemeSignedKxWithWrongAlgorithmServerNameDifferedOnRetryServerHelloMustOfferUncompressedEcPointsSelectedUnusableCipherSuiteForVersionSelectedUnofferedPskSelectedUnofferedKxGroupSelectedUnofferedCompressionSelectedUnofferedCipherSuiteSelectedUnofferedApplicationProtocolSelectedTls12UsingTls13VersionExtensionSelectedInvalidPskSelectedDifferentCipherSuiteAfterRetryResumptionOfferedWithIncompatibleCipherSuiteResumptionOfferedWithVariedEmsResumptionOfferedWithVariedCipherSuiteRejectedEarlyDataInterleavedWithHandshakeMessagePskExtensionWithMismatchedIdsAndBindersPskExtensionMustBeLastOfferedIncorrectCompressionsOfferedEmptyApplicationProtocolOfferedEarlyDataWithOldProtocolVersionOfferedDuplicateKeySharesMissingQuicTransportParametersMissingKeyShareMissingBinderInPskExtensionMessageInterleavedWithHandshakeMessageKeyUpdateReceivedInQuicConnectionKeyEpochWithPendingFragmentInvalidSctListInvalidKeyShareInvalidMaxEarlyDataSizeIncorrectBinderIllegalTlsInnerPlaintextIllegalHelloRetryRequestWithUnsupportedVersionIllegalHelloRetryRequestWithUnofferedNamedGroupIllegalHelloRetryRequestWithUnofferedCipherSuiteIllegalHelloRetryRequestWithOfferedGroupIllegalHelloRetryRequestWithNoChangesIllegalHelloRetryRequestWithEmptyCookieHandshakeHashVariedAfterRetryEarlyDataOfferedWithVariedCipherSuiteEarlyDataExtensionWithoutResumptionEarlyDataAttemptedInSecondClientHelloDuplicateServerNameTypesDuplicateServerHelloExtensionsDuplicateNewSessionTicketExtensionsDuplicateHelloRetryRequestExtensionsDuplicateEncryptedExtensionsDuplicateClientHelloExtensionsDisallowedEncryptedExtensionBadCertChainExtensionsAttemptedDowngradeToTls12WhenTls13IsSupportedUncompressedEcPointsRequiredTls13RequiredForQuicTls12NotOfferedOrEnabledTls12NotOfferedSupportedVersionsExtensionRequiredSignatureAlgorithmsExtensionRequiredServerTlsVersionIsDisabledByOurConfigServerSentHelloRetryRequestWithUnknownExtensionServerDoesNotSupportTls12Or13NullCompressionRequiredNoSignatureSchemesInCommonNoKxGroupsInCommonNoEcPointFormatsInCommonNoCipherSuitesInCommonNoCertificateRequestSignatureSchemesInCommonNamedGroupsExtensionRequiredKeyShareExtensionRequiredEcPointsExtensionRequiredOtherApplicationVerificationFailureInvalidPurposeNotValidForNameBadSignatureUnknownIssuerUnhandledCriticalExtensionRevokedNotValidYetExpiredBadEncoding-
-invalid HTTP versiontoo many headersinvalid new lineInvalidChunkSizeinvalid tokeninvalid response statusinvalid header valueinvalid header namePOSTnamepathGET
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/httparse-1.8.0/src/lib.rsVersionTooManyHeadersTokenStatusNewLineHeaderValueHeaderName
-description() is deprecated; use Displaycannot advance past `remaining`:  <= varylinkhostfrometagdateVaryLinkHostFromEtagDate/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/bytes-1.4.0/src/bytes.rs
+called `Result::unwrap()` on an `Err` value/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/data-encoding-2.4.0/src/lib.rs
+attempt to divide by zero
+explicit panic
+$2?k:yy::Scy
+#%')+L/P37@BDFHJC
+ "$&(*,.02468:<>@BC
+ "$&(*,.02468:<>@B
+CCCCCCCCC
+CCCCCCCCC
+CCCCCCCCC
+ "CCCCCCCC$CCCCCCCCC&(CCCCCCCC*CCCCC,CCC.CCCCCCCCC0CCCCCCCC2468:<>@CCCB
+"%(+.36;>CFINQV[^cfkpuz
+#(-27<AFKPUd
+!$).149>CHO	
+Certificate
+UnknownNoApplicationProtocolCertificateRequiredUnknownPSKIdentityBadCertificateHashValueBadCertificateStatusResponseCertificateUnobtainableUnsupportedExtensionNoRenegotiationUserCanceledInappropriateFallbackInternalErrorInsufficientSecurityProtocolVersionExportRestrictionDecryptErrorDecodeErrorAccessDeniedUnknownCACertificateUnknownCertificateExpiredCertificateRevokedUnsupportedCertificateBadCertificateNoCertificateDecompressionFailureRecordOverflowBadRecordMacUnexpectedMessageCloseNotify
+MessageHashKeyUpdateCertificateStatusCertificateURLClientKeyExchangeCertificateVerifyServerHelloDoneCertificateRequestServerKeyExchangeEncryptedExtensionsHelloRetryRequestEndOfEarlyDataHelloVerifyRequestServerHelloClientHelloHelloRequest
+HeartbeatApplicationDataHandshakeAlert
+ECDHERSADHEDH
+!#%')+-/13579;=?ACEGIKMOQSUWY[]_
+ "$&(*,.02468:<>@BDFHI
+ "$&(*,.02468:<>@BDFH
+33333333333433333
+ "$&(*,.0333332
+"%*-036;@EJOTWZ_bejoruz
+ "$&(*,.02468:<>?
+ "$&(*,.02468:<>
+ "$&(*,.02468:<>@BD
+!$'*-0369<?BEHPSV\bhkq
+assertion failed: mid <= self.len()attempt to join into collection with len > usize::MAX/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/alloc/src/str.rs
+,36<?EP[fq|
+"'*/9<AKUX]d
+the supplied max_fragment_size was too small or largepeer doesn't support any known protocolpeer sent excess record sizehandshake not completefailed to get random bytesfailed to get current timeunexpected error: invalid certificate timestamp: invalid peer certificate: received fatal alert: peer misbehaved: peer is incompatible: cannot encrypt messagecannot decrypt peer's messagepresented server name type wasn't supportedpeer sent no certificatesreceived corrupt message of type received unexpected handshake message: got received unexpected message: got 
+BadMaxFragmentSizeNoApplicationProtocolPeerSentOversizedRecordHandshakeNotCompleteFailedToGetRandomBytesFailedToGetCurrentTimeGeneralInvalidSctInvalidCertificateAlertReceivedPeerMisbehavedEncryptErrorDecryptErrorUnsupportedNameTypeNoCertificatesPresentedInvalidMessageInappropriateHandshakeMessageexpect_typesInappropriateMessageUnsupportedKeyExchangeAlgorithmUnsupportedCurveTypeUnsupportedCompressionUnknownProtocolVersionUnexpectedMessageTrailingDataNoSignatureSchemesMissingKeyExchangeMissingDataMessageTooShortMessageTooLargeInvalidServerNameInvalidEmptyPayloadInvalidDhParamsInvalidCertRequestInvalidCertificateStatusTypeInvalidContentTypeInvalidCcsHandshakePayloadTooLargeWrongGroupForKeyShareUnsolicitedServerHelloExtensionUnsolicitedSctListUnsolicitedEncryptedExtensionUnsolicitedCertExtensionUnexpectedCleartextExtensionTooMuchEarlyDataReceivedSignedHandshakeWithUnadvertisedSigSchemeSignedKxWithWrongAlgorithmServerNameMustContainOneHostNameServerNameDifferedOnRetryServerHelloMustOfferUncompressedEcPointsSelectedUnusableCipherSuiteForVersionSelectedUnofferedPskSelectedUnofferedKxGroupSelectedUnofferedCompressionSelectedUnofferedCipherSuiteSelectedUnofferedApplicationProtocolSelectedTls12UsingTls13VersionExtensionSelectedInvalidPskSelectedDifferentCipherSuiteAfterRetryResumptionOfferedWithIncompatibleCipherSuiteResumptionOfferedWithVariedEmsResumptionOfferedWithVariedCipherSuiteResumptionAttemptedWithVariedEmsRejectedEarlyDataInterleavedWithHandshakeMessageRefusedToFollowHelloRetryRequestPskExtensionWithMismatchedIdsAndBindersPskExtensionMustBeLastOfferedIncorrectCompressionsOfferedEmptyApplicationProtocolOfferedEarlyDataWithOldProtocolVersionOfferedDuplicateKeySharesMissingQuicTransportParametersMissingPskModesExtensionMissingKeyShareMissingBinderInPskExtensionMessageInterleavedWithHandshakeMessageKeyUpdateReceivedInQuicConnectionKeyEpochWithPendingFragmentInvalidSctListInvalidKeyShareInvalidMaxEarlyDataSizeIncorrectBinderIllegalTlsInnerPlaintextIllegalMiddleboxChangeCipherSpecIllegalHelloRetryRequestWithUnsupportedVersionIllegalHelloRetryRequestWithUnofferedNamedGroupIllegalHelloRetryRequestWithUnofferedCipherSuiteIllegalHelloRetryRequestWithOfferedGroupIllegalHelloRetryRequestWithNoChangesIllegalHelloRetryRequestWithEmptyCookieHandshakeHashVariedAfterRetryEarlyDataOfferedWithVariedCipherSuiteEarlyDataExtensionWithoutResumptionEarlyDataAttemptedInSecondClientHelloDuplicateServerNameTypesDuplicateServerHelloExtensionsDuplicateNewSessionTicketExtensionsDuplicateHelloRetryRequestExtensionsDuplicateEncryptedExtensionsDuplicateClientHelloExtensionsDisallowedEncryptedExtensionBadCertChainExtensionsAttemptedDowngradeToTls12WhenTls13IsSupportedUncompressedEcPointsRequiredTls13RequiredForQuicTls12NotOfferedOrEnabledTls12NotOfferedSupportedVersionsExtensionRequiredSignatureAlgorithmsExtensionRequiredServerTlsVersionIsDisabledByOurConfigServerSentHelloRetryRequestWithUnknownExtensionServerDoesNotSupportTls12Or13NullCompressionRequiredNoSignatureSchemesInCommonNoKxGroupsInCommonNoEcPointFormatsInCommonNoCipherSuitesInCommonNoCertificateRequestSignatureSchemesInCommonNamedGroupsExtensionRequiredKeyShareExtensionRequiredEcPointsExtensionRequiredOtherApplicationVerificationFailureInvalidPurposeNotValidForNameBadSignatureUnknownIssuerUnhandledCriticalExtensionRevokedNotValidYetExpiredBadEncoding
+PeerIncompatibleInvalidKeyUpdate
+invalid HTTP versioninvalid tokeninvalid response statusinvalid header valueinvalid header name
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/httparse-1.8.0/src/lib.rsVersionTooManyHeadersTokenStatusNewLineHeaderValueHeaderName
+too many headersinvalid new linePOST
+description() is deprecated; use Display
+scheme too longempty stringuri too longpath missingauthority missingscheme missinginvalid formatinvalid portinvalid authorityinvalid schemeinvalid uri character
+InvalidUriInvalidUriPartsSchemeTooLongEmptyTooLongPathAndQueryMissingSchemeMissingInvalidFormatInvalidPortInvalidSchemeInvalidUriChar
+AuthorityMissingInvalidAuthority
+description() is deprecated; use Displaycannot advance past `remaining`: /Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/bytes-1.4.0/src/bytes.rs
 0123456789
 abcdefghijklmnopqrstuvwxyz
 ^_`abcdefghijklmnopqrstuvwxyz
-InvalidHeaderNameinvalid HTTP header nameStandardlocationif-rangeif-matchLocationx-xss-protectionwww-authenticatecontent-locationcontent-languagecontent-encodingTransferEncodingx-frame-optionsx-dns-prefetch-controlx-content-type-optionswarningviaupgrade-insecure-requestsupgradeuser-agenttransfer-encodingtrailertestrict-transport-securityset-cookieserversec-websocket-versionsec-websocket-protocolsec-websocket-keysec-websocket-extensionssec-websocket-acceptretry-afterrefreshreferrer-policyrefererrangepublic-key-pins-report-onlypublic-key-pinsproxy-authorizationproxy-authenticatepragmaoriginmax-forwardslast-modifiedif-unmodified-sinceif-none-matchif-modified-sinceforwardedexpiresexpectdntcookiecontent-typecontent-security-policy-report-onlycontent-security-policycontent-rangecontent-lengthcontent-dispositionconnectioncdn-cache-controlcache-statuscache-controlauthorizationalt-svcallowageaccess-control-request-methodaccess-control-request-headersaccess-control-max-ageaccess-control-expose-headersaccess-control-allow-originaccess-control-allow-methodsaccess-control-allow-headersaccess-control-allow-credentialsaccept-rangesaccept-languageaccept-encodingaccept-charsetaccept#
-description() is deprecated; use Displayscheme too longempty stringuri too longpath missingauthority missingscheme missinginvalid formatinvalid portinvalid authorityinvalid schemeinvalid uri characterInvalidUriInvalidUriPartsSchemeTooLongEmptyTooLongPathAndQueryMissingAuthorityMissingInvalidAuthoritySchemeMissingInvalidFormatInvalidPortInvalidSchemeInvalidUriChar
-/*description() is deprecated; use DisplayInvalidMethodinvalid HTTP method/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/http-0.2.9/src/uri/scheme.rs
+InvalidHeaderNameinvalid HTTP header name
+x-frame-optionsx-dns-prefetch-controlx-content-type-optionswarningviaupgrade-insecure-requestsupgradeuser-agenttransfer-encodingtrailertestrict-transport-securityset-cookieserversec-websocket-versionsec-websocket-protocolsec-websocket-keysec-websocket-extensionssec-websocket-acceptretry-afterrefreshreferrer-policyrefererrangepublic-key-pins-report-onlypublic-key-pinsproxy-authorizationproxy-authenticatepragmaoriginmax-forwardslast-modifiedif-unmodified-sinceif-none-matchif-modified-sinceforwardedexpiresexpectdntcookiecontent-typecontent-security-policy-report-onlycontent-security-policycontent-rangecontent-lengthcontent-dispositionconnectioncdn-cache-controlcache-statuscache-controlauthorizationalt-svcallowageaccess-control-request-methodaccess-control-request-headersaccess-control-max-ageaccess-control-expose-headersaccess-control-allow-originaccess-control-allow-methodsaccess-control-allow-headersaccess-control-allow-credentialsaccept-rangesaccept-languageaccept-encodingaccept-charsetaccept
+varylinketag
+if-rangeif-match
+x-xss-protectionwww-authenticatecontent-locationcontent-languagecontent-encodingdescription() is deprecated; use DisplayInvalidMethodinvalid HTTP method/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/http-0.2.9/src/uri/scheme.rs
 0123456789:
 ABCDEFGHIJKLMNOPQRSTUVWXYZ
 abcdefghijklmnopqrstuvwxyz
-internal error: entered unreachable code/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/http-0.2.9/src/version.rsHTTP/3.0HTTP/2.0HTTP/1.1HTTP/1.0HTTP/0.9http::Error$
+internal error: entered unreachable code/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/http-0.2.9/src/version.rsHTTP/3.0HTTP/2.0HTTP/1.1HTTP/1.0HTTP/0.9
+TX\`dhlptx|
+description() is deprecated; use Display
+ <unknown status code>InvalidStatusCodeinvalid status code
+Network Authentication RequiredNot ExtendedLoop DetectedInsufficient StorageVariant Also NegotiatesHTTP Version Not SupportedGateway TimeoutService UnavailableBad GatewayNot ImplementedInternal Server ErrorUnavailable For Legal ReasonsRequest Header Fields Too LargeToo Many RequestsPrecondition RequiredFailed DependencyLockedUnprocessable EntityMisdirected RequestI'm a teapotExpectation FailedRange Not SatisfiableUnsupported Media TypeURI Too LongPayload Too LargePrecondition FailedLength RequiredRequest TimeoutProxy Authentication RequiredNot AcceptableMethod Not AllowedNot FoundForbiddenUnauthorizedBad RequestPermanent RedirectTemporary RedirectUse ProxyNot ModifiedSee OtherFoundMoved PermanentlyIM UsedMulti-StatusPartial ContentReset ContentNo ContentNon Authoritative InformationCreatedOKProcessingSwitching Protocols
+Upgrade RequiredPayment RequiredMultiple ChoicesAlready ReportedGone
+Conflict$
 &'()*+,-./0123456789:;
 ?@ABCDEFGHIJKLMNOPQRSTUVWXYZ[
 abcdefghijklmnopqrstuvwxyz
-description() is deprecated; use DisplaySensitive"/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/http-0.2.9/src/header/value.rs\x\"InvalidHeaderValuefailed to parse header value
-TX\`dhlptx|
-description() is deprecated; use Display <unknown status code>InvalidStatusCodeinvalid status codeNetwork Authentication RequiredNot ExtendedLoop DetectedInsufficient StorageVariant Also NegotiatesHTTP Version Not SupportedGateway TimeoutService UnavailableBad GatewayNot ImplementedInternal Server ErrorUnavailable For Legal ReasonsRequest Header Fields Too LargeToo Many RequestsPrecondition RequiredUpgrade RequiredPayment RequiredMultiple ChoicesAlready ReportedFailed DependencyLockedUnprocessable EntityMisdirected RequestI'm a teapotExpectation FailedRange Not SatisfiableUnsupported Media TypeURI Too LongPayload Too LargePrecondition FailedLength RequiredGoneConflictAcceptedRequest TimeoutProxy Authentication RequiredNot AcceptableMethod Not AllowedNot FoundForbiddenUnauthorizedBad RequestPermanent RedirectTemporary RedirectUse ProxyNot ModifiedSee OtherFoundMoved PermanentlyIM UsedMulti-StatusPartial ContentReset ContentNo ContentNon Authoritative InformationCreatedOKProcessingSwitching Protocols
-$*06<BHNTZ`flrxa Display implementation returned an error unexpectedly/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/alloc/src/string.rsrecursion limit exceededunexpected end of hex escapetrailing characterstrailing commalone leading surrogate in hex escapekey must be a stringcontrol character (\u0000-\u001F) found while parsing a stringinvalid unicode code pointnumber out of rangeinvalid numberinvalid escapeexpected valueexpected identexpected `,` or `}`expected `,` or `]`expected `:`EOF while parsing a valueEOF while parsing a stringEOF while parsing an objectEOF while parsing a list column , line: Error(, column: )0123456789abcdefuuuuuuuubtnufruuuuuuuuuuuuuuuuuu
-failed to spawn thread/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/std/src/thread/mod.rsthread name may not contain interior null bytesfatal runtime error: 
-thread result panicked on drop
-/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/std/src/io/mod.rsfailed to write whole bufferformatter error
-called `Result::unwrap()` on an `Err` value/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/mproxy-reverse-0.1.7/src/lib.rs:reverse_proxy: error 
-forwarding UDP downstreamassertion failed: c == c_outgot message with size 0 from upstream: binding TCP socketdropping client: err: sending to UDP socketno addresses to send data tocould not resolve to any addresses
-called `Result::unwrap()` on an `Err` value/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/mproxy-forward-0.1.7/src/lib.rsResolving DNS for Performing handshakeConnecting to GET / HTTP/1.1
-Connection: close
-Accept-Encoding: identity
-could not resolve to any addressesdescription() is deprecated; use Display
-/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/std/src/io/mod.rsfailed to write whole buffer/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/mproxy-forward-0.1.7/src/lib.rs
+description() is deprecated; use DisplaySensitive"/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/http-0.2.9/src/header/value.rs\x\"InvalidHeaderValuefailed to parse header valuehttp::Error
+!#%')+-/13579;=?ACEGIKMOQSUWY[]
+$*06<BHNTZ`flrxa Display implementation returned an error unexpectedly/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/alloc/src/string.rs
+recursion limit exceededunexpected end of hex escapetrailing characterstrailing commalone leading surrogate in hex escapekey must be a stringcontrol character (\u0000-\u001F) found while parsing a stringinvalid unicode code pointnumber out of rangeinvalid numberinvalid escapeexpected valueexpected identexpected `,` or `}`expected `,` or `]`expected `:`EOF while parsing a valueEOF while parsing a stringEOF while parsing an objectEOF while parsing a list
+Error(, column: )
+0123456789abcdefuuuuuuuubtnufruuuuuuuuuuuuuuuuuu
+failed to spawn thread/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/std/src/thread/mod.rsthread name may not contain interior null bytes
+fatal runtime error: thread result panicked on drop
+no addresses to send data to
+called `Result::unwrap()` on an `Err` value
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/mproxy-reverse-0.1.7/src/lib.rs:reverse_proxy: error 
+forwarding UDP downstreamassertion failed: c == c_outgot message with size 0 from upstream: binding TCP socketdropping client: err: sending to UDP socket
+!#%')+-/13579;=?ACEGIKMOQSUWY[]_/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/std/src/io/mod.rsfailed to write whole bufferformatter errorcould not resolve to any addresses
+could not resolve to any addresses
+description() is deprecated; use Display
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/mproxy-forward-0.1.7/src/lib.rs
 Retrying...
 err: sending to UDP socketencountered EOF, disconnecting TCP proxy thread...
-failed to spawn thread/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/std/src/thread/mod.rsthread name may not contain interior null bytes
-fatal runtime error: 
-thread result panicked on drop
-/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/std/src/io/mod.rsfailed to write whole bufferformatter errorno addresses to send data to
- "$&(.49;=?EJTVXZ\^!+%
-illegal middlebox CCS receivedDropping CCSrustls::conn/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/conn.rsreceived plaintext buffer full
-/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/std/src/io/mod.rsstream did not contain valid UTF-8/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/std/src/io/readbuf.rsfailed to fill whole buffer
-failed to fill bufferfailed to write whole buffer/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/std/src/io/mod.rsformatter error
-advancing io slices beyond their lengthadvancing IoSlice beyond its length/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/std/src/sys/unix/io.rs1
+!#%')+-/13579;=?ACEGIKMOQSUWY[]_/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/std/src/io/mod.rsfailed to write whole buffer
+!#%')+-/13579;=?ACEGIKMOQSUWY[]_/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/std/src/io/mod.rsfailed to write whole bufferformatter errorno addresses to send data to
+$2?k:yy::Scy
+#%')+4=ACEGPT]_aceg
+4BP8<LR(&Z
+illegal middlebox CCS receivedDropping CCSrustls::conn/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/conn.rsreceived plaintext buffer full
+failed to spawn thread/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/std/src/thread/mod.rsthread name may not contain interior null bytes
+fatal runtime error: thread result panicked on drop
+!#%')+-/13579;=?ACEGIKMOQSUWY[]_
+!#%')+-/13579;=?ACEGIKMOQSUWY[]_aceg/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/std/src/io/mod.rsstream did not contain valid UTF-8failed to fill whole buffer/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/std/src/io/readbuf.rs
+called `Result::unwrap()` on an `Err` value
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/mproxy-forward-0.1.7/src/lib.rsResolving DNS for Performing handshakeConnecting to GET / HTTP/1.1
+Connection: close
+Accept-Encoding: identity
+4BP8<LR(&Z
+!#%')+-/13579;=?ACEGIKMOQSUWY[]_
+!#%')+-/13579;=?ACEGIKMOQSUWY[]_failed to fill bufferfailed to write whole buffer/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/std/src/io/mod.rsformatter error
+advancing IoSlice beyond its length/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/std/src/sys/unix/io.rsadvancing io slices beyond their length1
 DigiCert, Inc.1&0$
 DigiCert TLS ECC P384 Root G50
 Entrust, Inc.1(0&
 See www.entrust.net/legal-terms1907
 0(c) 2012 Entrust, Inc. - for authorized use only1301
 *Entrust Root Certification Authority - EC10
 AffirmTrust1
@@ -673,27 +715,27 @@
 Athens1D0B
 ;Hellenic Academic and Research Institutions Cert. Authority1D0B
 ;Hellenic Academic and Research Institutions ECC RootCA 20150
 Arizona1
 Scottsdale1
 GoDaddy.com, Inc.110/
 (Go Daddy Root Certificate Authority - G20
+Gebze - Kocaeli1B0@
+9Turkiye Bilimsel ve Teknolojik Arastirma Kurumu - TUBITAK1-0+
+$Kamu Sertifikasyon Merkezi - Kamu SM1604
+-TUBITAK Kamu SM SSL Kok Sertifikasi - Surum 10
 .gov.tr0	
 .k12.tr0	
 .pol.tr0	
 .mil.tr0	
 .tsk.tr0	
 .kep.tr0	
 .bel.tr0	
 .edu.tr0	
 .org.tr1
-Gebze - Kocaeli1B0@
-9Turkiye Bilimsel ve Teknolojik Arastirma Kurumu - TUBITAK1-0+
-$Kamu Sertifikasyon Merkezi - Kamu SM1604
--TUBITAK Kamu SM SSL Kok Sertifikasi - Surum 10
 D-Trust GmbH1'0%
 D-TRUST Root Class 3 CA 2 20090
 GlobalSign nv-sa1
 GlobalSign Root R460
 New Jersey1
 Jersey City1
 The USERTRUST Network1.0,
@@ -940,108 +982,158 @@
 ANF Secure Server Root CA0
 "T-Systems Enterprise Services GmbH1
 T-Systems Trust Center1%0#
 T-TeleSec GlobalRoot Class 30
 Asseco Data Systems S.A.1'0%
 Certum Certification Authority1
 Certum Trusted Root CA0
-invalid dns nameClientConnectionOwnedTrustAnchorname_constraintsChacha20Poly1305AcceptedFinishedversionsRejectedAcceptedDisabled
-%%%%%%%%
-5%%9%%%%%%%%%%%%%%%%%%%%
-internal error: entered unreachable codea Display implementation returned an error unexpectedly/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/alloc/src/string.rs
-bulkLazy instance has previously been poisoned/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/once_cell-1.18.0/src/lib.rsb"\\x\0\t\r\n"
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/client/client_conn.rsEarlyData rejectedrustls::client::client_connEarlyData accepted
-EarlyData finishedbad EarlyData stateIpAddressDnsNameReady
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/msgs/codec.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/msgs/deframer.rsmessage buffer fullReceived a  message while expecting rustls::check/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/check.rs handshake message while expecting Unsolicited extension rustls::client::common/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/client/common.rsClient auth requested but no cert/sigscheme availableAttempting client auth
-Resuming sessionfinishedexporterGot HRR 
-called `Result::unwrap()` on an `Err` valuederivedres masterexp masters ap trafficc ap traffics hs trafficc hs trafficc e trafficres binderEXPORTER_SECRETSERVER_TRAFFIC_SECRET_0CLIENT_TRAFFIC_SECRET_0SERVER_HANDSHAKE_TRAFFIC_SECRETCLIENT_HANDSHAKE_TRAFFIC_SECRETCLIENT_EARLY_TRAFFIC_SECRET/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/digest.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/tls13/key_schedule.rsnot a loggable secrettraffic updresumptionexporting too muchtls13 keyiv/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/client/hs.rsNo cached session for rustls::client::hsNot resuming any sessionassertion failed: !supported_versions.is_empty()Sending ClientHello server sent non-offered ALPN protocolALPN protocol is 
-We got ServerHello server chose v1.2 when offering 0-rttserver chose v1.2 using v1.3 extension
-server chose non-Null compressionserver sent duplicate extensionsserver sent unsolicited extensionserver does not support uncompressed pointsserver chose unusable ciphersuite for versionserver varied selected ciphersuiteUsing ciphersuite called `Option::unwrap()` on a `None` valueserver does not support TLS v1.2/v1.3server's TLS version is disabled in clientserver chose non-offered ciphersuite
-server requested hrr with our groupserver requested hrr with empty cookieserver sent hrr with unhandled extensionserver send duplicate hrr extensionsserver requested hrr with no changesserver requested unsupported version in hrrserver requested unsupported cs in hrrserver requested hrr with bad group
-/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/alloc/src/slice.rs
-Tls13CipherSuite
-/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/std/src/io/impls.rs
-called `Result::unwrap()` on an `Err` value/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/cipher.rsencrypt not yet available/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/record_layer.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/tls13/key_schedule.rsencrypt failedpeer sent bad TLSInnerPlaintextkey agreement failedChangeCipherSpecPayload
-RSA_PKCS1_SHA512RSA_PKCS1_SHA384RSA_PKCS1_SHA256DTLSv1_3DTLSv1_2DTLSv1_0
-$*06<BHN
-rustls::conn/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/conn.rskey epoch or handshake flight with pending fragmentDropping undecryptable message after aborted early_dataSending warning alert TLS alert warning received: TLS alert received: Sending fatal alert TLSv1_3TLSv1_2TLSv1_1TLSv1_0SSLv3SSLv2UnknownSSL_RSA_FIPS_WITH_3DES_EDE_CBC_SHASSL_RSA_FIPS_WITH_DES_CBC_SHATLS_RSA_PSK_WITH_CHACHA20_POLY1305_SHA256TLS_DHE_PSK_WITH_CHACHA20_POLY1305_SHA256TLS_ECDHE_PSK_WITH_CHACHA20_POLY1305_SHA256TLS_PSK_WITH_CHACHA20_POLY1305_SHA256TLS_DHE_RSA_WITH_CHACHA20_POLY1305_SHA256TLS_ECDHE_ECDSA_WITH_CHACHA20_POLY1305_SHA256TLS_ECDHE_RSA_WITH_CHACHA20_POLY1305_SHA256TLS_ECDHE_ECDSA_WITH_AES_256_CCM_8TLS_ECDHE_ECDSA_WITH_AES_128_CCM_8TLS_ECDHE_ECDSA_WITH_AES_256_CCMTLS_ECDHE_ECDSA_WITH_AES_128_CCMTLS_PSK_WITH_ARIA_256_GCM_SHA384TLS_PSK_WITH_ARIA_128_GCM_SHA256TLS_PSK_WITH_ARIA_256_CBC_SHA384TLS_PSK_WITH_ARIA_128_CBC_SHA256TLS_RSA_WITH_ARIA_256_GCM_SHA384TLS_RSA_WITH_ARIA_128_GCM_SHA256TLS_RSA_WITH_ARIA_256_CBC_SHA384TLS_RSA_WITH_ARIA_128_CBC_SHA256TLS_SRP_SHA_WITH_AES_256_CBC_SHATLS_SRP_SHA_WITH_AES_128_CBC_SHATLS_ECDHE_ECDSA_WITH_RC4_128_SHATLS_RSA_PSK_WITH_AES_256_CBC_SHATLS_RSA_PSK_WITH_AES_128_CBC_SHATLS_DHE_PSK_WITH_AES_256_CBC_SHATLS_DHE_PSK_WITH_AES_128_CBC_SHATLS_DHE_RSA_WITH_AES_256_CBC_RMDTLS_DHE_RSA_WITH_AES_128_CBC_RMDTLS_DHE_DSS_WITH_AES_256_CBC_RMDTLS_DHE_DSS_WITH_AES_128_CBC_RMDTLS_DH_anon_WITH_AES_256_CBC_SHATLS_DHE_RSA_WITH_AES_256_CBC_SHATLS_DHE_DSS_WITH_AES_256_CBC_SHATLS_DH_anon_WITH_AES_128_CBC_SHATLS_DHE_RSA_WITH_AES_128_CBC_SHATLS_DHE_DSS_WITH_AES_128_CBC_SHATLS_DH_RSA_WITH_3DES_EDE_CBC_SHATLS_DH_DSS_WITH_3DES_EDE_CBC_SHATLS_PSK_DHE_WITH_AES_256_CCM_8TLS_PSK_DHE_WITH_AES_128_CCM_8TLS_PSK_WITH_AES_256_CCM_8TLS_PSK_WITH_AES_128_CCM_8TLS_DHE_PSK_WITH_AES_256_CCMTLS_DHE_PSK_WITH_AES_128_CCMTLS_PSK_WITH_AES_256_CCMTLS_PSK_WITH_AES_128_CCMTLS_DHE_RSA_WITH_AES_256_CCM_8TLS_DHE_RSA_WITH_AES_128_CCM_8TLS_RSA_WITH_AES_256_CCM_8TLS_RSA_WITH_AES_128_CCM_8TLS_DHE_RSA_WITH_AES_256_CCMTLS_DHE_RSA_WITH_AES_128_CCMTLS_RSA_WITH_AES_256_CCMTLS_RSA_WITH_AES_128_CCMTLS_ECDHE_PSK_WITH_CAMELLIA_256_CBC_SHA384TLS_ECDHE_PSK_WITH_CAMELLIA_128_CBC_SHA256TLS_RSA_PSK_WITH_CAMELLIA_256_CBC_SHA384TLS_RSA_PSK_WITH_CAMELLIA_128_CBC_SHA256TLS_DHE_PSK_WITH_CAMELLIA_256_CBC_SHA384TLS_DHE_PSK_WITH_CAMELLIA_128_CBC_SHA256TLS_PSK_WITH_CAMELLIA_256_CBC_SHA384TLS_PSK_WITH_CAMELLIA_128_CBC_SHA256TLS_RSA_PSK_WITH_CAMELLIA_256_GCM_SHA384TLS_RSA_PSK_WITH_CAMELLIA_128_GCM_SHA256TLS_DHE_PSK_WITH_CAMELLIA_256_GCM_SHA384TLS_DHE_PSK_WITH_CAMELLIA_128_GCM_SHA256TLS_PSK_WITH_CAMELLIA_256_GCM_SHA384TLS_PSK_WITH_CAMELLIA_128_GCM_SHA256TLS_ECDH_RSA_WITH_CAMELLIA_256_GCM_SHA384TLS_ECDH_RSA_WITH_CAMELLIA_128_GCM_SHA256TLS_ECDHE_RSA_WITH_CAMELLIA_256_GCM_SHA384TLS_ECDHE_RSA_WITH_CAMELLIA_128_GCM_SHA256TLS_ECDH_ECDSA_WITH_CAMELLIA_256_GCM_SHA384TLS_ECDH_ECDSA_WITH_CAMELLIA_128_GCM_SHA256TLS_ECDHE_ECDSA_WITH_CAMELLIA_256_GCM_SHA384TLS_ECDHE_ECDSA_WITH_CAMELLIA_128_GCM_SHA256TLS_DH_anon_WITH_CAMELLIA_256_GCM_SHA384TLS_DH_anon_WITH_CAMELLIA_128_GCM_SHA256TLS_DH_DSS_WITH_CAMELLIA_256_GCM_SHA384TLS_DH_DSS_WITH_CAMELLIA_128_GCM_SHA256TLS_DHE_DSS_WITH_CAMELLIA_256_GCM_SHA384TLS_DHE_DSS_WITH_CAMELLIA_128_GCM_SHA256TLS_DH_RSA_WITH_CAMELLIA_256_GCM_SHA384TLS_DH_RSA_WITH_CAMELLIA_128_GCM_SHA256TLS_DHE_RSA_WITH_CAMELLIA_256_GCM_SHA384TLS_DHE_RSA_WITH_CAMELLIA_128_GCM_SHA256TLS_RSA_WITH_CAMELLIA_256_GCM_SHA384TLS_RSA_WITH_CAMELLIA_128_GCM_SHA256TLS_ECDH_RSA_WITH_CAMELLIA_256_CBC_SHA384TLS_ECDH_RSA_WITH_CAMELLIA_128_CBC_SHA256TLS_ECDHE_RSA_WITH_CAMELLIA_256_CBC_SHA384TLS_ECDHE_RSA_WITH_CAMELLIA_128_CBC_SHA256TLS_ECDH_ECDSA_WITH_CAMELLIA_256_CBC_SHA384TLS_ECDH_ECDSA_WITH_CAMELLIA_128_CBC_SHA256TLS_ECDHE_ECDSA_WITH_CAMELLIA_256_CBC_SHA384TLS_ECDHE_ECDSA_WITH_CAMELLIA_128_CBC_SHA256TLS_ECDHE_PSK_WITH_ARIA_256_CBC_SHA384TLS_ECDHE_PSK_WITH_ARIA_128_CBC_SHA256TLS_RSA_PSK_WITH_ARIA_256_GCM_SHA384TLS_RSA_PSK_WITH_ARIA_128_GCM_SHA256TLS_DHE_PSK_WITH_ARIA_256_GCM_SHA384TLS_DHE_PSK_WITH_ARIA_128_GCM_SHA256TLS_RSA_PSK_WITH_ARIA_256_CBC_SHA384TLS_RSA_PSK_WITH_ARIA_128_CBC_SHA256TLS_DHE_PSK_WITH_ARIA_256_CBC_SHA384TLS_DHE_PSK_WITH_ARIA_128_CBC_SHA256TLS_ECDH_RSA_WITH_ARIA_256_GCM_SHA384TLS_ECDH_RSA_WITH_ARIA_128_GCM_SHA256TLS_ECDHE_RSA_WITH_ARIA_256_GCM_SHA384TLS_ECDHE_RSA_WITH_ARIA_128_GCM_SHA256TLS_ECDH_ECDSA_WITH_ARIA_256_GCM_SHA384TLS_ECDH_ECDSA_WITH_ARIA_128_GCM_SHA256TLS_ECDHE_ECDSA_WITH_ARIA_256_GCM_SHA384TLS_ECDHE_ECDSA_WITH_ARIA_128_GCM_SHA256TLS_DH_anon_WITH_ARIA_256_GCM_SHA384TLS_DH_anon_WITH_ARIA_128_GCM_SHA256TLS_DH_DSS_WITH_ARIA_256_GCM_SHA384TLS_DH_DSS_WITH_ARIA_128_GCM_SHA256TLS_DHE_DSS_WITH_ARIA_256_GCM_SHA384TLS_DHE_DSS_WITH_ARIA_128_GCM_SHA256TLS_DH_RSA_WITH_ARIA_256_GCM_SHA384TLS_DH_RSA_WITH_ARIA_128_GCM_SHA256TLS_DHE_RSA_WITH_ARIA_256_GCM_SHA384TLS_DHE_RSA_WITH_ARIA_128_GCM_SHA256TLS_ECDH_RSA_WITH_ARIA_256_CBC_SHA384TLS_ECDH_RSA_WITH_ARIA_128_CBC_SHA256TLS_ECDHE_RSA_WITH_ARIA_256_CBC_SHA384TLS_ECDHE_RSA_WITH_ARIA_128_CBC_SHA256TLS_ECDH_ECDSA_WITH_ARIA_256_CBC_SHA384TLS_ECDH_ECDSA_WITH_ARIA_128_CBC_SHA256TLS_ECDHE_ECDSA_WITH_ARIA_256_CBC_SHA384TLS_ECDHE_ECDSA_WITH_ARIA_128_CBC_SHA256TLS_DH_anon_WITH_ARIA_256_CBC_SHA384TLS_DH_anon_WITH_ARIA_128_CBC_SHA256TLS_DHE_RSA_WITH_ARIA_256_CBC_SHA384TLS_DHE_RSA_WITH_ARIA_128_CBC_SHA256TLS_DHE_DSS_WITH_ARIA_256_CBC_SHA384TLS_DHE_DSS_WITH_ARIA_128_CBC_SHA256TLS_DH_RSA_WITH_ARIA_256_CBC_SHA384TLS_DH_RSA_WITH_ARIA_128_CBC_SHA256TLS_DH_DSS_WITH_ARIA_256_CBC_SHA384TLS_DH_DSS_WITH_ARIA_128_CBC_SHA256TLS_ECDHE_PSK_WITH_NULL_SHA384TLS_ECDHE_PSK_WITH_NULL_SHA256TLS_ECDHE_PSK_WITH_NULL_SHATLS_ECDHE_PSK_WITH_AES_256_CBC_SHA384TLS_ECDHE_PSK_WITH_AES_128_CBC_SHA256TLS_ECDHE_PSK_WITH_AES_256_CBC_SHATLS_ECDHE_PSK_WITH_AES_128_CBC_SHATLS_ECDHE_PSK_WITH_3DES_EDE_CBC_SHATLS_ECDHE_PSK_WITH_RC4_128_SHATLS_ECDH_RSA_WITH_AES_256_GCM_SHA384TLS_ECDH_RSA_WITH_AES_128_GCM_SHA256TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384TLS_ECDHE_RSA_WITH_AES_128_GCM_SHA256TLS_ECDH_ECDSA_WITH_AES_256_GCM_SHA384TLS_ECDH_ECDSA_WITH_AES_128_GCM_SHA256TLS_ECDHE_ECDSA_WITH_AES_256_GCM_SHA384TLS_ECDHE_ECDSA_WITH_AES_128_GCM_SHA256TLS_ECDH_RSA_WITH_AES_256_CBC_SHA384TLS_ECDH_RSA_WITH_AES_128_CBC_SHA256TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA384TLS_ECDHE_RSA_WITH_AES_128_CBC_SHA256TLS_ECDH_ECDSA_WITH_AES_256_CBC_SHA384TLS_ECDH_ECDSA_WITH_AES_128_CBC_SHA256TLS_ECDHE_ECDSA_WITH_AES_256_CBC_SHA384TLS_ECDHE_ECDSA_WITH_AES_128_CBC_SHA256TLS_SRP_SHA_DSS_WITH_AES_256_CBC_SHATLS_SRP_SHA_RSA_WITH_AES_256_CBC_SHATLS_SRP_SHA_DSS_WITH_AES_128_CBC_SHATLS_SRP_SHA_RSA_WITH_AES_128_CBC_SHATLS_SRP_SHA_DSS_WITH_3DES_EDE_CBC_SHATLS_SRP_SHA_RSA_WITH_3DES_EDE_CBC_SHATLS_SRP_SHA_WITH_3DES_EDE_CBC_SHATLS_ECDH_anon_WITH_AES_256_CBC_SHATLS_ECDH_anon_WITH_AES_128_CBC_SHATLS_ECDH_anon_WITH_3DES_EDE_CBC_SHATLS_ECDH_anon_WITH_RC4_128_SHATLS_ECDH_anon_WITH_NULL_SHATLS_ECDHE_RSA_WITH_AES_256_CBC_SHATLS_ECDHE_RSA_WITH_AES_128_CBC_SHATLS_ECDHE_RSA_WITH_3DES_EDE_CBC_SHATLS_ECDHE_RSA_WITH_RC4_128_SHATLS_ECDHE_RSA_WITH_NULL_SHATLS_ECDH_RSA_WITH_AES_256_CBC_SHATLS_ECDH_RSA_WITH_AES_128_CBC_SHATLS_ECDH_RSA_WITH_3DES_EDE_CBC_SHATLS_ECDH_RSA_WITH_RC4_128_SHATLS_ECDH_RSA_WITH_NULL_SHATLS_ECDHE_ECDSA_WITH_AES_256_CBC_SHATLS_ECDHE_ECDSA_WITH_AES_128_CBC_SHATLS_ECDHE_ECDSA_WITH_3DES_EDE_CBC_SHATLS_ECDHE_ECDSA_WITH_NULL_SHATLS_ECDH_ECDSA_WITH_AES_256_CBC_SHATLS_ECDH_ECDSA_WITH_AES_128_CBC_SHATLS_ECDH_ECDSA_WITH_3DES_EDE_CBC_SHATLS_ECDH_ECDSA_WITH_RC4_128_SHATLS_ECDH_ECDSA_WITH_NULL_SHATLS13_AES_128_CCM_8_SHA256TLS13_AES_128_CCM_SHA256TLS13_CHACHA20_POLY1305_SHA256TLS13_AES_256_GCM_SHA384TLS13_AES_128_GCM_SHA256TLS_EMPTY_RENEGOTIATION_INFO_SCSVTLS_DH_anon_WITH_CAMELLIA_256_CBC_SHA256TLS_DHE_RSA_WITH_CAMELLIA_256_CBC_SHA256TLS_DHE_DSS_WITH_CAMELLIA_256_CBC_SHA256TLS_DH_RSA_WITH_CAMELLIA_256_CBC_SHA256TLS_DH_DSS_WITH_CAMELLIA_256_CBC_SHA256TLS_RSA_WITH_CAMELLIA_256_CBC_SHA256TLS_DH_anon_WITH_CAMELLIA_128_CBC_SHA256TLS_DHE_RSA_WITH_CAMELLIA_128_CBC_SHA256TLS_DHE_DSS_WITH_CAMELLIA_128_CBC_SHA256TLS_DH_RSA_WITH_CAMELLIA_128_CBC_SHA256TLS_DH_DSS_WITH_CAMELLIA_128_CBC_SHA256TLS_RSA_WITH_CAMELLIA_128_CBC_SHA256TLS_RSA_PSK_WITH_NULL_SHA384TLS_RSA_PSK_WITH_NULL_SHA256TLS_RSA_PSK_WITH_AES_256_CBC_SHA384TLS_RSA_PSK_WITH_AES_128_CBC_SHA256TLS_DHE_PSK_WITH_NULL_SHA384TLS_DHE_PSK_WITH_NULL_SHA256TLS_DHE_PSK_WITH_AES_256_CBC_SHA384TLS_DHE_PSK_WITH_AES_128_CBC_SHA256TLS_PSK_WITH_NULL_SHA384TLS_PSK_WITH_NULL_SHA256TLS_PSK_WITH_AES_256_CBC_SHA384TLS_PSK_WITH_AES_128_CBC_SHA256TLS_RSA_PSK_WITH_AES_256_GCM_SHA384TLS_RSA_PSK_WITH_AES_128_GCM_SHA256TLS_DHE_PSK_WITH_AES_256_GCM_SHA384TLS_DHE_PSK_WITH_AES_128_GCM_SHA256TLS_PSK_WITH_AES_256_GCM_SHA384TLS_PSK_WITH_AES_128_GCM_SHA256TLS_DH_anon_WITH_AES_256_GCM_SHA384TLS_DH_anon_WITH_AES_128_GCM_SHA256TLS_DH_DSS_WITH_AES_256_GCM_SHA384TLS_DH_DSS_WITH_AES_128_GCM_SHA256TLS_DHE_DSS_WITH_AES_256_GCM_SHA384TLS_DHE_DSS_WITH_AES_128_GCM_SHA256TLS_DH_RSA_WITH_AES_256_GCM_SHA384TLS_DH_RSA_WITH_AES_128_GCM_SHA256TLS_DHE_RSA_WITH_AES_256_GCM_SHA384TLS_DHE_RSA_WITH_AES_128_GCM_SHA256TLS_RSA_WITH_AES_256_GCM_SHA384TLS_RSA_WITH_AES_128_GCM_SHA256TLS_DH_anon_WITH_SEED_CBC_SHATLS_DHE_RSA_WITH_SEED_CBC_SHATLS_DHE_DSS_WITH_SEED_CBC_SHATLS_DH_RSA_WITH_SEED_CBC_SHATLS_DH_DSS_WITH_SEED_CBC_SHATLS_RSA_WITH_SEED_CBC_SHATLS_RSA_PSK_WITH_3DES_EDE_CBC_SHATLS_RSA_PSK_WITH_RC4_128_SHATLS_DHE_PSK_WITH_3DES_EDE_CBC_SHATLS_DHE_PSK_WITH_RC4_128_SHATLS_PSK_WITH_AES_256_CBC_SHATLS_PSK_WITH_AES_128_CBC_SHATLS_PSK_WITH_3DES_EDE_CBC_SHATLS_PSK_WITH_RC4_128_SHATLS_DH_anon_WITH_CAMELLIA_256_CBC_SHATLS_DHE_RSA_WITH_CAMELLIA_256_CBC_SHATLS_DHE_DSS_WITH_CAMELLIA_256_CBC_SHATLS_DH_RSA_WITH_CAMELLIA_256_CBC_SHATLS_DH_DSS_WITH_CAMELLIA_256_CBC_SHATLS_RSA_WITH_CAMELLIA_256_CBC_SHATLS_GOSTR341001_WITH_NULL_GOSTR3411TLS_GOSTR341094_WITH_NULL_GOSTR3411TLS_GOSTR341001_WITH_28147_CNT_IMITTLS_GOSTR341094_WITH_28147_CNT_IMITTLS_RSA_WITH_AES_256_CBC_RMDTLS_RSA_WITH_AES_128_CBC_RMDTLS_RSA_WITH_3DES_EDE_CBC_RMDTLS_DHE_RSA_WITH_3DES_EDE_CBC_RMDTLS_DHE_DSS_WITH_3DES_EDE_CBC_RMDTLS_DH_anon_WITH_AES_256_CBC_SHA256TLS_DH_anon_WITH_AES_128_CBC_SHA256TLS_DHE_RSA_WITH_AES_256_CBC_SHA256TLS_DHE_DSS_WITH_AES_256_CBC_SHA256TLS_DH_RSA_WITH_AES_256_CBC_SHA256TLS_DH_DSS_WITH_AES_256_CBC_SHA256TLS_DHE_RSA_WITH_AES_128_CBC_SHA256TLS_DHE_DSS_WITH_RC4_128_SHATLS_DHE_DSS_EXPORT1024_WITH_RC4_56_SHATLS_RSA_EXPORT1024_WITH_RC4_56_SHATLS_DHE_DSS_EXPORT1024_WITH_DES_CBC_SHATLS_RSA_EXPORT1024_WITH_DES_CBC_SHATLS_RSA_EXPORT1024_WITH_RC2_CBC_56_MD5TLS_RSA_EXPORT1024_WITH_RC4_56_MD5TLS_ECDH_anon_EXPORT_WITH_RC4_40_SHA_draftTLS_ECDH_anon_EXPORT_WITH_DES40_CBC_SHA_draftTLS_ECDH_anon_WITH_3DES_EDE_CBC_SHA_draftTLS_ECDH_anon_WITH_DES_CBC_SHA_draftTLS_ECDH_anon_WITH_RC4_128_SHA_draftTLS_ECDH_anon_NULL_WITH_SHA_draftTLS_ECMQV_ECNRA_WITH_3DES_EDE_CBC_SHA_draftTLS_ECMQV_ECNRA_WITH_DES_CBC_SHA_draftTLS_ECMQV_ECNRA_WITH_RC4_128_SHA_draftTLS_ECMQV_ECNRA_NULL_SHA_draftTLS_ECMQV_ECDSA_WITH_3DES_EDE_CBC_SHA_draftTLS_ECMQV_ECDSA_WITH_DES_CBC_SHA_draftTLS_ECMQV_ECDSA_WITH_RC4_128_SHA_draftTLS_ECMQV_ECDSA_NULL_SHA_draftTLS_ECDH_ECNRA_WITH_3DES_EDE_CBC_SHA_draftTLS_ECDH_ECNRA_WITH_DES_CBC_SHA_draftTLS_ECDH_ECDSA_WITH_AES_256_CBC_SHA_draftTLS_ECDH_ECDSA_WITH_AES_128_CBC_SHA_draftTLS_ECDH_ECDSA_WITH_3DES_EDE_CBC_SHA_draftTLS_ECDH_ECDSA_WITH_DES_CBC_SHA_draftTLS_ECDH_ECDSA_WITH_RC4_128_SHA_draftTLS_ECDH_ECDSA_WITH_NULL_SHA_draftTLS_DH_anon_WITH_CAMELLIA_128_CBC_SHATLS_DHE_RSA_WITH_CAMELLIA_128_CBC_SHATLS_DHE_DSS_WITH_CAMELLIA_128_CBC_SHATLS_DH_RSA_WITH_CAMELLIA_128_CBC_SHATLS_DH_DSS_WITH_CAMELLIA_128_CBC_SHATLS_RSA_WITH_CAMELLIA_128_CBC_SHATLS_DHE_DSS_WITH_AES_128_CBC_SHA256TLS_DH_RSA_WITH_AES_128_CBC_SHA256TLS_DH_DSS_WITH_AES_128_CBC_SHA256TLS_RSA_WITH_AES_256_CBC_SHA256TLS_RSA_WITH_AES_128_CBC_SHA256TLS_RSA_WITH_NULL_SHA256TLS_DH_RSA_WITH_AES_256_CBC_SHATLS_DH_DSS_WITH_AES_256_CBC_SHATLS_RSA_WITH_AES_256_CBC_SHATLS_DH_RSA_WITH_AES_128_CBC_SHATLS_DH_DSS_WITH_AES_128_CBC_SHATLS_RSA_WITH_AES_128_CBC_SHATLS_RSA_PSK_WITH_NULL_SHATLS_DHE_PSK_WITH_NULL_SHATLS_PSK_WITH_NULL_SHATLS_KRB5_EXPORT_WITH_RC4_40_MD5TLS_KRB5_EXPORT_WITH_RC2_CBC_40_MD5TLS_KRB5_EXPORT_WITH_DES_CBC_40_MD5TLS_KRB5_EXPORT_WITH_RC4_40_SHATLS_KRB5_EXPORT_WITH_RC2_CBC_40_SHATLS_KRB5_EXPORT_WITH_DES_CBC_40_SHATLS_KRB5_WITH_IDEA_CBC_MD5TLS_KRB5_WITH_RC4_128_MD5TLS_KRB5_WITH_3DES_EDE_CBC_MD5TLS_KRB5_WITH_DES_CBC_MD5TLS_KRB5_WITH_IDEA_CBC_SHATLS_KRB5_WITH_RC4_128_SHATLS_KRB5_WITH_3DES_EDE_CBC_SHATLS_KRB5_WITH_DES_CBC_SHA_or_SSL_FORTEZZA_KEA_WITH_RC4_128_SHASSL_FORTEZZA_KEA_WITH_FORTEZZA_CBC_SHASSL_FORTEZZA_KEA_WITH_NULL_SHATLS_DH_anon_WITH_3DES_EDE_CBC_SHATLS_DH_anon_WITH_DES_CBC_SHATLS_DH_anon_EXPORT_WITH_DES40_CBC_SHATLS_DH_anon_WITH_RC4_128_MD5TLS_DH_anon_EXPORT_WITH_RC4_40_MD5TLS_DHE_RSA_WITH_3DES_EDE_CBC_SHATLS_DHE_RSA_WITH_DES_CBC_SHATLS_DHE_RSA_EXPORT_WITH_DES40_CBC_SHATLS_DHE_DSS_WITH_3DES_EDE_CBC_SHATLS_DHE_DSS_WITH_DES_CBC_SHATLS_DHE_DSS_EXPORT_WITH_DES40_CBC_SHATLS_DH_RSA_WITH_DES_CBC_SHATLS_DH_RSA_EXPORT_WITH_DES40_CBC_SHATLS_DH_DSS_WITH_DES_CBC_SHATLS_DH_DSS_EXPORT_WITH_DES40_CBC_SHATLS_RSA_WITH_3DES_EDE_CBC_SHATLS_RSA_WITH_DES_CBC_SHATLS_RSA_EXPORT_WITH_DES40_CBC_SHATLS_RSA_WITH_IDEA_CBC_SHATLS_RSA_EXPORT_WITH_RC2_CBC_40_MD5TLS_RSA_WITH_RC4_128_SHATLS_RSA_WITH_RC4_128_MD5TLS_RSA_EXPORT_WITH_RC4_40_MD5TLS_RSA_WITH_NULL_SHATLS_RSA_WITH_NULL_MD5TLS_NULL_WITH_NULL_NULLED448ED25519RSA_PSS_SHA512RSA_PSS_SHA384RSA_PSS_SHA256ECDSA_NISTP521_SHA512ECDSA_NISTP384_SHA384ECDSA_NISTP256_SHA256ECDSA_SHA1_LegacyRSA_PKCS1_SHA1
-attempt to join into collection with len > usize::MAXassertion failed: mid <= self.len()/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/alloc/src/str.rsUnvalidated OCSP response: rustls::verify/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/verify.rscertificate transparency logs have expired, validation disabledSCT ignored because Valid SCT signed by  on No valid SCTs providedinvalid peer certificate: received unadvertised sig scheme received unsupported sig scheme TLS 1.3, client CertificateVerify
-TLS 1.3, server CertificateVerify
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/digest.rsDnsName
-ChangeCipherSpecClientSessionKeyapplication_data
-chunk size must be non-zero/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/alloc/src/slice.rsPoisonError/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/msgs/fragmenter.rssessionkx-hint/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/tls12/prf.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/digest.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/client/tls12.rsdowngrade to TLS1.2 when TLS1.3 is supportedServer supports ticketsrustls::client::tls12::server_helloServer may staple OCSP responseServer sent  SCTsserver sent invalid SCT listServer agreed to resumeabbreviated handshake offered, but with varied csserver varied ems support over resumeCLIENT_RANDOM
-ApplicationDataHandshakeparsedencodedAlertversionpayloadMessage
-cannot access a Thread Local Storage value during or after destruction/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/std/src/thread/local.rsassertion failed: mid <= self.len()called `Result::unwrap()` on an `Err` value/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/msgs/hsjoiner.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/digest.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/tls12/cipher.rsencrypt failedextended master secretmaster secret/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/tls12/mod.rskey expansionclient finishedserver finishedassertion failed: context.len() <= 0xffffCertificate/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/client/handy.rsAlertMessagePayloadleveldescription}I
-R #*ru-x0
- when expecting ServerConnection
-,4;CKS[iw
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/agreement.rssni the supplied max_fragment_size was too small or largepeer doesn't support any known protocolpeer sent excess record sizehandshake not completefailed to get random bytesfailed to get current timeunexpected error: invalid certificate timestamp: invalid peer certificate contents: invalid peer certificate signatureinvalid peer certificate signature typeinvalid peer certificate encodingreceived fatal alert: peer misbehaved: peer is incompatible: cannot encrypt messagecannot decrypt peer's messagepresented server name type wasn't supportedpeer sent no certificatesreceived corrupt message of type received corrupt messagereceived unexpected handshake message: got received unexpected message: got BadMaxFragmentSizeNoApplicationProtocolPeerSentOversizedRecordHandshakeNotCompleteFailedToGetRandomBytesFailedToGetCurrentTimeGeneralInvalidSctInvalidCertificateDataInvalidCertificateSignatureInvalidCertificateSignatureTypeInvalidCertificateEncodingAlertReceivedPeerMisbehavedErrorPeerIncompatibleErrorEncryptErrorDecryptErrorUnsupportedNameTypeNoCertificatesPresentedCorruptMessagePayloadCorruptMessageInappropriateHandshakeMessageexpect_typesInappropriateMessage
-invalid SCT listUnknownExtensionSessionTicketAckCertificateEntryClientECDHParamsServerECDHParamsNewSessionTicketCertificateTLS13
-"	+		4=	@CKXgpy					
+UnknownExtensionSessionTicketAckCertificateEntryServerECDHParamsCertificateTLS13identityBulkOnlylifetime
 ACEGIKMO
-n "$+-nnnnnnn6InnU`
-!#%')+-/
-oqsuwy{}
-\^`bdfhjlnprtvxz|~
-[]_	acegikmoqsu
+n#%'.0nnnnnnn9JnnWa
+ (08@HPX`hpx
+"$&(*,.0v
+egikmoqsu
+Z\^`bdfhjlnprtvxz|~
+Y[]	_acegikmoqs
+ (08@HPX`iI
  "$&(*,.02468:<>@BDFH
-RJX\TbN`HLZFPDV^d
-*6BHT`lx~
-*6BHNZfr~
-#)4?JU[alw
+DFHJLNPRTVXZ\^`bd
+%/9@JT^hmty
+%/9>CMWakr
+#)2;AFMS\enw
 called `Result::unwrap()` on an `Err` value
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/msgs/handshake.rsIllegal SNI hostname received rustls::msgs::handshakemeaningless CertificateRequest messagetyppayloadUnknownServerNameKeyShareEntrygroupPresharedKeyIdentityobfuscated_ticket_agePresharedKeyOfferidentitiesbindersOCSPCertificateStatusRequestresponder_idsextensionsEarlyDataTransportParametersDraftTransportParametersSignedCertificateTimestampRequestCertificateStatusRequestExtendedMasterSecretRequestCookiePresharedKeyPresharedKeyModesSupportedVersionsProtocolsSessionTicketSignatureAlgorithmsNamedGroupsECPointFormatsOfferRequestSignedCertificateTimestampCertificateStatusAckExtendedMasterSecretAckRenegotiationInfoServerNameAckclient_versionrandomsession_idcipher_suitescompression_methodsClientHelloPayloadHelloRetryRequestlegacy_versioncipher_suitecompression_methodServerHelloPayloadCertificateStatusCertificatePayloadTLS13contextentriesECDHEECParameterscurve_typenamed_groupDigitallySignedStructschemesigpubliccurve_paramsECDHEServerKeyExchangeparamsdssCertificateRequestPayloadcerttypessigschemescanamesAuthorityNamesCertificateRequestPayloadTLS13NewSessionTicketPayloadlifetime_hintticketNewSessionTicketPayloadTLS13age_addnonceocsp_responseMessageHashKeyUpdateEncryptedExtensionsNewSessionTicketTLS13ClientKeyExchangeEndOfEarlyDataServerHelloDoneCertificateVerifyCertificateRequestTLS13CertificateRequestServerKeyExchangeCertificateServerHelloClientHelloHelloRequestHandshakeMessagePayload
- (+8g3uu33M^u
-?9<6/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/alloc/src/slice.rswrong group for key shareNot resumingrustls::client::tls13/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/client/tls13.rsserver selected unoffered pskserver varied suite with early dataserver selected invalid pskResuming using PSKserver resuming incompatible suitemissing key shareserver sent unexpected cleartext extNo kx groups configured/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/digest.rsStarting early data trafficserver sent duplicate encrypted extensionsserver sent unsolicited encrypted extensionserver sent inappropriate encrypted extension
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/msgs/handshake.rsIllegal SNI hostname received rustls::msgs::handshake
+meaningless CertificateRequest messagetyppayloadUnknownServerNameKeyShareEntrygroupPresharedKeyIdentityobfuscated_ticket_agePresharedKeyOfferidentitiesbindersOCSPCertificateStatusRequestresponder_idsextensionsEarlyDataTransportParametersDraftTransportParametersSignedCertificateTimestampRequestCertificateStatusRequestExtendedMasterSecretRequestCookiePresharedKeyPresharedKeyModesSupportedVersionsProtocolsSessionTicketSignatureAlgorithmsNamedGroupsECPointFormatsOfferRequestSignedCertificateTimestampCertificateStatusAckExtendedMasterSecretAckRenegotiationInfoServerNameAckclient_versionrandomsession_idcipher_suitescompression_methodsClientHelloPayloadHelloRetryRequestlegacy_versioncipher_suitecompression_methodServerHelloPayloadCertificateStatusCertificatePayloadTLS13contextentriesECDHEECParameterscurve_typenamed_groupDigitallySignedStructschemesigpubliccurve_paramsECDHEServerKeyExchangeparamsdssCertificateRequestPayloadcerttypessigschemescanamesAuthorityNamesCertificateRequestPayloadTLS13NewSessionTicketPayloadlifetime_hintticketNewSessionTicketPayloadTLS13age_addnonceocsp_responseMessageHashKeyUpdateEncryptedExtensionsNewSessionTicketTLS13ClientKeyExchangeEndOfEarlyDataServerHelloDoneCertificateVerifyCertificateRequestTLS13CertificateRequestServerKeyExchangeCertificateServerHelloClientHelloHelloRequestHandshakeMessagePayload
+certextsECDH
+$'4`/nn//HXn
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/digest.rswrong group for key shareNot resumingrustls::client::tls13/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/client/tls13.rsserver selected unoffered pskserver varied suite with early dataserver selected invalid pskResuming using PSKserver resuming incompatible suitemissing key shareserver sent unexpected cleartext extNo kx groups configuredStarting early data trafficserver sent duplicate encrypted extensionsserver sent unsolicited encrypted extensionserver sent inappropriate encrypted extension
 TLS1.3 encrypted extensions: server sent early data extension without resumption
 Got CertificateRequest Server sent non-empty certreq contextserver sent bad certreq schemes
 certificate with non-empty context during handshakecertificate chain contains unsolicited/unknown extensionbad cert chain extensionsserver sent invalid SCT listserver sent unsolicited SCT list
 Server cert is 
-peer sent duplicate NewSessionTicket extensionsSession not saved: Ticket savedTicket not saved
-UnrecognisedNameMissingExtensionIllegalParameterHandshakeFailureDecryptionFailed
-$*06<BHNTZ`flrC
+peer sent duplicate NewSessionTicket extensionsSession not saved: Ticket saved
+Ticket not saved
+$2?k:yy::Scy
+#(-27<AFKPUd
+!$).149>CHOC
+ "$&(*,.02468:<>@BC
  "$&(*,.02468:<>@B
 CCCCCCCCC
 CCCCCCCCC
 CCCCCCCCC
  "CCCCCCCC$CCCCCCCCC&(CCCCCCCC*CCCCC,CCC.CCCCCCCCC0CCCCCCCC2468:<>@CCCB
-$*06<BHNTZ`flrx~
+"%(+.36;>CFINQV[^cfkpuz
+ "$&(*,.02468:<>@BDFHI
  "$&(*,.02468:<>@BDFH
-88888888888
-!#%')+-/1888883
-$*06<BHNTZ`flrx~
-UnknownSHA1NONENullX448ED448ED25519ECDSADSARSAAnonymousECDSAFixedECDHRSAFixedECDHECDSASignFortezzaDMSDSSEphemeralDHRSAEphemeralDHDSSFixedDHRSAFixedDHDSSSignRSASignLSZDeflateHeartbeatApplicationDataHandshakeAlertMessageHashKeyUpdateCertificateStatusCertificateURLResponseKeyShareHostNameClientKeyExchangeCertificateVerifyServerHelloDoneCertificateRequestServerKeyExchangeCertificateEncryptedExtensionsHelloRetryRequestEndOfEarlyDataHelloVerifyRequestServerHelloClientHelloHelloRequestFatalWarningNoApplicationProtocolCertificateRequiredUnknownPSKIdentityBadCertificateHashValueBadCertificateStatusResponseCertificateUnobtainableUnsupportedExtensionNoRenegotiationUserCanceledInappropriateFallbackInternalErrorInsufficientSecurityProtocolVersionExportRestrictionDecryptErrorDecodeErrorAccessDeniedUnknownCACertificateUnknownCertificateExpiredCertificateRevokedUnsupportedCertificateBadCertificateNoCertificateDecompressionFailureRecordOverflowBadRecordMacUnexpectedMessageCloseNotifyTransportParametersDraftRenegotiationInfoChannelIdNextProtocolNegotiationTransportParametersSignatureAlgorithmsCertPostHandshakeAuthOIDFiltersCertificateAuthoritiesTicketEarlyDataInfoPSKKeyExchangeModesCookieSupportedVersionsEarlyDataPreSharedKeySessionTicketExtendedMasterSecretPaddingSCTALProtocolNegotiationUseSRTPSignatureAlgorithmsSRPECPointFormatsEllipticCurvesCertificateTypeServerAuthzClientAuthzUserMappingStatusRequestTruncatedHMACTrustedCAKeysClientCertificateUrlMaxFragmentLengthServerNameX25519secp521r1secp384r1secp256r1FFDHE8192FFDHE6144FFDHE4096FFDHE3072FFDHE2048ANSIX962CompressedChar2ANSIX962CompressedPrimeUncompressedNamedCurveExplicitChar2ExplicitPrimePSK_DHE_KEPSK_KEUpdateRequestedUpdateNotRequested
-Server stapled OCSP response is rustls::client::tls12/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/client/tls12.rs	
+33333333333433333
+ "$&(*,.0333332
+"%*-036;@EJOTWZ_bejoruz
+ "$&(*,.02468:<>?
+ "$&(*,.02468:<>
+ "$&(*,.02468:<>@BD
+!$'*-0369<?BEHPSV\bhkq
+ED448ED25519ECDSADSARSAAnonymousECDSAFixedECDHRSAFixedECDHECDSASignFortezzaDMSDSSEphemeralDHRSAEphemeralDHDSSFixedDHRSAFixedDHDSSSignRSASignLSZDeflateHeartbeatApplicationDataHandshakeAlertMessageHashKeyUpdateCertificateStatusCertificateURLClientKeyExchangeCertificateVerifyServerHelloDoneCertificateRequestServerKeyExchangeCertificateEncryptedExtensionsHelloRetryRequestEndOfEarlyDataHelloVerifyRequestServerHelloClientHelloHelloRequestFatalWarningNoApplicationProtocolCertificateRequiredUnknownPSKIdentityBadCertificateHashValueBadCertificateStatusResponseCertificateUnobtainableUnsupportedExtensionNoRenegotiationUserCanceledInappropriateFallbackInternalErrorInsufficientSecurityProtocolVersionExportRestrictionDecryptErrorDecodeErrorAccessDeniedUnknownCACertificateUnknownCertificateExpiredCertificateRevokedUnsupportedCertificateBadCertificateNoCertificateDecompressionFailureRecordOverflowBadRecordMacUnexpectedMessageCloseNotify
+TransportParametersDraftRenegotiationInfoChannelIdNextProtocolNegotiationTransportParametersSignatureAlgorithmsCertPostHandshakeAuthOIDFiltersCertificateAuthoritiesTicketEarlyDataInfoPSKKeyExchangeModesCookieSupportedVersionsEarlyDataPreSharedKeySessionTicketExtendedMasterSecretPaddingSCTALProtocolNegotiationUseSRTPSignatureAlgorithmsSRPECPointFormatsEllipticCurvesCertificateTypeServerAuthzClientAuthzUserMappingStatusRequestTruncatedHMACTrustedCAKeysClientCertificateUrlMaxFragmentLengthServerName
+X448X25519
+secp521r1secp384r1secp256r1
+FFDHE8192FFDHE6144FFDHE4096FFDHE3072FFDHE2048ANSIX962CompressedChar2ANSIX962CompressedPrimeUncompressed
+NamedCurveExplicitChar2ExplicitPrimePSK_DHE_KEPSK_KEUpdateRequestedUpdateNotRequested
+NewSessionTicketUnrecognisedNameMissingExtensionIllegalParameterHandshakeFailureDecryptionFailedFinishedKeyShareHostName
+called `Result::unwrap()` on an `Err` valuederivedres masterexp masters ap trafficc ap traffics hs trafficc hs trafficc e trafficres binderEXPORTER_SECRETSERVER_TRAFFIC_SECRET_0CLIENT_TRAFFIC_SECRET_0SERVER_HANDSHAKE_TRAFFIC_SECRETCLIENT_HANDSHAKE_TRAFFIC_SECRETCLIENT_EARLY_TRAFFIC_SECRET/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/digest.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/tls13/key_schedule.rsnot a loggable secrettraffic updresumptionexporting too muchtls13 keyiv
+exporter
+chunk size must be non-zero
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/agreement.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/digest.rs
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/tls12/prf.rs
+AlertMessagePayloadleveldescription
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/client/hs.rsNo cached session for rustls::client::hsNot resuming any sessionassertion failed: !supported_versions.is_empty()Sending ClientHello server sent non-offered ALPN protocolALPN protocol is 
+We got ServerHello server chose v1.2 when offering 0-rttserver chose v1.2 using v1.3 extension
+server chose non-Null compressionserver sent duplicate extensionsserver sent unsolicited extensionserver does not support uncompressed pointsserver chose unusable ciphersuite for versionserver varied selected ciphersuiteUsing ciphersuite called `Option::unwrap()` on a `None` valueserver does not support TLS v1.2/v1.3server's TLS version is disabled in clientserver chose non-offered ciphersuite
+server requested hrr with our groupserver sent hrr with unhandled extensionserver send duplicate hrr extensionsserver requested hrr with no changesserver requested unsupported version in hrrserver requested hrr with bad groupserver requested unsupported cs in hrrserver requested hrr with empty cookie
+Server stapled OCSP response is rustls::client::tls12/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/client/tls12.rs	
 ECDHE curve is Expected transcript
 Got CertificateRequest 
-Server cert is Server DNS name is peer signed kx with wrong algorithm (got  expect )CLIENT_RANDOMpeer chose an unsupported group
+Server cert is Server DNS name is peer signed kx with wrong algorithm (got )peer chose an unsupported groupCLIENT_RANDOM
 Session not saved: server didn't allocate id or ticketSession not saved: Session savedSession not saved
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/sct-0.7.0/src/lib.rsUnknownLogUnsupportedSctVersionTimestampInFutureInvalidSignatureMalformedSct
-Once has panicked/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/spin-0.5.2/src/once.rsinternal error: entered unreachable codecalled `Result::unwrap()` on an `Err` value/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/webpki-0.22.0/src/name/dns_name.rsinternal error: entered unreachable codeDnsNameInvalidDnsNameErrorOnce has panicked/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/spin-0.5.2/src/once.rsinternal error: entered unreachable code
+Got HRR  expect Resuming session
+$2?z:nn::Sen
+/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/std/src/io/impls.rsa Display implementation returned an error unexpectedly/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/alloc/src/string.rs
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/msgs/deframer.rsmessage buffer full
+encrypt failedpeer sent bad TLSInnerPlaintext
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/client/client_conn.rsEarlyData rejectedrustls::client::client_connEarlyData accepted
+EarlyData finishedbad EarlyData stateinternal error: entered unreachable code
+IpAddressDnsName
+AcceptedFinishedRejectedAccepted
+called `Result::unwrap()` on an `Err` value/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/msgs/codec.rs
+Unvalidated OCSP response: rustls::verify/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/verify.rscertificate transparency logs have expired, validation disabledSCT ignored because Valid SCT signed by No valid SCTs providedinvalid peer certificate: 
+received unadvertised sig scheme received unsupported sig scheme TLS 1.3, client CertificateVerify
+TLS 1.3, server CertificateVerify
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/digest.rsCertificate/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/client/handy.rsDnsName
+!#%')+-/13579;=?ACEGIKMOQSUWY[]_
+$2?k:yy::Scy
+#%')+4=ACEGPT]_aceg
+assertion failed: mid <= self.len()
+attempt to join into collection with len > usize::MAX/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/alloc/src/str.rs
+rustls::conn/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/conn.rs
+key epoch or handshake flight with pending fragmentDropping undecryptable message after aborted early_dataSending warning alert TLS alert warning received: TLS alert received: Sending fatal alert Received a  message while expecting rustls::check/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/check.rs handshake message while expecting 
+ when expecting RSA_PKCS1_SHA512RSA_PKCS1_SHA384RSA_PKCS1_SHA256got_type
+,29<BEKValrx~
+assertion failed: mid <= self.len()called `Result::unwrap()` on an `Err` value
+the supplied max_fragment_size was too small or largepeer doesn't support any known protocolpeer sent excess record sizehandshake not completefailed to get random bytesfailed to get current timeunexpected error: invalid certificate timestamp: invalid peer certificate contents: invalid peer certificate signatureinvalid peer certificate signature typeinvalid peer certificate encodingreceived fatal alert: peer misbehaved: peer is incompatible: cannot encrypt messagecannot decrypt peer's messagepresented server name type wasn't supportedpeer sent no certificatesreceived corrupt message of type received corrupt messagereceived unexpected handshake message: got received unexpected message: got 
+extended master secretmaster secret/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/tls12/mod.rskey expansion/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/digest.rsclient finishedserver finishedassertion failed: context.len() <= 0xffff/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/tls13/key_schedule.rsBadMaxFragmentSizeNoApplicationProtocolPeerSentOversizedRecordHandshakeNotCompleteFailedToGetRandomBytesFailedToGetCurrentTimeGeneralInvalidSctInvalidCertificateDataInvalidCertificateSignatureInvalidCertificateSignatureTypeInvalidCertificateEncodingAlertReceivedPeerMisbehavedErrorPeerIncompatibleErrorEncryptErrorDecryptErrorUnsupportedNameTypeNoCertificatesPresentedCorruptMessagePayloadCorruptMessageInappropriateHandshakeMessageexpect_typesInappropriateMessageDTLSv1_3DTLSv1_2DTLSv1_0TLSv1_3TLSv1_2TLSv1_1TLSv1_0SSLv3SSLv2UnknownSSL_RSA_FIPS_WITH_3DES_EDE_CBC_SHASSL_RSA_FIPS_WITH_DES_CBC_SHATLS_RSA_PSK_WITH_CHACHA20_POLY1305_SHA256TLS_DHE_PSK_WITH_CHACHA20_POLY1305_SHA256TLS_ECDHE_PSK_WITH_CHACHA20_POLY1305_SHA256TLS_PSK_WITH_CHACHA20_POLY1305_SHA256TLS_DHE_RSA_WITH_CHACHA20_POLY1305_SHA256TLS_ECDHE_ECDSA_WITH_CHACHA20_POLY1305_SHA256TLS_ECDHE_RSA_WITH_CHACHA20_POLY1305_SHA256TLS_ECDHE_ECDSA_WITH_AES_256_CCM_8TLS_ECDHE_ECDSA_WITH_AES_128_CCM_8TLS_ECDHE_ECDSA_WITH_AES_256_CCMTLS_ECDHE_ECDSA_WITH_AES_128_CCMTLS_PSK_DHE_WITH_AES_256_CCM_8TLS_PSK_DHE_WITH_AES_128_CCM_8TLS_PSK_WITH_AES_256_CCM_8TLS_PSK_WITH_AES_128_CCM_8TLS_DHE_PSK_WITH_AES_256_CCMTLS_DHE_PSK_WITH_AES_128_CCMTLS_PSK_WITH_AES_256_CCMTLS_PSK_WITH_AES_128_CCMTLS_DHE_RSA_WITH_AES_256_CCM_8TLS_DHE_RSA_WITH_AES_128_CCM_8TLS_RSA_WITH_AES_256_CCM_8TLS_RSA_WITH_AES_128_CCM_8TLS_DHE_RSA_WITH_AES_256_CCMTLS_DHE_RSA_WITH_AES_128_CCMTLS_RSA_WITH_AES_256_CCMTLS_RSA_WITH_AES_128_CCMTLS_ECDHE_PSK_WITH_CAMELLIA_256_CBC_SHA384TLS_ECDHE_PSK_WITH_CAMELLIA_128_CBC_SHA256TLS_RSA_PSK_WITH_CAMELLIA_256_CBC_SHA384TLS_RSA_PSK_WITH_CAMELLIA_128_CBC_SHA256TLS_DHE_PSK_WITH_CAMELLIA_256_CBC_SHA384TLS_DHE_PSK_WITH_CAMELLIA_128_CBC_SHA256TLS_PSK_WITH_CAMELLIA_256_CBC_SHA384TLS_PSK_WITH_CAMELLIA_128_CBC_SHA256TLS_RSA_PSK_WITH_CAMELLIA_256_GCM_SHA384TLS_RSA_PSK_WITH_CAMELLIA_128_GCM_SHA256TLS_DHE_PSK_WITH_CAMELLIA_256_GCM_SHA384TLS_DHE_PSK_WITH_CAMELLIA_128_GCM_SHA256TLS_PSK_WITH_CAMELLIA_256_GCM_SHA384TLS_PSK_WITH_CAMELLIA_128_GCM_SHA256TLS_ECDH_RSA_WITH_CAMELLIA_256_GCM_SHA384TLS_ECDH_RSA_WITH_CAMELLIA_128_GCM_SHA256TLS_ECDHE_RSA_WITH_CAMELLIA_256_GCM_SHA384TLS_ECDHE_RSA_WITH_CAMELLIA_128_GCM_SHA256TLS_ECDH_ECDSA_WITH_CAMELLIA_256_GCM_SHA384TLS_ECDH_ECDSA_WITH_CAMELLIA_128_GCM_SHA256TLS_ECDHE_ECDSA_WITH_CAMELLIA_256_GCM_SHA384TLS_ECDHE_ECDSA_WITH_CAMELLIA_128_GCM_SHA256TLS_DH_anon_WITH_CAMELLIA_256_GCM_SHA384TLS_DH_anon_WITH_CAMELLIA_128_GCM_SHA256TLS_DH_DSS_WITH_CAMELLIA_256_GCM_SHA384TLS_DH_DSS_WITH_CAMELLIA_128_GCM_SHA256TLS_DHE_DSS_WITH_CAMELLIA_256_GCM_SHA384TLS_DHE_DSS_WITH_CAMELLIA_128_GCM_SHA256TLS_DH_RSA_WITH_CAMELLIA_256_GCM_SHA384TLS_DH_RSA_WITH_CAMELLIA_128_GCM_SHA256TLS_DHE_RSA_WITH_CAMELLIA_256_GCM_SHA384TLS_DHE_RSA_WITH_CAMELLIA_128_GCM_SHA256TLS_RSA_WITH_CAMELLIA_256_GCM_SHA384TLS_RSA_WITH_CAMELLIA_128_GCM_SHA256TLS_ECDH_RSA_WITH_CAMELLIA_256_CBC_SHA384TLS_ECDH_RSA_WITH_CAMELLIA_128_CBC_SHA256TLS_ECDHE_RSA_WITH_CAMELLIA_256_CBC_SHA384TLS_ECDHE_RSA_WITH_CAMELLIA_128_CBC_SHA256TLS_ECDH_ECDSA_WITH_CAMELLIA_256_CBC_SHA384TLS_ECDH_ECDSA_WITH_CAMELLIA_128_CBC_SHA256TLS_ECDHE_ECDSA_WITH_CAMELLIA_256_CBC_SHA384TLS_ECDHE_ECDSA_WITH_CAMELLIA_128_CBC_SHA256TLS_ECDHE_PSK_WITH_ARIA_256_CBC_SHA384TLS_ECDHE_PSK_WITH_ARIA_128_CBC_SHA256TLS_RSA_PSK_WITH_ARIA_256_GCM_SHA384TLS_RSA_PSK_WITH_ARIA_128_GCM_SHA256TLS_DHE_PSK_WITH_ARIA_256_GCM_SHA384TLS_DHE_PSK_WITH_ARIA_128_GCM_SHA256TLS_PSK_WITH_ARIA_256_GCM_SHA384TLS_PSK_WITH_ARIA_128_GCM_SHA256TLS_RSA_PSK_WITH_ARIA_256_CBC_SHA384TLS_RSA_PSK_WITH_ARIA_128_CBC_SHA256TLS_DHE_PSK_WITH_ARIA_256_CBC_SHA384TLS_DHE_PSK_WITH_ARIA_128_CBC_SHA256TLS_PSK_WITH_ARIA_256_CBC_SHA384TLS_PSK_WITH_ARIA_128_CBC_SHA256TLS_ECDH_RSA_WITH_ARIA_256_GCM_SHA384TLS_ECDH_RSA_WITH_ARIA_128_GCM_SHA256TLS_ECDHE_RSA_WITH_ARIA_256_GCM_SHA384TLS_ECDHE_RSA_WITH_ARIA_128_GCM_SHA256TLS_ECDH_ECDSA_WITH_ARIA_256_GCM_SHA384TLS_ECDH_ECDSA_WITH_ARIA_128_GCM_SHA256TLS_ECDHE_ECDSA_WITH_ARIA_256_GCM_SHA384TLS_ECDHE_ECDSA_WITH_ARIA_128_GCM_SHA256TLS_DH_anon_WITH_ARIA_256_GCM_SHA384TLS_DH_anon_WITH_ARIA_128_GCM_SHA256TLS_DH_DSS_WITH_ARIA_256_GCM_SHA384TLS_DH_DSS_WITH_ARIA_128_GCM_SHA256TLS_DHE_DSS_WITH_ARIA_256_GCM_SHA384TLS_DHE_DSS_WITH_ARIA_128_GCM_SHA256TLS_DH_RSA_WITH_ARIA_256_GCM_SHA384TLS_DH_RSA_WITH_ARIA_128_GCM_SHA256TLS_DHE_RSA_WITH_ARIA_256_GCM_SHA384TLS_DHE_RSA_WITH_ARIA_128_GCM_SHA256TLS_RSA_WITH_ARIA_256_GCM_SHA384TLS_RSA_WITH_ARIA_128_GCM_SHA256TLS_ECDH_RSA_WITH_ARIA_256_CBC_SHA384TLS_ECDH_RSA_WITH_ARIA_128_CBC_SHA256TLS_ECDHE_RSA_WITH_ARIA_256_CBC_SHA384TLS_ECDHE_RSA_WITH_ARIA_128_CBC_SHA256TLS_ECDH_ECDSA_WITH_ARIA_256_CBC_SHA384TLS_ECDH_ECDSA_WITH_ARIA_128_CBC_SHA256TLS_ECDHE_ECDSA_WITH_ARIA_256_CBC_SHA384TLS_ECDHE_ECDSA_WITH_ARIA_128_CBC_SHA256TLS_DH_anon_WITH_ARIA_256_CBC_SHA384TLS_DH_anon_WITH_ARIA_128_CBC_SHA256TLS_DHE_RSA_WITH_ARIA_256_CBC_SHA384TLS_DHE_RSA_WITH_ARIA_128_CBC_SHA256TLS_DHE_DSS_WITH_ARIA_256_CBC_SHA384TLS_DHE_DSS_WITH_ARIA_128_CBC_SHA256TLS_DH_RSA_WITH_ARIA_256_CBC_SHA384TLS_DH_RSA_WITH_ARIA_128_CBC_SHA256TLS_DH_DSS_WITH_ARIA_256_CBC_SHA384TLS_DH_DSS_WITH_ARIA_128_CBC_SHA256TLS_RSA_WITH_ARIA_256_CBC_SHA384TLS_RSA_WITH_ARIA_128_CBC_SHA256TLS_ECDHE_PSK_WITH_NULL_SHA384TLS_ECDHE_PSK_WITH_NULL_SHA256TLS_ECDHE_PSK_WITH_NULL_SHATLS_ECDHE_PSK_WITH_AES_256_CBC_SHA384TLS_ECDHE_PSK_WITH_AES_128_CBC_SHA256TLS_ECDHE_PSK_WITH_AES_256_CBC_SHATLS_ECDHE_PSK_WITH_AES_128_CBC_SHATLS_ECDHE_PSK_WITH_3DES_EDE_CBC_SHATLS_ECDHE_PSK_WITH_RC4_128_SHATLS_ECDH_RSA_WITH_AES_256_GCM_SHA384TLS_ECDH_RSA_WITH_AES_128_GCM_SHA256TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384TLS_ECDHE_RSA_WITH_AES_128_GCM_SHA256TLS_ECDH_ECDSA_WITH_AES_256_GCM_SHA384TLS_ECDH_ECDSA_WITH_AES_128_GCM_SHA256TLS_ECDHE_ECDSA_WITH_AES_256_GCM_SHA384TLS_ECDHE_ECDSA_WITH_AES_128_GCM_SHA256TLS_ECDH_RSA_WITH_AES_256_CBC_SHA384TLS_ECDH_RSA_WITH_AES_128_CBC_SHA256TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA384TLS_ECDHE_RSA_WITH_AES_128_CBC_SHA256TLS_ECDH_ECDSA_WITH_AES_256_CBC_SHA384TLS_ECDH_ECDSA_WITH_AES_128_CBC_SHA256TLS_ECDHE_ECDSA_WITH_AES_256_CBC_SHA384TLS_ECDHE_ECDSA_WITH_AES_128_CBC_SHA256TLS_SRP_SHA_DSS_WITH_AES_256_CBC_SHATLS_SRP_SHA_RSA_WITH_AES_256_CBC_SHATLS_SRP_SHA_WITH_AES_256_CBC_SHATLS_SRP_SHA_DSS_WITH_AES_128_CBC_SHATLS_SRP_SHA_RSA_WITH_AES_128_CBC_SHATLS_SRP_SHA_WITH_AES_128_CBC_SHATLS_SRP_SHA_DSS_WITH_3DES_EDE_CBC_SHATLS_SRP_SHA_RSA_WITH_3DES_EDE_CBC_SHATLS_SRP_SHA_WITH_3DES_EDE_CBC_SHATLS_ECDH_anon_WITH_AES_256_CBC_SHATLS_ECDH_anon_WITH_AES_128_CBC_SHATLS_ECDH_anon_WITH_3DES_EDE_CBC_SHATLS_ECDH_anon_WITH_RC4_128_SHATLS_ECDH_anon_WITH_NULL_SHATLS_ECDHE_RSA_WITH_AES_256_CBC_SHATLS_ECDHE_RSA_WITH_AES_128_CBC_SHATLS_ECDHE_RSA_WITH_3DES_EDE_CBC_SHATLS_ECDHE_RSA_WITH_RC4_128_SHATLS_ECDHE_RSA_WITH_NULL_SHATLS_ECDH_RSA_WITH_AES_256_CBC_SHATLS_ECDH_RSA_WITH_AES_128_CBC_SHATLS_ECDH_RSA_WITH_3DES_EDE_CBC_SHATLS_ECDH_RSA_WITH_RC4_128_SHATLS_ECDH_RSA_WITH_NULL_SHATLS_ECDHE_ECDSA_WITH_AES_256_CBC_SHATLS_ECDHE_ECDSA_WITH_AES_128_CBC_SHATLS_ECDHE_ECDSA_WITH_3DES_EDE_CBC_SHATLS_ECDHE_ECDSA_WITH_RC4_128_SHATLS_ECDHE_ECDSA_WITH_NULL_SHATLS_ECDH_ECDSA_WITH_AES_256_CBC_SHATLS_ECDH_ECDSA_WITH_AES_128_CBC_SHATLS_ECDH_ECDSA_WITH_3DES_EDE_CBC_SHATLS_ECDH_ECDSA_WITH_RC4_128_SHATLS_ECDH_ECDSA_WITH_NULL_SHATLS13_AES_128_CCM_8_SHA256TLS13_AES_128_CCM_SHA256TLS13_CHACHA20_POLY1305_SHA256TLS13_AES_256_GCM_SHA384TLS13_AES_128_GCM_SHA256TLS_EMPTY_RENEGOTIATION_INFO_SCSVTLS_DH_anon_WITH_CAMELLIA_256_CBC_SHA256TLS_DHE_RSA_WITH_CAMELLIA_256_CBC_SHA256TLS_DHE_DSS_WITH_CAMELLIA_256_CBC_SHA256TLS_DH_RSA_WITH_CAMELLIA_256_CBC_SHA256TLS_DH_DSS_WITH_CAMELLIA_256_CBC_SHA256TLS_RSA_WITH_CAMELLIA_256_CBC_SHA256TLS_DH_anon_WITH_CAMELLIA_128_CBC_SHA256TLS_DHE_RSA_WITH_CAMELLIA_128_CBC_SHA256TLS_DHE_DSS_WITH_CAMELLIA_128_CBC_SHA256TLS_DH_RSA_WITH_CAMELLIA_128_CBC_SHA256TLS_DH_DSS_WITH_CAMELLIA_128_CBC_SHA256TLS_RSA_WITH_CAMELLIA_128_CBC_SHA256TLS_RSA_PSK_WITH_NULL_SHA384TLS_RSA_PSK_WITH_NULL_SHA256TLS_RSA_PSK_WITH_AES_256_CBC_SHA384TLS_RSA_PSK_WITH_AES_128_CBC_SHA256TLS_DHE_PSK_WITH_NULL_SHA384TLS_DHE_PSK_WITH_NULL_SHA256TLS_DHE_PSK_WITH_AES_256_CBC_SHA384TLS_DHE_PSK_WITH_AES_128_CBC_SHA256TLS_PSK_WITH_NULL_SHA384TLS_PSK_WITH_NULL_SHA256TLS_PSK_WITH_AES_256_CBC_SHA384TLS_PSK_WITH_AES_128_CBC_SHA256TLS_RSA_PSK_WITH_AES_256_GCM_SHA384TLS_RSA_PSK_WITH_AES_128_GCM_SHA256TLS_DHE_PSK_WITH_AES_256_GCM_SHA384TLS_DHE_PSK_WITH_AES_128_GCM_SHA256TLS_PSK_WITH_AES_256_GCM_SHA384TLS_PSK_WITH_AES_128_GCM_SHA256TLS_DH_anon_WITH_AES_256_GCM_SHA384TLS_DH_anon_WITH_AES_128_GCM_SHA256TLS_DH_DSS_WITH_AES_256_GCM_SHA384TLS_DH_DSS_WITH_AES_128_GCM_SHA256TLS_DHE_DSS_WITH_AES_256_GCM_SHA384TLS_DHE_DSS_WITH_AES_128_GCM_SHA256TLS_DH_RSA_WITH_AES_256_GCM_SHA384TLS_DH_RSA_WITH_AES_128_GCM_SHA256TLS_DHE_RSA_WITH_AES_256_GCM_SHA384TLS_DHE_RSA_WITH_AES_128_GCM_SHA256TLS_RSA_WITH_AES_256_GCM_SHA384TLS_RSA_WITH_AES_128_GCM_SHA256TLS_DH_anon_WITH_SEED_CBC_SHATLS_DHE_RSA_WITH_SEED_CBC_SHATLS_DHE_DSS_WITH_SEED_CBC_SHATLS_DH_RSA_WITH_SEED_CBC_SHATLS_DH_DSS_WITH_SEED_CBC_SHATLS_RSA_WITH_SEED_CBC_SHATLS_RSA_PSK_WITH_AES_256_CBC_SHATLS_RSA_PSK_WITH_AES_128_CBC_SHATLS_RSA_PSK_WITH_3DES_EDE_CBC_SHATLS_RSA_PSK_WITH_RC4_128_SHATLS_DHE_PSK_WITH_AES_256_CBC_SHATLS_DHE_PSK_WITH_AES_128_CBC_SHATLS_DHE_PSK_WITH_3DES_EDE_CBC_SHATLS_DHE_PSK_WITH_RC4_128_SHATLS_PSK_WITH_AES_256_CBC_SHATLS_PSK_WITH_AES_128_CBC_SHATLS_PSK_WITH_3DES_EDE_CBC_SHATLS_PSK_WITH_RC4_128_SHATLS_DH_anon_WITH_CAMELLIA_256_CBC_SHATLS_DHE_RSA_WITH_CAMELLIA_256_CBC_SHATLS_DHE_DSS_WITH_CAMELLIA_256_CBC_SHATLS_DH_RSA_WITH_CAMELLIA_256_CBC_SHATLS_DH_DSS_WITH_CAMELLIA_256_CBC_SHATLS_RSA_WITH_CAMELLIA_256_CBC_SHATLS_GOSTR341001_WITH_NULL_GOSTR3411TLS_GOSTR341094_WITH_NULL_GOSTR3411TLS_GOSTR341001_WITH_28147_CNT_IMITTLS_GOSTR341094_WITH_28147_CNT_IMITTLS_RSA_WITH_AES_256_CBC_RMDTLS_RSA_WITH_AES_128_CBC_RMDTLS_RSA_WITH_3DES_EDE_CBC_RMDTLS_DHE_RSA_WITH_AES_256_CBC_RMDTLS_DHE_RSA_WITH_AES_128_CBC_RMDTLS_DHE_RSA_WITH_3DES_EDE_CBC_RMDTLS_DHE_DSS_WITH_AES_256_CBC_RMDTLS_DHE_DSS_WITH_AES_128_CBC_RMDTLS_DHE_DSS_WITH_3DES_EDE_CBC_RMDTLS_DH_anon_WITH_AES_256_CBC_SHA256TLS_DH_anon_WITH_AES_128_CBC_SHA256TLS_DHE_RSA_WITH_AES_256_CBC_SHA256TLS_DHE_DSS_WITH_AES_256_CBC_SHA256TLS_DH_RSA_WITH_AES_256_CBC_SHA256TLS_DH_DSS_WITH_AES_256_CBC_SHA256TLS_DHE_RSA_WITH_AES_128_CBC_SHA256TLS_DHE_DSS_WITH_RC4_128_SHATLS_DHE_DSS_EXPORT1024_WITH_RC4_56_SHATLS_RSA_EXPORT1024_WITH_RC4_56_SHATLS_DHE_DSS_EXPORT1024_WITH_DES_CBC_SHATLS_RSA_EXPORT1024_WITH_DES_CBC_SHATLS_RSA_EXPORT1024_WITH_RC2_CBC_56_MD5TLS_RSA_EXPORT1024_WITH_RC4_56_MD5TLS_ECDH_anon_EXPORT_WITH_RC4_40_SHA_draftTLS_ECDH_anon_EXPORT_WITH_DES40_CBC_SHA_draftTLS_ECDH_anon_WITH_3DES_EDE_CBC_SHA_draftTLS_ECDH_anon_WITH_DES_CBC_SHA_draftTLS_ECDH_anon_WITH_RC4_128_SHA_draftTLS_ECDH_anon_NULL_WITH_SHA_draftTLS_ECMQV_ECNRA_WITH_3DES_EDE_CBC_SHA_draftTLS_ECMQV_ECNRA_WITH_DES_CBC_SHA_draftTLS_ECMQV_ECNRA_WITH_RC4_128_SHA_draftTLS_ECMQV_ECNRA_NULL_SHA_draftTLS_ECMQV_ECDSA_WITH_3DES_EDE_CBC_SHA_draftTLS_ECMQV_ECDSA_WITH_DES_CBC_SHA_draftTLS_ECMQV_ECDSA_WITH_RC4_128_SHA_draftTLS_ECMQV_ECDSA_NULL_SHA_draftTLS_ECDH_ECNRA_WITH_3DES_EDE_CBC_SHA_draftTLS_ECDH_ECNRA_WITH_DES_CBC_SHA_draftTLS_ECDH_ECDSA_WITH_AES_256_CBC_SHA_draftTLS_ECDH_ECDSA_WITH_AES_128_CBC_SHA_draftTLS_ECDH_ECDSA_WITH_3DES_EDE_CBC_SHA_draftTLS_ECDH_ECDSA_WITH_DES_CBC_SHA_draftTLS_ECDH_ECDSA_WITH_RC4_128_SHA_draftTLS_ECDH_ECDSA_WITH_NULL_SHA_draftTLS_DH_anon_WITH_CAMELLIA_128_CBC_SHATLS_DHE_RSA_WITH_CAMELLIA_128_CBC_SHATLS_DHE_DSS_WITH_CAMELLIA_128_CBC_SHATLS_DH_RSA_WITH_CAMELLIA_128_CBC_SHATLS_DH_DSS_WITH_CAMELLIA_128_CBC_SHATLS_RSA_WITH_CAMELLIA_128_CBC_SHATLS_DHE_DSS_WITH_AES_128_CBC_SHA256TLS_DH_RSA_WITH_AES_128_CBC_SHA256TLS_DH_DSS_WITH_AES_128_CBC_SHA256TLS_RSA_WITH_AES_256_CBC_SHA256TLS_RSA_WITH_AES_128_CBC_SHA256TLS_RSA_WITH_NULL_SHA256TLS_DH_anon_WITH_AES_256_CBC_SHATLS_DHE_RSA_WITH_AES_256_CBC_SHATLS_DHE_DSS_WITH_AES_256_CBC_SHATLS_DH_RSA_WITH_AES_256_CBC_SHATLS_DH_DSS_WITH_AES_256_CBC_SHATLS_RSA_WITH_AES_256_CBC_SHATLS_DH_anon_WITH_AES_128_CBC_SHATLS_DHE_RSA_WITH_AES_128_CBC_SHATLS_DHE_DSS_WITH_AES_128_CBC_SHATLS_DH_RSA_WITH_AES_128_CBC_SHATLS_DH_DSS_WITH_AES_128_CBC_SHATLS_RSA_WITH_AES_128_CBC_SHATLS_RSA_PSK_WITH_NULL_SHATLS_DHE_PSK_WITH_NULL_SHATLS_PSK_WITH_NULL_SHATLS_KRB5_EXPORT_WITH_RC4_40_MD5TLS_KRB5_EXPORT_WITH_RC2_CBC_40_MD5TLS_KRB5_EXPORT_WITH_DES_CBC_40_MD5TLS_KRB5_EXPORT_WITH_RC4_40_SHATLS_KRB5_EXPORT_WITH_RC2_CBC_40_SHATLS_KRB5_EXPORT_WITH_DES_CBC_40_SHATLS_KRB5_WITH_IDEA_CBC_MD5TLS_KRB5_WITH_RC4_128_MD5TLS_KRB5_WITH_3DES_EDE_CBC_MD5TLS_KRB5_WITH_DES_CBC_MD5TLS_KRB5_WITH_IDEA_CBC_SHATLS_KRB5_WITH_RC4_128_SHATLS_KRB5_WITH_3DES_EDE_CBC_SHATLS_KRB5_WITH_DES_CBC_SHA_or_SSL_FORTEZZA_KEA_WITH_RC4_128_SHASSL_FORTEZZA_KEA_WITH_FORTEZZA_CBC_SHASSL_FORTEZZA_KEA_WITH_NULL_SHATLS_DH_anon_WITH_3DES_EDE_CBC_SHATLS_DH_anon_WITH_DES_CBC_SHATLS_DH_anon_EXPORT_WITH_DES40_CBC_SHATLS_DH_anon_WITH_RC4_128_MD5TLS_DH_anon_EXPORT_WITH_RC4_40_MD5TLS_DHE_RSA_WITH_3DES_EDE_CBC_SHATLS_DHE_RSA_WITH_DES_CBC_SHATLS_DHE_RSA_EXPORT_WITH_DES40_CBC_SHATLS_DHE_DSS_WITH_3DES_EDE_CBC_SHATLS_DHE_DSS_WITH_DES_CBC_SHATLS_DHE_DSS_EXPORT_WITH_DES40_CBC_SHATLS_DH_RSA_WITH_3DES_EDE_CBC_SHATLS_DH_RSA_WITH_DES_CBC_SHATLS_DH_RSA_EXPORT_WITH_DES40_CBC_SHATLS_DH_DSS_WITH_3DES_EDE_CBC_SHATLS_DH_DSS_WITH_DES_CBC_SHATLS_DH_DSS_EXPORT_WITH_DES40_CBC_SHATLS_RSA_WITH_3DES_EDE_CBC_SHATLS_RSA_WITH_DES_CBC_SHATLS_RSA_EXPORT_WITH_DES40_CBC_SHATLS_RSA_WITH_IDEA_CBC_SHATLS_RSA_EXPORT_WITH_RC2_CBC_40_MD5TLS_RSA_WITH_RC4_128_SHATLS_RSA_WITH_RC4_128_MD5TLS_RSA_EXPORT_WITH_RC4_40_MD5TLS_RSA_WITH_NULL_SHATLS_RSA_WITH_NULL_MD5TLS_NULL_WITH_NULL_NULLED448ED25519RSA_PSS_SHA512RSA_PSS_SHA384RSA_PSS_SHA256ECDSA_NISTP521_SHA512ECDSA_NISTP384_SHA384ECDSA_NISTP256_SHA256ECDSA_SHA1_LegacyRSA_PKCS1_SHA1
+%%%%%%%%
+5%%9%%%%%%%%%%%%%%%%%%%%
+called `Result::unwrap()` on an `Err` value
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/cipher.rsencrypt not yet available
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/record_layer.rsb"\\x\0\t\r\n"key agreement failed/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/client/tls12.rsdowngrade to TLS1.2 when TLS1.3 is supportedServer supports ticketsrustls::client::tls12::server_helloServer may staple OCSP responseServer sent  SCTsserver sent invalid SCT listServer agreed to resumeabbreviated handshake offered, but with varied csserver varied ems support over resumeCLIENT_RANDOMApplicationDataHandshakeparsedencodedAlertversionpayload
+ChangeCipherSpec
+PoisonError/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/msgs/hsjoiner.rssessionkx-hint/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/tls12/cipher.rsencrypt failedChangeCipherSpecPayload
+$2?k:yy::Scy
+chunk size must be non-zero
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/msgs/fragmenter.rs
+Unsolicited extension rustls::client::common/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustls-0.20.8/src/client/common.rsClient auth requested but no cert/sigscheme availableAttempting client auth
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/sct-0.7.0/src/lib.rs
+UnknownLogUnsupportedSctVersionTimestampInFutureMalformedSct
+InvalidSignature
+called `Option::unwrap()` on a `None` value/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/untrusted-0.7.1/src/untrusted.rscalled `Result::unwrap()` on an `Err` value
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/webpki-0.22.0/src/name/dns_name.rsinternal error: entered unreachable codeDnsNameInvalidDnsNameErrorcalled `Result::unwrap()` on an `Err` value/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/webpki-0.22.0/src/name/ip_address.rs
 UnsupportedSignatureAlgorithmUnsupportedSignatureAlgorithmForPublicKeyUnsupportedCriticalExtensionMissingOrMalformedExtensionsUnsupportedCertVersionUnknownIssuerRequiredEkuNotFoundSignatureAlgorithmMismatchPathLenConstraintViolatedNameConstraintViolationInvalidSignatureForPublicKeyInvalidCertValidityExtensionValueInvalidEndEntityUsedAsCaCertNotValidYetCertNotValidForNameCertExpiredCaUsedAsEndEntityBadDerTimeBadDer
+called `Result::unwrap()` on an `Err` value/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/webpki-0.22.0/src/verify_cert.rs+
+	/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/untrusted-0.7.1/src/untrusted.rs
+,,,,,,,,,,,,,,,,,,,,,,,
+ "$&(*internal error: entered unreachable code/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/webpki-0.22.0/src/calendar.rs
+"InvalidEncoding/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/arithmetic/bigint.rsassertion failed: exponent >= 1assertion failed: exponent <= PUBLIC_EXPONENT_MAX_VALUE/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/limb.rs
+assertion failed: mid <= self.len()called `Result::unwrap()` on an `Err` value
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/digest.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/ec/curve25519/scalar.rs
+x+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/ec/suite_b/ops/p384.rs
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/ec/suite_b/private_key.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/ec/suite_b/ops.rsassertion failed: ops.common.elem_verify_is_not_zero(&z).is_ok()
+assertion failed: mid <= self.len()called `Result::unwrap()` on an `Err` value/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/rsa/padding.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/untrusted-0.7.1/src/untrusted.rsassertion failed: em.len() >= digest_len + 11/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/digest.rs
+attempt to divide by zeroassertion failed: ctr_max <= u32::max_value() as usizePKCS1digest_algdigestinfo_prefix
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/limb.rs
+ring::signature::ED25519
+assertion failed: digest_alg.block_len >= digest_alg.output_len/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/hkdf.rscalled `Option::unwrap()` on a `None` value/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/digest.rsassertion failed: mid <= self.len()
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/aead/aes.rscalled `Option::unwrap()` on a `None` valueinternal error: entered unreachable code/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/aead/aes_gcm.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/ec/suite_b/ops.rsassertion failed: n_min_bits >= N_MIN_BITS/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/rsa/verification.rsassertion failed: padding.iter().all(|&b| b == 0)ECDSA_P384_SHA384_FIXEDECDSA_P384_SHA384_ASN1ECDSA_P384_SHA256_ASN1ECDSA_P256_SHA384_ASN1ECDSA_P256_SHA256_FIXEDECDSA_P256_SHA256_ASN1SystemRandom
+called `Result::unwrap()` on an `Err` value
+attempt to divide by zero/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/aead/block.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/aead/shift.rs
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/digest.rscalled `Option::unwrap()` on a `None` value
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/hmac.rs
+RsaParameterspadding_alg
+min_bitsInvalidEncoding/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/limb.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/rsa/padding.rs
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/digest.rs
+attempt to divide by zerocalled `Option::unwrap()` on a `None` valueassertion failed: num_pending <= pending.len()
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/ec/suite_b/ops.rsassertion failed: !self.common.is_zero(a)SHA512_256SHA512SHA384SHA256
 called `Result::unwrap()` on an `Err` value
-	/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/webpki-0.22.0/src/verify_cert.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/untrusted-0.7.1/src/untrusted.rs
-***********************
-called `Option::unwrap()` on a `None` value/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/untrusted-0.7.1/src/untrusted.rscalled `Result::unwrap()` on an `Err` value/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/webpki-0.22.0/src/name/ip_address.rs2
-!#%')+-/1internal error: entered unreachable code/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/webpki-0.22.0/src/calendar.rsring::signature::ED25519
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/ec/suite_b/ops.rsassertion failed: !self.common.is_zero(a)InvalidComponentTooSmallTooLargeUnexpectedErrorUnspecified
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/digest.rsassertion failed: digest_alg.block_len >= digest_alg.output_len/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/hkdf.rscalled `Option::unwrap()` on a `None` valuecalled `Result::unwrap()` on an `Err` valueassertion failed: mid <= self.len()/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/rsa/padding.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/untrusted-0.7.1/src/untrusted.rsassertion failed: em.len() >= digest_len + 11/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/digest.rs
-attempt to divide by zeroassertion failed: ctr_max <= u32::max_value() as usizePKCS1digest_algdigestinfo_prefix010
-internal error: entered unreachable code/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/aead/chacha20_poly1305.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/limb.rsinternal error: entered unreachable codeOnce has panicked/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/spin-0.5.2/src/once.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/ec/suite_b/ops.rs/dev/urandomECDSA_P384_SHA384_FIXEDECDSA_P384_SHA384_ASN1ECDSA_P384_SHA256_ASN1ECDSA_P256_SHA384_ASN1ECDSA_P256_SHA256_FIXEDECDSA_P256_SHA256_ASN1
-CHACHA20/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/aead/aes.rscalled `Option::unwrap()` on a `None` valueinternal error: entered unreachable code/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/aead/aes_gcm.rsassertion failed: mid <= self.len()called `Result::unwrap()` on an `Err` value/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/aead/block.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/aead/shift.rs
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/digest.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/ec/curve25519/scalar.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/ec/keys.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/ec/suite_b/ecdsa/digest_scalar.rsassertion failed: n_min_bits >= N_MIN_BITS/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/rsa/verification.rsassertion failed: padding.iter().all(|&b| b == 0)SystemRandomRsaParameterspadding_algmin_bits()
-called `Result::unwrap()` on an `Err` valueLazy instance has previously been poisoned/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/once_cell-1.18.0/src/lib.rsassertion failed: mid <= self.len()/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/aead.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/digest.rs
-attempt to divide by zerocalled `Option::unwrap()` on a `None` value/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/hmac.rsInvalidEncoding/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/limb.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/rsa/padding.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/digest.rs
-attempt to divide by zerocalled `Option::unwrap()` on a `None` valueassertion failed: num_pending <= pending.len()/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/ec/suite_b/ops.rsSHA512_256SHA512SHA384SHA256
-+1/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/std/src/io/mod.rsfailed to fill whole buffercalled `Result::unwrap()` on an `Err` value/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/ec/suite_b/private_key.rs
-BitLength
-A(Vector Permutation AES for ARMv8, Mike Hamburg (Stanford University)
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/ec/keys.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/ec/suite_b/private_key.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/ec/suite_b/ops/p256.rs
+InvalidComponent
+TooSmallTooLarge
+UnexpectedErrorUnspecified
+assertion failed: mid <= self.len()called `Result::unwrap()` on an `Err` value/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/aead.rs
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/ec/suite_b/ops.rs
+called `Result::unwrap()` on an `Err` valueinternal error: entered unreachable code/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/aead/chacha20_poly1305.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/digest.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/ec/suite_b/ecdsa/digest_scalar.rsBitLength
 expand 32-byte k
 ChaCha20 for ARMv8, CRYPTOGAMS by <appro@openssl.org>
-GHASH for ARMv8, derived from ARMv4 version by <appro@openssl.org>
 SHA512 block transform for ARMv8, CRYPTOGAMS by <appro@openssl.org>
 SHA256 block transform for ARMv8, CRYPTOGAMS by <appro@openssl.org>
 sJfw>7G9@>
 t0;?ZlP*m
 *D]WO"#y&
 $>Mm/JhA
 Y93a=7c@
@@ -1079,68 +1171,29 @@
 m>FC*a7H
  T;6P/Arc
 }9]Jn+LhyK
 C!OFtq74
 tA`KO/3G!
 Iw,e=2-b[
 !D]#t^;Gc
-InvalidEncoding/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/arithmetic/bigint.rsassertion failed: exponent >= 1assertion failed: exponent <= PUBLIC_EXPONENT_MAX_VALUE/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/limb.rsassertion failed: mid <= self.len()called `Result::unwrap()` on an `Err` value
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/ec/suite_b/private_key.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ring-0.16.20/src/ec/suite_b/ops.rsassertion failed: ops.common.elem_verify_is_not_zero(&z).is_ok()
 EndOfInput
-called `Result::unwrap()` on an `Err` value/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/mproxy-server-0.1.7/src/lib.rsparsing socket addressbinding server socket
+called `Result::unwrap()` on an `Err` value/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/mproxy-server-0.1.7/src/lib.rsparsing socket addressbinding server socketcould not resolve to any addresses
+called `Result::unwrap()` on an `Err` value/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/mproxy-client-0.1.7/src/lib.rsparsing socket addressbinding client socketGetting default network interfacecould not resolve to any addressesDefault Interface not foundLocal IP address not foundAttempted to create a NULL object./Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/system-configuration-0.5.1/src/network_configuration.rsNot supportedassertion failed: len as usize >= mem::size_of::<SockAddrIn6>()/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/default-net-0.14.1/src/sys/unix.rsassertion failed: len as usize >= mem::size_of::<SockAddrIn>()/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/default-net-0.14.1/src/socket/packet.rs0.0.0.0:0Failed to create UDP socket 1.1.1.1:80Failed to set TTL Failed to send data no addresses to send data tocalled `Result::unwrap()` on an `Err` value
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/default-net-0.14.1/src/interface/unix.rs
+called `Result::unwrap()` on an `Err` value/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/libc-0.2.146/src/unix/bsd/mod.rs
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/default-net-0.14.1/src/bpf/unix.rscalled `Option::unwrap()` on a `None` valueTimed out
+/dev/bpf0.0.0.0:01.1.1.1:80
+a Display implementation returned an error unexpectedly/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/alloc/src/string.rs
+chunk size must be non-zero/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/libc-0.2.146/src/unix/bsd/mod.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/default-net-0.14.1/src/bpf/unix.rsTimed outFailed to create channel Failed to send UDP packet Recieve timeout
 could not resolve to any addresses
-called `Result::unwrap()` on an `Err` value/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/mproxy-client-0.1.7/src/lib.rsparsing socket addressbinding client socketcould not resolve to any addresses
-/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/core/src/str/pattern.rscalled `Result::unwrap()` on an `Err` valueError while closing SQLite connection: 
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/inner_connection.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/cache.rswrong msg typeaisdb_lib/src/decode.rscalled `Option::unwrap()` on a `None` valuec:unknown file type! nmeaNMEA    elapsed: srate:  msgs/s count:getting db connCannot open .nm4 file ^^X
-VYkcalled `Option::unwrap()` on a `None` value/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/alloc/src/collections/btree/navigate.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-0.19.5/src/connection.rs
-writing;FieldSet corrupted (this is a bug)flushing framed transport/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-util-0.7.8/src/codec/framed_impl.rsfailed to write frame to transportframed transport flushedReturning None and setting pausedattempting to decode a frameframe decoded from bufferGot an error, going to errored state/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/csv-1.2.2/src/byte_record.rscalled `Result::unwrap()` on an `Err` valueError while closing SQLite connection: 
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/inner_connection.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/cache.rs%Y%m%d_%H%M%S%Y%m%dT%H%M%SZaisdb_lib/src/csvreader.rsparsing timestamp from '': called `Option::unwrap()` on a `None` value.csvgetting db connelapsed: srate:  msgs/s count:cannot open file 
-password missingapplication_name
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/message/backend.rsinvalid message length: expected to be at end of iterator for saslbytes remaining on stream/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/connect_raw.rs
-`async fn` resumed after panicking
-`async fn` resumed after completionunsupported authentication methoduser missingSCRAM-SHA-256-PLUSSCRAM-SHA-256unsupported SASL mechanismclient_encodingUTF8userdatabaseglob diroptions/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/connect_tls.rsserver does not support TLS/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/connect_socket.rs.s.PGSQL.could not resolve any addressesconnection timed out/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/config.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/connect.rsSHOW transaction_read_onlydatabase does not allow writeshost missinginvalid number of ports
-md5unexpected EOFvalue too large to transmit/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/message/frontend.rsstring contains embedded nulldescription() is deprecated; use Displayassertion failed: mid <= self.len()called `Option::unwrap()` on a `None` valuecalled `Result::unwrap()` on an `Err` value/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/alloc/src/collections/btree/navigate.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/net/lookup_host.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/net/tcp/stream.rscould not resolve to any addressassertion failed: 4 <= buf.len()/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/net/unix/stream.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/byteorder-1.4.3/src/lib.rscannot advance past `remaining`: /root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/bytes-1.4.0/src/bytes.rsfatal runtime error: 
-thread result panicked on drop`Ready` polled after completion/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/core/src/future/ready.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/io/poll_evented.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-0.19.5/src/transaction.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-0.19.5/src/config.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/io/util/write_all.rsaisdb_lib/src/util.rsgetting current timestamp
-R/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/core/src/str/pattern.rs
-R/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/io/read_buf.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-util-0.7.8/src/lib.rs
-cannot advance past `remaining`: /root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/bytes-1.4.0/src/bytes_mut.rsnew_len = ; capacity = 
-: tokio_postgres::connection/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/connection.rspoll_flush: waiting on socketpoll_flush: flushedpoll_write: donepoll_write: waiting on socketpoll_write: waiting on requestpoll_write: at eof, terminating/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/message/frontend.rspoll_write: waiting on copy_in streampoll_write: finished copy_in requestpoll_write: sent eof, closingpoll_write: at eof, pending responses polled new requestretrying pending requestretrying pending responsepoll_shutdown: waiting on socketpoll_shutdown: completepoll_read: donepoll_read: waiting on responseinternal error: entered unreachable codepoll_read: waiting on sendervalue too large to transmitcalled `Result::unwrap()` on an `Err` value/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/byteorder-1.4.3/src/lib.rscannot advance past `remaining`: /root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/bytes-1.4.0/src/bytes.rs
-&&&&&&&&!
-invalid message length: parameters is not drained/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/transaction.rs
-`async fn` resumed after panicking
-`async fn` resumed after completion/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/simple_query.rsexecuting simple query: tokio_postgres::simple_query/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/to_statement.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/query.rstokio_postgres::queryexecuting statement  with parameters: /root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/client.rs
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/prepare.rsSELECT t.typname, t.typtype, t.typelem, r.rngsubtype, t.typbasetype, n.nspname, t.typrelid
-FROM pg_catalog.pg_type t
-LEFT OUTER JOIN pg_catalog.pg_range r ON r.rngtypid = t.oid
-INNER JOIN pg_catalog.pg_namespace n ON t.typnamespace = n.oid
-WHERE t.oid = $1
-SELECT t.typname, t.typtype, t.typelem, NULL::OID, t.typbasetype, n.nspname, t.typrelid
-FROM pg_catalog.pg_type t
-INNER JOIN pg_catalog.pg_namespace n ON t.typnamespace = n.oid
-WHERE t.oid = $1
-SELECT enumlabel
-FROM pg_catalog.pg_enum
-WHERE enumtypid = $1
-ORDER BY enumsortorder
-SELECT enumlabel
-FROM pg_catalog.pg_enum
-WHERE enumtypid = $1
-ORDER BY oid
-SELECT attname, atttypid
-FROM pg_catalog.pg_attribute
-WHERE attrelid = $1
-AND NOT attisdropped
-AND attnum > 0
-ORDER BY attnum
-s/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/message/backend.rsunexpected EOFvalue too large to transmit/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/message/frontend.rsstring contains embedded null
-called `Option::unwrap()` on a `None` value/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/csv-1.2.2/src/byte_record.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/csv-1.2.2/src/reader.rsassertion failed: line > 0failed to fill whole buffercore::option::Option<u32>u32i8alloc::string::Stringdescription() is deprecated; use Display/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/byteorder-1.4.3/src/lib.rsassertion failed: 2 <= buf.len()assertion failed: fd >= 0/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/socket2-0.5.3/src/sockref.rsinvalid message length: field is not drained
-()a Display implementation returned an error unexpectedly/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/alloc/src/string.rs
-/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/core/src/str/pattern.rscalled `Result::unwrap_err()` on an `Ok` valuecalled `Result::unwrap()` on an `Err` valueError while closing SQLite connection: 
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/inner_connection.rsalready mutably borrowed/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/lib.rsBEGIN DEFERREDCOMMIT
-ROLLBACK:memory:/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/cache.rsSQLite version string is not valid UTF8 ?!/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/version.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/statement.rscoarsetype.sqlCREATE TABLE coarsetype_ref (
+Attempted to create a NULL object.
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/core-foundation-0.9.3/src/string.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/core-foundation-0.9.3/src/array.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/core-foundation-0.9.3/src/string.rs
+()a Display implementation returned an error unexpectedly/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/alloc/src/string.rs
+/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/core/src/str/pattern.rscalled `Result::unwrap_err()` on an `Ok` valuecalled `Result::unwrap()` on an `Err` valueError while closing SQLite connection: 
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/inner_connection.rsalready mutably borrowed/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/lib.rsBEGIN DEFERREDCOMMIT/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/cache.rsSQLite version string is not valid UTF8 ?!/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/version.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/statement.rscoarsetype.sqlCREATE TABLE coarsetype_ref (
     coarse_type integer,
     coarse_type_txt character varying(75),
     PRIMARY KEY (coarse_type)
 INSERT INTO coarsetype_ref VALUES(20,'Wing In Grnd');
 INSERT INTO coarsetype_ref VALUES(21,'Wing In Grnd, hazardous category A');
 INSERT INTO coarsetype_ref VALUES(22,'Wing In Grnd, hazardous category B');
 INSERT INTO coarsetype_ref VALUES(23,'Wing In Grnd, hazardous category C');
@@ -1255,15 +1308,15 @@
     fixing_device TEXT,
     eta_month INTEGER,
     eta_day INTEGER,
     eta_hour INTEGER,
     eta_minute INTEGER,
     source TEXT NOT NULL,
     PRIMARY KEY (mmsi, time, imo, source)
-createtable_static_aggregate.sqlinsert_webdata_marinetraffic.sqlCREATE TABLE static_{}_aggregate (
+createtable_static_aggregate.sqlCREATE TABLE static_{}_aggregate (
     mmsi INTEGER PRIMARY KEY,
     imo INTEGER,
     vessel_name TEXT,
     ship_type INTEGER,
     call_sign TEXT,
     dim_bow INTEGER,
     dim_stern INTEGER,
@@ -1352,15 +1405,15 @@
     eta_month,
     eta_day,
     eta_hour,
     eta_minute,
     source
 VALUES ($1,$2,$3,$4,$5,$6,$7,$8,$9,$10,$11,$12,$13,$14,$15,$16,$17,$18,$19)
 ON CONFLICT DO NOTHING
-INSERT INTO webdata_marinetraffic (
+insert_webdata_marinetraffic.sqlINSERT INTO webdata_marinetraffic (
     mmsi, 
     imo, 
     name,
     vesseltype_generic,
     vesseltype_detailed,
     callsign,
     flag,
@@ -1466,161 +1519,756 @@
     SELECT DISTINCT mmsi FROM ais_{}_dynamic
   ) as d_{}
   LEFT JOIN webdata_marinetraffic ON
     d_{}.mmsi = webdata_marinetraffic.mmsi
   WHERE webdata_marinetraffic.error404 != 1
 called `Option::unwrap()` on a `None` valueaisdb_lib/src/db.rsfile:SQLite3 version is too low! Need version 3.8.2 or higherConnected to postgres server
 {}creating dynamic table
-creating static table%m%d%H%Mpreparing SQL statement:
+creating static table
+%m%d%H%Mpreparing SQL statement:
 executing prepared row
 executing prepared row:
-%Y%mcreating dynamic tableinsert dynamiccreate static tableinsert static: get epoch
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/generic-array-0.14.7/src/hex.rsassertion failed: (*tail).value.is_none()/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/futures-channel-0.3.28/src/mpsc/queue.rsassertion failed: (*next).value.is_some()/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/std/src/io/mod.rsstream did not contain valid UTF-8fatal runtime error: 
-thread local panicked on drop
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/message/backend.rsinvalid message length: expected to be at end of iterator for sasl`NaiveDateTime + Duration` overflowed/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/naive/datetime/mod.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/connect_raw.rs
+creating dynamic tableinsert dynamiccreate static tableinsert static: get epoch
+ROLLBACK:memory:%Y%m
+!#%')+-/13579;=?ACEGIKMOQSUWY[]_
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/lib.rs/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/std/src/io/mod.rsfailed to write whole bufferformatter errorfatal runtime error: thread local panicked on drop
+value too large to transmitassertion failed: 4 <= buf.len()/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/byteorder-1.4.3/src/lib.rsassertion failed: fd >= 0/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/socket2-0.5.3/src/sockref.rsalready mutably borrowed/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/lib.rs
+aisdb_lib/src/util.rsgetting current timestamp
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/futures-channel-0.3.28/src/mpsc/mod.rsbuffer space exhausted; sending this messages would overflow the statecalled `Result::unwrap()` on an `Err` valuecalled `Option::unwrap()` on a `None` value
+llIMQlllX
+bytes remaining on stream
+description() is deprecated; use Displayassertion failed: mid <= self.len()called `Result::unwrap()` on an `Err` value/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/net/tcp/stream.rs
+`async fn` resumed after panicking
+`async fn` resumed after completioncould not resolve to any address/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/net/unix/stream.rscannot access a Thread Local Storage value during or after destruction/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/std/src/thread/local.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/context.rsfatal runtime error: thread result panicked on drop
+`Ready` polled after completion/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/core/src/future/ready.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-0.19.5/src/connection.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-0.19.5/src/config.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/io/util/write_all.rs
+YY6:>YYYE
+/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/core/src/str/pattern.rscalled `Result::unwrap()` on an `Err` valueError while closing SQLite connection: 
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/inner_connection.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/cache.rswrong msg typeaisdb_lib/src/decode.rscalled `Option::unwrap()` on a `None` valuec:unknown file type! elapsed: srate:  msgs/s count:getting db connCannot open .nm4 file @
+FieldSet corrupted (this is a bug)flushing framed transport
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-util-0.7.8/src/codec/framed_impl.rsfailed to write frame to transportframed transport flushedReturning None and setting pausedattempting to decode a frameframe decoded from bufferGot an error, going to errored state
+writing;
+password missingapplication_name
+1?M59IO%#W
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/message/backend.rsinvalid message length: expected to be at end of iterator for sasl/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/connect_raw.rs
 `async fn` resumed after panicking
-`async fn` resumed after completionunsupported authentication methoduser missingSCRAM-SHA-256-PLUSSCRAM-SHA-256unsupported SASL mechanismclient_encodingoptions/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/connect_tls.rsserver does not support TLS/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/connect_socket.rs.s.PGSQL.could not resolve any addressesconnection timed out/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/config.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/connect.rsSHOW transaction_read_onlydatabase does not allow writeshost missinginvalid number of ports
-md5value too large to transmit/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/lib.rsunexpected EOF/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/message/frontend.rsstring contains embedded null/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/std/src/io/mod.rsfailed to write whole bufferformatter errora Display implementation returned an error unexpectedly/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/alloc/src/string.rscalled `Option::unwrap()` on a `None` valuecalled `Result::unwrap()` on an `Err` value/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/net/lookup_host.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/net/tcp/stream.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/net/unix/stream.rsFailed to `Enter::block_on`/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/scheduler/current_thread.rscore missinga spawned task panicked and the runtime is configured to shut down on unhandled panic/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/byteorder-1.4.3/src/lib.rscannot advance past `remaining`: /root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/bytes-1.4.0/src/bytes.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/offset/fixed.rs`Ready` polled after completion/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/core/src/future/ready.rsalready mutably borrowed/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/lib.rs
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/row.rsa Display implementation returned an error unexpectedly/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/alloc/src/string.rsdescription() is deprecated; use Display/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/util/slab.rspage is unallocatedunexpected pointerassertion failed: idx < self.slots.len()PoisonError
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/futures-channel-0.3.28/src/mpsc/mod.rsbuffer space exhausted; sending this messages would overflow the statecalled `Result::unwrap()` on an `Err` valuecalled `Option::unwrap()` on a `None` value
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/message/frontend.rsvalue too large to transmitstring contains embedded nullcannot access a Thread Local Storage value during or after destruction/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/std/src/thread/local.rs
-!$'+.158;naninfcalled `Result::unwrap()` on an `Err` value/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/net/tcp/stream.rs
+`async fn` resumed after completionunsupported authentication methoduser missingSCRAM-SHA-256-PLUSSCRAM-SHA-256unsupported SASL mechanismclient_encodingoptions/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/connect_tls.rsserver does not support TLS/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/connect_socket.rs.s.PGSQL.could not resolve any addressesconnection timed out/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/row.rs
+core::option::Option<u32>alloc::string::Stringu32i8
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/message/frontend.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/config.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/connect.rsSHOW transaction_read_only
+database does not allow writeshost missinginvalid number of portsmd5unexpected EOF
+string contains embedded null/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/std/src/io/mod.rsstream did not contain valid UTF-8a Display implementation returned an error unexpectedly/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/alloc/src/string.rs
+called `Option::unwrap()` on a `None` valuecalled `Result::unwrap()` on an `Err` valuevalue too large to transmit
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/net/lookup_host.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/net/tcp/stream.rscould not resolve to any address/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/net/unix/stream.rsassertion failed: 4 <= buf.len()/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/byteorder-1.4.3/src/lib.rscannot advance past `remaining`: /Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/bytes-1.4.0/src/bytes.rs`Ready` polled after completion/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/core/src/future/ready.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/io/poll_evented.rspolled Feed after completion/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/futures-util-0.3.28/src/sink/feed.rs
+UTF8user
+database
+: tokio_postgres::connection/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/connection.rspoll_flush: waiting on socketpoll_flush: flushedpoll_write: waiting on socketpoll_write: waiting on requestpoll_write: at eof, terminating/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/message/frontend.rspoll_write: waiting on copy_in streampoll_write: finished copy_in requestpoll_write: sent eof, closingpoll_write: at eof, pending responses polled new requestretrying pending requestretrying pending responsepoll_shutdown: waiting on socketpoll_shutdown: completepoll_read: donepoll_read: waiting on responseinternal error: entered unreachable codepoll_read: waiting on sendercalled `Result::unwrap()` on an `Err` valuevalue too large to transmitassertion failed: 4 <= buf.len()/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/byteorder-1.4.3/src/lib.rscannot advance past `remaining`: /Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/bytes-1.4.0/src/bytes.rs
+poll_write: done)
+&&&&&&&&!
+Einvalid message length: parameters is not drained/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/message/backend.rsinvalid message length: expected to be at end of iterator for sasl/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/io/read_buf.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-util-0.7.8/src/lib.rs
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/connect_raw.rs
 `async fn` resumed after panicking
-`async fn` resumed after completion/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/net/unix/stream.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/task/list.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/context.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/scheduler/current_thread.rs
-attempt to calculate the remainder with a divisor of zero/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/byteorder-1.4.3/src/lib.rscannot advance past `remaining`: /root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/bytes-1.4.0/src/bytes.rs`Ready` polled after completion/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/core/src/future/ready.rspolled Feed after completion/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/futures-util-0.3.28/src/sink/feed.rsG,G
-called `Result::unwrap_err()` on an `Ok` value/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/statement.rsalready mutably borrowed/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/lib.rsPoisonErrorcalled `Option::unwrap()` on a `None` value/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/alloc/src/collections/btree/navigate.rs
-BlobRealtailInteger
- in  at offset Wrong number of parameters passed to query. Got , needed Multiple statements providedQuery is not read-onlyQuery changed  rowsInvalid column type  at index: , name: Integer NulErrorInvalid column name: Invalid column index: Query returned no rowsExecute returned results - did you mean to call query?Invalid path: Invalid parameter name:  out of range at index  out of rangeConversion error from type , SQLite was compiled or configured for single-threaded use onlySqlInputErrorerrormsgsqloffsetInvalidParameterCountMultipleStatementInvalidQueryToSqlConversionFailureStatementChangedRowsInvalidColumnTypeInvalidColumnNameInvalidColumnIndexQueryReturnedNoRowsExecuteReturnedResultsInvalidPathInvalidParameterNameUtf8ErrorIntegralValueOutOfRangeFromSqlConversionFailureSqliteSingleThreadedModeSqliteFailure
-called `Result::unwrap()` on an `Err` value: /root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/inner_connection.rsBug: Somehow interrupt_lock was cleared before the DB was closed&(
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/cache.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/lib.rsalready mutably borrowedcalled `Result::unwrap()` on an `Err` value/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/alloc/src/sync.rscalled `Option::unwrap()` on a `None` value/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/alloc/src/collections/btree/navigate.rs
-Pinternal error: entered unreachable code: state is never set to invalid values
-Once instance has previously been poisonedcalled `Option::unwrap()` on a `None` value/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/std/src/sync/once.rsCould not ensure safe initialization of SQLite.
+`async fn` resumed after completionunsupported authentication methoduser missingSCRAM-SHA-256-PLUSSCRAM-SHA-256unsupported SASL mechanismclient_encodingoptions/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/connect_tls.rsserver does not support TLS/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/transaction.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/simple_query.rsexecuting simple query: tokio_postgres::simple_query/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/to_statement.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/connect_socket.rs.s.PGSQL.could not resolve any addressesconnection timed out/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/query.rstokio_postgres::queryexecuting statement  with parameters: /Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/client.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/config.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/connect.rsSHOW transaction_read_only
+database does not allow writeshost missinginvalid number of ports/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/prepare.rsSELECT t.typname, t.typtype, t.typelem, r.rngsubtype, t.typbasetype, n.nspname, t.typrelid
+FROM pg_catalog.pg_type t
+LEFT OUTER JOIN pg_catalog.pg_range r ON r.rngtypid = t.oid
+INNER JOIN pg_catalog.pg_namespace n ON t.typnamespace = n.oid
+WHERE t.oid = $1
+SELECT t.typname, t.typtype, t.typelem, NULL::OID, t.typbasetype, n.nspname, t.typrelid
+FROM pg_catalog.pg_type t
+INNER JOIN pg_catalog.pg_namespace n ON t.typnamespace = n.oid
+WHERE t.oid = $1
+SELECT enumlabel
+FROM pg_catalog.pg_enum
+WHERE enumtypid = $1
+ORDER BY enumsortorder
+SELECT enumlabel
+FROM pg_catalog.pg_enum
+WHERE enumtypid = $1
+ORDER BY oid
+SELECT attname, atttypid
+FROM pg_catalog.pg_attribute
+WHERE attrelid = $1
+AND NOT attisdropped
+AND attnum > 0
+ORDER BY attnum
+smd5unexpected EOF/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/message/frontend.rsstring contains embedded nullfailed to fill whole buffer
+called `Option::unwrap()` on a `None` valuecalled `Result::unwrap()` on an `Err` valuevalue too large to transmit/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/net/lookup_host.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/net/tcp/stream.rscould not resolve to any address/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/net/unix/stream.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/byteorder-1.4.3/src/lib.rsassertion failed: 4 <= buf.len()cannot advance past `remaining`: /Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/bytes-1.4.0/src/bytes.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/bytes-1.4.0/src/bytes_mut.rsnew_len = ; capacity = PoisonError`Ready` polled after completion/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/core/src/future/ready.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-0.19.5/src/transaction.rsinvalid message length: field is not drained
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/generic-array-0.14.7/src/hex.rs
+called `Option::unwrap()` on a `None` value/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/alloc/src/collections/btree/navigate.rscannot access a Thread Local Storage value during or after destruction/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/std/src/thread/local.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/task/list.rsFailed to `Enter::block_on`/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/scheduler/current_thread.rscore missinga spawned task panicked and the runtime is configured to shut down on unhandled panic
+attempt to calculate the remainder with a divisor of zero
+`NaiveDateTime + Duration` overflowed/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/naive/datetime/mod.rs
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/prepare.rs
+`async fn` resumed after panicking
+`async fn` resumed after completion/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/message/frontend.rsstring contains embedded null
+a Display implementation returned an error unexpectedly/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/alloc/src/string.rs
+called `Option::unwrap()` on a `None` value
+value too large to transmit/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/util/slab.rspage is unallocatedunexpected pointerassertion failed: idx < self.slots.len()assertion failed: 2 <= buf.len()/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/byteorder-1.4.3/src/lib.rsassertion failed: 4 <= buf.len()/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/offset/fixed.rs
+assertion failed: (*tail).value.is_none()/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/futures-channel-0.3.28/src/mpsc/queue.rsassertion failed: (*next).value.is_some()called `Option::unwrap()` on a `None` value/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/csv-1.2.2/src/byte_record.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/csv-1.2.2/src/reader.rsassertion failed: line > 0
+i/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/csv-1.2.2/src/byte_record.rs
+called `Result::unwrap()` on an `Err` valueError while closing SQLite connection: 
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/inner_connection.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/cache.rs%Y%m%d_%H%M%S%Y%m%dT%H%M%SZaisdb_lib/src/csvreader.rsparsing timestamp from '': 
+called `Option::unwrap()` on a `None` value
+getting db connelapsed: srate:  msgs/s count:cannot open file 
+llIMQlllX/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/core/src/str/pattern.rs
+called `Result::unwrap_err()` on an `Ok` value
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/statement.rs
+already mutably borrowed
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/lib.rsPoisonErrorcalled `Option::unwrap()` on a `None` value/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/alloc/src/collections/btree/navigate.rs
+BlobReal
+(7COVbhnz
+ at offset Wrong number of parameters passed to query. Got , needed Multiple statements providedQuery is not read-onlyQuery changed  rowsInvalid column type  at index: Invalid column name: Invalid column index: Query returned no rowsExecute returned results - did you mean to call query?Invalid path: Invalid parameter name:  out of range at index  out of rangeConversion error from type , SQLite was compiled or configured for single-threaded use onlySqlInputErrorerrormsgsqloffsetInvalidParameterCountMultipleStatementInvalidQueryToSqlConversionFailureStatementChangedRowsInvalidColumnTypeInvalidColumnNameInvalidColumnIndexQueryReturnedNoRowsExecuteReturnedResultsInvalidPathInvalidParameterNameUtf8ErrorIntegralValueOutOfRangeFromSqlConversionFailureSqliteSingleThreadedModeSqliteFailure, name: Integer 	
+$'*called `Option::unwrap()` on a `None` value/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/std/src/sync/once.rs
+called `Result::unwrap()` on an `Err` value: /Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/inner_connection.rsBug: Somehow interrupt_lock was cleared before the DB was closed
+Could not ensure safe initialization of SQLite.
 To fix this, either:
 * Upgrade SQLite to at least version 3.7.0
 * Ensure that SQLite has been initialized in Multi-thread or Serialized mode and call
-rusqlite::bypass_sqlite_initialization() prior to your first connection attempt./root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/inner_connection.rs
-Hash table capacity overflow/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/hashbrown-0.13.2/src/raw/mod.rs
-Error code : Unknown error codeSQLITE_AUTH_USEROperationAbortedPermissionDeniedAutomatic indexing used - database might benefit from additional indexesHot journal was rolled backA WAL mode database file was recoveredSQLITE_CONSTRAINT_DATATYPESQLITE_CONSTRAINT_PINNEDA non-unique rowid occurredAn application-defined virtual table error occurredA UNIQUE constraint failedA RAISE function within a trigger firedA PRIMARY KEY constraint failedA NOT NULL constraint failedError returned from extension functionForeign key constraint failedCommit hook caused rollbackA CHECK constraint failedTransaction was rolled backSQLITE_READONLY_DIRECTORYSQLITE_READONLY_CANTINITDatabase cannot be modified because database file has movedDatabase has hot journal that must be rolled back (requires write access)Shared-memory file associated with WAL mode database is read-onlyWAL mode database file needs recovery (requires write access)SQLITE_CORRUPT_INDEXSQLITE_CORRUPT_SEQUENCEContent in the virtual table is corruptSQLITE_CANTOPEN_SYMLINKcygwin_conv_path() system call failedUnable to convert filename into full pathnameAttempted to open directory as fileSQLITE_CANTOPEN_NOTEMPDIRSQLITE_BUSY_TIMEOUTCannot promote read transaction to write transaction because of writes by another connectionAnother process is recovering a WAL mode database fileSQLITE_LOCKED_VTABLocking conflict due to another connection with a shared cacheSQLITE_IOERR_DATASQLITE_IOERR_ROLLBACK_ATOMICSQLITE_IOERR_COMMIT_ATOMICSQLITE_IOERR_BEGIN_ATOMICSQLITE_IOERR_AUTHSQLITE_IOERR_VNODEVFS is unable to determine a suitable directory for temporary filesI/O error while trying to map or unmap part of the database file into process address spaceFile being deleted does not existI/O error within the xRead or xWrite (trying to seek within a file)I/O error within the xShmMap method (trying to map a shared-memory segment into process address space)SQLITE_IOERR_SHMLOCKI/O error within the xShmMap method (trying to resize an existing shared-memory segment)I/O error within the xShmMap method (trying to open a new shared-memory segment)SQLITE_IOERR_DIR_CLOSEI/O error within the xClose methodI/O error in the advisory file locking layerI/O error within then xCheckReservedLock methodI/O error within xAccess of a VFS objectOut of memory in I/O layerSQLITE_IOERR_BLOCKEDI/O error within xDelete of a VFS objectI/O error within xLock of a VFS object (trying to obtain a read lock)I/O error within xUnlock of a VFS objectError invoking fstat to get file metadataError attempting to truncate fileError calling fsync on a directoryError flushing data to persistent storage (fsync)Error writing to diskUnable to obtain number of requested bytes (file truncated?)Error reading from diskSQLITE_ERROR_SNAPSHOTSQLITE_ERROR_RETRYSQLITE_ERROR_MISSING_COLLSEQsqlite3_step() has finished executingsqlite3_step() has another row readyWarnings from sqlite3_log()Notifications from sqlite3_log()Unable to open the database fileFile opened that is not a database file2nd parameter to sqlite3_bind out of rangeAuxiliary database format errorAuthorization deniedUses OS features not supported on hostLibrary used incorrectlyData type mismatchAbort due to constraint violationString or BLOB exceeds size limitThe database schema changedDatabase is emptyDatabase lock protocol errorInsertion failed because database is fullUnknown opcode in sqlite3_file_control()The database disk image is malformedSome kind of disk I/O error occurredOperation terminated by sqlite3_interrupt()Attempt to write a readonly databaseA malloc() failedA table in the database is lockedThe database file is lockedCallback routine requested an abortAccess permission deniedInternal logic error in SQLiteSQL error or missing databaseSuccessful resultUnknownNotADatabaseParameterOutOfRangeAuthorizationForStatementDeniedNoLargeFileSupportApiMisuseTypeMismatchConstraintViolationTooBigSchemaChangedFileLockingProtocolFailedCannotOpenDiskFullNotFoundReadOnlyDatabaseCorruptSystemIoFailureOperationInterruptedOutOfMemoryDatabaseLockedDatabaseBusyInternalMalfunctionErrorextended_code
-Wrong number of columns for an rtree table
-Too few columns for an rtree table
-Too many columns for an rtree table
-Auxiliary rtree columns must be last
-highlight
-unicode61
-CREATE TABlE vocab(term, col, doc, cnt)
-CREATE TABlE vocab(term, doc, cnt)
-CREATE TABlE vocab(term, doc, col, offset)
-SELECT %s FROM %s T WHERE T.%Q >= ? AND T.%Q <= ? ORDER BY T.%Q ASC
-SELECT %s FROM %s T WHERE T.%Q <= ? AND T.%Q >= ? ORDER BY T.%Q DESC
-SELECT %s FROM %s T WHERE T.%Q=?
-INSERT INTO %Q.'%q_content' VALUES(%s)
-REPLACE INTO %Q.'%q_content' VALUES(%s)
-DELETE FROM %Q.'%q_content' WHERE id=?
-REPLACE INTO %Q.'%q_docsize' VALUES(?,?)
-DELETE FROM %Q.'%q_docsize' WHERE id=?
-SELECT sz FROM %Q.'%q_docsize' WHERE id=?
-REPLACE INTO %Q.'%q_config' VALUES(?,?)
-SELECT %s FROM %s AS T
-DELETE FROM %Q.'%q_content' WHERE rowid = ?
-SELECT NOT EXISTS(SELECT docid FROM %Q.'%q_content' WHERE rowid!=?)
-DELETE FROM %Q.'%q_content'
-DELETE FROM %Q.'%q_segments'
-DELETE FROM %Q.'%q_segdir'
-DELETE FROM %Q.'%q_docsize'
-DELETE FROM %Q.'%q_stat'
-SELECT %s WHERE rowid=?
-SELECT (SELECT max(idx) FROM %Q.'%q_segdir' WHERE level = ?) + 1
-REPLACE INTO %Q.'%q_segments'(blockid, block) VALUES(?, ?)
-SELECT coalesce((SELECT max(blockid) FROM %Q.'%q_segments') + 1, 1)
-REPLACE INTO %Q.'%q_segdir' VALUES(?,?,?,?,?,?)
-SELECT idx, start_block, leaves_end_block, end_block, root FROM %Q.'%q_segdir' WHERE level = ? ORDER BY idx ASC
-SELECT idx, start_block, leaves_end_block, end_block, root FROM %Q.'%q_segdir' WHERE level BETWEEN ? AND ?ORDER BY level DESC, idx ASC
-SELECT count(*) FROM %Q.'%q_segdir' WHERE level = ?
-SELECT max(level) FROM %Q.'%q_segdir' WHERE level BETWEEN ? AND ?
-DELETE FROM %Q.'%q_segdir' WHERE level = ?
-DELETE FROM %Q.'%q_segments' WHERE blockid BETWEEN ? AND ?
-DELETE FROM %Q.'%q_docsize' WHERE docid = ?
-SELECT size FROM %Q.'%q_docsize' WHERE docid=?
-SELECT value FROM %Q.'%q_stat' WHERE id=?
-REPLACE INTO %Q.'%q_stat' VALUES(?,?)
-DELETE FROM %Q.'%q_segdir' WHERE level BETWEEN ? AND ?
-SELECT ? UNION SELECT level / (1024 * ?) FROM %Q.'%q_segdir'
-SELECT level, count(*) AS cnt FROM %Q.'%q_segdir'   GROUP BY level HAVING cnt>=?  ORDER BY (level %% 1024) ASC, 2 DESC LIMIT 1
-SELECT 2 * total(1 + leaves_end_block - start_block)   FROM (SELECT * FROM %Q.'%q_segdir'         WHERE level = ? ORDER BY idx ASC LIMIT ?  )
-DELETE FROM %Q.'%q_segdir' WHERE level = ? AND idx = ?
-UPDATE %Q.'%q_segdir' SET idx = ? WHERE level=? AND idx=?
-SELECT idx, start_block, leaves_end_block, end_block, root FROM %Q.'%q_segdir' WHERE level = ? AND idx = ?
-UPDATE %Q.'%q_segdir' SET start_block = ?, root = ?WHERE level = ? AND idx = ?
-SELECT 1 FROM %Q.'%q_segments' WHERE blockid=? AND block IS NULL
-SELECT idx FROM %Q.'%q_segdir' WHERE level=? ORDER BY 1 ASC
-SELECT max( level %% 1024 ) FROM %Q.'%q_segdir'
-SELECT level, idx, end_block FROM %Q.'%q_segdir' WHERE level BETWEEN ? AND ? ORDER BY level DESC, idx ASC
-UPDATE OR FAIL %Q.'%q_segdir' SET level=-1,idx=? WHERE level=? AND idx=?
-UPDATE OR FAIL %Q.'%q_segdir' SET level=? WHERE level=-1
-optimize
-matchinfo
-compress
-uncompress
-languageid
-notindexed
-segments
-INSERT OR REPLACE INTO '%q'.'%q_node' VALUES(?1, ?2)
-DELETE FROM '%q'.'%q_node' WHERE nodeno = ?1
-SELECT nodeno FROM '%q'.'%q_rowid' WHERE rowid = ?1
-INSERT OR REPLACE INTO '%q'.'%q_rowid' VALUES(?1, ?2)
-DELETE FROM '%q'.'%q_rowid' WHERE rowid = ?1
-SELECT parentnode FROM '%q'.'%q_parent' WHERE nodeno = ?1
-INSERT OR REPLACE INTO '%q'.'%q_parent' VALUES(?1, ?2)
-DELETE FROM '%q'.'%q_parent' WHERE nodeno = ?1
-,%.*s REAL
-,%.*s INT
-json_array
-json_array_length
-json_extract
-json_insert
-json_object
-json_patch
-json_quote
-json_remove
-json_replace
-json_set
-json_type
-json_valid
-json_group_array
-json_group_object
-datetime
-strftime
-current_time
-current_timestamp
-current_date
-sqlite_rename_column
-sqlite_rename_table
-sqlite_rename_test
-sqlite_drop_column
-sqlite_rename_quotefix
-implies_nonnull_row
-expr_compare
-expr_implies_expr
-affinity
-load_extension
-sqlite_compileoption_used
-sqlite_compileoption_get
-unlikely
-likelihood
-randomblob
-sqlite_version
-sqlite_source_id
-sqlite_log
-last_insert_rowid
-total_changes
-zeroblob
-substring
-group_concat
-NOT NULL
-FOREIGN KEY
+rusqlite::bypass_sqlite_initialization() prior to your first connection attempt.
+Hash table capacity overflow
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/hashbrown-0.14.0/src/raw/mod.rs:	@		
+=	M			E	/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/cache.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rusqlite-0.28.0/src/lib.rsalready mutably borrowed
+called `Result::unwrap()` on an `Err` value/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/alloc/src/sync.rs
+Error code : Unknown error codeAutomatic indexing used - database might benefit from additional indexesHot journal was rolled backA WAL mode database file was recoveredSQLITE_CONSTRAINT_DATATYPESQLITE_CONSTRAINT_PINNEDA non-unique rowid occurredAn application-defined virtual table error occurredA UNIQUE constraint failedA RAISE function within a trigger firedA PRIMARY KEY constraint failedA NOT NULL constraint failedError returned from extension functionForeign key constraint failedCommit hook caused rollbackA CHECK constraint failedTransaction was rolled backSQLITE_READONLY_DIRECTORYSQLITE_READONLY_CANTINITDatabase cannot be modified because database file has movedDatabase has hot journal that must be rolled back (requires write access)Shared-memory file associated with WAL mode database is read-onlyWAL mode database file needs recovery (requires write access)SQLITE_CORRUPT_INDEXSQLITE_CORRUPT_SEQUENCEContent in the virtual table is corruptSQLITE_CANTOPEN_SYMLINKcygwin_conv_path() system call failedUnable to convert filename into full pathnameAttempted to open directory as fileSQLITE_CANTOPEN_NOTEMPDIRSQLITE_BUSY_TIMEOUTCannot promote read transaction to write transaction because of writes by another connectionAnother process is recovering a WAL mode database fileSQLITE_LOCKED_VTABLocking conflict due to another connection with a shared cacheSQLITE_IOERR_DATASQLITE_IOERR_ROLLBACK_ATOMICSQLITE_IOERR_COMMIT_ATOMICSQLITE_IOERR_BEGIN_ATOMICSQLITE_IOERR_AUTHSQLITE_IOERR_VNODEVFS is unable to determine a suitable directory for temporary filesI/O error while trying to map or unmap part of the database file into process address spaceFile being deleted does not existI/O error within the xRead or xWrite (trying to seek within a file)I/O error within the xShmMap method (trying to map a shared-memory segment into process address space)SQLITE_IOERR_SHMLOCKI/O error within the xShmMap method (trying to resize an existing shared-memory segment)I/O error within the xShmMap method (trying to open a new shared-memory segment)SQLITE_IOERR_DIR_CLOSEI/O error within the xClose methodI/O error in the advisory file locking layerI/O error within then xCheckReservedLock methodI/O error within xAccess of a VFS objectOut of memory in I/O layerSQLITE_IOERR_BLOCKEDI/O error within xDelete of a VFS objectI/O error within xLock of a VFS object (trying to obtain a read lock)I/O error within xUnlock of a VFS objectError invoking fstat to get file metadataError attempting to truncate fileError calling fsync on a directoryError flushing data to persistent storage (fsync)Error writing to diskUnable to obtain number of requested bytes (file truncated?)Error reading from diskSQLITE_ERROR_SNAPSHOTSQLITE_ERROR_RETRYSQLITE_ERROR_MISSING_COLLSEQsqlite3_step() has finished executingsqlite3_step() has another row readyWarnings from sqlite3_log()Notifications from sqlite3_log()File opened that is not a database file2nd parameter to sqlite3_bind out of rangeAuxiliary database format errorAuthorization deniedUses OS features not supported on hostLibrary used incorrectlyData type mismatchAbort due to constraint violationString or BLOB exceeds size limitThe database schema changedDatabase is emptyDatabase lock protocol errorUnable to open the database fileInsertion failed because database is fullUnknown opcode in sqlite3_file_control()The database disk image is malformedSome kind of disk I/O error occurredOperation terminated by sqlite3_interrupt()Attempt to write a readonly databaseA malloc() failedA table in the database is lockedThe database file is lockedCallback routine requested an abortAccess permission deniedInternal logic error in SQLiteSQL error or missing databaseSuccessful resultUnknownNotADatabaseParameterOutOfRangeAuthorizationForStatementDeniedNoLargeFileSupportApiMisuseTypeMismatchConstraintViolationTooBigSchemaChangedFileLockingProtocolFailedCannotOpenDatabaseCorruptSystemIoFailureOperationInterruptedOutOfMemoryDatabaseLockedDatabaseBusyInternalMalfunctionErrorextended_code
+SQLITE_AUTH_USEROperationAbortedDiskFullReadOnlyV&^
+= "$&(*,.02468:<
+	+	2	F	Q	a	p	
+LLLSLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLL
+lllllllllll
+lllllllll
+llllllllll%
+zzzzzzzzzzzzzzzzzzzzzzzzzzzz%z%zzzzzzz
+9;;;;;;;;;;;;;;(;;;;;;;;;;
+;;0;;;9;;9
+============================
+============================================
+==========================================================
+vvvvvvvvvv?vvvvvvvTvvvvvivvvvvv
+Q'0QQQ5<F
+/6@@@@@@@@V@b@z@@
+4JM<?Q[?afks<
++;Ix3.39.2
+ !"#$%&'()*+,-./0123456789:;<=>?@abcdefghijklmnopqrstuvwxyz[\]^_`abcdefghijklmnopqrstuvwxyz{|}~
+******""""""""""""""""""""
+@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
+REINDEXEDESCAPEACHECKEYBEFOREIGNOREGEXPLAINSTEADDATABASELECTABLEFTHENDEFERRABLELSEXCLUDELETEMPORARYISNULLSAVEPOINTERSECTIESNOTNULLIKEXCEPTRANSACTIONATURALTERAISEXCLUSIVEXISTSCONSTRAINTOFFSETRIGGERANGENERATEDETACHAVINGLOBEGINNEREFERENCESUNIQUERYWITHOUTERELEASEATTACHBETWEENOTHINGROUPSCASCADEFAULTCASECOLLATECREATECURRENT_DATEIMMEDIATEJOINSERTMATCHPLANALYZEPRAGMATERIALIZEDEFERREDISTINCTUPDATEVALUESVIRTUALWAYSWHENWHERECURSIVEABORTAFTERENAMEANDROPARTITIONAUTOINCREMENTCASTCOLUMNCOMMITCONFLICTCROSSCURRENT_TIMESTAMPRECEDINGFAILASTFILTEREPLACEFIRSTFOLLOWINGFROMFULLIMITIFORDERESTRICTOTHERSOVERETURNINGRIGHTROLLBACKROWSUNBOUNDEDUNIONUSINGVACUUMVIEWINDOWBYINITIALLYPRIMARY
+SQLite format 3
+  !!""##$$%%&&''(())**++,,--..//00112233445566778899
+%vddUX*T
+&&&&&&&&&&
+row_number
+dense_rank
+percent_rank
+cume_dist
+nth_value
+first_value
+naturaleftouterightfullinnercross
+0123456789ABCDEFlast_value
+,,,,,,3M+
+55<@D5W\5]
+PPPPPP_PPiPnnPnnPPPPP[PPPedPPZgPPhPQ
+	:	;	<	=	>	A	I	M	N	P	Q	X	b	d	f	p	q	r	y	
+   ( ) * / 0 9 : ; ? A D E F G R S T U _ ` j p q t z } ~ 
+!$!%!&!'!(!)!*!.!/!0!4!5!9!:!<!>!@!E!G!J!K!L!N!O!P!`!
+# #"#)#*#+#|#}#
+'h'i'j'k'l'm'n'o'p'q'r's't'u'v'
++0+E+G+P+
+,0,`,c,e,g,n,q,r,t,u,w,|,~,
+-'---0-o-p-
+. .!.".#.$.%.&.'.(.).*./.0.:.
+0 0!0*0.000106080;0<0=0>0A0
+2 2*2H2P2Q2`2
+aceinouyyacdeeghijklnorstuuwyzouaiou
+aeiorusthae
+vwwxyzhtwya
+yCREATE TABLE x( name       TEXT, path       TEXT, pageno     INTEGER, pagetype   TEXT, ncell      INTEGER, payload    INTEGER, unused     INTEGER, mx_payload INTEGER, pgoffset   INTEGER, pgsize     INTEGER, schema     TEXT HIDDEN, aggregate  BOOLEAN HIDDEN)
+ !"#$%&'()*+,-./0123456789:;<=>?@ABCDEFGHIJKLMNOPQRSTUVWXYZ[\]^_`abcdefghijklmnopqrstuvwxyz{|}~
+?,?,?,?,?,?,?,?,
+Failed to `Enter::block_on`already borrowed/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/scheduler/current_thread.rscore missinga spawned task panicked and the runtime is configured to shut down on unhandled panic
+cannot access a Thread Local Storage value during or after destruction/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/std/src/thread/local.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/task/list.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/scheduler/current_thread.rs
+attempt to calculate the remainder with a divisor of zero
+called `Option::unwrap()` on a `None` value/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-0.19.5/src/transaction.rs
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/row.rsu32core::option::Option<u32>alloc::string::Stringi8/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/message/frontend.rs
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/prepare.rs
+`async fn` resumed after panicking
+`async fn` resumed after completion
+string contains embedded null
+a Display implementation returned an error unexpectedly/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/alloc/src/string.rscalled `Result::unwrap()` on an `Err` valuevalue too large to transmitassertion failed: 4 <= buf.len()/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/byteorder-1.4.3/src/lib.rscannot advance past `remaining`: /Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/bytes-1.4.0/src/bytes.rs
+!#%')+-/13579;=?ACEGIKMOQSUWY[]_/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/message/frontend.rsstring contains embedded null
+/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/std/src/io/mod.rsfailed to write whole bufferformatter errorfatal runtime error: thread local panicked on drop
+value too large to transmitassertion failed: 2 <= buf.len()/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/byteorder-1.4.3/src/lib.rsassertion failed: 4 <= buf.len()
+fatal runtime error: thread result panicked on drop
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-0.19.5/src/connection.rscannot access a Thread Local Storage value during or after destruction/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/std/src/thread/local.rsalready borrowed/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/context.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/lib.rsvalue too large to transmitassertion failed: 4 <= buf.len()/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/byteorder-1.4.3/src/lib.rs)
+invalid message length: parameters is not drained
+`async fn` resumed after panicking
+`async fn` resumed after completion
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/transaction.rs
+ROLLBACK TO /Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/simple_query.rs
+tokio_postgres::simple_queryexecuting statement batch: 
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/query.rstokio_postgres::queryexecuting statement  with parameters: /Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/client.rsBEGIN
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/prepare.rsSELECT t.typname, t.typtype, t.typelem, r.rngsubtype, t.typbasetype, n.nspname, t.typrelid
+FROM pg_catalog.pg_type t
+LEFT OUTER JOIN pg_catalog.pg_range r ON r.rngtypid = t.oid
+INNER JOIN pg_catalog.pg_namespace n ON t.typnamespace = n.oid
+WHERE t.oid = $1
+SELECT t.typname, t.typtype, t.typelem, NULL::OID, t.typbasetype, n.nspname, t.typrelid
+FROM pg_catalog.pg_type t
+INNER JOIN pg_catalog.pg_namespace n ON t.typnamespace = n.oid
+WHERE t.oid = $1
+SELECT enumlabel
+FROM pg_catalog.pg_enum
+WHERE enumtypid = $1
+ORDER BY enumsortorder
+SELECT enumlabel
+FROM pg_catalog.pg_enum
+WHERE enumtypid = $1
+ORDER BY oid
+SELECT attname, atttypid
+FROM pg_catalog.pg_attribute
+WHERE attrelid = $1
+AND NOT attisdropped
+AND attnum > 0
+ORDER BY attnum
+sassertion failed: (*tail).value.is_none()/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/futures-channel-0.3.28/src/mpsc/queue.rsassertion failed: (*next).value.is_some()/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/message/backend.rsunexpected EOFfailed to fill whole buffer
+invalid message length: field is not drained
+RELEASE /Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/futures-channel-0.3.28/src/mpsc/mod.rscalled `Result::unwrap()` on an `Err` valuecalled `Option::unwrap()` on a `None` valuedescription() is deprecated; use Display
+PoisonError
+: /Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-0.19.5/src/config.rs
+postgres::config
+/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/core/src/str/mod.rsdescription() is deprecated; use Display/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/core/src/str/pattern.rs
+connect_timeoutkeepaliveskeepalives_idlekeepalives_intervalkeepalives_retriestarget_session_attrs
+channel_binding
+`invalid value for option `/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/config.rsunexpected character at byte : expected `` but got `unexpected EOFunterminated quoted connection parameter valuecalled `Option::unwrap()` on a `None` valueunterminated parameter
+UnknownOptionInvalidValue
+tcp_user_timeoutunknown option `host@
+S/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/phf_shared-0.11.1/src/lib.rs
+attempt to calculate the remainder with a divisor of zero/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/message/frontend.rsstring contains embedded null
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/phf-0.11.1/src/map.rs()value too large to transmitassertion failed: 2 <= buf.len()/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/byteorder-1.4.3/src/lib.rsassertion failed: 4 <= buf.len()/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/core/src/str/pattern.rscalled `Option::unwrap()` on a `None` value/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/query.rs
+invalid message length: parameters is not drained/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/lib.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/message/backend.rsunexpected EOFfailed to fill whole buffer
+value too large to transmit/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/byteorder-1.4.3/src/lib.rsassertion failed: 4 <= buf.len()invalid message length: field is not drained/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/client.rs
+`async fn` resumed after panicking
+`async fn` resumed after completion/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/prepare.rsspreparing query  with types : tokio_postgres::prepareSELECT t.typname, t.typtype, t.typelem, r.rngsubtype, t.typbasetype, n.nspname, t.typrelid
+FROM pg_catalog.pg_type t
+LEFT OUTER JOIN pg_catalog.pg_range r ON r.rngtypid = t.oid
+INNER JOIN pg_catalog.pg_namespace n ON t.typnamespace = n.oid
+WHERE t.oid = $1
+SELECT t.typname, t.typtype, t.typelem, NULL::OID, t.typbasetype, n.nspname, t.typrelid
+FROM pg_catalog.pg_type t
+INNER JOIN pg_catalog.pg_namespace n ON t.typnamespace = n.oid
+WHERE t.oid = $1
+SELECT enumlabel
+FROM pg_catalog.pg_enum
+WHERE enumtypid = $1
+ORDER BY enumsortorder
+SELECT enumlabel
+FROM pg_catalog.pg_enum
+WHERE enumtypid = $1
+ORDER BY oid
+SELECT attname, atttypid
+FROM pg_catalog.pg_attribute
+WHERE attrelid = $1
+AND NOT attisdropped
+AND attnum > 0
+ORDER BY attnum
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/query.rstokio_postgres::queryexecuting statement  with parameters: assertion failed: (*tail).value.is_none()/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/futures-channel-0.3.28/src/mpsc/queue.rsassertion failed: (*next).value.is_some()
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/message/backend.rsunexpected EOFinvalid message length: header length < 4invalid message length: parsing u32unknown message tag ``unknown authentication tag `invalid message length: expected buffer to be empty
+range start must not be greater than end: /Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/bytes-1.4.0/src/bytes.rsrange end out of bounds: cannot advance past `remaining`: 
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/codec.rscalled `Option::unwrap()` on a `None` value
+ROLLBACK TO 
+PoisonError
+!,<?DILQV[`c/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/message/backend.rsinvalid message length: error fields is not drainedunexpected EOFfailed to fill whole buffer
+description() is deprecated; use Display
+`P` field did not contain an integer`p` field did not contain an integer`L` field did not contain an integer`V` field contained an invalid value`S` field missing`C` field missing`M` field missing`q` field missing but `p` field present: 
+DETAIL: 
+HINT: Errorcausetimeout waiting for servererror connecting to serverquery returned an unexpected number of rowsinvalid configurationinvalid connection stringauthentication errorerror encoding message to servererror parsing response from serverconnection closedexpected  parameters but got `error deserializing column error serializing parameter error performing TLS handshakeunexpected message from servererror communicating with the serverLogDebugNoticeWarningFatalPanicparsed_severitymessagedetailwhere_schematablecolumnconstraintroutineDbErrorqueryTimeoutConnectConfigConfigParseAuthenticationEncodeParseDbClosedParametersColumnFromSqlToSqlTlsUnexpectedMessageIo
+db errorseveritydatatypeOriginalRowCountinvalid column `/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/futures-channel-0.3.28/src/mpsc/mod.rsbuffer space exhausted; sending this messages would overflow the staterequested buffer size too largecalled `Result::unwrap()` on an `Err` valuecalled `Option::unwrap()` on a `None` value
+XX002XX001XX000P0004P0003P0002P0001P0000HV00NHV00MHV00LHV00RHV00QHV00KHV00JHV00PHV001HV014HV009HV00AHV090HV00DHV00CHV00BHV091HV006HV004HV008HV007HV024HV021HV010HV002HV005HV000F0001F00007200058P0258P01580305800057P0557P0457P0357P0257P01570145700055P0455P0355P0255006550005402354011540015400053400533005320053100530004400042P1742P1642P1542P1442P1342P1242P114261142P1042P0942P084272542702427104271242P0742P0642P054272342P0442P03427014270442P0242P014288342703428C94280942P2242P2142P18428044293942622426024283042P1942P20428034284642501426014200040P01400034000140002400003F0003D0003B0013B00039P0339P0239P013900439001390003800438003380023800138000340002F0042F0032F0022F0052F0002D0002BP012B00028P0128000270002600025P0325P0225P012500725006250052500425003250082500225001250002400023P012351423505235032350223001230002203G2203F2203E2203D2203C2203B2203A220392203822037220362203522034220332203222031220302200T2200S2200N2200M2200L22P0522P0422P0322P0222P012200F22024220272201122001220262200H2200322002220042200G2200C220092202G2202H2201X2201W2201B22013220232201022P06220252200D2201922007220182201G2201F22016220142201E22015220222200B220052201222008220212202E2200021000200000Z0020Z0000P0000LP010L0000F0010F0000B0000A0000900008P0108007080040800108006080030800003000020010200001P0101004010060100701003010080100C0100000000OtherEXX002EXX001EXX000EP0004EP0003EP0002EP0001EP0000EHV00NEHV00MEHV00LEHV00REHV00QEHV00KEHV00JEHV00PEHV001EHV014EHV009EHV00AEHV090EHV00DEHV00CEHV00BEHV091EHV006EHV004EHV008EHV007EHV024EHV021EHV010EHV002EHV005EHV000EF0001EF0000E72000E58P02E58P01E58030E58000E57P05E57P04E57P03E57P02E57P01E57014E57000E55P04E55P03E55P02E55006E55000E54023E54011E54001E54000E53400E53300E53200E53100E53000E44000E42P17E42P16E42P15E42P14E42P13E42P12E42P11E42611E42P10E42P09E42P08E42725E42702E42710E42712E42P07E42P06E42P05E42723E42P04E42P03E42701E42704E42P02E42P01E42883E42703E428C9E42809E42P22E42P21E42P18E42804E42939E42622E42602E42830E42P19E42P20E42803E42846E42501E42601E42000E40P01E40003E40001E40002E40000E3F000E3D000E3B001E3B000E39P03E39P02E39P01E39004E39001E39000E38004E38003E38002E38001E38000E34000E2F004E2F003E2F002E2F005E2F000E2D000E2BP01E2B000E28P01E28000E27000E26000E25P03E25P02E25P01E25007E25006E25005E25004E25003E25008E25002E25001E25000E24000E23P01E23514E23505E23503E23502E23001E23000E2203GE2203FE2203EE2203DE2203CE2203BE2203AE22039E22038E22037E22036E22035E22034E22033E22032E22031E22030E2200TE2200SE2200NE2200ME2200LE22P05E22P04E22P03E22P02E22P01E2200FE22024E22027E22011E22001E22026E2200HE22003E22002E22004E2200GE2200CE22009E2202GE2202HE2201XE2201WE2201BE22013E22023E22010E22P06E22025E2200DE22019E22007E22018E2201GE2201FE22016E22014E2201EE22015E22022E2200BE22005E22012E22008E22021E2202EE22000E21000E20000E0Z002E0Z000E0P000E0LP01E0L000E0F001E0F000E0B000E0A000E09000E08P01E08007E08004E08001E08006E08003E08000E03000E02001E02000E01P01E01004E01006E01007E01003E01008E0100CE01000E00000
+SqlState
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/message/backend.rsunexpected EOF/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/message/frontend.rsfailed to fill whole buffer
+called `Result::unwrap()` on an `Err` valuevalue too large to transmit/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/byteorder-1.4.3/src/lib.rsassertion failed: 4 <= buf.len()cannot advance past `remaining`: /Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/bytes-1.4.0/src/bytes.rs
+invalid message length: field is not drained/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/copy_in.rs
+called `Result::unwrap()` on an `Err` valueArc counter overflow/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/alloc/src/sync.rs
+unexpected EOFinvalid message length: datarowrange is not emptyfailed to fill whole buffera Display implementation returned an error unexpectedly/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/alloc/src/string.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/row.rsi8u32alloc::string::Stringcore::option::Option<u32>
+failed to fill whole bufferdescription() is deprecated; use Display/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/message/backend.rs
+server did not use channel binding/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/prepare.rs
+`async fn` resumed after panicking
+`async fn` resumed after completionno TLS implementation configured
+NoTlsError
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/message/frontend.rsstring contains embedded null
+called `Result::unwrap()` on an `Err` valuevalue too large to transmit/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/byteorder-1.4.3/src/lib.rsassertion failed: 2 <= buf.len()assertion failed: 4 <= buf.len()cannot advance past `remaining`: /Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/bytes-1.4.0/src/bytes.rs
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/client.rs
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/statement.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/transaction.rs
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/percent-encoding-2.3.0/src/lib.rs
+tried to create a `Socket` with an invalid fd/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/socket2-0.5.3/src/socket.rs
+event /Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-util-0.7.8/src/codec/framed_impl.rs:302tokio_util::codec::framed_implmessage/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-util-0.7.8/src/codec/framed_impl.rsevent /Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-util-0.7.8/src/codec/framed_impl.rs:285remainingevent /Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-util-0.7.8/src/codec/framed_impl.rs:280event /Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-util-0.7.8/src/codec/framed_impl.rs:223event /Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-util-0.7.8/src/codec/framed_impl.rs:208event /Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-util-0.7.8/src/codec/framed_impl.rs:204event /Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-util-0.7.8/src/codec/framed_impl.rs:201event /Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-util-0.7.8/src/codec/framed_impl.rs:189event /Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-util-0.7.8/src/codec/framed_impl.rs:167
+!#%')+-/13579;=?ACEGIKMOQSUWY[]_/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/std/src/io/mod.rsfailed to write whole bufferformatter erroralready mutably borrowed/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tracing-core-0.1.31/src/dispatcher.rs
+fatal runtime error: thread local panicked on drop
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tracing-core-0.1.31/src/callsite.rsAttempted to register a `DefaultCallsite` that already exists! This will cause an infinite loop when attempting to read from the callsite cache. This is likely a bug! You should only need to call `DefaultCallsite::register` once per `DefaultCallsite`.
+already mutably borrowed/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tracing-core-0.1.31/src/dispatcher.rs
+!#%')+-/13579;=?ACEGIKMOQSUWY[]_/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/std/src/io/mod.rsfailed to write whole bufferformatter error
+fatal runtime error: thread local panicked on drop
+Lazy instance has previously been poisoned/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/once_cell-1.18.0/src/lib.rs
+Arc counter overflow/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/alloc/src/sync.rs
+rwlock maximum reader count exceeded
+/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/std/src/sys/unix/locks/pthread_rwlock.rsrwlock read lock would result in deadlockunexpected error during rwlock read lock: 
+called `Result::unwrap()` on an `Err` value/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tracing-core-0.1.31/src/callsite.rsPoisonError
+grwlock maximum reader count exceeded
+/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/std/src/sys/unix/locks/pthread_rwlock.rsrwlock read lock would result in deadlockunexpected error during rwlock read lock: rwlock write lock would result in deadlockcalled `Result::unwrap()` on an `Err` value
+PoisonErrorcannot access a Thread Local Storage value during or after destruction/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/std/src/thread/local.rs
+assertion failed: handle.shared.owned.is_empty()/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/scheduler/current_thread.rs
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/io/mod.rsunexpected error when polling the I/O driver: 
+failed to wake I/O driver
+A Tokio 1.x context was found, but it is being shutdown.reactor at max registered I/O resources
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/time/wheel/level.rs
+attempt to divide by zero
+[internal exception] blocking task ran twice./Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/blocking/task.rs
+RNG seed generator is internally corrupt/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/util/rand.rs
+setybdetmodnarod
+Index out of bounds
+attempted to use a condition variable with two mutexes/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/std/src/sys/unix/locks/pthread_condvar.rs
+/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/core/src/slice/sort.rscalled `Option::unwrap()` on a `None` valueassertion failed: end >= start && end <= lenassertion failed: offset != 0 && offset <= len
+early eof
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/net/addr.rs
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/time/mod.rsassertion failed: !handle.is_shutdown()
+task panickedtask was cancelled
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/time/sleep.rstimer error: 
+assertion failed: value <= self.max_value()/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/util/bit.rs
+Interval
+arenegylmodnaroduespemossetybdet
+called `Option::unwrap()` on a `None` value/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/std/src/thread/mod.rsthread name may not contain interior null bytes
+fatal runtime error: thread result panicked on drop
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/blocking/shutdown.rsCannot drop a runtime in a context where blocking is not allowed. This happens when a runtime is dropped from within an asynchronous context.
+called after complete/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/sync/oneshot.rs
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/util/slab.rs
+page is unallocatedunexpected pointerassertion failed: idx < self.slots.len()
+internal error: entered unreachable codefatal runtime error: thread local panicked on drop
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/blocking/schedule.rs
+timer duration exceeds maximum durationtimer is at capacity and cannot create a new entrythe timer is shutdown, must be called from the context of Tokio runtime/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/net/unix/stream.rsA Tokio 1.x context was found, but IO is disabled. Call `enable_io` on the runtime builder to enable IO.A Tokio 1.x context was found, but timers are disabled. Call `enable_time` on the runtime builder to enable timers.
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/util/wake_list.rsassertion failed: self.curr <= NUM_WAKERS/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/time/wheel/mod.rs; when=
+elapsed=
+%v>assertion failed: snapshot.is_complete()/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/task/harness.rsassertion failed: snapshot.is_join_interested()assertion failed: !snapshot.is_join_waker_set()
+!#%')+-/13579;=?ACEGIKMOQSUWY[]_
+"$&(*,.02468:<>@BDFHJLNPRTVXZ\^`bdfhjln/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/std/src/io/mod.rsfailed to write whole bufferformatter error
+Oh no! We never placed the Core back, this is a bug!/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/scheduler/current_thread.rs
+called `Option::unwrap()` on a `None` valuedriver missingalready borrowedcore missing
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/time/mod.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/util/linked_list.rsassertion failed: self.tail.is_none()
+ "$&(*,.02468:<>@BDFHJLNPRTVXZ\^`b
+called `Result::unwrap()` on an `Err` valueassertion failed: next.is_notified()/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/task/state.rsassertion failed: curr.is_running()assertion failed: prev.is_running()assertion failed: !prev.is_complete()current: , sub: assertion failed: snapshot.ref_count() > 0assertion failed: curr.is_join_interested()assertion failed: !curr.is_join_waker_set()assertion failed: curr.is_join_waker_set()assertion failed: prev.ref_count() >= 1assertion failed: prev.ref_count() >= 2assertion failed: self.0 <= isize::MAX as usizeassertion failed: self.ref_count() > 0
+OS can't spawn worker thread: assertion failed: shared.shutdown_tx.is_some()/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/blocking/pool.rsnum_idle_threads underflowed on thread exit/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/io/registration.rsA Tokio 1.x context was found, but it is being shutdown.
+internal error: entered unreachable code: unexpected stage/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/task/core.rsJoinHandle polled after completioncalled `Option::unwrap()` on a `None` valuewaker missingtokio-runtime-worker
+The Tokio context thread-local variable has been destroyed./Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/handle.rs
+there is no reactor running, must be called from the context of a Tokio 1.x runtime
+ $&(*,.02468:<>@BDFHJLNPRTVXZ\^`bdfhjlnp
+ $&(*,.02468:<>@BDFHJLNPRTVXZ\^`bdfhjlnp
+ $&(*,.02468:<>@BDFHJLNPRTVXZ\^`bdfhjlnp
+ $&(*,.02468:<>@BDFHJLNPRTVXZ\^`bdfhjlnp
+ $&(*,.02468:<>@BDFHJLNPRTVXZ\^`bdfhjlnp
+ $&(*,.02468:<>@BDFHJLNPRTVXZ\^`bdfhjlnp
+filled overflowfilled must not become larger than initializedcalled `Option::unwrap()` on a `None` value/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/io/poll_evented.rs
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/io/read_buf.rs
+mark_pending called when the timer entry is in an invalid state/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/time/entry.rs
+Timer already firedA Tokio 1.x context was found, but it is being shutdown.
+/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/std/src/os/fd/owned.rs
+called `Result::unwrap()` on an `Err` value
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/net/tcp/stream.rsassertion failed: fd != u32::MAX as RawFd
+cannot access a Thread Local Storage value during or after destruction/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/std/src/thread/local.rsinconsistent park state; actual = /Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/park.rsinconsistent park_timeout state; actual = inconsistent park_timeout state: inconsistent state in unparkalready mutably borrowed/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/context.rsCannot start a runtime from within a runtime. This happens because a function (like `block_on`) attempted to block the current thread while the thread is being used to drive asynchronous tasks.already borrowed
+assertion failed: c.runtime.get().is_entered()
+called `Option::unwrap()` on a `None` value
+internal error: entered unreachable code/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/sync/notify.rsassertion failed: actual_state == EMPTY || actual_state == NOTIFIED/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/std/src/os/fd/owned.rs/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/std/src/os/fd/owned.rspath must be shorter than libc::sockaddr_un.sun_pathpath must be no longer than libc::sockaddr_un.sun_path
+_int8multirange_datemultirange_tstzmultirange_tsmultirange_nummultirange_int4multirangeanycompatiblerangeanycompatiblenonarrayanycompatiblearrayanycompatible_pg_snapshotpg_snapshotpg_mcv_listpg_brin_minmax_multi_summarypg_brin_bloom_summaryanycompatiblemultirangeanymultirangeint8multirangedatemultirangetstzmultirangetsmultirangenummultirangeint4multirange_regcollationregcollationregrole_regnamespaceregnamespace_jsonpath_int8rangeint8range_daterangedaterange_tstzrangetstzrangetsrange_numrange_int4rangeint4rangeevent_trigger_jsonbjsonb_regdictionaryregdictionary_regconfigregconfig_gtsvector_tsvectorgtsvectortsqueryanyenumpg_dependenciespg_ndistincttsm_handler_pg_lsnpg_lsnfdw_handlertxid_snapshot_uuid_txid_snapshotanynonarray_recordanyelementtriggeranycstringrecord_regclass_regoperator_regprocedureregtyperegoperatorregoperregprocedure_refcursorrefcursornumeric_varbitvarbitbit_timetztimetz_interval_timestamptztimestamptz_time_date_timestamptimestampvarcharbpchar_inetaclitem_float8_float4_path_lseg_point_int8_bpchar_oidvector_text_int4_int2vector_int2_name_char_bytea_boolmacaddr_moneymoney_macaddr8_circlecircleunknownfloat8float4_cidr_linepolygonboxpoint_xid8_jsonpg_node_treexmlpg_ddl_commandoidvectorcidxidtidoidregprocint2vectornamebyteaOtherkindschemaInt8multiRangeArrayDatemultiRangeArrayTstzmultiRangeArrayTsmultiRangeArrayNummultiRangeArrayInt4multiRangeArrayAnycompatibleRangeAnycompatiblenonarrayAnycompatiblearrayAnycompatiblePgSnapshotArrayPgSnapshotPgMcvListPgBrinMinmaxMultiSummaryPgBrinBloomSummaryAnycompatiblemultiRangeAnymultiRangeInt8multiRangeDatemultiRangeTstzmultiRangeTsmultiRangeNummultiRangeInt4multiRangeRegcollationArrayRegcollationRegroleArrayRegroleRegnamespaceArrayRegnamespaceJsonpathArrayInt8RangeArrayInt8RangeDateRangeArrayDateRangeTstzRangeArrayTstzRangeTsRangeArrayTsRangeNumRangeArrayInt4RangeArrayInt4RangeEventTriggerJsonbArrayJsonbRegdictionaryArrayRegdictionaryRegconfigArrayRegconfigTsqueryArrayGtsVectorArrayTsVectorArrayGtsVectorTsqueryAnyenumPgDependenciesPgNdistinctTsmHandlerPgLsnArrayPgLsnFdwHandlerTxidSnapshotUuidArrayTxidSnapshotArrayAnynonarrayRecordArrayAnyelementLanguageHandlerTriggerAnyCstringRecordRegtypeArrayRegclassArrayRegoperArrayRegprocedureArrayRegtypeRegoperatorRegoperRegprocedureRefcursorArrayRefcursorNumericVarbitArrayVarbitBitTimetzArrayTimetzCstringArrayNumericArrayIntervalArrayTimestamptzTimeArrayDateArrayTimestampArrayTimestampVarcharBpcharInetArrayMacaddrArrayAclitemArrayAclitemPolygonArrayFloat8ArrayFloat4ArrayPathArrayLsegArrayPointArrayInt8ArrayVarcharArrayBpcharArrayOidVectorArrayTextArrayRegprocArrayInt4ArrayInt2VectorArrayInt2ArrayNameArrayCharArrayByteaArrayBoolArrayMacaddrMoneyArrayMoneyMacaddr8ArrayCircleArrayCircleUnknownFloat8Float4CidrArrayLineArrayPolygonBoxPointIndexAmHandlerXid8ArrayTableAmHandlerJsonArrayPgNodeTreeXmlPgDdlCommandOidVectorCidXidTidOidRegprocInt2VectorByteaxid8uuidvoid_bit_oid_box_cid_xid_tidinetcidrlseg_xmljsonint4int2int8Xid8UuidVoidTimeDateInetCidrLineLsegJsonInt4Int2Int8
+_regrolejsonpath_tsrangenumrangeanyrange_tsquerytsvectorinternalanyarray_regtype_regoperregclass_cstring_numeric_macaddr_aclitem_polygon_varchar_regprocmacaddr8JsonpathNumRangeAnyRangeTsVectorAnyarrayRegclassBitArrayOidArrayBoxArrayCidArrayXidArrayTidArrayMacaddr8XmlArraylanguage_handlerindex_am_handlertable_am_handlerRegoperatorArrayTimestamptzArray)
+#-7invalid buffer sizeltree version 1 only supportedlquery version 1 only supportedltxtquery version 1 only supportedfailed to fill whole buffer
+description() is deprecated; use Displayalloc::string::String
+pg_catalog.a Postgres value was `NULL`cannot convert between the Rust type `` and the Postgres type ``
+CompositeDomainMultirangeRangeArrayPseudoSimpleFieldtype_WasNullWrongType
+&strEnumrust
+postgres)
+called `Result::unwrap()` on an `Err` value
+[HMAC is able to accept all key sizes/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/authentication/sasl.rsalready checked abovep=tls-server-end-point,,n,,y,,n=,r=invalid SCRAM stateinvalid nonce
+ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/
+?456789:;<=
+ !"#$%&'()*+,-./0123
+Client Keyc=,r=,,p=Server KeySCRAM error: SCRAM verification errorunexpected character at byte : expected `` but got `unexpected EOFunexpected trailing data at byte 
+integer overflow when calculating buffer size/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/base64-0.21.2/src/engine/mod.rsInvalid UTF8/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/base64-0.21.2/src/chunked_encoder.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/base64-0.21.2/src/encode.rsusize overflow when calculating b64 length
+[description() is deprecated; use DisplayIndex out of bounds
+/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/core/src/slice/sort.rscalled `Option::unwrap()` on a `None` valueassertion failed: end >= start && end <= lenassertion failed: offset != 0 && offset <= len
+called `Option::unwrap()` on a `None` value/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/stringprep-0.1.2/src/lib.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tinyvec-1.6.0/src/arrayvec.rs
+)))))))))))))))))))))))))))))))))
+)))))))))))))))))))))))))))))))))))))))))))))))
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tinyvec-1.6.0/src/tinyvec.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/unicode-normalization-0.1.22/src/decompose.rs
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/unicode-normalization-0.1.22/src/lookups.rs
+could not initialize thread_rng: /Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rand-0.8.5/src/rngs/thread.rs
+cannot access a Thread Local Storage value during or after destruction/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/std/src/thread/local.rscalled `Option::unwrap()` on a `None` value/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/std/src/sync/once.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rand-0.8.5/src/rngs/adapter/reseeding.rslibc::pthread_atfork failed with code 
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rand_chacha-0.3.1/src/guts.rsdescription() is deprecated; use Display
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/base64-0.21.2/src/engine/general_purpose/decode.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/base64-0.21.2/src/engine/general_purpose/mod.rsbase64 data was not utf8/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/base64-0.21.2/src/display.rs
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/base64-0.21.2/src/engine/general_purpose/decode_suffix.rsinternal error: entered unreachable code: Impossible: must only have 0 to 8 input bytes in last chunk, with no invalid lengths
+Invalid paddingInvalid last symbol , offset .Encoded text cannot have a 6-bit remainder.Invalid byte 
+InvalidPaddingInvalidLastSymbolInvalidLengthInvalidByte
+internal error: entered unreachable code: Impossible remainder/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/base64-0.21.2/src/encode.rsDon't use a tiny buffer/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/base64-0.21.2/src/chunked_encoder.rsInvalidLength
+called `Option::unwrap()` on a `None` value/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/futures-core-0.3.28/src/task/__internal/atomic_waker.rs
+overflow/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/bytes-1.4.0/src/bytes_mut.rssplit_to out of bounds: set_end out of boundsnew_len = ; capacity = 
+called `Result::unwrap()` on an `Err` value
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/bytes-1.4.0/src/bytes.rs
+split_off out of bounds: split_to out of bounds: 
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/csv-1.2.2/src/byte_record.rs
+called `Option::unwrap()` on a `None` value/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/csv-1.2.2/src/byte_record.rscalled `Option::unwrap()` on a `None` value00010203040506070809101112131415161718192021222324252627282930313233343536373839404142434445464748495051525354555657585960616263646566676869707172737475767778798081828384858687888990919293949596979899
+nGV5}$ e
+G(SN\_T8h
+ =U7el#|67
+internal error: entered unreachable code/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/csv-core-0.1.10/src/lib.rs
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/csv-core-0.1.10/src/reader.rsinternal error: entered unreachable code
+	called `Option::unwrap()` on a `None` value
+(called `Option::unwrap()` on a `None` value/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/pyo3-0.18.3/src/sync.rspyo3_runtime.PanicException
+The exception raised when Rust code called from Python panics.
+Like SystemExit, this exception is derived from BaseException so that
+it will typically propagate all the way through the stack and cause the
+Python interpreter to exit.
+Failed to initialize new exception type./Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/pyo3-0.18.3/src/panic.rs
+Y]Mio_uSsKQmG[Ecq
+wayIC=?;
+exceptions must derive from BaseException
+Unwrapped panic from Python code--- PyO3 is resuming a panic after fetching a PanicException from Python. ---
+Python stack trace below:
+attempted to fetch exception but none was setFailed to initialize nul terminated exception name/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/pyo3-0.18.3/src/err/mod.rsFailed to initialize nul terminated docstringCannot access exception type while normalizingCannot normalize a PyErr while already normalizing it.Exception type missingException value missingPyErrvaluetraceback
+'' object cannot be converted to '<failed to extract type name>Python API call failed
+typefrom
+(attempted to fetch exception but none was set
+(a Display implementation returned an error unexpectedly/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/alloc/src/string.rsattempted to fetch exception but none was set
+PyStringattempted to fetch exception but none was setThe first GILGuard acquired must be the last one dropped./Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/pyo3-0.18.3/src/gil.rscannot access a Thread Local Storage value during or after destruction/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/std/src/thread/local.rsalready mutably borrowedalready borrowed
+surrogatepass
+The Python interpreter is not initialized and the `auto-initialize` feature is not enabled.
+Consider calling `pyo3::prepare_freethreaded_python()` before attempting to use Python APIs.
+uespemosarenegylmodnarodsetybdet
+3).exceptions must derive from BaseExceptionattempted to fetch exception but none was set
+attempted to fetch exception but none was setargument '': ().was takes from  positional arguments but   given takes  got multiple values for argument '' got an unexpected keyword argument ' got some positional-only arguments passed as keyword arguments: arguments missing  required : keywordpositional
+__qualname__were to argument
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/pyo3-0.18.3/src/impl_/panic.rsattempted to fetch exception but none was seta Display implementation returned an error unexpectedly/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/alloc/src/string.rsattempted to fetch exception but none was setFunction name cannot contain NUL byte.Document cannot contain NUL byte.
+panic from Rust code
+PyListattempted to fetch exception but none was set
+PyO3 modules may only be initialized once per interpreter process
+PyModule_GetName expected to return utf8/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/pyo3-0.18.3/src/types/module.rscould not append __name__ to __all__
+__all____name__Path
+attempted to fetch exception but none was set
+ in called `Result::unwrap()` on an `Err` value/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/smallvec-1.10.0/src/lib.rscapacity overflowassertion failed: new_cap >= len
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/parking_lot_core-0.9.8/src/parking_lot.rsOnce instance has previously been poisoned/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/parking_lot-0.12.1/src/once.rs
+fatal runtime error: thread local panicked on drop
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/parking_lot_core-0.9.8/src/parking_lot.rs
+!#%')+-/13579;=?ACEGIKMOQSUWY[]_/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/std/src/io/mod.rsfailed to write whole bufferformatter error
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/parking_lot_core-0.9.8/src/parking_lot.rs
+!#%')+-/13579;=?ACEGIKMOQSUWY[]_/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/std/src/io/mod.rsfailed to write whole bufferformatter error
+fatal runtime error: thread local panicked on drop
+/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/core/src/str/pattern.rsNo checksum found for sentence: nmea_parser/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/nmea-parser-0.10.0/src/lib.rsInvalid checksum found for sentence: Corrupted NMEA sentence: Invalid NMEA sentence: $!Failed to parse fragment count: NMEA sentence fragment count greater () than supported 2NMEA message_id missing from  than supported 2Unexpected NMEA fragment number: /Unsupported  message type: Unsupported sentence type: 
+a Display implementation returned an error unexpectedly/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/alloc/src/string.rs
+called `Result::unwrap()` on an `Err` valueassertion failed: self.is_char_boundary(new_len)
+bit-vector capacity exceeded:  > /Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/bitvec-1.0.1/src/vec.rs
+@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@BBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZX^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^dbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdb,/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/nmea-parser-0.10.0/src/util.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/offset/mod.rsinvalid time/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/date.rs`DateTime - Duration` overflowed/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/datetime/mod.rsFailed to parse field : Failed to parse hex field Invalid time format: Invalid date format: 0Time zone offset out of bounds: :.0Failed to parse Utc Date from y: m: d: h: s:Failed to parse latitude (DDMM.MMM) from 
+Failed to parse longitude (DDDMM.MMM) from 
+Failed to parse float: Bad hemispehre: 
+Invalid GPGSA fix type: Invalid GPGSA mode: 
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/wyz-0.5.1/src/comu.rsbit-vector capacity exceeded:  > /Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/bitvec-1.0.1/src/vec.rsUnrecognized Maneuver Indicator value: nmea_parser::ais::vdm_t1t2t3/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/nmea-parser-0.10.0/src/ais/vdm_t1t2t3.rs
+InvalidSentenceCorruptedSentenceUnsupportedSentenceType
+Hash table capacity overflow
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/hashbrown-0.12.3/src/raw/mod.rs
+range /Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/bitvec-1.0.1/src/slice/api.rs
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/offset/mod.rsinvalid time/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/date.rs
+ out of bounds: text
+`NaiveDateTime + Duration` overflowed/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/naive/datetime/mod.rs
+Ambiguous local time, ranging from  to No such local timecalled `Option::unwrap()` on a `None` value/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/offset/fixed.rsinternal error: entered unreachable code: This should never be reached as all four bit cases are covered (value: )/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/nmea-parser-0.10.0/src/ais/vdm_t23.rs
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/offset/mod.rsinvalid time/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/date.rs
+interval
+*VVVVVVVVV
+VVVVVVVVV3VVVVVVVVV
+VVVVVVVVV9!?-0B
+<E$VVVVVVVVV'VVVVVVVVVHVVVVVVVVV
+e0oGLtQVjy5
+Mismatching AIS types: Mismatching MMSI numbers: Mismatching IMO numbers: Mismatching AIS version indicators: 
+Invalid station identifier/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/nmea-parser-0.10.0/src/ais/mod.rsClass BClass Aunknown
+Unexpected ship and cargo type: nmea_parser::ais
+Unrecognized position fix type: 
+ !"#$%&'((((((((((23456789:;<<<<<<<<<<FFFFFFFFFFPPPPPPPPPPZZZZZZZZZZ
+range /Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/bitvec-1.0.1/src/slice/api.rscalled `Option::unwrap()` on a `None` value../rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/core/src/str/pattern.rs
+Invalid talker identifier
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/nmea-parser-0.10.0/src/gnss/mod.rs
+Unrecognized FAA information value: 
+AIVDM type 24 part number has unexpected value: 
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/offset/mod.rsinvalid time/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/date.rs
+bit-vector capacity exceeded:  > /Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/bitvec-1.0.1/src/vec.rs/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/bitvec-1.0.1/src/vec/api.rsbit-vector capacity exceeded
+Invalid RMC variation side: Invalid RMC navigation receiver status: 
+Unsupported AIVDM message type: 19called `Option::unwrap()` on a `None` value/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/nmea-parser-0.10.0/src/gnss/mwv.rs
+getrandom::getrandom() failed./Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ahash-0.7.6/src/random_state.rs/dev/urandom
+Errorunknown_codeinternal_codedescriptionUnknown Error: OS Error: Node.js ES modules are not directly supported, see https://docs.rs/getrandom#nodejs-es-module-supportCalling Node.js API crypto.randomFillSync failedNode.js crypto CommonJS module is unavailablerandSecure: VxWorks RNG module is not initializedCalling Web API crypto.getRandomValues failedWeb Crypto API is unavailableRDRAND: instruction not supportedRDRAND: failed multiple times: CPU issue likelyRtlGenRandom: Windows system function failureSecRandomCopyBytes: iOS Security framework failureerrno: did not return a positive valuegetrandom: this target is not supported
+os_errorgetentropy
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/once_cell-1.18.0/src/imp_std.rscalled `Option::unwrap()` on a `None` value
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/format/parse.rsassertion failed: min <= max/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/format/scan.rs
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/time-0.1.45/src/duration.rsDuration::seconds out of bounds
+called `Option::unwrap()` on a `None` value/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/naive/time/mod.rs.
+`NaiveDateTime + Duration` overflowed/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/naive/datetime/mod.rs
+    !!!!""""####$$$$%%%%&&&&''''(((())))****++++,,,,----....////00001111111122223333444455556666777788889999::::;;;;<<<<====>>>>????@@@@AAAABBBBCCCCDDDDEEEEFFFFGGGGHHHHIIIIIIIIJJJJKKKKLLLLMMMMNNNNOOOOPPPPQQQQRRRRSSSSTTTTUUUUVVVVWWWWXXXXYYYYZZZZ[[[[\\\\]]]]^^^^____````aaaa/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/naive/internals.rs
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/offset/fixed.rscalled `Option::unwrap()` on a `None` value
+#(-27<AFKPUZ_
+ #(-25:?DILS
+internal error: entered unreachable code/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/format/mod.rsbad or unsupported format stringtrailing inputpremature end of inputinput contains invalid charactersinput is not enough for unique date and timeno possible date and time matching inputinput is out of range
+JanFebMarAprMayJunJulAugSepOctNovDecJanuaryMarchAprilAugustSeptemberOctoberSunMonTueWedThuFriSatSundayMondayTuesdayWednesdayFridayAMPMDo not try to write %#z it is undefined.
+@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@BBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZX^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^dbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdb
+FebruaryNovemberDecemberThursdaySaturday
+JuneJuly
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/naive/internals.rs
+@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
+BBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBB
+HJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJ
+JLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJL
+NPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNP
+PRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPR
+TVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTV
+VXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVX
+XZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZ
+\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^
+^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`
+bdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbd
+@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@BBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZX^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^dbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdb
+%%%%%%%%%%%%%%%%%%%%%%%%%%
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/format/scan.rs
+uaryruarychil
+eyusttemberoberemberdaysdaynesdayrsdayurdaycstmdtmstpdtpst
+internal error: entered unreachable code/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/format/parsed.rs`NaiveDateTime - Duration` overflowed/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/naive/datetime/mod.rs
+@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@BBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZX^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^dbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdb
+/ :/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/format/strftime.rsassertion failed: nextspec > 0%
+/Users/matt/.cargo/registry/src/index.crates.io-6f17d22bba15001f/log-0.4.19/src/lib.rs
+key-value support is experimental and must be enabled using the `kv_unstable` featureInfolayout
+AllocErr
+1gikmoqsuwy{}
+0>L48HN$"V
+ "$&(*,.02468:<>@BDFHJLNP
+ "$&(*,.02468:<>@BDFHJLNP
+#'+/37;?BFJNRVZ^bfjnrvz~
+!#%')+-/13579;=?ACEGIKMOQSUWY[]_ac
+(,.02468:<>@BDFHJLNPRTVXZ\^`bdfhjlnprtvx
+1?M59IO%#W
+!#%')+-/13579;=?ACEGIKMOQSUWY[]_ac
+!#%')+-/13579;=?ACEGIKMOQSUWY[]_aceg
+MMMMMMMM
+@MMBMMMMMMMMMMMMMMMMMMMM>MMMM>
+called `Option::unwrap()` on a `None` value/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/alloc/src/collections/btree/navigate.rs/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/core/src/slice/iter.rsIndex out of bounds
+/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/core/src/str/pattern.rsoverflow in Duration::new/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/core/src/time.rs
+attempt to divide by zeroassertion failed: mid <= self.len()/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/core/src/slice/sort.rsassertion failed: end >= start && end <= lenassertion failed: offset != 0 && offset <= lenassertion failed: offset != 0 && offset <= len && len >= 2called `Result::unwrap()` on an `Err` value
+internal error: entered unreachable code
+/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/alloc/src/vec/mod.rs/Users/runner/.cargo/registry/src/index.crates.io-6f17d22bba15001f/gimli-0.27.2/src/read/line.rs
+attempt to calculate the remainder with a divisor of zero/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/core/src/num/mod.rs/Users/runner/.cargo/registry/src/index.crates.io-6f17d22bba15001f/object-0.30.1/src/read/macho/section.rs/Users/runner/.cargo/registry/src/index.crates.io-6f17d22bba15001f/object-0.30.1/src/read/macho/segment.rsInvalid AIX big archive member headerInvalid AIX big archive member name lengthInvalid AIX big archive member nameInvalid AIX big archive terminatorInvalid archive member size in AIX big archiveInvalid archive member headerInvalid archive terminatorInvalid archive member sizeArchive member size is too large/Users/runner/.cargo/registry/src/index.crates.io-6f17d22bba15001f/object-0.30.1/src/read/archive.rsInvalid archive extended name offsetInvalid archive extended name length
+/Users/runner/.cargo/registry/src/index.crates.io-6f17d22bba15001f/addr2line-0.19.0/src/lib.rs/Users/runner/.cargo/registry/src/index.crates.io-6f17d22bba15001f/addr2line-0.19.0/src/function.rs
+library/std/src/rt.rs
+too many running threads in thread scopelibrary/std/src/thread/scoped.rs
+AccessError
+use of std::thread::current() is not possible after the thread's local data has been destroyedlibrary/std/src/thread/mod.rsfatal runtime error: an irrecoverable error occurred while synchronizing threads
+failed to generate unique thread ID: bitspace exhausted
+RUST_BACKTRACE
+failed to write the buffered datalibrary/std/src/io/buffered/bufwriter.rs
+library/std/src/io/buffered/linewritershim.rs
+uncategorized errorother errorout of memoryunexpected end of fileunsupportedoperation interruptedargument list too longtoo many linkscross-device link or renameexecutable file busyresource busyfile too largefilesystem quota exceededseek on unseekable filewrite zerotimed outinvalid datainvalid input parameterstale network file handlefilesystem loop or indirection limit (e.g. symlink loop)read-only filesystem or storage mediumdirectory not emptyis a directorynot a directoryoperation would blockentity already existsbroken pipenetwork downaddress not availableaddress in usenot connectedconnection abortednetwork unreachableconnection refusedpermission deniedErrormessageOs (os error )
+library/std/src/io/readbuf.rs
+library/std/src/io/stdio.rscannot access a Thread Local Storage value during or after destructionlibrary/std/src/thread/local.rsfailed printing to : stdoutstderr
+library/std/src/io/mod.rsfailed to fill whole bufferadvancing IoSlice beyond its lengthlibrary/std/src/sys/unix/io.rsadvancing io slices beyond their lengthfailed to write whole bufferformatter error
+library/std/src/panic.rslibrary/std/src/path.rs
+library/std/src/sync/once.rs
+lock count overflow in reentrant mutexlibrary/std/src/sync/remutex.rsoverflow when adding duration to instantlibrary/std/src/time.rs
+second time provided was later than selffile name contained an unexpected NUL bytestack backtrace:
+note: Some details are omitted, run with `RUST_BACKTRACE=full` for a verbose backtrace.
+__rust_begin_short_backtrace__rust_end_short_backtrace<unknown>
+RUST_MIN_STACKlibrary/std/src/sys_common/thread_info.rsfatal runtime error: assertion failed: thread_info.is_none()
+memory allocation of  bytes failedlibrary/std/src/alloc.rs bytes failed
+fatal runtime error: Rust panics must be rethrown
+fatal runtime error: Rust cannot catch foreign exceptions
+library/std/src/panicking.rsBox<dyn Any><unnamed>' panicked at '', note: run with `RUST_BACKTRACE=1` environment variable to display a backtrace
+thread panicked while processing panic. aborting.
+panicked after panic::always_abort(), aborting.
+thread caused non-unwinding panic. aborting.
+thread panicked while panicking. aborting.
+fatal runtime error: failed to initiate panic, error 
+library/std/src/../../backtrace/src/symbolize/mod.rs       - :
+Unsupported
+CustomerrorUncategorizedOtherOutOfMemoryUnexpectedEofInterruptedArgumentListTooLongInvalidFilenameTooManyLinksCrossesDevicesExecutableFileBusyResourceBusyFileTooLargeFilesystemQuotaExceededNotSeekableStorageFullWriteZeroInvalidDataInvalidInputStaleNetworkFileHandleFilesystemLoopReadOnlyFilesystemDirectoryNotEmptyIsADirectoryNotADirectoryWouldBlockAlreadyExistsBrokenPipeNetworkDownAddrInUseNotConnectedConnectionAbortedNetworkUnreachableHostUnreachableConnectionResetConnectionRefused
+SystemTimeErrorunexpected error during closedir: library/std/src/sys/unix/fs.rs
+library/std/src/sys/unix/net.rsfailed to lookup address information: 
+strerror_r failurelibrary/std/src/sys/unix/os.rs
+library/std/src/sys/unix/rand.rsunexpected getentropy error: /dev/urandomfailed to open /dev/urandomfailed to read /dev/urandom
+failed to allocate an alternative stack: library/std/src/sys/unix/stack_overflow.rsfailed to set up alternative stack guard page: library/std/src/sys/unix/thread.rsfailed to join thread: 
+assertion failed: tv_nsec >= 0 && tv_nsec < NSEC_PER_SEC as i64library/std/src/sys/unix/time.rs
+library/std/src/sys/unix/locks/pthread_mutex.rs
+rwlock maximum reader count exceededlibrary/std/src/sys/unix/locks/pthread_rwlock.rsrwlock read lock would result in deadlockunexpected error during rwlock read lock: 
+attempted to use a condition variable with two mutexeslibrary/std/src/sys/unix/locks/pthread_condvar.rs
+failed to create dispatch semaphore for thread synchronizationlibrary/std/src/sys/unix/thread_parking/darwin.rsassertion failed: state_and_queue.addr() & STATE_MASK == RUNNINGOnce instance has previously been poisonedlibrary/std/src/sys_common/once/queue.rs
+assertion failed: len as usize >= mem::size_of::<c::sockaddr_in6>()library/std/src/sys_common/net.rsassertion failed: len as usize >= mem::size_of::<c::sockaddr_in>()invalid port valueinvalid socket address
+UdpSocket
+library/std/src/../../backtrace/src/symbolize/gimli.rs
+Contents/Resources/DWARF
+library/std/src/../../backtrace/src/symbolize/gimli/libs_macos.rs
+getentropy
+(#(("(((
+((((((((((((
+((((((($
+invalid filenameno storage spacehost unreachableconnection resetentity not found             at AddrNotAvailablePermissionDeniedinvalid argument
+, line: deadlockthread '
+DisabledInternalDeadlockTimedOutNotFound
+SomeNonenamekindKindcode
+addrpath
+/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/core/src/char/methods.rsto_digit: radix is too high (maximum 36)
+/Users/runner/.cargo/registry/src/index.crates.io-6f17d22bba15001f/object-0.30.1/src/read/archive.rsDataTextNamedate
+ %05>CLQX"
+ $(dh,0l48<|||||@D|||||||||||||||ptH|||||||||||||||L{|||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||x|||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||P
+!%)-158<?CGJMPSW[_cglptx|
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+ $(,048<@DLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLH
+%)-159=AEIMQUY]`dhlptx|
+   !               %               )               -               1                                               5
+='*-				047:			C															G															K															O															S																																															W
+assertion failed: idx < CAPACITY/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/alloc/src/collections/btree/node.rsassertion failed: edge.height == self.height - 1assertion failed: src.len() == dst.len().debug_types.debug_tu_index.debug_str_offsets.debug_str.debug_rnglists.debug_ranges.debug_pubtypes.debug_pubnames.debug_macro.debug_macinfo.debug_loclists.debug_loc.debug_line_str.debug_line.debug_info.eh_frame_hdr.eh_frame.debug_frame.debug_cu_index.debug_aranges.debug_addr.debug_abbrev
+/Users/runner/.cargo/registry/src/index.crates.io-6f17d22bba15001f/gimli-0.27.2/src/read/abbrev.rs
+/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/core/src/ops/function.rs/rustc/dbba594575ce75b1b57ccb1e4223b9909a28b1b8/library/core/src/str/pattern.rscalled `Result::unwrap()` on an `Err` value
+/Users/runner/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustc-demangle-0.1.21/src/legacy.rs
+)C,called `Option::unwrap()` on a `None` value
+/Users/runner/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustc-demangle-0.1.21/src/v0.rs
+`fmt::Error`s should be impossible without a `fmt::Formatter`punycode{-}0internal error: entered unreachable codeinternal error: entered unreachable code: str::from_utf8( was expected to have 1 char, but  chars were found..._!f64f32usizeu64u32u16u8isizei64i32i16i8str{recursion limit reached}?', > ::{closure:#[] + ; const  unsafe " fn( =  {  }false{: 0x.llvm./Users/runner/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rustc-demangle-0.1.21/src/lib.rs`fmt::Error` from `SizeLimitedFmtAdapter` was discarded{size limit reached}
+SizeLimitExhausted
+{invalid syntax}extern ") = u128i128charboolfor< as shimdyn mut  -> 
+Hash table capacity overflow
+/Users/runner/.cargo/registry/src/index.crates.io-6f17d22bba15001f/hashbrown-0.12.3/src/raw/mod.rs
+CapacityOverflow
+called `Result::unwrap()` on an `Err` valuelibrary/alloc/src/raw_vec.rscapacity overflow
+library/alloc/src/ffi/c_str.rscalled `Option::unwrap()` on a `None` value
+nul byte found in provided data at position: 
+a formatting trait implementation returned an errorlibrary/alloc/src/fmt.rs
+library/alloc/src/sync.rs
+errorFromUtf8Error
+NulError
+0123456789abcdefrange end index ) when slicing `
+,,2,,,,,,,,,,,,,,,,,,,,4,,,,6=
+library/core/src/num/dec2flt/decimal.rs
+$ + 3 < F(P([(g0s0
+I)I>QSQiQ
+!$'+.158;
+library/core/src/num/dec2flt/parse.rsinvalid float literalcannot parse float from empty stringassertion failed: edelta >= 0library/core/src/num/diy_float.rs
+library/core/src/num/flt2dec/strategy/dragon.rsassertion failed: d.mant > 0assertion failed: d.minus > 0assertion failed: d.plus > 0assertion failed: d.mant.checked_add(d.plus).is_some()assertion failed: d.mant.checked_sub(d.minus).is_some()assertion failed: buf.len() >= MAX_SIG_DIGITS
+library/core/src/num/flt2dec/strategy/grisu.rsassertion failed: d.mant + d.plus < (1 << 61)
+attempt to divide by zeroassertion failed: !buf.is_empty()called `Option::unwrap()` on a `None` valueassertion failed: d.mant < (1 << 61)
+;library/core/src/num/flt2dec/mod.rsassertion failed: buf[0] > b\'0\'assertion failed: parts.len() >= 40..assertion failed: parts.len() >= 6E-e-Ee-+0infNaN0E00e0
+assertion failed: buf.len() >= maxlen
+out of range integral type conversion attemptednumber would be zero for non-zero typenumber too small to fit in target typenumber too large to fit in target typeinvalid digit found in stringcannot parse integer from empty string
+from_str_radix_int: must lie in the range `[2, 36]` - found library/core/src/num/mod.rs (1 << )library/core/src/fmt/mod.rs
+BorrowErrorBorrowMutError
+to_digit: radix is too high (maximum 36)library/core/src/char/methods.rs
+library/core/src/net/ip_addr.rslibrary/core/src/net/display_buffer.rs::::1internal error: entered unreachable code::ffff:library/core/src/net/parser.rs:library/core/src/net/socket_addr.rs[%]:panicked at '', library/core/src/panicking.rsindex out of bounds: the len is  but the index is 
+panic in a function that cannot unwindmatches!===assertion failed: `(left  right)`
+  left: ``,
+ right: ``: `called `Result::unwrap()` on an `Err` value:  {
+}, .. } { .. } }(
+{]attempted to begin a new map entry without completing the previous onelibrary/core/src/fmt/builders.rsattempted to format a map value before its keyattempted to finish a map with a partial entrylibrary/core/src/fmt/num.rs0x
+00010203040506070809101112131415161718192021222324252627282930313233343536373839404142434445464748495051525354555657585960616263646566676869707172737475767778798081828384858687888990919293949596979899
+0000000000000000000000000000000000000000000000000000000000000000false()
+library/core/src/slice/memchr.rs
+range start index  out of range for slice of length slice index starts at  but ends at 
+attempted to index slice up to maximum usize
+source slice length () does not match destination slice length (
+incomplete utf-8 byte sequence from index invalid utf-8 sequence of  bytes from index invalid utf-8: corrupt contents
+attempted to index str up to maximum usizelibrary/core/src/str/pattern.rs
+library/core/src/str/lossy.rs\x
+[...]byte index  is out of bounds of `begin <= end ( is not a char boundary; it is inside ) of `library/core/src/str/mod.rs
+library/core/src/time.rs
+sns18446744073709551616
+library/core/src/unicode/printable.rs
+)147:;=IJ]
+)14:;EFIJ^de
+):;EIW[\^_de
+FGNOXZ\^~
+)14:EFIJNOde\
+ #%&(38:HJLPSUVXZ\^`cefksx}
+library/core/src/unicode/unicode_data.rs
+library/core/src/num/bignum.rsassertion failed: noborrowassertion failed: digits < 40assertion failed: other > 0
+7Cxl2i5n
+TryFromIntErrorParseIntErrorNegOverflowPosOverflowInvalidDigit
+TryFromSliceError
+Utf8Errorvalid_up_toerror_len
+LayoutalignLayoutError&
+finished (bytes locationposition    true <= ZeroCharfilelinesize%
+thstndrd
+0123456789ABCDEF0123456789abcdef
+(join-%u)
+(subquery-%u)
+unix-none
+unix-dotfile
+unix-excl
+unix-posix
+unix-flock
+unix-afp
+unix-nfs
+unix-proxy
+PRAGMA "%w".page_count
+ATTACH x AS %Q
+source and destination must be distinct
+string or blob too big
+cannot open virtual table: %s
+cannot open table without rowid: %s
+cannot open view: %s
+no such column: "%s"
+foreign key
+cannot open %s column for writing
+temporary
+unknown database: %s
+no such table column: %s.%s
+2022-07-21 15:24:47 698edb77537b67c41adc68f9b892db56bcf9a55e00371a61420f3ddd668e6603
+unopened
+API call with %s database connection pointer
+cannot fstat db file %s
+file unlinked while open: %s
+multiple links to file: %s
+file renamed while open: %s
+os_unix.c:%d: (%d) %s(%s) - %s
+ftruncate
+full_fsync
+%s/etilqs_%llx%c
+/var/tmp
+/usr/tmp
+:auto: (not held)
+path error (len %d)
+read error (len %d)
+create failed (%d)
+write failed (%d)
+rename failed (%d)
+broke stale lock on %s
+failed to break stale lock on %s, %s
+sqliteplocks
+attempt to open "%s" as file descriptor %d
+/dev/null
+cannot open file
+%s at line %d of [%.10s]
+readonly_shm
+pwrite64
+fallocate
+openDirectory
+getpagesize
+readlink
+SQLITE_FORCE_PROXY_LOCKING
+/dev/urandom
+SQLITE_TMPDIR
+memdb(%p,%lld)
+unknown database %s
+unable to open a temporary database file for storing temporary tables
+:memory:
+immutable
+recovered %d frames from WAL file %s
+database corruption
+cannot limit WAL size: %s
+recovered %d pages from %s
+destination database is in use
+API called with finalized prepared statement
+FOREIGN KEY constraint failed
+%.4c%s%.16c
+MJ delete: %s
+MJ collide: %s
+-mj%06X9%02X
+922337203685477580
+out of memory
+API called with NULL prepared statement
+%.18s-%s
 Savepoint
 AutoCommit
 Transaction
 Checkpoint
 JournalMode
 InitCoroutine
 MustBeInt
@@ -1705,52 +2353,108 @@
 Pagecount
 MaxPgcnt
 ClrSubtype
 FilterAdd
 CursorHint
 ReleaseReg
 Abortable
-tbl,idx,stat
-tbl,idx,neq,nlt,ndlt,sample
-sqlite_stat3
-sqlite_detach
-sqlite_attach
-UTF-16le
-UTF-16be
-frame starting offset must be a non-negative integer
-frame ending offset must be a non-negative integer
-frame starting offset must be a non-negative number
-frame ending offset must be a non-negative number
+NOT NULL
+FOREIGN KEY
+%s constraint failed
+abort at %d in [%s]: %s
+cannot store %s value in %s column %s.%s
+cannot open savepoint - SQL statements in progress
+no such savepoint: %s
+cannot release savepoint - SQL statements in progress
+cannot commit transaction - SQL statements in progress
+cannot start a transaction within a transaction
+cannot rollback - no transaction is active
+cannot commit - no transaction is active
+database schema has changed
+index corruption
+sqlite_master
+SELECT*FROM"%w".%s WHERE %s ORDER BY rowid
+too many levels of trigger recursion
+cannot change %s wal mode from within a transaction
+database table is locked: %s
+ValueList
+statement aborts at %d: [%s] %s
+sqlite_temp_master
+CREATE TABLE x(type text,name text,tbl_name text,rootpage int,sql text)
+attached databases must use the same text encoding as main database
+unsupported file format
+SELECT*FROM"%w".%s ORDER BY rowid
+invalid rootpage
+orphan index
 drop column
 add column
-SQL logic error
-access permission denied
-query aborted
-database is locked
-database table is locked
-attempt to write a readonly database
-disk I/O error
-unknown operation
-database or disk is full
-unable to open database file
-locking protocol
-constraint failed
-datatype mismatch
-authorization denied
-column index out of range
-file is not a database
-notification message
-warning message
-unix-none
-unix-dotfile
+error in %s %s after %s: %s
+malformed database schema (%s)
+database schema is locked: %s
+statement too long
+sqlite_stat1
+SELECT tbl,idx,stat FROM %Q.sqlite_stat1
+unordered*
+sz=[0-9]*
+noskipscan*
+sqlite_stat4
+SELECT idx,count(*) FROM %Q.sqlite_stat4 GROUP BY idx
+SELECT idx,neq,nlt,ndlt,sample FROM %Q.sqlite_stat4
+Main freelist: 
+max rootpage (%d) disagrees with header (%d)
+incremental_vacuum enabled with a max rootpage of zero
+Page %d is never used
+Pointer map page %d is referenced
+failed to get page %d
+freelist leaf count too big on page %d
+%s is %d but should be %d
+overflow list length
+invalid page number %d
+2nd reference to page %d
+Failed to read ptrmap key=%d
+Bad ptr map entry key=%d expected=(%d,%d) got=(%d,%d)
+Page %u: 
+unable to get the page. error code=%d
+btreeInitPage() returns error code %d
+free space corruption
+On tree page %u cell %d: 
+On page %u at right child: 
+Offset %d out of range %d..%d
+Extends off end of page
+Rowid %lld out of order
+Child page depth differs
+Multiple uses for byte %u of page %u
+Fragmentation of %d bytes reported as %d on page %u
+truncate
+cannot VACUUM from within a transaction
+cannot VACUUM - SQL statements in progress
+non-text filename
+ATTACH %Q AS vacuum_db
+output file already exists
+SELECT sql FROM "%w".sqlite_schema WHERE type='table'AND name<>'sqlite_sequence' AND coalesce(rootpage,1)>0
+SELECT sql FROM "%w".sqlite_schema WHERE type='index'
+SELECT'INSERT INTO vacuum_db.'||quote(name)||' SELECT*FROM"%w".'||quote(name)FROM vacuum_db.sqlite_schema WHERE type='table'AND coalesce(rootpage,1)>0
+INSERT INTO vacuum_db.sqlite_schema SELECT*FROM "%w".sqlite_schema WHERE type IN('view','trigger') OR(type='table'AND rootpage=0)
+no such module: %s
+vtable constructor called recursively: %s
+vtable constructor failed: %s
+vtable constructor did not declare schema: %s
+bind on a busy prepared statement: [%s]
+zeroblob(%d)
+cannot open value of type %s
+no such rowid: %lld
+no such view
+no such table
+%s: %s.%s
 analysis_limit
 application_id
 auto_vacuum
 automatic_index
 busy_timeout
+cache_size
 cache_spill
 case_sensitive_like
 cell_size_check
 checkpoint_fullfsync
 collation_list
 compile_options
 count_changes
@@ -1769,21 +2473,24 @@
 function_list
 hard_heap_limit
 ignore_check_constraints
 incremental_vacuum
 index_info
 index_list
 index_xinfo
+integrity_check
 journal_mode
 journal_size_limit
 legacy_alter_table
+lock_proxy_file
 locking_mode
 max_page_count
 mmap_size
 module_list
+optimize
 page_count
 page_size
 pragma_list
 query_only
 quick_check
 read_uncommitted
 recursive_triggers
@@ -1800,1127 +2507,1243 @@
 temp_store
 temp_store_directory
 trusted_schema
 user_version
 wal_autocheckpoint
 wal_checkpoint
 writable_schema
+CREATE TABLE x
+,arg HIDDEN
+,schema HIDDEN
 on_update
 on_delete
 dflt_value
 checkpointed
-stat_get
-stat_push
-stat_init
-/var/tmp
-/usr/tmp
-pwrite64
-fallocate
-getpagesize
-ATOMIC_INTRINSICS=1
-COMPILER=gcc-10.2.1 20210130 (Red Hat 10.2.1-11)
-DEFAULT_AUTOVACUUM
-DEFAULT_CACHE_SIZE=-2000
-DEFAULT_FILE_FORMAT=4
-DEFAULT_FOREIGN_KEYS
-DEFAULT_JOURNAL_SIZE_LIMIT=-1
-DEFAULT_MMAP_SIZE=0
-DEFAULT_PAGE_SIZE=4096
-DEFAULT_PCACHE_INITSZ=20
-DEFAULT_RECURSIVE_TRIGGERS
-DEFAULT_SECTOR_SIZE=4096
-DEFAULT_SYNCHRONOUS=2
-DEFAULT_WAL_AUTOCHECKPOINT=1000
-DEFAULT_WAL_SYNCHRONOUS=2
-DEFAULT_WORKER_THREADS=0
-ENABLE_API_ARMOR
-ENABLE_COLUMN_METADATA
-ENABLE_DBSTAT_VTAB
-ENABLE_FTS3
-ENABLE_FTS3_PARENTHESIS
-ENABLE_FTS5
-ENABLE_LOAD_EXTENSION
-ENABLE_MEMORY_MANAGEMENT
-ENABLE_RTREE
-ENABLE_STAT4
-HAVE_ISNAN
-MALLOC_SOFT_LIMIT=1024
-MAX_ATTACHED=10
-MAX_COLUMN=2000
-MAX_COMPOUND_SELECT=500
-MAX_DEFAULT_PAGE_SIZE=8192
-MAX_EXPR_DEPTH=1000
-MAX_FUNCTION_ARG=127
-MAX_LENGTH=1000000000
-MAX_LIKE_PATTERN_LENGTH=50000
-MAX_MMAP_SIZE=0x7fff0000
-MAX_PAGE_COUNT=1073741823
-MAX_PAGE_SIZE=65536
-MAX_SQL_LENGTH=1000000000
-MAX_TRIGGER_DEPTH=1000
-MAX_VARIABLE_NUMBER=32766
-MAX_VDBE_OP=250000000
-MAX_WORKER_THREADS=8
-MUTEX_PTHREADS
-SYSTEM_MALLOC
-TEMP_STORE=1
-THREADSAFE=1
-922337203685477580
-2022-07-21 15:24:47 698edb77537b67c41adc68f9b892db56bcf9a55e00371a61420f3ddd668e6603
-fts5_api_ptr
-sqlite_temp_schema
-sqlite_schema
-sqlite_master
-sqlite_temp_master
-unknown error
-abort due to ROLLBACK
-another row available
-no more rows available
-sqlite_returning
-string or blob too big
-(join-%u)
-(subquery-%u)
-out of memory
+database
+too many columns on %s
 not authorized
-authorizer malfunction
-Expression tree is too large (maximum depth %d)
-%s %T cannot reference objects in database %s
-%s cannot use variables
-unknown join type: %T%s%T%s%T
-%s RETURNING is not available on virtual tables
-ORDER BY
-INTERSECT
-UNION ALL
-%s clause should come after %s not before
-too many terms in compound SELECT
-object name reserved for internal use: %s
-table %s may not be altered
-table %s may not be modified
-cannot modify %s because it is a view
-misuse of aggregate: %s()
-sub-select returns %d columns - expected %d
-row value misused
-foreign key mismatch - "%w" referencing "%w"
-corrupt database
-unknown database %T
-not an error
-IN(...) element has %d term%s - expected %d
-foreign key on %s should reference only one column of table %T
-number of columns in foreign key does not match the number of columns in the referenced table
-unknown column "%s" in foreign key definition
-too many arguments on function %T
-too many terms in %s BY clause
-%r %s BY term out of range - should be between 1 and %d
-ORDER BY clause
-frame specification
-PARTITION clause
-cannot override %s of window: %s
-no such window: %s
-column%d
-database corruption
-%s at line %d of [%.10s]
-cannot fstat db file %s
-file unlinked while open: %s
-multiple links to file: %s
-file renamed while open: %s
-cannot limit WAL size: %s
-attempt to open "%s" as file descriptor %d
-/dev/null
-failed memory resize %u to %u bytes
-failed to allocate %u bytes of memory
-API call with %s database connection pointer
-os_unix.c:%d: (%d) %s(%s) - %s
-ftruncate
-/dev/urandom
-full_fsync
-unopened
-cannot open file
-openDirectory
-API called with NULL prepared statement
-API called with finalized prepared statement
-bind on a busy prepared statement: [%s]
-bad parameter or other API misuse
-temporary
-error in %s %s after %s: %s
-malformed database schema (%s)
-readlink
-unsupported frame specification
+sqlite3_extension_init
+no entry point [%s] in shared library [%s]
+error during initialization: %s
+unable to open shared library [%.*s]
+sqlite3_get_table() called with two or more incompatible queries
 no such collation sequence: %s
+unrecognized token: "%T"
+%s in "%s"
+parser stack overflow
+unknown table option: %.*s
+set list
+near "%T": syntax error
+qualified table names are not allowed on INSERT, UPDATE, and DELETE statements within triggers
+the INDEXED BY clause is not allowed on UPDATE or DELETE statements within triggers
+the NOT INDEXED clause is not allowed on UPDATE or DELETE statements within triggers
+generated column loop on "%s"
+misuse of aggregate: %#T()
+unknown function: %#T()
 %d columns assigned %d values
-syntax error after column name "%.*s"
-virtual tables cannot use computed columns
-generated columns cannot be part of the PRIMARY KEY
-error in generated column "%s"
-default value of column [%s] is not constant
-cannot use DEFAULT on a generated column
-too many columns on %s
-%s.rowid
+row value misused
+RAISE() may only be used within a trigger-program
 hex literal too big: %s%#T
-too many FROM clause terms, max: %d
-duplicate WITH table name: %s
-index '%q'
-Failed to read ptrmap key=%d
-Bad ptr map entry key=%d expected=(%d,%d) got=(%d,%d)
-overflow list length
-invalid page number %d
-2nd reference to page %d
-failed to get page %d
-freelist leaf count too big on page %d
-%s is %d but should be %d
-Page %u: 
-unable to get the page. error code=%d
-btreeInitPage() returns error code %d
-free space corruption
-On tree page %u cell %d: 
-On page %u at right child: 
-Offset %d out of range %d..%d
-Extends off end of page
-Rowid %lld out of order
-Child page depth differs
-Multiple uses for byte %u of page %u
-Fragmentation of %d bytes reported as %d on page %u
-zeroblob(%d)
-AUTOMATIC PARTIAL COVERING INDEX
-AUTOMATIC COVERING INDEX
-COVERING INDEX %s
-INDEX %s
- USING INTEGER PRIMARY KEY (%s
->? AND %s
- VIRTUAL TABLE INDEX %d:%s
- LEFT-JOIN
-FOREIGN KEY constraint failed
-a JOIN clause is required before %s
-cannot use RETURNING in a trigger
-DISTINCT aggregates must have exactly one argument
-USE TEMP B-TREE FOR %s(DISTINCT)
-json_each
-json_tree
-unable to delete/modify collation sequence due to active statements
-argument of ntile must be a positive integer
-integer overflow
-Invalid argument to rtreedepth()
-local time unavailable
-fts5: 2022-07-21 15:24:47 698edb77537b67c41adc68f9b892db56bcf9a55e00371a61420f3ddd668e6603
-vtable constructor called recursively: %s
-vtable constructor failed: %s
-vtable constructor did not declare schema: %s
-unable to delete/modify user-function due to active statements
-no query solution
-HAVING clause on a non-aggregate query
-aggregate functions are not allowed in the GROUP BY clause
-all VALUES must have the same number of terms
-SELECTs to the left and right of %s do not have the same number of result columns
-too many terms in ORDER BY clause
-%r ORDER BY term does not match any column in the result set
-rtreenode
-rtreedepth
-rtreecheck
-rtree_i32
-LIKE or GLOB pattern too complex
-ESCAPE expression must be a single character
-unordered*
-sz=[0-9]*
-noskipscan*
-%s.xBestIndex malfunction
-abbreviated query algorithm search
-SQLITE_TMPDIR
-second argument to nth_value must be a positive integer
-fts5vocab
-fts5_source_id
-case_sensitive
-tokenchars
-separators
-recovered %d frames from WAL file %s
-RtreeMatchArg
-hashsize
-automerge
-usermerge
-crisismerge
-readonly_shm
-0123456789abcdef
-JSON cannot hold BLOB values
-malformed JSON
-L* N* Co
-categories
-remove_diacritics
-json_object() requires an even number of arguments
-json_object() labels must be TEXT
-fts5: column queries are not supported (detail=none)
-no such column: %s
-memdb(%p,%lld)
-access to %z is prohibited
+unsafe use of %#T()
+sub-select returns %d columns - expected %d
+REUSE SUBQUERY %d
+%sSCALAR SUBQUERY %d
+CORRELATED 
+USING ROWID SEARCH ON TABLE %s FOR IN-OPERATOR
+USING INDEX %s FOR IN-OPERATOR
+REUSE LIST SUBQUERY %d
+%sLIST SUBQUERY %d
+authorizer malfunction
+ROLLBACK
+temporary table name must be unqualified
+%s %T already exists
+there is already an index named %s
+corrupt database
+unknown database %T
+object name reserved for internal use: %s
+unknown datatype for %s.%s: "%s"
+missing datatype for %s.%s
+AUTOINCREMENT not allowed on WITHOUT ROWID tables
+PRIMARY KEY missing on table %s
+must have at least one non-generated column
+CREATE %s %.*s
+UPDATE %Q.sqlite_master SET type='%s', name=%Q, tbl_name=%Q, rootpage=#%d, sql=%Q WHERE rowid=#%d
+CREATE TABLE %Q.sqlite_sequence(name,seq)
+tbl_name='%q' AND type!='trigger'
+sqlite_sequence
+the "." operator
+second argument to %#T() must be a constant between 0.0 and 1.0
+not authorized to use function: %#T
+non-deterministic functions
+%#T() may not be used as a window function
+aggregate
+misuse of %s function %#T()
+no such function: %#T
+wrong number of arguments to function %#T()
+FILTER may not be used with non-aggregate %#T()
+subqueries
+parameters
 partial index WHERE clauses
 index expressions
 CHECK constraints
 generated columns
-excluded
-ambiguous column name
-no such column
-aggregate
-the "." operator
 %s prohibited in %s
+excluded
 misuse of aliased aggregate %s
 misuse of aliased window function %s
 double-quoted string literal: "%w"
 coalesce
+no such column
+ambiguous column name
 %s: %s.%s.%s
-%s: %s.%s
-second argument to %#T() must be a constant between 0.0 and 1.0
-not authorized to use function: %#T
-non-deterministic functions
-unsafe use of %#T()
-%#T() may not be used as a window function
-misuse of %s function %#T()
-no such function: %#T
-wrong number of arguments to function %#T()
-FILTER may not be used with non-aggregate %#T()
+access to %z is prohibited
 RANGE with offset PRECEDING/FOLLOWING requires one ORDER BY expression
 FILTER clause may only be used with aggregate window functions
-subqueries
-parameters
-localhost
-invalid uri authority: %.*s
-no such %s mode: %s
-%s mode not allowed: %s
-no such vfs: %s
-sqlite3_extension_init
-no entry point [%s] in shared library [%s]
-error during initialization: %s
-unable to open shared library [%.*s]
-sqlite3_get_table() called with two or more incompatible queries
-fts3_tokenizer
-fts3tokenize
-unable to use function %s in the requested context
-JSON path error near '%q'
-no such cursor: %lld
-recursively defined fts5 content table
-no such tokenizer: %s
-error in tokenizer constructor
-unknown tokenizer: %s
-unknown tokenizer
-argument type mismatch
-fts3tokenize disabled
-instance
-fts5vocab: unknown table type: %Q
-a CHECK constraint
-a generated column
-an index
-non-deterministic use of %s() in %s
-json_%s() needs an odd number of arguments
-wrong number of arguments to function highlight()
-wrong number of arguments to function snippet()
-40f-21a-21d
-julianday
-localtime
-unixepoch
-weekday 
-start of 
-%s/etilqs_%llx%c
-unix-excl
-recovered %d pages from %s
-SQLite format 3
-ValueList
-cannot detach database %s
-database %s is locked
-no such database: %s
-unable to close due to unfinalized statements or unfinished backups
-:memory:
-immutable
-unable to open a temporary database file for storing temporary tables
-unknown database %s
-source and destination must be distinct
-destination database is in use
-%.4c%s%.16c
-MJ delete: %s
-MJ collide: %s
--mj%06X9%02X
-fts5: %s queries are not supported (detail!=full)
-unterminated string
-fts5: syntax error near "%.1s"
-fts5: parser stack overflow
-fts5: syntax error near "%.*s"
-expected integer, got "%.*s"
-GROUP BY
-DISTINCT
- USING COVERING INDEX 
-RIGHT PART OF ORDER BY
+no such window: %s
+HAVING clause on a non-aggregate query
+aggregate functions are not allowed in the GROUP BY clause
+too many references to "%s": max 65535
+access to view "%s" prohibited
+unsafe use of virtual table "%s"
+%s.%s.%s
+no such table: %s
+no tables specified
+too many columns in result set
+column%d
+no such index: "%s"
+multiple references to recursive table: %s
+circular reference: %s
+table %s has %d values for %d columns
+multiple recursive references: %s
+recursive reference in a subquery: %s
+'%s' is not a function
+view %s is circularly defined
+no such index: %s
+a NATURAL join may not have an ON or USING clause
+cannot join using column %s - column not present in both tables
+ambiguous reference to %s in USING()
+%r %s BY term out of range - should be between 1 and %d
+too many terms in %s BY clause
+all VALUES must have the same number of terms
+SELECTs to the left and right of %s do not have the same number of result columns
+UNION ALL
+INTERSECT
+too many terms in ORDER BY clause
+%r ORDER BY term does not match any column in the result set
+Expression tree is too large (maximum depth %d)
+CREATE TABLE 
+generated
+duplicate column name: %s
+default value of column [%s] is not constant
+cannot use DEFAULT on a generated column
+table "%s" has more than one primary key
+AUTOINCREMENT is only allowed on an INTEGER PRIMARY KEY
+generated columns cannot be part of the PRIMARY KEY
+unsupported use of NULLS %s
+cannot create a TEMP index on non-TEMP table "%s"
+table %s may not be indexed
+views may not be indexed
+virtual tables may not be indexed
+there is already a table named %s
+index %s already exists
+sqlite_autoindex_%s_%d
+expressions prohibited in PRIMARY KEY and UNIQUE constraints
+conflicting ON CONFLICT clauses specified
+CREATE%s INDEX %.*s
+INSERT INTO %Q.sqlite_master VALUES('index',%Q,%Q,#%d,%Q);
+name='%q' AND type='index'
+%s cannot use variables
+%s %T cannot reference objects in database %s
+index '%q'
+foreign key on %s should reference only one column of table %T
+number of columns in foreign key does not match the number of columns in the referenced table
+unknown column "%s" in foreign key definition
+virtual tables cannot use computed columns
+error in generated column "%s"
+table %s may not be dropped
+use DROP TABLE to delete table %s
+use DROP VIEW to delete view %s
+sqlite_stat%d
+DELETE FROM %Q.%s WHERE %s=%Q
+DELETE FROM %Q.sqlite_sequence WHERE name=%Q
+DELETE FROM %Q.sqlite_master WHERE tbl_name=%Q and type!='trigger'
+DELETE FROM %Q.sqlite_master WHERE name=%Q AND type='trigger'
+corrupt schema
+UPDATE %Q.sqlite_master SET rootpage=%d WHERE #%d AND rootpage=#%d
+parameters are not allowed in views
 target object/alias may not appear in FROM clause: %s
 expected %d columns for '%s' but got %d
 CO-ROUTINE %!S
 MATERIALIZE %!S
-USE TEMP B-TREE FOR %s
-SCAN %s%s%s
-CORRELATED 
-REUSE SUBQUERY %d
-%sSCALAR SUBQUERY %d
-REUSE LIST SUBQUERY %d
-%sLIST SUBQUERY %d
-USING ROWID SEARCH ON TABLE %s FOR IN-OPERATOR
-USING INDEX %s FOR IN-OPERATOR
-generated column loop on "%s"
-misuse of aggregate: %#T()
-unknown function: %#T()
-RAISE() may only be used within a trigger-program
-RETURNING may not use "TABLE.*" wildcards
-sqlite\_%
+DISTINCT
+GROUP BY
+RIGHT PART OF ORDER BY
+ORDER BY
+misuse of aggregate: %s()
+too many FROM clause terms, max: %d
+COMPOUND QUERY
+LEFT-MOST SUBQUERY
+%s USING TEMP B-TREE
+SCAN %d CONSTANT ROW%s
+cannot use window functions in recursive queries
+recursive aggregate queries not supported
+RECURSIVE STEP
+MERGE (%s)
+at most %d tables in a join
+SCAN CONSTANT ROW
+too many arguments on %s() - max %d
 ON clause references tables to its right
-BLOOM FILTER ON %S (
+abbreviated query algorithm search
+%s.xBestIndex malfunction
+no query solution
 automatic index on %s(%s)
 auto-index
+BLOOM FILTER ON %S (
+PRIMARY KEY
+AUTOMATIC PARTIAL COVERING INDEX
+AUTOMATIC COVERING INDEX
+COVERING INDEX %s
+INDEX %s
+ USING INTEGER PRIMARY KEY (%s
+>? AND %s
+ VIRTUAL TABLE INDEX %d:%s
+ LEFT-JOIN
 MULTI-INDEX OR
 INDEX %d
-at most %d tables in a join
-SCAN CONSTANT ROW
-too many arguments on %s() - max %d
+frame starting offset must be a non-negative integer
+frame ending offset must be a non-negative integer
+second argument to nth_value must be a positive integer
+frame starting offset must be a non-negative number
+frame ending offset must be a non-negative number
 RIGHT-JOIN %s
-SCAN %d CONSTANT ROW%s
-cannot use window functions in recursive queries
-recursive aggregate queries not supported
-RECURSIVE STEP
-MERGE (%s)
-COMPOUND QUERY
-LEFT-MOST SUBQUERY
-%s USING TEMP B-TREE
-no such module: %s
-view %s is circularly defined
-unknown datatype for %s.%s: "%s"
-missing datatype for %s.%s
-AUTOINCREMENT not allowed on WITHOUT ROWID tables
-PRIMARY KEY missing on table %s
-must have at least one non-generated column
-CREATE TABLE 
-CREATE %s %.*s
-UPDATE %Q.sqlite_master SET type='%s', name=%Q, tbl_name=%Q, rootpage=#%d, sql=%Q WHERE rowid=#%d
-CREATE TABLE %Q.sqlite_sequence(name,seq)
-tbl_name='%q' AND type!='trigger'
-sqlite_sequence
-ROLLBACK
-unrecognized token: "%T"
-parser stack overflow
-unknown table option: %.*s
-generated
-parameters are not allowed in views
-set list
+USE TEMP B-TREE FOR %s
+DISTINCT aggregates must have exactly one argument
+USE TEMP B-TREE FOR %s(DISTINCT)
+SCAN %s%s%s
+ USING COVERING INDEX 
+%s clause should come after %s not before
+too many terms in compound SELECT
+a JOIN clause is required before %s
+unknown join type: %T%s%T%s%T
+rows deleted
+%s RETURNING is not available on virtual tables
+table %s may not be modified
+cannot modify %s because it is a view
+-- TRIGGER %s
+foreign key mismatch - "%w" referencing "%w"
+RETURNING may not use "TABLE.*" wildcards
+cannot use RETURNING in a trigger
+sqlite_returning
 too many columns in %s
+cannot UPDATE generated column "%s"
+no such column: %s
+rows updated
+%s.rowid
+cannot INSERT into generated column "%s"
+table %S has no column named %s
+table %S has %d columns but %d values were supplied
+%d values for %d columns
+UPSERT not implemented for virtual table "%s"
+cannot UPSERT a view
+rows inserted
+%sON CONFLICT clause does not match any PRIMARY KEY or UNIQUE constraint
 variable number must be between ?1 and ?%d
 too many SQL variables
-near "%T": syntax error
+too many arguments on function %T
 DISTINCT is not supported for window functions
+IN(...) element has %d term%s - expected %d
+syntax error after column name "%.*s"
 no such index: %S
 index associated with UNIQUE or PRIMARY KEY constraint cannot be dropped
 DELETE FROM %Q.sqlite_master WHERE name=%Q AND type='index'
-sqlite_stat%d
-DELETE FROM %Q.%s WHERE %s=%Q
+exclusive
+not a writable directory
+failed to set lock proxy file
+Safety level may not be changed inside a transaction
+SELECT*FROM"%w"
+iissssss
+*** in database %s ***
+NULL value in %s.%s
+non-%s value in %s.%s
+CHECK constraint failed in %s
+ missing from index 
+non-unique entry in index 
+wrong # of entries in index 
+UTF-16le
+UTF-16be
+unsupported encoding: %s
+ANALYZE "%w"."%w"
+incremental
+temporary storage cannot be changed from within a transaction
+sqlite_schema
+sqlite_temp_schema
+SET NULL
+SET DEFAULT
+RESTRICT
+NO ACTION
+LIKE or GLOB pattern too complex
+ESCAPE expression must be a single character
 INSERT INTO %Q.sqlite_master VALUES('trigger',%Q,%Q,0,'CREATE TRIGGER %q')
 type='trigger' AND name='%q'
 temporary trigger may not have qualified name
 cannot create triggers on virtual tables
 trigger %T already exists
 cannot create trigger on system table
 cannot create %s trigger on view: %S
 cannot create INSTEAD OF trigger on table: %S
-qualified table names are not allowed on INSERT, UPDATE, and DELETE statements within triggers
-the INDEXED BY clause is not allowed on UPDATE or DELETE statements within triggers
-the NOT INDEXED clause is not allowed on UPDATE or DELETE statements within triggers
-unsupported use of NULLS %s
 no such trigger: %S
+sqlite_attach
+too many attached databases - max %d
+database %s is already in use
+database is already attached
+unable to open database: %s
+invalid uri authority: %.*s
+no such %s mode: %s
+%s mode not allowed: %s
+no such vfs: %s
+sqlite_detach
+no such database: %s
+cannot detach database %s
+database %s is locked
+unable to identify the object to be reindexed
+tbl,idx,stat
+tbl,idx,neq,nlt,ndlt,sample
+sqlite_stat3
+CREATE TABLE %Q.%s(%s)
+sqlite\_%
+stat_init
+stat_push
+stat_get
 there is already another table or index with this name: %s
 view %s may not be altered
 UPDATE "%w".sqlite_master SET sql = sqlite_rename_table(%Q, type, name, sql, %Q, %Q, %d) WHERE (type!='index' OR tbl_name=%Q COLLATE nocase)AND   name NOT LIKE 'sqliteX_%%' ESCAPE 'X'
 UPDATE %Q.sqlite_master SET tbl_name = %Q, name = CASE WHEN type='table' THEN %Q WHEN name LIKE 'sqliteX_autoindex%%' ESCAPE 'X'      AND type='index' THEN 'sqlite_autoindex_' || %Q || substr(name,%d+18) ELSE name END WHERE tbl_name=%Q COLLATE nocase AND (type='table' OR type='index' OR type='trigger');
 UPDATE "%w".sqlite_sequence set name = %Q WHERE name = %Q
 UPDATE sqlite_temp_schema SET sql = sqlite_rename_table(%Q, type, name, sql, %Q, %Q, 1), tbl_name = CASE WHEN tbl_name=%Q COLLATE nocase AND   sqlite_rename_test(%Q, sql, type, name, 1, 'after rename', 0) THEN %Q ELSE tbl_name END WHERE type IN ('view', 'trigger')
 after rename
+table %s may not be altered
+SELECT 1 FROM "%w".sqlite_master WHERE name NOT LIKE 'sqliteX_%%' ESCAPE 'X' AND sql NOT LIKE 'create virtual%%' AND sqlite_rename_test(%Q, sql, type, name, %d, %Q, %d)=NULL 
 SELECT 1 FROM temp.sqlite_master WHERE name NOT LIKE 'sqliteX_%%' ESCAPE 'X' AND sql NOT LIKE 'create virtual%%' AND sqlite_rename_test(%Q, sql, type, name, 1, %Q, %d)=NULL 
+Cannot add a PRIMARY KEY column
+Cannot add a UNIQUE column
+Cannot add a REFERENCES column with non-NULL default value
+Cannot add a NOT NULL column with default value NULL
+Cannot add a column with non-constant default
+cannot add a STORED column
+UPDATE "%w".sqlite_master SET sql = printf('%%.%ds, ',sql) || %Q || substr(sql,1+length(printf('%%.%ds',sql))) WHERE type = 'table' AND name = %Q
+SELECT CASE WHEN quick_check GLOB 'CHECK*' THEN raise(ABORT,'CHECK constraint failed') ELSE raise(ABORT,'NOT NULL constraint failed') END  FROM pragma_quick_check(%Q,%Q) WHERE quick_check GLOB 'CHECK*' OR quick_check GLOB 'NULL*'
+SELECT raise(ABORT,%Q) FROM "%w"."%w"
+no such column: "%T"
+cannot drop %s column: "%s"
+cannot drop column "%s": no other columns exist
+UPDATE "%w".sqlite_master SET sql = sqlite_drop_column(%d, sql, %d) WHERE (type=='table' AND tbl_name=%Q COLLATE nocase)
+after drop column
+virtual table
+cannot %s %s "%s"
+drop column from
+rename columns of
+UPDATE "%w".sqlite_master SET sql = sqlite_rename_quotefix(%Q, sql)WHERE name NOT LIKE 'sqliteX_%%' ESCAPE 'X' AND sql NOT LIKE 'create virtual%%'
+UPDATE temp.sqlite_master SET sql = sqlite_rename_quotefix('temp', sql)WHERE name NOT LIKE 'sqliteX_%%' ESCAPE 'X' AND sql NOT LIKE 'create virtual%%'
 virtual tables may not be altered
 Cannot add a column to a view
 sqlite_altertab_%s
+UPDATE "%w".sqlite_master SET sql = sqlite_rename_column(sql, type, name, %Q, %Q, %d, %Q, %d, %d) WHERE name NOT LIKE 'sqliteX_%%' ESCAPE 'X'  AND (type != 'index' OR tbl_name = %Q)
+UPDATE temp.sqlite_master SET sql = sqlite_rename_column(sql, type, name, %Q, %Q, %d, %Q, %d, 1) WHERE type IN ('trigger', 'view')
+CREATE VIRTUAL TABLE %T
+UPDATE %Q.sqlite_master SET type='table', name=%Q, tbl_name=%Q, rootpage=0, sql=%Q WHERE rowid=#%d
+name=%Q AND sql=%Q
+duplicate WITH table name: %s
+PARTITION clause
+ORDER BY clause
+frame specification
+cannot override %s of window: %s
+unsupported frame specification
 incomplete input
-%s in "%s"
-duplicate column name: %s
-SELECT 1 FROM "%w".sqlite_master WHERE name NOT LIKE 'sqliteX_%%' ESCAPE 'X' AND sql NOT LIKE 'create virtual%%' AND sqlite_rename_test(%Q, sql, type, name, %d, %Q, %d)=NULL 
-?	)	&	#	-
-database schema is locked: %s
-statement too long
-SELECT * FROM %Q.%Q
-UNIQUE constraint failed: %s.%s
-rtree constraint failed: %s.(%s<=%s)
-SELECT rowid, rank FROM %Q.%Q ORDER BY %s("%w"%s%s) %s
-INSERT INTO '%q'.'%q_idx'(segid,term,pgno) VALUES(?,?,?)
-invalid rootpage
-orphan index
-CREATE TABLE x(type text,name text,tbl_name text,rootpage int,sql text)
-attached databases must use the same text encoding as main database
-unsupported file format
-SELECT*FROM"%w".%s ORDER BY rowid
-cannot start a transaction within a transaction
-cannot rollback - no transaction is active
-cannot commit - no transaction is active
-database disk image is malformed
-%s constraint failed
-abort at %d in [%s]: %s
-cannot store %s value in %s column %s.%s
-cannot open savepoint - SQL statements in progress
-cannot release savepoint - SQL statements in progress
-cannot commit transaction - SQL statements in progress
-database schema has changed
-index corruption
-SELECT*FROM"%w".%s WHERE %s ORDER BY rowid
-Main freelist: 
-max rootpage (%d) disagrees with header (%d)
-incremental_vacuum enabled with a max rootpage of zero
-Page %d is never used
-Pointer map page %d is referenced
-too many levels of trigger recursion
-cannot change %s wal mode from within a transaction
-statement aborts at %d: [%s] %s
-no such savepoint: %s
-database table is locked: %s
-	~	_	6	$	
+implies_nonnull_row
+expr_compare
+expr_implies_expr
+affinity
+load_extension
+sqlite_compileoption_used
+sqlite_compileoption_get
+unlikely
+likelihood
+randomblob
+sqlite_version
+sqlite_source_id
+sqlite_log
+last_insert_rowid
+total_changes
+zeroblob
+substring
+group_concat
+integer overflow
+sqlite_rename_column
+sqlite_rename_table
+sqlite_rename_test
+sqlite_drop_column
+sqlite_rename_quotefix
+error in %s %s%s%s: %s
+argument of ntile must be a positive integer
+julianday
+unixepoch
+datetime
+strftime
+current_time
+current_timestamp
+current_date
+a CHECK constraint
+a generated column
+an index
+non-deterministic use of %s() in %s
+40f-21a-21d
+localtime
+weekday 
+start of 
+local time unavailable
+json_array
+json_array_length
+json_extract
+json_insert
+json_object
+json_patch
+json_quote
+json_remove
+json_replace
+json_set
+json_type
+json_valid
+json_group_array
+json_group_object
+malformed JSON
+JSON path error near '%q'
+JSON cannot hold BLOB values
+0123456789abcdef
+json_%s() needs an odd number of arguments
+json_object() requires an even number of arguments
+json_object() labels must be TEXT
+failed to allocate %u bytes of memory
+failed memory resize %u to %u bytes
+Sqlite_Heap
+unable to close due to unfinalized statements or unfinished backups
+not an error
+SQL logic error
+access permission denied
+query aborted
+database is locked
+database table is locked
+attempt to write a readonly database
 interrupted
-%.18s-%s
+disk I/O error
+database disk image is malformed
+unknown operation
+database or disk is full
+unable to open database file
+locking protocol
+constraint failed
+datatype mismatch
+bad parameter or other API misuse
+authorization denied
+column index out of range
+file is not a database
+notification message
+warning message
+unknown error
+abort due to ROLLBACK
+another row available
+no more rows available
+unable to delete/modify user-function due to active statements
+unable to use function %s in the requested context
 PRAGMA table_list
-unknown database: %s
-ALTER TABLE %Q.'%q_node'   RENAME TO "%w_node";ALTER TABLE %Q.'%q_parent' RENAME TO "%w_parent";ALTER TABLE %Q.'%q_rowid'  RENAME TO "%w_rowid";
-DROP TABLE '%q'.'%q_node';DROP TABLE '%q'.'%q_rowid';DROP TABLE '%q'.'%q_parent';
-DROP TABLE IF EXISTS %Q.'%q_data';DROP TABLE IF EXISTS %Q.'%q_idx';DROP TABLE IF EXISTS %Q.'%q_config';
-DROP TABLE IF EXISTS %Q.'%q_docsize';
-DROP TABLE IF EXISTS %Q.'%q_content';
+unicode61
+fts3_tokenizer
+matchinfo
+CREATE TABLE x(term, col, documents, occurrences, languageid HIDDEN)
+invalid arguments to fts4aux constructor
+DELETE FROM %Q.'%q_content' WHERE rowid = ?
+SELECT NOT EXISTS(SELECT docid FROM %Q.'%q_content' WHERE rowid!=?)
+DELETE FROM %Q.'%q_content'
+DELETE FROM %Q.'%q_segments'
+DELETE FROM %Q.'%q_segdir'
+DELETE FROM %Q.'%q_docsize'
+DELETE FROM %Q.'%q_stat'
+SELECT %s WHERE rowid=?
+SELECT (SELECT max(idx) FROM %Q.'%q_segdir' WHERE level = ?) + 1
+REPLACE INTO %Q.'%q_segments'(blockid, block) VALUES(?, ?)
+SELECT coalesce((SELECT max(blockid) FROM %Q.'%q_segments') + 1, 1)
+REPLACE INTO %Q.'%q_segdir' VALUES(?,?,?,?,?,?)
+SELECT idx, start_block, leaves_end_block, end_block, root FROM %Q.'%q_segdir' WHERE level = ? ORDER BY idx ASC
+SELECT idx, start_block, leaves_end_block, end_block, root FROM %Q.'%q_segdir' WHERE level BETWEEN ? AND ?ORDER BY level DESC, idx ASC
+SELECT count(*) FROM %Q.'%q_segdir' WHERE level = ?
+SELECT max(level) FROM %Q.'%q_segdir' WHERE level BETWEEN ? AND ?
+DELETE FROM %Q.'%q_segdir' WHERE level = ?
+DELETE FROM %Q.'%q_segments' WHERE blockid BETWEEN ? AND ?
+INSERT INTO %Q.'%q_content' VALUES(%s)
+DELETE FROM %Q.'%q_docsize' WHERE docid = ?
+REPLACE INTO %Q.'%q_docsize' VALUES(?,?)
+SELECT size FROM %Q.'%q_docsize' WHERE docid=?
+SELECT value FROM %Q.'%q_stat' WHERE id=?
+REPLACE INTO %Q.'%q_stat' VALUES(?,?)
+DELETE FROM %Q.'%q_segdir' WHERE level BETWEEN ? AND ?
+SELECT ? UNION SELECT level / (1024 * ?) FROM %Q.'%q_segdir'
+SELECT level, count(*) AS cnt FROM %Q.'%q_segdir'   GROUP BY level HAVING cnt>=?  ORDER BY (level %% 1024) ASC, 2 DESC LIMIT 1
+SELECT 2 * total(1 + leaves_end_block - start_block)   FROM (SELECT * FROM %Q.'%q_segdir'         WHERE level = ? ORDER BY idx ASC LIMIT ?  )
+DELETE FROM %Q.'%q_segdir' WHERE level = ? AND idx = ?
+UPDATE %Q.'%q_segdir' SET idx = ? WHERE level=? AND idx=?
+SELECT idx, start_block, leaves_end_block, end_block, root FROM %Q.'%q_segdir' WHERE level = ? AND idx = ?
+UPDATE %Q.'%q_segdir' SET start_block = ?, root = ?WHERE level = ? AND idx = ?
+SELECT 1 FROM %Q.'%q_segments' WHERE blockid=? AND block IS NULL
+SELECT idx FROM %Q.'%q_segdir' WHERE level=? ORDER BY 1 ASC
+SELECT max( level %% 1024 ) FROM %Q.'%q_segdir'
+SELECT level, idx, end_block FROM %Q.'%q_segdir' WHERE level BETWEEN ? AND ? ORDER BY level DESC, idx ASC
+UPDATE OR FAIL %Q.'%q_segdir' SET level=-1,idx=? WHERE level=? AND idx=?
+UPDATE OR FAIL %Q.'%q_segdir' SET level=? WHERE level=-1
+%s_segments
+argument type mismatch
+fts3tokenize disabled
+unknown tokenizer: %s
+tokenize
+compress
+uncompress
+languageid
+notindexed
+unrecognized matchinfo: %s
+unrecognized order: %s
+unrecognized parameter: %s
+error parsing prefix parameter: %s
+missing %s parameter in fts4 constructor
+unknown tokenizer
+SELECT * FROM %Q.%Q
+,%s(x.'c%d%q')
+, x.'%q'
+ FROM '%q'.'%q%s' AS x
+_content
+docid INTEGER PRIMARY KEY
+%z, 'c%d%q'
+%z, langid
+CREATE TABLE %Q.'%q_content'(%s)
+CREATE TABLE %Q.'%q_segments'(blockid INTEGER PRIMARY KEY, block BLOB);
+CREATE TABLE %Q.'%q_segdir'(level INTEGER,idx INTEGER,start_block INTEGER,leaves_end_block INTEGER,end_block INTEGER,root BLOB,PRIMARY KEY(level, idx));
+CREATE TABLE %Q.'%q_docsize'(docid INTEGER PRIMARY KEY, size BLOB);
+CREATE TABLE IF NOT EXISTS %Q.'%q_stat'(id INTEGER PRIMARY KEY, value BLOB);
+PRAGMA %Q.page_size
+__langid
+CREATE TABLE x(%s %Q HIDDEN, docid HIDDEN, %Q HIDDEN)
 DROP TABLE IF EXISTS %Q.'%q_segments';DROP TABLE IF EXISTS %Q.'%q_segdir';DROP TABLE IF EXISTS %Q.'%q_docsize';DROP TABLE IF EXISTS %Q.'%q_stat';%s DROP TABLE IF EXISTS %Q.'%q_content';
-PRAGMA "%w".page_count
-ATTACH x AS %Q
-cannot VACUUM from within a transaction
-cannot VACUUM - SQL statements in progress
-non-text filename
-ATTACH %Q AS vacuum_db
-output file already exists
-SELECT sql FROM "%w".sqlite_schema WHERE type='table'AND name<>'sqlite_sequence' AND coalesce(rootpage,1)>0
-SELECT sql FROM "%w".sqlite_schema WHERE type='index'
-SELECT'INSERT INTO vacuum_db.'||quote(name)||' SELECT*FROM"%w".'||quote(name)FROM vacuum_db.sqlite_schema WHERE type='table'AND coalesce(rootpage,1)>0
-INSERT INTO vacuum_db.sqlite_schema SELECT*FROM "%w".sqlite_schema WHERE type IN('view','trigger') OR(type='table'AND rootpage=0)
-%s%.3x+%.6x
-internal
-corrupted
-SELECT * FROM (SELECT 'sqlite_schema' AS name,1 AS rootpage,'table' AS type UNION ALL SELECT name,rootpage,type FROM "%w".sqlite_schema WHERE rootpage!=0)
-WHERE name=%Q
- ORDER BY name
-%_parent
-SELECT parentnode FROM %Q.'%q_parent' WHERE nodeno=?1
-SELECT nodeno FROM %Q.'%q_rowid' WHERE rowid=?1
-Mapping (%lld -> %lld) missing from %s table
-Found (%lld -> %lld) in %s table, expected (%lld -> %lld)
-REPLACE INTO '%q'.'%q_data'(id, block) VALUES(?,?)
-DELETE FROM '%q'.'%q_data' WHERE id>=? AND id<=?
-SELECT %s
-no such function: %s
-%lld %lld
+SELECT %s WHERE rowid BETWEEN %lld AND %lld ORDER BY rowid %s
+SELECT %s ORDER BY rowid %s
+FTS expression tree is too large (maximum depth %d)
+malformed MATCH expression: [%s]
 SELECT %s WHERE rowid = ?
-SELECT data FROM %Q.'%q_node' WHERE nodeno=?
-Node %lld missing from database
-Node %lld is too small (%d bytes)
-Rtree depth out of range (%d)
-Node %lld is too small for cell count of %d (%d bytes)
-Dimension %d of cell %d on node %lld is corrupt
-Dimension %d of cell %d on node %lld is corrupt relative to parent
-sqlite_stat1
-sqlite_stat4
-SELECT tbl,idx,stat FROM %Q.sqlite_stat1
-SELECT idx,count(*) FROM %Q.sqlite_stat4 GROUP BY idx
-SELECT idx,neq,nlt,ndlt,sample FROM %Q.sqlite_stat4
-SELECT count(*) FROM %Q.'%q_%s'
-PRAGMA %Q.data_version
-wrong number of arguments to function rtreecheck()
-SELECT * FROM %Q.'%q_rowid'
-Schema corrupt or not an rtree
-SELECT count(*) FROM %Q.'%q%s'
-Wrong number of entries in %%%s table - expected %lld, actual %lld
 fts3cursor
-cannot open value of type %s
-no such rowid: %lld
-too many attached databases - max %d
-database %s is already in use
-database is already attached
-unable to open database: %s
-no such table column: %s.%s
-unable to identify the object to be reindexed
-integrity_check
-no such view
-no such table
-exclusive
-incremental
-NO ACTION
-SET NULL
-SET DEFAULT
-RESTRICT
-truncate
-temporary storage cannot be changed from within a transaction
-not a writable directory
-Safety level may not be changed inside a transaction
-SELECT*FROM"%w"
-iissssss
-*** in database %s ***
-NULL value in %s.%s
-non-%s value in %s.%s
-CHECK constraint failed in %s
- missing from index 
-non-unique entry in index 
-wrong # of entries in index 
-unsupported encoding: %s
-ANALYZE "%w"."%w"
-foreign key
-cannot open virtual table: %s
-cannot open table without rowid: %s
-cannot open view: %s
-no such column: "%s"
-cannot open %s column for writing
-SELECT k, v FROM %Q.'%q_config'
-invalid fts5 file format (found %d, expected %d) - run 'rebuild'
-%s_segments
+integrity-check
+automerge=
+%lld %lld
+SELECT %s
+<b>...</b>
+wrong number of arguments to function snippet()
+illegal first argument to %s
+%d %d %d %d 
+Index optimized
+Index already optimal
+SAVEPOINT fts3
+RELEASE fts3
+ROLLBACK TO fts3
+unrecognized matchinfo request: %c
 ALTER TABLE %Q.'%q_content'  RENAME TO '%q_content';
 ALTER TABLE %Q.'%q_docsize'  RENAME TO '%q_docsize';
 ALTER TABLE %Q.'%q_stat'  RENAME TO '%q_stat';
 ALTER TABLE %Q.'%q_segments' RENAME TO '%q_segments';
 ALTER TABLE %Q.'%q_segdir'   RENAME TO '%q_segdir';
-SAVEPOINT fts3
-illegal first argument to %s
-RELEASE fts3
-ROLLBACK TO fts3
-Index optimized
-Index already optimal
-%d %d %d %d 
-<b>...</b>
-unrecognized matchinfo request: %c
-DELETE FROM %Q.'%q_data';DELETE FROM %Q.'%q_idx';
-DELETE FROM %Q.'%q_docsize';
-FTS expression tree is too large (maximum depth %d)
-malformed MATCH expression: [%s]
-SELECT %s WHERE rowid BETWEEN %lld AND %lld ORDER BY rowid %s
-SELECT %s ORDER BY rowid %s
-integrity-check
-CREATE TABLE IF NOT EXISTS %Q.'%q_stat'(id INTEGER PRIMARY KEY, value BLOB);
-automerge=
-SELECT pgno FROM '%q'.'%q_idx' WHERE segid=? AND term<=? ORDER BY term DESC LIMIT 1
-unknown special query: %.*s
-parse error in rank function: %s
-%s: table does not support scanning
-DELETE FROM '%q'.'%q_idx' WHERE segid=?
-recursive definition for %s.%s
-SELECT t.%Q FROM %Q.%Q AS t WHERE t.%Q MATCH '*id'
-no such fts5 table: %s.%s
-ALTER TABLE %Q.'%q_%s' RENAME TO '%q_%s';
-DELETE from
-delete-all
-'delete-all' may only be used with a contentless or external content fts5 table
-'rebuild' may not be used with a contentless fts5 table
-SELECT segid, term, (pgno>>1), (pgno&1) FROM %Q.'%q_idx' WHERE segid=%d ORDER BY 1, 2
-cannot %s contentless fts5 table: %s
-no such index: %s
-cannot UPDATE generated column "%s"
-rows updated
--- TRIGGER %s
-cannot INSERT into generated column "%s"
-table %S has no column named %s
-table %S has %d columns but %d values were supplied
-%d values for %d columns
-UPSERT not implemented for virtual table "%s"
-cannot UPSERT a view
-%sON CONFLICT clause does not match any PRIMARY KEY or UNIQUE constraint
-rows inserted
-rows deleted
-temporary table name must be unqualified
-%s %T already exists
-there is already an index named %s
-DELETE FROM %Q.sqlite_master WHERE name=%Q AND type='trigger'
-corrupt schema
-UPDATE %Q.sqlite_master SET rootpage=%d WHERE #%d AND rootpage=#%d
-table %s may not be dropped
-use DROP TABLE to delete table %s
-use DROP VIEW to delete view %s
-DELETE FROM %Q.sqlite_sequence WHERE name=%Q
-DELETE FROM %Q.sqlite_master WHERE tbl_name=%Q and type!='trigger'
-cannot create a TEMP index on non-TEMP table "%s"
-table %s may not be indexed
-views may not be indexed
-virtual tables may not be indexed
-there is already a table named %s
-index %s already exists
-sqlite_autoindex_%s_%d
-expressions prohibited in PRIMARY KEY and UNIQUE constraints
-conflicting ON CONFLICT clauses specified
-CREATE%s INDEX %.*s
-INSERT INTO %Q.sqlite_master VALUES('index',%Q,%Q,#%d,%Q);
-name='%q' AND type='index'
-table "%s" has more than one primary key
-AUTOINCREMENT is only allowed on an INTEGER PRIMARY KEY
-CREATE TABLE %Q.%s(%s)
-Cannot add a PRIMARY KEY column
-Cannot add a UNIQUE column
-Cannot add a REFERENCES column with non-NULL default value
-SELECT raise(ABORT,%Q) FROM "%w"."%w"
-Cannot add a NOT NULL column with default value NULL
-Cannot add a column with non-constant default
-cannot add a STORED column
-SELECT CASE WHEN quick_check GLOB 'CHECK*' THEN raise(ABORT,'CHECK constraint failed') ELSE raise(ABORT,'NOT NULL constraint failed') END  FROM pragma_quick_check(%Q,%Q) WHERE quick_check GLOB 'CHECK*' OR quick_check GLOB 'NULL*'
-UPDATE "%w".sqlite_master SET sql = printf('%%.%ds, ',sql) || %Q || substr(sql,1+length(printf('%%.%ds',sql))) WHERE type = 'table' AND name = %Q
-CREATE VIRTUAL TABLE %T
-UPDATE %Q.sqlite_master SET type='table', name=%Q, tbl_name=%Q, rootpage=0, sql=%Q WHERE rowid=#%d
-name=%Q AND sql=%Q
-virtual table
-no such column: "%T"
-UPDATE "%w".sqlite_master SET sql = sqlite_rename_quotefix(%Q, sql)WHERE name NOT LIKE 'sqliteX_%%' ESCAPE 'X' AND sql NOT LIKE 'create virtual%%'
-UPDATE temp.sqlite_master SET sql = sqlite_rename_quotefix('temp', sql)WHERE name NOT LIKE 'sqliteX_%%' ESCAPE 'X' AND sql NOT LIKE 'create virtual%%'
-UPDATE "%w".sqlite_master SET sql = sqlite_rename_column(sql, type, name, %Q, %Q, %d, %Q, %d, %d) WHERE name NOT LIKE 'sqliteX_%%' ESCAPE 'X'  AND (type != 'index' OR tbl_name = %Q)
-UPDATE temp.sqlite_master SET sql = sqlite_rename_column(sql, type, name, %Q, %Q, %d, %Q, %d, 1) WHERE type IN ('trigger', 'view')
-rename columns of
-cannot %s %s "%s"
-cannot drop %s column: "%s"
-cannot drop column "%s": no other columns exist
-UPDATE "%w".sqlite_master SET sql = sqlite_drop_column(%d, sql, %d) WHERE (type=='table' AND tbl_name=%Q COLLATE nocase)
-after drop column
-drop column from
-CREATE TABLE x
-,arg HIDDEN
-,schema HIDDEN
-CREATE TABLE x(key,value,type,atom,id,parent,fullkey,path,json HIDDEN,root HIDDEN)
-wrong number of vtable arguments
+segments
+fts3tokenize
+CREATE TABLE x(input, token, start, end, position)
+fts5_source_id
 reserved fts5 table name: %s
 parse error in "%s"
+%Q.'%q_%s'
 malformed prefix=... directive
 too many prefix indexes (max %d)
 prefix length out of range (max 999)
-tokenize
 multiple tokenize=... directives
+parse error in tokenize directive
 multiple content=... directives
 content_rowid
 multiple content_rowid=... directives
 columnsize
 malformed columnsize=... directive
 malformed detail=... directive
 unrecognized option: "%.*s"
+no such tokenizer: %s
+error in tokenizer constructor
+case_sensitive
 reserved fts5 column name: %s
 unindexed
 unrecognized column option: %s
-%Q.'%q_%s'
 id INTEGER PRIMARY KEY, block BLOB
+segid, term, pgno, PRIMARY KEY(segid, term)
 CREATE TABLE %Q.'%q_%q'(%s)%s
-fts5: error creating shadow table %q_%s: %s
  WITHOUT ROWID
-segid, term, pgno, PRIMARY KEY(segid, term)
-k PRIMARY KEY, v
-id INTEGER PRIMARY KEY, sz BLOB
+fts5: error creating shadow table %q_%s: %s
+REPLACE INTO '%q'.'%q_data'(id, block) VALUES(?,?)
 id INTEGER PRIMARY KEY
+id INTEGER PRIMARY KEY, sz BLOB
+k PRIMARY KEY, v
+SELECT %s FROM %s T WHERE T.%Q >= ? AND T.%Q <= ? ORDER BY T.%Q ASC
+SELECT %s FROM %s T WHERE T.%Q <= ? AND T.%Q >= ? ORDER BY T.%Q DESC
+SELECT %s FROM %s T WHERE T.%Q=?
+REPLACE INTO %Q.'%q_content' VALUES(%s)
+DELETE FROM %Q.'%q_content' WHERE id=?
+DELETE FROM %Q.'%q_docsize' WHERE id=?
+SELECT sz FROM %Q.'%q_docsize' WHERE id=?
+REPLACE INTO %Q.'%q_config' VALUES(?,?)
+SELECT %s FROM %s AS T
 CREATE TABLE x(
 %z, %Q HIDDEN, %s HIDDEN)
-parse error in tokenize directive
-_content
-__langid
-unrecognized matchinfo: %s
-unrecognized order: %s
-unrecognized parameter: %s
-error parsing prefix parameter: %s
-missing %s parameter in fts4 constructor
-,%s(x.'c%d%q')
-, x.'%q'
- FROM '%q'.'%q%s' AS x
-docid INTEGER PRIMARY KEY
-%z, 'c%d%q'
-%z, langid
-CREATE TABLE %Q.'%q_content'(%s)
-CREATE TABLE %Q.'%q_segments'(blockid INTEGER PRIMARY KEY, block BLOB);
-CREATE TABLE %Q.'%q_segdir'(level INTEGER,idx INTEGER,start_block INTEGER,leaves_end_block INTEGER,end_block INTEGER,root BLOB,PRIMARY KEY(level, idx));
-CREATE TABLE %Q.'%q_docsize'(docid INTEGER PRIMARY KEY, size BLOB);
-CREATE TABLE x(%s %Q HIDDEN, docid HIDDEN, %Q HIDDEN)
-PRAGMA %Q.page_size
-CREATE TABLE x(term, col, documents, occurrences, languageid HIDDEN)
-invalid arguments to fts4aux constructor
-CREATE TABLE x(input, token, start, end, position)
-INSERT INTO"%w"."%w_rowid"(rowid,nodeno)VALUES(?1,?2)ON CONFLICT(rowid)DO UPDATE SET nodeno=excluded.nodeno
+PRAGMA %Q.data_version
+SELECT k, v FROM %Q.'%q_config'
+invalid fts5 file format (found %d, expected %d) - run 'rebuild'
+hashsize
+automerge
+usermerge
+crisismerge
+recursively defined fts5 content table
+DROP TABLE IF EXISTS %Q.'%q_data';DROP TABLE IF EXISTS %Q.'%q_idx';DROP TABLE IF EXISTS %Q.'%q_config';
+DROP TABLE IF EXISTS %Q.'%q_docsize';
+DROP TABLE IF EXISTS %Q.'%q_content';
+%s: table does not support scanning
+unknown special query: %.*s
+unterminated string
+fts5: syntax error near "%.1s"
+fts5: parser stack overflow
+fts5: %s queries are not supported (detail!=full)
+fts5: syntax error near "%.*s"
+expected integer, got "%.*s"
+fts5: column queries are not supported (detail=none)
+SELECT pgno FROM '%q'.'%q_idx' WHERE segid=? AND term<=? ORDER BY term DESC LIMIT 1
+parse error in rank function: %s
+SELECT rowid, rank FROM %Q.%Q ORDER BY %s("%w"%s%s) %s
+no such function: %s
+cannot %s contentless fts5 table: %s
+DELETE from
+delete-all
+'delete-all' may only be used with a contentless or external content fts5 table
+'rebuild' may not be used with a contentless fts5 table
+DELETE FROM %Q.'%q_data';DELETE FROM %Q.'%q_idx';
+DELETE FROM %Q.'%q_docsize';
+INSERT INTO '%q'.'%q_idx'(segid,term,pgno) VALUES(?,?,?)
+DELETE FROM '%q'.'%q_idx' WHERE segid=?
+DELETE FROM '%q'.'%q_data' WHERE id>=? AND id<=?
+SELECT count(*) FROM %Q.'%q_%s'
+SELECT segid, term, (pgno>>1), (pgno&1) FROM %Q.'%q_idx' WHERE segid=%d ORDER BY 1, 2
+no such cursor: %lld
+ALTER TABLE %Q.'%q_%s' RENAME TO '%q_%s';
+highlight
+wrong number of arguments to function highlight()
+L* N* Co
+categories
+remove_diacritics
+tokenchars
+separators
+fts5vocab
+CREATE TABlE vocab(term, col, doc, cnt)
+CREATE TABlE vocab(term, doc, cnt)
+CREATE TABlE vocab(term, doc, col, offset)
+wrong number of vtable arguments
+instance
+fts5vocab: unknown table type: %Q
+recursive definition for %s.%s
+SELECT t.%Q FROM %Q.%Q AS t WHERE t.%Q MATCH '*id'
+no such fts5 table: %s.%s
+fts5_api_ptr
+fts5: 2022-07-21 15:24:47 698edb77537b67c41adc68f9b892db56bcf9a55e00371a61420f3ddd668e6603
+rtreenode
+rtreedepth
+rtreecheck
+rtree_i32
+Invalid argument to rtreedepth()
+wrong number of arguments to function rtreecheck()
+SELECT * FROM %Q.'%q_rowid'
+Schema corrupt or not an rtree
+Node %lld is too small (%d bytes)
+Rtree depth out of range (%d)
+Node %lld is too small for cell count of %d (%d bytes)
+SELECT data FROM %Q.'%q_node' WHERE nodeno=?
+Node %lld missing from database
+Dimension %d of cell %d on node %lld is corrupt
+Dimension %d of cell %d on node %lld is corrupt relative to parent
+SELECT parentnode FROM %Q.'%q_parent' WHERE nodeno=?1
+SELECT nodeno FROM %Q.'%q_rowid' WHERE rowid=?1
+Mapping (%lld -> %lld) missing from %s table
+%_parent
+Found (%lld -> %lld) in %s table, expected (%lld -> %lld)
+SELECT count(*) FROM %Q.'%q%s'
+Wrong number of entries in %%%s table - expected %lld, actual %lld
+Wrong number of columns for an rtree table
+Too few columns for an rtree table
+Too many columns for an rtree table
+Auxiliary rtree columns must be last
 CREATE TABLE x(%.*s INT
+,%.*s REAL
+,%.*s INT
 SELECT length(data) FROM '%q'.'%q_node' WHERE nodeno = 1
 undersize RTree blobs in "%q_node"
+INSERT OR REPLACE INTO '%q'.'%q_node' VALUES(?1, ?2)
+DELETE FROM '%q'.'%q_node' WHERE nodeno = ?1
+SELECT nodeno FROM '%q'.'%q_rowid' WHERE rowid = ?1
+INSERT OR REPLACE INTO '%q'.'%q_rowid' VALUES(?1, ?2)
+DELETE FROM '%q'.'%q_rowid' WHERE rowid = ?1
+SELECT parentnode FROM '%q'.'%q_parent' WHERE nodeno = ?1
+INSERT OR REPLACE INTO '%q'.'%q_parent' VALUES(?1, ?2)
+DELETE FROM '%q'.'%q_parent' WHERE nodeno = ?1
+CREATE TABLE "%w"."%w_rowid"(rowid INTEGER PRIMARY KEY,nodeno
 );CREATE TABLE "%w"."%w_node"(nodeno INTEGER PRIMARY KEY,data);
 CREATE TABLE "%w"."%w_parent"(nodeno INTEGER PRIMARY KEY,parentnode);
 INSERT INTO "%w"."%w_node"VALUES(1,zeroblob(%d))
-SELECT stat FROM %Q.sqlite_stat1 WHERE tbl = '%q_rowid'
+INSERT INTO"%w"."%w_rowid"(rowid,nodeno)VALUES(?1,?2)ON CONFLICT(rowid)DO UPDATE SET nodeno=excluded.nodeno
 SELECT * FROM "%w"."%w_rowid" WHERE rowid=?1
 UPDATE "%w"."%w_rowid"SET 
-CREATE TABLE "%w"."%w_rowid"(rowid INTEGER PRIMARY KEY,nodeno
-error in %s %s%s%s: %s
-multiple recursive references: %s
-recursive reference in a subquery: %s
-'%s' is not a function
-no such index: "%s"
-multiple references to recursive table: %s
-circular reference: %s
-table %s has %d values for %d columns
-too many references to "%s": max 65535
-access to view "%s" prohibited
-unsafe use of virtual table "%s"
-a NATURAL join may not have an ON or USING clause
-cannot join using column %s - column not present in both tables
-ambiguous reference to %s in USING()
-%s.%s.%s
-no such table: %s
-no tables specified
-too many columns in result set
+ WHERE rowid=?1
+SELECT stat FROM %Q.sqlite_stat1 WHERE tbl = '%q_rowid'
+DROP TABLE '%q'.'%q_node';DROP TABLE '%q'.'%q_rowid';DROP TABLE '%q'.'%q_parent';
+RtreeMatchArg
+UNIQUE constraint failed: %s.%s
+rtree constraint failed: %s.(%s<=%s)
+ALTER TABLE %Q.'%q_node'   RENAME TO "%w_node";ALTER TABLE %Q.'%q_parent' RENAME TO "%w_parent";ALTER TABLE %Q.'%q_rowid'  RENAME TO "%w_rowid";
+SELECT * FROM (SELECT 'sqlite_schema' AS name,1 AS rootpage,'table' AS type UNION ALL SELECT name,rootpage,type FROM "%w".sqlite_schema WHERE rootpage!=0)
+WHERE name=%Q
+ ORDER BY name
+overflow
+%s%.3x+%.6x
+internal
+corrupted
+json_each
+json_tree
+CREATE TABLE x(key,value,type,atom,id,parent,fullkey,path,json HIDDEN,root HIDDEN)
 automatic extension loading failed: %s
- !"#$%&'()*+,-./0123456789:;<=>?@ABCDEFGHIJKLMNOPQRSTUVWXYZ[\]^_`abcdefghijklmnopqrstuvwxyz{|}~
-?,?,?,?,?,?,?,?,
-}<Afffff
-aceinouyyacdeeghijklnorstuuwyzouaiou
-aeiorusthae
-vwwxyzhtwya
-0123456789ABCDEF0123456789abcdef
-	:	;	<	=	>	A	I	M	N	P	Q	X	b	d	f	p	q	r	y	
-   ( ) * / 0 9 : ; ? A D E F G R S T U _ ` j p q t z } ~ 
-!$!%!&!'!(!)!*!.!/!0!4!5!9!:!<!>!@!E!G!J!K!L!N!O!P!`!
-# #"#)#*#+#|#}#
-'h'i'j'k'l'm'n'o'p'q'r's't'u'v'
-+0+E+G+P+
-,0,`,c,e,g,n,q,r,t,u,w,|,~,
--'---0-o-p-
-. .!.".#.$.%.&.'.(.).*./.0.:.
-0 0!0*0.000106080;0<0=0>0A0
-2 2*2H2P2Q2`2
-%vddUX*T
-cume_dist
-dense_rank
-first_value
-PPPPPP_PPiPnnPnnPPPPP[PPPedPPZgPPhP
-,,,,,,3M+
-55<@D5W\5]
-0123456789ABCDEF
-last_value
-nth_value
-percent_rank
-row_number
-******""""""""""""""""""""
-@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
-&&&&&&&&&&
-  !!""##$$%%&&''(())**++,,--..//00112233445566778899
- !"#$%&'()*+,-./0123456789:;<=>?@abcdefghijklmnopqrstuvwxyz[\]^_`abcdefghijklmnopqrstuvwxyz{|}~
-CREATE TABLE x( name       TEXT, path       TEXT, pageno     INTEGER, pagetype   TEXT, ncell      INTEGER, payload    INTEGER, unused     INTEGER, mx_payload INTEGER, pgoffset   INTEGER, pgsize     INTEGER, schema     TEXT HIDDEN, aggregate  BOOLEAN HIDDEN)
-REINDEXEDESCAPEACHECKEYBEFOREIGNOREGEXPLAINSTEADDATABASELECTABLEFTHENDEFERRABLELSEXCLUDELETEMPORARYISNULLSAVEPOINTERSECTIESNOTNULLIKEXCEPTRANSACTIONATURALTERAISEXCLUSIVEXISTSCONSTRAINTOFFSETRIGGERANGENERATEDETACHAVINGLOBEGINNEREFERENCESUNIQUERYWITHOUTERELEASEATTACHBETWEENOTHINGROUPSCASCADEFAULTCASECOLLATECREATECURRENT_DATEIMMEDIATEJOINSERTMATCHPLANALYZEPRAGMATERIALIZEDEFERREDISTINCTUPDATEVALUESVIRTUALWAYSWHENWHERECURSIVEABORTAFTERENAMEANDROPARTITIONAUTOINCREMENTCASTCOLUMNCOMMITCONFLICTCROSSCURRENT_TIMESTAMPRECEDINGFAILASTFILTEREPLACEFIRSTFOLLOWINGFROMFULLIMITIFORDERESTRICTOTHERSOVERETURNINGRIGHTROLLBACKROWSUNBOUNDEDUNIONUSINGVACUUMVIEWINDOWBYINITIALLYPRIMARY
-naturaleftouterightfullinnercross
-thstndrd
-onoffalseyestruextrafull
-value too large to transmit/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/message/frontend.rsstring contains embedded null
-description() is deprecated; use Display/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/byteorder-1.4.3/src/lib.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/task/list.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/scheduler/current_thread.rs
-attempt to calculate the remainder with a divisor of zero
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/prepare.rs
-`async fn` resumed after panicking
-`async fn` resumed after completion/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/std/src/io/mod.rsfailed to write whole bufferformatter errorfatal runtime error: 
-thread local panicked on drop
-core::option::Option<u32>i8alloc::string::Stringu32/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-0.19.5/src/connection.rsassertion failed: (*tail).value.is_none()/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/futures-channel-0.3.28/src/mpsc/queue.rsassertion failed: (*next).value.is_some()value too large to transmit/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/lib.rscannot access a Thread Local Storage value during or after destruction/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/std/src/thread/local.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/context.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/byteorder-1.4.3/src/lib.rs
-RELEASE 
-invalid message length: parameters is not drained
-`async fn` resumed after panicking
-`async fn` resumed after completion/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/transaction.rsROLLBACK TO /root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/simple_query.rstokio_postgres::simple_queryexecuting statement batch: /root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/query.rstokio_postgres::queryexecuting statement  with parameters: /root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/client.rsBEGIN
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/prepare.rsSELECT t.typname, t.typtype, t.typelem, r.rngsubtype, t.typbasetype, n.nspname, t.typrelid
-FROM pg_catalog.pg_type t
-LEFT OUTER JOIN pg_catalog.pg_range r ON r.rngtypid = t.oid
-INNER JOIN pg_catalog.pg_namespace n ON t.typnamespace = n.oid
-WHERE t.oid = $1
-SELECT t.typname, t.typtype, t.typelem, NULL::OID, t.typbasetype, n.nspname, t.typrelid
-FROM pg_catalog.pg_type t
-INNER JOIN pg_catalog.pg_namespace n ON t.typnamespace = n.oid
-WHERE t.oid = $1
-SELECT enumlabel
-FROM pg_catalog.pg_enum
-WHERE enumtypid = $1
-ORDER BY enumsortorder
-SELECT enumlabel
-FROM pg_catalog.pg_enum
-WHERE enumtypid = $1
-ORDER BY oid
-SELECT attname, atttypid
-FROM pg_catalog.pg_attribute
-WHERE attrelid = $1
-AND NOT attisdropped
-AND attnum > 0
-ORDER BY attnum
-s/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/message/backend.rsunexpected EOFfailed to fill whole bufferPoisonErrorinvalid message length: field is not drained/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/futures-channel-0.3.28/src/mpsc/mod.rscalled `Result::unwrap()` on an `Err` valuecalled `Option::unwrap()` on a `None` valueG,G
-: postgres::config/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-0.19.5/src/config.rscalled `Option::unwrap()` on a `None` value/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-0.19.5/src/transaction.rs
-Failed to `Enter::block_on`/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/scheduler/current_thread.rscore missinga spawned task panicked and the runtime is configured to shut down on unhandled panic
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/row.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/message/frontend.rs
-value too large to transmitstring contains embedded nulla Display implementation returned an error unexpectedly/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/alloc/src/string.rscalled `Result::unwrap()` on an `Err` value/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/byteorder-1.4.3/src/lib.rscannot advance past `remaining`: /root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/bytes-1.4.0/src/bytes.rsfatal runtime error: 
-thread result panicked on drop
-/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/core/src/str/mod.rsdescription() is deprecated; use Display/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/core/src/str/pattern.rs
-userhostport@
-Unixpasswordssl_mode/
-application_nametcp_user_timeoutunknown option `sslmodeconnect_timeoutkeepaliveskeepalives_idlekeepalives_intervalkeepalives_retriestarget_session_attrschannel_binding`invalid value for option `/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/config.rsunexpected character at byte : expected `` but got `unexpected EOFunterminated quoted connection parameter valuecalled `Option::unwrap()` on a `None` valueunterminated parameterUnknownOptionInvalidValue
-invalid message length: parameters is not drainedvalue too large to transmit/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/lib.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/message/backend.rsunexpected EOFfailed to fill whole buffer()
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/byteorder-1.4.3/src/lib.rsinvalid message length: field is not drained/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/client.rs
-`async fn` resumed after panicking
-`async fn` resumed after completion/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/prepare.rsspreparing query  with types : tokio_postgres::prepareSELECT t.typname, t.typtype, t.typelem, r.rngsubtype, t.typbasetype, n.nspname, t.typrelid
-FROM pg_catalog.pg_type t
-LEFT OUTER JOIN pg_catalog.pg_range r ON r.rngtypid = t.oid
-INNER JOIN pg_catalog.pg_namespace n ON t.typnamespace = n.oid
-WHERE t.oid = $1
-SELECT t.typname, t.typtype, t.typelem, NULL::OID, t.typbasetype, n.nspname, t.typrelid
-FROM pg_catalog.pg_type t
-INNER JOIN pg_catalog.pg_namespace n ON t.typnamespace = n.oid
-WHERE t.oid = $1
-SELECT enumlabel
-FROM pg_catalog.pg_enum
-WHERE enumtypid = $1
-ORDER BY enumsortorder
-SELECT enumlabel
-FROM pg_catalog.pg_enum
-WHERE enumtypid = $1
-ORDER BY oid
-SELECT attname, atttypid
-FROM pg_catalog.pg_attribute
-WHERE attrelid = $1
-AND NOT attisdropped
-AND attnum > 0
-ORDER BY attnum
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/query.rstokio_postgres::queryexecuting statement  with parameters: G,G
-called `Result::unwrap()` on an `Err` value/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/alloc/src/sync.rsassertion failed: (*tail).value.is_none()/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/futures-channel-0.3.28/src/mpsc/queue.rsassertion failed: (*next).value.is_some()
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/phf_shared-0.11.1/src/lib.rs
-attempt to calculate the remainder with a divisor of zero/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/message/backend.rsunexpected EOFinvalid message length: header length < 4invalid message length: parsing u32unknown message tag ``unknown authentication tag `invalid message length: expected buffer to be empty/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/phf-0.11.1/src/map.rscannot advance past `remaining`: Unix/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/bytes-1.4.0/src/bytes.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/codec.rscalled `Option::unwrap()` on a `None` valueROLLBACK TO 
-range start must not be greater than end: type/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/bytes-1.4.0/src/bytes.rsrange end out of bounds: PoisonError
-*6EKQW]ciou{/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/message/backend.rsinvalid message length: error fields is not drainedunexpected EOFfailed to fill whole buffer
-description() is deprecated; use DisplayINFOkindInfohintfileline`P` field did not contain an integer`p` field did not contain an integer`L` field did not contain an integer`V` field contained an invalid value`S` field missing`C` field missing`M` field missing`q` field missing but `p` field present: 
-DETAIL: 
-HINT: Errorcausetimeout waiting for servererror connecting to serverquery returned an unexpected number of rowsinvalid configurationinvalid connection stringauthentication errorerror encoding message to servererror parsing response from serverdb errorseveritypositiondatatypeInternalOriginalRowCountconnection closedexpected  parameters but got invalid column ``error deserializing column error serializing parameter error performing TLS handshakeunexpected message from servererror communicating with the serverLogDebugNoticeWarningFatalPanicparsed_severitymessagedetailwhere_schematablecolumnconstraintroutineDbErrorqueryTimeoutConnectConfigConfigParseAuthenticationEncodeParseDbClosedParametersColumnFromSqlToSqlTlsUnexpectedMessageIo
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/futures-channel-0.3.28/src/mpsc/mod.rsbuffer space exhausted; sending this messages would overflow the staterequested buffer size too largecalled `Result::unwrap()` on an `Err` valuecalled `Option::unwrap()` on a `None` value
-description() is deprecated; use Display
-XX002XX001XX000P0004P0003P0002P0001P0000HV00NHV00MHV00LHV00RHV00QHV00KHV00JHV00PHV001HV014HV009HV00AHV090HV00DHV00CHV00BHV091HV006HV004HV008HV007HV024HV021HV010HV002HV005HV000F0001F00007200058P0258P01580305800057P0557P0457P0357P0257P01570145700055P0455P0355P0255006550005402354011540015400053400533005320053100530004400042P1742P1642P1542P1442P1342P1242P114261142P1042P0942P084272542702427104271242P0742P0642P054272342P0442P03427014270442P0242P014288342703428C94280942P2242P2142P18428044293942622426024283042P1942P20428034284642501426014200040P01400034000140002400003F0003D0003B0013B00039P0339P0239P013900439001390003800438003380023800138000340002F0042F0032F0022F0052F0002D0002BP012B00028P0128000270002600025P0325P0225P012500725006250052500425003250082500225001250002400023P012351423505235032350223001230002203G2203F2203E2203D2203C2203B2203A220392203822037220362203522034220332203222031220302200T2200S2200N2200M2200L22P0522P0422P0322P0222P012200F22024220272201122001220262200H2200322002220042200G2200C220092202G2202H2201X2201W2201B22013220232201022P06220252200D2201922007220182201G2201F22016220142201E22015220222200B220052201222008220212202E2200021000200000Z0020Z0000P0000LP010L0000F0010F0000B0000A0000900008P0108007080040800108006080030800003000020010200001P0101004010060100701003010080100C0100000000SqlStateOtherEXX002EXX001EXX000EP0004EP0003EP0002EP0001EP0000EHV00NEHV00MEHV00LEHV00REHV00QEHV00KEHV00JEHV00PEHV001EHV014EHV009EHV00AEHV090EHV00DEHV00CEHV00BEHV091EHV006EHV004EHV008EHV007EHV024EHV021EHV010EHV002EHV005EHV000EF0001EF0000E72000E58P02E58P01E58030E58000E57P05E57P04E57P03E57P02E57P01E57014E57000E55P04E55P03E55P02E55006E55000E54023E54011E54001E54000E53400E53300E53200E53100E53000E44000E42P17E42P16E42P15E42P14E42P13E42P12E42P11E42611E42P10E42P09E42P08E42725E42702E42710E42712E42P07E42P06E42P05E42723E42P04E42P03E42701E42704E42P02E42P01E42883E42703E428C9E42809E42P22E42P21E42P18E42804E42939E42622E42602E42830E42P19E42P20E42803E42846E42501E42601E42000E40P01E40003E40001E40002E40000E3F000E3D000E3B001E3B000E39P03E39P02E39P01E39004E39001E39000E38004E38003E38002E38001E38000E34000E2F004E2F003E2F002E2F005E2F000E2D000E2BP01E2B000E28P01E28000E27000E26000E25P03E25P02E25P01E25007E25006E25005E25004E25003E25008E25002E25001E25000E24000E23P01E23514E23505E23503E23502E23001E23000E2203GE2203FE2203EE2203DE2203CE2203BE2203AE22039E22038E22037E22036E22035E22034E22033E22032E22031E22030E2200TE2200SE2200NE2200ME2200LE22P05E22P04E22P03E22P02E22P01E2200FE22024E22027E22011E22001E22026E2200HE22003E22002E22004E2200GE2200CE22009E2202GE2202HE2201XE2201WE2201BE22013E22023E22010E22P06E22025E2200DE22019E22007E22018E2201GE2201FE22016E22014E2201EE22015E22022E2200BE22005E22012E22008E22021E2202EE22000E21000E20000E0Z002E0Z000E0P000E0LP01E0L000E0F001E0F000E0B000E0A000E09000E08P01E08007E08004E08001E08006E08003E08000E03000E02001E02000E01P01E01004E01006E01007E01003E01008E0100CE01000E00000
-unexpected EOF/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/message/backend.rsinvalid message length: datarowrange is not emptyfailed to fill whole buffera Display implementation returned an error unexpectedly/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/alloc/src/string.rsu32i8alloc::string::Stringcore::option::Option<u32>invalid message length: field is not drainedserver did not use channel binding/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/row.rs
-no TLS implementation configured
-NoTlsError
-value too large to transmit/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/message/frontend.rsstring contains embedded null
-called `Result::unwrap()` on an `Err` value/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/byteorder-1.4.3/src/lib.rscannot advance past `remaining`: /root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/bytes-1.4.0/src/bytes.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/client.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/statement.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/transaction.rs
-Svalue too large to transmit/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/message/frontend.rsstring contains embedded null
-failed to fill whole buffer
-called `Result::unwrap()` on an `Err` value/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/byteorder-1.4.3/src/lib.rscannot advance past `remaining`: /root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/bytes-1.4.0/src/bytes.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/message/backend.rs/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/core/src/str/pattern.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/copy_in.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/prepare.rs
-`async fn` resumed after panicking
-`async fn` resumed after completioncalled `Option::unwrap()` on a `None` value/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-postgres-0.7.8/src/query.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/percent-encoding-2.3.0/src/lib.rs
-tried to create a `Socket` with an invalid fd/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/socket2-0.5.3/src/socket.rs
-messagetokio_util::codec::framed_impl/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-util-0.7.8/src/codec/framed_impl.rsevent /root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-util-0.7.8/src/codec/framed_impl.rs:302remainingevent /root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-util-0.7.8/src/codec/framed_impl.rs:285event /root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-util-0.7.8/src/codec/framed_impl.rs:280event /root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-util-0.7.8/src/codec/framed_impl.rs:223event /root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-util-0.7.8/src/codec/framed_impl.rs:208event /root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-util-0.7.8/src/codec/framed_impl.rs:204event /root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-util-0.7.8/src/codec/framed_impl.rs:201event /root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-util-0.7.8/src/codec/framed_impl.rs:189event /root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-util-0.7.8/src/codec/framed_impl.rs:167already mutably borrowed/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tracing-core-0.1.31/src/dispatcher.rsfatal runtime error: 
-thread local panicked on drop
-/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/std/src/io/mod.rsfailed to write whole bufferformatter error/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tracing-core-0.1.31/src/callsite.rsAttempted to register a `DefaultCallsite` that already exists! This will cause an infinite loop when attempting to read from the callsite cache. This is likely a bug! You should only need to call `DefaultCallsite::register` once per `DefaultCallsite`.
-Lazy instance has previously been poisoned/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/once_cell-1.18.0/src/lib.rscalled `Result::unwrap()` on an `Err` value/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tracing-core-0.1.31/src/callsite.rsPoisonError
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tracing-core-0.1.31/src/dispatcher.rsalready mutably borrowed
-/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/std/src/io/mod.rsfailed to write whole bufferformatter errorfatal runtime error: 
-thread local panicked on drop
-Index out of bounds
-internal error: entered unreachable code/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/core/src/slice/sort.rscalled `Option::unwrap()` on a `None` valueassertion failed: end >= start && end <= lenassertion failed: offset != 0 && offset <= lenassertion failed: handle.shared.owned.is_empty()/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/scheduler/current_thread.rstask panickedtask was cancelled/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/blocking/schedule.rs[internal exception] blocking task ran twice./root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/blocking/task.rsassertion failed: value <= self.max_value()/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/util/bit.rs
-/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/std/src/io/mod.rsfailed to write whole bufferformatter error
-Blocking/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/time/mod.rsassertion failed: !handle.is_shutdown()
-ItemDoneInit
-IntoIterReceiverThreadIdpointersNotifiedShutdowncalled `Option::unwrap()` on a `None` valueinternal error: entered unreachable code/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/sync/notify.rsassertion failed: actual_state == EMPTY || actual_state == NOTIFIEDtimer duration exceeds maximum durationtimer is at capacity and cannot create a new entrythe timer is shutdown, must be called from the context of Tokio runtime/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/io/registration.rsA Tokio 1.x context was found, but it is being shutdown.
-poisonedReadHalf/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/net/unix/stream.rstokio-runtime-worker
-called `Result::unwrap()` on an `Err` value/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/io/mod.rsunexpected error when polling the I/O driver: failed to wake I/O driverA Tokio 1.x context was found, but it is being shutdown.reactor at max registered I/O resources
-A Tokio 1.x context was found, but IO is disabled. Call `enable_io` on the runtime builder to enable IO.A Tokio 1.x context was found, but timers are disabled. Call `enable_time` on the runtime builder to enable timers.
-elapsed=/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/time/wheel/mod.rs; when=/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/time/sleep.rstimer error: called `Option::unwrap()` on a `None` value/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/util/slab.rspage is unallocatedunexpected pointerassertion failed: idx < self.slots.len()
-semaphore closedcannot access a Thread Local Storage value during or after destruction/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/std/src/thread/local.rs
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/net/addr.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/context.rsassertion failed: c.runtime.get().is_entered()
-&=;assertion failed: snapshot.is_complete()/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/task/harness.rsassertion failed: snapshot.is_join_interested()assertion failed: !snapshot.is_join_waker_set()assertion failed: next.is_notified()/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/task/state.rsassertion failed: curr.is_running()assertion failed: prev.is_running()assertion failed: !prev.is_complete()current: , sub: assertion failed: snapshot.ref_count() > 0assertion failed: curr.is_join_interested()assertion failed: !curr.is_join_waker_set()assertion failed: curr.is_join_waker_set()assertion failed: prev.ref_count() >= 1assertion failed: prev.ref_count() >= 2assertion failed: self.0 <= isize::MAX as usizeassertion failed: self.ref_count() > 0
-/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/alloc/src/vec/mod.rsOh no! We never placed the Core back, this is a bug!/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/scheduler/current_thread.rscalled `Option::unwrap()` on a `None` valuedriver missingunexpected stagecore missinginternal error: entered unreachable code: /root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/task/core.rsJoinHandle polled after completionwaker missing
-filled overflowfilled must not become larger than initializedcalled `Option::unwrap()` on a `None` value/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/io/poll_evented.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/io/read_buf.rsmark_pending called when the timer entry is in an invalid state/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/time/entry.rsTimer already firedA Tokio 1.x context was found, but it is being shutdown.RNG seed generator is internally corrupt/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/util/rand.rs/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/std/src/os/fd/owned.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/util/wake_list.rsassertion failed: self.curr <= NUM_WAKERSearly eof/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/net/tcp/stream.rsassertion failed: fd != u32::MAX as RawFd/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/time/wheel/level.rs
-attempt to divide by zerofatal runtime error: 
-thread local panicked on drop
-shutdown_on_drop_handle_lifetimealready mutably borrowed/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/context.rsCannot start a runtime from within a runtime. This happens because a function (like `block_on`) attempted to block the current thread while the thread is being used to drive asynchronous tasks./root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/time/mod.rscalled `Option::unwrap()` on a `None` value/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/blocking/shutdown.rsCannot drop a runtime in a context where blocking is not allowed. This happens when a runtime is dropped from within an asynchronous context.The Tokio context thread-local variable has been destroyed./root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/handle.rsthere is no reactor running, must be called from the context of a Tokio 1.x runtimecalled after complete/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/sync/oneshot.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/util/linked_list.rsassertion failed: self.tail.is_none()
-called `Option::unwrap()` on a `None` value/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/std/src/thread/mod.rsthread name may not contain interior null bytescalled `Result::unwrap()` on an `Err` valuefatal runtime error: 
-thread result panicked on dropPoisonErrorinconsistent park state; actual = /root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/park.rsinconsistent park_timeout state; actual = inconsistent park_timeout state: inconsistent state in unparkOS can't spawn worker thread: assertion failed: shared.shutdown_tx.is_some()/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tokio-1.28.2/src/runtime/blocking/pool.rsnum_idle_threads underflowed on thread exit
-overflow in Duration::new/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/core/src/time.rs
-path must be shorter than libc::sockaddr_un.sun_pathpath must be no longer than libc::sockaddr_un.sun_pathN.N
-(4@invalid buffer sizeltree version 1 only supportedlquery version 1 only supportedltxtquery version 1 only supportedfailed to fill whole buffer
-description() is deprecated; use Displaypg_catalog.a Postgres value was `NULL`cannot convert between the Rust type `` and the Postgres type ``CompositeDomainMultirangeRangeArrayPseudoEnumrustSimpleFieldtype_WasNullWrongTypepostgres&strboolu32alloc::string::Stringf32i32G,G
-aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaadaafaaah
-hjlqnqpr
-_int8multirange_datemultirange_tstzmultirange_tsmultirange_nummultirange_int4multirangeanycompatiblerangeanycompatiblenonarrayanycompatiblearrayanycompatiblexid8uuidvoid_bit_oid_box_cid_xid_tidinetcidrlseg_xmljsontextint4int2int8charXid8UuidVoidTimeInetCidrLinePathLsegJsonInt4Int2Int8NameCharBool_pg_snapshotpg_snapshotpg_mcv_listpg_brin_minmax_multi_summarypg_brin_bloom_summaryanycompatiblemultirangeanymultirangeint8multirangedatemultirangetstzmultirangetsmultirangenummultirangeint4multirange_regcollationregcollation_regrolejsonpath_tsrangenumrangeanyrange_tsquerytsvectorinternalanyarray_regtype_regoperregclass_cstring_numericinterval_macaddr_aclitem_polygon_varchar_regprocmacaddr8JsonpathNumRangeAnyRangeTsVectorAnyarrayRegclassBitArrayIntervalOidArrayBoxArrayCidArrayXidArrayTidArrayMacaddr8XmlArrayregrole_regnamespaceregnamespace_jsonpath_int8rangeint8range_daterangedaterange_tstzrangetstzrangetsrange_numrange_int4rangeint4rangeevent_trigger_jsonbjsonb_regdictionaryregdictionary_regconfigregconfig_gtsvector_tsvectorgtsvectortsqueryanyenumpg_dependenciespg_ndistincttsm_handler_pg_lsnpg_lsnfdw_handlertxid_snapshot_uuid_txid_snapshotanynonarray_recordanyelementlanguage_handlerindex_am_handlertable_am_handlerRegoperatorArrayTimestamptzArraytriggeranycstringrecord_regclass_regoperator_regprocedureregtyperegoperatorregoperregprocedure_refcursorrefcursornumeric_varbitvarbitbit_timetztimetz_interval_timestamptztimestamptz_time_date_timestamptimestampvarcharbpchar_inetaclitem_float8_float4_path_lseg_point_int8_bpchar_oidvector_text_int4_int2vector_int2_name_char_bytea_boolmacaddr_moneymoney_macaddr8_circlecircleunknownfloat8float4_cidr_linepolygonboxpoint_xid8_jsonpg_node_treexmlpg_ddl_commandoidvectorcidxidtidoidregprocint2vectorbyteaOtherschemaInt8multiRangeArrayDatemultiRangeArrayTstzmultiRangeArrayTsmultiRangeArrayNummultiRangeArrayInt4multiRangeArrayAnycompatibleRangeAnycompatiblenonarrayAnycompatiblearrayAnycompatiblePgSnapshotArrayPgSnapshotPgMcvListPgBrinMinmaxMultiSummaryPgBrinBloomSummaryAnycompatiblemultiRangeAnymultiRangeInt8multiRangeDatemultiRangeTstzmultiRangeTsmultiRangeNummultiRangeInt4multiRangeRegcollationArrayRegcollationRegroleArrayRegroleRegnamespaceArrayRegnamespaceJsonpathArrayInt8RangeArrayInt8RangeDateRangeArrayDateRangeTstzRangeArrayTstzRangeTsRangeArrayTsRangeNumRangeArrayInt4RangeArrayInt4RangeEventTriggerJsonbArrayJsonbRegdictionaryArrayRegdictionaryRegconfigArrayRegconfigTsqueryArrayGtsVectorArrayTsVectorArrayGtsVectorTsqueryAnyenumPgDependenciesPgNdistinctTsmHandlerPgLsnArrayPgLsnFdwHandlerTxidSnapshotUuidArrayTxidSnapshotArrayAnynonarrayRecordArrayAnyelementLanguageHandlerTriggerAnyCstringRecordRegtypeArrayRegclassArrayRegoperArrayRegprocedureArrayRegtypeRegoperatorRegoperRegprocedureRefcursorArrayRefcursorNumericVarbitArrayVarbitBitTimetzArrayTimetzCstringArrayNumericArrayIntervalArrayTimestamptzTimeArrayDateArrayTimestampArrayTimestampVarcharBpcharInetArrayMacaddrArrayAclitemArrayAclitemPolygonArrayFloat8ArrayFloat4ArrayPathArrayLsegArrayPointArrayInt8ArrayVarcharArrayBpcharArrayOidVectorArrayTextArrayRegprocArrayInt4ArrayInt2VectorArrayInt2ArrayNameArrayCharArrayByteaArrayBoolArrayMacaddrMoneyArrayMoneyMacaddr8ArrayCircleArrayCircleUnknownFloat8Float4CidrArrayLineArrayPolygonBoxPointIndexAmHandlerXid8ArrayTableAmHandlerJsonArrayPgNodeTreeXmlPgDdlCommandOidVectorCidXidTidOidRegprocInt2VectorBytea
-called `Result::unwrap()` on an `Err` value
-[HMAC is able to accept all key sizes/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/postgres-protocol-0.6.5/src/authentication/sasl.rs
-already checked abovep=tls-server-end-point,,n,,y,,n=,r=invalid SCRAM stateinvalid nonce
-?456789:;<=
- !"#$%&'()*+,-./0123
-ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789+/
-Client Keyc=,r=,,p=Server KeySCRAM error: SCRAM verification errorunexpected character at byte : expected `` but got `unexpected EOFunexpected trailing data at byte 
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/base64-0.21.2/src/chunked_encoder.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/base64-0.21.2/src/encode.rsusize overflow when calculating b64 lengthinteger overflow when calculating buffer size/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/base64-0.21.2/src/engine/mod.rsInvalid UTF8description() is deprecated; use Displaycalled `Option::unwrap()` on a `None` value/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/stringprep-0.1.2/src/lib.rs
-)))))))))))))))))))))))))))))))))
-)))))))))))))))))))))))))))))))))))))))))))))))
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tinyvec-1.6.0/src/arrayvec.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/unicode-normalization-0.1.22/src/decompose.rsIndex out of bounds
-/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/core/src/slice/sort.rscalled `Option::unwrap()` on a `None` valueassertion failed: end >= start && end <= lenassertion failed: offset != 0 && offset <= len/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/tinyvec-1.6.0/src/arrayvec.rs
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/unicode-normalization-0.1.22/src/lookups.rs
-could not initialize thread_rng: /root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rand-0.8.5/src/rngs/thread.rscannot access a Thread Local Storage value during or after destruction/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/std/src/thread/local.rs
-Ointernal error: entered unreachable code: state is never set to invalid values
-Once instance has previously been poisonedcalled `Option::unwrap()` on a `None` value/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/std/src/sync/once.rslibc::pthread_atfork failed with code /root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rand-0.8.5/src/rngs/adapter/reseeding.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rand-0.8.5/src/rngs/adapter/reseeding.rs
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/rand_chacha-0.3.1/src/guts.rsdescription() is deprecated; use Display
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/base64-0.21.2/src/engine/general_purpose/decode.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/base64-0.21.2/src/engine/general_purpose/mod.rsbase64 data was not utf8/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/base64-0.21.2/src/display.rs
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/base64-0.21.2/src/engine/general_purpose/decode_suffix.rsinternal error: entered unreachable code: Impossible: must only have 0 to 8 input bytes in last chunk, with no invalid lengths
-Invalid paddingInvalid last symbol , offset .Encoded text cannot have a 6-bit remainder.Invalid byte InvalidPaddingInvalidLastSymbolInvalidLengthInvalidByte
-internal error: entered unreachable code: Impossible remainder/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/base64-0.21.2/src/encode.rsDon't use a tiny buffer/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/base64-0.21.2/src/chunked_encoder.rsInvalidLength0123456789abcdef0123456789ABCDEFcalled `Option::unwrap()` on a `None` value/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/futures-core-0.3.28/src/task/__internal/atomic_waker.rs
-called `Result::unwrap()` on an `Err` valuedrop/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/bytes-1.4.0/src/bytes.rssplit_off out of bounds: split_to out of bounds: /root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/bytes-1.4.0/src/bytes_mut.rssplit_to out of bounds: set_end out of boundsnew_len = ; capacity = /root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/csv-1.2.2/src/byte_record.rscalled `Option::unwrap()` on a `None` value/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/csv-1.2.2/src/byte_record.rscalled `Option::unwrap()` on a `None` value
-nGV5}$ e
-G(SN\_T8h
- =U7el#|67
-00010203040506070809101112131415161718192021222324252627282930313233343536373839404142434445464748495051525354555657585960616263646566676869707172737475767778798081828384858687888990919293949596979899
-Dfa(N/A)has_readDfaState
-(024/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/csv-core-0.1.10/src/reader.rsinternal error: entered unreachable code
-	called `Option::unwrap()` on a `None` valueinternal error: entered unreachable code/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/csv-core-0.1.10/src/lib.rsattempted to fetch exception but none was set
-%cannot access a Thread Local Storage value during or after destruction/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/std/src/thread/local.rsa Display implementation returned an error unexpectedly/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/alloc/src/string.rs
-attempted to fetch exception but none was set/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/pyo3-0.18.3/src/gil.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/pyo3-0.18.3/src/impl_/panic.rsattempted to fetch exception but none was set
-The first GILGuard acquired must be the last one dropped./root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/pyo3-0.18.3/src/gil.rsalready mutably borrowed
-The Python interpreter is not initialized and the `auto-initialize` feature is not enabled.
-Consider calling `pyo3::prepare_freethreaded_python()` before attempting to use Python APIs.
-exceptions must derive from BaseException--- PyO3 is resuming a panic after fetching a PanicException from Python. ---
-Python stack trace below:
-Unwrapped panic from Python codeattempted to fetch exception but none was setFailed to initialize nul terminated exception name/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/pyo3-0.18.3/src/err/mod.rsFailed to initialize nul terminated docstringCannot access exception type while normalizingCannot normalize a PyErr while already normalizing it.Exception type missingException value missingPyErrvaluetraceback'' object cannot be converted to '<failed to extract type name>Python API call failed
-%Ucs4Ucs2Ucs1PyTzInfoStringIOgetvalueattempted to fetch exception but none was setutf-8
-surrogatepass
-%attempted to fetch exception but none was set
-?-6argumentSequencesequencePyBoolexceptions must derive from BaseExceptionargument '': ().were to was takes from  positional arguments but   given takes  got multiple values for argument '' got an unexpected keyword argument ' got some positional-only arguments passed as keyword arguments: arguments missing  required : keywordpositional
-__qualname__attempted to fetch exception but none was setPyListattempted to fetch exception but none was seta Display implementation returned an error unexpectedly/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/alloc/src/string.rsFunction name cannot contain NUL byte.Document cannot contain NUL byte.
-panic from Rust code
-UPyModulegaierror__name__attempted to fetch exception but none was setcalled `Option::unwrap()` on a `None` value/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/pyo3-0.18.3/src/sync.rsPyModule_GetName expected to return utf8/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/pyo3-0.18.3/src/types/module.rscould not append __name__ to __all__pyo3_runtime.PanicException
-The exception raised when Rust code called from Python panics.
-Like SystemExit, this exception is derived from BaseException so that
-it will typically propagate all the way through the stack and cause the
-Python interpreter to exit.
-Failed to initialize new exception type./root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/pyo3-0.18.3/src/panic.rs__all__attempted to fetch exception but none was setPyO3 modules may only be initialized once per interpreter process
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/parking_lot_core-0.9.8/src/parking_lot.rsOnce instance has previously been poisoned/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/parking_lot-0.12.1/src/once.rsfatal runtime error: 
-thread local panicked on drop
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/parking_lot_core-0.9.8/src/parking_lot.rs
-/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/std/src/io/mod.rsfailed to write whole bufferformatter errorcalled `Result::unwrap()` on an `Err` value/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/smallvec-1.10.0/src/lib.rscapacity overflowassertion failed: new_cap >= len/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/parking_lot_core-0.9.8/src/parking_lot.rs
-repeater stationnmea_parser::aishigh-speed craftclass_b_css_flagEngagedInFishingdimension_to_bowVesselStaticDataMedicalTransport
- $$$$$$$$$$
- $$$$$$$$$$
-Mismatching AIS types:  != portPortMismatching MMSI numbers: Mismatching IMO numbers: Mismatching AIS version indicators: Invalid station identifier/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/nmea-parser-0.10.0/src/ais/mod.rsClass BClass Aunknown
-Unexpected ship and cargo type: Unrecognized position fix type: 	
- !"#$%&'((((((((((23456789:;<<<<<<<<<<FFFFFFFFFFPPPPPPPPPPZZZZZZZZZZ
-/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/core/src/str/pattern.rsNo checksum found for sentence: Failed to parse fragment count: nmea_parser/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/nmea-parser-0.10.0/src/lib.rsInvalid checksum found for sentence: Corrupted NMEA sentence: $GGA$RMC$GNS$GSA$GSV$VTG$GLL$ALM$DTM$MSS$STN$VBW$ZDA!VDM!VDO$DPT$DBS$MTW$VHW$HDT$MWVInvalid NMEA sentence: $!NMEA sentence fragment count greater () than supported 2NMEA message_id missing from  than supported 2Unexpected NMEA fragment number: /Unsupported  message type: Unsupported sentence type: 
- out of bounds: wind_speed_knotsv
-?relativeNotValidrange /root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/bitvec-1.0.1/src/slice/api.rsAmbiguous local time, ranging from QZSSdataQzssNo such local time/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/offset/mod.rscalled `Option::unwrap()` on a `None` value/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/nmea-parser-0.10.0/src/gnss/mwv.rsInvalid talker identifier/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/nmea-parser-0.10.0/src/gnss/mod.rsUnrecognized FAA information value: !
-!$'+.158;AIVDM type 24 part number has unexpected value: invalid time/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/date.rs,
-naninfbit-vector capacity exceeded:  > 
-latitudegps_modealtitude/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/bitvec-1.0.1/src/vec.rsinvalid time
-mmsihdop/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/date.rs
-?capacityregionalassignedtimeout1timeout2timeout3timeout4
-bit-vector capacity exceeded:  > /root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/bitvec-1.0.1/src/vec.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/bitvec-1.0.1/src/vec/api.rsbit-vector capacity exceeded
-Unsupported AIVDM message type: 19
-invalid time/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/date.rsInvalid RMC variation side: Invalid RMC navigation receiver status: 
-Bad hemispehre: a Display implementation returned an error unexpectedly/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/alloc/src/string.rs
-called `Result::unwrap()` on an `Err` valueassertion failed: self.is_char_boundary(new_len)bit-vector capacity exceeded:  > /root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/bitvec-1.0.1/src/vec.rs
-@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@BBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZX^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^dbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdb,/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/nmea-parser-0.10.0/src/util.rsinvalid time/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/date.rs`DateTime - Duration` overflowedTime zone offset out of bounds: Failed to parse Utc Date from y:/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/datetime/mod.rsFailed to parse field : Failed to parse hex field Invalid time format: Invalid date format: 0:.0 m: d: h: s:Failed to parse latitude (DDMM.MMM) from Failed to parse longitude (DDDMM.MMM) from Failed to parse float: ;
-@Unrecognized Maneuver Indicator value: nmea_parser::ais::vdm_t1t2t3/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/nmea-parser-0.10.0/src/ais/vdm_t1t2t3.rs
-/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/core/src/str/pattern.rs
-Hash table capacity overflow/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/hashbrown-0.12.3/src/raw/mod.rs
-range  out of bounds: destination_mmsi/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/bitvec-1.0.1/src/slice/api.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/wyz-0.5.1/src/comu.rscalled `Option::unwrap()` on a `None` value..InvalidSentenceCorruptedSentenceUnsupportedSentenceType
-intervalAllTypesTime5secTime1minTime3minTime6minmode2_3d`NaiveDateTime + Duration` overflowed/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/naive/datetime/mod.rs
-called `Option::unwrap()` on a `None` value/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/offset/fixed.rsinternal error: entered unreachable code: This should never be reached as all four bit cases are covered (value: )/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/nmea-parser-0.10.0/src/ais/vdm_t23.rsInvalid GPGSA fix type: Invalid GPGSA mode: 
-getrandom::getrandom() failed./root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/ahash-0.7.6/src/random_state.rsErrorunknown_codeinternal_codedescriptionos_errorUnknown Error: OS Error: Node.js ES modules are not directly supported, see https://docs.rs/getrandom#nodejs-es-module-supportCalling Node.js API crypto.randomFillSync failedNode.js crypto CommonJS module is unavailablerandSecure: VxWorks RNG module is not initializedCalling Web API crypto.getRandomValues failedWeb Crypto API is unavailableRDRAND: instruction not supportedRDRAND: failed multiple times: CPU issue likelyRtlGenRandom: Windows system function failureSecRandomCopyBytes: iOS Security framework failureerrno: did not return a positive valuegetrandom: this target is not supported
-/dev/urandom
-/dev/random
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/once_cell-1.18.0/src/imp_std.rscalled `Option::unwrap()` on a `None` value
-/ :/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/format/strftime.rsassertion failed: nextspec > 0%-	
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/time-0.1.45/src/duration.rsDuration::seconds out of boundscalled `Option::unwrap()` on a `None` value/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/naive/time/mod.rs.
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/naive/internals.rs
-@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
-BBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBB
-HJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJ
-JLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJL
-NPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNP
-PRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPR
-TVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTV
-VXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVX
-XZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZ
-\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^
-^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`
-bdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbd
-@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@BBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZX^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^dbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdb
-ShortWeekdayNameNanosecond9NoDotNanosecond6NoDotNanosecond3NoDot
-FebruaryNovemberDecemberThursdaySaturdayInternalTooShort
-):>ADR_cjmquz
-internal error: entered unreachable code/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/format/mod.rs
-bad or unsupported format string
-trailing inputpremature end of inputinput contains invalid charactersinput is not enough for unique date and timeno possible date and time matching inputinput is out of rangeJanFebMarAprMayJunJulAugSepOctNovDecJanuaryMarchAprilJuneJulyZeroHourYearAugustSeptemberOctoberSunMonTueWedThuFriSatSundayMondayTuesdayWednesdayFridayAMPMDo not try to write %#z it is undefined.
-@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@BBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZX^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^dbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdb
-$Duration::days out of bounds/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/time-0.1.45/src/duration.rsDuration::seconds out of boundsinternal error: entered unreachable code/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/format/parsed.rs`NaiveDateTime - Duration` overflowed/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/naive/datetime/mod.rs
-@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@BBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBBJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHJHLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJLJPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNPNRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPRPVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTVTXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVXVZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZXZX^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\^\`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^`^dbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdbdb
-`NaiveDateTime + Duration` overflowed/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/naive/datetime/mod.rs
-    !!!!""""####$$$$%%%%&&&&''''(((())))****++++,,,,----....////00001111111122223333444455556666777788889999::::;;;;<<<<====>>>>????@@@@AAAABBBBCCCCDDDDEEEEFFFFGGGGHHHHIIIIIIIIJJJJKKKKLLLLMMMMNNNNOOOOPPPPQQQQRRRRSSSSTTTTUUUUVVVVWWWWXXXXYYYYZZZZ[[[[\\\\]]]]^^^^____````aaaa/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/naive/internals.rs/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/offset/fixed.rscalled `Option::unwrap()` on a `None` valueZUTC
-/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/format/parse.rsassertion failed: min <= max/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/format/scan.rs
-//////////////////////////
-%%%%%%%%%%%%%%%%%%%%%%%%%%
-assertion failed: min <= max/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/chrono-0.4.26/src/format/scan.rs
-uaryobersdayruarychileyusttemberemberdaynesdayrsdayurday/root/.cargo/registry/src/index.crates.io-6f17d22bba15001f/log-0.4.18/src/lib.rskey-value support is experimental and must be enabled using the `kv_unstable` featureAllocErrlayoutCapacityOverflow
-invalid filenameno storage spacehost unreachableconnection resetentity not foundprefix not found             at AddrNotAvailablePermissionDeniedStripPrefixErrorunix_exit_statuscpu.cfs_quota_usunix_wait_statusinvalid argument
-<8:@68:@6SW
-, line: MetadatamodifiedaccessedDirEntrydeadlock<locked> and/or thread '
-CapturedFileTypeDeadlockTimedOutNotFoundIncominglistenerDeviceNSVerbatimStartDirExitCodeFileDesctruncateMakePipeAbsoluteRelative (SIGIO)signal: .zdebug_
- $(,048<@DHLPTX\`dhlptx|
-/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/core/src/slice/iter.rsIndex out of bounds()/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/core/src/str/pattern.rs
-overflow in Duration::new/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/core/src/time.rs
-attempt to divide by zeroassertion failed: mid <= self.len()/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/core/src/slice/sort.rscalled `Option::unwrap()` on a `None` valueassertion failed: end >= start && end <= lenassertion failed: offset != 0 && offset <= lenassertion failed: offset != 0 && offset <= len && len >= 2called `Result::unwrap()` on an `Err` value
-assertion failed: idx < CAPACITYlibrary/std/src/thread/scoped.rsfailed to initiate panic, error library/std/src/sys/unix/rand.rsassertion failed: page_size != 0library/std/src/sys/unix/time.rs
-internal error: entered unreachable code: internal error: entered unreachable code/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/alloc/src/collections/btree/navigate.rs/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/alloc/src/vec/mod.rs/cargo/registry/src/index.crates.io-6f17d22bba15001f/gimli-0.26.2/src/read/line.rs
-attempt to calculate the remainder with a divisor of zero/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/core/src/num/uint_macros.rsSomeNonemainnameVarsArgskindKindcodeinitSinkpeer
-fullIterOnce/
-varsPATHaddrBothReadFullDiskDoneBodynextslotlistzeroFilepathreadHOMEargs && 
-modeNullNOEXiterWide/cargo/registry/src/index.crates.io-6f17d22bba15001f/addr2line-0.17.0/src/lib.rs/cargo/registry/src/index.crates.io-6f17d22bba15001f/addr2line-0.17.0/src/function.rsfatal runtime error: 
-library/std/src/rt.rstoo many running threads in thread scopeAccessErrorcannot access a Thread Local Storage value during or after destructionlibrary/std/src/thread/local.rsuse of std::thread::current() is not possible after the thread's local data has been destroyedlibrary/std/src/thread/mod.rsan irrecoverable error occurred while synchronizing threadsfailed to generate unique thread ID: bitspace exhaustedRUST_BACKTRACEfailed to write the buffered datalibrary/std/src/io/buffered/bufwriter.rs/library/std/src/io/buffered/linewritershim.rslibrary/std/src/io/readbuf.rsuncategorized errorother errorout of memoryunexpected end of fileunsupportedoperation interruptedargument list too longtoo many linkscross-device link or renameexecutable file busyresource busyfile too largefilesystem quota exceededseek on unseekable filewrite zerotimed outinvalid datainvalid input parameterstale network file handlefilesystem loop or indirection limit (e.g. symlink loop)read-only filesystem or storage mediumdirectory not emptyis a directorynot a directoryoperation would blockentity already existsbroken pipenetwork downaddress not availableaddress in usenot connectedconnection abortednetwork unreachableconnection refusedpermission deniedErrormessageOs (os error )library/std/src/io/stdio.rsfailed printing to : stdoutstderrlibrary/std/src/io/mod.rsfailed to fill whole bufferadvancing io slices beyond their lengthfailed to write whole bufferformatter errorfdlibrary/std/src/panic.rslibrary/std/src/path.rs.library/std/src/sync/once.rslock count overflow in reentrant mutexlibrary/std/src/sync/remutex.rsoverflow when adding duration to instantlibrary/std/src/time.rssecond time provided was later than selffile name contained an unexpected NUL bytestack backtrace:
-note: Some details are omitted, run with `RUST_BACKTRACE=full` for a verbose backtrace.
-__rust_begin_short_backtrace__rust_end_short_backtrace<unknown>RUST_MIN_STACKlibrary/std/src/sys_common/thread_info.rsassertion failed: thread_info.is_none()
-memory allocation of  bytes failedlibrary/std/src/alloc.rs bytes failed
-Rust panics must be rethrownRust cannot catch foreign exceptionslibrary/std/src/panicking.rsBox<dyn Any><unnamed>' panicked at '', note: run with `RUST_BACKTRACE=1` environment variable to display a backtrace
-thread panicked while processing panic. aborting.
-panicked after panic::always_abort(), aborting.
-thread caused non-unwinding panic. aborting.
-thread panicked while panicking. aborting.
-library/std/src/../../backtrace/src/symbolize/mod.rs       - :UnsupportedCustomerrorUncategorizedOtherOutOfMemoryUnexpectedEofInterruptedArgumentListTooLongInvalidFilenameTooManyLinksCrossesDevicesExecutableFileBusyResourceBusyFileTooLargeFilesystemQuotaExceededNotSeekableStorageFullWriteZeroInvalidDataInvalidInputStaleNetworkFileHandleFilesystemLoopReadOnlyFilesystemDirectoryNotEmptyIsADirectoryNotADirectoryWouldBlockAlreadyExistsBrokenPipeNetworkDownAddrInUseNotConnectedConnectionAbortedNetworkUnreachableHostUnreachableConnectionResetConnectionRefusedSystemTimeErroradvancing IoSlice beyond its lengthlibrary/std/src/sys/unix/io.rslibrary/std/src/sys/unix/net.rsfailed to lookup address information: strerror_r failurelibrary/std/src/sys/unix/os.rs/proc/self/exeno /proc/self/exe available. Is /proc mounted?unexpected getrandom error: /dev/urandomfailed to open /dev/urandomfailed to read /dev/urandomfailed to allocate an alternative stack: library/std/src/sys/unix/stack_overflow.rsfailed to set up alternative stack guard page: library/std/src/sys/unix/thread.rsfailed to join thread: there is no guard pagelibrary/std/src/sys/unix/thread_local_key.rsassertion failed: tv_nsec >= 0 && tv_nsec < NSEC_PER_SEC as i64too many active read locks on RwLocklibrary/std/src/sys/unix/locks/futex_rwlock.rsassertion failed: is_unlocked(state)state is never set to invalid valuesOnce instance has previously been poisonedassertion failed: key as usize != KEY_SENTVALassertion failed: len as usize >= mem::size_of::<c::sockaddr_in6>()library/std/src/sys_common/net.rsassertion failed: len as usize >= mem::size_of::<c::sockaddr_in>()invalid port valueinvalid socket addressUdpSocketlibrary/std/src/../../backtrace/src/symbolize/gimli/stash.rsassertion failed: mmap_aux.is_none()library/std/src/../../backtrace/src/symbolize/gimli.rslibrary/std/src/../../backtrace/src/symbolize/gimli/elf.rs/usr/lib/debug/usr/lib/debug/.build-id/__pthread_get_minstack
-An unknown DW_CFA_* instructiionThe line range must not be zero.Found an unknown extended opcodeFound an unknown standard opcodeDW_TAG_SUN_fortran_vax_structureDW_TAG_GNU_formal_parameter_packDW_AT_BORLAND_Delphi_constructor
-/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/alloc/src/collections/btree/node.rsassertion failed: edge.height == self.height - 1assertion failed: src.len() == dst.len().debug_types.debug_tu_index.debug_str_offsets.debug_str.debug_rnglists.debug_ranges.debug_pubtypes.debug_pubnames.debug_macro.debug_macinfo.debug_loclists.debug_loc.debug_line_str.debug_line.debug_info.eh_frame_hdr.eh_frame.debug_frame.debug_cu_index.debug_aranges.debug_addr.debug_abbrev
-EncodingRegisterDebugStrDebugLocSPSR_SVCSPSR_UNDSPSR_ABTSPSR_IRQSPSR_FIQUnknown DwSectV2DwAccessDW_OP_neDW_OP_ltDW_OP_leDW_OP_gtDW_OP_geDW_OP_eqDW_OP_oreh_frameIndirectop_indexLeftEdgeencodingRawRangeNotCieId/cargo/registry/src/index.crates.io-6f17d22bba15001f/gimli-0.26.2/src/read/abbrev.rs
-{invalid syntax}TryDemangleError*
-extern "()
-/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/core/src/ops/function.rs/rustc/84c898d65adf2f39a5a98507f1fe0ce10a2b8dbc/library/core/src/str/pattern.rscalled `Result::unwrap()` on an `Err` value/cargo/registry/src/index.crates.io-6f17d22bba15001f/rustc-demangle-0.1.21/src/legacy.rs__ZN) = u128i128for< as shimdyn mut  -> true::.@*&<>()C,called `Option::unwrap()` on a `None` value/cargo/registry/src/index.crates.io-6f17d22bba15001f/rustc-demangle-0.1.21/src/v0.rs`fmt::Error`s should be impossible without a `fmt::Formatter`punycode{-}0internal error: entered unreachable codeinternal error: entered unreachable code: str::from_utf8( was expected to have 1 char, but  chars were found..._!f64f32usizeu64u32u16u8isizei64i32i16i8str{recursion limit reached}?', > ::{closure:#[] + ; const  unsafe " fn( =  {  }false{: 0x.llvm./cargo/registry/src/index.crates.io-6f17d22bba15001f/rustc-demangle-0.1.21/src/lib.rs`fmt::Error` from `SizeLimitedFmtAdapter` was discarded{size limit reached}SizeLimitExhausted
-Hash table capacity overflow/cargo/registry/src/index.crates.io-6f17d22bba15001f/hashbrown-0.12.3/src/raw/mod.rs
-FilteredBadParamNeedDict3
-/cargo/registry/src/index.crates.io-6f17d22bba15001f/miniz_oxide-0.5.3/src/inflate/core.rs/cargo/registry/src/index.crates.io-6f17d22bba15001f/miniz_oxide-0.5.3/src/inflate/output_buffer.rs
-CapacityOverflowNotNulTerminatedcalled `Result::unwrap()` on an `Err` valuelibrary/alloc/src/raw_vec.rscapacity overflowlibrary/alloc/src/ffi/c_str.rscalled `Option::unwrap()` on a `None` valuenul byte found in provided data at position: a formatting trait implementation returned an errorlibrary/alloc/src/fmt.rslibrary/alloc/src/sync.rsbyteserrorFromUtf8Error
-0123456789abcdefrange end index ) when slicing `CharTryFromErrorDecodeUtf16ErrorTryFromCharError
-AChaystack (bytes AsciiStrBiasedFpexponentmantissanegativeInfinitevaliditybackiterSocketV6SocketV4LocationlocationLinesAnysearcherpositioncrit_posNegativeResumeTyRawWakerint8x8_t
-library/core/src/num/dec2flt/decimal.rs
-$ + 3 < F(P([(g0s0
-I)I>QSQiQ
-library/core/src/num/dec2flt/lemire.rsinvalid float literalcannot parse float from empty stringassertion failed: edelta >= 0library/core/src/num/diy_float.rs
-library/core/src/num/flt2dec/strategy/dragon.rsassertion failed: d.mant > 0assertion failed: d.minus > 0assertion failed: d.plus > 0assertion failed: d.mant.checked_add(d.plus).is_some()assertion failed: d.mant.checked_sub(d.minus).is_some()assertion failed: buf.len() >= MAX_SIG_DIGITS
-library/core/src/num/flt2dec/strategy/grisu.rsassertion failed: d.mant + d.plus < (1 << 61)
-attempt to divide by zeroassertion failed: !buf.is_empty()called `Option::unwrap()` on a `None` valueassertion failed: d.mant < (1 << 61)library/core/src/num/flt2dec/mod.rsassertion failed: buf[0] > b\'0\'assertion failed: parts.len() >= 40..assertion failed: parts.len() >= 6E-e-Ee-+0infNaN0E00e0assertion failed: buf.len() >= maxlenout of range integral type conversion attemptednumber would be zero for non-zero typenumber too small to fit in target typenumber too large to fit in target typeinvalid digit found in stringcannot parse integer from empty stringfrom_str_radix_int: must lie in the range `[2, 36]` - found library/core/src/num/mod.rs (1 << )..could not convert slice to arrayindex out of bounds: the len is library/core/src/fmt/builders.rslibrary/core/src/slice/memchr.rsBorrowErrorBorrowMutError
- but the index is iterItermantplusCopyLessTypeFuseIpv6Ipv4Leftwakeu8x2i8x2u8x4i8x4u8x8i8x8library/core/src/net/ip_addr.rslibrary/core/src/net/display_buffer.rs::::1internal error: entered unreachable code::ffff:library/core/src/net/parser.rs:library/core/src/net/socket_addr.rs[%]:panicked at '', library/core/src/panicking.rspanic in a function that cannot unwindmatches!===assertion failed: `(left  right)`
-  left: ``,
- right: ``: `called `Result::unwrap()` on an `Err` value:  {
-}, .. } { .. } }(
-{]attempted to begin a new map entry without completing the previous oneattempted to format a map value before its keyattempted to finish a map with a partial entrylibrary/core/src/fmt/num.rs0x00010203040506070809101112131415161718192021222324252627282930313233343536373839404142434445464748495051525354555657585960616263646566676869707172737475767778798081828384858687888990919293949596979899library/core/src/fmt/mod.rs0000000000000000000000000000000000000000000000000000000000000000false()range start index  out of range for slice of length slice index starts at  but ends at attempted to index slice up to maximum usizesource slice length () does not match destination slice length (
-incomplete utf-8 byte sequence from index invalid utf-8 sequence of  bytes from index invalid utf-8: corrupt contentsattempted to index str up to maximum usizelibrary/core/src/str/pattern.rslibrary/core/src/str/lossy.rs\x[...]byte index  is out of bounds of `begin <= end ( is not a char boundary; it is inside ) of `library/core/src/str/mod.rslibrary/core/src/time.rssms
-sns18446744073709551616library/core/src/unicode/printable.rs
-)147:;=IJ]
-)14:;EFIJ^de
-):;EIW[\^_de
-FGNOXZ\^~
-)14:EFIJNOde\
- #%&(38:HJLPSUVXZ\^`cefksx}
-library/core/src/unicode/unicode_data.rslibrary/core/src/num/bignum.rsassertion failed: noborrowassertion failed: digits < 40assertion failed: other > 0
-7Cxl2i5n
-WEmptyTryFromIntErrorParseIntErrorNegOverflowPosOverflowInvalidDigitTryFromSliceErrorErrorUtf8Errorvalid_up_toerror_len
-LayoutalignLayoutError
-GCC: (GNU) 10.2.1 20210130 (Red Hat 10.2.1-11)
-GCC: (crosstool-NG UNKNOWN) 8.3.0
-GCC: (GNU) 4.8.5 20150623 (Red Hat 4.8.5-44)
-.shstrtab
-.note.gnu.build-id
-.gnu.hash
-.gnu.version
-.gnu.version_r
-.rela.dyn
-.rela.plt
-.eh_frame_hdr
-.eh_frame
-.gcc_except_table
-.init_array
-.fini_array
-.data.rel.ro
-.dynamic
-.comment
+unable to delete/modify collation sequence due to active statements
+ATOMIC_INTRINSICS=1
+COMPILER=clang-14.0.3
+DEFAULT_AUTOVACUUM
+DEFAULT_CACHE_SIZE=-2000
+DEFAULT_FILE_FORMAT=4
+DEFAULT_FOREIGN_KEYS
+DEFAULT_JOURNAL_SIZE_LIMIT=-1
+DEFAULT_MMAP_SIZE=0
+DEFAULT_PAGE_SIZE=4096
+DEFAULT_PCACHE_INITSZ=20
+DEFAULT_RECURSIVE_TRIGGERS
+DEFAULT_SECTOR_SIZE=4096
+DEFAULT_SYNCHRONOUS=2
+DEFAULT_WAL_AUTOCHECKPOINT=1000
+DEFAULT_WAL_SYNCHRONOUS=2
+DEFAULT_WORKER_THREADS=0
+ENABLE_API_ARMOR
+ENABLE_COLUMN_METADATA
+ENABLE_DBSTAT_VTAB
+ENABLE_FTS3
+ENABLE_FTS3_PARENTHESIS
+ENABLE_FTS5
+ENABLE_LOAD_EXTENSION
+ENABLE_MEMORY_MANAGEMENT
+ENABLE_RTREE
+ENABLE_STAT4
+HAVE_ISNAN
+MALLOC_SOFT_LIMIT=1024
+MAX_ATTACHED=10
+MAX_COLUMN=2000
+MAX_COMPOUND_SELECT=500
+MAX_DEFAULT_PAGE_SIZE=8192
+MAX_EXPR_DEPTH=1000
+MAX_FUNCTION_ARG=127
+MAX_LENGTH=1000000000
+MAX_LIKE_PATTERN_LENGTH=50000
+MAX_MMAP_SIZE=0x7fff0000
+MAX_PAGE_COUNT=1073741823
+MAX_PAGE_SIZE=65536
+MAX_SQL_LENGTH=1000000000
+MAX_TRIGGER_DEPTH=1000
+MAX_VARIABLE_NUMBER=32766
+MAX_VDBE_OP=250000000
+MAX_WORKER_THREADS=8
+MUTEX_PTHREADS
+SYSTEM_MALLOC
+TEMP_STORE=1
+THREADSAFE=1
+SBTBRBRBRBRBp
+TBTBRBRBRBRBRBRAp
+RBRBRBRBRBRB
+RBRBRBRBRBRA
+RBRBRBRAp
+RBRBRBRA
+RBRBRBRB
+RBRBRBRBRBRBRBRAp
+RBRBRBRA
+RBRBRBRBRA
+RBRBRBRBRAp
+RBRBRBRBRAp
+RBXBRBRBp
+RBRBRBRBRBRBRBRBRBRBRBRBRB`UB`
+RBRBYBRBYBRBYBRBYBRBYBRB`
+RBRBRBRBRAp
+RBYBXBYAp
+RBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRA
+RBRBRBRBRBRBRBRBRA
+RBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRB
+RBRBRBRBRB
+RBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRBRA
+RBRBRBRBRBRBRBRBRBRBRBp
+UBRBRBRBRBRBRBSBTB
+SFSCSCVBRB
+RBRBSARARATBTCSB
+SASASASA
+RBWARARARAp
+RBWARARAWBRB
+RMRMRMVBRB
+SBTBRBYBTBp
+RBRBRBRBRBRBRBRBRB
+RBRBRBRBRB
+TBTBTBRBRAp
+RBYBRBYBSBTBRBRBRB
+RBRBRBRBRBRBp
+TBRBRBRBRBRBRBRB
+RBYBRBYB
+RBYBRBYBRBYB
+RBRBRBRBRBRBRBRBRBRBRBRBRBRBSBp
+A\AUA\AUA\AUA\AUA\AUA\AUAXAp
+`xA`lA`CA`
+C]A]AUAp
+AUB\K`(AUBUAXA\L`"A`#A\K`ABRBRB
+RBRBRBRBp
+RBYBRBYBRBYB
+RBYBRBYBTBTBTA
+RBYBRBYA
+RBYBRBRB
+RBYBRBYA
+RBRBRBRBRBRBRBRBRBRBRBZB
+RBYBRBYBRBYBRBYBRBYBp
+TBRBRBRBp
+RBRBRBRBRBRBRBYBp
+RBYBRBYBp
+RBRBRBRBYAp
+RBRBRBRBRBRBRBRBRBp
+RBRBRBRBRBp
+RBYBRBRBRBRBRBRBYBp
+RBRBRBRBRBRBRBRBRBYBRBYBRBYBRBRBp
+RBRBYBRBYBRBYBTA
+RBSBRBRBRBRB
+RBRBRBRBRBRA
+TBRBSBRBRBp
+RBYBTBTBTBTBTBp
+RBRBRBRBRBRB
+RBRBRBRAp
+RBRBSBSAp
+RBRBRBRB
+TBRBRBRAp
+RBRBRBRB
+RBRBRBRBp
+p@p SAp p
+p@p SAp p
+p UDUDUDUDUDUDUBp
+SAWMSAWNp
+p UDUDUDUDUDUDUDUDUDUDUDUDUDUDUDp
+>@_PyBool_Type
+@_PyExc_AttributeError
+@_PyExc_BaseException
+@_PyExc_ImportError
+@_PyExc_OverflowError
+@_PyExc_SystemError
+@_PyExc_TypeError
+@_PyExc_ValueError
+@_PyUnicode_Type
+@__Py_NoneStruct
+@__Py_TrueStruct
+@_kSecRandomDefault
+@___stack_chk_guard
+@___stderrp
+@__tlv_bootstrap
+@_access
+@_fchmod
+@_fchown
+@_ftruncate
+@_getcwd
+@_geteuid
+@_munmap
+@_pwrite
+@_readlink
+@_unlink
+@dyld_stub_binder
+@_CFArrayGetCount
+@_CFArrayGetValueAtIndex
+@_CFRelease
+@_CFRetain
+@_CFStringGetBytes
+@_CFStringGetCStringPtr
+@_CFStringGetLength
+r8>@_PyBytes_AsString
+r@>@_PyBytes_Size
+rH>@_PyCMethod_New
+rP>@_PyErr_CheckSignals
+rX>@_PyErr_Fetch
+r`>@_PyErr_GivenExceptionMatches
+rh>@_PyErr_NewExceptionWithDoc
+rp>@_PyErr_NormalizeException
+rx>@_PyErr_Print
+>@_PyErr_PrintEx
+>@_PyErr_Restore
+>@_PyException_GetCause
+>@_PyException_SetCause
+>@_PyFloat_AsDouble
+>@_PyFloat_FromDouble
+>@_PyGILState_Ensure
+>@_PyGILState_Release
+>@_PyIter_Next
+>@_PyList_Append
+>@_PyList_New
+>@_PyLong_AsLong
+>@_PyLong_AsUnsignedLongLong
+>@_PyLong_FromLong
+>@_PyLong_FromUnsignedLongLong
+>@_PyModule_Create2
+>@_PyModule_GetName
+>@_PyNumber_Index
+>@_PyObject_GetAttr
+>@_PyObject_GetIter
+>@_PyObject_IsInstance
+>@_PyObject_Repr
+>@_PyObject_SetAttr
+>@_PyObject_Str
+>@_PySequence_Check
+>@_PySequence_Size
+>@_PyTuple_New
+>@_PyTuple_SetItem
+>@_PyUnicode_AsEncodedString
+>@_PyUnicode_AsUTF8AndSize
+>@_PyUnicode_FromStringAndSize
+>@_PyUnicode_InternInPlace
+>@_Py_IsInitialized
+@_SCNetworkInterfaceCopyAll
+@_SCNetworkInterfaceGetBSDName
+@_SCNetworkInterfaceGetInterfaceType
+@_SecRandomCopyBytes
+>@__Py_Dealloc
+@__Unwind_Backtrace
+@__Unwind_DeleteException
+@__Unwind_GetDataRelBase
+@__Unwind_GetIP
+@__Unwind_GetIPInfo
+@__Unwind_GetLanguageSpecificData
+@__Unwind_GetRegionStart
+@__Unwind_GetTextRelBase
+@__Unwind_RaiseException
+@__Unwind_Resume
+@__Unwind_SetGR
+@__Unwind_SetIP
+@___error
+@___memcpy_chk
+@___memset_chk
+@___stack_chk_fail
+@___strlcat_chk
+@___strlcpy_chk
+@__dyld_get_image_header
+@__dyld_get_image_name
+@__dyld_get_image_vmaddr_slide
+@__dyld_image_count
+@__tlv_atexit
+@_accept
+@_calloc
+@_clock_gettime
+@_closedir
+@_confstr
+@_connect
+@_dispatch_release
+@_dispatch_semaphore_create
+@_dispatch_semaphore_signal
+@_dispatch_semaphore_wait
+@_dlclose
+@_dlerror
+@_dlopen
+@_fprintf
+@_freeaddrinfo
+@_freeifaddrs
+@_fstatfs
+@_futimes
+@_gai_strerror
+@_getaddrinfo
+@_getcwd
+@_getenv
+@_gethostuuid
+@_getifaddrs
+@_getpeername
+@_getpid
+@_getsockname
+@_getsockopt
+@_gettimeofday
+@_if_nametoindex
+@_kevent
+@_kqueue
+@_listen
+@_localtime_r
+@_malloc
+@_malloc_create_zone
+@_malloc_default_zone
+@_malloc_set_zone_name
+@_malloc_size
+@_malloc_zone_free
+@_malloc_zone_malloc
+@_malloc_zone_realloc
+@_memchr
+@_memcmp
+@_memcpy
+@_memmove
+@_memset
+@_mprotect
+@_munmap
+@_nanosleep
+@_opendir
+@_posix_memalign
+@_pselect
+@_pthread_atfork
+@_pthread_attr_destroy
+@_pthread_attr_init
+@_pthread_attr_setstacksize
+@_pthread_cond_broadcast
+@_pthread_cond_destroy
+@_pthread_cond_signal
+@_pthread_cond_timedwait
+@_pthread_cond_wait
+@_pthread_create
+@_pthread_detach
+@_pthread_get_stackaddr_np
+@_pthread_get_stacksize_np
+@_pthread_join
+@_pthread_mutex_destroy
+@_pthread_mutex_init
+@_pthread_mutex_lock
+@_pthread_mutex_trylock
+@_pthread_mutex_unlock
+@_pthread_mutexattr_destroy
+@_pthread_mutexattr_init
+@_pthread_mutexattr_settype
+@_pthread_rwlock_destroy
+@_pthread_rwlock_rdlock
+@_pthread_rwlock_unlock
+@_pthread_rwlock_wrlock
+@_pthread_self
+@_pthread_setname_np
+@_random
+@_readdir_r
+@_realloc
+@_recvfrom
+@_rename
+@_sched_yield
+@_sendto
+@_setsockopt
+@_shutdown
+@_sigaltstack
+@_socket
+@_srandomdev
+@_statfs
+@_strcmp
+@_strcspn
+@_strerror_r
+@_strlcpy
+@_strlen
+@_strncmp
+@_strrchr
+@_sysconf
+@_sysctlbyname
+@_usleep
+@_utimes
+@_writev
+GFp_armcap_P
+PyInit_aisdb
+$    X,d
+xxxx|x|txx
+,@<@@<@@<<<<<<H|<<<,T@
+DDDDDLPPtx
+_GFp_armcap_P
+_PyInit_aisdb
+_CFArrayGetCount
+_CFArrayGetValueAtIndex
+_CFRelease
+_CFRetain
+_CFStringGetBytes
+_CFStringGetCStringPtr
+_CFStringGetLength
+_PyBool_Type
+_PyBytes_AsString
+_PyBytes_Size
+_PyCMethod_New
+_PyErr_CheckSignals
+_PyErr_Fetch
+_PyErr_GivenExceptionMatches
+_PyErr_NewExceptionWithDoc
+_PyErr_NormalizeException
+_PyErr_Print
+_PyErr_PrintEx
+_PyErr_Restore
+_PyExc_AttributeError
+_PyExc_BaseException
+_PyExc_ImportError
+_PyExc_OverflowError
+_PyExc_SystemError
+_PyExc_TypeError
+_PyExc_ValueError
+_PyException_GetCause
+_PyException_SetCause
+_PyFloat_AsDouble
+_PyFloat_FromDouble
+_PyGILState_Ensure
+_PyGILState_Release
+_PyIter_Next
+_PyList_Append
+_PyList_New
+_PyLong_AsLong
+_PyLong_AsUnsignedLongLong
+_PyLong_FromLong
+_PyLong_FromUnsignedLongLong
+_PyModule_Create2
+_PyModule_GetName
+_PyNumber_Index
+_PyObject_GetAttr
+_PyObject_GetIter
+_PyObject_IsInstance
+_PyObject_Repr
+_PyObject_SetAttr
+_PyObject_Str
+_PySequence_Check
+_PySequence_Size
+_PyTuple_New
+_PyTuple_SetItem
+_PyUnicode_AsEncodedString
+_PyUnicode_AsUTF8AndSize
+_PyUnicode_FromStringAndSize
+_PyUnicode_InternInPlace
+_PyUnicode_Type
+_Py_IsInitialized
+_SCNetworkInterfaceCopyAll
+_SCNetworkInterfaceGetBSDName
+_SCNetworkInterfaceGetInterfaceType
+_SecRandomCopyBytes
+__Py_Dealloc
+__Py_NoneStruct
+__Py_TrueStruct
+__Unwind_Backtrace
+__Unwind_DeleteException
+__Unwind_GetDataRelBase
+__Unwind_GetIP
+__Unwind_GetIPInfo
+__Unwind_GetLanguageSpecificData
+__Unwind_GetRegionStart
+__Unwind_GetTextRelBase
+__Unwind_RaiseException
+__Unwind_Resume
+__Unwind_SetGR
+__Unwind_SetIP
+___error
+___memcpy_chk
+___memset_chk
+___stack_chk_fail
+___stack_chk_guard
+___stderrp
+___strlcat_chk
+___strlcpy_chk
+__dyld_get_image_header
+__dyld_get_image_name
+__dyld_get_image_vmaddr_slide
+__dyld_image_count
+__tlv_atexit
+__tlv_bootstrap
+_clock_gettime
+_closedir
+_confstr
+_connect
+_dispatch_release
+_dispatch_semaphore_create
+_dispatch_semaphore_signal
+_dispatch_semaphore_wait
+_dlclose
+_dlerror
+_fprintf
+_freeaddrinfo
+_freeifaddrs
+_fstatfs
+_ftruncate
+_futimes
+_gai_strerror
+_getaddrinfo
+_geteuid
+_gethostuuid
+_getifaddrs
+_getpeername
+_getsockname
+_getsockopt
+_gettimeofday
+_if_nametoindex
+_kSecRandomDefault
+_localtime_r
+_malloc_create_zone
+_malloc_default_zone
+_malloc_set_zone_name
+_malloc_size
+_malloc_zone_free
+_malloc_zone_malloc
+_malloc_zone_realloc
+_memmove
+_mprotect
+_nanosleep
+_opendir
+_posix_memalign
+_pselect
+_pthread_atfork
+_pthread_attr_destroy
+_pthread_attr_init
+_pthread_attr_setstacksize
+_pthread_cond_broadcast
+_pthread_cond_destroy
+_pthread_cond_signal
+_pthread_cond_timedwait
+_pthread_cond_wait
+_pthread_create
+_pthread_detach
+_pthread_get_stackaddr_np
+_pthread_get_stacksize_np
+_pthread_join
+_pthread_mutex_destroy
+_pthread_mutex_init
+_pthread_mutex_lock
+_pthread_mutex_trylock
+_pthread_mutex_unlock
+_pthread_mutexattr_destroy
+_pthread_mutexattr_init
+_pthread_mutexattr_settype
+_pthread_rwlock_destroy
+_pthread_rwlock_rdlock
+_pthread_rwlock_unlock
+_pthread_rwlock_wrlock
+_pthread_self
+_pthread_setname_np
+_readdir_r
+_readlink
+_realloc
+_recvfrom
+_sched_yield
+_setsockopt
+_shutdown
+_sigaltstack
+_srandomdev
+_strcspn
+_strerror_r
+_strlcpy
+_strncmp
+_strrchr
+_sysconf
+_sysctlbyname
+dyld_stub_binder
+aisdb.cpython-39-darwin.so
+>#Zir?O`
+]prC9*:y?
+3j	">e*D
+ZXD}_^2T
+m1[bv-<]]@
+d9B*&Eq&Lc
```

## Comparing `aisdb-1.6.4.dist-info/RECORD` & `aisdb-1.6.5.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-aisdb-1.6.4.dist-info/METADATA,sha256=sIke8kFDJyPIPiDxzdhnKZPTHz_lsugmF_OWS99AKkA,4949
-aisdb-1.6.4.dist-info/WHEEL,sha256=hohAQhx-IlxsGxpxdWKbHeBIU8tVv0m1QVyIZstromA,129
-aisdb/__init__.py,sha256=cUCgLOVpgddH6wOO48p9vcVDAbf05i9BOlbFsoJo0zE,1605
-aisdb/aisdb_sql/coarsetype.sql,sha256=WdpuCzyY8DkrxbBw6--SD4V9Ui0sh1dkfg67d-2uEnQ,4924
-aisdb/aisdb_sql/createtable_dynamic_clustered.sql,sha256=q02bPdAhnjKvYG6nx550wMFv0i9jynA_FtY5kO4lV48,358
-aisdb/aisdb_sql/createtable_griddata.sql,sha256=GD2xarR0qeJMC_ISL3DQgAPLSLttmU2jEfczd7gEvcc,108
-aisdb/aisdb_sql/createtable_static.sql,sha256=vNd5LIQvnDIf5--rsXFGMV4KDYwPS4_Df2ZvI_FaoMo,539
-aisdb/aisdb_sql/createtable_static_aggregate.sql,sha256=acov9GgYft8PwmfZV0T-SXe71cc4LOBS6H31Ot35Y-U,258
-aisdb/aisdb_sql/createtable_webdata_marinetraffic.sql,sha256=CzTkJudERK1O2JIsFZvlLKvg5Wlfm-mO1WMTLjpQtq0,369
-aisdb/aisdb_sql/cte_aliases.sql,sha256=99vjXG1Cnnvp20DVmBygXTNFBol18xTZKx5VZMAmLjg,43
-aisdb/aisdb_sql/cte_coarsetype.sql,sha256=B1Z-FMBZg-RrOiUHdIOKIKwve73PT7DhIT641eZdDlo,91
-aisdb/aisdb_sql/cte_dynamic_clusteredidx.sql,sha256=tMFikmWgwujGiAA8o9MixS2qaIFwEbiL3U2dZmnmGwg,125
-aisdb/aisdb_sql/cte_static.sql,sha256=SyvlE4Wjbc0OdiVY7d5UaJL5HPZ5TReueh1u67qBesI,185
-aisdb/aisdb_sql/cte_static_aggregate.sql,sha256=JmGGcFMpykL46myHGX7trYYfwIkh5p9FUzEN18wai0M,210
-aisdb/aisdb_sql/insert_dynamic_clusteredidx.sql,sha256=kQH1TZP8nejbVeffWu1fjKP681IKbzpv51ypLDJpBrM,230
-aisdb/aisdb_sql/insert_static.sql,sha256=3G9yNPbaIrMolwraLxng1Hoe8GDle4IEB2hGdEfD6v8,400
-aisdb/aisdb_sql/insert_webdata_marinetraffic.sql,sha256=UkzuriXqOvo7yuElM4vQcGFpqGOeFruFrXquzE6wzME,763
-aisdb/aisdb_sql/select_columns_static.sql,sha256=LvMFWE2nFh6wI38sFIwLLRC4g0N3IeaSW9_kfgHDXv4,312
-aisdb/aisdb_sql/select_join_dynamic_static_clusteredidx.sql,sha256=U99iGgVgZKG2a4BvZOgFUgJDxLbAJCipvmop__TH05g,493
-aisdb/aisdb_sql/select_merged_all.sql,sha256=Hzc-POgmUf3pBTswjKUfU51mhX_6u29K-xYFiDJqiwc,881
-aisdb/aisdb_sql/select_static_join_webdata.sql,sha256=jpDQ9LhbN-r-shmtXfcvy1UwkdSTSEFMmUeJFE-e_vY,658
+aisdb-1.6.5.dist-info/METADATA,sha256=q6rnwPbte99tznPy3VMAYtY151fVf-pt52-Z2TzC-qs,4949
+aisdb-1.6.5.dist-info/WHEEL,sha256=cERpwH07uNU-oSFnr3JrGcE8PTsymFPyUNeYOEo-RFw,102
+aisdb/database/decoder.py,sha256=P2MUSqPatVZbV5BZepvZaKcitysvqXs7jPxfktaGFIM,9816
+aisdb/database/sqlfcn_callbacks.py,sha256=H9DRSbAb-2W0Gzx19D19GVhloO8PR9ajE34_YORjk60,1739
 aisdb/database/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+aisdb/database/dbqry.py,sha256=kgKE4GAs_ovrw2E-dCzsDyVcum43_NS9ZE1RCrT5Zj4,11962
 aisdb/database/create_tables.py,sha256=JPgTk4-8fE4ZenOOb9lJb1k0c8O2wtueavL1IGxfDhQ,4900
 aisdb/database/dbconn.py,sha256=NfafD7kwYiyUSN2BmZM1ch9scBNejpI2Y6QFJBiKXiI,6358
-aisdb/database/dbqry.py,sha256=kgKE4GAs_ovrw2E-dCzsDyVcum43_NS9ZE1RCrT5Zj4,11962
-aisdb/database/decoder.py,sha256=P2MUSqPatVZbV5BZepvZaKcitysvqXs7jPxfktaGFIM,9816
-aisdb/database/sql_query_strings.py,sha256=QXrMGHy04Hwl141_2fYe5FtCWcMRZiScB_87RIcgu9Q,4170
 aisdb/database/sqlfcn.py,sha256=tns7PNlkucQA69ero8qE1UZ9xJ2cSqOGQ93zJzDR0T8,3188
-aisdb/database/sqlfcn_callbacks.py,sha256=H9DRSbAb-2W0Gzx19D19GVhloO8PR9ajE34_YORjk60,1739
-aisdb/denoising_encoder.py,sha256=qOUaLRxZQrIWVXB2DIhAuI0ApuSSGH2i7JiD_6CEpSw,7783
-aisdb/gis.py,sha256=1wzEcPKniFE22rlCDN3nLBNIbLeLcCXLVxYC8DrG8lU,18568
-aisdb/interp.py,sha256=oniRtFCvpbN3h92NH7hJsSvgnrkavlmhejJuo4oS8vQ,1599
+aisdb/database/sql_query_strings.py,sha256=QXrMGHy04Hwl141_2fYe5FtCWcMRZiScB_87RIcgu9Q,4170
+aisdb/track_gen.py,sha256=CSZxYv_cX_w2pyxusTcpLUl09EAyMFEw0KDJ3Rrh7Ok,7650
+aisdb/webdata/_scraper.py,sha256=74I-pckc_SyiZSgR7S9DFCSMswJbYJrizCoM614s-VY,2505
+aisdb/webdata/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+aisdb/webdata/load_raster.py,sha256=uYMMGTsK1Ey82MKwGZruzlQw-OulBDbU7DrYW8a8Gm0,2448
+aisdb/webdata/marinetraffic.py,sha256=jHFZh1vLvr9mC-CbxjN7SmmchgKJZKQc4bEo7s4uf30,11002
+aisdb/webdata/bathymetry.py,sha256=T1sw1Q41vZmMHUBHWfz32EY5zhIi0I3R9DQxueQFkK0,5440
+aisdb/webdata/shore_dist.py,sha256=ZJ7CoPnnCM7vsnqSC1DeYfeAjAXmOn10G5X-SXXicwQ,2690
 aisdb/network_graph.py,sha256=Gm8oMtmzb28leaOZfaoSCATyfrXcMF5SQ5OGKiNEfTY,18893
-aisdb/proc_util.py,sha256=Wgcql2gD6dgW4iYuyx4MCDAmXMU8uWil0o2eTqRyPIU,8060
-aisdb/receiver.py,sha256=GI0MlFR9atRb9W3qtod-2anaHjXBkf9hN_DYA9ViFsU,2470
-aisdb/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-aisdb/tests/create_testing_data.py,sha256=nk1Ry_D0hzfpfDfoDFksm2IBKWPJSuPdT8jWjrMdqt0,3139
-aisdb/tests/test_00_decode.py,sha256=_KJqPFMnaypDDmLYY4fBSOU7FgNgLWbsrFvbE1JkYcs,1420
+aisdb/tests/testdata/test_data_20211101.nm4.gz,sha256=wzIRA3otVkC5XZair_fD4vzWu3DUYZT-mnQ6qkPp0gI,23613
+aisdb/tests/testdata/test_data_20211101.nm4,sha256=khnnrunY_ZCPYEYWCgK-vMsoPC3FOG0w52rbx-FHj6o,84630
 aisdb/tests/test_01_createtables.py,sha256=3s5qtrX4Up8bx_7j8PGmreUDaItqVUErqzhbFTpqatw,2738
+aisdb/tests/test_00_decode.py,sha256=_KJqPFMnaypDDmLYY4fBSOU7FgNgLWbsrFvbE1JkYcs,1420
 aisdb/tests/test_02_dbqry.py,sha256=-1x_ubB2rOKjyzWE6sfgHWcYQxzXIoPfiZ3-N7D8EyM,2803
-aisdb/tests/test_02_sqlfcn.py,sha256=CbAcHDOBcRWE7yz-P-ftkDNh1Al0x5a0K9fqAnfdMCg,2956
-aisdb/tests/test_03_gis.py,sha256=ttvp7Kh03Wuc1271Bn52Tu_rYQGXaSaOg44B8BZigYY,2956
-aisdb/tests/test_04_trackgen.py,sha256=t7fKiRh8fL2D29eeGHNPsorgEAI-Bm4eZPUnu_wN5jw,2332
-aisdb/tests/test_05_proc_util.py,sha256=x2Cj0fZiyUDUNXWuTbkCQRazvMZRY8ybSYLOSaAwLKg,4385
-aisdb/tests/test_06_interp.py,sha256=bE39lHY7EKPHrPgORit7tZUdPRnOIKsTin_-B63Y2bA,1090
-aisdb/tests/test_07_bathymetry.py,sha256=BE6yvl6pgStj7vXG_9raMVdNGKD4LaXop8PJs6rSd8o,1256
-aisdb/tests/test_07_shore_dist.py,sha256=dw9iDbDC8WbpGnUeJwzMNoau97tryVYZPe1ue2scvfI,1131
 aisdb/tests/test_08_marinetraffic.py,sha256=rDkmOQM8SARSxf89T6sRxFpT_1gJvDDTomBe9pE07bc,2580
+aisdb/tests/test_07_shore_dist.py,sha256=dw9iDbDC8WbpGnUeJwzMNoau97tryVYZPe1ue2scvfI,1131
+aisdb/tests/test_07_bathymetry.py,sha256=BE6yvl6pgStj7vXG_9raMVdNGKD4LaXop8PJs6rSd8o,1256
+aisdb/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 aisdb/tests/test_08_wsa.py,sha256=SqwNAAhRlcKsVyVIZDrFDhOIFrth6mqzjVr-yQbRrvs,1679
-aisdb/tests/test_09_network_graph.py,sha256=oAUOqoRMAPpxoO6Q-Pln240dBm-a7HRa2mF9rc9tvo4,3596
+aisdb/tests/test_04_trackgen.py,sha256=t7fKiRh8fL2D29eeGHNPsorgEAI-Bm4eZPUnu_wN5jw,2332
+aisdb/tests/test_06_interp.py,sha256=bE39lHY7EKPHrPgORit7tZUdPRnOIKsTin_-B63Y2bA,1090
+aisdb/tests/test_05_proc_util.py,sha256=x2Cj0fZiyUDUNXWuTbkCQRazvMZRY8ybSYLOSaAwLKg,4385
+aisdb/tests/test_03_gis.py,sha256=ttvp7Kh03Wuc1271Bn52Tu_rYQGXaSaOg44B8BZigYY,2956
 aisdb/tests/test_11_postgres.py,sha256=_UMAJtat8YEIIR-NQbOH_DlFfsevw_kT1IrQo_dh_8M,778
+aisdb/tests/create_testing_data.py,sha256=nk1Ry_D0hzfpfDfoDFksm2IBKWPJSuPdT8jWjrMdqt0,3139
+aisdb/tests/test_09_network_graph.py,sha256=oAUOqoRMAPpxoO6Q-Pln240dBm-a7HRa2mF9rc9tvo4,3596
 aisdb/tests/test_rx.py,sha256=Gh6y85fv6O-CZlHouwNHAjVVVce4lXwgL2PQNJjcIKo,74
-aisdb/tests/testdata/test_data_20211101.nm4,sha256=khnnrunY_ZCPYEYWCgK-vMsoPC3FOG0w52rbx-FHj6o,84630
-aisdb/tests/testdata/test_data_20211101.nm4.gz,sha256=wzIRA3otVkC5XZair_fD4vzWu3DUYZT-mnQ6qkPp0gI,23613
-aisdb/track_gen.py,sha256=CSZxYv_cX_w2pyxusTcpLUl09EAyMFEw0KDJ3Rrh7Ok,7650
-aisdb/web_interface.py,sha256=XQ3M9nzQIVpFrCsL6c5UEjdRinqSFphaF63di-Jz49Y,6994
-aisdb/webdata/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-aisdb/webdata/_scraper.py,sha256=74I-pckc_SyiZSgR7S9DFCSMswJbYJrizCoM614s-VY,2505
-aisdb/webdata/bathymetry.py,sha256=T1sw1Q41vZmMHUBHWfz32EY5zhIi0I3R9DQxueQFkK0,5440
-aisdb/webdata/load_raster.py,sha256=uYMMGTsK1Ey82MKwGZruzlQw-OulBDbU7DrYW8a8Gm0,2448
-aisdb/webdata/marinetraffic.py,sha256=jHFZh1vLvr9mC-CbxjN7SmmchgKJZKQc4bEo7s4uf30,11002
-aisdb/webdata/shore_dist.py,sha256=ZJ7CoPnnCM7vsnqSC1DeYfeAjAXmOn10G5X-SXXicwQ,2690
+aisdb/tests/test_02_sqlfcn.py,sha256=CbAcHDOBcRWE7yz-P-ftkDNh1Al0x5a0K9fqAnfdMCg,2956
+aisdb/receiver.py,sha256=GI0MlFR9atRb9W3qtod-2anaHjXBkf9hN_DYA9ViFsU,2470
+aisdb/__init__.py,sha256=cUCgLOVpgddH6wOO48p9vcVDAbf05i9BOlbFsoJo0zE,1605
+aisdb/denoising_encoder.py,sha256=qOUaLRxZQrIWVXB2DIhAuI0ApuSSGH2i7JiD_6CEpSw,7783
+aisdb/aisdb_sql/createtable_webdata_marinetraffic.sql,sha256=CzTkJudERK1O2JIsFZvlLKvg5Wlfm-mO1WMTLjpQtq0,369
+aisdb/aisdb_sql/createtable_static_aggregate.sql,sha256=acov9GgYft8PwmfZV0T-SXe71cc4LOBS6H31Ot35Y-U,258
+aisdb/aisdb_sql/insert_webdata_marinetraffic.sql,sha256=UkzuriXqOvo7yuElM4vQcGFpqGOeFruFrXquzE6wzME,763
+aisdb/aisdb_sql/cte_dynamic_clusteredidx.sql,sha256=tMFikmWgwujGiAA8o9MixS2qaIFwEbiL3U2dZmnmGwg,125
+aisdb/aisdb_sql/createtable_griddata.sql,sha256=GD2xarR0qeJMC_ISL3DQgAPLSLttmU2jEfczd7gEvcc,108
+aisdb/aisdb_sql/coarsetype.sql,sha256=WdpuCzyY8DkrxbBw6--SD4V9Ui0sh1dkfg67d-2uEnQ,4924
+aisdb/aisdb_sql/select_merged_all.sql,sha256=Hzc-POgmUf3pBTswjKUfU51mhX_6u29K-xYFiDJqiwc,881
+aisdb/aisdb_sql/cte_coarsetype.sql,sha256=B1Z-FMBZg-RrOiUHdIOKIKwve73PT7DhIT641eZdDlo,91
+aisdb/aisdb_sql/cte_static.sql,sha256=SyvlE4Wjbc0OdiVY7d5UaJL5HPZ5TReueh1u67qBesI,185
+aisdb/aisdb_sql/createtable_static.sql,sha256=vNd5LIQvnDIf5--rsXFGMV4KDYwPS4_Df2ZvI_FaoMo,539
+aisdb/aisdb_sql/cte_static_aggregate.sql,sha256=JmGGcFMpykL46myHGX7trYYfwIkh5p9FUzEN18wai0M,210
+aisdb/aisdb_sql/select_join_dynamic_static_clusteredidx.sql,sha256=U99iGgVgZKG2a4BvZOgFUgJDxLbAJCipvmop__TH05g,493
+aisdb/aisdb_sql/insert_static.sql,sha256=3G9yNPbaIrMolwraLxng1Hoe8GDle4IEB2hGdEfD6v8,400
+aisdb/aisdb_sql/select_static_join_webdata.sql,sha256=jpDQ9LhbN-r-shmtXfcvy1UwkdSTSEFMmUeJFE-e_vY,658
+aisdb/aisdb_sql/select_columns_static.sql,sha256=LvMFWE2nFh6wI38sFIwLLRC4g0N3IeaSW9_kfgHDXv4,312
+aisdb/aisdb_sql/insert_dynamic_clusteredidx.sql,sha256=kQH1TZP8nejbVeffWu1fjKP681IKbzpv51ypLDJpBrM,230
+aisdb/aisdb_sql/createtable_dynamic_clustered.sql,sha256=q02bPdAhnjKvYG6nx550wMFv0i9jynA_FtY5kO4lV48,358
+aisdb/aisdb_sql/cte_aliases.sql,sha256=99vjXG1Cnnvp20DVmBygXTNFBol18xTZKx5VZMAmLjg,43
+aisdb/proc_util.py,sha256=Wgcql2gD6dgW4iYuyx4MCDAmXMU8uWil0o2eTqRyPIU,8060
+aisdb/web_interface.py,sha256=ssQyuqvfpU5BC7eFyRwPLE-RXhsjzyFH32ujyIg1aRM,7421
+aisdb/interp.py,sha256=oniRtFCvpbN3h92NH7hJsSvgnrkavlmhejJuo4oS8vQ,1599
+aisdb/gis.py,sha256=1wzEcPKniFE22rlCDN3nLBNIbLeLcCXLVxYC8DrG8lU,18568
 aisdb/wsa.py,sha256=rLhpGbEf3G60Ml30v4a3I4NoUFGOI_qdvk64wwiM3Hw,3845
 aisdb/__init__.py,sha256=cUCgLOVpgddH6wOO48p9vcVDAbf05i9BOlbFsoJo0zE,1605
 aisdb/denoising_encoder.py,sha256=qOUaLRxZQrIWVXB2DIhAuI0ApuSSGH2i7JiD_6CEpSw,7783
 aisdb/gis.py,sha256=1wzEcPKniFE22rlCDN3nLBNIbLeLcCXLVxYC8DrG8lU,18568
 aisdb/interp.py,sha256=oniRtFCvpbN3h92NH7hJsSvgnrkavlmhejJuo4oS8vQ,1599
 aisdb/network_graph.py,sha256=Gm8oMtmzb28leaOZfaoSCATyfrXcMF5SQ5OGKiNEfTY,18893
 aisdb/proc_util.py,sha256=Wgcql2gD6dgW4iYuyx4MCDAmXMU8uWil0o2eTqRyPIU,8060
 aisdb/receiver.py,sha256=GI0MlFR9atRb9W3qtod-2anaHjXBkf9hN_DYA9ViFsU,2470
 aisdb/track_gen.py,sha256=CSZxYv_cX_w2pyxusTcpLUl09EAyMFEw0KDJ3Rrh7Ok,7650
-aisdb/web_interface.py,sha256=XQ3M9nzQIVpFrCsL6c5UEjdRinqSFphaF63di-Jz49Y,6994
+aisdb/web_interface.py,sha256=ssQyuqvfpU5BC7eFyRwPLE-RXhsjzyFH32ujyIg1aRM,7421
 aisdb/wsa.py,sha256=rLhpGbEf3G60Ml30v4a3I4NoUFGOI_qdvk64wwiM3Hw,3845
 aisdb/aisdb_sql/coarsetype.sql,sha256=WdpuCzyY8DkrxbBw6--SD4V9Ui0sh1dkfg67d-2uEnQ,4924
 aisdb/aisdb_sql/createtable_dynamic_clustered.sql,sha256=q02bPdAhnjKvYG6nx550wMFv0i9jynA_FtY5kO4lV48,358
 aisdb/aisdb_sql/createtable_griddata.sql,sha256=GD2xarR0qeJMC_ISL3DQgAPLSLttmU2jEfczd7gEvcc,108
 aisdb/aisdb_sql/createtable_static.sql,sha256=vNd5LIQvnDIf5--rsXFGMV4KDYwPS4_Df2ZvI_FaoMo,539
 aisdb/aisdb_sql/createtable_static_aggregate.sql,sha256=acov9GgYft8PwmfZV0T-SXe71cc4LOBS6H31Ot35Y-U,258
 aisdb/aisdb_sql/createtable_webdata_marinetraffic.sql,sha256=CzTkJudERK1O2JIsFZvlLKvg5Wlfm-mO1WMTLjpQtq0,369
@@ -118,80 +118,118 @@
 aisdb/tests/testdata/test_data_20211101.nm4,sha256=khnnrunY_ZCPYEYWCgK-vMsoPC3FOG0w52rbx-FHj6o,84630
 aisdb/webdata/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 aisdb/webdata/_scraper.py,sha256=74I-pckc_SyiZSgR7S9DFCSMswJbYJrizCoM614s-VY,2505
 aisdb/webdata/bathymetry.py,sha256=T1sw1Q41vZmMHUBHWfz32EY5zhIi0I3R9DQxueQFkK0,5440
 aisdb/webdata/load_raster.py,sha256=uYMMGTsK1Ey82MKwGZruzlQw-OulBDbU7DrYW8a8Gm0,2448
 aisdb/webdata/marinetraffic.py,sha256=jHFZh1vLvr9mC-CbxjN7SmmchgKJZKQc4bEo7s4uf30,11002
 aisdb/webdata/shore_dist.py,sha256=ZJ7CoPnnCM7vsnqSC1DeYfeAjAXmOn10G5X-SXXicwQ,2690
-aisdb_lib/Cargo.lock,sha256=A1MWd4TwcGvdr1GhmeFnQdwEGEY0LCH2hFt8DxYJz_w,36655
-aisdb_lib/Cargo.toml,sha256=R4PJw4YzytpMk_5Zu7D6YBxASWaXELMTBMNcdpkGtx8,946
+aisdb_lib/Cargo.lock,sha256=_hn7ExZscAtnyY2NZPigEBAN0YBalhnEyCR3tscO4dg,32701
+aisdb_lib/Cargo.toml,sha256=eBAdg1ynfIRxzzUmmI1gBk4Y4dkn-2yFlCI1FqUgnck,946
 aisdb_lib/build.rs,sha256=O6Mps8rydIPRoUU4WVDtvfAwE_pnEw7LCZ69qQ6aqqI,135
 aisdb_web/dist_map/assets/OSM-18e3061c.js,sha256=bk5cwBk6o6869yj2wZA7vNmzlP1aa9m8Pjhk0wR9bgs,1672
 aisdb_web/dist_map/assets/OSM-3d3b8c7a.js,sha256=3VVVxC2ibWH4AStzrdKCjXnANbDgt2lJNAdNDKl5N64,1672
 aisdb_web/dist_map/assets/OSM-a7270865.js,sha256=rWSdH6eLV4A474bNt5XLjYr0RqcLhq42eDehxiY-9OU,1672
+aisdb_web/dist_map/assets/OSM-f12b1a18.js,sha256=ET2nYUaAtD0TJ9zWBL32KCviHkMac94LN4YDzoJRzOc,1672
+aisdb_web/dist_map/assets/OSM-fff71e55.js,sha256=3-KDCj-PTGMeihyeydUPiFRWtR0yZZOrAJFrnwrgAAU,1672
+aisdb_web/dist_map/assets/TileImage-809400bf.js,sha256=aLukhEb1zgEimGfJnECHdr8fYSupTQumuKnNPdxy2hE,17519
 aisdb_web/dist_map/assets/TileImage-865fdc14.js,sha256=xZQKNhOu9KQULmCXJGfG-pEz7BG3_NQqRUxXi4HCY7Q,17519
+aisdb_web/dist_map/assets/TileImage-b8366ddc.js,sha256=iSPv2HXqLrLzcDlB0HTdsodf0fUaxHmY8h60xmZye-s,17292
 aisdb_web/dist_map/assets/TileImage-e0a2bc65.js,sha256=AiFXgTd3PLeGLFEV5FbaJ0HixXJTFLpIJSXTTBe-LJk,17519
 aisdb_web/dist_map/assets/TileImage-e2e53f79.js,sha256=mq37YsITDee2Y3zk3JygqTqoFTXZYtV09R-6uJ7Neec,17519
 aisdb_web/dist_map/assets/client_bg-05f4a55d.wasm,sha256=BfSlXYmetRCJhJ25mYKD2SJjeXanVTFxS3vB4P1aPD8,173279
+aisdb_web/dist_map/assets/client_bg-505558bc.wasm,sha256=UFVYvEtet-ClTLqnQTrItg9HTQ1hDvOZC9DdfktTAfs,173403
 aisdb_web/dist_map/assets/client_bg-6a509824.wasm,sha256=alCYJEqrMJGqbbpRfZfdyW5XPxHpccXY9XVWfWPQHuA,173279
 aisdb_web/dist_map/assets/client_bg-916ba2c4.wasm,sha256=kWuixLQgou9Sh4krEh-UtrkbPxgLMaZZQB7c6tI_c0A,173278
+aisdb_web/dist_map/assets/constants-36dce06f.js,sha256=hAw7A1VNkUrUJ-T1jW4unoR0OW1lsoVglqxDDzbq6X8,760
 aisdb_web/dist_map/assets/constants-a418eeb2.js,sha256=6XpubRSknht1nMcdNjKV4THpi2DBAiVqydEWZ3ci518,723
 aisdb_web/dist_map/assets/index-f2c4f58e.css,sha256=8sT1jseE3LNxWJ_S05N816ALqs_E6ZceC8Hl0ElSGx8,8224
 aisdb_web/dist_map/assets/livestream-04f2da24.js,sha256=lAL4T275uII_bcNYuEUJ1P4jHXmQ7WQfWEGJr67zO_I,1185
 aisdb_web/dist_map/assets/livestream-7a84f2e5.js,sha256=tnuOsXaBk6nv8oZF9ibYuQYZlU0wfaLe9dTWrMDmE0s,1185
 aisdb_web/dist_map/assets/livestream-7c48cb34.js,sha256=RSo_p2wRWmQExozZZuaSNvk8Dn4St9ue0lkZ6Jj1Gig,1185
+aisdb_web/dist_map/assets/livestream-86d0ab65.js,sha256=AppB9IdTkYNBSa7HkpeHObaAULDtCkZdpgpnTWGqqgw,1185
+aisdb_web/dist_map/assets/livestream-87738d04.js,sha256=x9DZRqokqafLZaw_uZKvICWJUwdWXNfdfuEa6dQWV6A,1185
 aisdb_web/dist_map/assets/main-12a41ab2.js,sha256=GzdPc2BUIF4CgPDkjpEYvVsVQvsI6VOt8RNqBygJMDo,2662
+aisdb_web/dist_map/assets/main-4986f97e.js,sha256=8hBKEjUHSubbWYEFhIWXF8COXt_WKDLyh97GioL7onA,2662
+aisdb_web/dist_map/assets/main-4e7182f2.js,sha256=Rz5iN4aPnxfl_UaTsz55ERXP03djBRA69skDTPPZsIQ,2662
 aisdb_web/dist_map/assets/main-b42e8f3c.js,sha256=qHhSZnAdNc4-Zbziom5Jsl81uPNILTtcDet_P9ZXQ00,2662
 aisdb_web/dist_map/assets/main-c046974e.js,sha256=zCRXf7Fv1GwtME_1h6QWEdICtzqQtme9JAQd2MtQ-Vc,2662
 aisdb_web/dist_map/assets/map-0df0429f.js,sha256=9aRUG0KQ-4Cck8sjn2DCjZdmp8rvBH_tbzs9VpB5B70,405869
+aisdb_web/dist_map/assets/map-0f7724e3.js,sha256=inFJPaBTPEhubeh-_n8ZX-uxD-uNVIXCvIz9PAPlwPM,406688
+aisdb_web/dist_map/assets/map-8b360aef.js,sha256=_tHy8Z-eVtldKNM3mGlLsY7-frXAsZVR9U8rWQyl88A,405998
 aisdb_web/dist_map/assets/map-abddb635.js,sha256=Mjc0Q7En53LIGNprrFj8cX20O7LaM9AUycdOfFuTV0U,405869
 aisdb_web/dist_map/assets/map-b057f40e.js,sha256=fGoSKRoE9mfU4vi5fmaDKcflYp7Uaddy1kbNyyhpSaE,405869
 aisdb_web/dist_map/assets/map-c04ede37.css,sha256=wE7eN3fQO3muXiTjgPLskMQiWIF25PplqxbTZK63G_U,15782
+aisdb_web/dist_map/assets/proj-20c50701.js,sha256=NXGYVb1iMt49Bb2kvDvfkrrkSP38k7J3PzSDjAroY48,16617
 aisdb_web/dist_map/assets/proj-3e4e3ac0.js,sha256=CDa_OOHYJMO6jn34L2d31REY1OziTpippM_UC86frq4,16622
 aisdb_web/dist_map/assets/render-15f8910a.js,sha256=5GcEv8d14nN3ay9RHATHZX2VHQB_-KDkNnU_4kD_VAY,203253
 aisdb_web/dist_map/assets/render-29aaa5e2.js,sha256=oPZTQ-6RFgaigaBdgA-F44i6n3c75ASQTCjylVAJUPQ,203253
+aisdb_web/dist_map/assets/render-3e217d1c.js,sha256=NYm3V3PUDlAW2m6SoyPFlZJmbHfAJiKCv6cLtodep-8,203229
 aisdb_web/dist_map/assets/render-9978d19f.js,sha256=PfipRc2k0V9AaJxJIPIZPUZQAeObdchdL9ADIH6LP_k,203253
+aisdb_web/dist_map/assets/render-9ee6ddf6.js,sha256=YKpFglbtj0HE_Mhs6gNexg5FoNY4K6EMea6j5KwJ6Tk,203253
 aisdb_web/dist_map/assets/tileserver-24a57af3.js,sha256=bqnbceio2C8fRFNJ7-3IKrN2TfHdmefyoZjRL8B_nAo,3092
 aisdb_web/dist_map/assets/tileserver-8260d47b.js,sha256=X1KSz-HUv0w4i-NAOaACJcNDxTWQFkjDFt21KxLfdXk,3092
 aisdb_web/dist_map/assets/tileserver-b56401ad.js,sha256=VqqVM5VkY2HhICfICTkFdvX726_OlSG1zURqR9vP_dU,3092
+aisdb_web/dist_map/assets/tileserver-f7324a05.js,sha256=mNqnXw4ARJxN9Ojj_9xtZovesBfVyz94wcz3xqmsx4M,3092
+aisdb_web/dist_map/assets/tileserver-f89aaf92.js,sha256=UiN1Bet1CrE5YbMl7JbAXl1D3ekjbq5qotLL0fClxzM,3092
 aisdb_web/dist_map/assets/url-3f93404c.js,sha256=nQxq4asVrhziNAQtF8Fmq5jz_PjCjR7YEiWXXDZ0ReA,3114
 aisdb_web/dist_map/assets/url-7cac731b.js,sha256=3p5xQ-aNMmiPGfj8yVj5i3BtiXBIlnUJ04HIpP2iwaE,3114
+aisdb_web/dist_map/assets/url-89988760.js,sha256=uP17ApjV3y_MTSF2IGOMAlcvMi_C_jwR9SewqkQ6Uwo,3114
 aisdb_web/dist_map/assets/url-b43e4d73.js,sha256=vA40DSupDeVg2jYvaEMk4qZkAGVgqbcLz8VuM1qFSqQ,3114
+aisdb_web/dist_map/assets/url-daaf27e9.js,sha256=kpJ6nuhn7_lEEMQrr4RL7JbMZ8R1SFRHQNEKUy6cWT8,3114
 aisdb_web/dist_map/assets/vessel_metadata-52b84ad7.js,sha256=SIEmIe2mg9ElDgLUXFcYf3K4dnRLUpB3gIz6mR8jfX8,1203
 aisdb_web/dist_map/assets/vessel_metadata-a539ebc6.js,sha256=uH46frlTdZJANcvZBG0P-ppLxL_JKbGFsv9G65uCOIg,1203
+aisdb_web/dist_map/assets/vessel_metadata-b3364c5a.js,sha256=HCWuxLkgiK_a9qtCnFCxQyP7D0-3W9GGRIUiuYf0XEc,1203
+aisdb_web/dist_map/assets/vessel_metadata-c128d07d.js,sha256=c7y--BMsUfvyTK2_Gp_FThFRTnMBlu82WZjXRMqAuAE,1084
 aisdb_web/dist_map/assets/vessel_metadata-d682b0f2.js,sha256=TW9HIPn_emfO0CLruDDDldWlWKvogWOXQZvHJVBzfDU,1203
 aisdb_web/dist_map/favicon.png,sha256=Uo5iXGbmz5ixSuP0EHvOgpOIb0vAmBTiq4D5Ry7q7VQ,26223
 aisdb_web/dist_map/favicon.svg,sha256=_4w8x1EeNtZKElqoucElo6q6vIIa8HbYG5fpcbmdqCg,21560
-aisdb_web/dist_map/index.html,sha256=bVOUAe--Q8t3mZXct9QQyP60UfIixSvle6RYtQyig94,2615
+aisdb_web/dist_map/index.html,sha256=-2lyN8jJh8RGbitiKnoYIs1h5nBuJZhBg1Qh82J5Q0M,2615
 aisdb_web/dist_map_bingmaps/assets/client_bg-05f4a55d.wasm,sha256=BfSlXYmetRCJhJ25mYKD2SJjeXanVTFxS3vB4P1aPD8,173279
+aisdb_web/dist_map_bingmaps/assets/client_bg-505558bc.wasm,sha256=UFVYvEtet-ClTLqnQTrItg9HTQ1hDvOZC9DdfktTAfs,173403
 aisdb_web/dist_map_bingmaps/assets/client_bg-6a509824.wasm,sha256=alCYJEqrMJGqbbpRfZfdyW5XPxHpccXY9XVWfWPQHuA,173279
 aisdb_web/dist_map_bingmaps/assets/client_bg-916ba2c4.wasm,sha256=kWuixLQgou9Sh4krEh-UtrkbPxgLMaZZQB7c6tI_c0A,173278
 aisdb_web/dist_map_bingmaps/assets/constants-870f4956.js,sha256=pU6L74Z_8CmmU6qkJJu9Toql52-WeRhA1iqEL_vLJxY,616
+aisdb_web/dist_map_bingmaps/assets/constants-b9e7c6db.js,sha256=dmQefbABTgjHu7Te8c29Fr5NMiWU76ptunIeoQrBoLA,653
 aisdb_web/dist_map_bingmaps/assets/index-f2c4f58e.css,sha256=8sT1jseE3LNxWJ_S05N816ALqs_E6ZceC8Hl0ElSGx8,8224
 aisdb_web/dist_map_bingmaps/assets/livestream-3a02edee.js,sha256=94e5GP-2pBPAUq4EvqMK9Dj5JHUPmBJLXNPHWAGunns,1185
 aisdb_web/dist_map_bingmaps/assets/livestream-6755c91e.js,sha256=bSq0jVAafulXw40aJ00YP3FZkFPZgD5se9Kql-svbkA,1185
 aisdb_web/dist_map_bingmaps/assets/livestream-73586b67.js,sha256=9eJBTgjx6HHoEBpM5lPtTspsfgdFHW3TxGlrP-EmaBY,1185
+aisdb_web/dist_map_bingmaps/assets/livestream-e1be7db5.js,sha256=IFNpIze539NyaYf2zOdcwsdoAb1H5VZW8BNaqyANLQs,1185
+aisdb_web/dist_map_bingmaps/assets/livestream-ffcfc7b5.js,sha256=rrRAp-Rf59Vrt0cVPCeTUidbTPf4GqPyPvNX3P-eWdo,1185
+aisdb_web/dist_map_bingmaps/assets/main-49cea758.js,sha256=qMeD88KvNoDCdYvWeOGQthCYiffrBeByxYcD8QrSqsM,2662
 aisdb_web/dist_map_bingmaps/assets/main-7f6e0eb2.js,sha256=gtVJBNlgjmhF0WKZCWeHAD0Zg6B_B4m-CwVTdbz4zw4,2662
 aisdb_web/dist_map_bingmaps/assets/main-8b0e81cf.js,sha256=mbPU7gEaOLYY6lKOxjpFXF_RpBIBPsd1nHVgZV1Kr1I,2662
+aisdb_web/dist_map_bingmaps/assets/main-f2134a8e.js,sha256=CnVLNrXLXFEWqhW4jBn2lXswCEJAlCe8RTuVrzs4WSM,2662
 aisdb_web/dist_map_bingmaps/assets/main-feaa3a7b.js,sha256=zI0Ip6M64Z_HXwgcGkGFgFZphqgur4f58XJH_SVXmCM,2662
+aisdb_web/dist_map_bingmaps/assets/map-17890f38.js,sha256=mKZ31j8B07Hl2nTKx-3cC6Hg8OHHpzJuDC1C16JTsvo,406288
+aisdb_web/dist_map_bingmaps/assets/map-54e8d9a1.js,sha256=-LNaMUAcd-g9ysiDnlrd2azjx1_WUfyky9XT8Td79kQ,405598
 aisdb_web/dist_map_bingmaps/assets/map-64a6868c.js,sha256=4cBZ1r7cBxq2MXrXETVhQVlv3nxZHwJBQzFa3pPFGNk,405469
 aisdb_web/dist_map_bingmaps/assets/map-967b67d1.js,sha256=_gGPStEnrrw_HK5AXL3JVTtDWEAId-Q00u6m58LySuE,405469
 aisdb_web/dist_map_bingmaps/assets/map-c04ede37.css,sha256=wE7eN3fQO3muXiTjgPLskMQiWIF25PplqxbTZK63G_U,15782
 aisdb_web/dist_map_bingmaps/assets/map-c0ca9a66.js,sha256=xK58bvhTYtvsn8dl3PqDh38BqPXruyH7MHFXDFN9AQs,405469
 aisdb_web/dist_map_bingmaps/assets/proj-04f64360.js,sha256=mf3SgagDwAypPtlFocyzkSaF-tHB7iuFHPHeMvvdIAA,16622
+aisdb_web/dist_map_bingmaps/assets/proj-cfc8763a.js,sha256=zFKcmmJ7_4a-6tO2HMi2JSwJ1GiTc6Aj4JppgoUOCOA,16617
+aisdb_web/dist_map_bingmaps/assets/render-002f1925.js,sha256=RrJLxwwtBxU_oGRr6Sb6yXyq1snOzNeSzy-VMK0PI2A,203253
 aisdb_web/dist_map_bingmaps/assets/render-75680345.js,sha256=jV8n-ssU6VlNVn74pxXEfKUvqwxvLBKNXvzC_Y0PyiM,203253
+aisdb_web/dist_map_bingmaps/assets/render-9dc74427.js,sha256=3uM9brO4X914fVQGE9qbXB9eDWeEVtNEG4X5qUYsJrE,203229
 aisdb_web/dist_map_bingmaps/assets/render-c2851da9.js,sha256=rwYkfCfIWj7cXT-_tkCDS2Z2cPQC3eeR5UDbZmvL8M8,203253
 aisdb_web/dist_map_bingmaps/assets/render-c61cd003.js,sha256=JfZ9UdxVn044a4rL9CRccbqmToi8emUOG-_BCFCtwak,203253
 aisdb_web/dist_map_bingmaps/assets/tileserver-0d479a70.js,sha256=rKE4ZmzzF7ankTShgFiFiSdgNfkU7boHs3mo5gyDq3M,20179
 aisdb_web/dist_map_bingmaps/assets/tileserver-1d4ceaca.js,sha256=gqWj7qqYwLEJMLBiDmmGW8blDSprAuUPehpjRfL-WgY,20179
 aisdb_web/dist_map_bingmaps/assets/tileserver-2ce22ad4.js,sha256=TZTtzkypnobeMsrWQSLkSGMuo_PKKNgk_sXI3Sp3QHo,20179
+aisdb_web/dist_map_bingmaps/assets/tileserver-a213d9f6.js,sha256=0gG5np0s-lxe2M8D91rxQFmQJuAnkPkt5vyIqYnaHCg,19952
+aisdb_web/dist_map_bingmaps/assets/tileserver-ce29a4c1.js,sha256=76u-8OZyIqmiPBcyVnr5OHBImDC7ToLfqu1sek3IlN0,20179
 aisdb_web/dist_map_bingmaps/assets/url-3542f36d.js,sha256=8XDE2_g3Nk-_ofB21sTZIQB3fEqyxauED3fwkD0AwPM,3114
 aisdb_web/dist_map_bingmaps/assets/url-43e87897.js,sha256=y1kzeDj7yW1LVwCi5V3UHPI6V9F9VrS39By_bHsoy3c,3114
+aisdb_web/dist_map_bingmaps/assets/url-447c8bef.js,sha256=sHkI2sZHwx7yJlycjZbFfYWCB1GzA7YW9sAeX6eqRl4,3114
 aisdb_web/dist_map_bingmaps/assets/url-be1cb54a.js,sha256=mRjOTf-0hJu5vbMt8jSZjIPVFiWvWMpTTtHEa5eAk4o,3114
+aisdb_web/dist_map_bingmaps/assets/url-decb3532.js,sha256=7fpdEAyIM2OuUR4FAlH80CrF2SLeKomm9x96oKTmhac,3114
+aisdb_web/dist_map_bingmaps/assets/vessel_metadata-a1e91a33.js,sha256=gqJ3K3kBrLolrSg-WPKTnG34O0MG6xfaxGVdGymP2kY,1084
 aisdb_web/dist_map_bingmaps/assets/vessel_metadata-a3d1e26e.js,sha256=UDqwJfnFsCkFrgbWM2MwuOF_Pw5J-0067ZAuLs7Sqlg,1203
 aisdb_web/dist_map_bingmaps/assets/vessel_metadata-b8bf0fe9.js,sha256=5pQzujezSISzD4jInU4tKAFbm1yISyVYT54HfhgTe0o,1203
 aisdb_web/dist_map_bingmaps/assets/vessel_metadata-df772244.js,sha256=_yP8vMfPao4WJolovML-t66akjDEOaXfYbG3VOJuguk,1203
+aisdb_web/dist_map_bingmaps/assets/vessel_metadata-fe112f38.js,sha256=0ouHCZHzmy0p9XBU9sH3dmZndY1_jDG4o5YZiJfTm2w,1203
 aisdb_web/dist_map_bingmaps/favicon.png,sha256=Uo5iXGbmz5ixSuP0EHvOgpOIb0vAmBTiq4D5Ry7q7VQ,26223
 aisdb_web/dist_map_bingmaps/favicon.svg,sha256=_4w8x1EeNtZKElqoucElo6q6vIIa8HbYG5fpcbmdqCg,21560
-aisdb_web/dist_map_bingmaps/index.html,sha256=-STP38pyx3KYo0PXDZYYb0DBghRm-Qj0og7ejlZAplE,2615
-aisdb/aisdb.cpython-39-aarch64-linux-gnu.so,sha256=32LoEFMv4dOf9dU9oEc4LTuQXhIJTwaovU_l_gdnSx0,4800368
-aisdb-1.6.4.dist-info/RECORD,,
+aisdb_web/dist_map_bingmaps/index.html,sha256=WfK2s3GH2amDHyzrsXa5omtu66xg55pz86zT589oO1k,2615
+aisdb/aisdb.cpython-39-darwin.so,sha256=_eS9WcjDmnvhmzKjfaVyhJTnMhOv7-xzeC7MCYt2h9k,4624391
+aisdb-1.6.5.dist-info/RECORD,,
```

