# Comparing `tmp/usda-0.0.24.tar.gz` & `tmp/usda-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usda-0.0.24.tar", last modified: Tue Jul 11 03:35:34 2023, max compression
+gzip compressed data, was "usda-0.0.25.tar", last modified: Tue Jul 11 03:55:24 2023, max compression
```

## Comparing `usda-0.0.24.tar` & `usda-0.0.25.tar`

### file list

```diff
@@ -1,294 +1,294 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:34.280500 usda-0.0.24/
--rw-rw-rw-   0        0        0     1084 2022-10-07 01:27:44.000000 usda-0.0.24/LICENSE
--rw-rw-rw-   0        0        0     1563 2023-07-11 03:35:34.274500 usda-0.0.24/PKG-INFO
--rw-rw-rw-   0        0        0       63 2022-10-24 05:51:49.000000 usda-0.0.24/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-11 03:35:34.280500 usda-0.0.24/setup.cfg
--rw-rw-rw-   0        0        0     4305 2023-05-21 04:03:07.000000 usda-0.0.24/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:33.256736 usda-0.0.24/src/
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:33.326377 usda-0.0.24/src/usda/
--rw-rw-rw-   0        0        0      636 2023-07-11 03:35:26.000000 usda-0.0.24/src/usda/__init__.py
--rw-rw-rw-   0        0        0      731 2022-10-16 01:25:29.000000 usda-0.0.24/src/usda/_min_dependencies.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:33.373413 usda-0.0.24/src/usda/data_process/
--rw-rw-rw-   0        0        0     1147 2023-03-26 03:42:04.000000 usda-0.0.24/src/usda/data_process/__init__.py
--rw-rw-rw-   0        0        0     2125 2022-10-22 01:48:58.000000 usda-0.0.24/src/usda/data_process/_geoinfodata_conversion.py
--rw-rw-rw-   0        0        0    14577 2022-10-28 01:52:51.000000 usda-0.0.24/src/usda/data_process/_image_pixel_sampling_zoom.py
--rw-rw-rw-   0        0        0     1425 2022-10-31 06:03:57.000000 usda-0.0.24/src/usda/data_process/_kitti_dataprocess.py
--rw-rw-rw-   0        0        0     2037 2022-10-26 01:37:19.000000 usda-0.0.24/src/usda/data_process/_landsat_dataprocess.py
--rw-rw-rw-   0        0        0     1854 2023-03-26 07:52:38.000000 usda-0.0.24/src/usda/data_process/_naip_dataprocess.py
--rw-rw-rw-   0        0        0     6348 2022-10-22 00:18:38.000000 usda-0.0.24/src/usda/data_process/_osm_dataprocess.py
--rw-rw-rw-   0        0        0     1085 2023-02-11 08:44:30.000000 usda-0.0.24/src/usda/data_process/_raster_dataprocess.py
--rw-rw-rw-   0        0        0     1332 2022-10-30 06:27:55.000000 usda-0.0.24/src/usda/data_process/_tiler_calculation.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:33.382407 usda-0.0.24/src/usda/data_visual/
--rw-rw-rw-   0        0        0      304 2023-07-09 12:19:47.000000 usda-0.0.24/src/usda/data_visual/__init__.py
--rw-rw-rw-   0        0        0      499 2023-05-14 10:52:12.000000 usda-0.0.24/src/usda/data_visual/_plot_style.py
--rw-rw-rw-   0        0        0     1362 2023-07-09 12:16:31.000000 usda-0.0.24/src/usda/data_visual/_worldcover_plot_style.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:33.448379 usda-0.0.24/src/usda/data_visualization/
--rw-rw-rw-   0        0        0     3205 2023-05-30 14:40:53.000000 usda-0.0.24/src/usda/data_visualization/__init__.py
--rw-rw-rw-   0        0        0     5300 2023-02-17 02:29:25.000000 usda-0.0.24/src/usda/data_visualization/_chart_custom.py
--rw-rw-rw-   0        0        0     3729 2023-05-30 14:40:34.000000 usda-0.0.24/src/usda/data_visualization/_colors.py
--rw-rw-rw-   0        0        0     3221 2022-10-29 07:58:07.000000 usda-0.0.24/src/usda/data_visualization/_dynamic_streetView_visual_perception.py
--rw-rw-rw-   0        0        0     3557 2023-02-19 14:47:51.000000 usda-0.0.24/src/usda/data_visualization/_gdf_plot.py
--rw-rw-rw-   0        0        0      952 2022-10-28 11:19:32.000000 usda-0.0.24/src/usda/data_visualization/_gif_show.py
--rw-rw-rw-   0        0        0     2347 2022-10-28 06:34:44.000000 usda-0.0.24/src/usda/data_visualization/_graphic_drawing.py
--rw-rw-rw-   0        0        0     4787 2022-10-31 05:36:51.000000 usda-0.0.24/src/usda/data_visualization/_image_process.py
--rw-rw-rw-   0        0        0     8500 2022-10-29 06:42:38.000000 usda-0.0.24/src/usda/data_visualization/_img_feature_extraction.py
--rw-rw-rw-   0        0        0     7196 2022-10-30 12:18:06.000000 usda-0.0.24/src/usda/data_visualization/_img_theme_color.py
--rw-rw-rw-   0        0        0     2846 2022-10-30 11:18:24.000000 usda-0.0.24/src/usda/data_visualization/_imgs_layout_show.py
--rw-rw-rw-   0        0        0     4174 2023-03-15 02:00:19.000000 usda-0.0.24/src/usda/data_visualization/_imgs_show.py
--rw-rw-rw-   0        0        0      822 2022-11-02 06:07:14.000000 usda-0.0.24/src/usda/data_visualization/_knee_line_graph.py
--rw-rw-rw-   0        0        0     7393 2022-10-29 08:23:53.000000 usda-0.0.24/src/usda/data_visualization/_moving_average_inflection.py
--rw-rw-rw-   0        0        0     3176 2023-02-24 07:31:39.000000 usda-0.0.24/src/usda/data_visualization/_panorama_show.py
--rw-rw-rw-   0        0        0     8051 2023-03-19 04:08:53.000000 usda-0.0.24/src/usda/data_visualization/_plot_single_function.py
--rw-rw-rw-   0        0        0     2310 2022-10-28 01:13:41.000000 usda-0.0.24/src/usda/data_visualization/_raster_percentile_slider.py
--rw-rw-rw-   0        0        0     1224 2022-10-28 00:45:13.000000 usda-0.0.24/src/usda/data_visualization/_raster_show.py
--rw-rw-rw-   0        0        0     2130 2022-10-28 06:32:06.000000 usda-0.0.24/src/usda/data_visualization/_stats_charts.py
--rw-rw-rw-   0        0        0     2666 2022-10-30 07:27:14.000000 usda-0.0.24/src/usda/data_visualization/_superpixel_segmentation_show.py
--rw-rw-rw-   0        0        0     1577 2022-10-22 23:37:39.000000 usda-0.0.24/src/usda/data_visualization/_table_show.py
--rw-rw-rw-   0        0        0     1673 2022-11-02 06:07:23.000000 usda-0.0.24/src/usda/data_visualization/_tile_show.py
--rw-rw-rw-   0        0        0     4464 2020-07-17 02:38:10.000000 usda-0.0.24/src/usda/data_visualization/data_generator.py
--rw-rw-rw-   0        0        0    10263 2020-07-17 02:38:10.000000 usda-0.0.24/src/usda/data_visualization/knee_locator.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:33.465607 usda-0.0.24/src/usda/database/
--rw-rw-rw-   0        0        0      839 2023-03-21 05:11:06.000000 usda-0.0.24/src/usda/database/__init__.py
--rw-rw-rw-   0        0        0      693 2022-10-30 12:15:41.000000 usda-0.0.24/src/usda/database/_data_file_rw.py
--rw-rw-rw-   0        0        0     4636 2023-03-21 05:10:00.000000 usda-0.0.24/src/usda/database/_data_format_conversion.py
--rw-rw-rw-   0        0        0     5605 2023-03-21 05:08:27.000000 usda-0.0.24/src/usda/database/_database.py
--rw-rw-rw-   0        0        0     1384 2022-10-28 08:27:55.000000 usda-0.0.24/src/usda/database/_read_matlab_fig.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:33.482644 usda-0.0.24/src/usda/datasets/
--rw-rw-rw-   0        0        0     2003 2023-07-09 08:35:22.000000 usda-0.0.24/src/usda/datasets/__init__.py
--rw-rw-rw-   0        0        0    17136 2023-03-13 12:40:56.000000 usda-0.0.24/src/usda/datasets/_artificial_data.py
--rw-rw-rw-   0        0        0    19730 2023-03-14 01:14:44.000000 usda-0.0.24/src/usda/datasets/_base.py
--rw-rw-rw-   0        0        0     2745 2022-10-31 05:44:19.000000 usda-0.0.24/src/usda/datasets/_dataset_info.py
--rw-rw-rw-   0        0        0     5119 2023-07-09 08:43:54.000000 usda-0.0.24/src/usda/datasets/_files_downloading.py
--rw-rw-rw-   0        0        0     2681 2022-10-30 11:21:33.000000 usda-0.0.24/src/usda/datasets/_img_info.py
--rw-rw-rw-   0        0        0     2806 2022-10-30 10:50:28.000000 usda-0.0.24/src/usda/datasets/_kml_info.py
--rw-rw-rw-   0        0        0     1547 2022-10-30 07:02:03.000000 usda-0.0.24/src/usda/datasets/_rs_image.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:33.511603 usda-0.0.24/src/usda/datasets/data/
--rw-rw-rw-   0        0        0      125 2022-08-21 07:11:20.000000 usda-0.0.24/src/usda/datasets/data/__init__.py
--rw-rw-rw-   0        0        0     1224 2022-10-19 04:41:26.000000 usda-0.0.24/src/usda/datasets/data/bowling_contest_cartoon_statistic.pickle
--rw-rw-rw-   0        0        0      950 2023-02-23 02:44:29.000000 usda-0.0.24/src/usda/datasets/data/evaluation_criteria_raw_values.pickle
--rw-rw-rw-   0        0        0     8356 2023-03-13 12:16:36.000000 usda-0.0.24/src/usda/datasets/data/jisperveld_data.pickle
--rw-rw-rw-   0        0        0     1486 2023-02-27 14:21:28.000000 usda-0.0.24/src/usda/datasets/data/microclimate_in_office_rooms.pickle
--rw-rw-rw-   0        0        0     1089 2022-10-19 01:41:55.000000 usda-0.0.24/src/usda/datasets/data/ramen_price_cartoon_statistic.pickle
--rw-rw-rw-   0        0        0     2123 2022-10-15 01:16:56.000000 usda-0.0.24/src/usda/datasets/data/sales_data_cartoon_database.pickle
--rw-rw-rw-   0        0        0     1352 2023-02-24 07:53:38.000000 usda-0.0.24/src/usda/datasets/data/sustainability_attributes4electricity_generation_tech.pickle
--rw-rw-rw-   0        0        0     1340 2022-10-19 05:00:19.000000 usda-0.0.24/src/usda/datasets/data/test_score_cartoon_statistic.pickle
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:33.546347 usda-0.0.24/src/usda/geodata_process/
--rw-rw-rw-   0        0        0     1932 2023-07-10 10:21:46.000000 usda-0.0.24/src/usda/geodata_process/__init__.py
--rw-rw-rw-   0        0        0     2906 2023-07-10 11:42:14.000000 usda-0.0.24/src/usda/geodata_process/_build_clipped_raster_dataset.py
--rw-rw-rw-   0        0        0     1197 2023-07-10 09:55:02.000000 usda-0.0.24/src/usda/geodata_process/_build_clipped_raster_dataset_pool.py
--rw-rw-rw-   0        0        0     6447 2023-07-10 00:45:07.000000 usda-0.0.24/src/usda/geodata_process/_quadrat.py
--rw-rw-rw-   0        0        0     6535 2023-03-22 16:40:23.000000 usda-0.0.24/src/usda/geodata_process/_raster_dataprocess.py
--rw-rw-rw-   0        0        0     6633 2023-03-22 14:50:33.000000 usda-0.0.24/src/usda/geodata_process/_raster_stats.py
--rw-rw-rw-   0        0        0     6661 2023-03-21 13:11:59.000000 usda-0.0.24/src/usda/geodata_process/_rasterize.py
--rw-rw-rw-   0        0        0     3097 2023-07-07 04:06:42.000000 usda-0.0.24/src/usda/geodata_process/_rio_tiler.py
--rw-rw-rw-   0        0        0     4952 2023-06-02 02:08:47.000000 usda-0.0.24/src/usda/geodata_process/_sample_pts.py
--rw-rw-rw-   0        0        0     1040 2023-04-17 23:16:55.000000 usda-0.0.24/src/usda/geodata_process/_shp_dataprocess.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:33.555349 usda-0.0.24/src/usda/imgs_process/
--rw-rw-rw-   0        0        0      457 2023-06-08 12:42:37.000000 usda-0.0.24/src/usda/imgs_process/__init__.py
--rw-rw-rw-   0        0        0     2768 2023-06-08 12:45:27.000000 usda-0.0.24/src/usda/imgs_process/_imgs_process_basic.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:33.560328 usda-0.0.24/src/usda/indices/
--rw-rw-rw-   0        0        0      189 2022-10-26 06:14:56.000000 usda-0.0.24/src/usda/indices/__init__.py
--rw-rw-rw-   0        0        0      574 2022-10-26 06:15:29.000000 usda-0.0.24/src/usda/indices/_rs_indices.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:33.581433 usda-0.0.24/src/usda/maths/
--rw-rw-rw-   0        0        0      645 2023-04-11 23:36:35.000000 usda-0.0.24/src/usda/maths/__init__.py
--rw-rw-rw-   0        0        0     4335 2022-10-26 02:53:02.000000 usda-0.0.24/src/usda/maths/_algebra.py
--rw-rw-rw-   0        0        0     1519 2022-10-26 03:05:19.000000 usda-0.0.24/src/usda/maths/_geometric_calculation.py
--rw-rw-rw-   0        0        0     8051 2023-04-11 23:36:06.000000 usda-0.0.24/src/usda/maths/_plot_single_function.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:33.628400 usda-0.0.24/src/usda/meta_heuristics/
--rw-rw-rw-   0        0        0      843 2023-03-19 01:33:28.000000 usda-0.0.24/src/usda/meta_heuristics/__init__.py
--rw-rw-rw-   0        0        0     5889 2023-03-18 13:00:33.000000 usda-0.0.24/src/usda/meta_heuristics/_cuckoo_s.py
--rw-rw-rw-   0        0        0     4919 2023-03-19 01:22:52.000000 usda-0.0.24/src/usda/meta_heuristics/_firefly_a.py
--rw-rw-rw-   0        0        0    11373 2023-03-10 03:50:42.000000 usda-0.0.24/src/usda/meta_heuristics/_ga.py
--rw-rw-rw-   0        0        0    13840 2023-03-15 22:13:00.000000 usda-0.0.24/src/usda/meta_heuristics/_ga_2d.py
--rw-rw-rw-   0        0        0    14213 2023-03-16 01:38:05.000000 usda-0.0.24/src/usda/meta_heuristics/_ga_2d_fixed_map.py
--rw-rw-rw-   0        0        0    15440 2023-03-15 14:33:57.000000 usda-0.0.24/src/usda/meta_heuristics/_ga_2d_testing_1.py
--rw-rw-rw-   0        0        0    25287 2023-03-17 02:56:06.000000 usda-0.0.24/src/usda/meta_heuristics/_ga_2d_testing_2.py
--rw-rw-rw-   0        0        0     4177 2023-03-10 02:05:28.000000 usda-0.0.24/src/usda/meta_heuristics/_ga_SegaranT.py
--rw-rw-rw-   0        0        0     7982 2023-03-01 00:42:26.000000 usda-0.0.24/src/usda/meta_heuristics/_gwo.py
--rw-rw-rw-   0        0        0     5251 2023-03-17 04:06:12.000000 usda-0.0.24/src/usda/meta_heuristics/_pso.py
--rw-rw-rw-   0        0        0     7564 2023-03-18 04:30:41.000000 usda-0.0.24/src/usda/meta_heuristics/_pso_2d.py
--rw-rw-rw-   0        0        0     8467 2023-03-18 05:15:54.000000 usda-0.0.24/src/usda/meta_heuristics/_pso_2d_testing.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:33.630402 usda-0.0.24/src/usda/migrated_project/
--rw-rw-rw-   0        0        0      180 2023-04-17 02:04:10.000000 usda-0.0.24/src/usda/migrated_project/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:33.633401 usda-0.0.24/src/usda/migrated_project/invest/
--rw-rw-rw-   0        0        0      711 2023-06-11 01:34:27.000000 usda-0.0.24/src/usda/migrated_project/invest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:33.676364 usda-0.0.24/src/usda/migrated_project/invest/configs/
--rw-rw-rw-   0        0        0     1150 2023-06-09 12:59:23.000000 usda-0.0.24/src/usda/migrated_project/invest/configs/__init__.py
--rw-rw-rw-   0        0        0     1320 2023-05-21 14:16:56.000000 usda-0.0.24/src/usda/migrated_project/invest/configs/_carbon_configs.py
--rw-rw-rw-   0        0        0     5303 2023-05-22 07:01:13.000000 usda-0.0.24/src/usda/migrated_project/invest/configs/_crop_pollination_configs.py
--rw-rw-rw-   0        0        0     2352 2023-05-22 09:31:32.000000 usda-0.0.24/src/usda/migrated_project/invest/configs/_crop_production_percentile_configs.py
--rw-rw-rw-   0        0        0     3674 2023-05-22 08:55:38.000000 usda-0.0.24/src/usda/migrated_project/invest/configs/_crop_production_regression_configs.py
--rw-rw-rw-   0        0        0      490 2023-05-21 18:26:40.000000 usda-0.0.24/src/usda/migrated_project/invest/configs/_habitat_quality_configs.py
--rw-rw-rw-   0        0        0      117 2023-06-09 13:00:21.000000 usda-0.0.24/src/usda/migrated_project/invest/configs/_urban_cooling_configs.py
--rw-rw-rw-   0        0        0     2095 2023-04-29 10:05:57.000000 usda-0.0.24/src/usda/migrated_project/invest/configs/carbon_pools_willamette.csv
--rw-rw-rw-   0        0        0     1684 2023-05-16 20:54:57.000000 usda-0.0.24/src/usda/migrated_project/invest/configs/unit_definitions.txt
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:33.712895 usda-0.0.24/src/usda/migrated_project/invest/esv/
--rw-rw-rw-   0        0        0      700 2023-06-09 23:15:32.000000 usda-0.0.24/src/usda/migrated_project/invest/esv/__init__.py
--rw-rw-rw-   0        0        0    23442 2023-05-31 01:40:43.000000 usda-0.0.24/src/usda/migrated_project/invest/esv/_carbon.py
--rw-rw-rw-   0        0        0    66377 2023-05-22 12:57:02.000000 usda-0.0.24/src/usda/migrated_project/invest/esv/_crop_pollination.py
--rw-rw-rw-   0        0        0    37499 2023-05-22 10:16:20.000000 usda-0.0.24/src/usda/migrated_project/invest/esv/_crop_production_percentile.py
--rw-rw-rw-   0        0        0    43341 2023-05-22 13:20:45.000000 usda-0.0.24/src/usda/migrated_project/invest/esv/_crop_production_regression.py
--rw-rw-rw-   0        0        0    41477 2023-05-22 12:35:30.000000 usda-0.0.24/src/usda/migrated_project/invest/esv/_habitat_quality.py
--rw-rw-rw-   0        0        0      610 2023-05-21 04:07:41.000000 usda-0.0.24/src/usda/migrated_project/invest/esv/_unit_registry.py
--rw-rw-rw-   0        0        0    56182 2023-06-10 02:41:05.000000 usda-0.0.24/src/usda/migrated_project/invest/esv/_urban_cooling_model.py
--rw-rw-rw-   0        0        0    44236 2023-05-21 14:00:31.000000 usda-0.0.24/src/usda/migrated_project/invest/esv/_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:33.726883 usda-0.0.24/src/usda/migrated_project/pix2pix/
--rw-rw-rw-   0        0        0     1969 2023-04-20 08:47:17.000000 usda-0.0.24/src/usda/migrated_project/pix2pix/A2B.py
--rw-rw-rw-   0        0        0      217 2023-04-21 13:54:27.000000 usda-0.0.24/src/usda/migrated_project/pix2pix/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:33.755857 usda-0.0.24/src/usda/migrated_project/pix2pix/data/
--rw-rw-rw-   0        0        0     4100 2023-04-20 05:37:10.000000 usda-0.0.24/src/usda/migrated_project/pix2pix/data/__init__.py
--rw-rw-rw-   0        0        0     2728 2023-04-17 06:17:12.000000 usda-0.0.24/src/usda/migrated_project/pix2pix/data/_aligned_dataset.py
--rw-rw-rw-   0        0        0     6235 2023-04-17 05:52:31.000000 usda-0.0.24/src/usda/migrated_project/pix2pix/data/_base_dataset.py
--rw-rw-rw-   0        0        0     2897 2023-04-17 06:21:59.000000 usda-0.0.24/src/usda/migrated_project/pix2pix/data/_colorization_dataset.py
--rw-rw-rw-   0        0        0     1885 2023-03-14 20:28:49.000000 usda-0.0.24/src/usda/migrated_project/pix2pix/data/_image_folder.py
--rw-rw-rw-   0        0        0     1658 2023-04-17 06:19:58.000000 usda-0.0.24/src/usda/migrated_project/pix2pix/data/_single_dataset.py
--rw-rw-rw-   0        0        0     3589 2023-04-17 03:48:21.000000 usda-0.0.24/src/usda/migrated_project/pix2pix/data/_template_dataset.py
--rw-rw-rw-   0        0        0     3526 2023-04-17 05:45:03.000000 usda-0.0.24/src/usda/migrated_project/pix2pix/data/_unaligned_dataset.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:33.758856 usda-0.0.24/src/usda/migrated_project/pix2pix/datasets/
--rw-rw-rw-   0        0        0      198 2023-04-17 01:54:37.000000 usda-0.0.24/src/usda/migrated_project/pix2pix/datasets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:33.772533 usda-0.0.24/src/usda/migrated_project/pix2pix/imgs/
--rw-rw-rw-   0        0        0      127 2023-04-21 13:57:19.000000 usda-0.0.24/src/usda/migrated_project/pix2pix/imgs/__init__.py
--rw-rw-rw-   0        0        0    14064 2023-04-21 14:08:05.000000 usda-0.0.24/src/usda/migrated_project/pix2pix/imgs/example.jpg
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:33.786531 usda-0.0.24/src/usda/migrated_project/pix2pix/models/
--rw-rw-rw-   0        0        0     3349 2023-04-20 02:44:45.000000 usda-0.0.24/src/usda/migrated_project/pix2pix/models/__init__.py
--rw-rw-rw-   0        0        0    10810 2023-04-17 07:20:11.000000 usda-0.0.24/src/usda/migrated_project/pix2pix/models/_base_model.py
--rw-rw-rw-   0        0        0    29098 2023-04-17 07:31:07.000000 usda-0.0.24/src/usda/migrated_project/pix2pix/models/_networks.py
--rw-rw-rw-   0        0        0     7024 2023-04-17 07:21:10.000000 usda-0.0.24/src/usda/migrated_project/pix2pix/models/_pix2pix_model.py
--rw-rw-rw-   0        0        0     3392 2023-04-17 12:08:31.000000 usda-0.0.24/src/usda/migrated_project/pix2pix/models/_test_model.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:33.807494 usda-0.0.24/src/usda/migrated_project/pix2pix/options/
--rw-rw-rw-   0        0        0      425 2023-04-17 11:42:46.000000 usda-0.0.24/src/usda/migrated_project/pix2pix/options/__init__.py
--rw-rw-rw-   0        0        0     3447 2023-04-17 08:10:06.000000 usda-0.0.24/src/usda/migrated_project/pix2pix/options/_base_options.py
--rw-rw-rw-   0        0        0     1045 2023-04-17 12:42:33.000000 usda-0.0.24/src/usda/migrated_project/pix2pix/options/_test_options.py
--rw-rw-rw-   0        0        0     2533 2023-04-17 11:39:45.000000 usda-0.0.24/src/usda/migrated_project/pix2pix/options/_train_options.py
--rw-rw-rw-   0        0        0     8846 2023-04-22 00:58:18.000000 usda-0.0.24/src/usda/migrated_project/pix2pix/sketch_A2B.py
--rw-rw-rw-   0        0        0     6019 2023-04-17 13:04:35.000000 usda-0.0.24/src/usda/migrated_project/pix2pix/test.py
--rw-rw-rw-   0        0        0     6788 2023-04-18 09:54:15.000000 usda-0.0.24/src/usda/migrated_project/pix2pix/train.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:33.832420 usda-0.0.24/src/usda/migrated_project/pix2pix/util/
--rw-rw-rw-   0        0        0      270 2023-04-17 11:51:19.000000 usda-0.0.24/src/usda/migrated_project/pix2pix/util/__init__.py
--rw-rw-rw-   0        0        0     3639 2023-03-14 20:28:49.000000 usda-0.0.24/src/usda/migrated_project/pix2pix/util/_get_data.py
--rw-rw-rw-   0        0        0     3223 2023-03-14 20:28:49.000000 usda-0.0.24/src/usda/migrated_project/pix2pix/util/_html.py
--rw-rw-rw-   0        0        0     2226 2023-03-14 20:28:49.000000 usda-0.0.24/src/usda/migrated_project/pix2pix/util/_image_pool.py
--rw-rw-rw-   0        0        0     3175 2023-03-14 20:28:49.000000 usda-0.0.24/src/usda/migrated_project/pix2pix/util/_util.py
--rw-rw-rw-   0        0        0    12408 2023-04-17 09:41:44.000000 usda-0.0.24/src/usda/migrated_project/pix2pix/util/_visualizer.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:33.877339 usda-0.0.24/src/usda/migrated_project/stylegan/
--rw-rw-rw-   0        0        0      898 2023-04-17 10:27:41.000000 usda-0.0.24/src/usda/migrated_project/stylegan/__init__.py
--rw-rw-rw-   0        0        0     3082 2023-04-16 06:09:08.000000 usda-0.0.24/src/usda/migrated_project/stylegan/_config.py
--rw-rw-rw-   0        0        0     4425 2023-04-11 12:13:43.000000 usda-0.0.24/src/usda/migrated_project/stylegan/_convert.py
--rw-rw-rw-   0        0        0     3527 2023-04-11 12:16:24.000000 usda-0.0.24/src/usda/migrated_project/stylegan/_generate_grid.py
--rw-rw-rw-   0        0        0     5616 2023-04-16 11:14:57.000000 usda-0.0.24/src/usda/migrated_project/stylegan/_generate_mixing_figure.py
--rw-rw-rw-   0        0        0     4595 2023-04-16 07:34:49.000000 usda-0.0.24/src/usda/migrated_project/stylegan/_generate_samples.py
--rw-rw-rw-   0        0        0     3430 2023-04-16 08:58:05.000000 usda-0.0.24/src/usda/migrated_project/stylegan/_generate_truncation_figure.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:33.908708 usda-0.0.24/src/usda/migrated_project/stylegan/data/
--rw-rw-rw-   0        0        0      558 2023-04-11 11:18:10.000000 usda-0.0.24/src/usda/migrated_project/stylegan/data/__init__.py
--rw-rw-rw-   0        0        0     4744 2023-04-11 10:36:07.000000 usda-0.0.24/src/usda/migrated_project/stylegan/data/_datasets.py
--rw-rw-rw-   0        0        0     1457 2023-04-11 10:36:54.000000 usda-0.0.24/src/usda/migrated_project/stylegan/data/_make_dataset.py
--rw-rw-rw-   0        0        0     1014 2023-04-11 10:37:15.000000 usda-0.0.24/src/usda/migrated_project/stylegan/data/_transforms.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:33.916666 usda-0.0.24/src/usda/migrated_project/stylegan/dnnlib/
--rw-rw-rw-   0        0        0      799 2021-12-18 03:07:03.000000 usda-0.0.24/src/usda/migrated_project/stylegan/dnnlib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:33.936035 usda-0.0.24/src/usda/migrated_project/stylegan/dnnlib/submission/
--rw-rw-rw-   0        0        0      392 2021-12-18 03:07:03.000000 usda-0.0.24/src/usda/migrated_project/stylegan/dnnlib/submission/__init__.py
--rw-rw-rw-   0        0        0     4337 2021-12-18 03:07:03.000000 usda-0.0.24/src/usda/migrated_project/stylegan/dnnlib/submission/run_context.py
--rw-rw-rw-   0        0        0    11131 2021-12-18 03:07:03.000000 usda-0.0.24/src/usda/migrated_project/stylegan/dnnlib/submission/submit.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:33.964037 usda-0.0.24/src/usda/migrated_project/stylegan/dnnlib/tflib/
--rw-rw-rw-   0        0        0      524 2021-12-18 03:07:03.000000 usda-0.0.24/src/usda/migrated_project/stylegan/dnnlib/tflib/__init__.py
--rw-rw-rw-   0        0        0     7537 2021-12-18 03:07:03.000000 usda-0.0.24/src/usda/migrated_project/stylegan/dnnlib/tflib/autosummary.py
--rw-rw-rw-   0        0        0    30121 2021-12-18 03:07:03.000000 usda-0.0.24/src/usda/migrated_project/stylegan/dnnlib/tflib/network.py
--rw-rw-rw-   0        0        0    10027 2021-12-18 03:07:03.000000 usda-0.0.24/src/usda/migrated_project/stylegan/dnnlib/tflib/optimizer.py
--rw-rw-rw-   0        0        0     9306 2023-04-11 12:36:18.000000 usda-0.0.24/src/usda/migrated_project/stylegan/dnnlib/tflib/tfutil.py
--rw-rw-rw-   0        0        0    13756 2021-12-18 03:07:03.000000 usda-0.0.24/src/usda/migrated_project/stylegan/dnnlib/util.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:33.971079 usda-0.0.24/src/usda/migrated_project/stylegan/extracted_funcs/
--rw-rw-rw-   0        0        0      186 2023-04-12 06:22:03.000000 usda-0.0.24/src/usda/migrated_project/stylegan/extracted_funcs/__init__.py
--rw-rw-rw-   0        0        0     1354 2023-04-12 06:27:22.000000 usda-0.0.24/src/usda/migrated_project/stylegan/extracted_funcs/_gadgets.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:34.000077 usda-0.0.24/src/usda/migrated_project/stylegan/models/
--rw-rw-rw-   0        0        0     6331 2023-04-11 11:53:57.000000 usda-0.0.24/src/usda/migrated_project/stylegan/models/_Blocks.py
--rw-rw-rw-   0        0        0    11748 2023-04-11 11:32:52.000000 usda-0.0.24/src/usda/migrated_project/stylegan/models/_CustomLayers.py
--rw-rw-rw-   0        0        0    38792 2023-04-11 11:52:55.000000 usda-0.0.24/src/usda/migrated_project/stylegan/models/_GAN.py
--rw-rw-rw-   0        0        0     8277 2023-04-11 11:27:22.000000 usda-0.0.24/src/usda/migrated_project/stylegan/models/_Losses.py
--rw-rw-rw-   0        0        0     1771 2023-04-11 11:56:27.000000 usda-0.0.24/src/usda/migrated_project/stylegan/models/__init__.py
--rw-rw-rw-   0        0        0     1388 2023-04-11 11:40:43.000000 usda-0.0.24/src/usda/migrated_project/stylegan/models/_update_average.py
--rw-rw-rw-   0        0        0     6150 2023-04-17 03:27:42.000000 usda-0.0.24/src/usda/migrated_project/stylegan/train.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:34.009077 usda-0.0.24/src/usda/migrated_project/stylegan/utils/
--rw-rw-rw-   0        0        0      247 2023-04-11 07:34:41.000000 usda-0.0.24/src/usda/migrated_project/stylegan/utils/__init__.py
--rw-rw-rw-   0        0        0     2159 2023-04-11 09:44:25.000000 usda-0.0.24/src/usda/migrated_project/stylegan/utils/_copy.py
--rw-rw-rw-   0        0        0      685 2023-04-11 10:33:56.000000 usda-0.0.24/src/usda/migrated_project/stylegan/utils/_logger.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:34.094738 usda-0.0.24/src/usda/models/
--rw-rw-rw-   0        0        0     5058 2023-07-02 05:03:24.000000 usda-0.0.24/src/usda/models/__init__.py
--rw-rw-rw-   0        0        0     3873 2022-10-31 06:56:19.000000 usda-0.0.24/src/usda/models/_bow_feature_builder.py
--rw-rw-rw-   0        0        0     1014 2023-03-24 02:28:49.000000 usda-0.0.24/src/usda/models/_clustering.py
--rw-rw-rw-   0        0        0     3105 2022-10-25 01:59:30.000000 usda-0.0.24/src/usda/models/_computational_performance.py
--rw-rw-rw-   0        0        0     1897 2022-10-28 08:34:08.000000 usda-0.0.24/src/usda/models/_curve_segmentation.py
--rw-rw-rw-   0        0        0     3928 2022-10-31 07:59:05.000000 usda-0.0.24/src/usda/models/_decision_tree.py
--rw-rw-rw-   0        0        0     5811 2022-10-28 08:15:41.000000 usda-0.0.24/src/usda/models/_dim1_convolution.py
--rw-rw-rw-   0        0        0     2676 2022-10-31 07:41:49.000000 usda-0.0.24/src/usda/models/_entropy.py
--rw-rw-rw-   0        0        0     1458 2023-03-24 10:49:05.000000 usda-0.0.24/src/usda/models/_global_local_autocorrelation.py
--rw-rw-rw-   0        0        0     1427 2022-11-02 06:11:04.000000 usda-0.0.24/src/usda/models/_image_tag_extractor.py
--rw-rw-rw-   0        0        0     2087 2023-06-21 23:53:49.000000 usda-0.0.24/src/usda/models/_label_encoder.py
--rw-rw-rw-   0        0        0     1022 2022-10-25 01:02:56.000000 usda-0.0.24/src/usda/models/_neighbors.py
--rw-rw-rw-   0        0        0     9967 2023-06-30 10:21:03.000000 usda-0.0.24/src/usda/models/_nlp_tools.py
--rw-rw-rw-   0        0        0     1422 2022-10-31 08:30:25.000000 usda-0.0.24/src/usda/models/_random_forest_classifier.py
--rw-rw-rw-   0        0        0     9501 2023-06-22 03:39:31.000000 usda-0.0.24/src/usda/models/_rnn_lstm.py
--rw-rw-rw-   0        0        0    16007 2023-06-30 12:22:03.000000 usda-0.0.24/src/usda/models/_seq2seq.py
--rw-rw-rw-   0        0        0    11923 2022-10-28 11:44:45.000000 usda-0.0.24/src/usda/models/_sir_model.py
--rw-rw-rw-   0        0        0     3200 2022-10-30 07:33:05.000000 usda-0.0.24/src/usda/models/_superpixel_segmentation.py
--rw-rw-rw-   0        0        0     9756 2023-07-01 03:01:16.000000 usda-0.0.24/src/usda/models/_transformer.py
--rw-rw-rw-   0        0        0     8560 2023-07-11 01:52:35.000000 usda-0.0.24/src/usda/models/_vit.py
--rw-rw-rw-   0        0        0     9313 2023-06-27 08:00:23.000000 usda-0.0.24/src/usda/models/_word2vec_sgns.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:34.101743 usda-0.0.24/src/usda/net/
--rw-rw-rw-   0        0        0      120 2023-04-05 02:07:48.000000 usda-0.0.24/src/usda/net/_.py
--rw-rw-rw-   0        0        0      856 2023-04-05 02:18:09.000000 usda-0.0.24/src/usda/net/__init__.py
--rw-rw-rw-   0        0        0    28490 2023-04-05 02:16:39.000000 usda-0.0.24/src/usda/net/_networks_pix2pix.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:34.114740 usda-0.0.24/src/usda/network/
--rw-rw-rw-   0        0        0      404 2023-04-01 07:37:21.000000 usda-0.0.24/src/usda/network/__init__.py
--rw-rw-rw-   0        0        0     4050 2023-03-10 11:37:13.000000 usda-0.0.24/src/usda/network/_g_drawing.py
--rw-rw-rw-   0        0        0     2896 2023-04-01 07:46:50.000000 usda-0.0.24/src/usda/network/_pt_pattern.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:34.141964 usda-0.0.24/src/usda/pattern_signature/
--rw-rw-rw-   0        0        0     1340 2023-03-24 06:18:07.000000 usda-0.0.24/src/usda/pattern_signature/__init__.py
--rw-rw-rw-   0        0        0     5975 2023-02-12 02:57:51.000000 usda-0.0.24/src/usda/pattern_signature/_distance_metric.py
--rw-rw-rw-   0        0        0     1182 2023-02-09 14:05:16.000000 usda-0.0.24/src/usda/pattern_signature/_grid_neighbors_xy_finder.py
--rw-rw-rw-   0        0        0     8778 2023-02-19 14:00:29.000000 usda-0.0.24/src/usda/pattern_signature/_img_region_growing.py
--rw-rw-rw-   0        0        0    20197 2023-02-19 13:21:56.000000 usda-0.0.24/src/usda/pattern_signature/_pattern_module.py
--rw-rw-rw-   0        0        0     7729 2023-03-24 07:51:30.000000 usda-0.0.24/src/usda/pattern_signature/_signature.py
--rw-rw-rw-   0        0        0     3191 2023-02-12 09:54:49.000000 usda-0.0.24/src/usda/pattern_signature/_signature2distance_integration.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:34.167497 usda-0.0.24/src/usda/pgm/
--rw-rw-rw-   0        0        0     3024 2023-06-08 14:28:48.000000 usda-0.0.24/src/usda/pgm/_MRF.py
--rw-rw-rw-   0        0        0     6429 2023-06-12 05:30:15.000000 usda-0.0.24/src/usda/pgm/_MRF_urban_cooling.py
--rw-rw-rw-   0        0        0     1374 2023-06-10 12:20:49.000000 usda-0.0.24/src/usda/pgm/__init__.py
--rw-rw-rw-   0        0        0     4688 2023-06-09 02:45:56.000000 usda-0.0.24/src/usda/pgm/_image_segmentation_using_mrf.py
--rw-rw-rw-   0        0        0     3817 2023-06-02 07:46:23.000000 usda-0.0.24/src/usda/pgm/_pgm_calculating.py
--rw-rw-rw-   0        0        0      372 2023-05-11 01:14:44.000000 usda-0.0.24/src/usda/pgm/_pgm_conversion.py
--rw-rw-rw-   0        0        0     4763 2023-06-08 02:43:36.000000 usda-0.0.24/src/usda/pgm/_pgm_draw.py
--rw-rw-rw-   0        0        0     1292 2023-05-15 12:25:44.000000 usda-0.0.24/src/usda/pgm/_probability_theory.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:34.188499 usda-0.0.24/src/usda/stats/
--rw-rw-rw-   0        0        0     1045 2023-05-02 13:19:46.000000 usda-0.0.24/src/usda/stats/__init__.py
--rw-rw-rw-   0        0        0     3501 2022-10-20 03:25:19.000000 usda-0.0.24/src/usda/stats/_descriptive_stats.py
--rw-rw-rw-   0        0        0     2233 2022-10-22 02:45:57.000000 usda-0.0.24/src/usda/stats/_kde.py
--rw-rw-rw-   0        0        0      778 2022-10-20 03:57:18.000000 usda-0.0.24/src/usda/stats/_outlier.py
--rw-rw-rw-   0        0        0    10793 2022-10-24 05:19:28.000000 usda-0.0.24/src/usda/stats/_regression.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:34.192498 usda-0.0.24/src/usda/tools/
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:34.212501 usda-0.0.24/src/usda/tools/DL_layers_visualizer/
--rw-rw-rw-   0        0        0     4066 2023-03-29 04:55:10.000000 usda-0.0.24/src/usda/tools/DL_layers_visualizer/0_72.jpg
--rw-rw-rw-   0        0        0    13876 2023-03-29 04:55:11.000000 usda-0.0.24/src/usda/tools/DL_layers_visualizer/0_8.jpg
--rw-rw-rw-   0        0        0     3757 2023-03-29 04:55:13.000000 usda-0.0.24/src/usda/tools/DL_layers_visualizer/0_9.jpg
--rw-rw-rw-   0        0        0     1064 2023-04-08 15:24:36.000000 usda-0.0.24/src/usda/tools/DL_layers_visualizer/DL_layers_visualizer.py
--rw-rw-rw-   0        0        0      199 2023-04-09 05:39:15.000000 usda-0.0.24/src/usda/tools/DL_layers_visualizer/__init__.py
--rw-rw-rw-   0        0        0      232 2023-04-09 05:39:58.000000 usda-0.0.24/src/usda/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:34.251506 usda-0.0.24/src/usda/utils/
--rw-rw-rw-   0        0        0     1190 2023-06-18 03:46:31.000000 usda-0.0.24/src/usda/utils/__init__.py
--rw-rw-rw-   0        0        0     1497 2022-10-17 01:46:32.000000 usda-0.0.24/src/usda/utils/_bunch.py
--rw-rw-rw-   0        0        0     5197 2022-10-18 07:06:26.000000 usda-0.0.24/src/usda/utils/_coordinate_transformation.py
--rw-rw-rw-   0        0        0     3970 2023-02-23 09:40:47.000000 usda-0.0.24/src/usda/utils/_df_process.py
--rw-rw-rw-   0        0        0     2938 2022-10-17 01:57:17.000000 usda-0.0.24/src/usda/utils/_displayable_path.py
--rw-rw-rw-   0        0        0     1857 2022-10-26 01:31:31.000000 usda-0.0.24/src/usda/utils/_file_structure.py
--rw-rw-rw-   0        0        0     4232 2023-06-18 03:45:41.000000 usda-0.0.24/src/usda/utils/_gadgets.py
--rw-rw-rw-   0        0        0      606 2022-10-22 00:35:56.000000 usda-0.0.24/src/usda/utils/_operating_time.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:34.271499 usda-0.0.24/src/usda/weight/
--rw-rw-rw-   0        0        0     1014 2023-03-03 07:14:29.000000 usda-0.0.24/src/usda/weight/__init__.py
--rw-rw-rw-   0        0        0    38486 2023-03-03 07:13:35.000000 usda-0.0.24/src/usda/weight/_decision_rule.py
--rw-rw-rw-   0        0        0     2745 2023-02-23 12:30:34.000000 usda-0.0.24/src/usda/weight/_entropy_weight.py
-drwxrwxrwx   0        0        0        0 2023-07-11 03:35:33.347376 usda-0.0.24/src/usda.egg-info/
--rw-rw-rw-   0        0        0     1563 2023-07-11 03:35:32.000000 usda-0.0.24/src/usda.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    11103 2023-07-11 03:35:33.000000 usda-0.0.24/src/usda.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 03:35:32.000000 usda-0.0.24/src/usda.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-10-16 07:33:50.000000 usda-0.0.24/src/usda.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       55 2023-07-11 03:35:32.000000 usda-0.0.24/src/usda.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-11 03:35:32.000000 usda-0.0.24/src/usda.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:24.044077 usda-0.0.25/
+-rw-rw-rw-   0        0        0     1084 2022-10-07 01:27:44.000000 usda-0.0.25/LICENSE
+-rw-rw-rw-   0        0        0     1563 2023-07-11 03:55:24.044077 usda-0.0.25/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2022-10-24 05:51:49.000000 usda-0.0.25/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-11 03:55:24.044077 usda-0.0.25/setup.cfg
+-rw-rw-rw-   0        0        0     4305 2023-05-21 04:03:07.000000 usda-0.0.25/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:22.786337 usda-0.0.25/src/
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:22.927971 usda-0.0.25/src/usda/
+-rw-rw-rw-   0        0        0      636 2023-07-11 03:55:07.000000 usda-0.0.25/src/usda/__init__.py
+-rw-rw-rw-   0        0        0      731 2022-10-16 01:25:29.000000 usda-0.0.25/src/usda/_min_dependencies.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:23.006130 usda-0.0.25/src/usda/data_process/
+-rw-rw-rw-   0        0        0     1147 2023-03-26 03:42:04.000000 usda-0.0.25/src/usda/data_process/__init__.py
+-rw-rw-rw-   0        0        0     2125 2022-10-22 01:48:58.000000 usda-0.0.25/src/usda/data_process/_geoinfodata_conversion.py
+-rw-rw-rw-   0        0        0    14577 2022-10-28 01:52:51.000000 usda-0.0.25/src/usda/data_process/_image_pixel_sampling_zoom.py
+-rw-rw-rw-   0        0        0     1425 2022-10-31 06:03:57.000000 usda-0.0.25/src/usda/data_process/_kitti_dataprocess.py
+-rw-rw-rw-   0        0        0     2037 2022-10-26 01:37:19.000000 usda-0.0.25/src/usda/data_process/_landsat_dataprocess.py
+-rw-rw-rw-   0        0        0     1854 2023-03-26 07:52:38.000000 usda-0.0.25/src/usda/data_process/_naip_dataprocess.py
+-rw-rw-rw-   0        0        0     6348 2022-10-22 00:18:38.000000 usda-0.0.25/src/usda/data_process/_osm_dataprocess.py
+-rw-rw-rw-   0        0        0     1085 2023-02-11 08:44:30.000000 usda-0.0.25/src/usda/data_process/_raster_dataprocess.py
+-rw-rw-rw-   0        0        0     1332 2022-10-30 06:27:55.000000 usda-0.0.25/src/usda/data_process/_tiler_calculation.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:23.022783 usda-0.0.25/src/usda/data_visual/
+-rw-rw-rw-   0        0        0      304 2023-07-09 12:19:47.000000 usda-0.0.25/src/usda/data_visual/__init__.py
+-rw-rw-rw-   0        0        0      499 2023-05-14 10:52:12.000000 usda-0.0.25/src/usda/data_visual/_plot_style.py
+-rw-rw-rw-   0        0        0     1362 2023-07-09 12:16:31.000000 usda-0.0.25/src/usda/data_visual/_worldcover_plot_style.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:23.148369 usda-0.0.25/src/usda/data_visualization/
+-rw-rw-rw-   0        0        0     3205 2023-05-30 14:40:53.000000 usda-0.0.25/src/usda/data_visualization/__init__.py
+-rw-rw-rw-   0        0        0     5300 2023-02-17 02:29:25.000000 usda-0.0.25/src/usda/data_visualization/_chart_custom.py
+-rw-rw-rw-   0        0        0     3729 2023-05-30 14:40:34.000000 usda-0.0.25/src/usda/data_visualization/_colors.py
+-rw-rw-rw-   0        0        0     3221 2022-10-29 07:58:07.000000 usda-0.0.25/src/usda/data_visualization/_dynamic_streetView_visual_perception.py
+-rw-rw-rw-   0        0        0     3557 2023-02-19 14:47:51.000000 usda-0.0.25/src/usda/data_visualization/_gdf_plot.py
+-rw-rw-rw-   0        0        0      952 2022-10-28 11:19:32.000000 usda-0.0.25/src/usda/data_visualization/_gif_show.py
+-rw-rw-rw-   0        0        0     2347 2022-10-28 06:34:44.000000 usda-0.0.25/src/usda/data_visualization/_graphic_drawing.py
+-rw-rw-rw-   0        0        0     4787 2022-10-31 05:36:51.000000 usda-0.0.25/src/usda/data_visualization/_image_process.py
+-rw-rw-rw-   0        0        0     8500 2022-10-29 06:42:38.000000 usda-0.0.25/src/usda/data_visualization/_img_feature_extraction.py
+-rw-rw-rw-   0        0        0     7196 2022-10-30 12:18:06.000000 usda-0.0.25/src/usda/data_visualization/_img_theme_color.py
+-rw-rw-rw-   0        0        0     2846 2022-10-30 11:18:24.000000 usda-0.0.25/src/usda/data_visualization/_imgs_layout_show.py
+-rw-rw-rw-   0        0        0     4174 2023-03-15 02:00:19.000000 usda-0.0.25/src/usda/data_visualization/_imgs_show.py
+-rw-rw-rw-   0        0        0      822 2022-11-02 06:07:14.000000 usda-0.0.25/src/usda/data_visualization/_knee_line_graph.py
+-rw-rw-rw-   0        0        0     7393 2022-10-29 08:23:53.000000 usda-0.0.25/src/usda/data_visualization/_moving_average_inflection.py
+-rw-rw-rw-   0        0        0     3176 2023-02-24 07:31:39.000000 usda-0.0.25/src/usda/data_visualization/_panorama_show.py
+-rw-rw-rw-   0        0        0     8051 2023-03-19 04:08:53.000000 usda-0.0.25/src/usda/data_visualization/_plot_single_function.py
+-rw-rw-rw-   0        0        0     2310 2022-10-28 01:13:41.000000 usda-0.0.25/src/usda/data_visualization/_raster_percentile_slider.py
+-rw-rw-rw-   0        0        0     1224 2022-10-28 00:45:13.000000 usda-0.0.25/src/usda/data_visualization/_raster_show.py
+-rw-rw-rw-   0        0        0     2130 2022-10-28 06:32:06.000000 usda-0.0.25/src/usda/data_visualization/_stats_charts.py
+-rw-rw-rw-   0        0        0     2666 2022-10-30 07:27:14.000000 usda-0.0.25/src/usda/data_visualization/_superpixel_segmentation_show.py
+-rw-rw-rw-   0        0        0     1577 2022-10-22 23:37:39.000000 usda-0.0.25/src/usda/data_visualization/_table_show.py
+-rw-rw-rw-   0        0        0     1673 2022-11-02 06:07:23.000000 usda-0.0.25/src/usda/data_visualization/_tile_show.py
+-rw-rw-rw-   0        0        0     4464 2020-07-17 02:38:10.000000 usda-0.0.25/src/usda/data_visualization/data_generator.py
+-rw-rw-rw-   0        0        0    10263 2020-07-17 02:38:10.000000 usda-0.0.25/src/usda/data_visualization/knee_locator.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:23.163958 usda-0.0.25/src/usda/database/
+-rw-rw-rw-   0        0        0      839 2023-03-21 05:11:06.000000 usda-0.0.25/src/usda/database/__init__.py
+-rw-rw-rw-   0        0        0      693 2022-10-30 12:15:41.000000 usda-0.0.25/src/usda/database/_data_file_rw.py
+-rw-rw-rw-   0        0        0     4636 2023-03-21 05:10:00.000000 usda-0.0.25/src/usda/database/_data_format_conversion.py
+-rw-rw-rw-   0        0        0     5605 2023-03-21 05:08:27.000000 usda-0.0.25/src/usda/database/_database.py
+-rw-rw-rw-   0        0        0     1384 2022-10-28 08:27:55.000000 usda-0.0.25/src/usda/database/_read_matlab_fig.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:23.195210 usda-0.0.25/src/usda/datasets/
+-rw-rw-rw-   0        0        0     2003 2023-07-09 08:35:22.000000 usda-0.0.25/src/usda/datasets/__init__.py
+-rw-rw-rw-   0        0        0    17136 2023-03-13 12:40:56.000000 usda-0.0.25/src/usda/datasets/_artificial_data.py
+-rw-rw-rw-   0        0        0    19730 2023-03-14 01:14:44.000000 usda-0.0.25/src/usda/datasets/_base.py
+-rw-rw-rw-   0        0        0     2745 2022-10-31 05:44:19.000000 usda-0.0.25/src/usda/datasets/_dataset_info.py
+-rw-rw-rw-   0        0        0     5119 2023-07-09 08:43:54.000000 usda-0.0.25/src/usda/datasets/_files_downloading.py
+-rw-rw-rw-   0        0        0     2681 2022-10-30 11:21:33.000000 usda-0.0.25/src/usda/datasets/_img_info.py
+-rw-rw-rw-   0        0        0     2806 2022-10-30 10:50:28.000000 usda-0.0.25/src/usda/datasets/_kml_info.py
+-rw-rw-rw-   0        0        0     1547 2022-10-30 07:02:03.000000 usda-0.0.25/src/usda/datasets/_rs_image.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:23.242568 usda-0.0.25/src/usda/datasets/data/
+-rw-rw-rw-   0        0        0      125 2022-08-21 07:11:20.000000 usda-0.0.25/src/usda/datasets/data/__init__.py
+-rw-rw-rw-   0        0        0     1224 2022-10-19 04:41:26.000000 usda-0.0.25/src/usda/datasets/data/bowling_contest_cartoon_statistic.pickle
+-rw-rw-rw-   0        0        0      950 2023-02-23 02:44:29.000000 usda-0.0.25/src/usda/datasets/data/evaluation_criteria_raw_values.pickle
+-rw-rw-rw-   0        0        0     8356 2023-03-13 12:16:36.000000 usda-0.0.25/src/usda/datasets/data/jisperveld_data.pickle
+-rw-rw-rw-   0        0        0     1486 2023-02-27 14:21:28.000000 usda-0.0.25/src/usda/datasets/data/microclimate_in_office_rooms.pickle
+-rw-rw-rw-   0        0        0     1089 2022-10-19 01:41:55.000000 usda-0.0.25/src/usda/datasets/data/ramen_price_cartoon_statistic.pickle
+-rw-rw-rw-   0        0        0     2123 2022-10-15 01:16:56.000000 usda-0.0.25/src/usda/datasets/data/sales_data_cartoon_database.pickle
+-rw-rw-rw-   0        0        0     1352 2023-02-24 07:53:38.000000 usda-0.0.25/src/usda/datasets/data/sustainability_attributes4electricity_generation_tech.pickle
+-rw-rw-rw-   0        0        0     1340 2022-10-19 05:00:19.000000 usda-0.0.25/src/usda/datasets/data/test_score_cartoon_statistic.pickle
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:23.289483 usda-0.0.25/src/usda/geodata_process/
+-rw-rw-rw-   0        0        0     1932 2023-07-10 10:21:46.000000 usda-0.0.25/src/usda/geodata_process/__init__.py
+-rw-rw-rw-   0        0        0     2906 2023-07-10 11:42:14.000000 usda-0.0.25/src/usda/geodata_process/_build_clipped_raster_dataset.py
+-rw-rw-rw-   0        0        0     1197 2023-07-10 09:55:02.000000 usda-0.0.25/src/usda/geodata_process/_build_clipped_raster_dataset_pool.py
+-rw-rw-rw-   0        0        0     6447 2023-07-10 00:45:07.000000 usda-0.0.25/src/usda/geodata_process/_quadrat.py
+-rw-rw-rw-   0        0        0     6535 2023-03-22 16:40:23.000000 usda-0.0.25/src/usda/geodata_process/_raster_dataprocess.py
+-rw-rw-rw-   0        0        0     6633 2023-03-22 14:50:33.000000 usda-0.0.25/src/usda/geodata_process/_raster_stats.py
+-rw-rw-rw-   0        0        0     6661 2023-03-21 13:11:59.000000 usda-0.0.25/src/usda/geodata_process/_rasterize.py
+-rw-rw-rw-   0        0        0     3097 2023-07-07 04:06:42.000000 usda-0.0.25/src/usda/geodata_process/_rio_tiler.py
+-rw-rw-rw-   0        0        0     4952 2023-06-02 02:08:47.000000 usda-0.0.25/src/usda/geodata_process/_sample_pts.py
+-rw-rw-rw-   0        0        0     1040 2023-04-17 23:16:55.000000 usda-0.0.25/src/usda/geodata_process/_shp_dataprocess.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:23.296519 usda-0.0.25/src/usda/imgs_process/
+-rw-rw-rw-   0        0        0      457 2023-06-08 12:42:37.000000 usda-0.0.25/src/usda/imgs_process/__init__.py
+-rw-rw-rw-   0        0        0     2768 2023-06-08 12:45:27.000000 usda-0.0.25/src/usda/imgs_process/_imgs_process_basic.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:23.305549 usda-0.0.25/src/usda/indices/
+-rw-rw-rw-   0        0        0      189 2022-10-26 06:14:56.000000 usda-0.0.25/src/usda/indices/__init__.py
+-rw-rw-rw-   0        0        0      574 2022-10-26 06:15:29.000000 usda-0.0.25/src/usda/indices/_rs_indices.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:23.323737 usda-0.0.25/src/usda/maths/
+-rw-rw-rw-   0        0        0      645 2023-04-11 23:36:35.000000 usda-0.0.25/src/usda/maths/__init__.py
+-rw-rw-rw-   0        0        0     4335 2022-10-26 02:53:02.000000 usda-0.0.25/src/usda/maths/_algebra.py
+-rw-rw-rw-   0        0        0     1519 2022-10-26 03:05:19.000000 usda-0.0.25/src/usda/maths/_geometric_calculation.py
+-rw-rw-rw-   0        0        0     8051 2023-04-11 23:36:06.000000 usda-0.0.25/src/usda/maths/_plot_single_function.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:23.384202 usda-0.0.25/src/usda/meta_heuristics/
+-rw-rw-rw-   0        0        0      843 2023-03-19 01:33:28.000000 usda-0.0.25/src/usda/meta_heuristics/__init__.py
+-rw-rw-rw-   0        0        0     5889 2023-03-18 13:00:33.000000 usda-0.0.25/src/usda/meta_heuristics/_cuckoo_s.py
+-rw-rw-rw-   0        0        0     4919 2023-03-19 01:22:52.000000 usda-0.0.25/src/usda/meta_heuristics/_firefly_a.py
+-rw-rw-rw-   0        0        0    11373 2023-03-10 03:50:42.000000 usda-0.0.25/src/usda/meta_heuristics/_ga.py
+-rw-rw-rw-   0        0        0    13840 2023-03-15 22:13:00.000000 usda-0.0.25/src/usda/meta_heuristics/_ga_2d.py
+-rw-rw-rw-   0        0        0    14213 2023-03-16 01:38:05.000000 usda-0.0.25/src/usda/meta_heuristics/_ga_2d_fixed_map.py
+-rw-rw-rw-   0        0        0    15440 2023-03-15 14:33:57.000000 usda-0.0.25/src/usda/meta_heuristics/_ga_2d_testing_1.py
+-rw-rw-rw-   0        0        0    25287 2023-03-17 02:56:06.000000 usda-0.0.25/src/usda/meta_heuristics/_ga_2d_testing_2.py
+-rw-rw-rw-   0        0        0     4177 2023-03-10 02:05:28.000000 usda-0.0.25/src/usda/meta_heuristics/_ga_SegaranT.py
+-rw-rw-rw-   0        0        0     7982 2023-03-01 00:42:26.000000 usda-0.0.25/src/usda/meta_heuristics/_gwo.py
+-rw-rw-rw-   0        0        0     5251 2023-03-17 04:06:12.000000 usda-0.0.25/src/usda/meta_heuristics/_pso.py
+-rw-rw-rw-   0        0        0     7564 2023-03-18 04:30:41.000000 usda-0.0.25/src/usda/meta_heuristics/_pso_2d.py
+-rw-rw-rw-   0        0        0     8467 2023-03-18 05:15:54.000000 usda-0.0.25/src/usda/meta_heuristics/_pso_2d_testing.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:23.384202 usda-0.0.25/src/usda/migrated_project/
+-rw-rw-rw-   0        0        0      180 2023-04-17 02:04:10.000000 usda-0.0.25/src/usda/migrated_project/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:23.399802 usda-0.0.25/src/usda/migrated_project/invest/
+-rw-rw-rw-   0        0        0      711 2023-06-11 01:34:27.000000 usda-0.0.25/src/usda/migrated_project/invest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:23.431528 usda-0.0.25/src/usda/migrated_project/invest/configs/
+-rw-rw-rw-   0        0        0     1150 2023-06-09 12:59:23.000000 usda-0.0.25/src/usda/migrated_project/invest/configs/__init__.py
+-rw-rw-rw-   0        0        0     1320 2023-05-21 14:16:56.000000 usda-0.0.25/src/usda/migrated_project/invest/configs/_carbon_configs.py
+-rw-rw-rw-   0        0        0     5303 2023-05-22 07:01:13.000000 usda-0.0.25/src/usda/migrated_project/invest/configs/_crop_pollination_configs.py
+-rw-rw-rw-   0        0        0     2352 2023-05-22 09:31:32.000000 usda-0.0.25/src/usda/migrated_project/invest/configs/_crop_production_percentile_configs.py
+-rw-rw-rw-   0        0        0     3674 2023-05-22 08:55:38.000000 usda-0.0.25/src/usda/migrated_project/invest/configs/_crop_production_regression_configs.py
+-rw-rw-rw-   0        0        0      490 2023-05-21 18:26:40.000000 usda-0.0.25/src/usda/migrated_project/invest/configs/_habitat_quality_configs.py
+-rw-rw-rw-   0        0        0      117 2023-06-09 13:00:21.000000 usda-0.0.25/src/usda/migrated_project/invest/configs/_urban_cooling_configs.py
+-rw-rw-rw-   0        0        0     2095 2023-04-29 10:05:57.000000 usda-0.0.25/src/usda/migrated_project/invest/configs/carbon_pools_willamette.csv
+-rw-rw-rw-   0        0        0     1684 2023-05-16 20:54:57.000000 usda-0.0.25/src/usda/migrated_project/invest/configs/unit_definitions.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:23.462811 usda-0.0.25/src/usda/migrated_project/invest/esv/
+-rw-rw-rw-   0        0        0      700 2023-06-09 23:15:32.000000 usda-0.0.25/src/usda/migrated_project/invest/esv/__init__.py
+-rw-rw-rw-   0        0        0    23442 2023-05-31 01:40:43.000000 usda-0.0.25/src/usda/migrated_project/invest/esv/_carbon.py
+-rw-rw-rw-   0        0        0    66377 2023-05-22 12:57:02.000000 usda-0.0.25/src/usda/migrated_project/invest/esv/_crop_pollination.py
+-rw-rw-rw-   0        0        0    37499 2023-05-22 10:16:20.000000 usda-0.0.25/src/usda/migrated_project/invest/esv/_crop_production_percentile.py
+-rw-rw-rw-   0        0        0    43341 2023-05-22 13:20:45.000000 usda-0.0.25/src/usda/migrated_project/invest/esv/_crop_production_regression.py
+-rw-rw-rw-   0        0        0    41477 2023-05-22 12:35:30.000000 usda-0.0.25/src/usda/migrated_project/invest/esv/_habitat_quality.py
+-rw-rw-rw-   0        0        0      610 2023-05-21 04:07:41.000000 usda-0.0.25/src/usda/migrated_project/invest/esv/_unit_registry.py
+-rw-rw-rw-   0        0        0    56182 2023-06-10 02:41:05.000000 usda-0.0.25/src/usda/migrated_project/invest/esv/_urban_cooling_model.py
+-rw-rw-rw-   0        0        0    44236 2023-05-21 14:00:31.000000 usda-0.0.25/src/usda/migrated_project/invest/esv/_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:23.494061 usda-0.0.25/src/usda/migrated_project/pix2pix/
+-rw-rw-rw-   0        0        0     1969 2023-04-20 08:47:17.000000 usda-0.0.25/src/usda/migrated_project/pix2pix/A2B.py
+-rw-rw-rw-   0        0        0      217 2023-04-21 13:54:27.000000 usda-0.0.25/src/usda/migrated_project/pix2pix/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:23.525823 usda-0.0.25/src/usda/migrated_project/pix2pix/data/
+-rw-rw-rw-   0        0        0     4100 2023-04-20 05:37:10.000000 usda-0.0.25/src/usda/migrated_project/pix2pix/data/__init__.py
+-rw-rw-rw-   0        0        0     2728 2023-04-17 06:17:12.000000 usda-0.0.25/src/usda/migrated_project/pix2pix/data/_aligned_dataset.py
+-rw-rw-rw-   0        0        0     6235 2023-04-17 05:52:31.000000 usda-0.0.25/src/usda/migrated_project/pix2pix/data/_base_dataset.py
+-rw-rw-rw-   0        0        0     2897 2023-04-17 06:21:59.000000 usda-0.0.25/src/usda/migrated_project/pix2pix/data/_colorization_dataset.py
+-rw-rw-rw-   0        0        0     1885 2023-03-14 20:28:49.000000 usda-0.0.25/src/usda/migrated_project/pix2pix/data/_image_folder.py
+-rw-rw-rw-   0        0        0     1658 2023-04-17 06:19:58.000000 usda-0.0.25/src/usda/migrated_project/pix2pix/data/_single_dataset.py
+-rw-rw-rw-   0        0        0     3589 2023-04-17 03:48:21.000000 usda-0.0.25/src/usda/migrated_project/pix2pix/data/_template_dataset.py
+-rw-rw-rw-   0        0        0     3526 2023-04-17 05:45:03.000000 usda-0.0.25/src/usda/migrated_project/pix2pix/data/_unaligned_dataset.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:23.525823 usda-0.0.25/src/usda/migrated_project/pix2pix/datasets/
+-rw-rw-rw-   0        0        0      198 2023-04-17 01:54:37.000000 usda-0.0.25/src/usda/migrated_project/pix2pix/datasets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:23.541476 usda-0.0.25/src/usda/migrated_project/pix2pix/imgs/
+-rw-rw-rw-   0        0        0      127 2023-04-21 13:57:19.000000 usda-0.0.25/src/usda/migrated_project/pix2pix/imgs/__init__.py
+-rw-rw-rw-   0        0        0    14064 2023-04-21 14:08:05.000000 usda-0.0.25/src/usda/migrated_project/pix2pix/imgs/example.jpg
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:23.557114 usda-0.0.25/src/usda/migrated_project/pix2pix/models/
+-rw-rw-rw-   0        0        0     3349 2023-04-20 02:44:45.000000 usda-0.0.25/src/usda/migrated_project/pix2pix/models/__init__.py
+-rw-rw-rw-   0        0        0    10810 2023-04-17 07:20:11.000000 usda-0.0.25/src/usda/migrated_project/pix2pix/models/_base_model.py
+-rw-rw-rw-   0        0        0    29098 2023-04-17 07:31:07.000000 usda-0.0.25/src/usda/migrated_project/pix2pix/models/_networks.py
+-rw-rw-rw-   0        0        0     7024 2023-04-17 07:21:10.000000 usda-0.0.25/src/usda/migrated_project/pix2pix/models/_pix2pix_model.py
+-rw-rw-rw-   0        0        0     3392 2023-04-17 12:08:31.000000 usda-0.0.25/src/usda/migrated_project/pix2pix/models/_test_model.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:23.572768 usda-0.0.25/src/usda/migrated_project/pix2pix/options/
+-rw-rw-rw-   0        0        0      425 2023-04-17 11:42:46.000000 usda-0.0.25/src/usda/migrated_project/pix2pix/options/__init__.py
+-rw-rw-rw-   0        0        0     3447 2023-04-17 08:10:06.000000 usda-0.0.25/src/usda/migrated_project/pix2pix/options/_base_options.py
+-rw-rw-rw-   0        0        0     1045 2023-04-17 12:42:33.000000 usda-0.0.25/src/usda/migrated_project/pix2pix/options/_test_options.py
+-rw-rw-rw-   0        0        0     2533 2023-04-17 11:39:45.000000 usda-0.0.25/src/usda/migrated_project/pix2pix/options/_train_options.py
+-rw-rw-rw-   0        0        0     8846 2023-04-22 00:58:18.000000 usda-0.0.25/src/usda/migrated_project/pix2pix/sketch_A2B.py
+-rw-rw-rw-   0        0        0     6019 2023-04-17 13:04:35.000000 usda-0.0.25/src/usda/migrated_project/pix2pix/test.py
+-rw-rw-rw-   0        0        0     6788 2023-04-18 09:54:15.000000 usda-0.0.25/src/usda/migrated_project/pix2pix/train.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:23.604016 usda-0.0.25/src/usda/migrated_project/pix2pix/util/
+-rw-rw-rw-   0        0        0      270 2023-04-17 11:51:19.000000 usda-0.0.25/src/usda/migrated_project/pix2pix/util/__init__.py
+-rw-rw-rw-   0        0        0     3639 2023-03-14 20:28:49.000000 usda-0.0.25/src/usda/migrated_project/pix2pix/util/_get_data.py
+-rw-rw-rw-   0        0        0     3223 2023-03-14 20:28:49.000000 usda-0.0.25/src/usda/migrated_project/pix2pix/util/_html.py
+-rw-rw-rw-   0        0        0     2226 2023-03-14 20:28:49.000000 usda-0.0.25/src/usda/migrated_project/pix2pix/util/_image_pool.py
+-rw-rw-rw-   0        0        0     3175 2023-03-14 20:28:49.000000 usda-0.0.25/src/usda/migrated_project/pix2pix/util/_util.py
+-rw-rw-rw-   0        0        0    12408 2023-04-17 09:41:44.000000 usda-0.0.25/src/usda/migrated_project/pix2pix/util/_visualizer.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:23.624172 usda-0.0.25/src/usda/migrated_project/stylegan/
+-rw-rw-rw-   0        0        0      898 2023-04-17 10:27:41.000000 usda-0.0.25/src/usda/migrated_project/stylegan/__init__.py
+-rw-rw-rw-   0        0        0     3082 2023-04-16 06:09:08.000000 usda-0.0.25/src/usda/migrated_project/stylegan/_config.py
+-rw-rw-rw-   0        0        0     4425 2023-04-11 12:13:43.000000 usda-0.0.25/src/usda/migrated_project/stylegan/_convert.py
+-rw-rw-rw-   0        0        0     3527 2023-04-11 12:16:24.000000 usda-0.0.25/src/usda/migrated_project/stylegan/_generate_grid.py
+-rw-rw-rw-   0        0        0     5616 2023-04-16 11:14:57.000000 usda-0.0.25/src/usda/migrated_project/stylegan/_generate_mixing_figure.py
+-rw-rw-rw-   0        0        0     4595 2023-04-16 07:34:49.000000 usda-0.0.25/src/usda/migrated_project/stylegan/_generate_samples.py
+-rw-rw-rw-   0        0        0     3430 2023-04-16 08:58:05.000000 usda-0.0.25/src/usda/migrated_project/stylegan/_generate_truncation_figure.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:23.651367 usda-0.0.25/src/usda/migrated_project/stylegan/data/
+-rw-rw-rw-   0        0        0      558 2023-04-11 11:18:10.000000 usda-0.0.25/src/usda/migrated_project/stylegan/data/__init__.py
+-rw-rw-rw-   0        0        0     4744 2023-04-11 10:36:07.000000 usda-0.0.25/src/usda/migrated_project/stylegan/data/_datasets.py
+-rw-rw-rw-   0        0        0     1457 2023-04-11 10:36:54.000000 usda-0.0.25/src/usda/migrated_project/stylegan/data/_make_dataset.py
+-rw-rw-rw-   0        0        0     1014 2023-04-11 10:37:15.000000 usda-0.0.25/src/usda/migrated_project/stylegan/data/_transforms.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:23.651367 usda-0.0.25/src/usda/migrated_project/stylegan/dnnlib/
+-rw-rw-rw-   0        0        0      799 2021-12-18 03:07:03.000000 usda-0.0.25/src/usda/migrated_project/stylegan/dnnlib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:23.666992 usda-0.0.25/src/usda/migrated_project/stylegan/dnnlib/submission/
+-rw-rw-rw-   0        0        0      392 2021-12-18 03:07:03.000000 usda-0.0.25/src/usda/migrated_project/stylegan/dnnlib/submission/__init__.py
+-rw-rw-rw-   0        0        0     4337 2021-12-18 03:07:03.000000 usda-0.0.25/src/usda/migrated_project/stylegan/dnnlib/submission/run_context.py
+-rw-rw-rw-   0        0        0    11131 2021-12-18 03:07:03.000000 usda-0.0.25/src/usda/migrated_project/stylegan/dnnlib/submission/submit.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:23.682618 usda-0.0.25/src/usda/migrated_project/stylegan/dnnlib/tflib/
+-rw-rw-rw-   0        0        0      524 2021-12-18 03:07:03.000000 usda-0.0.25/src/usda/migrated_project/stylegan/dnnlib/tflib/__init__.py
+-rw-rw-rw-   0        0        0     7537 2021-12-18 03:07:03.000000 usda-0.0.25/src/usda/migrated_project/stylegan/dnnlib/tflib/autosummary.py
+-rw-rw-rw-   0        0        0    30121 2021-12-18 03:07:03.000000 usda-0.0.25/src/usda/migrated_project/stylegan/dnnlib/tflib/network.py
+-rw-rw-rw-   0        0        0    10027 2021-12-18 03:07:03.000000 usda-0.0.25/src/usda/migrated_project/stylegan/dnnlib/tflib/optimizer.py
+-rw-rw-rw-   0        0        0     9306 2023-04-11 12:36:18.000000 usda-0.0.25/src/usda/migrated_project/stylegan/dnnlib/tflib/tfutil.py
+-rw-rw-rw-   0        0        0    13756 2021-12-18 03:07:03.000000 usda-0.0.25/src/usda/migrated_project/stylegan/dnnlib/util.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:23.698249 usda-0.0.25/src/usda/migrated_project/stylegan/extracted_funcs/
+-rw-rw-rw-   0        0        0      186 2023-04-12 06:22:03.000000 usda-0.0.25/src/usda/migrated_project/stylegan/extracted_funcs/__init__.py
+-rw-rw-rw-   0        0        0     1354 2023-04-12 06:27:22.000000 usda-0.0.25/src/usda/migrated_project/stylegan/extracted_funcs/_gadgets.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:23.724424 usda-0.0.25/src/usda/migrated_project/stylegan/models/
+-rw-rw-rw-   0        0        0     6331 2023-04-11 11:53:57.000000 usda-0.0.25/src/usda/migrated_project/stylegan/models/_Blocks.py
+-rw-rw-rw-   0        0        0    11748 2023-04-11 11:32:52.000000 usda-0.0.25/src/usda/migrated_project/stylegan/models/_CustomLayers.py
+-rw-rw-rw-   0        0        0    38792 2023-04-11 11:52:55.000000 usda-0.0.25/src/usda/migrated_project/stylegan/models/_GAN.py
+-rw-rw-rw-   0        0        0     8277 2023-04-11 11:27:22.000000 usda-0.0.25/src/usda/migrated_project/stylegan/models/_Losses.py
+-rw-rw-rw-   0        0        0     1771 2023-04-11 11:56:27.000000 usda-0.0.25/src/usda/migrated_project/stylegan/models/__init__.py
+-rw-rw-rw-   0        0        0     1388 2023-04-11 11:40:43.000000 usda-0.0.25/src/usda/migrated_project/stylegan/models/_update_average.py
+-rw-rw-rw-   0        0        0     6150 2023-04-17 03:27:42.000000 usda-0.0.25/src/usda/migrated_project/stylegan/train.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:23.745664 usda-0.0.25/src/usda/migrated_project/stylegan/utils/
+-rw-rw-rw-   0        0        0      247 2023-04-11 07:34:41.000000 usda-0.0.25/src/usda/migrated_project/stylegan/utils/__init__.py
+-rw-rw-rw-   0        0        0     2159 2023-04-11 09:44:25.000000 usda-0.0.25/src/usda/migrated_project/stylegan/utils/_copy.py
+-rw-rw-rw-   0        0        0      685 2023-04-11 10:33:56.000000 usda-0.0.25/src/usda/migrated_project/stylegan/utils/_logger.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:23.824789 usda-0.0.25/src/usda/models/
+-rw-rw-rw-   0        0        0     5058 2023-07-02 05:03:24.000000 usda-0.0.25/src/usda/models/__init__.py
+-rw-rw-rw-   0        0        0     3873 2022-10-31 06:56:19.000000 usda-0.0.25/src/usda/models/_bow_feature_builder.py
+-rw-rw-rw-   0        0        0     1014 2023-03-24 02:28:49.000000 usda-0.0.25/src/usda/models/_clustering.py
+-rw-rw-rw-   0        0        0     3105 2022-10-25 01:59:30.000000 usda-0.0.25/src/usda/models/_computational_performance.py
+-rw-rw-rw-   0        0        0     1897 2022-10-28 08:34:08.000000 usda-0.0.25/src/usda/models/_curve_segmentation.py
+-rw-rw-rw-   0        0        0     3928 2022-10-31 07:59:05.000000 usda-0.0.25/src/usda/models/_decision_tree.py
+-rw-rw-rw-   0        0        0     5811 2022-10-28 08:15:41.000000 usda-0.0.25/src/usda/models/_dim1_convolution.py
+-rw-rw-rw-   0        0        0     2676 2022-10-31 07:41:49.000000 usda-0.0.25/src/usda/models/_entropy.py
+-rw-rw-rw-   0        0        0     1458 2023-03-24 10:49:05.000000 usda-0.0.25/src/usda/models/_global_local_autocorrelation.py
+-rw-rw-rw-   0        0        0     1427 2022-11-02 06:11:04.000000 usda-0.0.25/src/usda/models/_image_tag_extractor.py
+-rw-rw-rw-   0        0        0     2087 2023-06-21 23:53:49.000000 usda-0.0.25/src/usda/models/_label_encoder.py
+-rw-rw-rw-   0        0        0     1022 2022-10-25 01:02:56.000000 usda-0.0.25/src/usda/models/_neighbors.py
+-rw-rw-rw-   0        0        0     9967 2023-06-30 10:21:03.000000 usda-0.0.25/src/usda/models/_nlp_tools.py
+-rw-rw-rw-   0        0        0     1422 2022-10-31 08:30:25.000000 usda-0.0.25/src/usda/models/_random_forest_classifier.py
+-rw-rw-rw-   0        0        0     9501 2023-06-22 03:39:31.000000 usda-0.0.25/src/usda/models/_rnn_lstm.py
+-rw-rw-rw-   0        0        0    16007 2023-06-30 12:22:03.000000 usda-0.0.25/src/usda/models/_seq2seq.py
+-rw-rw-rw-   0        0        0    11923 2022-10-28 11:44:45.000000 usda-0.0.25/src/usda/models/_sir_model.py
+-rw-rw-rw-   0        0        0     3200 2022-10-30 07:33:05.000000 usda-0.0.25/src/usda/models/_superpixel_segmentation.py
+-rw-rw-rw-   0        0        0     9756 2023-07-01 03:01:16.000000 usda-0.0.25/src/usda/models/_transformer.py
+-rw-rw-rw-   0        0        0     8564 2023-07-11 03:52:36.000000 usda-0.0.25/src/usda/models/_vit.py
+-rw-rw-rw-   0        0        0     9313 2023-06-27 08:00:23.000000 usda-0.0.25/src/usda/models/_word2vec_sgns.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:23.839820 usda-0.0.25/src/usda/net/
+-rw-rw-rw-   0        0        0      120 2023-04-05 02:07:48.000000 usda-0.0.25/src/usda/net/_.py
+-rw-rw-rw-   0        0        0      856 2023-04-05 02:18:09.000000 usda-0.0.25/src/usda/net/__init__.py
+-rw-rw-rw-   0        0        0    28490 2023-04-05 02:16:39.000000 usda-0.0.25/src/usda/net/_networks_pix2pix.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:23.855483 usda-0.0.25/src/usda/network/
+-rw-rw-rw-   0        0        0      404 2023-04-01 07:37:21.000000 usda-0.0.25/src/usda/network/__init__.py
+-rw-rw-rw-   0        0        0     4050 2023-03-10 11:37:13.000000 usda-0.0.25/src/usda/network/_g_drawing.py
+-rw-rw-rw-   0        0        0     2896 2023-04-01 07:46:50.000000 usda-0.0.25/src/usda/network/_pt_pattern.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:23.886736 usda-0.0.25/src/usda/pattern_signature/
+-rw-rw-rw-   0        0        0     1340 2023-03-24 06:18:07.000000 usda-0.0.25/src/usda/pattern_signature/__init__.py
+-rw-rw-rw-   0        0        0     5975 2023-02-12 02:57:51.000000 usda-0.0.25/src/usda/pattern_signature/_distance_metric.py
+-rw-rw-rw-   0        0        0     1182 2023-02-09 14:05:16.000000 usda-0.0.25/src/usda/pattern_signature/_grid_neighbors_xy_finder.py
+-rw-rw-rw-   0        0        0     8778 2023-02-19 14:00:29.000000 usda-0.0.25/src/usda/pattern_signature/_img_region_growing.py
+-rw-rw-rw-   0        0        0    20197 2023-02-19 13:21:56.000000 usda-0.0.25/src/usda/pattern_signature/_pattern_module.py
+-rw-rw-rw-   0        0        0     7729 2023-03-24 07:51:30.000000 usda-0.0.25/src/usda/pattern_signature/_signature.py
+-rw-rw-rw-   0        0        0     3191 2023-02-12 09:54:49.000000 usda-0.0.25/src/usda/pattern_signature/_signature2distance_integration.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:23.925023 usda-0.0.25/src/usda/pgm/
+-rw-rw-rw-   0        0        0     3024 2023-06-08 14:28:48.000000 usda-0.0.25/src/usda/pgm/_MRF.py
+-rw-rw-rw-   0        0        0     6429 2023-06-12 05:30:15.000000 usda-0.0.25/src/usda/pgm/_MRF_urban_cooling.py
+-rw-rw-rw-   0        0        0     1374 2023-06-10 12:20:49.000000 usda-0.0.25/src/usda/pgm/__init__.py
+-rw-rw-rw-   0        0        0     4688 2023-06-09 02:45:56.000000 usda-0.0.25/src/usda/pgm/_image_segmentation_using_mrf.py
+-rw-rw-rw-   0        0        0     3817 2023-06-02 07:46:23.000000 usda-0.0.25/src/usda/pgm/_pgm_calculating.py
+-rw-rw-rw-   0        0        0      372 2023-05-11 01:14:44.000000 usda-0.0.25/src/usda/pgm/_pgm_conversion.py
+-rw-rw-rw-   0        0        0     4763 2023-06-08 02:43:36.000000 usda-0.0.25/src/usda/pgm/_pgm_draw.py
+-rw-rw-rw-   0        0        0     1292 2023-05-15 12:25:44.000000 usda-0.0.25/src/usda/pgm/_probability_theory.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:23.949753 usda-0.0.25/src/usda/stats/
+-rw-rw-rw-   0        0        0     1045 2023-05-02 13:19:46.000000 usda-0.0.25/src/usda/stats/__init__.py
+-rw-rw-rw-   0        0        0     3501 2022-10-20 03:25:19.000000 usda-0.0.25/src/usda/stats/_descriptive_stats.py
+-rw-rw-rw-   0        0        0     2233 2022-10-22 02:45:57.000000 usda-0.0.25/src/usda/stats/_kde.py
+-rw-rw-rw-   0        0        0      778 2022-10-20 03:57:18.000000 usda-0.0.25/src/usda/stats/_outlier.py
+-rw-rw-rw-   0        0        0    10793 2022-10-24 05:19:28.000000 usda-0.0.25/src/usda/stats/_regression.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:23.949753 usda-0.0.25/src/usda/tools/
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:23.981011 usda-0.0.25/src/usda/tools/DL_layers_visualizer/
+-rw-rw-rw-   0        0        0     4066 2023-03-29 04:55:10.000000 usda-0.0.25/src/usda/tools/DL_layers_visualizer/0_72.jpg
+-rw-rw-rw-   0        0        0    13876 2023-03-29 04:55:11.000000 usda-0.0.25/src/usda/tools/DL_layers_visualizer/0_8.jpg
+-rw-rw-rw-   0        0        0     3757 2023-03-29 04:55:13.000000 usda-0.0.25/src/usda/tools/DL_layers_visualizer/0_9.jpg
+-rw-rw-rw-   0        0        0     1064 2023-04-08 15:24:36.000000 usda-0.0.25/src/usda/tools/DL_layers_visualizer/DL_layers_visualizer.py
+-rw-rw-rw-   0        0        0      199 2023-04-09 05:39:15.000000 usda-0.0.25/src/usda/tools/DL_layers_visualizer/__init__.py
+-rw-rw-rw-   0        0        0      232 2023-04-09 05:39:58.000000 usda-0.0.25/src/usda/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:24.028408 usda-0.0.25/src/usda/utils/
+-rw-rw-rw-   0        0        0     1190 2023-06-18 03:46:31.000000 usda-0.0.25/src/usda/utils/__init__.py
+-rw-rw-rw-   0        0        0     1497 2022-10-17 01:46:32.000000 usda-0.0.25/src/usda/utils/_bunch.py
+-rw-rw-rw-   0        0        0     5197 2022-10-18 07:06:26.000000 usda-0.0.25/src/usda/utils/_coordinate_transformation.py
+-rw-rw-rw-   0        0        0     3970 2023-02-23 09:40:47.000000 usda-0.0.25/src/usda/utils/_df_process.py
+-rw-rw-rw-   0        0        0     2938 2022-10-17 01:57:17.000000 usda-0.0.25/src/usda/utils/_displayable_path.py
+-rw-rw-rw-   0        0        0     1857 2022-10-26 01:31:31.000000 usda-0.0.25/src/usda/utils/_file_structure.py
+-rw-rw-rw-   0        0        0     4232 2023-06-18 03:45:41.000000 usda-0.0.25/src/usda/utils/_gadgets.py
+-rw-rw-rw-   0        0        0      606 2022-10-22 00:35:56.000000 usda-0.0.25/src/usda/utils/_operating_time.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:24.028408 usda-0.0.25/src/usda/weight/
+-rw-rw-rw-   0        0        0     1014 2023-03-03 07:14:29.000000 usda-0.0.25/src/usda/weight/__init__.py
+-rw-rw-rw-   0        0        0    38486 2023-03-03 07:13:35.000000 usda-0.0.25/src/usda/weight/_decision_rule.py
+-rw-rw-rw-   0        0        0     2745 2023-02-23 12:30:34.000000 usda-0.0.25/src/usda/weight/_entropy_weight.py
+drwxrwxrwx   0        0        0        0 2023-07-11 03:55:22.959251 usda-0.0.25/src/usda.egg-info/
+-rw-rw-rw-   0        0        0     1563 2023-07-11 03:55:22.000000 usda-0.0.25/src/usda.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    11103 2023-07-11 03:55:22.000000 usda-0.0.25/src/usda.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 03:55:22.000000 usda-0.0.25/src/usda.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-10-16 07:33:50.000000 usda-0.0.25/src/usda.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       55 2023-07-11 03:55:22.000000 usda-0.0.25/src/usda.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-11 03:55:22.000000 usda-0.0.25/src/usda.egg-info/top_level.txt
```

### Comparing `usda-0.0.24/LICENSE` & `usda-0.0.25/LICENSE`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/PKG-INFO` & `usda-0.0.25/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usda
-Version: 0.0.24
+Version: 0.0.25
 Summary: A set of python modules for Urban Spatial Data Analysis Method (USDA)
 Home-page: https://richiebao.github.io/USDA_PyPI
 Download-URL: https://github.com/richieBao/USDA_PyPI
 Maintainer: Richie Bao
 Maintainer-email: richiebao@outlook.com
 License: new BSD
 Project-URL: Documentation, https://richiebao.github.io/USDA_PyPI
```

### Comparing `usda-0.0.24/setup.py` & `usda-0.0.25/setup.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/__init__.py` & `usda-0.0.25/src/usda/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Created on Sun Aug 21 15:11:00 2022
 
 @author: Richie Bao-caDesign设计(cadesign.cn)
 
 python setup.py sdist
 twine upload dist/usda-0.0.22.tar.gz
 """
-__version__ = "0.0.24"
+__version__ = "0.0.25"
 
 __all__ = [
     "data_process"
     "datasets",
     "database",
     "utils",
     "data_visualization",
```

### Comparing `usda-0.0.24/src/usda/_min_dependencies.py` & `usda-0.0.25/src/usda/_min_dependencies.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/data_process/__init__.py` & `usda-0.0.25/src/usda/data_process/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/data_process/_geoinfodata_conversion.py` & `usda-0.0.25/src/usda/data_process/_geoinfodata_conversion.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/data_process/_image_pixel_sampling_zoom.py` & `usda-0.0.25/src/usda/data_process/_image_pixel_sampling_zoom.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/data_process/_kitti_dataprocess.py` & `usda-0.0.25/src/usda/data_process/_kitti_dataprocess.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/data_process/_landsat_dataprocess.py` & `usda-0.0.25/src/usda/data_process/_landsat_dataprocess.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/data_process/_naip_dataprocess.py` & `usda-0.0.25/src/usda/data_process/_naip_dataprocess.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/data_process/_osm_dataprocess.py` & `usda-0.0.25/src/usda/data_process/_osm_dataprocess.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/data_process/_raster_dataprocess.py` & `usda-0.0.25/src/usda/data_process/_raster_dataprocess.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/data_process/_tiler_calculation.py` & `usda-0.0.25/src/usda/data_process/_tiler_calculation.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/data_visual/_worldcover_plot_style.py` & `usda-0.0.25/src/usda/data_visual/_worldcover_plot_style.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/data_visualization/__init__.py` & `usda-0.0.25/src/usda/data_visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/data_visualization/_chart_custom.py` & `usda-0.0.25/src/usda/data_visualization/_chart_custom.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/data_visualization/_colors.py` & `usda-0.0.25/src/usda/data_visualization/_colors.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/data_visualization/_dynamic_streetView_visual_perception.py` & `usda-0.0.25/src/usda/data_visualization/_dynamic_streetView_visual_perception.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/data_visualization/_gdf_plot.py` & `usda-0.0.25/src/usda/data_visualization/_gdf_plot.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/data_visualization/_gif_show.py` & `usda-0.0.25/src/usda/data_visualization/_gif_show.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/data_visualization/_graphic_drawing.py` & `usda-0.0.25/src/usda/data_visualization/_graphic_drawing.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/data_visualization/_image_process.py` & `usda-0.0.25/src/usda/data_visualization/_image_process.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/data_visualization/_img_feature_extraction.py` & `usda-0.0.25/src/usda/data_visualization/_img_feature_extraction.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/data_visualization/_img_theme_color.py` & `usda-0.0.25/src/usda/data_visualization/_img_theme_color.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/data_visualization/_imgs_layout_show.py` & `usda-0.0.25/src/usda/data_visualization/_imgs_layout_show.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/data_visualization/_imgs_show.py` & `usda-0.0.25/src/usda/data_visualization/_imgs_show.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/data_visualization/_knee_line_graph.py` & `usda-0.0.25/src/usda/data_visualization/_knee_line_graph.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/data_visualization/_moving_average_inflection.py` & `usda-0.0.25/src/usda/data_visualization/_moving_average_inflection.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/data_visualization/_panorama_show.py` & `usda-0.0.25/src/usda/data_visualization/_panorama_show.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/data_visualization/_plot_single_function.py` & `usda-0.0.25/src/usda/data_visualization/_plot_single_function.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/data_visualization/_raster_percentile_slider.py` & `usda-0.0.25/src/usda/data_visualization/_raster_percentile_slider.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/data_visualization/_raster_show.py` & `usda-0.0.25/src/usda/data_visualization/_raster_show.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/data_visualization/_stats_charts.py` & `usda-0.0.25/src/usda/data_visualization/_stats_charts.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/data_visualization/_superpixel_segmentation_show.py` & `usda-0.0.25/src/usda/data_visualization/_superpixel_segmentation_show.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/data_visualization/_table_show.py` & `usda-0.0.25/src/usda/data_visualization/_table_show.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/data_visualization/_tile_show.py` & `usda-0.0.25/src/usda/data_visualization/_tile_show.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/data_visualization/data_generator.py` & `usda-0.0.25/src/usda/data_visualization/data_generator.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/data_visualization/knee_locator.py` & `usda-0.0.25/src/usda/data_visualization/knee_locator.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/database/__init__.py` & `usda-0.0.25/src/usda/database/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/database/_data_file_rw.py` & `usda-0.0.25/src/usda/database/_data_file_rw.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/database/_data_format_conversion.py` & `usda-0.0.25/src/usda/database/_data_format_conversion.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/database/_database.py` & `usda-0.0.25/src/usda/database/_database.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/database/_read_matlab_fig.py` & `usda-0.0.25/src/usda/database/_read_matlab_fig.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/datasets/__init__.py` & `usda-0.0.25/src/usda/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/datasets/_artificial_data.py` & `usda-0.0.25/src/usda/datasets/_artificial_data.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/datasets/_base.py` & `usda-0.0.25/src/usda/datasets/_base.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/datasets/_dataset_info.py` & `usda-0.0.25/src/usda/datasets/_dataset_info.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/datasets/_files_downloading.py` & `usda-0.0.25/src/usda/datasets/_files_downloading.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/datasets/_img_info.py` & `usda-0.0.25/src/usda/datasets/_img_info.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/datasets/_kml_info.py` & `usda-0.0.25/src/usda/datasets/_kml_info.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/datasets/_rs_image.py` & `usda-0.0.25/src/usda/datasets/_rs_image.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/datasets/data/bowling_contest_cartoon_statistic.pickle` & `usda-0.0.25/src/usda/datasets/data/bowling_contest_cartoon_statistic.pickle`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/datasets/data/evaluation_criteria_raw_values.pickle` & `usda-0.0.25/src/usda/datasets/data/evaluation_criteria_raw_values.pickle`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/datasets/data/jisperveld_data.pickle` & `usda-0.0.25/src/usda/datasets/data/jisperveld_data.pickle`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/datasets/data/microclimate_in_office_rooms.pickle` & `usda-0.0.25/src/usda/datasets/data/microclimate_in_office_rooms.pickle`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/datasets/data/ramen_price_cartoon_statistic.pickle` & `usda-0.0.25/src/usda/datasets/data/ramen_price_cartoon_statistic.pickle`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/datasets/data/sales_data_cartoon_database.pickle` & `usda-0.0.25/src/usda/datasets/data/sales_data_cartoon_database.pickle`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/datasets/data/sustainability_attributes4electricity_generation_tech.pickle` & `usda-0.0.25/src/usda/datasets/data/sustainability_attributes4electricity_generation_tech.pickle`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/datasets/data/test_score_cartoon_statistic.pickle` & `usda-0.0.25/src/usda/datasets/data/test_score_cartoon_statistic.pickle`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/geodata_process/__init__.py` & `usda-0.0.25/src/usda/geodata_process/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/geodata_process/_build_clipped_raster_dataset.py` & `usda-0.0.25/src/usda/geodata_process/_build_clipped_raster_dataset.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/geodata_process/_build_clipped_raster_dataset_pool.py` & `usda-0.0.25/src/usda/geodata_process/_build_clipped_raster_dataset_pool.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/geodata_process/_quadrat.py` & `usda-0.0.25/src/usda/geodata_process/_quadrat.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/geodata_process/_raster_dataprocess.py` & `usda-0.0.25/src/usda/geodata_process/_raster_dataprocess.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/geodata_process/_raster_stats.py` & `usda-0.0.25/src/usda/geodata_process/_raster_stats.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/geodata_process/_rasterize.py` & `usda-0.0.25/src/usda/geodata_process/_rasterize.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/geodata_process/_rio_tiler.py` & `usda-0.0.25/src/usda/geodata_process/_rio_tiler.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/geodata_process/_sample_pts.py` & `usda-0.0.25/src/usda/geodata_process/_sample_pts.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/geodata_process/_shp_dataprocess.py` & `usda-0.0.25/src/usda/geodata_process/_shp_dataprocess.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/imgs_process/_imgs_process_basic.py` & `usda-0.0.25/src/usda/imgs_process/_imgs_process_basic.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/indices/_rs_indices.py` & `usda-0.0.25/src/usda/indices/_rs_indices.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/maths/__init__.py` & `usda-0.0.25/src/usda/maths/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/maths/_algebra.py` & `usda-0.0.25/src/usda/maths/_algebra.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/maths/_geometric_calculation.py` & `usda-0.0.25/src/usda/maths/_geometric_calculation.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/maths/_plot_single_function.py` & `usda-0.0.25/src/usda/maths/_plot_single_function.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/meta_heuristics/__init__.py` & `usda-0.0.25/src/usda/meta_heuristics/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/meta_heuristics/_cuckoo_s.py` & `usda-0.0.25/src/usda/meta_heuristics/_cuckoo_s.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/meta_heuristics/_firefly_a.py` & `usda-0.0.25/src/usda/meta_heuristics/_firefly_a.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/meta_heuristics/_ga.py` & `usda-0.0.25/src/usda/meta_heuristics/_ga.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/meta_heuristics/_ga_2d.py` & `usda-0.0.25/src/usda/meta_heuristics/_ga_2d.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/meta_heuristics/_ga_2d_fixed_map.py` & `usda-0.0.25/src/usda/meta_heuristics/_ga_2d_fixed_map.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/meta_heuristics/_ga_2d_testing_1.py` & `usda-0.0.25/src/usda/meta_heuristics/_ga_2d_testing_1.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/meta_heuristics/_ga_2d_testing_2.py` & `usda-0.0.25/src/usda/meta_heuristics/_ga_2d_testing_2.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/meta_heuristics/_ga_SegaranT.py` & `usda-0.0.25/src/usda/meta_heuristics/_ga_SegaranT.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/meta_heuristics/_gwo.py` & `usda-0.0.25/src/usda/meta_heuristics/_gwo.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/meta_heuristics/_pso.py` & `usda-0.0.25/src/usda/meta_heuristics/_pso.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/meta_heuristics/_pso_2d.py` & `usda-0.0.25/src/usda/meta_heuristics/_pso_2d.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/meta_heuristics/_pso_2d_testing.py` & `usda-0.0.25/src/usda/meta_heuristics/_pso_2d_testing.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/invest/__init__.py` & `usda-0.0.25/src/usda/migrated_project/invest/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/invest/configs/__init__.py` & `usda-0.0.25/src/usda/migrated_project/invest/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/invest/configs/_carbon_configs.py` & `usda-0.0.25/src/usda/migrated_project/invest/configs/_carbon_configs.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/invest/configs/_crop_pollination_configs.py` & `usda-0.0.25/src/usda/migrated_project/invest/configs/_crop_pollination_configs.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/invest/configs/_crop_production_percentile_configs.py` & `usda-0.0.25/src/usda/migrated_project/invest/configs/_crop_production_percentile_configs.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/invest/configs/_crop_production_regression_configs.py` & `usda-0.0.25/src/usda/migrated_project/invest/configs/_crop_production_regression_configs.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/invest/configs/carbon_pools_willamette.csv` & `usda-0.0.25/src/usda/migrated_project/invest/configs/carbon_pools_willamette.csv`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/invest/configs/unit_definitions.txt` & `usda-0.0.25/src/usda/migrated_project/invest/configs/unit_definitions.txt`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/invest/esv/__init__.py` & `usda-0.0.25/src/usda/migrated_project/invest/esv/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/invest/esv/_carbon.py` & `usda-0.0.25/src/usda/migrated_project/invest/esv/_carbon.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/invest/esv/_crop_pollination.py` & `usda-0.0.25/src/usda/migrated_project/invest/esv/_crop_pollination.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/invest/esv/_crop_production_percentile.py` & `usda-0.0.25/src/usda/migrated_project/invest/esv/_crop_production_percentile.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/invest/esv/_crop_production_regression.py` & `usda-0.0.25/src/usda/migrated_project/invest/esv/_crop_production_regression.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/invest/esv/_habitat_quality.py` & `usda-0.0.25/src/usda/migrated_project/invest/esv/_habitat_quality.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/invest/esv/_unit_registry.py` & `usda-0.0.25/src/usda/migrated_project/invest/esv/_unit_registry.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/invest/esv/_urban_cooling_model.py` & `usda-0.0.25/src/usda/migrated_project/invest/esv/_urban_cooling_model.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/invest/esv/_utils.py` & `usda-0.0.25/src/usda/migrated_project/invest/esv/_utils.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/pix2pix/A2B.py` & `usda-0.0.25/src/usda/migrated_project/pix2pix/A2B.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/pix2pix/data/__init__.py` & `usda-0.0.25/src/usda/migrated_project/pix2pix/data/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/pix2pix/data/_aligned_dataset.py` & `usda-0.0.25/src/usda/migrated_project/pix2pix/data/_aligned_dataset.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/pix2pix/data/_base_dataset.py` & `usda-0.0.25/src/usda/migrated_project/pix2pix/data/_base_dataset.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/pix2pix/data/_colorization_dataset.py` & `usda-0.0.25/src/usda/migrated_project/pix2pix/data/_colorization_dataset.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/pix2pix/data/_image_folder.py` & `usda-0.0.25/src/usda/migrated_project/pix2pix/data/_image_folder.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/pix2pix/data/_single_dataset.py` & `usda-0.0.25/src/usda/migrated_project/pix2pix/data/_single_dataset.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/pix2pix/data/_template_dataset.py` & `usda-0.0.25/src/usda/migrated_project/pix2pix/data/_template_dataset.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/pix2pix/data/_unaligned_dataset.py` & `usda-0.0.25/src/usda/migrated_project/pix2pix/data/_unaligned_dataset.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/pix2pix/imgs/example.jpg` & `usda-0.0.25/src/usda/migrated_project/pix2pix/imgs/example.jpg`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/pix2pix/models/__init__.py` & `usda-0.0.25/src/usda/migrated_project/pix2pix/models/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/pix2pix/models/_base_model.py` & `usda-0.0.25/src/usda/migrated_project/pix2pix/models/_base_model.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/pix2pix/models/_networks.py` & `usda-0.0.25/src/usda/migrated_project/pix2pix/models/_networks.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/pix2pix/models/_pix2pix_model.py` & `usda-0.0.25/src/usda/migrated_project/pix2pix/models/_pix2pix_model.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/pix2pix/models/_test_model.py` & `usda-0.0.25/src/usda/migrated_project/pix2pix/models/_test_model.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/pix2pix/options/_base_options.py` & `usda-0.0.25/src/usda/migrated_project/pix2pix/options/_base_options.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/pix2pix/options/_test_options.py` & `usda-0.0.25/src/usda/migrated_project/pix2pix/options/_test_options.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/pix2pix/options/_train_options.py` & `usda-0.0.25/src/usda/migrated_project/pix2pix/options/_train_options.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/pix2pix/sketch_A2B.py` & `usda-0.0.25/src/usda/migrated_project/pix2pix/sketch_A2B.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/pix2pix/test.py` & `usda-0.0.25/src/usda/migrated_project/pix2pix/test.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/pix2pix/train.py` & `usda-0.0.25/src/usda/migrated_project/pix2pix/train.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/pix2pix/util/_get_data.py` & `usda-0.0.25/src/usda/migrated_project/pix2pix/util/_get_data.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/pix2pix/util/_html.py` & `usda-0.0.25/src/usda/migrated_project/pix2pix/util/_html.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/pix2pix/util/_image_pool.py` & `usda-0.0.25/src/usda/migrated_project/pix2pix/util/_image_pool.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/pix2pix/util/_util.py` & `usda-0.0.25/src/usda/migrated_project/pix2pix/util/_util.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/pix2pix/util/_visualizer.py` & `usda-0.0.25/src/usda/migrated_project/pix2pix/util/_visualizer.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/stylegan/__init__.py` & `usda-0.0.25/src/usda/migrated_project/stylegan/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/stylegan/_config.py` & `usda-0.0.25/src/usda/migrated_project/stylegan/_config.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/stylegan/_convert.py` & `usda-0.0.25/src/usda/migrated_project/stylegan/_convert.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/stylegan/_generate_grid.py` & `usda-0.0.25/src/usda/migrated_project/stylegan/_generate_grid.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/stylegan/_generate_mixing_figure.py` & `usda-0.0.25/src/usda/migrated_project/stylegan/_generate_mixing_figure.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/stylegan/_generate_samples.py` & `usda-0.0.25/src/usda/migrated_project/stylegan/_generate_samples.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/stylegan/_generate_truncation_figure.py` & `usda-0.0.25/src/usda/migrated_project/stylegan/_generate_truncation_figure.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/stylegan/data/__init__.py` & `usda-0.0.25/src/usda/migrated_project/stylegan/data/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/stylegan/data/_datasets.py` & `usda-0.0.25/src/usda/migrated_project/stylegan/data/_datasets.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/stylegan/data/_make_dataset.py` & `usda-0.0.25/src/usda/migrated_project/stylegan/data/_make_dataset.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/stylegan/data/_transforms.py` & `usda-0.0.25/src/usda/migrated_project/stylegan/data/_transforms.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/stylegan/dnnlib/__init__.py` & `usda-0.0.25/src/usda/migrated_project/stylegan/dnnlib/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/stylegan/dnnlib/submission/run_context.py` & `usda-0.0.25/src/usda/migrated_project/stylegan/dnnlib/submission/run_context.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/stylegan/dnnlib/submission/submit.py` & `usda-0.0.25/src/usda/migrated_project/stylegan/dnnlib/submission/submit.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/stylegan/dnnlib/tflib/__init__.py` & `usda-0.0.25/src/usda/migrated_project/stylegan/dnnlib/tflib/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/stylegan/dnnlib/tflib/autosummary.py` & `usda-0.0.25/src/usda/migrated_project/stylegan/dnnlib/tflib/autosummary.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/stylegan/dnnlib/tflib/network.py` & `usda-0.0.25/src/usda/migrated_project/stylegan/dnnlib/tflib/network.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/stylegan/dnnlib/tflib/optimizer.py` & `usda-0.0.25/src/usda/migrated_project/stylegan/dnnlib/tflib/optimizer.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/stylegan/dnnlib/tflib/tfutil.py` & `usda-0.0.25/src/usda/migrated_project/stylegan/dnnlib/tflib/tfutil.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/stylegan/dnnlib/util.py` & `usda-0.0.25/src/usda/migrated_project/stylegan/dnnlib/util.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/stylegan/extracted_funcs/_gadgets.py` & `usda-0.0.25/src/usda/migrated_project/stylegan/extracted_funcs/_gadgets.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/stylegan/models/_Blocks.py` & `usda-0.0.25/src/usda/migrated_project/stylegan/models/_Blocks.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/stylegan/models/_CustomLayers.py` & `usda-0.0.25/src/usda/migrated_project/stylegan/models/_CustomLayers.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/stylegan/models/_GAN.py` & `usda-0.0.25/src/usda/migrated_project/stylegan/models/_GAN.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/stylegan/models/_Losses.py` & `usda-0.0.25/src/usda/migrated_project/stylegan/models/_Losses.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/stylegan/models/__init__.py` & `usda-0.0.25/src/usda/migrated_project/stylegan/models/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/stylegan/models/_update_average.py` & `usda-0.0.25/src/usda/migrated_project/stylegan/models/_update_average.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/stylegan/train.py` & `usda-0.0.25/src/usda/migrated_project/stylegan/train.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/stylegan/utils/_copy.py` & `usda-0.0.25/src/usda/migrated_project/stylegan/utils/_copy.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/migrated_project/stylegan/utils/_logger.py` & `usda-0.0.25/src/usda/migrated_project/stylegan/utils/_logger.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/models/__init__.py` & `usda-0.0.25/src/usda/models/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/models/_bow_feature_builder.py` & `usda-0.0.25/src/usda/models/_bow_feature_builder.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/models/_clustering.py` & `usda-0.0.25/src/usda/models/_clustering.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/models/_computational_performance.py` & `usda-0.0.25/src/usda/models/_computational_performance.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/models/_curve_segmentation.py` & `usda-0.0.25/src/usda/models/_curve_segmentation.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/models/_decision_tree.py` & `usda-0.0.25/src/usda/models/_decision_tree.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/models/_dim1_convolution.py` & `usda-0.0.25/src/usda/models/_dim1_convolution.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/models/_entropy.py` & `usda-0.0.25/src/usda/models/_entropy.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/models/_global_local_autocorrelation.py` & `usda-0.0.25/src/usda/models/_global_local_autocorrelation.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/models/_image_tag_extractor.py` & `usda-0.0.25/src/usda/models/_image_tag_extractor.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/models/_label_encoder.py` & `usda-0.0.25/src/usda/models/_label_encoder.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/models/_neighbors.py` & `usda-0.0.25/src/usda/models/_neighbors.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/models/_nlp_tools.py` & `usda-0.0.25/src/usda/models/_nlp_tools.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/models/_random_forest_classifier.py` & `usda-0.0.25/src/usda/models/_random_forest_classifier.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/models/_rnn_lstm.py` & `usda-0.0.25/src/usda/models/_rnn_lstm.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/models/_seq2seq.py` & `usda-0.0.25/src/usda/models/_seq2seq.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/models/_sir_model.py` & `usda-0.0.25/src/usda/models/_sir_model.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/models/_superpixel_segmentation.py` & `usda-0.0.25/src/usda/models/_superpixel_segmentation.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/models/_transformer.py` & `usda-0.0.25/src/usda/models/_transformer.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/models/_vit.py` & `usda-0.0.25/src/usda/models/_vit.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,21 +119,21 @@
         # Perform classification prediction
         cls = x[0]
         out = self.mlp_head(cls)
         return out
 
 class ViT(pl.LightningModule):
 
-    def __init__(self, model_kwargs, lr,device='cuda'):
+    def __init__(self, model_kwargs, lr): # ,device='cuda'
         super().__init__()
         self.save_hyperparameters()
         self.model = VisionTransformer(**model_kwargs)
         # self.example_input_array = next(iter(train_loader))[0]
         # self.valid_acc = Accuracy()
-        self.valid_acc=Accuracy(task='multiclass',num_classes=model_kwargs['num_classes']).to(device)
+        self.valid_acc=Accuracy(task='multiclass',num_classes=model_kwargs['num_classes'])#.to(device)
 
     def forward(self, x):
         return self.model(x)
 
     def configure_optimizers(self):
         optimizer = optim.AdamW(self.parameters(), lr=self.hparams.lr)
         lr_scheduler = optim.lr_scheduler.MultiStepLR(optimizer, milestones=[100,150], gamma=0.1)
```

### Comparing `usda-0.0.24/src/usda/models/_word2vec_sgns.py` & `usda-0.0.25/src/usda/models/_word2vec_sgns.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/net/__init__.py` & `usda-0.0.25/src/usda/net/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/net/_networks_pix2pix.py` & `usda-0.0.25/src/usda/net/_networks_pix2pix.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/network/_g_drawing.py` & `usda-0.0.25/src/usda/network/_g_drawing.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/network/_pt_pattern.py` & `usda-0.0.25/src/usda/network/_pt_pattern.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/pattern_signature/__init__.py` & `usda-0.0.25/src/usda/pattern_signature/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/pattern_signature/_distance_metric.py` & `usda-0.0.25/src/usda/pattern_signature/_distance_metric.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/pattern_signature/_grid_neighbors_xy_finder.py` & `usda-0.0.25/src/usda/pattern_signature/_grid_neighbors_xy_finder.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/pattern_signature/_img_region_growing.py` & `usda-0.0.25/src/usda/pattern_signature/_img_region_growing.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/pattern_signature/_pattern_module.py` & `usda-0.0.25/src/usda/pattern_signature/_pattern_module.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/pattern_signature/_signature.py` & `usda-0.0.25/src/usda/pattern_signature/_signature.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/pattern_signature/_signature2distance_integration.py` & `usda-0.0.25/src/usda/pattern_signature/_signature2distance_integration.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/pgm/_MRF.py` & `usda-0.0.25/src/usda/pgm/_MRF.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/pgm/_MRF_urban_cooling.py` & `usda-0.0.25/src/usda/pgm/_MRF_urban_cooling.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/pgm/__init__.py` & `usda-0.0.25/src/usda/pgm/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/pgm/_image_segmentation_using_mrf.py` & `usda-0.0.25/src/usda/pgm/_image_segmentation_using_mrf.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/pgm/_pgm_calculating.py` & `usda-0.0.25/src/usda/pgm/_pgm_calculating.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/pgm/_pgm_draw.py` & `usda-0.0.25/src/usda/pgm/_pgm_draw.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/pgm/_probability_theory.py` & `usda-0.0.25/src/usda/pgm/_probability_theory.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/stats/__init__.py` & `usda-0.0.25/src/usda/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/stats/_descriptive_stats.py` & `usda-0.0.25/src/usda/stats/_descriptive_stats.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/stats/_kde.py` & `usda-0.0.25/src/usda/stats/_kde.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/stats/_outlier.py` & `usda-0.0.25/src/usda/stats/_outlier.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/stats/_regression.py` & `usda-0.0.25/src/usda/stats/_regression.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/tools/DL_layers_visualizer/0_72.jpg` & `usda-0.0.25/src/usda/tools/DL_layers_visualizer/0_72.jpg`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/tools/DL_layers_visualizer/0_8.jpg` & `usda-0.0.25/src/usda/tools/DL_layers_visualizer/0_8.jpg`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/tools/DL_layers_visualizer/0_9.jpg` & `usda-0.0.25/src/usda/tools/DL_layers_visualizer/0_9.jpg`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/tools/DL_layers_visualizer/DL_layers_visualizer.py` & `usda-0.0.25/src/usda/tools/DL_layers_visualizer/DL_layers_visualizer.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/utils/__init__.py` & `usda-0.0.25/src/usda/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/utils/_bunch.py` & `usda-0.0.25/src/usda/utils/_bunch.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/utils/_coordinate_transformation.py` & `usda-0.0.25/src/usda/utils/_coordinate_transformation.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/utils/_df_process.py` & `usda-0.0.25/src/usda/utils/_df_process.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/utils/_displayable_path.py` & `usda-0.0.25/src/usda/utils/_displayable_path.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/utils/_file_structure.py` & `usda-0.0.25/src/usda/utils/_file_structure.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/utils/_gadgets.py` & `usda-0.0.25/src/usda/utils/_gadgets.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/utils/_operating_time.py` & `usda-0.0.25/src/usda/utils/_operating_time.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/weight/__init__.py` & `usda-0.0.25/src/usda/weight/__init__.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/weight/_decision_rule.py` & `usda-0.0.25/src/usda/weight/_decision_rule.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda/weight/_entropy_weight.py` & `usda-0.0.25/src/usda/weight/_entropy_weight.py`

 * *Files identical despite different names*

### Comparing `usda-0.0.24/src/usda.egg-info/PKG-INFO` & `usda-0.0.25/src/usda.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usda
-Version: 0.0.24
+Version: 0.0.25
 Summary: A set of python modules for Urban Spatial Data Analysis Method (USDA)
 Home-page: https://richiebao.github.io/USDA_PyPI
 Download-URL: https://github.com/richieBao/USDA_PyPI
 Maintainer: Richie Bao
 Maintainer-email: richiebao@outlook.com
 License: new BSD
 Project-URL: Documentation, https://richiebao.github.io/USDA_PyPI
```

### Comparing `usda-0.0.24/src/usda.egg-info/SOURCES.txt` & `usda-0.0.25/src/usda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

