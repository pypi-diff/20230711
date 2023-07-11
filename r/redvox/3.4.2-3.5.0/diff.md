# Comparing `tmp/redvox-3.4.2.tar.gz` & `tmp/redvox-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redvox-3.4.2.tar", last modified: Wed May 17 22:37:40 2023, max compression
+gzip compressed data, was "redvox-3.5.0.tar", last modified: Tue Jul 11 21:03:45 2023, max compression
```

## Comparing `redvox-3.4.2.tar` & `redvox-3.5.0.tar`

### file list

```diff
@@ -1,153 +1,155 @@
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-05-17 22:37:40.942336 redvox-3.4.2/
--rw-r--r--   0 tyler      (501) staff       (20)    11343 2023-04-28 20:38:30.000000 redvox-3.4.2/LICENSE
--rw-r--r--   0 tyler      (501) staff       (20)    13906 2023-05-17 22:37:40.941757 redvox-3.4.2/PKG-INFO
--rw-r--r--   0 tyler      (501) staff       (20)      517 2021-06-16 20:22:36.000000 redvox-3.4.2/README.md
--rw-r--r--   0 tyler      (501) staff       (20)     1375 2023-04-28 20:38:30.000000 redvox-3.4.2/pyproject.toml
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-05-17 22:37:40.812976 redvox-3.4.2/redvox/
--rw-r--r--   0 tyler      (501) staff       (20)      728 2023-05-17 22:14:20.000000 redvox-3.4.2/redvox/__init__.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-05-17 22:37:40.816955 redvox-3.4.2/redvox/api1000/
--rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api1000/__init__.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-05-17 22:37:40.823528 redvox-3.4.2/redvox/api1000/common/
--rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api1000/common/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)    20204 2021-03-31 23:04:52.000000 redvox-3.4.2/redvox/api1000/common/common.py
--rw-r--r--   0 tyler      (501) staff       (20)     1050 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api1000/common/decorators.py
--rw-r--r--   0 tyler      (501) staff       (20)     5359 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api1000/common/generic.py
--rw-r--r--   0 tyler      (501) staff       (20)      875 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api1000/common/lz4.py
--rw-r--r--   0 tyler      (501) staff       (20)     2570 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api1000/common/mapping.py
--rw-r--r--   0 tyler      (501) staff       (20)     2237 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api1000/common/metadata.py
--rw-r--r--   0 tyler      (501) staff       (20)     2435 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api1000/common/typing.py
--rw-r--r--   0 tyler      (501) staff       (20)     2114 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api1000/errors.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-05-17 22:37:40.824720 redvox-3.4.2/redvox/api1000/gui/
--rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api1000/gui/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)     4672 2021-04-09 20:02:21.000000 redvox-3.4.2/redvox/api1000/gui/image_viewer.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-05-17 22:37:40.826033 redvox-3.4.2/redvox/api1000/proto/
--rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api1000/proto/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)    39434 2023-05-17 22:01:02.000000 redvox-3.4.2/redvox/api1000/proto/redvox_api_m_pb2.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-05-17 22:37:40.830873 redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/
--rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)     5639 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/event_streams.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-05-17 22:37:40.838024 redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/sensors/
--rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/sensors/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)    11949 2021-03-31 23:04:52.000000 redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/sensors/audio.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-05-17 22:37:40.839433 redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/sensors/derived/
--rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/sensors/derived/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)    14890 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/sensors/derived/movement.py
--rw-r--r--   0 tyler      (501) staff       (20)     7398 2021-03-31 23:04:52.000000 redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/sensors/image.py
--rw-r--r--   0 tyler      (501) staff       (20)    40936 2021-03-31 23:04:52.000000 redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/sensors/location.py
--rw-r--r--   0 tyler      (501) staff       (20)    42236 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/sensors/sensors.py
--rw-r--r--   0 tyler      (501) staff       (20)     3425 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/sensors/single.py
--rw-r--r--   0 tyler      (501) staff       (20)     5576 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/sensors/xyz.py
--rw-r--r--   0 tyler      (501) staff       (20)    50437 2022-12-15 01:35:54.000000 redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/station_information.py
--rw-r--r--   0 tyler      (501) staff       (20)    19060 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/timing_information.py
--rw-r--r--   0 tyler      (501) staff       (20)    21971 2021-03-31 23:04:52.000000 redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/wrapped_packet.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-05-17 22:37:40.854994 redvox-3.4.2/redvox/api900/
--rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)    17514 2021-03-31 23:04:52.000000 redvox-3.4.2/redvox/api900/concat.py
--rw-r--r--   0 tyler      (501) staff       (20)      494 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/constants.py
--rw-r--r--   0 tyler      (501) staff       (20)     1689 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/deprecation.py
--rw-r--r--   0 tyler      (501) staff       (20)      351 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/exceptions.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-05-17 22:37:40.857067 redvox-3.4.2/redvox/api900/lib/
--rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/lib/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)     7591 2023-05-17 22:01:02.000000 redvox-3.4.2/redvox/api900/lib/api900_pb2.py
--rw-r--r--   0 tyler      (501) staff       (20)    43091 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/location_analyzer.py
--rw-r--r--   0 tyler      (501) staff       (20)     2597 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/migrations.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-05-17 22:37:40.858404 redvox-3.4.2/redvox/api900/qa/
--rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/qa/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)     2813 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/qa/gap_detection.py
--rw-r--r--   0 tyler      (501) staff       (20)    16939 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/reader.py
--rw-r--r--   0 tyler      (501) staff       (20)    17096 2021-06-01 21:32:52.000000 redvox-3.4.2/redvox/api900/reader_utils.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-05-17 22:37:40.874601 redvox-3.4.2/redvox/api900/sensors/
--rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/sensors/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)     2113 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/sensors/accelerometer_sensor.py
--rw-r--r--   0 tyler      (501) staff       (20)     2298 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/sensors/barometer_sensor.py
--rw-r--r--   0 tyler      (501) staff       (20)     2665 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/sensors/evenly_sampled_channel.py
--rw-r--r--   0 tyler      (501) staff       (20)     6283 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/sensors/evenly_sampled_sensor.py
--rw-r--r--   0 tyler      (501) staff       (20)     1989 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/sensors/gyroscope_sensor.py
--rw-r--r--   0 tyler      (501) staff       (20)     4854 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/sensors/image_sensor.py
--rw-r--r--   0 tyler      (501) staff       (20)     2264 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/sensors/infrared_sensor.py
--rw-r--r--   0 tyler      (501) staff       (20)    16540 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/sensors/interleaved_channel.py
--rw-r--r--   0 tyler      (501) staff       (20)     2261 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/sensors/light_sensor.py
--rw-r--r--   0 tyler      (501) staff       (20)    10051 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/sensors/location_sensor.py
--rw-r--r--   0 tyler      (501) staff       (20)     2022 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/sensors/magnetometer_sensor.py
--rw-r--r--   0 tyler      (501) staff       (20)     3209 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/sensors/microphone_sensor.py
--rw-r--r--   0 tyler      (501) staff       (20)     4655 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/sensors/time_synchronization_sensor.py
--rw-r--r--   0 tyler      (501) staff       (20)     3536 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/sensors/unevenly_sampled_channel.py
--rw-r--r--   0 tyler      (501) staff       (20)     6619 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/sensors/unevenly_sampled_sensor.py
--rw-r--r--   0 tyler      (501) staff       (20)     5907 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/sensors/xyz_unevenly_sampled_sensor.py
--rw-r--r--   0 tyler      (501) staff       (20)     1128 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/stat_utils.py
--rw-r--r--   0 tyler      (501) staff       (20)     8780 2021-03-31 23:04:52.000000 redvox-3.4.2/redvox/api900/summarize.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-05-17 22:37:40.880006 redvox-3.4.2/redvox/api900/timesync/
--rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/timesync/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)    27606 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/timesync/api900_timesync.py
--rw-r--r--   0 tyler      (501) staff       (20)    13824 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/timesync/tri_message_stats.py
--rw-r--r--   0 tyler      (501) staff       (20)     1537 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/api900/types.py
--rw-r--r--   0 tyler      (501) staff       (20)    54392 2021-03-31 23:04:52.000000 redvox-3.4.2/redvox/api900/wrapped_redvox_packet.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-05-17 22:37:40.886577 redvox-3.4.2/redvox/cli/
--rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/cli/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)    22678 2021-04-09 20:02:21.000000 redvox-3.4.2/redvox/cli/cli.py
--rw-r--r--   0 tyler      (501) staff       (20)     6683 2021-06-01 21:32:52.000000 redvox-3.4.2/redvox/cli/conversions.py
--rw-r--r--   0 tyler      (501) staff       (20)     1797 2021-04-09 20:02:21.000000 redvox-3.4.2/redvox/cli/data_req.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-05-17 22:37:40.902033 redvox-3.4.2/redvox/cloud/
--rw-r--r--   0 tyler      (501) staff       (20)        0 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/cloud/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)     2267 2021-04-06 01:58:10.000000 redvox-3.4.2/redvox/cloud/api.py
--rw-r--r--   0 tyler      (501) staff       (20)   142063 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/cloud/api_m_fqns.py
--rw-r--r--   0 tyler      (501) staff       (20)     4334 2021-03-31 23:04:52.000000 redvox-3.4.2/redvox/cloud/auth_api.py
--rw-r--r--   0 tyler      (501) staff       (20)    27215 2022-12-15 01:35:54.000000 redvox-3.4.2/redvox/cloud/client.py
--rw-r--r--   0 tyler      (501) staff       (20)     5905 2022-12-15 01:35:54.000000 redvox-3.4.2/redvox/cloud/config.py
--rw-r--r--   0 tyler      (501) staff       (20)     6088 2021-04-09 20:02:21.000000 redvox-3.4.2/redvox/cloud/data_api.py
--rw-r--r--   0 tyler      (501) staff       (20)     3829 2022-12-15 01:35:54.000000 redvox-3.4.2/redvox/cloud/data_client.py
--rw-r--r--   0 tyler      (501) staff       (20)     3094 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/cloud/data_io.py
--rw-r--r--   0 tyler      (501) staff       (20)      487 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/cloud/errors.py
--rw-r--r--   0 tyler      (501) staff       (20)    18946 2022-12-15 01:35:54.000000 redvox-3.4.2/redvox/cloud/metadata_api.py
--rw-r--r--   0 tyler      (501) staff       (20)     3770 2021-04-14 22:44:11.000000 redvox-3.4.2/redvox/cloud/query_timing_correction.py
--rw-r--r--   0 tyler      (501) staff       (20)      902 2022-12-15 01:35:54.000000 redvox-3.4.2/redvox/cloud/routes.py
--rw-r--r--   0 tyler      (501) staff       (20)     4262 2021-04-14 22:44:11.000000 redvox-3.4.2/redvox/cloud/station_stats.py
--rw-r--r--   0 tyler      (501) staff       (20)     7707 2022-12-15 01:35:54.000000 redvox-3.4.2/redvox/cloud/subscription.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-05-17 22:37:40.939383 redvox-3.4.2/redvox/common/
--rw-r--r--   0 tyler      (501) staff       (20)      195 2021-03-30 21:57:13.000000 redvox-3.4.2/redvox/common/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)    55240 2023-01-05 19:44:31.000000 redvox-3.4.2/redvox/common/api_conversions.py
--rw-r--r--   0 tyler      (501) staff       (20)    23092 2023-05-17 22:01:02.000000 redvox-3.4.2/redvox/common/api_reader.py
--rw-r--r--   0 tyler      (501) staff       (20)     5532 2023-05-17 22:01:02.000000 redvox-3.4.2/redvox/common/api_reader_dw.py
--rw-r--r--   0 tyler      (501) staff       (20)     1173 2021-04-19 23:26:28.000000 redvox-3.4.2/redvox/common/constants.py
--rw-r--r--   0 tyler      (501) staff       (20)     4126 2021-06-29 20:11:21.000000 redvox-3.4.2/redvox/common/cross_stats.py
--rw-r--r--   0 tyler      (501) staff       (20)    44735 2023-05-17 22:01:02.000000 redvox-3.4.2/redvox/common/data_window.py
--rw-r--r--   0 tyler      (501) staff       (20)     8246 2022-12-15 01:35:54.000000 redvox-3.4.2/redvox/common/data_window_configuration.py
--rw-r--r--   0 tyler      (501) staff       (20)     7301 2023-05-17 22:01:02.000000 redvox-3.4.2/redvox/common/data_window_io.py
--rw-r--r--   0 tyler      (501) staff       (20)    16785 2023-01-05 19:44:31.000000 redvox-3.4.2/redvox/common/date_time_utils.py
--rw-r--r--   0 tyler      (501) staff       (20)     3250 2022-12-15 01:35:54.000000 redvox-3.4.2/redvox/common/errors.py
--rw-r--r--   0 tyler      (501) staff       (20)    41765 2023-05-17 22:01:02.000000 redvox-3.4.2/redvox/common/event_stream.py
--rw-r--r--   0 tyler      (501) staff       (20)     3397 2022-12-15 01:35:54.000000 redvox-3.4.2/redvox/common/event_stream_io.py
--rw-r--r--   0 tyler      (501) staff       (20)    13655 2023-05-17 22:01:02.000000 redvox-3.4.2/redvox/common/file_statistics.py
--rw-r--r--   0 tyler      (501) staff       (20)    17695 2023-05-17 22:01:02.000000 redvox-3.4.2/redvox/common/gap_and_pad_utils.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-05-17 22:37:40.940659 redvox-3.4.2/redvox/common/gui/
--rw-r--r--   0 tyler      (501) staff       (20)        0 2021-04-09 20:02:21.000000 redvox-3.4.2/redvox/common/gui/__init__.py
--rw-r--r--   0 tyler      (501) staff       (20)    16251 2021-04-15 01:00:48.000000 redvox-3.4.2/redvox/common/gui/cloud_data_retrieval.py
--rw-r--r--   0 tyler      (501) staff       (20)    56756 2023-05-17 22:01:02.000000 redvox-3.4.2/redvox/common/io.py
--rw-r--r--   0 tyler      (501) staff       (20)    26136 2023-05-17 22:01:02.000000 redvox-3.4.2/redvox/common/offset_model.py
--rw-r--r--   0 tyler      (501) staff       (20)    27551 2023-05-17 22:01:02.000000 redvox-3.4.2/redvox/common/packet_to_pyarrow.py
--rw-r--r--   0 tyler      (501) staff       (20)     5022 2022-12-15 01:35:54.000000 redvox-3.4.2/redvox/common/parallel_utils.py
--rw-r--r--   0 tyler      (501) staff       (20)     1256 2022-12-15 01:35:54.000000 redvox-3.4.2/redvox/common/run_me.py
--rw-r--r--   0 tyler      (501) staff       (20)    94611 2023-05-17 22:01:02.000000 redvox-3.4.2/redvox/common/sensor_data.py
--rw-r--r--   0 tyler      (501) staff       (20)     1206 2022-12-15 01:35:54.000000 redvox-3.4.2/redvox/common/sensor_io.py
--rw-r--r--   0 tyler      (501) staff       (20)    18349 2023-01-05 19:44:31.000000 redvox-3.4.2/redvox/common/sensor_reader_utils.py
--rw-r--r--   0 tyler      (501) staff       (20)     3352 2023-01-05 19:44:31.000000 redvox-3.4.2/redvox/common/session_io.py
--rw-r--r--   0 tyler      (501) staff       (20)    44873 2023-05-17 22:01:02.000000 redvox-3.4.2/redvox/common/session_model.py
--rw-r--r--   0 tyler      (501) staff       (20)    14986 2023-01-05 19:44:31.000000 redvox-3.4.2/redvox/common/session_model_utils.py
--rw-r--r--   0 tyler      (501) staff       (20)    69098 2023-05-17 22:01:02.000000 redvox-3.4.2/redvox/common/station.py
--rw-r--r--   0 tyler      (501) staff       (20)     1679 2022-12-15 01:35:54.000000 redvox-3.4.2/redvox/common/station_io.py
--rw-r--r--   0 tyler      (501) staff       (20)     4549 2023-04-26 02:27:01.000000 redvox-3.4.2/redvox/common/station_model.py
--rw-r--r--   0 tyler      (501) staff       (20)    18151 2023-05-17 22:01:02.000000 redvox-3.4.2/redvox/common/station_utils.py
--rw-r--r--   0 tyler      (501) staff       (20)     4002 2022-12-15 01:35:54.000000 redvox-3.4.2/redvox/common/stats_helper.py
--rw-r--r--   0 tyler      (501) staff       (20)    21477 2023-05-17 22:01:02.000000 redvox-3.4.2/redvox/common/timesync.py
--rw-r--r--   0 tyler      (501) staff       (20)     1295 2022-12-15 01:35:54.000000 redvox-3.4.2/redvox/common/timesync_io.py
--rw-r--r--   0 tyler      (501) staff       (20)    14257 2023-05-17 22:01:02.000000 redvox-3.4.2/redvox/common/tri_message_stats.py
--rw-r--r--   0 tyler      (501) staff       (20)     1867 2021-06-29 20:11:21.000000 redvox-3.4.2/redvox/common/versioning.py
--rw-r--r--   0 tyler      (501) staff       (20)     2205 2023-05-17 22:01:02.000000 redvox-3.4.2/redvox/settings.py
-drwxr-xr-x   0 tyler      (501) staff       (20)        0 2023-05-17 22:37:40.815924 redvox-3.4.2/redvox.egg-info/
--rw-r--r--   0 tyler      (501) staff       (20)    13906 2023-05-17 22:37:40.000000 redvox-3.4.2/redvox.egg-info/PKG-INFO
--rw-r--r--   0 tyler      (501) staff       (20)     4483 2023-05-17 22:37:40.000000 redvox-3.4.2/redvox.egg-info/SOURCES.txt
--rw-r--r--   0 tyler      (501) staff       (20)        1 2023-05-17 22:37:40.000000 redvox-3.4.2/redvox.egg-info/dependency_links.txt
--rw-r--r--   0 tyler      (501) staff       (20)       51 2023-05-17 22:37:40.000000 redvox-3.4.2/redvox.egg-info/entry_points.txt
--rw-r--r--   0 tyler      (501) staff       (20)      386 2023-05-17 22:37:40.000000 redvox-3.4.2/redvox.egg-info/requires.txt
--rw-r--r--   0 tyler      (501) staff       (20)        7 2023-05-17 22:37:40.000000 redvox-3.4.2/redvox.egg-info/top_level.txt
--rw-r--r--   0 tyler      (501) staff       (20)       38 2023-05-17 22:37:40.942487 redvox-3.4.2/setup.cfg
+drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-11 21:03:45.439884 redvox-3.5.0/
+-rw-r--r--   0 anthony    (501) staff       (20)    11343 2023-05-10 20:30:19.000000 redvox-3.5.0/LICENSE
+-rw-r--r--   0 anthony    (501) staff       (20)    13906 2023-07-11 21:03:45.439712 redvox-3.5.0/PKG-INFO
+-rw-r--r--   0 anthony    (501) staff       (20)      517 2021-12-29 23:42:43.000000 redvox-3.5.0/README.md
+-rw-r--r--   0 anthony    (501) staff       (20)     1375 2023-05-10 20:30:19.000000 redvox-3.5.0/pyproject.toml
+drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-11 21:03:45.424030 redvox-3.5.0/redvox/
+-rw-r--r--   0 anthony    (501) staff       (20)      728 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/__init__.py
+drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-11 21:03:45.424859 redvox-3.5.0/redvox/api1000/
+-rw-r--r--   0 anthony    (501) staff       (20)        0 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/__init__.py
+drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-11 21:03:45.425680 redvox-3.5.0/redvox/api1000/common/
+-rw-r--r--   0 anthony    (501) staff       (20)        0 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/common/__init__.py
+-rw-r--r--   0 anthony    (501) staff       (20)    20204 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/common/common.py
+-rw-r--r--   0 anthony    (501) staff       (20)     1050 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/common/decorators.py
+-rw-r--r--   0 anthony    (501) staff       (20)     5359 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/common/generic.py
+-rw-r--r--   0 anthony    (501) staff       (20)      875 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/common/lz4.py
+-rw-r--r--   0 anthony    (501) staff       (20)     2570 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/common/mapping.py
+-rw-r--r--   0 anthony    (501) staff       (20)     2237 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/common/metadata.py
+-rw-r--r--   0 anthony    (501) staff       (20)     2435 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/common/typing.py
+-rw-r--r--   0 anthony    (501) staff       (20)     2114 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/errors.py
+drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-11 21:03:45.425862 redvox-3.5.0/redvox/api1000/gui/
+-rw-r--r--   0 anthony    (501) staff       (20)        0 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/gui/__init__.py
+-rw-r--r--   0 anthony    (501) staff       (20)     4672 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/gui/image_viewer.py
+drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-11 21:03:45.426053 redvox-3.5.0/redvox/api1000/proto/
+-rw-r--r--   0 anthony    (501) staff       (20)        0 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/proto/__init__.py
+-rw-r--r--   0 anthony    (501) staff       (20)    39434 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/api1000/proto/redvox_api_m_pb2.py
+drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-11 21:03:45.426749 redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/
+-rw-r--r--   0 anthony    (501) staff       (20)        0 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/__init__.py
+-rw-r--r--   0 anthony    (501) staff       (20)     5639 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/event_streams.py
+-rw-r--r--   0 anthony    (501) staff       (20)    10817 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/ml.py
+drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-11 21:03:45.427576 redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/sensors/
+-rw-r--r--   0 anthony    (501) staff       (20)        0 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/sensors/__init__.py
+-rw-r--r--   0 anthony    (501) staff       (20)    11949 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/sensors/audio.py
+drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-11 21:03:45.427772 redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/sensors/derived/
+-rw-r--r--   0 anthony    (501) staff       (20)        0 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/sensors/derived/__init__.py
+-rw-r--r--   0 anthony    (501) staff       (20)    14890 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/sensors/derived/movement.py
+-rw-r--r--   0 anthony    (501) staff       (20)     7398 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/sensors/image.py
+-rw-r--r--   0 anthony    (501) staff       (20)    40936 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/sensors/location.py
+-rw-r--r--   0 anthony    (501) staff       (20)    42236 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/sensors/sensors.py
+-rw-r--r--   0 anthony    (501) staff       (20)     3425 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/sensors/single.py
+-rw-r--r--   0 anthony    (501) staff       (20)     5576 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/sensors/xyz.py
+-rw-r--r--   0 anthony    (501) staff       (20)    50437 2022-08-04 18:31:21.000000 redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/station_information.py
+-rw-r--r--   0 anthony    (501) staff       (20)    19060 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/timing_information.py
+-rw-r--r--   0 anthony    (501) staff       (20)    21971 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/wrapped_packet.py
+drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-11 21:03:45.429228 redvox-3.5.0/redvox/api900/
+-rw-r--r--   0 anthony    (501) staff       (20)        0 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/__init__.py
+-rw-r--r--   0 anthony    (501) staff       (20)    17514 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/concat.py
+-rw-r--r--   0 anthony    (501) staff       (20)      494 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/constants.py
+-rw-r--r--   0 anthony    (501) staff       (20)     1689 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/deprecation.py
+-rw-r--r--   0 anthony    (501) staff       (20)      351 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/exceptions.py
+drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-11 21:03:45.429453 redvox-3.5.0/redvox/api900/lib/
+-rw-r--r--   0 anthony    (501) staff       (20)        0 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/lib/__init__.py
+-rw-r--r--   0 anthony    (501) staff       (20)     7591 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/api900/lib/api900_pb2.py
+-rw-r--r--   0 anthony    (501) staff       (20)    43091 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/location_analyzer.py
+-rw-r--r--   0 anthony    (501) staff       (20)     2597 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/migrations.py
+drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-11 21:03:45.429653 redvox-3.5.0/redvox/api900/qa/
+-rw-r--r--   0 anthony    (501) staff       (20)        0 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/qa/__init__.py
+-rw-r--r--   0 anthony    (501) staff       (20)     2813 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/qa/gap_detection.py
+-rw-r--r--   0 anthony    (501) staff       (20)    16939 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/reader.py
+-rw-r--r--   0 anthony    (501) staff       (20)    17096 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/reader_utils.py
+drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-11 21:03:45.431541 redvox-3.5.0/redvox/api900/sensors/
+-rw-r--r--   0 anthony    (501) staff       (20)        0 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/sensors/__init__.py
+-rw-r--r--   0 anthony    (501) staff       (20)     2113 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/sensors/accelerometer_sensor.py
+-rw-r--r--   0 anthony    (501) staff       (20)     2298 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/sensors/barometer_sensor.py
+-rw-r--r--   0 anthony    (501) staff       (20)     2665 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/sensors/evenly_sampled_channel.py
+-rw-r--r--   0 anthony    (501) staff       (20)     6283 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/sensors/evenly_sampled_sensor.py
+-rw-r--r--   0 anthony    (501) staff       (20)     1989 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/sensors/gyroscope_sensor.py
+-rw-r--r--   0 anthony    (501) staff       (20)     4854 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/sensors/image_sensor.py
+-rw-r--r--   0 anthony    (501) staff       (20)     2264 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/sensors/infrared_sensor.py
+-rw-r--r--   0 anthony    (501) staff       (20)    16540 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/sensors/interleaved_channel.py
+-rw-r--r--   0 anthony    (501) staff       (20)     2261 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/sensors/light_sensor.py
+-rw-r--r--   0 anthony    (501) staff       (20)    10051 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/sensors/location_sensor.py
+-rw-r--r--   0 anthony    (501) staff       (20)     2022 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/sensors/magnetometer_sensor.py
+-rw-r--r--   0 anthony    (501) staff       (20)     3209 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/sensors/microphone_sensor.py
+-rw-r--r--   0 anthony    (501) staff       (20)     4655 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/sensors/time_synchronization_sensor.py
+-rw-r--r--   0 anthony    (501) staff       (20)     3536 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/sensors/unevenly_sampled_channel.py
+-rw-r--r--   0 anthony    (501) staff       (20)     6619 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/sensors/unevenly_sampled_sensor.py
+-rw-r--r--   0 anthony    (501) staff       (20)     5907 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/sensors/xyz_unevenly_sampled_sensor.py
+-rw-r--r--   0 anthony    (501) staff       (20)     1128 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/stat_utils.py
+-rw-r--r--   0 anthony    (501) staff       (20)     8780 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/summarize.py
+drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-11 21:03:45.431899 redvox-3.5.0/redvox/api900/timesync/
+-rw-r--r--   0 anthony    (501) staff       (20)        0 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/timesync/__init__.py
+-rw-r--r--   0 anthony    (501) staff       (20)    27606 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/timesync/api900_timesync.py
+-rw-r--r--   0 anthony    (501) staff       (20)    13824 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/timesync/tri_message_stats.py
+-rw-r--r--   0 anthony    (501) staff       (20)     1537 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/types.py
+-rw-r--r--   0 anthony    (501) staff       (20)    54392 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/api900/wrapped_redvox_packet.py
+drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-11 21:03:45.433731 redvox-3.5.0/redvox/cli/
+-rw-r--r--   0 anthony    (501) staff       (20)        0 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/cli/__init__.py
+-rw-r--r--   0 anthony    (501) staff       (20)    22678 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/cli/cli.py
+-rw-r--r--   0 anthony    (501) staff       (20)     6683 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/cli/conversions.py
+-rw-r--r--   0 anthony    (501) staff       (20)     1797 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/cli/data_req.py
+drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-11 21:03:45.435441 redvox-3.5.0/redvox/cloud/
+-rw-r--r--   0 anthony    (501) staff       (20)        0 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/cloud/__init__.py
+-rw-r--r--   0 anthony    (501) staff       (20)     2267 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/cloud/api.py
+-rw-r--r--   0 anthony    (501) staff       (20)   142063 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/cloud/api_m_fqns.py
+-rw-r--r--   0 anthony    (501) staff       (20)     4334 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/cloud/auth_api.py
+-rw-r--r--   0 anthony    (501) staff       (20)    29429 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/cloud/client.py
+-rw-r--r--   0 anthony    (501) staff       (20)     5905 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/cloud/config.py
+-rw-r--r--   0 anthony    (501) staff       (20)     6088 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/cloud/data_api.py
+-rw-r--r--   0 anthony    (501) staff       (20)     3829 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/cloud/data_client.py
+-rw-r--r--   0 anthony    (501) staff       (20)     3266 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/cloud/data_io.py
+-rw-r--r--   0 anthony    (501) staff       (20)      487 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/cloud/errors.py
+-rw-r--r--   0 anthony    (501) staff       (20)    18946 2022-08-04 18:31:21.000000 redvox-3.5.0/redvox/cloud/metadata_api.py
+-rw-r--r--   0 anthony    (501) staff       (20)     3770 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/cloud/query_timing_correction.py
+-rw-r--r--   0 anthony    (501) staff       (20)     1086 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/cloud/routes.py
+-rw-r--r--   0 anthony    (501) staff       (20)    10985 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/cloud/session_model_api.py
+-rw-r--r--   0 anthony    (501) staff       (20)     4262 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/cloud/station_stats.py
+-rw-r--r--   0 anthony    (501) staff       (20)     7707 2022-08-04 18:31:21.000000 redvox-3.5.0/redvox/cloud/subscription.py
+drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-11 21:03:45.439330 redvox-3.5.0/redvox/common/
+-rw-r--r--   0 anthony    (501) staff       (20)      195 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/common/__init__.py
+-rw-r--r--   0 anthony    (501) staff       (20)    55240 2023-03-01 21:44:51.000000 redvox-3.5.0/redvox/common/api_conversions.py
+-rw-r--r--   0 anthony    (501) staff       (20)    23894 2023-07-11 21:00:08.000000 redvox-3.5.0/redvox/common/api_reader.py
+-rw-r--r--   0 anthony    (501) staff       (20)     5249 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/api_reader_dw.py
+-rw-r--r--   0 anthony    (501) staff       (20)     1173 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/common/constants.py
+-rw-r--r--   0 anthony    (501) staff       (20)     4126 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/common/cross_stats.py
+-rw-r--r--   0 anthony    (501) staff       (20)    42995 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/data_window.py
+-rw-r--r--   0 anthony    (501) staff       (20)     8266 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/data_window_configuration.py
+-rw-r--r--   0 anthony    (501) staff       (20)     7154 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/data_window_io.py
+-rw-r--r--   0 anthony    (501) staff       (20)    16785 2023-03-01 21:44:51.000000 redvox-3.5.0/redvox/common/date_time_utils.py
+-rw-r--r--   0 anthony    (501) staff       (20)     3252 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/errors.py
+-rw-r--r--   0 anthony    (501) staff       (20)    41889 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/event_stream.py
+-rw-r--r--   0 anthony    (501) staff       (20)     3104 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/event_stream_io.py
+-rw-r--r--   0 anthony    (501) staff       (20)    13655 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/file_statistics.py
+-rw-r--r--   0 anthony    (501) staff       (20)    17541 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/gap_and_pad_utils.py
+drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-11 21:03:45.439517 redvox-3.5.0/redvox/common/gui/
+-rw-r--r--   0 anthony    (501) staff       (20)        0 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/common/gui/__init__.py
+-rw-r--r--   0 anthony    (501) staff       (20)    16251 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/common/gui/cloud_data_retrieval.py
+-rw-r--r--   0 anthony    (501) staff       (20)    56756 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/io.py
+-rw-r--r--   0 anthony    (501) staff       (20)    26597 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/offset_model.py
+-rw-r--r--   0 anthony    (501) staff       (20)    26988 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/packet_to_pyarrow.py
+-rw-r--r--   0 anthony    (501) staff       (20)     5022 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/common/parallel_utils.py
+-rw-r--r--   0 anthony    (501) staff       (20)     1256 2022-08-04 18:31:21.000000 redvox-3.5.0/redvox/common/run_me.py
+-rw-r--r--   0 anthony    (501) staff       (20)    94752 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/sensor_data.py
+-rw-r--r--   0 anthony    (501) staff       (20)     1086 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/sensor_io.py
+-rw-r--r--   0 anthony    (501) staff       (20)    17894 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/sensor_reader_utils.py
+-rw-r--r--   0 anthony    (501) staff       (20)     2947 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/session_io.py
+-rw-r--r--   0 anthony    (501) staff       (20)    17172 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/session_model.py
+-rw-r--r--   0 anthony    (501) staff       (20)    15794 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/session_model_utils.py
+-rw-r--r--   0 anthony    (501) staff       (20)    70537 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/station.py
+-rw-r--r--   0 anthony    (501) staff       (20)     1441 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/station_io.py
+-rw-r--r--   0 anthony    (501) staff       (20)     4909 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/station_model.py
+-rw-r--r--   0 anthony    (501) staff       (20)    17541 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/station_utils.py
+-rw-r--r--   0 anthony    (501) staff       (20)     3964 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/stats_helper.py
+-rw-r--r--   0 anthony    (501) staff       (20)    21550 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/timesync.py
+-rw-r--r--   0 anthony    (501) staff       (20)     1175 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/timesync_io.py
+-rw-r--r--   0 anthony    (501) staff       (20)    13810 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/common/tri_message_stats.py
+-rw-r--r--   0 anthony    (501) staff       (20)     1867 2021-12-29 23:42:43.000000 redvox-3.5.0/redvox/common/versioning.py
+-rw-r--r--   0 anthony    (501) staff       (20)     2205 2023-07-11 20:34:17.000000 redvox-3.5.0/redvox/settings.py
+drwxr-xr-x   0 anthony    (501) staff       (20)        0 2023-07-11 21:03:45.424660 redvox-3.5.0/redvox.egg-info/
+-rw-r--r--   0 anthony    (501) staff       (20)    13906 2023-07-11 21:03:45.000000 redvox-3.5.0/redvox.egg-info/PKG-INFO
+-rw-r--r--   0 anthony    (501) staff       (20)     4560 2023-07-11 21:03:45.000000 redvox-3.5.0/redvox.egg-info/SOURCES.txt
+-rw-r--r--   0 anthony    (501) staff       (20)        1 2023-07-11 21:03:45.000000 redvox-3.5.0/redvox.egg-info/dependency_links.txt
+-rw-r--r--   0 anthony    (501) staff       (20)       51 2023-07-11 21:03:45.000000 redvox-3.5.0/redvox.egg-info/entry_points.txt
+-rw-r--r--   0 anthony    (501) staff       (20)      386 2023-07-11 21:03:45.000000 redvox-3.5.0/redvox.egg-info/requires.txt
+-rw-r--r--   0 anthony    (501) staff       (20)        7 2023-07-11 21:03:45.000000 redvox-3.5.0/redvox.egg-info/top_level.txt
+-rw-r--r--   0 anthony    (501) staff       (20)       38 2023-07-11 21:03:45.439917 redvox-3.5.0/setup.cfg
```

### Comparing `redvox-3.4.2/LICENSE` & `redvox-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/PKG-INFO` & `redvox-3.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redvox
-Version: 3.4.2
+Version: 3.5.0
 Summary: Library for working with RedVox files. 
 Author-email: "RedVox, Inc" <support@redvox.io>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `redvox-3.4.2/README.md` & `redvox-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/pyproject.toml` & `redvox-3.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/__init__.py` & `redvox-3.5.0/redvox/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Provides library level metadata and constants.
 """
 
 NAME: str = "redvox"
-VERSION: str = "3.4.2"
+VERSION: str = "3.5.0"
 
 
 def version() -> str:
     """Returns the version number of this library."""
     return VERSION
```

### Comparing `redvox-3.4.2/redvox/api1000/common/common.py` & `redvox-3.5.0/redvox/api1000/common/common.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api1000/common/decorators.py` & `redvox-3.5.0/redvox/api1000/common/decorators.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api1000/common/generic.py` & `redvox-3.5.0/redvox/api1000/common/generic.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api1000/common/lz4.py` & `redvox-3.5.0/redvox/api1000/common/lz4.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api1000/common/mapping.py` & `redvox-3.5.0/redvox/api1000/common/mapping.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api1000/common/metadata.py` & `redvox-3.5.0/redvox/api1000/common/metadata.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api1000/common/typing.py` & `redvox-3.5.0/redvox/api1000/common/typing.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api1000/errors.py` & `redvox-3.5.0/redvox/api1000/errors.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api1000/gui/image_viewer.py` & `redvox-3.5.0/redvox/api1000/gui/image_viewer.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api1000/proto/redvox_api_m_pb2.py` & `redvox-3.5.0/redvox/api1000/proto/redvox_api_m_pb2.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/event_streams.py` & `redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/event_streams.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/sensors/audio.py` & `redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/sensors/audio.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/sensors/derived/movement.py` & `redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/sensors/derived/movement.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/sensors/image.py` & `redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/sensors/image.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/sensors/location.py` & `redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/sensors/location.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/sensors/sensors.py` & `redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/sensors/sensors.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/sensors/single.py` & `redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/sensors/single.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/sensors/xyz.py` & `redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/sensors/xyz.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/station_information.py` & `redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/station_information.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/timing_information.py` & `redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/timing_information.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api1000/wrapped_redvox_packet/wrapped_packet.py` & `redvox-3.5.0/redvox/api1000/wrapped_redvox_packet/wrapped_packet.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api900/concat.py` & `redvox-3.5.0/redvox/api900/concat.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api900/deprecation.py` & `redvox-3.5.0/redvox/api900/deprecation.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api900/lib/api900_pb2.py` & `redvox-3.5.0/redvox/api900/lib/api900_pb2.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api900/location_analyzer.py` & `redvox-3.5.0/redvox/api900/location_analyzer.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api900/migrations.py` & `redvox-3.5.0/redvox/api900/migrations.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api900/qa/gap_detection.py` & `redvox-3.5.0/redvox/api900/qa/gap_detection.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api900/reader.py` & `redvox-3.5.0/redvox/api900/reader.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api900/reader_utils.py` & `redvox-3.5.0/redvox/api900/reader_utils.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api900/sensors/accelerometer_sensor.py` & `redvox-3.5.0/redvox/api900/sensors/accelerometer_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api900/sensors/barometer_sensor.py` & `redvox-3.5.0/redvox/api900/sensors/barometer_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api900/sensors/evenly_sampled_channel.py` & `redvox-3.5.0/redvox/api900/sensors/evenly_sampled_channel.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api900/sensors/evenly_sampled_sensor.py` & `redvox-3.5.0/redvox/api900/sensors/evenly_sampled_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api900/sensors/gyroscope_sensor.py` & `redvox-3.5.0/redvox/api900/sensors/gyroscope_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api900/sensors/image_sensor.py` & `redvox-3.5.0/redvox/api900/sensors/image_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api900/sensors/infrared_sensor.py` & `redvox-3.5.0/redvox/api900/sensors/infrared_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api900/sensors/interleaved_channel.py` & `redvox-3.5.0/redvox/api900/sensors/interleaved_channel.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api900/sensors/light_sensor.py` & `redvox-3.5.0/redvox/api900/sensors/light_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api900/sensors/location_sensor.py` & `redvox-3.5.0/redvox/api900/sensors/location_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api900/sensors/magnetometer_sensor.py` & `redvox-3.5.0/redvox/api900/sensors/magnetometer_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api900/sensors/microphone_sensor.py` & `redvox-3.5.0/redvox/api900/sensors/microphone_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api900/sensors/time_synchronization_sensor.py` & `redvox-3.5.0/redvox/api900/sensors/time_synchronization_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api900/sensors/unevenly_sampled_channel.py` & `redvox-3.5.0/redvox/api900/sensors/unevenly_sampled_channel.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api900/sensors/unevenly_sampled_sensor.py` & `redvox-3.5.0/redvox/api900/sensors/unevenly_sampled_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api900/sensors/xyz_unevenly_sampled_sensor.py` & `redvox-3.5.0/redvox/api900/sensors/xyz_unevenly_sampled_sensor.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api900/stat_utils.py` & `redvox-3.5.0/redvox/api900/stat_utils.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api900/summarize.py` & `redvox-3.5.0/redvox/api900/summarize.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api900/timesync/api900_timesync.py` & `redvox-3.5.0/redvox/api900/timesync/api900_timesync.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api900/timesync/tri_message_stats.py` & `redvox-3.5.0/redvox/api900/timesync/tri_message_stats.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api900/types.py` & `redvox-3.5.0/redvox/api900/types.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/api900/wrapped_redvox_packet.py` & `redvox-3.5.0/redvox/api900/wrapped_redvox_packet.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/cli/cli.py` & `redvox-3.5.0/redvox/cli/cli.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/cli/conversions.py` & `redvox-3.5.0/redvox/cli/conversions.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/cli/data_req.py` & `redvox-3.5.0/redvox/cli/data_req.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/cloud/api.py` & `redvox-3.5.0/redvox/cloud/api.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/cloud/api_m_fqns.py` & `redvox-3.5.0/redvox/cloud/api_m_fqns.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/cloud/auth_api.py` & `redvox-3.5.0/redvox/cloud/auth_api.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/cloud/client.py` & `redvox-3.5.0/redvox/cloud/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,35 @@
 """
 This module contains the RedVox Cloud API client.
 
 This client provides convenient access to RedVox metadata and data. This client manages the tedious business of keeping
 an up-to-date authentication token for making authenticated API requests.
 """
 
-from collections import defaultdict
 import contextlib
 import threading
 from multiprocessing import Queue
-from typing import Dict, List, Optional, Tuple, TYPE_CHECKING, Iterator
+from typing import List, Optional, Tuple, TYPE_CHECKING, Iterator
 
 import requests
 
 import redvox.cloud.api as api
 import redvox.cloud.auth_api as auth_api
 from redvox.cloud.config import RedVoxConfig
 import redvox.cloud.errors as cloud_errors
 import redvox.common.constants as constants
-from redvox.common.offset_model import compute_offsets
 from redvox.cloud.query_timing_correction import (
     correct_query_timing as do_correct_query_timing,
-    CorrectedQuery,
 )
 import redvox.cloud.data_api as data_api
 import redvox.cloud.metadata_api as metadata_api
 import redvox.cloud.station_stats as station_stats_api
+import redvox.cloud.session_model_api as session_model_api
 
 if TYPE_CHECKING:
-    from redvox.cloud.station_stats import StationStatsResp
-    from redvox.common.file_statistics import StationStat
-    from redvox.common.offset_model import TimingOffsets
     from redvox.cloud.query_timing_correction import CorrectedQuery
 
 
 def chunk_time_range(
     start_ts: int, end_ts: int, max_chunk: int
 ) -> List[Tuple[int, int]]:
     """
@@ -682,14 +677,75 @@
             )
         )
 
         return station_stats_api.request_station_stats(
             self.redvox_config, station_stats_req, self.__session, self.timeout
         )
 
+    def request_session_model(
+        self, session_key: str
+    ) -> session_model_api.SessionModelResp:
+        """
+        Requests a session model.
+        :param session_key: The session key.
+        :return: An instance of a SessionModelResp.
+        """
+        req: session_model_api.SessionModelReq = session_model_api.SessionModelReq(
+            self.auth_token, session_key
+        )
+        return session_model_api.request_session(
+            self.redvox_config, req, self.__session, self.timeout
+        )
+
+    def request_session_models(
+        self,
+        id_uuids: Optional[List[str]] = None,
+        owner: Optional[str] = None,
+        start_ts: Optional[int] = None,
+        end_ts: Optional[int] = None,
+        include_public: bool = False,
+    ) -> session_model_api.SessionModelsResp:
+        """
+        Requests a range of session models.
+        :param id_uuids: An optional list of IDs or ID:UUIDs.
+        :param owner: An optional owner.
+        :param start_ts: An optional start timestamp (microseconds).
+        :param end_ts: An optional end timestamp (microseconds).
+        :param include_public: Additionally include public sessions that may not be the same as the owner.
+        :return: An instance of SessionModelsResp.
+        """
+        req: session_model_api.SessionModelsReq = session_model_api.SessionModelsReq(
+            self.auth_token, id_uuids, owner, start_ts, end_ts, include_public
+        )
+        return session_model_api.request_sessions(
+            self.redvox_config, req, self.__session, self.timeout
+        )
+
+    def request_dynamic_session_model(
+        self,
+        session_key: str,
+        start_ts: int,
+        end_ts: int,
+    ) -> session_model_api.DynamicSessionModelResp:
+        """
+        Requests a dynamic session given the fields that make up its key.
+        :param session_key: The parent session model key.
+        :param start_ts: The start of the dynamic session (microseconds).
+        :param end_ts: The end of the dynamic session (microseconds).
+        :return: An instance of DynamicSessionModelResp.
+        """
+        req: session_model_api.DynamicSessionModelReq = (
+            session_model_api.DynamicSessionModelReq(
+                self.auth_token, session_key, start_ts, end_ts
+            )
+        )
+        return session_model_api.request_dynamic_session(
+            self.redvox_config, req, self.__session, self.timeout
+        )
+
 
 @contextlib.contextmanager
 def cloud_client(
     redvox_config: Optional[RedVoxConfig] = RedVoxConfig.find(),
     refresh_token_interval: float = 600.0,
     timeout: float = 10.0,
 ):
```

### Comparing `redvox-3.4.2/redvox/cloud/config.py` & `redvox-3.5.0/redvox/cloud/config.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/cloud/data_api.py` & `redvox-3.5.0/redvox/cloud/data_api.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/cloud/data_client.py` & `redvox-3.5.0/redvox/cloud/data_client.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/cloud/data_io.py` & `redvox-3.5.0/redvox/cloud/data_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,15 +73,20 @@
     :param out_dir: The output directory where files will be stored.
     :param retries: The number of times to retry failed file downloads.
     :return: A tuple containing the data_key and the length of the download response.
     """
     buf: Optional[bytes] = get_file(url, retries, session)
 
     if buf:
-        data_key = find_between("/rdvxdata/", "?X-Amz-Algorithm=", url)
+        if "/rdvxdata/" in url:
+            data_key = find_between("/rdvxdata/", "?X-Amz-Algorithm=", url)
+        else:
+            data_key = find_between(
+                "/rdvxdata.s3.amazonaws.com/", "?AWSAccessKeyId=", url
+            )
 
         directory = os.path.dirname(data_key)
         full_dir = f"{out_dir}/{directory}"
         if not os.path.exists(full_dir):
             log.debug("Directory %s does not exist, creating it", full_dir)
             os.makedirs(full_dir)
```

### Comparing `redvox-3.4.2/redvox/cloud/metadata_api.py` & `redvox-3.5.0/redvox/cloud/metadata_api.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/cloud/query_timing_correction.py` & `redvox-3.5.0/redvox/cloud/query_timing_correction.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/cloud/routes.py` & `redvox-3.5.0/redvox/cloud/routes.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,8 +22,15 @@
     STATION_STATS: str = "/api/v1/metadata/stats"
 
 
 class RoutesV2:
     """
     Route definitions for version 2 of the RedVox Cloud API.
     """
+
     GEO_METADATA_REQ: str = "/api/v2/metadata/geo"
+
+
+class RoutesV3:
+    SESSION_MODEL: str = "/api/v3/session_model"
+    SESSION_MODELS: str = "/api/v3/session_models"
+    DYNAMIC_SESSION_MODEL: str = "/api/v3/dynamic_session_model"
```

### Comparing `redvox-3.4.2/redvox/cloud/station_stats.py` & `redvox-3.5.0/redvox/cloud/station_stats.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/cloud/subscription.py` & `redvox-3.5.0/redvox/cloud/subscription.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/common/api_conversions.py` & `redvox-3.5.0/redvox/common/api_conversions.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/common/api_reader.py` & `redvox-3.5.0/redvox/common/api_reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,34 +8,50 @@
 import multiprocessing.pool
 
 import pyarrow as pa
 import psutil
 
 import redvox.settings as settings
 import redvox.api1000.proto.redvox_api_m_pb2 as api_m
-from redvox.common import offset_model as om,\
-    io,\
-    api_conversions as ac,\
-    file_statistics as fs
+import redvox.common.date_time_utils as dtu
+from redvox.common import io, api_conversions as ac
 from redvox.common.parallel_utils import maybe_parallel_map
 from redvox.common.station import Station
 from redvox.common.session_model import SessionModel
 from redvox.common.errors import RedVoxExceptions
+from redvox.cloud.client import cloud_client
+from redvox.cloud.session_model_api import SessionModelsResp, Session
+from redvox.cloud.errors import CloudApiError
+
+
+id_py_stct = pa.struct(
+    [
+        ("id", pa.string()),
+        ("uuid", pa.string()),
+        ("start_time", pa.float64()),
+    ]
+)
+meta_py_stct = pa.struct(
+    [
+        ("api", pa.float64()),
+        ("sub_api", pa.float64()),
+        ("make", pa.string()),
+        ("model", pa.string()),
+        ("os", pa.int64()),
+        ("os_version", pa.string()),
+        ("app", pa.string()),
+        ("app_version", pa.string()),
+        ("is_private", pa.bool_()),
+        ("packet_duration_s", pa.float64()),
+        ("station_description", pa.string()),
+    ]
+)
 
 
-id_py_stct = pa.struct([("id", pa.string()), ("uuid", pa.string()), ("start_time", pa.float64()),
-                        ])
-meta_py_stct = pa.struct([("api", pa.float64()), ("sub_api", pa.float64()), ("make", pa.string()),
-                          ("model", pa.string()), ("os", pa.int64()), ("os_version", pa.string()),
-                          ("app", pa.string()), ("app_version", pa.string()), ("is_private", pa.bool_()),
-                          ("packet_duration_s", pa.float64()), ("station_description", pa.string()),
-                          ])
-
-
-PERCENT_FREE_MEM_USE = .8  # Percentage of total free memory to use when creating stations (1. is 100%)
+PERCENT_FREE_MEM_USE = 0.8  # Percentage of total free memory to use when creating stations (1. is 100%)
 
 
 class ApiReader:
     """
     Reads data from api 900 or api 1000 format, converting all data read into RedvoxPacketM for
     ease of comparison and use.
 
@@ -68,17 +84,15 @@
 
         :param base_dir: directory containing the files to read
         :param structured_dir: if True, base_dir contains a specific directory structure used by the respective
                                 api formats.  If False, base_dir only has the data files.  Default False.
         :param read_filter: ReadFilter for the data files, if None, get everything.  Default None
         :param debug: if True, output program warnings/errors during function execution.  Default False.
         """
-        _pool: multiprocessing.pool.Pool = (
-            multiprocessing.Pool() if pool is None else pool
-        )
+        _pool: multiprocessing.pool.Pool = multiprocessing.Pool() if pool is None else pool
 
         if read_filter:
             self.filter = read_filter
             if self.filter.station_ids:
                 self.filter.station_ids = set(self.filter.station_ids)
         else:
             self.filter = io.ReadFilter()
@@ -90,26 +104,34 @@
         self.index_summary = io.IndexSummary.from_index(self._flatten_files_index())
         if len(self.files_index) > 0:
             mem_split_factor = len(self.files_index) if settings.is_parallelism_enabled() else 1
             self.chunk_limit = psutil.virtual_memory().available * PERCENT_FREE_MEM_USE / mem_split_factor
             max_file_size = max([fe.decompressed_file_size_bytes for fi in self.files_index for fe in fi.entries])
             total_est_size = max_file_size * sum([len(fi.entries) for fi in self.files_index])
             if max_file_size > self.chunk_limit:
-                raise MemoryError(f"System requires {max_file_size} bytes of memory to process a file but only has "
-                                  f"{self.chunk_limit} available.  Please free or add more RAM.")
+                raise MemoryError(
+                    f"System requires {max_file_size} bytes of memory to process a file but only has "
+                    f"{self.chunk_limit} available.  Please free or add more RAM."
+                )
             elif total_est_size / mem_split_factor > self.chunk_limit:
-                raise MemoryError(f"{total_est_size} of data requested, but only {self.chunk_limit} available; "
-                                  f"please reduce the amount of data you are requesting.")
+                raise MemoryError(
+                    f"{total_est_size} of data requested, but only {self.chunk_limit} available; "
+                    f"please reduce the amount of data you are requesting."
+                )
             if debug:
                 if mem_split_factor == 1:
-                    print(f"{len(self.files_index)} stations have {int(self.chunk_limit)} "
-                          f"bytes for loading files in memory.")
+                    print(
+                        f"{len(self.files_index)} stations have {int(self.chunk_limit)} "
+                        f"bytes for loading files in memory."
+                    )
                 else:
-                    print(f"{mem_split_factor} stations each have "
-                          f"{int(self.chunk_limit)} bytes for loading files in memory.")
+                    print(
+                        f"{mem_split_factor} stations each have "
+                        f"{int(self.chunk_limit)} bytes for loading files in memory."
+                    )
         else:
             self.chunk_limit = 0
 
         if debug:
             self.errors.print()
 
         if pool is None:
@@ -117,34 +139,112 @@
 
     def _flatten_files_index(self):
         """
         :return: flattened version of files_index
         """
         result = io.Index()
         for i in self.files_index:
-            result.append(i.entries)
+            result.append(iter(i.entries))
         return result
 
-    def _get_all_files(
-        self, pool: Optional[multiprocessing.pool.Pool] = None
-    ) -> List[io.Index]:
+    def _get_cloud_models(self, ids: List[str]) -> SessionModelsResp:
+        try:
+            with cloud_client() as client:
+                resp: SessionModelsResp = client.request_session_models(
+                    owner=client.redvox_config.username,
+                    id_uuids=ids,
+                    start_ts=int(dtu.datetime_to_epoch_microseconds_utc(self.filter.start_dt))
+                    if self.filter.start_dt
+                    else None,
+                    end_ts=int(dtu.datetime_to_epoch_microseconds_utc(self.filter.end_dt))
+                    if self.filter.end_dt
+                    else None,
+                )
+                if len(resp.sessions) < 1:
+                    self.errors.append(
+                        "Unable to find sessions.  Check if the requested stations: belong to your "
+                        "account or are public."
+                    )
+                return resp
+        except CloudApiError as e:
+            self.errors.append(f"Error while connecting to server.  Error message: {e}")
+        except Exception as e:
+            self.errors.append(f"An error occurred.  Error message: {e}")
+
+    def _reset_index(self, model: Session) -> List[io.Index]:
+        """
+        reset the filter used to get files, then get the updated list of files
+
+        :param model: model to use to reset filter
+        :return: updated index of files
+        """
+        insufficient_str = ""
+        # reset the filter used to get files
+        new_filter = (
+            io.ReadFilter()
+            .with_extensions(self.filter.extensions)
+            .with_api_versions(self.filter.api_versions)
+            .with_station_ids({model.id})
+            .with_start_dt_buf(dtu.timedelta(seconds=0))
+            .with_end_dt_buf(dtu.timedelta(seconds=0))
+        )
+        # update the start and end times for the filter by the mean offset and the packet duration
+        if self.filter.start_dt is not None:
+            if timedelta(microseconds=abs(model.timing.mean_off)) > self.filter.start_dt_buf:
+                insufficient_str += "start "
+            new_filter.with_start_dt(
+                self.filter.start_dt + timedelta(microseconds=(model.timing.mean_off - model.packet_dur))
+            )
+        if self.filter.end_dt is not None:
+            if timedelta(microseconds=abs(model.timing.mean_off)) > self.filter.end_dt_buf:
+                insufficient_str += "end"
+            new_filter.with_end_dt(
+                self.filter.end_dt + timedelta(microseconds=(model.timing.mean_off + model.packet_dur))
+            )
+
+        if len(insufficient_str) > 0:
+            self.errors.append(f"Required more data for {model.id} at: {insufficient_str}")
+        return [self._apply_filter(new_filter)]
+
+    def _get_all_files(self, pool: Optional[multiprocessing.pool.Pool] = None) -> List[io.Index]:
         """
         get all files in the base dir of the ApiReader
 
         :return: index with all the files that match the filter
         """
-        _pool: multiprocessing.pool.Pool = (
-            multiprocessing.Pool() if pool is None else pool
-        )
+        _pool: multiprocessing.pool.Pool = multiprocessing.Pool() if pool is None else pool
         index: List[io.Index] = []
         # this guarantees that all ids we search for are valid
         all_index = self._apply_filter(pool=_pool)
-        for station_id in all_index.summarize().station_ids():
-            id_index = all_index.get_index_for_station_id(station_id)
-            checked_index = self._check_station_stats(id_index, pool=_pool)
+        all_index_ids = all_index.summarize().station_ids()
+        # get models using the cloud to correct timing
+        resp = self._get_cloud_models(all_index_ids)
+        resp_ids = [n.id for n in resp.sessions] if resp is not None else []
+
+        for station_id in all_index_ids:
+            # if start and end are both not defined, just use what we got
+            if self.filter.start_dt is None and self.filter.end_dt is None:
+                checked_index = [all_index.get_index_for_station_id(station_id)]
+            # if we need to update the start or end, use the first session model from cloud if it exists
+            elif station_id in resp_ids:
+                checked_index = self._reset_index([n for n in resp.sessions if n.id == station_id][0])
+            # if no models from cloud, use the data available to update start and end of index
+            else:
+                id_index = all_index.get_index_for_station_id(station_id)
+                if len(id_index.entries) < 1:
+                    checked_index = []
+                else:
+                    # attempt to make a session model using local data.  if failure, use what we got initially.
+                    try:
+                        stats = SessionModel().create_from_stream(self.read_files_in_index(id_index))
+                        checked_index = self._reset_index(stats.cloud_session)
+                    except Exception as e:
+                        checked_index = [id_index]
+
+            # add the updated list of files to the index
             index.extend(checked_index)
 
         if pool is None:
             _pool.close()
 
         return index
 
@@ -155,120 +255,50 @@
     ) -> io.Index:
         """
         apply the filter of the reader, or another filter if specified
 
         :param reader_filter: optional filter; if None, use the reader's filter, default None
         :return: index of the filtered files
         """
-        _pool: multiprocessing.pool.Pool = (
-            multiprocessing.Pool() if pool is None else pool
-        )
+        _pool: multiprocessing.pool.Pool = multiprocessing.Pool() if pool is None else pool
         if not reader_filter:
             reader_filter = self.filter
         if self.structured_dir:
             index = io.index_structured(self.base_dir, reader_filter, pool=_pool)
         else:
             index = io.index_unstructured(self.base_dir, reader_filter, pool=_pool)
         if pool is None:
             _pool.close()
         return index
 
-    def _redo_index(self, station_ids: set, new_start: datetime, new_end: datetime):
+    def _redo_index(self, station_ids: set, new_start: datetime, new_end: datetime) -> Optional[io.Index]:
         """
         Redo the index for files using new start and end dates.  removes any buffer time at the start and end of the
         new query.  Returns the updated index or None
 
         :param station_ids: set of ids to get
         :param new_start: new start time to get data from
         :param new_end: new end time to get data from
         :return: Updated index or None
         """
         diff_s = diff_e = timedelta(seconds=0)
-        new_index = self._apply_filter(io.ReadFilter()
-                                       .with_start_dt(new_start)
-                                       .with_end_dt(new_end)
-                                       .with_extensions(self.filter.extensions)
-                                       .with_api_versions(self.filter.api_versions)
-                                       .with_station_ids(station_ids)
-                                       .with_start_dt_buf(diff_s)
-                                       .with_end_dt_buf(diff_e))
+        new_index = self._apply_filter(
+            io.ReadFilter()
+            .with_start_dt(new_start)
+            .with_end_dt(new_end)
+            .with_extensions(self.filter.extensions)
+            .with_api_versions(self.filter.api_versions)
+            .with_station_ids(station_ids)
+            .with_start_dt_buf(diff_s)
+            .with_end_dt_buf(diff_e)
+        )
         if len(new_index.entries) > 0:
             return new_index
         return None
 
-    def _check_station_stats(
-            self,
-            station_index: io.Index,
-            pool: Optional[multiprocessing.pool.Pool] = None,
-    ) -> List[io.Index]:
-        """
-        check the index's results; if it has enough information, return it, otherwise search for more data.
-        The index should only request one station id
-        If the station was restarted during the request period, a new group of indexes will be created
-        to represent the change in station metadata.
-
-        :param station_index: index representing the requested information
-        :return: List of Indexes that includes as much information as possible that fits the request
-        """
-        _pool: multiprocessing.pool.Pool = multiprocessing.Pool() if pool is None else pool
-        # if we found nothing, return the index
-        if len(station_index.entries) < 1:
-            return [station_index]
-
-        stats = fs.extract_stats(station_index, pool=_pool)
-        # Close pool if created here
-        if pool is None:
-            _pool.close()
-
-        timing_offsets: Optional[om.TimingOffsets] = om.compute_offsets(stats)
-
-        # punt if duration or other important values are invalid or if the latency array was empty
-        if timing_offsets is None:
-            return [station_index]
-
-        # if our filtered files do not encompass the request even when the packet times are updated
-        # try getting the difference of the expected start/end and the start/end of the data plus one packet
-        insufficient_str = ""
-        if (self.filter.start_dt and timing_offsets.adjusted_start > self.filter.start_dt) or \
-                (self.filter.end_dt and timing_offsets.adjusted_start >= self.filter.end_dt):
-            insufficient_str += f" {self.filter.start_dt} (start)"
-            new_end = self.filter.start_dt - self.filter.start_dt_buf
-            new_start = new_end - (timing_offsets.adjusted_start - self.filter.start_dt + stats[0].packet_duration)
-            new_index = self._redo_index(set(station_index.summarize().station_ids()), new_start, new_end)
-            if new_index:
-                station_index.append(new_index.entries)
-                stats.extend(fs.extract_stats(new_index))
-
-        if (self.filter.end_dt and timing_offsets.adjusted_end < self.filter.end_dt) or \
-                (self.filter.start_dt and timing_offsets.adjusted_end <= self.filter.start_dt):
-            insufficient_str += f" {self.filter.end_dt} (end)"
-            new_start = self.filter.end_dt + self.filter.end_dt_buf
-            new_end = new_start + (self.filter.end_dt - timing_offsets.adjusted_end + stats[0].packet_duration)
-            new_index = self._redo_index(set(station_index.summarize().station_ids()), new_start, new_end)
-            if new_index:
-                station_index.append(new_index.entries)
-                stats.extend(fs.extract_stats(new_index))
-
-        if len(insufficient_str) > 0:
-            self.errors.append(f"Data for {station_index.summarize().station_ids()} exists, "
-                               f"but not at:{insufficient_str}")
-
-        results = {}
-        keys = []
-
-        for v, e in enumerate(stats):
-            key = e.app_start_dt
-            if key not in keys:
-                keys.append(key)
-                results[key] = io.Index()
-
-            results[key].append(entries=[station_index.entries[v]])
-
-        return list(results.values())
-
     def _split_workload(self, findex: io.Index) -> List[io.Index]:
         """
         takes an index and splits it into chunks based on a size limit
         while running_total + next_file_size < limit, adds files to a chunk (Index)
         if limit is exceeded, adds the chunk and puts the next file into a new chunk
 
         :param findex: index of files to split
@@ -295,27 +325,21 @@
         :return: list of RedvoxPacketM, converted from API 900 if necessary
         """
         result: List[api_m.RedvoxPacketM] = []
 
         # Iterate over the API 900 packets in a memory efficient way
         # and convert to API 1000
         # noinspection PyTypeChecker
-        for packet_900 in indexf.stream_raw(
-                io.ReadFilter.empty().with_api_versions({io.ApiVersion.API_900})
-        ):
+        for packet_900 in indexf.stream_raw(io.ReadFilter.empty().with_api_versions({io.ApiVersion.API_900})):
             # noinspection Mypy
-            result.append(
-                ac.convert_api_900_to_1000_raw(packet_900)
-            )
+            result.append(ac.convert_api_900_to_1000_raw(packet_900))
 
         # Grab the API 1000 packets
         # noinspection PyTypeChecker
-        for packet in indexf.stream_raw(
-                io.ReadFilter.empty().with_api_versions({io.ApiVersion.API_1000})
-        ):
+        for packet in indexf.stream_raw(io.ReadFilter.empty().with_api_versions({io.ApiVersion.API_1000})):
             # noinspection Mypy
             result.append(packet)
 
         return result
 
     # noinspection PyTypeChecker
     def read_files_by_id(self, station_id: str) -> Optional[List[api_m.RedvoxPacketM]]:
@@ -325,26 +349,22 @@
         """
 
         result: List[api_m.RedvoxPacketM] = []
 
         # Iterate over the API 900 packets in a memory efficient way
         # and convert to API 1000
         for packet_900 in self._flatten_files_index().stream_raw(
-            io.ReadFilter.empty()
-            .with_api_versions({io.ApiVersion.API_900})
-            .with_station_ids({station_id})
+            io.ReadFilter.empty().with_api_versions({io.ApiVersion.API_900}).with_station_ids({station_id})
         ):
             # noinspection Mypy
             result.append(ac.convert_api_900_to_1000_raw(packet_900))
 
         # Grab the API 1000 packets
         for packet in self._flatten_files_index().stream_raw(
-            io.ReadFilter.empty()
-            .with_api_versions({io.ApiVersion.API_1000})
-            .with_station_ids({station_id})
+            io.ReadFilter.empty().with_api_versions({io.ApiVersion.API_1000}).with_station_ids({station_id})
         ):
             # noinspection Mypy
             result.append(packet)
 
         if len(result) == 0:
             return None
 
@@ -358,20 +378,15 @@
         return Station.create_from_packets(self.read_files_in_index(findex))
 
     def get_stations(self, pool: Optional[multiprocessing.pool.Pool] = None) -> List[Station]:
         """
         :param pool: optional multiprocessing pool
         :return: List of all stations in the ApiReader
         """
-        return list(maybe_parallel_map(pool,
-                                       self._station_by_index,
-                                       self.files_index,
-                                       chunk_size=1
-                                       )
-                    )
+        return list(maybe_parallel_map(pool, self._station_by_index, iter(self.files_index), chunk_size=1))
 
     def get_station_by_id(self, get_id: str) -> Optional[List[Station]]:
         """
         :param get_id: the id to filter on
         :return: list of all stations with the requested id or None if id can't be found
         """
         result = [s for s in self.get_stations() if s.id() == get_id]
@@ -379,187 +394,188 @@
             return None
         return result
 
 
 # This class uses a slightly stripped down version of the above ApiReader meant to quickly create SessionModels.
 # Some of the checks used in ApiReader are not necessary when creating SessionModel, while the core functionality
 #  of finding and reading files remains.
-class ApiReaderModel:
-    """
-    Reads data from api 900 or api 1000 format, converting all data read into RedvoxPacketM for
-    ease of comparison and use.
-    Creates SessionModels for each station session within the data read.
-
-    Properties:
-        filter: io.ReadFilter with the station ids, start and end time, start and end time padding, and
-        types of files to read
-
-        base_dir: str of the directory containing all the files to read
-
-        structured_dir: bool, if True, the base_dir contains a specific directory structure used by the
-        respective api formats.  If False, base_dir only has the data files.  Default False.
-
-        files_index: io.Index of the files that match the filter that are in base_dir
-
-        index_summary: io.IndexSummary of the filtered data
-
-        debug: bool, if True, output additional information during function execution.  Default False.
-
-        errors: RedVoxExceptions, a container for any errors encountered during function execution.
-    """
-
-    def __init__(
-            self,
-            base_dir: str,
-            structured_dir: bool = False,
-            read_filter: io.ReadFilter = None,
-            debug: bool = False,
-            pool: Optional[multiprocessing.pool.Pool] = None,
-    ):
-        """
-        Initialize the ApiReader object
-
-        :param base_dir: directory containing the files to read
-        :param structured_dir: if True, base_dir contains a specific directory structure used by the respective
-                                api formats.  If False, base_dir only has the data files.  Default False.
-        :param read_filter: ReadFilter for the data files, if None, get everything.  Default None
-        :param debug: if True, output program warnings/errors during function execution.  Default False.
-        """
-        _pool: multiprocessing.pool.Pool = (
-            multiprocessing.Pool() if pool is None else pool
-        )
-
-        if read_filter:
-            self.filter = read_filter
-            if self.filter.station_ids:
-                self.filter.station_ids = set(self.filter.station_ids)
-        else:
-            self.filter = io.ReadFilter()
-        self.base_dir = base_dir
-        self.structured_dir = structured_dir
-        self.debug = debug
-        self.errors = RedVoxExceptions("APIReader")
-        self.session_models: List[SessionModel] = []
-        self.files_index = self._get_all_files(_pool)
-        self.index_summary = io.IndexSummary.from_index(self._flatten_files_index())
-
-        if debug:
-            self.errors.print()
-
-        if pool is None:
-            _pool.close()
-
-    def _flatten_files_index(self):
-        """
-        :return: flattened version of files_index
-        """
-        result = io.Index()
-        for i in self.files_index:
-            result.append(i.entries)
-        return result
-
-    def _get_session(self, s_id: str, uuid: str, start_date: float) -> Optional[SessionModel]:
-        """
-        get a session that matches all the inputs or None if no match
-
-        :param s_id: station id to get
-        :param uuid: station uuid to get
-        :param start_date: station start date to get
-        :return: SessionModel or None
-        """
-        for m in self.session_models:
-            if m.id == s_id and m.uuid == uuid and m.start_date == start_date:
-                return m
-        return None
-
-    def _get_all_files(
-            self, pool: Optional[multiprocessing.pool.Pool] = None
-    ) -> List[io.Index]:
-        """
-        get all files in the base dir of the ApiReader
-
-        :return: index with all the files that match the filter
-        """
-        _pool: multiprocessing.pool.Pool = (
-            multiprocessing.Pool() if pool is None else pool
-        )
-        index: List[io.Index] = []
-        # this guarantees that all ids we search for are valid
-        all_index = self._apply_filter(pool=_pool)
-        for station_id in all_index.summarize().station_ids():
-            id_index = all_index.get_index_for_station_id(station_id)
-            for f in id_index.read_contents():
-                sd = f.timing_information.app_start_mach_timestamp
-                uid = f.station_information.uuid
-                n = self._get_session(station_id, uid, sd)
-                n.add_data_from_packet(f) if n is not None \
-                    else self.session_models.append(SessionModel.create_from_packet(f))
-            index.append(id_index)
-
-        if pool is None:
-            _pool.close()
-
-        return index
-
-    def _apply_filter(
-            self,
-            reader_filter: Optional[io.ReadFilter] = None,
-            pool: Optional[multiprocessing.pool.Pool] = None,
-    ) -> io.Index:
-        """
-        apply the filter of the reader, or another filter if specified
-
-        :param reader_filter: optional filter; if None, use the reader's filter, default None
-        :return: index of the filtered files
-        """
-        _pool: multiprocessing.pool.Pool = (
-            multiprocessing.Pool() if pool is None else pool
-        )
-        if not reader_filter:
-            reader_filter = self.filter
-        if self.structured_dir:
-            index = io.index_structured(self.base_dir, reader_filter, pool=_pool)
-        else:
-            index = io.index_unstructured(self.base_dir, reader_filter, pool=_pool)
-        if pool is None:
-            _pool.close()
-        return index
-
-    def _check_station_stats(
-            self,
-            station_index: io.Index,
-            pool: Optional[multiprocessing.pool.Pool] = None,
-    ) -> List[io.Index]:
-        """
-        check the index's results; if it has enough information, return it, otherwise search for more data.
-        The index should only request one station id
-        If the station was restarted during the request period, a new group of indexes will be created
-        to represent the change in station metadata.
-        Creates SessionModels for each station session found in the requested data.
-
-        :param station_index: index representing the requested information
-        :return: List of Indexes that includes as much information as possible that fits the request
-        """
-        # if we found nothing, return the index
-        if len(station_index.entries) < 1:
-            return [station_index]
-
-        _pool: multiprocessing.pool.Pool = multiprocessing.Pool() if pool is None else pool
-
-        stats = fs.extract_stats(station_index, pool=_pool)
-        # Close pool if created here
-        if pool is None:
-            _pool.close()
-
-        results = {}
-
-        for v, e in enumerate(stats):
-            key = e.app_start_dt
-            if key not in results.keys():
-                results[key] = io.Index()
-            results[key].append(entries=[station_index.entries[v]])
-
-        for s in results.values():
-            m = SessionModel.create_from_stream(s.read_contents())
-            self.session_models.append(m)
-
-        return list(results.values())
+# class ApiReaderModel:
+#     """
+#     Reads data from api 900 or api 1000 format, converting all data read into RedvoxPacketM for
+#     ease of comparison and use.
+#     Creates SessionModels for each station session within the data read.
+#
+#     Properties:
+#         filter: io.ReadFilter with the station ids, start and end time, start and end time padding, and
+#         types of files to read
+#
+#         base_dir: str of the directory containing all the files to read
+#
+#         structured_dir: bool, if True, the base_dir contains a specific directory structure used by the
+#         respective api formats.  If False, base_dir only has the data files.  Default False.
+#
+#         files_index: io.Index of the files that match the filter that are in base_dir
+#
+#         index_summary: io.IndexSummary of the filtered data
+#
+#         debug: bool, if True, output additional information during function execution.  Default False.
+#
+#         errors: RedVoxExceptions, a container for any errors encountered during function execution.
+#     """
+#
+#     def __init__(
+#             self,
+#             base_dir: str,
+#             structured_dir: bool = False,
+#             read_filter: io.ReadFilter = None,
+#             debug: bool = False,
+#             pool: Optional[multiprocessing.pool.Pool] = None,
+#     ):
+#         """
+#         Initialize the ApiReader object
+#
+#         :param base_dir: directory containing the files to read
+#         :param structured_dir: if True, base_dir contains a specific directory structure used by the respective
+#                                 api formats.  If False, base_dir only has the data files.  Default False.
+#         :param read_filter: ReadFilter for the data files, if None, get everything.  Default None
+#         :param debug: if True, output program warnings/errors during function execution.  Default False.
+#         """
+#         _pool: multiprocessing.pool.Pool = (
+#             multiprocessing.Pool() if pool is None else pool
+#         )
+#
+#         if read_filter:
+#             self.filter = read_filter
+#             if self.filter.station_ids:
+#                 self.filter.station_ids = set(self.filter.station_ids)
+#         else:
+#             self.filter = io.ReadFilter()
+#         self.base_dir = base_dir
+#         self.structured_dir = structured_dir
+#         self.debug = debug
+#         self.errors = RedVoxExceptions("APIReader")
+#         self.session_models: List[SessionModel] = []
+#         self.files_index = self._get_all_files(_pool)
+#         self.index_summary = io.IndexSummary.from_index(self._flatten_files_index())
+#
+#         if debug:
+#             self.errors.print()
+#
+#         if pool is None:
+#             _pool.close()
+#
+#     def _flatten_files_index(self):
+#         """
+#         :return: flattened version of files_index
+#         """
+#         result = io.Index()
+#         for i in self.files_index:
+#             result.append(iter(i.entries))
+#         return result
+#
+#     def _get_session(self, s_id: str, uuid: str, start_date: float) -> Optional[SessionModel]:
+#         """
+#         get a session that matches all the inputs or None if no match
+#
+#         :param s_id: station id to get
+#         :param uuid: station uuid to get
+#         :param start_date: station start date to get
+#         :return: SessionModel or None
+#         """
+#         for m in self.session_models:
+#             if m.cloud_session.id == s_id and m.cloud_session.uuid == uuid and
+#             m.cloud_session.start_date == start_date:
+#                 return m
+#         return None
+#
+#     def _get_all_files(
+#             self, pool: Optional[multiprocessing.pool.Pool] = None
+#     ) -> List[io.Index]:
+#         """
+#         get all files in the base dir of the ApiReader
+#
+#         :return: index with all the files that match the filter
+#         """
+#         _pool: multiprocessing.pool.Pool = (
+#             multiprocessing.Pool() if pool is None else pool
+#         )
+#         index: List[io.Index] = []
+#         # this guarantees that all ids we search for are valid
+#         all_index = self._apply_filter(pool=_pool)
+#         for station_id in all_index.summarize().station_ids():
+#             id_index = all_index.get_index_for_station_id(station_id)
+#             for f in id_index.read_contents():
+#                 sd = f.timing_information.app_start_mach_timestamp
+#                 uid = f.station_information.uuid
+#                 n = self._get_session(station_id, uid, sd)
+#                 n.create_from_packet(f) if n is not None \
+#                     else self.session_models.append(SessionModel.create_from_packet(f))
+#             index.append(id_index)
+#
+#         if pool is None:
+#             _pool.close()
+#
+#         return index
+#
+#     def _apply_filter(
+#             self,
+#             reader_filter: Optional[io.ReadFilter] = None,
+#             pool: Optional[multiprocessing.pool.Pool] = None,
+#     ) -> io.Index:
+#         """
+#         apply the filter of the reader, or another filter if specified
+#
+#         :param reader_filter: optional filter; if None, use the reader's filter, default None
+#         :return: index of the filtered files
+#         """
+#         _pool: multiprocessing.pool.Pool = (
+#             multiprocessing.Pool() if pool is None else pool
+#         )
+#         if not reader_filter:
+#             reader_filter = self.filter
+#         if self.structured_dir:
+#             index = io.index_structured(self.base_dir, reader_filter, pool=_pool)
+#         else:
+#             index = io.index_unstructured(self.base_dir, reader_filter, pool=_pool)
+#         if pool is None:
+#             _pool.close()
+#         return index
+#
+#     def _check_station_stats(
+#             self,
+#             station_index: io.Index,
+#             pool: Optional[multiprocessing.pool.Pool] = None,
+#     ) -> List[io.Index]:
+#         """
+#         check the index's results; if it has enough information, return it, otherwise search for more data.
+#         The index should only request one station id
+#         If the station was restarted during the request period, a new group of indexes will be created
+#         to represent the change in station metadata.
+#         Creates SessionModels for each station session found in the requested data.
+#
+#         :param station_index: index representing the requested information
+#         :return: List of Indexes that includes as much information as possible that fits the request
+#         """
+#         # if we found nothing, return the index
+#         if len(station_index.entries) < 1:
+#             return [station_index]
+#
+#         _pool: multiprocessing.pool.Pool = multiprocessing.Pool() if pool is None else pool
+#
+#         stats = fs.extract_stats(station_index, pool=_pool)
+#         # Close pool if created here
+#         if pool is None:
+#             _pool.close()
+#
+#         results = {}
+#
+#         for v, e in enumerate(stats):
+#             key = e.app_start_dt
+#             if key not in results.keys():
+#                 results[key] = io.Index()
+#             results[key].append(entries=iter([station_index.entries[v]]))
+#
+#         for s in results.values():
+#             m = SessionModel.create_from_stream(s.read_contents())
+#             self.session_models.append(m)
+#
+#         return list(results.values())
```

### Comparing `redvox-3.4.2/redvox/common/api_reader_dw.py` & `redvox-3.5.0/redvox/common/api_reader_dw.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,87 +1,93 @@
 """
 For use with DataWindow specifically.  Do NOT use with non-DataWindow objects
 Read Redvox data from a single directory
 Data files can be either API 900 or API 1000 data formats
 """
 from typing import List, Optional
 import multiprocessing.pool
+
 import numpy as np
 
 import redvox.settings as settings
 from redvox.common import io
 from redvox.common.api_reader import ApiReader
 from redvox.common.parallel_utils import maybe_parallel_map
 from redvox.common.station import Station
 
 
 class ApiReaderDw(ApiReader):
     """
     For use with DataWindow specifically.  Do NOT use with non-DataWindow objects
     """
-    def __init__(self,
-                 base_dir: str,
-                 structured_dir: bool = False,
-                 read_filter: io.ReadFilter = None,
-                 correct_timestamps: bool = False,
-                 use_model_correction: bool = True,
-                 dw_base_dir: str = ".",
-                 dw_save_mode: io.FileSystemSaveMode = io.FileSystemSaveMode.TEMP,
-                 debug: bool = False,
-                 pool: Optional[multiprocessing.pool.Pool] = None):
+
+    def __init__(
+        self,
+        base_dir: str,
+        structured_dir: bool = False,
+        read_filter: io.ReadFilter = None,
+        correct_timestamps: bool = False,
+        use_model_correction: bool = True,
+        dw_base_dir: str = ".",
+        dw_save_mode: io.FileSystemSaveMode = io.FileSystemSaveMode.TEMP,
+        debug: bool = False,
+        pool: Optional[multiprocessing.pool.Pool] = None,
+    ):
         """
         initialize API reader for data window
 
         :param base_dir: directory containing the files to read
         :param structured_dir: if True, base_dir contains a specific directory structure used by the respective
                                 api formats.  If False, base_dir only has the data files.  Default False.
         :param read_filter: ReadFilter for the data files, if None, get everything.  Default None
         :param correct_timestamps: if True, correct the timestamps of the data.  Default False
         :param use_model_correction: if True, use the offset model of the station to correct the timestamps.
                                         if correct_timestamps is False, this value doesn't matter.  Default True
-        :param dw_base_dir: the directory to save DataWindow files to.  if save_mode is FileSystemSaveMode.MEM,
+        :param dw_base_dir: the directory to save DataWindow files to.  if dw_save_mode is "FileSystemSaveMode.MEM",
                             this value doesn't matter.  default "." (current directory)
-        :param dw_save_mode: save method for the data window.  Default FileSystemSaveMode.TEMP which saves to a temp_dir
+        :param dw_save_mode: save method for the data window.  Default "FileSystemSaveMode.TEMP"; save to temp_dir
         :param debug: if True, output program warnings/errors during function execution.  Default False.
         """
         super().__init__(base_dir, structured_dir, read_filter, debug, pool)
         self.correct_timestamps = correct_timestamps
         self.use_model_correction = use_model_correction
         self.dw_base_dir = dw_base_dir
         self.dw_save_mode = dw_save_mode
         self.all_files_size = np.sum([idx.files_size() for idx in self.files_index])
         self._stations = self._read_stations()
 
     def _station_by_index(self, findex: io.Index) -> Station:
         """
         builds station using the index of files to read
+
         splits the index into smaller chunks if entire record cannot be held in memory
 
         :param findex: index with files to build a station with
         :return: Station built from files in findex, without building the data from parquet
         """
         split_list = self._split_workload(findex)
         use_temp_dir = True if len(split_list) > 1 else False
 
         if len(split_list) > 0:
             if self.debug and use_temp_dir:
-                print("Writing data to disk; this may take a few minutes to complete.")
-            stpa = Station.create_from_indexes(split_list,
-                                               correct_timestamps=self.correct_timestamps,
-                                               use_model_correction=self.use_model_correction,
-                                               base_out_dir=self.dw_base_dir,
-                                               use_temp_dir=use_temp_dir
-                                               )
+                print("Writing data to temporary disk; this may take a few minutes to complete.")
+            station_from_index = Station.create_from_indexes(
+                split_list,
+                correct_timestamps=self.correct_timestamps,
+                use_model_correction=self.use_model_correction,
+                base_out_dir=self.dw_base_dir,
+                use_temp_dir=use_temp_dir,
+            )
             if self.debug:
-                print(f"station {stpa.id()} files read: {len(findex.entries)}")
+                print(f"station {station_from_index.id()} files read: {len(findex.entries)}")
                 if len(split_list) > 1:
                     print(f"required making {len(split_list)} smaller segments due to memory restraints")
             if self.dw_save_mode == io.FileSystemSaveMode.MEM and use_temp_dir:
                 self.dw_save_mode = io.FileSystemSaveMode.TEMP
-            return stpa
+            return station_from_index
         self.errors.append("No files found to create station.")
         return Station()
 
     def get_stations(self, pool: Optional[multiprocessing.pool.Pool] = None) -> List[Station]:
         """
         :return: a list of stations read by the ApiReader
         """
@@ -89,18 +95,15 @@
 
     def _read_stations(self, pool: Optional[multiprocessing.pool.Pool] = None) -> List[Station]:
         """
         :param pool: optional multiprocessing pool
         :return: List of all stations in the ApiReader, without building the data from parquet
         """
         if settings.is_parallelism_enabled() and len(self.files_index) > 1:
-            return list(maybe_parallel_map(pool, self._station_by_index,
-                                           self.files_index,
-                                           chunk_size=1
-                                           ))
+            return list(maybe_parallel_map(pool, self._station_by_index, self.files_index, chunk_size=1))
         return list(map(self._station_by_index, self.files_index))
 
     def get_station_by_id(self, get_id: str) -> Optional[List[Station]]:
         """
         :param get_id: the id to filter on
         :return: list of all stations with the requested id or None if id can't be found
         """
```

### Comparing `redvox-3.4.2/redvox/common/constants.py` & `redvox-3.5.0/redvox/common/constants.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/common/cross_stats.py` & `redvox-3.5.0/redvox/common/cross_stats.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/common/data_window.py` & `redvox-3.5.0/redvox/common/data_window.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,46 +1,43 @@
 """
 This module creates specific time-bounded segments of data for users
 combines the base data files into a single composite object based on the user parameters
 """
 from pathlib import Path
 from typing import Optional, Set, List, Dict, Iterable
 from datetime import timedelta
+from dataclasses import dataclass
+from dataclasses_json import dataclass_json
 import shutil
 import os
 import inspect
-from redvox.common import run_me
 
 import pprint
 import multiprocessing
 import multiprocessing.pool
 import numpy as np
 import pyarrow as pa
 
 import redvox
-from redvox.common import date_time_utils as dtu
-from redvox.common.date_time_utils import (
-    datetime_to_epoch_microseconds_utc as us_dt,
-)
-from redvox.common import io
-from redvox.common import data_window_io as dw_io
+from redvox.common import run_me, io, data_window_io as dw_io, date_time_utils as dtu, gap_and_pad_utils as gpu
 from redvox.common.data_window_configuration import DataWindowConfigFile
 from redvox.common.parallel_utils import maybe_parallel_map
 from redvox.common.station import Station, STATION_ID_LENGTH
 from redvox.common.sensor_data import SensorType, SensorData
 from redvox.common.api_reader_dw import ApiReaderDw
-from redvox.common import gap_and_pad_utils as gpu
 from redvox.common.errors import RedVoxExceptions
 
 DEFAULT_START_BUFFER_TD: timedelta = timedelta(minutes=2.0)  # default padding to start time of data
 DEFAULT_END_BUFFER_TD: timedelta = timedelta(minutes=2.0)  # default padding to end time of data
 # minimum default length of time in seconds for data to be off by to be considered suspicious
 DATA_DROP_DURATION_S: float = 0.2
 
 
+@dataclass_json
+@dataclass
 class EventOrigin:
     """
     The origin event's latitude, longitude, altitude and their standard deviations, the device used to measure
     the location data and the radius of the event
 
     Properties:
         provider: str, source of the location data (i.e. "GPS" or "NETWORK"), default "UNKNOWN"
@@ -55,68 +52,23 @@
 
         altitude: float, best estimate of altitude in meters, default np.nan
 
         altitude_std: float, standard deviation of best estimate of altitude, default np.nan
 
         event_radius_m: float, radius of event in meters, default 0.0
     """
-    def __init__(self,
-                 provider: str = "UNKNOWN",
-                 lat: float = np.nan,
-                 lat_std: float = np.nan,
-                 lon: float = np.nan,
-                 lon_std: float = np.nan,
-                 alt: float = np.nan,
-                 alt_std: float = np.nan,
-                 event_radius_m: float = 0.0):
-        """
-        :param provider: name of device that provided the information
-        :param lat: latitude in +/- degrees
-        :param lat_std: standard deviation of latitude
-        :param lon: longitude in +/- degrees
-        :param lon_std: standard deviation of longitude
-        :param alt: altitude in meters
-        :param alt_std: standard deviation of altitude
-        :param event_radius_m: radius of event in meters
-        """
-        self.provider = provider
-        self.latitude = lat
-        self.longitude = lon
-        self.altitude = alt
-        self.latitude_std = lat_std
-        self.longitude_std = lon_std
-        self.altitude_std = alt_std
-        self.event_radius_m = event_radius_m
 
-    def __repr__(self):
-        return str(self.as_dict())
-
-    def __str__(self):
-        return str(self.as_dict())
-
-    def as_dict(self) -> Dict:
-        """
-        :return: self as dict
-        """
-        return {
-            "provider": self.provider,
-            "latitude": self.latitude,
-            "latitude_std": self.latitude_std,
-            "longitude": self.longitude,
-            "longitude_std": self.longitude_std,
-            "altitude": self.altitude,
-            "altitude_std": self.altitude_std,
-            "event_radius_m": self.event_radius_m
-        }
-
-    @staticmethod
-    def from_dict(data_dict: Dict) -> "EventOrigin":
-        return EventOrigin(data_dict["provider"], data_dict["latitude"], data_dict["latitude_std"],
-                           data_dict["longitude"], data_dict["longitude_std"], data_dict["altitude"],
-                           data_dict["altitude_std"], data_dict["event_radius_m"])
+    provider: str = "UNKNOWN"
+    latitude: float = np.nan
+    latitude_std: float = np.nan
+    longitude: float = np.nan
+    longitude_std: float = np.nan
+    altitude: float = np.nan
+    altitude_std: float = np.nan
+    event_radius_m: float = 0.0
 
 
 class DataWindowConfig:
     """
     Configuration of DataWindow properties
 
     Properties:
@@ -137,15 +89,16 @@
         end_buffer_td: timedelta, the amount of time to include after the end_datetime when filtering data.
         Negative values are converted to 0.  Default DEFAULT_END_BUFFER_TD (2 minutes)
 
         drop_time_s: float, the minimum amount of seconds between data files that would indicate a gap.
         Negative values are converted to default value.  Default DATA_DROP_DURATION_S (0.2 seconds)
 
         station_ids: optional set of strings, representing the station ids to filter on.
-        If empty or None, get any ids found in the input directory.  Default None
+        If empty or None, get any ids found in the input directory.  You may pass in any iterable, as long as it can be
+        turned into a set.  Default None
 
         extensions: optional set of strings, representing file extensions to filter on.
         If None, gets as much data as it can in the input directory.  Default None
 
         api_versions: optional set of ApiVersions, representing api versions to filter on.
         If None, get as much data as it can in the input directory.  Default None
 
@@ -153,112 +106,130 @@
 
         copy_edge_points: enumeration of DataPointCreationMode.  Determines how new points are created.
         Valid values are NAN, COPY, and INTERPOLATE.  Default COPY
 
         use_model_correction: bool, if True, use the offset model's correction functions, otherwise use the best
         offset.  Default True
     """
+
     def __init__(
-            self,
-            input_dir: str,
-            structured_layout: bool = True,
-            start_datetime: Optional[dtu.datetime] = None,
-            end_datetime: Optional[dtu.datetime] = None,
-            start_buffer_td: timedelta = DEFAULT_START_BUFFER_TD,
-            end_buffer_td: timedelta = DEFAULT_END_BUFFER_TD,
-            drop_time_s: float = DATA_DROP_DURATION_S,
-            station_ids: Optional[Iterable[str]] = None,
-            extensions: Optional[Set[str]] = None,
-            api_versions: Optional[Set[io.ApiVersion]] = None,
-            apply_correction: bool = True,
-            use_model_correction: bool = True,
-            copy_edge_points: gpu.DataPointCreationMode = gpu.DataPointCreationMode.COPY,
+        self,
+        input_dir: str,
+        structured_layout: bool = True,
+        start_datetime: Optional[dtu.datetime] = None,
+        end_datetime: Optional[dtu.datetime] = None,
+        start_buffer_td: timedelta = DEFAULT_START_BUFFER_TD,
+        end_buffer_td: timedelta = DEFAULT_END_BUFFER_TD,
+        drop_time_s: float = DATA_DROP_DURATION_S,
+        station_ids: Optional[Iterable[str]] = None,
+        extensions: Optional[Set[str]] = None,
+        api_versions: Optional[Set[io.ApiVersion]] = None,
+        apply_correction: bool = True,
+        use_model_correction: bool = True,
+        copy_edge_points: gpu.DataPointCreationMode = gpu.DataPointCreationMode.COPY,
     ):
         self.input_dir: str = input_dir
         self.structured_layout: bool = structured_layout
         self.start_datetime: Optional[dtu.datetime] = start_datetime
         self.end_datetime: Optional[dtu.datetime] = end_datetime
-        self.start_buffer_td: timedelta = start_buffer_td if start_buffer_td > timedelta(seconds=0) \
-            else timedelta(seconds=0)
-        self.end_buffer_td: timedelta = end_buffer_td if end_buffer_td > timedelta(seconds=0) \
-            else timedelta(seconds=0)
+        self.start_buffer_td: timedelta = (
+            start_buffer_td if start_buffer_td > timedelta(seconds=0) else timedelta(seconds=0)
+        )
+        self.end_buffer_td: timedelta = end_buffer_td if end_buffer_td > timedelta(seconds=0) else timedelta(seconds=0)
         self.drop_time_s: float = drop_time_s if drop_time_s > 0 else DATA_DROP_DURATION_S
         self.station_ids: Optional[Set[str]] = set(station_ids) if station_ids else None
         self.extensions: Optional[Set[str]] = extensions
         self.api_versions: Optional[Set[io.ApiVersion]] = api_versions
         self.apply_correction: bool = apply_correction
         self.use_model_correction = use_model_correction
         self.copy_edge_points = copy_edge_points
 
     def __repr__(self):
-        return f"input_dir: {self.input_dir}, " \
-               f"structured_layout: {self.structured_layout}, " \
-               f"start_datetime: {self.start_datetime.__repr__()}, " \
-               f"end_datetime: {self.end_datetime.__repr__()}, " \
-               f"start_buffer_td: {self.start_buffer_td.__repr__()}, " \
-               f"end_buffer_td: {self.end_buffer_td.__repr__()}, " \
-               f"drop_time_s: {self.drop_time_s}, " \
-               f"station_ids: {list(self.station_ids) if self.station_ids else []}, " \
-               f"extensions: {list(self.extensions) if self.extensions else []}, " \
-               f"api_versions: {[a_v.value for a_v in self.api_versions] if self.api_versions else []}, " \
-               f"apply_correction: {self.apply_correction}, " \
-               f"use_model_correction: {self.use_model_correction}, " \
-               f"copy_edge_points: {self.copy_edge_points.value}"
+        return (
+            f"input_dir: {self.input_dir}, "
+            f"structured_layout: {self.structured_layout}, "
+            f"start_datetime: {self.start_datetime.__repr__()}, "
+            f"end_datetime: {self.end_datetime.__repr__()}, "
+            f"start_buffer_td: {self.start_buffer_td.__repr__()}, "
+            f"end_buffer_td: {self.end_buffer_td.__repr__()}, "
+            f"drop_time_s: {self.drop_time_s}, "
+            f"station_ids: {list(self.station_ids) if self.station_ids else []}, "
+            f"extensions: {list(self.extensions) if self.extensions else []}, "
+            f"api_versions: {[a_v.value for a_v in self.api_versions] if self.api_versions else []}, "
+            f"apply_correction: {self.apply_correction}, "
+            f"use_model_correction: {self.use_model_correction}, "
+            f"copy_edge_points: {self.copy_edge_points.value}"
+        )
 
     def __str__(self):
-        return f"input_dir: {self.input_dir}, " \
-               f"structured_layout: {self.structured_layout}, " \
-               f"start_datetime: " \
-               f"{self.start_datetime.strftime('%Y-%m-%dT%H:%M:%S.%fZ') if self.start_datetime else None}, " \
-               f"end_datetime: {self.end_datetime.strftime('%Y-%m-%dT%H:%M:%S.%fZ') if self.end_datetime else None}, " \
-               f"start_buffer_td (in s): {self.start_buffer_td.total_seconds()}, " \
-               f"end_buffer_td (in s): {self.end_buffer_td.total_seconds()}, " \
-               f"drop_time_s: {self.drop_time_s}, " \
-               f"station_ids: {list(self.station_ids) if self.station_ids else []}, " \
-               f"extensions: {list(self.extensions) if self.extensions else []}, " \
-               f"api_versions: {[a_v.value for a_v in self.api_versions] if self.api_versions else []}, " \
-               f"apply_correction: {self.apply_correction}, " \
-               f"use_model_correction: {self.use_model_correction}, " \
-               f"copy_edge_points: {self.copy_edge_points.name}"
+        return (
+            f"input_dir: {self.input_dir}, "
+            f"structured_layout: {self.structured_layout}, "
+            f"start_datetime: "
+            f"{self.start_datetime.strftime('%Y-%m-%dT%H:%M:%S.%fZ') if self.start_datetime else None}, "
+            f"end_datetime: {self.end_datetime.strftime('%Y-%m-%dT%H:%M:%S.%fZ') if self.end_datetime else None}, "
+            f"start_buffer_td (in s): {self.start_buffer_td.total_seconds()}, "
+            f"end_buffer_td (in s): {self.end_buffer_td.total_seconds()}, "
+            f"drop_time_s: {self.drop_time_s}, "
+            f"station_ids: {list(self.station_ids) if self.station_ids else []}, "
+            f"extensions: {list(self.extensions) if self.extensions else []}, "
+            f"api_versions: {[a_v.value for a_v in self.api_versions] if self.api_versions else []}, "
+            f"apply_correction: {self.apply_correction}, "
+            f"use_model_correction: {self.use_model_correction}, "
+            f"copy_edge_points: {self.copy_edge_points.name}"
+        )
 
-    def as_dict(self) -> Dict:
-        return {"input_dir": self.input_dir,
-                "structured_layout": self.structured_layout,
-                "start_datetime": us_dt(self.start_datetime),
-                "end_datetime": us_dt(self.end_datetime),
-                "start_buffer_td": self.start_buffer_td.total_seconds(),
-                "end_buffer_td": self.end_buffer_td.total_seconds(),
-                "drop_time_s": self.drop_time_s,
-                "station_ids": list(self.station_ids) if self.station_ids else [],
-                "extensions": list(self.extensions) if self.extensions else [],
-                "api_versions": [a_v.value for a_v in self.api_versions] if self.api_versions else [],
-                "apply_correction": self.apply_correction,
-                "use_model_correction": self.use_model_correction,
-                "copy_edge_points": self.copy_edge_points.value
-                }
+    def to_dict(self) -> Dict:
+        return {
+            "input_dir": self.input_dir,
+            "structured_layout": self.structured_layout,
+            "start_datetime": dtu.datetime_to_epoch_microseconds_utc(self.start_datetime)
+            if self.start_datetime
+            else None,
+            "end_datetime": dtu.datetime_to_epoch_microseconds_utc(self.end_datetime) if self.end_datetime else None,
+            "start_buffer_td": self.start_buffer_td.total_seconds(),
+            "end_buffer_td": self.end_buffer_td.total_seconds(),
+            "drop_time_s": self.drop_time_s,
+            "station_ids": list(self.station_ids) if self.station_ids else [],
+            "extensions": list(self.extensions) if self.extensions else [],
+            "api_versions": [a_v.value for a_v in self.api_versions] if self.api_versions else [],
+            "apply_correction": self.apply_correction,
+            "use_model_correction": self.use_model_correction,
+            "copy_edge_points": self.copy_edge_points.value,
+        }
 
     @staticmethod
     def from_dict(data_dict: Dict) -> "DataWindowConfig":
-        return DataWindowConfig(data_dict["input_dir"], data_dict["structured_layout"],
-                                dtu.datetime_from_epoch_microseconds_utc(data_dict["start_datetime"]),
-                                dtu.datetime_from_epoch_microseconds_utc(data_dict["end_datetime"]),
-                                timedelta(seconds=data_dict["start_buffer_td"]),
-                                timedelta(seconds=data_dict["end_buffer_td"]),
-                                data_dict["drop_time_s"], data_dict["station_ids"], set(data_dict["extensions"]),
-                                set([io.ApiVersion.from_str(v) for v in data_dict["api_versions"]]),
-                                data_dict["apply_correction"], data_dict["use_model_correction"],
-                                gpu.DataPointCreationMode(data_dict["copy_edge_points"])
-                                )
+        return DataWindowConfig(
+            data_dict["input_dir"],
+            data_dict["structured_layout"],
+            dtu.datetime_from_epoch_microseconds_utc(data_dict["start_datetime"])
+            if data_dict["start_datetime"]
+            else None,
+            dtu.datetime_from_epoch_microseconds_utc(data_dict["end_datetime"]) if data_dict["end_datetime"] else None,
+            timedelta(seconds=data_dict["start_buffer_td"]),
+            timedelta(seconds=data_dict["end_buffer_td"]),
+            data_dict["drop_time_s"],
+            data_dict["station_ids"],
+            set(data_dict["extensions"]),
+            set([io.ApiVersion.from_str(v) for v in data_dict["api_versions"]]),
+            data_dict["apply_correction"],
+            data_dict["use_model_correction"],
+            gpu.DataPointCreationMode(data_dict["copy_edge_points"]),
+        )
 
 
 class DataWindow:
     """
     Holds the data for a given time window; adds interpolated timestamps to fill gaps and pad the start and end values
+
     If a start time is given, data starting from that time will be included.
+
     If an end time is given, data up to but not including that time will be included.
+
     Refer to the DataWindowConfig class for more details on DataWindow parameters.
 
     Properties:
         event_name: str, name of the DataWindow.  defaults to "dw"
 
         event_origin: Optional EventOrigin which describes the physical location and radius of the
         origin event.  Default empty EventOrigin (no valid data)
@@ -268,82 +239,88 @@
 
         sdk_version: str, the version of the Redvox SDK used to create the DataWindow
 
         debug: bool, if True, outputs additional information during initialization. Default False
 
     Protected:
         _fs_writer: DataWindowFileSystemWriter; includes event_name, output directory (Default "."),
-        output type (options: "PARQUET", "LZ4", "NONE".  Default NONE), and option to make a
+        output type (options: "PARQUET", "LZ4", "JSON", "NONE".  Default NONE), and option to make a
         runme.py example file (Default False)
 
         _stations: List of Stations that belong to the DataWindow
 
         _errors: RedVoxExceptions; contains a list of all errors encountered by the DataWindow
     """
+
     def __init__(
-            self,
-            event_name: str = "dw",
-            event_origin: Optional[EventOrigin] = None,
-            config: Optional[DataWindowConfig] = None,
-            output_dir: str = ".",
-            out_type: str = "NONE",
-            make_runme: bool = False,
-            debug: bool = False,
+        self,
+        event_name: str = "dw",
+        event_origin: Optional[EventOrigin] = None,
+        config: Optional[DataWindowConfig] = None,
+        output_dir: str = ".",
+        out_type: str = "NONE",
+        make_runme: bool = False,
+        debug: bool = False,
     ):
         """
         Initialize the DataWindow
 
         :param event_name: name of the DataWindow.  defaults to "dw"
         :param event_origin: Optional EventOrigin which describes the physical location and radius of the
                                 origin event.  Default empty EventOrigin (no valid data)
         :param config: Optional DataWindowConfig which describes how to extract data from Redvox files.
                         Default None
         :param output_dir: output directory for saving files.  Default "." (current directory)
-        :param out_type: type of file to save the DataWindow as.  Options: "PARQUET", "LZ4", "NONE".
+        :param out_type: type of file to save the DataWindow as.  Options: "PARQUET", "LZ4", "JSON", "NONE".
                             Default "NONE" (no saving)
         :param make_runme: if True, saves an example runme.py file with the data.  Default False
         :param debug: if True, outputs additional information during initialization.  Default False
         """
         self.event_name: str = event_name
         self.event_origin: EventOrigin = event_origin if event_origin else EventOrigin()
         self._fs_writer = dw_io.DataWindowFileSystemWriter(self.event_name, out_type, output_dir, make_runme)
         self.debug: bool = debug
         self._sdk_version: str = redvox.VERSION
         self._errors = RedVoxExceptions("DataWindow")
         self._stations: List[Station] = []
         self._config = config
         if config:
             if config.start_datetime and config.end_datetime and (config.end_datetime <= config.start_datetime):
-                self._errors.append("DataWindow will not work when end datetime is before or equal to start datetime.\n"
-                                    f"Your times: {config.end_datetime} <= {config.start_datetime}")
+                self._errors.append(
+                    "DataWindow will not work when end datetime is before or equal to start datetime.\n"
+                    f"Your times: {config.end_datetime} <= {config.start_datetime}"
+                )
             else:
                 self.create_data_window()
         if self.debug:
             self.print_errors()
 
     def __repr__(self):
-        return f"event_name: {self.event_name}, " \
-               f"event_origin: {self.event_origin.__repr__()}, " \
-               f"config: {self._config.__repr__()}, " \
-               f"output_dir: {os.path.abspath(self.save_dir())}, " \
-               f"out_type: {self._fs_writer.file_extension}, " \
-               f"make_runme: {self._fs_writer.make_run_me}, " \
-               f"sdk_version: {self._sdk_version}, " \
-               f"debug: {self.debug}"
+        return (
+            f"event_name: {self.event_name}, "
+            f"event_origin: {self.event_origin.__repr__()}, "
+            f"config: {self._config.__repr__()}, "
+            f"output_dir: {os.path.abspath(self.save_dir())}, "
+            f"out_type: {self._fs_writer.file_extension}, "
+            f"make_runme: {self._fs_writer.make_run_me}, "
+            f"sdk_version: {self._sdk_version}, "
+            f"debug: {self.debug}"
+        )
 
     def __str__(self):
-        return f"event_name: {self.event_name}, " \
-               f"event_origin: {self.event_origin.__str__()}, " \
-               f"config: {self._config.__str__()}, " \
-               f"output_dir: {os.path.abspath(self.save_dir())}, " \
-               f"out_type: {self._fs_writer.file_extension}, " \
-               f"make_runme: {self._fs_writer.make_run_me}, " \
-               f"sdk_version: {self._sdk_version}, " \
-               f"debug: {self.debug}"
-        # "stations": [s.__str__() for s in self._stations],
+        return (
+            f"event_name: {self.event_name}, "
+            f"event_origin: {self.event_origin.__str__()}, "
+            f"config: {self._config.__str__()}, "
+            f"output_dir: {os.path.abspath(self.save_dir())}, "
+            f"out_type: {self._fs_writer.file_extension}, "
+            f"make_runme: {self._fs_writer.make_run_me}, "
+            f"sdk_version: {self._sdk_version}, "
+            f"debug: {self.debug}"
+        )
 
     def save_dir(self) -> str:
         """
         :return: directory data is saved to (empty string means saving to memory)
         """
         return self._fs_writer.save_dir()
 
@@ -375,37 +352,39 @@
         """
         :return: string of the output type of the DataWindow
         """
         return self._fs_writer.file_extension
 
     def set_out_type(self, new_out_type: str):
         """
-        set the output type of the DataWindow.  options are "NONE", "PARQUET" and "LZ4".  invalid values become "NONE"
+        set the output type of the DataWindow.  options are "NONE", "PARQUET", "LZ4" and "JSON".
+        Invalid values become "NONE"
 
         :param new_out_type: new output type of the DataWindow
         """
         self._fs_writer.set_extension(new_out_type)
 
     def as_dict(self) -> Dict:
         """
         :return: DataWindow properties as dictionary
         """
-        return {"event_name": self.event_name,
-                "event_origin": self.event_origin.as_dict(),
-                "start_time": self.start_date(),
-                "end_time": self.end_date(),
-                "base_dir": self.save_dir(),
-                "stations": [s.default_station_json_file_name() for s in self._stations],
-                "config": self._config.as_dict(),
-                "debug": self.debug,
-                "errors": self._errors.as_dict(),
-                "sdk_version": self._sdk_version,
-                "out_type": self._fs_writer.file_extension,
-                "make_runme": self._fs_writer.make_run_me
-                }
+        return {
+            "event_name": self.event_name,
+            "event_origin": self.event_origin.to_dict(),
+            "start_time": self.start_date(),
+            "end_time": self.end_date(),
+            "base_dir": self.save_dir(),
+            "stations": [s.default_station_json_file_name() for s in self._stations],
+            "config": self._config.to_dict(),
+            "debug": self.debug,
+            "errors": self._errors.as_dict(),
+            "sdk_version": self._sdk_version,
+            "out_type": self._fs_writer.file_extension,
+            "make_runme": self._fs_writer.make_run_me,
+        }
 
     def pretty(self) -> str:
         """
         :return: DataWindow as dictionary, but easier to read
         """
         # noinspection Mypy
         return pprint.pformat(self.as_dict())
@@ -414,24 +393,48 @@
     def from_config(config: DataWindowConfigFile) -> "DataWindow":
         """
         Use a config file to create a DataWindow
 
         :param config: DataWindowConfigFile to load from
         :return: DataWindow
         """
-        event_origin = EventOrigin(config.origin_provider, config.origin_latitude, config.origin_latitude_std,
-                                   config.origin_longitude, config.origin_longitude_std, config.origin_altitude,
-                                   config.origin_altitude_std, config.origin_event_radius_m)
-        dw_config = DataWindowConfig(config.input_directory, config.structured_layout, config.start_dt(),
-                                     config.end_dt(), config.start_buffer_td(), config.end_buffer_td(),
-                                     config.drop_time_seconds, config.station_ids, config.extensions,
-                                     config.api_versions, config.apply_correction, config.use_model_correction,
-                                     config.copy_edge_points())
-        return DataWindow(config.event_name, event_origin, dw_config, config.output_dir, config.output_type,
-                          config.make_runme, config.debug)
+        event_origin = EventOrigin(
+            config.origin_provider,
+            config.origin_latitude,
+            config.origin_latitude_std,
+            config.origin_longitude,
+            config.origin_longitude_std,
+            config.origin_altitude,
+            config.origin_altitude_std,
+            config.origin_event_radius_m,
+        )
+        dw_config = DataWindowConfig(
+            config.input_directory,
+            config.structured_layout,
+            config.start_dt(),
+            config.end_dt(),
+            config.start_buffer_td(),
+            config.end_buffer_td(),
+            config.drop_time_seconds,
+            config.station_ids,
+            config.extensions,
+            config.api_versions,
+            config.apply_correction,
+            config.use_model_correction,
+            config.copy_edge_points(),
+        )
+        return DataWindow(
+            config.event_name,
+            event_origin,
+            dw_config,
+            config.output_dir,
+            config.output_type,
+            config.make_runme,
+            config.debug,
+        )
 
     @staticmethod
     def from_config_file(file: str) -> "DataWindow":
         """
         Loads a configuration file to create the DataWindow
 
         :param file: full path to config file
@@ -489,49 +492,59 @@
         """
         Reads a JSON dictionary and loads the data into the DataWindow.
         If dictionary is improperly formatted, raises a ValueError.
 
         :param json_dict: the dictionary to read
         :return: The DataWindow as defined by the JSON
         """
-        if "out_type" not in json_dict.keys() \
-                or json_dict["out_type"].upper() not in dw_io.DataWindowOutputType.list_names():
-            raise ValueError('Dictionary loading type is invalid or unknown.  '
-                             'Check the value "out_type"; it must be one of: '
-                             f'{dw_io.DataWindowOutputType.list_non_none_names()}')
+        if (
+            "out_type" not in json_dict.keys()
+            or json_dict["out_type"].upper() not in dw_io.DataWindowOutputType.list_names()
+        ):
+            raise ValueError(
+                "Dictionary loading type is invalid or unknown.  "
+                'Check the value "out_type"; it must be one of: '
+                f"{dw_io.DataWindowOutputType.list_non_none_names()}"
+            )
         else:
             out_type = dw_io.DataWindowOutputType.str_to_type(json_dict["out_type"])
-            if out_type == dw_io.DataWindowOutputType.PARQUET:
-                dwin = DataWindow(json_dict["event_name"], EventOrigin.from_dict(json_dict["event_origin"]),
-                                  None, json_dict["base_dir"], json_dict["out_type"], json_dict["make_runme"],
-                                  json_dict["debug"])
+            if out_type == dw_io.DataWindowOutputType.PARQUET or out_type == dw_io.DataWindowOutputType.JSON:
+                dwin = DataWindow(
+                    json_dict["event_name"],
+                    EventOrigin.from_dict(json_dict["event_origin"]),
+                    None,
+                    json_dict["base_dir"],
+                    json_dict["out_type"],
+                    json_dict["make_runme"],
+                    json_dict["debug"],
+                )
                 dwin._config = DataWindowConfig.from_dict(json_dict["config"])
                 dwin._errors = RedVoxExceptions.from_dict(json_dict["errors"])
                 dwin._sdk_version = json_dict["sdk_version"]
                 for st in json_dict["stations"]:
                     dwin.add_station(Station.from_json_file(os.path.join(json_dict["base_dir"], st), f"{st}.json"))
             elif out_type == dw_io.DataWindowOutputType.LZ4:
-                dwin = DataWindow.deserialize(os.path.join(json_dict["base_dir"],
-                                                           f"{json_dict['event_name']}.pkl.lz4"))
+                dwin = DataWindow.deserialize(os.path.join(json_dict["base_dir"], f"{json_dict['event_name']}.pkl.lz4"))
             else:
                 dwin = DataWindow()
             return dwin
 
     def save(self) -> Path:
         """
         save the DataWindow to disk if saving is enabled
         if saving is not enabled, adds an error to the DataWindow and returns an empty path.
 
         :return: the path to where the files exist; an empty path means no files were saved
         """
         if self._fs_writer.is_save_disk():
             if self._fs_writer.is_use_disk() and self._fs_writer.make_run_me:
-                shutil.copyfile(os.path.abspath(inspect.getfile(run_me)),
-                                os.path.join(self._fs_writer.save_dir(), "runme.py"))
-            if self._fs_writer.file_extension == "parquet":
+                shutil.copyfile(
+                    os.path.abspath(inspect.getfile(run_me)), os.path.join(self._fs_writer.save_dir(), "runme.py")
+                )
+            if self._fs_writer.file_extension in ["parquet", "json"]:
                 return self._to_json_file()
             elif self._fs_writer.file_extension == "lz4":
                 return self.serialize()
         else:
             self._errors.append("Saving not enabled.")
             print("WARNING: Cannot save data window without knowing extension.")
             return Path()
@@ -658,16 +671,17 @@
                 return result[0]
             self._errors.append(f"Attempted to get station {station_id}, but that station is not in this data window!")
             if self.debug:
                 print(f"Attempted to get station {station_id}, but that station is not in this data window!")
             return None
         return self._stations[0]
 
-    def get_station(self, station_id: str, station_uuid: Optional[str] = None,
-                    start_timestamp: Optional[float] = None) -> Optional[List[Station]]:
+    def get_station(
+        self, station_id: str, station_uuid: Optional[str] = None, start_timestamp: Optional[float] = None
+    ) -> Optional[List[Station]]:
         """
         Get stations from the DataWindow.  Must give at least the station's id.  Other parameters may be None,
         which means the value will be ignored when searching.  Results will match all non-None parameters given.
 
         :param station_id: station id
         :param station_uuid: station uuid, default None
         :param start_timestamp: station start timestamp in microseconds since UTC epoch, default None
@@ -708,36 +722,41 @@
         r_f.with_start_dt_buf(self._config.start_buffer_td)
         r_f.with_end_dt_buf(self._config.end_buffer_td)
 
         if self.debug:
             print("Reading files from disk.  This may take a few minutes to complete.")
 
         # get the data to convert into a window
-        a_r = ApiReaderDw(self._config.input_dir, self._config.structured_layout, r_f,
-                          correct_timestamps=self._config.apply_correction,
-                          use_model_correction=self._config.use_model_correction,
-                          dw_base_dir=self.save_dir(),
-                          dw_save_mode=self._fs_writer.save_mode(),
-                          debug=self.debug, pool=_pool)
+        a_r = ApiReaderDw(
+            self._config.input_dir,
+            self._config.structured_layout,
+            r_f,
+            correct_timestamps=self._config.apply_correction,
+            use_model_correction=self._config.use_model_correction,
+            dw_base_dir=self.save_dir(),
+            dw_save_mode=self._fs_writer.save_mode(),
+            debug=self.debug,
+            pool=_pool,
+        )
 
         # self._errors.extend_error(a_r.errors)
 
         if self._fs_writer.is_use_mem() and a_r.dw_save_mode != self._fs_writer.save_mode():
             if self.debug:
                 print("Estimated size of files exceeds available memory.")
                 print("Automatically using temporary directory to store data.")
             self._fs_writer.set_use_temp(True)
 
         # Parallel update
         # Apply timing correction in parallel by station
         sts = a_r.get_stations()
         if self.debug:
-            print("num stations loaded: ", len(sts))
+            print("number of stations loaded: ", len(sts))
 
-        for st in maybe_parallel_map(_pool, Station.update_timestamps, iter(sts), chunk_size=1):
+        for st in maybe_parallel_map(_pool, lambda s: s, iter(sts), chunk_size=1):
             self.create_window_in_sensors(st, self._config.start_datetime, self._config.end_datetime)
             if self.debug:
                 print("station processed: ", st.id())
 
         # check for stations without data
         self._check_for_audio()
         self._check_valid_ids()
@@ -746,19 +765,21 @@
         if self.event_name == "dw" and len(self._stations) > 0:
             self.event_name = f"dw_{int(self.start_date())}_{len(self._stations)}"
 
         # must update the start and end in order for the data to be saved
         # update remaining data window values if they're still default
         if not self._config.start_datetime and len(self._stations) > 0:
             self._config.start_datetime = dtu.datetime_from_epoch_microseconds_utc(
-                np.min([t.first_data_timestamp() for t in self._stations]))
+                np.min([t.first_data_timestamp() for t in self._stations])
+            )
         # end_datetime is non-inclusive, so it must be greater than our latest timestamp
         if not self._config.end_datetime and len(self._stations) > 0:
             self._config.end_datetime = dtu.datetime_from_epoch_microseconds_utc(
-                np.max([t.last_data_timestamp() for t in self._stations]) + 1)
+                np.max([t.last_data_timestamp() for t in self._stations]) + 1
+            )
 
         # If the pool was created by this function, then it needs to managed by this function.
         if pool is None:
             _pool.close()
 
     def _check_for_audio(self):
         """
@@ -778,63 +799,70 @@
         if there are no stations, creates a single error message declaring no data found
         """
         if len(self._stations) < 1 and self._config.station_ids:
             if len(self._config.station_ids) > 1:
                 add_ids = f"for all stations {self._config.station_ids} "
             else:
                 add_ids = ""
-            self._errors.append(f"No data matching criteria {add_ids}in {self._config.input_dir}"
-                                f"\nPlease adjust parameters of DataWindow")
+            self._errors.append(
+                f"No data matching criteria {add_ids}in {self._config.input_dir}"
+                f"\nPlease adjust parameters of DataWindow"
+            )
         elif len(self._stations) > 0 and self._config.station_ids:
             for ids in self._config.station_ids:
                 if ids.zfill(STATION_ID_LENGTH) not in [i.id() for i in self._stations]:
-                    self._errors.append(
-                        f"Requested {ids} but there is no data to read for that station"
-                    )
+                    self._errors.append(f"Requested {ids} but there is no data to read for that station")
 
     def create_window_in_sensors(
-            self, station: Station, start_datetime: Optional[dtu.datetime] = None,
-            end_datetime: Optional[dtu.datetime] = None
+        self,
+        station: Station,
+        start_datetime: Optional[dtu.datetime] = None,
+        end_datetime: Optional[dtu.datetime] = None,
     ):
         """
-        truncate the sensors in the station to only contain data from start_date_timestamp to end_date_timestamp
-        if the start and/or end are not specified, keeps all audio data that fits and uses it
-        to truncate the other sensors.
+        truncate the sensors in the station to only contain data from start_datetime to end_datetime.
+
+        if the start and/or end are not specified, uses the audio start and end to truncate the other sensors.
+
         returns nothing, updates the station in place
 
         :param station: station object to truncate sensors of
         :param start_datetime: datetime of start of window, default None
         :param end_datetime: datetime of end of window, default None
         """
-        if start_datetime:
-            start_datetime = dtu.datetime_to_epoch_microseconds_utc(start_datetime)
-        else:
-            start_datetime = 0
-        if end_datetime:
-            end_datetime = dtu.datetime_to_epoch_microseconds_utc(end_datetime)
-        else:
-            end_datetime = dtu.datetime_to_epoch_microseconds_utc(dtu.datetime.max)
+        start_datetime = dtu.datetime_to_epoch_microseconds_utc(start_datetime) if start_datetime else 0
+        end_datetime = dtu.datetime_to_epoch_microseconds_utc(end_datetime if end_datetime else dtu.datetime.max)
         self.process_sensor(station.audio_sensor(), station.id(), start_datetime, end_datetime)
         if station.has_audio_data():
             for sensor in [s for s in station.data() if s.type() != SensorType.AUDIO]:
-                self.process_sensor(sensor, station.id(), station.audio_sensor().first_data_timestamp(),
-                                    station.audio_sensor().last_data_timestamp())
+                self.process_sensor(
+                    sensor,
+                    station.id(),
+                    station.audio_sensor().first_data_timestamp(),
+                    station.audio_sensor().last_data_timestamp(),
+                )
             # recalculate metadata
             station.update_first_and_last_data_timestamps()
-            station.set_packet_metadata([meta for meta in station.packet_metadata()
-                                         if meta.packet_start_mach_timestamp < station.last_data_timestamp() and
-                                         meta.packet_end_mach_timestamp >= station.first_data_timestamp()])
+            station.set_packet_metadata(
+                [
+                    meta
+                    for meta in station.packet_metadata()
+                    if meta.packet_start_mach_timestamp < station.last_data_timestamp()
+                    and meta.packet_end_mach_timestamp >= station.first_data_timestamp()
+                ]
+            )
             station.event_data().create_event_window(station.first_data_timestamp(), station.last_data_timestamp())
             if self._fs_writer.is_save_disk():
                 station.set_save_mode(io.FileSystemSaveMode.DISK)
                 station.set_save_dir(self.save_dir() if self._fs_writer.is_use_disk() else self._fs_writer.get_temp())
             self._stations.append(station)
 
-    def process_sensor(self, sensor: SensorData, station_id: str, start_date_timestamp: float,
-                       end_date_timestamp: float):
+    def process_sensor(
+        self, sensor: SensorData, station_id: str, start_date_timestamp: float, end_date_timestamp: float
+    ):
         """
         process a sensor to fit within the DataWindow.  Updates sensor in place, returns nothing.
 
         :param sensor: sensor to process
         :param station_id: station id
         :param start_date_timestamp: start of DataWindow
         :param end_date_timestamp: end of DataWindow
@@ -873,18 +901,23 @@
                     sensor.write_pyarrow_table(pa.Table.from_pydict(first_entry))
                 elif last_before_start is None and first_after_end is not None:
                     last_entry = sensor.pyarrow_table().slice(first_after_end, 1).to_pydict()
                     last_entry["timestamps"] = [start_date_timestamp]
                     sensor.write_pyarrow_table(pa.Table.from_pydict(last_entry))
                 elif last_before_start is not None and first_after_end is not None:
                     sensor.write_pyarrow_table(
-                        sensor.interpolate(start_date_timestamp, last_before_start, 1,
-                                           self._config.copy_edge_points == gpu.DataPointCreationMode.COPY))
+                        sensor.interpolate(
+                            start_date_timestamp,
+                            last_before_start,
+                            1,
+                            self._config.copy_edge_points == gpu.DataPointCreationMode.COPY,
+                        )
+                    )
             else:
-                _arrow = sensor.pyarrow_table().slice(start_index, end_index-start_index)
+                _arrow = sensor.pyarrow_table().slice(start_index, end_index - start_index)
                 # if sensor is audio or location, we want nan'd edge points
                 if sensor.type() in [SensorType.LOCATION, SensorType.AUDIO]:
                     new_point_mode = gpu.DataPointCreationMode.NAN
                 else:
                     new_point_mode = self._config.copy_edge_points
                 # add in the data points at the edges of the window if there are defined start and/or end times
                 slice_start = _arrow["timestamps"].to_numpy()[0]
@@ -894,38 +927,46 @@
                     end_samples_to_add = 1
                     start_sample_interval = start_date_timestamp - slice_start
                     start_samples_to_add = 1
                 else:
                     end_sample_interval = dtu.seconds_to_microseconds(sensor.sample_interval_s())
                     start_sample_interval = -end_sample_interval
                     if self._config.end_datetime:
-                        end_samples_to_add = int((dtu.datetime_to_epoch_microseconds_utc(self._config.end_datetime)
-                                                  - slice_end) / end_sample_interval)
+                        end_samples_to_add = int(
+                            (dtu.datetime_to_epoch_microseconds_utc(self._config.end_datetime) - slice_end)
+                            / end_sample_interval
+                        )
                     else:
                         end_samples_to_add = 0
                     if self._config.start_datetime:
-                        start_samples_to_add = int((slice_start -
-                                                    dtu.datetime_to_epoch_microseconds_utc(self._config.start_datetime))
-                                                   / end_sample_interval)
+                        start_samples_to_add = int(
+                            (slice_start - dtu.datetime_to_epoch_microseconds_utc(self._config.start_datetime))
+                            / end_sample_interval
+                        )
                     else:
                         start_samples_to_add = 0
                 # add to end
-                _arrow = (gpu.add_data_points_to_df(data_table=_arrow, start_index=_arrow.num_rows - 1,
-                                                    sample_interval_micros=end_sample_interval,
-                                                    num_samples_to_add=end_samples_to_add,
-                                                    point_creation_mode=new_point_mode))
+                _arrow = gpu.add_data_points_to_df(
+                    data_table=_arrow,
+                    start_index=_arrow.num_rows - 1,
+                    sample_interval_micros=end_sample_interval,
+                    num_samples_to_add=end_samples_to_add,
+                    point_creation_mode=new_point_mode,
+                )
                 # add to begin
-                _arrow = (gpu.add_data_points_to_df(data_table=_arrow, start_index=0,
-                                                    sample_interval_micros=start_sample_interval,
-                                                    num_samples_to_add=start_samples_to_add,
-                                                    point_creation_mode=new_point_mode))
+                _arrow = gpu.add_data_points_to_df(
+                    data_table=_arrow,
+                    start_index=0,
+                    sample_interval_micros=start_sample_interval,
+                    num_samples_to_add=start_samples_to_add,
+                    point_creation_mode=new_point_mode,
+                )
                 sensor.sort_by_data_timestamps(_arrow)
         else:
-            self._errors.append(f"Data window for {station_id} {sensor.type().name} "
-                                f"sensor has no data points!")
+            self._errors.append(f"Data window for {station_id} {sensor.type().name} " f"sensor has no data points!")
 
     def print_errors(self):
         """
         prints errors to screen
         """
         self._errors.print()
         for stn in self._stations:
```

### Comparing `redvox-3.4.2/redvox/common/data_window_configuration.py` & `redvox-3.5.0/redvox/common/data_window_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-This module provide type-safe data window configuration
+This module provides type-safe data window configuration using an external file
 """
 
 from dataclasses import dataclass
 from dataclasses_json import dataclass_json
 from typing import Optional, List, MutableMapping
 
 import pprint
@@ -158,30 +158,32 @@
 
     def pretty(self) -> str:
         # noinspection Mypy
         return pprint.pformat(self.to_dict())
 
     def start_dt(self) -> Optional[dtu.datetime]:
         if self.start_year is not None:
-            return dtu.datetime(self.start_year, self.start_month, self.start_day,
-                                self.start_hour, self.start_minute, self.start_second)
+            return dtu.datetime(
+                self.start_year, self.start_month, self.start_day, self.start_hour, self.start_minute, self.start_second
+            )
         return None
 
     def set_start_dt(self, start_dt: dtu.datetime):
         self.start_year = start_dt.year
         self.start_month = start_dt.month
         self.start_day = start_dt.day
         self.start_hour = start_dt.hour
         self.start_minute = start_dt.minute
         self.start_second = start_dt.second
 
     def end_dt(self) -> Optional[dtu.datetime]:
         if self.end_year is not None:
-            return dtu.datetime(self.end_year, self.end_month, self.end_day,
-                                self.end_hour, self.end_minute, self.end_second)
+            return dtu.datetime(
+                self.end_year, self.end_month, self.end_day, self.end_hour, self.end_minute, self.end_second
+            )
         return None
 
     def set_end_dt(self, end_dt: dtu.datetime):
         self.end_year = end_dt.year
         self.end_month = end_dt.month
         self.end_day = end_dt.day
         self.end_hour = end_dt.hour
```

### Comparing `redvox-3.4.2/redvox/common/data_window_io.py` & `redvox-3.5.0/redvox/common/data_window_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,32 +13,30 @@
     List,
     Optional,
     TYPE_CHECKING,
 )
 
 import lz4.frame
 
-from redvox.common.io import FileSystemWriter, FileSystemSaveMode, json_to_dict, dict_to_json
-from redvox.common.date_time_utils import (
-    datetime_to_epoch_microseconds_utc as us_dt,
-)
+from redvox.common.io import FileSystemWriter, FileSystemSaveMode, json_to_dict
 
 
 if TYPE_CHECKING:
-    from redvox.common.data_window import DataWindow, DataWindowConfig
+    from redvox.common.data_window import DataWindow
 
 
 class DataWindowOutputType(enum.Enum):
     """
     Type of file to create when exporting DataWindow
     """
 
     NONE: int = 0
     LZ4: int = 1
     PARQUET: int = 2
+    JSON: int = 3
 
     @staticmethod
     def list_names() -> List[str]:
         """
         :return: list of possible values for OutputType
         """
         return [n.name for n in DataWindowOutputType]
@@ -56,15 +54,15 @@
         converts the string to the corresponding OutputType
         if the type given is not in list_non_none_names(), returns NONE value
 
         :param str_type: string to convert
         :return: DataWindowOutputType matching string given or NONE
         """
         str_type = str_type.upper()
-        if str_type == "LZ4" or str_type == "PARQUET":
+        if str_type in DataWindowOutputType.list_non_none_names():
             return DataWindowOutputType[str_type]
         return DataWindowOutputType["NONE"]
 
 
 class DataWindowFileSystemWriter(FileSystemWriter):
     """
     This class holds the FileSystemWriter info for DataWindows.  Extends the FileSystemWriter from io.py
@@ -95,52 +93,54 @@
         :param base_dir: directory to save file to, default "." (current dir)
         :param make_run_me: if True, add a runme.py file to the saved files.  Default False
         """
         self.orig_path = os.getcwd()
         if not os.path.exists(base_dir):
             os.makedirs(base_dir, exist_ok=True)
         os.chdir(base_dir)
-        super().__init__(file_name, file_ext, ".",
-                         FileSystemSaveMode.DISK
-                         if DataWindowOutputType.str_to_type(file_ext) != DataWindowOutputType.NONE
-                         else FileSystemSaveMode.MEM)
+        super().__init__(
+            file_name,
+            file_ext,
+            ".",
+            FileSystemSaveMode.DISK
+            if DataWindowOutputType.str_to_type(file_ext) != DataWindowOutputType.NONE
+            else FileSystemSaveMode.MEM,
+        )
         self.make_run_me = make_run_me
 
     def set_extension(self, ext: str):
         """
-        change the file extension.  Valid values are "PARQUET", "LZ4" and "NONE".  Invalid values become "NONE"
+        change the file extension.  Valid values are "PARQUET", "LZ4", "JSON" and "NONE".  Invalid values become "NONE"
 
         :param ext: extension to change to
         """
         self.file_extension = DataWindowOutputType.str_to_type(ext).name.lower()
 
 
 @dataclass
 class DataWindowSerializationResult:
     path: str
     serialized_bytes: int
     compressed_bytes: int
 
 
-def data_window_as_json(
-        data_window: "DataWindow"
-) -> str:
+def data_window_as_json(data_window: "DataWindow") -> str:
     """
     Converts the DataWindow's metadata into a JSON dictionary
 
     :param data_window: The data window to convert
     :return: The data window's metadata as a JSON dictionary
     """
     return json.dumps(data_window.as_dict())
 
 
 def data_window_to_json(
-        data_window: "DataWindow",
-        base_dir: str = ".",
-        file_name: Optional[str] = None,
+    data_window: "DataWindow",
+    base_dir: str = ".",
+    file_name: Optional[str] = None,
 ) -> Path:
     """
     Converts the DataWindow into a JSON metadata file
 
     :param data_window: The data window to convert.
     :param base_dir: The base directory to write the JSON file to (default=.).
     :param file_name: The optional file name. If None, a default filename with the following format is used:
@@ -165,18 +165,18 @@
     :return: the dictionary of the DataWindow if it exists, or None otherwise
     """
     with open(file_path, "r") as f_p:
         return json_to_dict(f_p.read())
 
 
 def serialize_data_window(
-        data_window: "DataWindow",
-        base_dir: str = ".",
-        file_name: Optional[str] = None,
-        compression_factor: int = 4,
+    data_window: "DataWindow",
+    base_dir: str = ".",
+    file_name: Optional[str] = None,
+    compression_factor: int = 4,
 ) -> Path:
     """
     Serializes and compresses a DataWindow to a file and creates a JSON metadata file for the compressed file.
 
     :param data_window: The data window to serialize and compress.
     :param base_dir: The base directory to write the serialized file to (default=.).
     :param file_name: The optional file name. If None, a default filename with the following format is used:
@@ -186,28 +186,26 @@
     :return: The path to the written compressed file.
     """
 
     _file_name: str = (
         file_name
         if file_name is not None
         else f"{int(data_window.start_date())}"
-             f"_{int(data_window.end_date())}"
-             f"_{len(data_window.event_name)}.pkl.lz4"
+        f"_{int(data_window.end_date())}"
+        f"_{len(data_window.event_name)}.pkl.lz4"
     )
 
     json_path: Path = data_window.fs_writer().json_path()
     with open(json_path, "w") as f:
         f.write(data_window.to_json())
         json_path.resolve(False)
 
     file_path: Path = Path(base_dir).joinpath(_file_name)
 
-    with lz4.frame.open(
-            file_path, "wb", compression_level=compression_factor
-    ) as compressed_out:
+    with lz4.frame.open(file_path, "wb", compression_level=compression_factor) as compressed_out:
         pickle.dump(data_window, compressed_out)
         compressed_out.flush()
         return file_path.resolve(False)
 
 
 def deserialize_data_window(path: str) -> "DataWindow":
     """
```

### Comparing `redvox-3.4.2/redvox/common/date_time_utils.py` & `redvox-3.5.0/redvox/common/date_time_utils.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/common/errors.py` & `redvox-3.5.0/redvox/common/errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,16 +98,16 @@
                 "errors": [str(e) for e in self._errors]
             }
         return {"obj_class": self._obj_class}
 
     @staticmethod
     def from_dict(errors_dict: dict) -> "RedVoxExceptions":
         """
-        :param errors_dict: dictionary representing a RedvoxExceptions object
-        :return: RedvoxExceptions object
+        :param errors_dict: dictionary representing a RedVoxExceptions object
+        :return: a RedVoxExceptions object
         """
         if "obj_class" not in errors_dict.keys():
             result = RedVoxExceptions("ExceptionsLoadFailure")
             result.append("Failed to load errors due to missing obj_class")
         else:
             result = RedVoxExceptions(errors_dict["obj_class"])
             if "errors" in errors_dict.keys():
```

### Comparing `redvox-3.4.2/redvox/common/event_stream.py` & `redvox-3.5.0/redvox/common/event_stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""
+This module provides classes to organize events recorded on a station.
+"""
 from typing import List, Optional, Dict, Union
 from dataclasses import dataclass, field
 from pathlib import Path
 import enum
 import os
 import re
 
@@ -9,29 +12,30 @@
 from dataclasses_json import dataclass_json
 
 from redvox.api1000.common.mapping import Mapping
 from redvox.api1000.proto.redvox_api_m_pb2 import RedvoxPacketM
 from redvox.api1000.wrapped_redvox_packet import event_streams as es
 from redvox.common.errors import RedVoxExceptions
 from redvox.common import offset_model as om
-from redvox.common.io import FileSystemWriter as Fsw, FileSystemSaveMode
+from redvox.common.io import FileSystemWriter as Fsw, FileSystemSaveMode, json_file_to_dict
 import redvox.common.event_stream_io as io
 
 
 class EventDataTypes(enum.Enum):
     """
     Enumeration of data types for event data
     """
-    STRING = 0   # string data
+
+    STRING = 0  # string data
     NUMERIC = 1  # numeric data
     BOOLEAN = 2  # boolean data
-    BYTE = 3     # bytes data
+    BYTE = 3  # bytes data
 
     @staticmethod
-    def types_list() -> List['EventDataTypes']:
+    def types_list() -> List["EventDataTypes"]:
         """
         :return: the values of EventDataTypes as a list in order of: STRING, NUMERIC, BOOLEAN, BYTE
         """
         return [EventDataTypes.STRING, EventDataTypes.NUMERIC, EventDataTypes.BOOLEAN, EventDataTypes.BYTE]
 
 
 def get_empty_event_data_dict() -> dict:
@@ -43,20 +47,23 @@
 
 class Event:
     """
     stores event data from Redvox Api1000 packets
 
     ALL timestamps in microseconds since epoch UTC unless otherwise stated
     """
-    def __init__(self,
-                 timestamp: float,
-                 name: str = "event",
-                 data: Optional[Dict[EventDataTypes, dict]] = None,
-                 save_mode: FileSystemSaveMode = FileSystemSaveMode.MEM,
-                 base_dir: str = "."):
+
+    def __init__(
+        self,
+        timestamp: float,
+        name: str = "event",
+        data: Optional[Dict[EventDataTypes, dict]] = None,
+        save_mode: FileSystemSaveMode = FileSystemSaveMode.MEM,
+        base_dir: str = ".",
+    ):
         """
         initialize Event
 
         :param timestamp: timestamp when Event occurred in microseconds since epoch UTC
         :param name: name of the Event.  Default "event"
         :param data: a structured dictionary of the data.  Dictionary must look like:
                     {EventDataTypes.STRING: {s_values}, EventDataTypes.NUMERIC: {n_values},
@@ -77,45 +84,50 @@
         self._uncorrected_timestamp = timestamp
         if data is not None:
             self._data = data
         else:
             self._data = get_empty_event_data_dict()
 
     def __repr__(self):
-        return f"name: {self.name}, " \
-               f"timestamp: {self._timestamp}, " \
-               f"uncorrected_timestamp: {self._uncorrected_timestamp}, " \
-               f"schema: {self.get_schema()}, " \
-               f"save_mode: {self._fs_writer.save_mode()}"
+        return (
+            f"name: {self.name}, "
+            f"timestamp: {self._timestamp}, "
+            f"uncorrected_timestamp: {self._uncorrected_timestamp}, "
+            f"schema: {self.get_schema()}, "
+            f"save_mode: {self._fs_writer.save_mode()}"
+        )
 
     def __str__(self):
-        return f"name: {self.name}, " \
-               f"timestamp: {self._timestamp}, " \
-               f"uncorrected_timestamp: {self._uncorrected_timestamp}, " \
-               f"schema: {self.__schema_as_str()}"
+        return (
+            f"name: {self.name}, "
+            f"timestamp: {self._timestamp}, "
+            f"uncorrected_timestamp: {self._uncorrected_timestamp}, "
+            f"schema: {self.__schema_as_str()}"
+        )
 
     def as_dict(self) -> dict:
         """
         :return: EventStream as a dictionary
         """
         return {
             "name": self.name,
             "timestamp": self._timestamp,
             "uncorrected_timestamp": self._uncorrected_timestamp,
             "metadata": self.metadata,
             "data": self.__data_as_dict(),
-            "errors": self._errors.as_dict()
+            "errors": self._errors.as_dict(),
         }
 
     def __data_as_dict(self) -> dict:
-        return {EventDataTypes.STRING.name: self.get_string_values(),
-                EventDataTypes.NUMERIC.name: self.get_numeric_values(),
-                EventDataTypes.BOOLEAN.name: self.get_boolean_values(),
-                EventDataTypes.BYTE.name: self.get_byte_values()
-                }
+        return {
+            EventDataTypes.STRING.name: self.get_string_values(),
+            EventDataTypes.NUMERIC.name: self.get_numeric_values(),
+            EventDataTypes.BOOLEAN.name: self.get_boolean_values(),
+            EventDataTypes.BYTE.name: self.get_byte_values(),
+        }
 
     def __schema_as_str(self) -> str:
         result = ""
         for f in self._data.keys():
             result += f"{f.name}: {list(self._data[f].keys())}"
             if f != EventDataTypes.BYTE:
                 result += ", "
@@ -141,52 +153,61 @@
     def __get_data_from_event(event: es.Event):
         """
         load data from an Event;
         gets data in order of: string, numeric, boolean, byte
 
         :param event: event to load data from
         """
-        return map(Event.__get_items, [event.get_string_payload(), event.get_numeric_payload(),
-                                       event.get_boolean_payload(), event.get_byte_payload()])
+        return map(
+            Event.__get_items,
+            [
+                event.get_string_payload(),
+                event.get_numeric_payload(),
+                event.get_boolean_payload(),
+                event.get_byte_payload(),
+            ],
+        )
 
     @staticmethod
     def __get_data_from_event_raw(event: RedvoxPacketM.EventStream.Event):
         """
         load data from an Event;
         gets data in order of: string, numeric, boolean, byte
 
         :param event: event to load data from
         """
-        return map(Event.__get_items_raw, [event.string_payload, event.numeric_payload,
-                                           event.boolean_payload, event.byte_payload])
+        return map(
+            Event.__get_items_raw,
+            [event.string_payload, event.numeric_payload, event.boolean_payload, event.byte_payload],
+        )
 
     def _set_data(self, data: iter):
         """
         sets the data of the Event
 
         :param data: an iterable of data to insert
         """
         for g, h in map(lambda l, p: (l, p), data, EventDataTypes.types_list()):
             for k, v in g:
                 self._data[h][k] = v
 
-    def read_event(self, event: es.Event) -> 'Event':
+    def read_event(self, event: es.Event) -> "Event":
         """
         read the payloads of a Redvox Event, separate the data by payload type, then add it to the SDK Event
 
         :param event: event to process
         :return: updated self
         """
         self.name = event.get_description()
         self._fs_writer.file_name = f"event_{self.name}"
         self.metadata = event.get_metadata()
         self._set_data(self.__get_data_from_event(event))
         return self
 
-    def read_raw(self, event: RedvoxPacketM.EventStream.Event) -> 'Event':
+    def read_raw(self, event: RedvoxPacketM.EventStream.Event) -> "Event":
         """
         read the contents of a Redvox Api1000 protobuf stream
 
         :param event: the protobuf stream to read
         """
         self.name = event.description
         self._fs_writer.file_name = f"event_{self.name}"
@@ -313,16 +334,20 @@
         return None
 
     def get_item(self, data_key: str) -> Union[List[str], str, bool, float]:
         """
         :param data_key: key of data to get
         :return: data with matching data_key or the list of all possible data keys
         """
-        for r in [self.get_string_item(data_key), self.get_numeric_item(data_key),
-                  self.get_boolean_item(data_key), self.get_byte_item(data_key)]:
+        for r in [
+            self.get_string_item(data_key),
+            self.get_numeric_item(data_key),
+            self.get_boolean_item(data_key),
+            self.get_byte_item(data_key),
+        ]:
             if r is not None:
                 return r
         return self.get_data_keys()
 
     def get_classification(self, index: int = 0) -> dict:
         """
         get a classification from an event (anything that ends with "_X" where X is the index value)
@@ -555,23 +580,22 @@
     @staticmethod
     def from_json_file(file_dir: str, file_name: str) -> "Event":
         """
         :param file_dir: full path to containing directory for the file
         :param file_name: name of file to load data from
         :return: Event from json file
         """
-        json_data = io.json_file_to_dict(os.path.join(file_dir, f"{file_name}"))
+        json_data = json_file_to_dict(os.path.join(file_dir, f"{file_name}"))
         if "timestamp" in json_data.keys():
             data = get_empty_event_data_dict()
             data[EventDataTypes.STRING] = json_data["data"]["STRING"]
             data[EventDataTypes.NUMERIC] = json_data["data"]["NUMERIC"]
             data[EventDataTypes.BOOLEAN] = json_data["data"]["BOOLEAN"]
             data[EventDataTypes.BYTE] = json_data["data"]["BYTE"]
-            result = Event(json_data["timestamp"], json_data["name"], data, FileSystemSaveMode.DISK,
-                           file_dir)
+            result = Event(json_data["timestamp"], json_data["name"], data, FileSystemSaveMode.DISK, file_dir)
             result.metadata = json_data["metadata"]
             result._uncorrected_timestamp = json_data["uncorrected_timestamp"]
             result.set_errors(RedVoxExceptions.from_dict(json_data["errors"]))
         else:
             result = Event(np.nan, "Empty")
             result.append_error(f"Loading from {file_name} failed; missing Event timestamp.")
         return result
@@ -637,51 +661,56 @@
 
         model_version: string; version of the model.  Default "0.0"
 
         metadata: Dict[str, str]; metadata as dict of strings.  Default empty dict
 
         debug: boolean; if True, outputs additional information at runtime.  Default False.
     """
+
     name: str = "stream"
     events: List[Event] = field(default_factory=lambda: [])
     input_sample_rate: int = 0
     samples_per_window: int = 0
     samples_per_hop: int = 0
     model_version: str = "n/a"
     metadata: Dict[str, str] = field(default_factory=lambda: {})
     debug: bool = False
 
     def __repr__(self):
-        return f"name: {self.name}, " \
-               f"events: {[s.__repr__() for s in self.events]}, " \
-               f"input_sample_rate: {self.input_sample_rate}, " \
-               f"samples_per_window: {self.samples_per_window}, " \
-               f"samples_per_hop: {self.samples_per_hop}, " \
-               f"model_version: {self.model_version}"
+        return (
+            f"name: {self.name}, "
+            f"events: {[s.__repr__() for s in self.events]}, "
+            f"input_sample_rate: {self.input_sample_rate}, "
+            f"samples_per_window: {self.samples_per_window}, "
+            f"samples_per_hop: {self.samples_per_hop}, "
+            f"model_version: {self.model_version}"
+        )
 
     def __str__(self):
-        return f"name: {self.name}, " \
-               f"events: {[s.__str__() for s in self.events]}, " \
-               f"input_sample_rate: {self.input_sample_rate}, " \
-               f"samples_per_window: {self.samples_per_window}, " \
-               f"samples_per_hop: {self.samples_per_hop}, " \
-               f"model_version: {self.model_version}"
+        return (
+            f"name: {self.name}, "
+            f"events: {[s.__str__() for s in self.events]}, "
+            f"input_sample_rate: {self.input_sample_rate}, "
+            f"samples_per_window: {self.samples_per_window}, "
+            f"samples_per_hop: {self.samples_per_hop}, "
+            f"model_version: {self.model_version}"
+        )
 
     def as_dict(self) -> dict:
         """
         :return: EventStream as a dictionary
         """
         return {
             "name": self.name,
             "events": [e.as_dict() for e in self.events],
             "input_sample_rate": self.input_sample_rate,
             "samples_per_window": self.samples_per_window,
             "samples_per_hop": self.samples_per_hop,
             "model_version": self.model_version,
-            "metadata": self.metadata
+            "metadata": self.metadata,
         }
 
     def has_data(self):
         """
         :return: if there is at least one event
         """
         return len(self.events) > 0
@@ -722,17 +751,17 @@
                 for v in val:
                     column_list.add(v)
         if len(result) > 0:
             return result
         return list(column_list)
 
     @staticmethod
-    def from_eventstream(stream: RedvoxPacketM.EventStream,
-                         save_mode: FileSystemSaveMode = FileSystemSaveMode.MEM,
-                         base_dir: str = ".") -> 'EventStream':
+    def from_eventstream(
+        stream: RedvoxPacketM.EventStream, save_mode: FileSystemSaveMode = FileSystemSaveMode.MEM, base_dir: str = "."
+    ) -> "EventStream":
         """
         convert a Redvox Api1000 Packet EventStream into its sdk version
 
         :param stream: Redvox Api1000 Packet EventStream to read data from
         :param save_mode: FileSystemSaveMode that determines how Event data is saved.
                             Default FileSystemSaveMode.MEM (use RAM).  Other options are DISK (save to directory)
                             and TEMP (save to temporary directory)
@@ -745,22 +774,23 @@
             result.input_sample_rate = int(stream.metadata.get("input_sample_rate"))
         if "input_samples_per_window" in stream.metadata.keys():
             result.samples_per_window = int(stream.metadata.get("input_samples_per_window"))
         if "input_samples_per_hop" in stream.metadata.keys():
             result.samples_per_hop = int(stream.metadata.get("input_samples_per_hop"))
         if "model_version" in stream.metadata.keys():
             result.model_version = stream.metadata.get("model_version")
-        result.add_events(stream,
-                          save_mode=save_mode,
-                          base_dir=base_dir)
+        result.add_events(stream, save_mode=save_mode, base_dir=base_dir)
         return result
 
-    def add_events(self, stream: RedvoxPacketM.EventStream,
-                   save_mode: FileSystemSaveMode = FileSystemSaveMode.MEM,
-                   base_dir: str = "."):
+    def add_events(
+        self,
+        stream: RedvoxPacketM.EventStream,
+        save_mode: FileSystemSaveMode = FileSystemSaveMode.MEM,
+        base_dir: str = ".",
+    ):
         """
         add events from a Redvox Api1000 Packet EventStream with the same name.
         Does nothing if names do not match
 
         :param stream: stream of events to add
         :param save_mode: FileSystemSaveMode that determines how Event data is saved.
                             Default FileSystemSaveMode.MEM (use RAM).  Other options are DISK (save to directory)
@@ -768,16 +798,15 @@
         :param base_dir: the location of the parquet file that holds the Event data.  Not used if save_data is False.
                             Default current directory (".")
         """
         if self.name == stream.name:
             timestamps = stream.timestamps.timestamps
             events = stream.events
             for i in range(len(timestamps)):
-                self.events.append(Event(timestamps[i], save_mode=save_mode,
-                                         base_dir=base_dir).read_raw(events[i]))
+                self.events.append(Event(timestamps[i], save_mode=save_mode, base_dir=base_dir).read_raw(events[i]))
         elif self.debug:
             print(f"Stream name mismatch while adding to EventStream.  Expected {self.name}, got {stream.name}.")
 
     def sort_events(self, asc: bool = True):
         """
         sort the events in the stream via ascending or descending timestamp order
 
@@ -885,33 +914,45 @@
     @staticmethod
     def from_json_dict(json_dict: dict) -> "EventStream":
         """
         :param json_dict: json dict to parse
         :return: EventStream from json dict
         """
         if "name" in json_dict.keys():
-            result = EventStream(json_dict["name"], [Event.from_json_dict(e) for e in json_dict["events"]],
-                                 json_dict["input_sample_rate"], json_dict["samples_per_window"],
-                                 json_dict["samples_per_hop"], json_dict["model_version"], json_dict["metadata"])
+            result = EventStream(
+                json_dict["name"],
+                [Event.from_json_dict(e) for e in json_dict["events"]],
+                json_dict["input_sample_rate"],
+                json_dict["samples_per_window"],
+                json_dict["samples_per_hop"],
+                json_dict["model_version"],
+                json_dict["metadata"],
+            )
         else:
             result = EventStream("Empty Stream; no name for identification")
         return result
 
     @staticmethod
     def from_json_file(file_dir: str, file_name: str) -> "EventStream":
         """
         :param file_dir: full path to containing directory for the file
         :param file_name: name of file to load data from
         :return: EventStream from json file
         """
-        json_data = io.json_file_to_dict(os.path.join(file_dir, f"{file_name}"))
+        json_data = json_file_to_dict(os.path.join(file_dir, f"{file_name}"))
         if "name" in json_data.keys():
-            result = EventStream(json_data["name"], json_data["events"], json_data["input_sample_rate"],
-                                 json_data["samples_per_window"], json_data["samples_per_hop"],
-                                 json_data["model_version"], json_data["metadata"])
+            result = EventStream(
+                json_data["name"],
+                json_data["events"],
+                json_data["input_sample_rate"],
+                json_data["samples_per_window"],
+                json_data["samples_per_hop"],
+                json_data["model_version"],
+                json_data["metadata"],
+            )
             result.set_save_mode(FileSystemSaveMode.DISK)
             result.set_save_dir(file_dir)
         else:
             result = EventStream("Empty Stream; no name for identification")
         return result
 
     def to_json_file(self, file_dir: str = ".", file_name: Optional[str] = None) -> Path:
@@ -943,20 +984,20 @@
     ALL timestamps in microseconds since epoch UTC unless otherwise stated
 
     Properties:
         streams: List[EventStream]; list of all EventStream.  Default empty list
 
         debug: bool; if True, output additional information during runtime.  Default False
     """
+
     streams: List[EventStream] = field(default_factory=lambda: [])
     debug: bool = False
 
     def __repr__(self):
-        return f"streams: {[s.__repr__() for s in self.streams]}, " \
-               f"debug: {self.debug}"
+        return f"streams: {[s.__repr__() for s in self.streams]}, " f"debug: {self.debug}"
 
     def __str__(self):
         return str([s.__str__() for s in self.streams])
 
     def as_dict(self) -> dict:
         """
         :return: EventStreams as dict
@@ -1087,15 +1128,15 @@
     @staticmethod
     def from_json_file(file_dir: str, file_name: str) -> "EventStreams":
         """
         :param file_dir: full path to containing directory for the file
         :param file_name: name of file to load data from
         :return: EventStreams from json file
         """
-        json_data = io.json_file_to_dict(os.path.join(file_dir, f"{file_name}"))
+        json_data = json_file_to_dict(os.path.join(file_dir, f"{file_name}"))
         if "streams" in json_data.keys():
             result = EventStreams([EventStream.from_json_dict(s) for s in json_data["streams"]])
             result.set_save_mode(FileSystemSaveMode.DISK)
             result.set_save_dir(file_dir)
         else:
             result = EventStreams()
         return result
```

### Comparing `redvox-3.4.2/redvox/common/event_stream_io.py` & `redvox-3.5.0/redvox/common/event_stream_io.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,104 +5,93 @@
 import json
 import os
 from typing import (
     Optional,
     TYPE_CHECKING,
 )
 
-from redvox.common.io import get_json_file, json_file_to_dict, json_to_dict
-
 
 if TYPE_CHECKING:
     from redvox.common.event_stream import Event, EventStream, EventStreams
 
 
-def event_to_json(event: "Event", ) -> str:
+def event_to_json(
+    event: "Event",
+) -> str:
     """
     :param event: event to save
     :return: Event as json string
     """
     return json.dumps(event.as_dict())
 
 
-def event_to_json_file(event: "Event",
-                       file_name: Optional[str] = None) -> Path:
+def event_to_json_file(event: "Event", file_name: Optional[str] = None) -> Path:
     """
     saves the Event as json and data in the same directory.
 
     :param event: Event to save
     :param file_name: the optional base file name.  Do not include a file extension.
                         If None, uses the default event_[id].json
     :return: path to json file
     """
-    _file_name: str = (
-        file_name
-        if file_name is not None
-        else event.default_json_file_name()
-    )
+    _file_name: str = file_name if file_name is not None else event.default_json_file_name()
 
     file_path: Path = event.fs_writer().json_path()
     with open(file_path, "w") as f_p:
         f_p.write(event_to_json(event))
         return file_path.resolve(False)
 
 
-def eventstream_to_json(event_stream: "EventStream", ) -> str:
+def eventstream_to_json(
+    event_stream: "EventStream",
+) -> str:
     """
     :return: EventStream as json string
     """
     return json.dumps(event_stream.as_dict())
 
 
-def eventstream_to_json_file(event_stream: "EventStream",
-                             file_dir: str = ".",
-                             file_name: Optional[str] = None) -> Path:
+def eventstream_to_json_file(event_stream: "EventStream", file_dir: str = ".", file_name: Optional[str] = None) -> Path:
     """
     saves the EventStream as json and data in the same directory.
 
     :param event_stream: EventStream to save
     :param file_dir: the directory to save the file into.  default current directory (".")
     :param file_name: the optional base file name.  Do not include a file extension.
                         If None, uses the default eventstream_[eventstream.name].json
     :return: path to json file
     """
-    _file_name: str = (
-        file_name
-        if file_name is not None
-        else f"eventstream_{event_stream.name}"
-    )
+    _file_name: str = file_name if file_name is not None else f"eventstream_{event_stream.name}"
 
     file_path: Path = Path(os.path.join(file_dir, f"{_file_name}.json"))
     with open(file_path, "w") as f_p:
         f_p.write(eventstream_to_json(event_stream))
         return file_path.resolve(False)
 
 
-def eventstreams_to_json(event_streams: "EventStreams", ) -> str:
+def eventstreams_to_json(
+    event_streams: "EventStreams",
+) -> str:
     """
     :return: EventStreams as json string
     """
     return json.dumps(event_streams.as_dict())
 
 
-def eventstreams_to_json_file(event_streams: "EventStreams",
-                              file_dir: str = ".",
-                              file_name: Optional[str] = None) -> Path:
+def eventstreams_to_json_file(
+    event_streams: "EventStreams", file_dir: str = ".", file_name: Optional[str] = None
+) -> Path:
     """
     saves the EventStreams as json and data in the same directory.
 
     :param event_streams: EventStreams to save
     :param file_dir: the directory to save the file into.  default current directory (".")
     :param file_name: the optional base file name.  Do not include a file extension.
                         If None, uses the default eventstreams.json
     :return: path to json file
     """
-    _file_name: str = (
-        file_name
-        if file_name is not None
-        else "eventstreams"
-    )
+    _file_name: str = file_name if file_name is not None else "eventstreams"
 
     file_path: Path = Path(os.path.join(file_dir, f"{_file_name}.json"))
     with open(file_path, "w") as f_p:
         f_p.write(eventstreams_to_json(event_streams))
         return file_path.resolve(False)
```

### Comparing `redvox-3.4.2/redvox/common/file_statistics.py` & `redvox-3.5.0/redvox/common/file_statistics.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/common/gap_and_pad_utils.py` & `redvox-3.5.0/redvox/common/gap_and_pad_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""
+This module provides tools to fill gaps and pad the ends of timestamp arrays
+"""
 import sys
 from typing import List, Tuple, Optional, Dict
 import enum
 from math import modf
 from dataclasses import dataclass, field
 
 from dataclasses_json import dataclass_json
@@ -10,28 +13,41 @@
 import pyarrow.compute as pc
 
 from redvox.common import date_time_utils as dtu
 from redvox.common.errors import RedVoxExceptions
 from redvox.api1000.wrapped_redvox_packet.sensors.audio import AudioCodec
 from redvox.api1000.wrapped_redvox_packet.sensors.location import LocationProvider
 from redvox.api1000.wrapped_redvox_packet.sensors.image import ImageCodec
-from redvox.api1000.wrapped_redvox_packet.station_information import \
-    NetworkType, PowerState, CellServiceState, WifiWakeLock, ScreenState
+from redvox.api1000.wrapped_redvox_packet.station_information import (
+    NetworkType,
+    PowerState,
+    CellServiceState,
+    WifiWakeLock,
+    ScreenState,
+)
 
 # percent of packet duration/sample rate required for gap to be considered a whole unit
 DEFAULT_GAP_UPPER_LIMIT: float = 0.8
 # percent of packet duration/sample rate required for gap to be considered nothing
 DEFAULT_GAP_LOWER_LIMIT: float = 0.02
 # columns for audio table
 AUDIO_DF_COLUMNS = ["timestamps", "unaltered_timestamps", "microphone"]
 # columns that cannot be interpolated
 NON_INTERPOLATED_COLUMNS = ["compressed_audio", "image"]
 # columns that are not numeric but can be interpolated
-NON_NUMERIC_COLUMNS = ["location_provider", "image_codec", "audio_codec", "network_type",
-                       "power_state", "cell_service", "wifi_wake_lock", "screen_state"]
+NON_NUMERIC_COLUMNS = [
+    "location_provider",
+    "image_codec",
+    "audio_codec",
+    "network_type",
+    "power_state",
+    "cell_service",
+    "wifi_wake_lock",
+    "screen_state",
+]
 
 
 # noinspection Mypy,DuplicatedCode
 class DataPointCreationMode(enum.Enum):
     """
     Type of data point to create
     """
@@ -56,14 +72,15 @@
 
         metadata: list of start times in microseconds since epoch UTC and the data to add
 
         gaps: the list of start and end points of gaps (the start and end are actual data points)
 
         errors: the errors encountered while getting the data
     """
+
     sample_interval_micros: float
     metadata: Optional[List[Tuple[float, pa.Table]]] = None
     gaps: List[Tuple[float, float]] = field(default_factory=lambda: [])
     errors: RedVoxExceptions = field(default_factory=lambda: RedVoxExceptions("AudioWithGaps"))
 
     def create_timestamps(self) -> pa.Table:
         """
@@ -74,16 +91,17 @@
             timestamps = calc_evenly_sampled_timestamps(m[0], m[1].num_rows, self.sample_interval_micros)
             result_array[0].extend(timestamps)
             result_array[1].extend(timestamps)
             result_array[2].extend(m[1]["microphone"].to_numpy())
         for gs, ge in self.gaps:
             fractional, whole = modf((ge - gs) / self.sample_interval_micros)
             num_samples = int((whole - 1) if fractional < DEFAULT_GAP_LOWER_LIMIT else whole)
-            timestamps = calc_evenly_sampled_timestamps(gs + self.sample_interval_micros, num_samples,
-                                                        self.sample_interval_micros)
+            timestamps = calc_evenly_sampled_timestamps(
+                gs + self.sample_interval_micros, num_samples, self.sample_interval_micros
+            )
             gap_array = [timestamps, np.full(len(timestamps), np.nan)]
             result_array[0].extend(gap_array[0])
             result_array[1].extend(gap_array[0])
             result_array[2].extend(gap_array[1])
         ptable = pa.Table.from_pydict(dict(zip(AUDIO_DF_COLUMNS, result_array)))
         return pc.take(ptable, pc.sort_indices(ptable, sort_keys=[("timestamps", "ascending")]))
 
@@ -91,30 +109,29 @@
         """
         add an error to the result
         :param error: error message to add
         """
         self.errors.append(error)
 
 
-def calc_evenly_sampled_timestamps(
-        start: float, samples: int, sample_interval_micros: float
-) -> np.array:
+def calc_evenly_sampled_timestamps(start: float, samples: int, sample_interval_micros: float) -> np.array:
     """
     given a start time, calculates samples amount of evenly spaced timestamps at rate_hz
 
     :param start: float, start timestamp in microseconds
     :param samples: int, number of samples
     :param sample_interval_micros: float, sample interval in microseconds
     :return: np.array with number of samples timestamps, evenly spaced starting at start
     """
     return start + (np.arange(0, samples) * sample_interval_micros)
 
 
-def check_gap_list(gaps: List[Tuple[float, float]], start_timestamp: float = None,
-                   end_timestamp: float = None) -> List[Tuple[float, float]]:
+def check_gap_list(
+    gaps: List[Tuple[float, float]], start_timestamp: float = None, end_timestamp: float = None
+) -> List[Tuple[float, float]]:
     """
     removes any gaps where end time <= start time, consolidates overlapping gaps, and ensures that no gap
     starts or ends before start_timestamp and starts or ends after end_timestamp.  All timestamps are in
     microseconds since epoch UTC
 
     :param gaps: list of gaps to check
     :param start_timestamp: lowest possible timestamp for a gap to start at
@@ -140,18 +157,15 @@
                     if gap[0] < r_g[1] < gap[1]:
                         r_g = (r_g[0], gap[1])
                     return_gaps[a] = r_g
     return return_gaps
 
 
 def fill_gaps(
-        arrow_df: pa.Table,
-        gaps: List[Tuple[float, float]],
-        sample_interval_micros: float,
-        fill_mode: str = "nan"
+    arrow_df: pa.Table, gaps: List[Tuple[float, float]], sample_interval_micros: float, fill_mode: str = "nan"
 ) -> Tuple[pa.Table, List[Tuple[float, float]]]:
     """
     fills gaps in the table with np.nan or interpolated values by interpolating timestamps based on the
     calculated sample interval
 
     :param arrow_df: pyarrow table with data.  first column is "timestamps"
     :param gaps: list of tuples of known non-inclusive start and end timestamps of the gaps
@@ -160,17 +174,18 @@
                         Will convert input to lowercase.
     :return: table without gaps and the list of gaps
     """
     # extract the necessary information to compute gap size and gap timestamps
     data_time_stamps = arrow_df["timestamps"].to_numpy()
     if len(data_time_stamps) > 1:
         data_duration = data_time_stamps[-1] - data_time_stamps[0]
-        expected_samples = (np.floor(data_duration / sample_interval_micros)
-                            + (1 if data_duration % sample_interval_micros >=
-                               sample_interval_micros * DEFAULT_GAP_UPPER_LIMIT else 0)) + 1
+        expected_samples = (
+            np.floor(data_duration / sample_interval_micros)
+            + (1 if data_duration % sample_interval_micros >= sample_interval_micros * DEFAULT_GAP_UPPER_LIMIT else 0)
+        ) + 1
         if expected_samples > len(data_time_stamps):
             if fill_mode.lower() == "copy":
                 pcm = DataPointCreationMode["COPY"]
             elif fill_mode.lower() == "interpolate":
                 pcm = DataPointCreationMode["INTERPOLATE"]
             else:
                 pcm = DataPointCreationMode["NAN"]
@@ -191,28 +206,28 @@
                     after_end = after_end[0][0]
                     # sim = gap[1] - data_time_stamps[after_end]
                     gap = (gap[0], data_time_stamps[after_end])
                 else:
                     after_end = None
                 num_new_points = int((gap[1] - gap[0]) / sample_interval_micros) - 1
                 if before_start is not None:
-                    arrow_df = add_data_points_to_df(arrow_df, before_start, sample_interval_micros,
-                                                     num_new_points, pcm)
+                    arrow_df = add_data_points_to_df(
+                        arrow_df, before_start, sample_interval_micros, num_new_points, pcm
+                    )
                 elif after_end is not None:
-                    arrow_df = add_data_points_to_df(arrow_df, after_end, -sample_interval_micros,
-                                                     num_new_points, pcm)
+                    arrow_df = add_data_points_to_df(arrow_df, after_end, -sample_interval_micros, num_new_points, pcm)
         indic = pc.sort_indices(arrow_df, sort_keys=[("timestamps", "ascending")])
         return arrow_df.take(indic), gaps
     return arrow_df, gaps
 
 
 def fill_audio_gaps(
-        packet_data: List[Tuple[float, pa.Table]],
-        sample_interval_micros: float,
-        gap_lower_limit: float = DEFAULT_GAP_LOWER_LIMIT
+    packet_data: List[Tuple[float, pa.Table]],
+    sample_interval_micros: float,
+    gap_lower_limit: float = DEFAULT_GAP_LOWER_LIMIT,
 ) -> AudioWithGaps:
     """
     fills gaps in the table with np.nan by interpolating timestamps based on the expected sample interval
       * ignores gaps with duration less than or equal to packet length * gap_lower_limit
 
     :param packet_data: list of tuples, each tuple containing two pieces of packet information:
                         packet_start_timestamps; float of packet start timestamp in microseconds
@@ -232,28 +247,31 @@
         # check if start_ts is close to the last timestamp in data_timestamps
         last_timestamp_diff = start_ts - last_data_timestamp
         if last_timestamp_diff > gap_lower_limit * packet_length:
             gap_start = last_data_timestamp - sample_interval_micros
             last_data_timestamp = start_ts
             gaps.append((gap_start, last_data_timestamp))
         elif last_timestamp_diff < -gap_lower_limit * packet_length:
-            result.add_error(f"Packet start timestamp: {dtu.microseconds_to_seconds(start_ts)} "
-                             f"is before last timestamp of previous "
-                             f"packet: {dtu.microseconds_to_seconds(last_data_timestamp - sample_interval_micros)}")
+            result.add_error(
+                f"Packet start timestamp: {dtu.microseconds_to_seconds(start_ts)} "
+                f"is before last timestamp of previous "
+                f"packet: {dtu.microseconds_to_seconds(last_data_timestamp - sample_interval_micros)}"
+            )
         last_data_timestamp += samples_in_packet * sample_interval_micros
     result.gaps = gaps
     return result
 
 
-def add_data_points_to_df(data_table: pa.Table,
-                          start_index: int,
-                          sample_interval_micros: float,
-                          num_samples_to_add: int = 1,
-                          point_creation_mode: DataPointCreationMode = DataPointCreationMode.COPY,
-                          ) -> pa.Table:
+def add_data_points_to_df(
+    data_table: pa.Table,
+    start_index: int,
+    sample_interval_micros: float,
+    num_samples_to_add: int = 1,
+    point_creation_mode: DataPointCreationMode = DataPointCreationMode.COPY,
+) -> pa.Table:
     """
     adds data points to the end of the table, starting from the index specified.
         Note:
             * table must not be empty
             * start_index must be non-negative and less than the length of table
             * num_samples_to_add must be greater than 0
             * sample_interval_micros cannot be 0
@@ -267,46 +285,53 @@
     :param start_index: index of the table to use as starting point for creating new values
     :param sample_interval_micros: sample interval in microseconds of the timestamps; use negative values to
                                     add points before the start_index
     :param num_samples_to_add: the number of timestamps to create, default 1
     :param point_creation_mode: the mode of point creation to use
     :return: updated table with synthetic data points
     """
-    if len(data_table) > start_index and len(data_table) > 0 and num_samples_to_add > 0 \
-            and sample_interval_micros != 0.:
+    if (
+        len(data_table) > start_index
+        and len(data_table) > 0
+        and num_samples_to_add > 0
+        and sample_interval_micros != 0.0
+    ):
         start_timestamp = data_table["timestamps"][start_index].as_py()
         # create timestamps for every point that needs to be added
         new_timestamps = start_timestamp + np.arange(1, num_samples_to_add + 1) * sample_interval_micros
         if point_creation_mode == DataPointCreationMode.COPY:
             # copy the start point
             copy_row = data_table.slice(start_index, 1).to_pydict()
             for t in new_timestamps:
                 copy_row["timestamps"] = [t]
                 # for k in copy_row.keys():
                 #     new_dict[k].append(copy_row[k])
             empty_df = pa.Table.from_pydict(copy_row)
         elif point_creation_mode == DataPointCreationMode.INTERPOLATE:
             # use the start point and the next point as the edges for interpolation
             start_point = data_table.slice(start_index, 1).to_pydict()
-            numeric_start = start_point[[col for col in data_table.schema.names
-                                         if col not in NON_INTERPOLATED_COLUMNS + NON_NUMERIC_COLUMNS]]
+            numeric_start = start_point[
+                [col for col in data_table.schema.names if col not in NON_INTERPOLATED_COLUMNS + NON_NUMERIC_COLUMNS]
+            ]
             non_numeric_start = start_point[[col for col in data_table.schema.names if col in NON_NUMERIC_COLUMNS]]
             end_point = data_table.slice(start_index + (1 if sample_interval_micros > 0 else -1), 1).to_pydict()
-            numeric_end = end_point[[col for col in data_table.schema.names
-                                     if col not in NON_INTERPOLATED_COLUMNS + NON_NUMERIC_COLUMNS]]
+            numeric_end = end_point[
+                [col for col in data_table.schema.names if col not in NON_INTERPOLATED_COLUMNS + NON_NUMERIC_COLUMNS]
+            ]
             non_numeric_end = end_point[[col for col in data_table.schema.names if col in NON_NUMERIC_COLUMNS]]
-            if np.abs(start_point["timestamps"] - new_timestamps[0]) \
-                    <= np.abs(end_point["timestamps"] - new_timestamps[0]):
+            if np.abs(start_point["timestamps"] - new_timestamps[0]) <= np.abs(
+                end_point["timestamps"] - new_timestamps[0]
+            ):
                 non_numeric_diff = non_numeric_start
             else:
                 non_numeric_diff = non_numeric_end
             numeric_diff = numeric_end - numeric_start
-            numeric_diff = \
-                (numeric_diff / numeric_diff["timestamps"]) * \
-                (new_timestamps - numeric_start) + numeric_start
+            numeric_diff = (numeric_diff / numeric_diff["timestamps"]) * (
+                new_timestamps - numeric_start
+            ) + numeric_start
             if sys.version_info[0] > 3 or (sys.version_info[0] == 3 and sys.version_info[1] >= 9):
                 # merge dicts (python 3.9):
                 empty_df = pa.Table.from_pydict(numeric_diff | non_numeric_diff)
             else:
                 # merge dicts (python 3.5 to 3.8)
                 empty_df = pa.Table.from_pydict({**numeric_diff, **non_numeric_diff})
         else:
@@ -322,22 +347,24 @@
                 elif column_index == "image_codec":
                     empty_dict[column_index] = [ImageCodec["UNKNOWN"].value for i in range(num_samples_to_add)]
                 elif column_index == "audio_codec":
                     empty_dict[column_index] = [AudioCodec["UNKNOWN"].value for i in range(num_samples_to_add)]
                 elif column_index == "network_type":
                     empty_dict[column_index] = [NetworkType["UNKNOWN_NETWORK"].value for i in range(num_samples_to_add)]
                 elif column_index == "power_state":
-                    empty_dict[column_index] = [PowerState["UNKNOWN_POWER_STATE"].value
-                                                for i in range(num_samples_to_add)]
+                    empty_dict[column_index] = [
+                        PowerState["UNKNOWN_POWER_STATE"].value for i in range(num_samples_to_add)
+                    ]
                 elif column_index == "cell_service":
                     empty_dict[column_index] = [CellServiceState["UNKNOWN"].value for i in range(num_samples_to_add)]
                 elif column_index == "wifi_wake_lock":
                     empty_dict[column_index] = [WifiWakeLock["NONE"].value for i in range(num_samples_to_add)]
                 elif column_index == "screen_state":
-                    empty_dict[column_index] = [ScreenState["UNKNOWN_SCREEN_STATE"].value
-                                                for i in range(num_samples_to_add)]
+                    empty_dict[column_index] = [
+                        ScreenState["UNKNOWN_SCREEN_STATE"].value for i in range(num_samples_to_add)
+                    ]
                 else:
                     empty_dict[column_index] = np.full(num_samples_to_add, np.nan).tolist()
             empty_df = pa.Table.from_pydict(empty_dict)
         data_table = pa.concat_tables([data_table, empty_df])
 
     return data_table
```

### Comparing `redvox-3.4.2/redvox/common/gui/cloud_data_retrieval.py` & `redvox-3.5.0/redvox/common/gui/cloud_data_retrieval.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/common/io.py` & `redvox-3.5.0/redvox/common/io.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -130,14 +130,20 @@
 
     def __str__(self):
         return f"file_name: {self.file_name}, " \
                f"extension: {self.file_extension}, " \
                f"base_dir: {self.base_dir}, " \
                f"save_mode: {self._save_mode.name if hasattr(self, '_save_mode') else FileSystemSaveMode.TEMP.name}"
 
+    def __del__(self):
+        """
+        remove temp dir
+        """
+        self._temp_dir.cleanup()
+
     def is_use_temp(self) -> bool:
         """
         :return: if writing to temp dir
         """
         if hasattr(self, "_save_mode"):
             return self._save_mode == FileSystemSaveMode.TEMP
         return False
@@ -274,20 +280,14 @@
                 remove_dir_contents(Path(self.save_dir()))
             else:
                 os.makedirs(self.save_dir())
         elif self.is_use_temp():
             self._temp_dir.cleanup()
             self._temp_dir = tempfile.TemporaryDirectory()
 
-    def __del__(self):
-        """
-        remove temp dir
-        """
-        self._temp_dir.cleanup()
-
     def as_dict(self) -> dict:
         """
         :return: FileSystemWriter as dictionary
         """
         return {
             "file_name": self.file_name,
             "file_extension": self.file_extension,
```

### Comparing `redvox-3.4.2/redvox/common/offset_model.py` & `redvox-3.5.0/redvox/common/offset_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Offset model used to predict offset change over a period of time
 
 Author: Samuel Kei Takazawa
+Maintained by: Tyler Yoshiyama
 """
 
 from datetime import timedelta, datetime
 from typing import Tuple, Optional, List, TYPE_CHECKING
 
 import numpy as np
 import pandas as pd
@@ -17,14 +18,15 @@
 import redvox.common.date_time_utils as dt_utils
 
 
 MIN_VALID_LATENCY_MICROS = 100  # minimum value of latency before it's unreliable
 DEFAULT_SAMPLES = 3  # default number of samples per bin
 MIN_SAMPLES = 3  # minimum number of samples per 5 minutes for reliable data
 MIN_TIMESYNC_DURATION_MIN = 5  # minimum number of minutes of data required to produce reliable results
+GPS_LATENCY_MICROS = 60000  # estimated latency for GPS communications
 
 
 __MIN_VALID_LATENCY_MICROS: Optional[float] = MIN_VALID_LATENCY_MICROS
 
 
 __MIN_SAMPLES: Optional[float] = MIN_SAMPLES
 
@@ -94,19 +96,26 @@
         __MIN_TIMESYNC_DURATION_MIN = MIN_TIMESYNC_DURATION_MIN
     return __MIN_TIMESYNC_DURATION_MIN
 
 
 class OffsetModel:
     """
     Offset model which represents the change in offset over a period of time
-    Computes and returns the slope and intercept for the offset function (offset = slope * time + intercept)
-    Invalidates latencies that are below our recognition threshold MIN_VALID_LATENCY_MICROS
-    The data is binned by k_bins in equally spaced times; in each bin the n_samples best latencies are taken to get
+
+    * All timestamps are in microseconds since epoch UTC.
+
+    * Computes and returns the slope and intercept for the offset function (offset = slope * time + intercept)
+
+    * Invalidates latencies that are below our recognition threshold MIN_VALID_LATENCY_MICROS
+
+    * The data is binned by k_bins in equally spaced times; in each bin the n_samples best latencies are taken to get
     the weighted linear regression.
-    All timestamps are in microseconds since epoch UTC.
+
+    * If given zero latencies, but an equal number of offsets and timestamps, it will assume you are giving it GPS data
+    and will put all values into a single bin with equal weights on all values.
 
     Properties:
         start_time: float, start timestamp of model in microseconds since epoch UTC
 
         end_time: float, end timestamp of model in microseconds since epoch UTC
 
         k_bins: int, the number of data bins used to create the model, default is 1 if model is empty
@@ -130,25 +139,25 @@
         min_samples_per_bin: int, the minimum number of samples per bin of data for the model to be reliable.
         default 3
 
         min_timesync_dur_min: int, the minimum number of minutes of data for the model to be reliable.  default 5
     """
 
     def __init__(
-            self,
-            latencies: np.ndarray,
-            offsets: np.ndarray,
-            times: np.ndarray,
-            start_time: float,
-            end_time: float,
-            n_samples: int = DEFAULT_SAMPLES,
-            debug: bool = False,
-            min_valid_latency_us: Optional[float] = None,
-            min_samples_per_bin: Optional[int] = None,
-            min_timesync_dur_min: Optional[int] = None
+        self,
+        latencies: np.ndarray,
+        offsets: np.ndarray,
+        times: np.ndarray,
+        start_time: float,
+        end_time: float,
+        n_samples: int = DEFAULT_SAMPLES,
+        debug: bool = False,
+        min_valid_latency_us: Optional[float] = None,
+        min_samples_per_bin: Optional[int] = None,
+        min_timesync_dur_min: Optional[int] = None,
     ):
         """
         Create an OffsetModel
 
         :param latencies: latencies within the time specified
         :param offsets: offsets that correspond to the latencies
         :param times: timestamps that correspond to the latencies
@@ -162,37 +171,46 @@
         :param min_timesync_dur_min: the minimum number of minutes of data for the model to be reliable.  default 5
         """
         self.start_time = start_time
         self.end_time = end_time
         self.k_bins = get_bins_per_5min(start_time, end_time)
         self.n_samples = n_samples
         self.debug = debug
-        self.min_valid_latency_micros = \
+        self.min_valid_latency_micros = (
             get_min_valid_latency_micros() if min_valid_latency_us is None else min_valid_latency_us
+        )
         self.min_samples_per_bin = get_min_samples() if min_samples_per_bin is None else min_samples_per_bin
         self.min_timesync_dur_min = get_min_timesync_dur() if min_timesync_dur_min is None else min_timesync_dur_min
+        use_bins = True
         if len(latencies) > 0:
             latencies = np.where(latencies < self.min_valid_latency_micros, np.nan, latencies)
-            use_model = timesync_quality_check(latencies, start_time, end_time, self.debug,
-                                               self.min_timesync_dur_min, self.min_samples_per_bin)
+            use_model = timesync_quality_check(
+                latencies, start_time, end_time, self.debug, self.min_timesync_dur_min, self.min_samples_per_bin
+            )
+        elif len(offsets) > 0 and len(offsets) == len(times):
+            latencies = np.full(len(offsets), GPS_LATENCY_MICROS)
+            use_model = True
+            use_bins = False
         else:
             use_model = False
         if use_model:
             # Organize the data into a data frame
             full_df = pd.DataFrame(data=times, columns=["times"])
             full_df["latencies"] = latencies
             full_df["offsets"] = offsets
 
-            # Get the index for the separations (add +1 to k_bins so that there would be k_bins bins)
-            bin_times = np.linspace(start_time, end_time, self.k_bins + 1)
+            if use_bins:
+                # Get the index for the separations (add +1 to k_bins so that there would be k_bins bins)
+                bin_times = np.linspace(start_time, end_time, self.k_bins + 1)
 
-            # Make the dataframe with the data with n_samples per bins
-            binned_df = get_binned_df(
-                full_df=full_df, bin_times=bin_times, n_samples=n_samples
-            )
+                # Make the dataframe with the data with n_samples per bins
+                binned_df = get_binned_df(full_df=full_df, bin_times=bin_times, n_samples=n_samples)
+            else:
+                # everything is in one bin
+                binned_df = full_df.sort_values(by=["times"])
 
             # Compute the weighted linear regression
             self.slope, zero_intercept, self.score = offset_weighted_linear_regression(
                 latencies=binned_df["latencies"].values,
                 offsets=binned_df["offsets"].values,
                 times=binned_df["times"].values,
             )
@@ -206,56 +224,60 @@
             )
 
             self.mean_latency = np.nanmean(binned_df["latencies"].values)
             self.std_dev_latency = np.nanstd(binned_df["latencies"].values)
 
             # slope == 0 means constant offset, so if slope is not 0, model is good.
             use_model = self.slope != 0.0
-        # if data or model is not sufficient, use the offset corresponding to lowest latency:
+        # if data or model is not sufficient, use the offset corresponding to the lowest latency:
         if not use_model:
             self.score = 0.0
             self.slope = 0.0
             if all(np.nan_to_num(latencies) == 0.0):
                 self.intercept = 0.0
                 self.mean_latency = 0.0
                 self.std_dev_latency = 0.0
             else:
                 best_latency = np.nanmin(latencies[np.nonzero(latencies)])
                 self.intercept = offsets[np.argwhere(latencies == best_latency)[0][0]]
                 self.mean_latency = np.nanmean(latencies)
                 self.std_dev_latency = np.nanstd(latencies)
 
     def __repr__(self):
-        return f"start_time: {self.start_time}, " \
-               f"end_time: {self.end_time}, " \
-               f"k_bins: {self.k_bins}, " \
-               f"n_samples: {self.n_samples}, " \
-               f"slope: {self.slope}, " \
-               f"intercept: {self.intercept}, " \
-               f"score: {self.score}, " \
-               f"mean_latency: {self.mean_latency}, " \
-               f"std_dev_latency: {self.std_dev_latency}, " \
-               f"min_valid_latency_micros: {self.min_valid_latency_micros}, " \
-               f"min_samples_per_bin: {self.min_samples_per_bin}, " \
-               f"min_timesync_dur_min: {self.min_timesync_dur_min}, " \
-               f"debug: {self.debug}"
+        return (
+            f"start_time: {self.start_time}, "
+            f"end_time: {self.end_time}, "
+            f"k_bins: {self.k_bins}, "
+            f"n_samples: {self.n_samples}, "
+            f"slope: {self.slope}, "
+            f"intercept: {self.intercept}, "
+            f"score: {self.score}, "
+            f"mean_latency: {self.mean_latency}, "
+            f"std_dev_latency: {self.std_dev_latency}, "
+            f"min_valid_latency_micros: {self.min_valid_latency_micros}, "
+            f"min_samples_per_bin: {self.min_samples_per_bin}, "
+            f"min_timesync_dur_min: {self.min_timesync_dur_min}, "
+            f"debug: {self.debug}"
+        )
 
     def __str__(self):
-        return f"start_time: {self.start_time}, " \
-               f"end_time: {self.end_time}, " \
-               f"k_bins: {self.k_bins}, " \
-               f"n_samples: {self.n_samples}, " \
-               f"slope: {self.slope}, " \
-               f"intercept: {self.intercept}, " \
-               f"score: {self.score}, " \
-               f"mean_latency: {self.mean_latency}, " \
-               f"std_dev_latency: {self.std_dev_latency}, " \
-               f"min_valid_latency_micros: {self.min_valid_latency_micros}, " \
-               f"min_samples_per_bin: {self.min_samples_per_bin}, " \
-               f"min_timesync_dur_min: {self.min_timesync_dur_min}"
+        return (
+            f"start_time: {self.start_time}, "
+            f"end_time: {self.end_time}, "
+            f"k_bins: {self.k_bins}, "
+            f"n_samples: {self.n_samples}, "
+            f"slope: {self.slope}, "
+            f"intercept: {self.intercept}, "
+            f"score: {self.score}, "
+            f"mean_latency: {self.mean_latency}, "
+            f"std_dev_latency: {self.std_dev_latency}, "
+            f"min_valid_latency_micros: {self.min_valid_latency_micros}, "
+            f"min_samples_per_bin: {self.min_samples_per_bin}, "
+            f"min_timesync_dur_min: {self.min_timesync_dur_min}"
+        )
 
     def as_dict(self) -> dict:
         """
         :return: OffsetModel as a dictionary
         """
         return {
             "start_time": self.start_time,
@@ -266,15 +288,15 @@
             "intercept": self.intercept,
             "score": self.score,
             "mean_latency": self.mean_latency,
             "std_dev_latency": self.std_dev_latency,
             "min_valid_latency_micros": self.min_valid_latency_micros,
             "min_samples_per_bin": self.min_samples_per_bin,
             "min_timesync_dur_min": self.min_timesync_dur_min,
-            "debug": self.debug
+            "debug": self.debug,
         }
 
     @staticmethod
     def from_dict(data: dict) -> "OffsetModel":
         """
         create OffsetModel from a dictionary
 
@@ -304,20 +326,18 @@
         """
         return OffsetModel(np.array([]), np.array([]), np.array([]), 0, 0)
 
     def get_offset_at_time(self, time: float) -> float:
         """
         Gets offset at time based on the offset model.
 
-        :param time: The time corresponding to the new offset
+        :param time: The time to get the new offset for
         :return: new offset corresponding to the time
         """
-        return get_offset_at_new_time(
-            time, self.slope, self.intercept, self.start_time
-        )
+        return get_offset_at_new_time(time, self.slope, self.intercept, self.start_time)
 
     def update_time(self, time: float, use_model_function: bool = True) -> float:
         """
         update time based on the offset model.
 
         :param time: The time to update
         :param use_model_function: if True, use the slope of the model, otherwise use the intercept.  default True
@@ -364,27 +384,23 @@
     # Divide the duration by 5 minutes
     return int((end_time - start_time) / (1e6 * 300) + 1)
 
 
 # min max scaling for the weights
 def minmax_scale(data: np.ndarray) -> np.ndarray:
     """
-    Returns scaled data by subtracting the min value and dividing by (max - min) value.
-
     :param data: the data to be scaled
-    :return: scaled data
+    :return: data scaled by subtracting the min value and dividing by (max - min) value.
     """
     # Use np.nanmin and np.nanmax to avoid issues with nan values
     return (data - np.nanmin(data)) / (np.nanmax(data) - np.nanmin(data))
 
 
 # The score for Weighted Linear Regression Function
-def get_wlr_score(
-        model: LinearRegression, offsets: np.ndarray, times: np.ndarray, weights: np.ndarray
-) -> float:
+def get_wlr_score(model: LinearRegression, offsets: np.ndarray, times: np.ndarray, weights: np.ndarray) -> float:
     """
     Computes and returns a R2 score for the weighted linear regression using sklearn's score method.
     The best value is 1.0, and 0.0 corresponds to a function with no slope.
     Negative values are also adjusted to be 0.0.
 
     :param model: The linear regression model
     :param offsets: array of offsets corresponding to the best latencies per packet
@@ -400,15 +416,15 @@
 
     # Adjust the score so negative values are cast to 0.0
     return np.max([score, 0.0])
 
 
 # The Weighted Linear Regression Function for offsets
 def offset_weighted_linear_regression(
-        latencies: np.ndarray, offsets: np.ndarray, times: np.ndarray
+    latencies: np.ndarray, offsets: np.ndarray, times: np.ndarray
 ) -> Tuple[float, float, float]:
     """
     Computes and returns the slope and intercept for the offset function (offset = slope * time + intercept)
     The intercept is based on first UTC time 0, all units are in microseconds
     The function uses sklearn's LinearRegression with sample weights, and also returns the R2 score.
 
     :param latencies: array of the best latencies per packet
@@ -423,22 +439,23 @@
         # remove nan values for sklearn sake
         times = times[~np.isnan(latencies)]
         offsets = offsets[~np.isnan(latencies)]
         latencies = latencies[~np.isnan(latencies)]
 
     # Compute the weights for the linear regression by the latencies
     latencies_ms = latencies / 1e3
-    weights = latencies_ms ** -2
-    norm_weights = minmax_scale(weights)
+    weights = latencies_ms**-2
+    if np.all(weights == weights[0]):
+        norm_weights = None
+    else:
+        norm_weights = minmax_scale(weights)
 
     # Set up the weighted linear regression
     wls = LinearRegression()
-    wls.fit(
-        X=times.reshape(-1, 1), y=offsets.reshape(-1, 1), sample_weight=norm_weights
-    )
+    wls.fit(X=times.reshape(-1, 1), y=offsets.reshape(-1, 1), sample_weight=norm_weights)
 
     # get the score of the model
     score = get_wlr_score(model=wls, offsets=offsets, times=times, weights=norm_weights)
 
     # return the slope and intercept
     return wls.coef_[0][0], wls.intercept_[0], score
 
@@ -448,56 +465,51 @@
     Computes and returns the slope and intercept for the offset function (offset = slope * time + intercept)
     for GPS timestamps vs device timestamps
     The intercept is based on first UTC time 0, all units are in microseconds
     The function uses sklearn's LinearRegression with no weights.
 
     :param offsets: array of offsets
     :param times: array of device times used to get the offsets
-    :return: slope, intercept
+    :return: slope of the model line, offset intercept at UTC 0
     """
     # Set up the linear regression
     wls = LinearRegression()
-    wls.fit(
-        X=times.reshape(-1, 1), y=offsets.reshape(-1, 1))
+    wls.fit(X=times.reshape(-1, 1), y=offsets.reshape(-1, 1))
     intercept = get_offset_at_new_time(
         new_time=times[0],
         slope=wls.coef_[0][0],
         intercept=wls.intercept_[0],
         model_time=0,
     )
     # return the slope and intercept
     return wls.coef_[0][0], intercept
 
 
 # Function to correct the intercept value
-def get_offset_at_new_time(
-        new_time: float, slope: float, intercept: float, model_time: float
-) -> float:
+def get_offset_at_new_time(new_time: float, slope: float, intercept: float, model_time: float) -> float:
     """
     Gets offset at new_time time based on the offset model.
 
-    :param new_time: The time of corresponding to the new offset
+    :param new_time: The time to get the new offset at
     :param slope: slope of the offset model
     :param intercept: the intercept of the offset model relative to the model_time
-    :param model_time: the time corresponding to the intercept of the offset model
-    :return: new offset corresponding to the new_time
+    :param model_time: the starting time corresponding to the intercept of the offset model
+    :return: new offset at the new_time
     """
     # get the time difference
     time_diff = new_time - model_time
 
     # apply the offset model to get new intercept
     new_offset = slope * time_diff + intercept
 
     return new_offset
 
 
 # Function to get the subset data frame to do the weighted linear regression
-def get_binned_df(
-        full_df: pd.DataFrame, bin_times: np.ndarray, n_samples: float
-) -> pd.DataFrame:
+def get_binned_df(full_df: pd.DataFrame, bin_times: np.ndarray, n_samples: float) -> pd.DataFrame:
     """
     Returns a subset of the full_df with n_samples per binned times.
     nan latencies values will be ignored.
 
     :param full_df: pandas DataFrame containing latencies, offsets, and times.
     :param bin_times: array of edge times for each bin
     :param n_samples: number of samples to take per bin
@@ -522,16 +534,20 @@
     # Sort the binned_df by time
     binned_df = binned_df.sort_values(by=["times"])
 
     return binned_df
 
 
 def timesync_quality_check(
-        latencies: np.ndarray, start_time: float, end_time: float, debug: bool = False,
-        min_timesync_dur_mins: Optional[int] = None, min_samples: Optional[int] = None
+    latencies: np.ndarray,
+    start_time: float,
+    end_time: float,
+    debug: bool = False,
+    min_timesync_dur_mins: Optional[int] = None,
+    min_samples: Optional[int] = None,
 ) -> bool:
     """
     Checks quality of timesync data to determine if offset model should be used.
     The following list is the quality check:
         If timesync duration is longer than min_timesync_dur_mins (default 5) min
         If there are min_samples (default 3) latency values (non-nan) per 5 minutes on average
     Returns False if the data quality is not up to "standards".
@@ -620,33 +636,25 @@
         times[i] = stat.best_latency_timestamp
 
     if len(latencies) == 0:
         return None
 
     # Prep clock model
     start_dt: datetime = station_stats[0].packet_start_dt
-    end_dt: datetime = (
-            station_stats[-1].packet_start_dt + station_stats[-1].packet_duration
-    )
+    end_dt: datetime = station_stats[-1].packet_start_dt + station_stats[-1].packet_duration
     start_time: float = dt_utils.datetime_to_epoch_microseconds_utc(start_dt)
     end_time: float = dt_utils.datetime_to_epoch_microseconds_utc(end_dt)
 
     model: OffsetModel = OffsetModel(latencies, offsets, times, start_time, end_time)
 
     # Compute new start and end offsets
-    start_offset: timedelta = timedelta(
-        microseconds=model.get_offset_at_time(start_time)
-    )
-    end_offset: timedelta = timedelta(
-        microseconds=model.get_offset_at_time(end_time)
-    )
+    start_offset: timedelta = timedelta(microseconds=model.get_offset_at_time(start_time))
+    end_offset: timedelta = timedelta(microseconds=model.get_offset_at_time(end_time))
 
-    return TimingOffsets(
-        start_offset, start_dt + start_offset, end_offset, end_dt + end_offset
-    )
+    return TimingOffsets(start_offset, start_dt + start_offset, end_offset, end_dt + end_offset)
 
 
 def model_from_stats(station_stats: List["StationStat"]) -> Optional[OffsetModel]:
     """
     Computes the offset model from the provided station statistics.
 
     :param station_stats: Statistics to compute model from.
@@ -669,14 +677,12 @@
         times[i] = stat.best_latency_timestamp
 
     if len(latencies) == 0:
         return None
 
     # Prep clock model
     start_dt: datetime = station_stats[0].packet_start_dt
-    end_dt: datetime = (
-            station_stats[-1].packet_start_dt + station_stats[-1].packet_duration
-    )
+    end_dt: datetime = station_stats[-1].packet_start_dt + station_stats[-1].packet_duration
     start_time: float = dt_utils.datetime_to_epoch_microseconds_utc(start_dt)
     end_time: float = dt_utils.datetime_to_epoch_microseconds_utc(end_dt)
 
     return OffsetModel(latencies, offsets, times, start_time, end_time)
```

### Comparing `redvox-3.4.2/redvox/common/packet_to_pyarrow.py` & `redvox-3.5.0/redvox/common/packet_to_pyarrow.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+Converts data from RedVox packets into pyarrow tables.
+"""
+
 from typing import Optional, Dict, Callable, List, Tuple
 import os
 from pathlib import Path
 from itertools import repeat
 from glob import glob
 
 import numpy as np
@@ -15,32 +19,44 @@
 from redvox.common import sensor_reader_utils as srupa
 from redvox.common import date_time_utils as dtu
 from redvox.common import gap_and_pad_utils as gpu
 from redvox.common.sensor_data import SensorType
 from redvox.common.errors import RedVoxExceptions
 
 
-packet_schema = pa.schema([("packet_start_mach_timestamp", pa.float64()),
-                           ("packet_end_mach_timestamp", pa.float64()),
-                           ("packet_start_os_timestamp", pa.float64()),
-                           ("packet_end_os_timestamp", pa.float64()),
-                           ("timing_info_score", pa.int64())
-                           ])
-
-sensor_schema = pa.schema([("description", pa.string()),
-                           ("first_timestamp", pa.float64())
-                           ])
-
-station_schema = pa.schema([("id", pa.string()), ("uuid", pa.string()),
-                            ("start_time", pa.float64()), ("api", pa.float64()),
-                            ("sub_api", pa.float64()), ("make", pa.string()),
-                            ("model", pa.string()), ("os", pa.int64()), ("os_version", pa.string()),
-                            ("app", pa.string()), ("app_version", pa.string()),
-                            ("is_private", pa.bool_()), ("packet_duration_s", pa.float64()),
-                            ("station_description", pa.string())])
+packet_schema = pa.schema(
+    [
+        ("packet_start_mach_timestamp", pa.float64()),
+        ("packet_end_mach_timestamp", pa.float64()),
+        ("packet_start_os_timestamp", pa.float64()),
+        ("packet_end_os_timestamp", pa.float64()),
+        ("timing_info_score", pa.int64()),
+    ]
+)
+
+sensor_schema = pa.schema([("description", pa.string()), ("first_timestamp", pa.float64())])
+
+station_schema = pa.schema(
+    [
+        ("id", pa.string()),
+        ("uuid", pa.string()),
+        ("start_time", pa.float64()),
+        ("api", pa.float64()),
+        ("sub_api", pa.float64()),
+        ("make", pa.string()),
+        ("model", pa.string()),
+        ("os", pa.int64()),
+        ("os_version", pa.string()),
+        ("app", pa.string()),
+        ("app_version", pa.string()),
+        ("is_private", pa.bool_()),
+        ("packet_duration_s", pa.float64()),
+        ("station_description", pa.string()),
+    ]
+)
 
 
 @dataclass_json
 @dataclass
 class PyarrowSummary:
     """
     Summary of a sensor using Pyarrow Tables or parquet files to store the data
@@ -60,39 +76,25 @@
 
         smint: float, mean interval of sample rate in seconds
 
         sstd: float, std dev of sample rate in seconds
 
         _data: optional data as a Pyarrow Table
     """
+
     name: str
     stype: srupa.SensorType
     start: float
     srate_hz: float
     fdir: str
     scount: int
     smint_s: float = np.nan
     sstd_s: float = np.nan
     _data: Optional[pa.Table] = None
 
-    def to_dict(self) -> dict:
-        """
-        :return: dictionary representation of the data
-        """
-        return {
-            "name": self.name,
-            "stype": self.stype.name,
-            "start": self.start,
-            "srate_hz": self.srate_hz,
-            "fdir": self.fdir,
-            "smint_s": self.smint_s,
-            "sstd_s": self.sstd_s,
-            "scount": self.scount
-        }
-
     def file_name(self) -> str:
         """
         :return: full path and file name of where the file should exist
         """
         return os.path.join(self.fdir, f"{self.stype.name}_{int(self.start)}.parquet")
 
     def fdir_stem(self) -> str:
@@ -147,40 +149,20 @@
     """
     aggregate of summaries
 
     properties:
         summaries: the summaries of sensors
         gaps: gaps in audio data as a list of tuples of start and end time
     """
+
     summaries: List[PyarrowSummary] = field(default_factory=lambda: [])
     gaps: List[Tuple[float, float]] = field(default_factory=lambda: [])
     errors: RedVoxExceptions = RedVoxExceptions("AggregateSummary")
 
-    def to_dict(self) -> dict:
-        """
-        :return: dictionary representation of all summaries
-        """
-        result = {}
-        for ps in self.summaries:
-            result[ps.stype.name] = ps.to_dict()
-        return result
-
-    @staticmethod
-    def from_dict(summary_dict: dict) -> "AggregateSummary":
-        """
-        :param summary_dict: dictionary to load data from
-        :return: AggregateSummary from a dictionary
-        """
-        result = AggregateSummary()
-        for v in summary_dict.values():
-            result.summaries.append(PyarrowSummary(v["name"], SensorType[v["stype"]], v["start"], v["srate_hz"],
-                                                   v["fdir"], v["scount"], v["smint_s"], v["sstd_s"]))
-        return result
-
-    def add_aggregate_summary(self, agg_sum: 'AggregateSummary'):
+    def add_aggregate_summary(self, agg_sum: "AggregateSummary"):
         """
         adds another aggregate summary to this one
 
         :param agg_sum: another aggregate summary to add
         """
         self.summaries.extend(agg_sum.summaries)
 
@@ -199,21 +181,27 @@
         pckt_info = []
         audio_lst = self.get_audio()
         frst_audio = audio_lst[0]
         use_mem = frst_audio.check_data()
         for adl in audio_lst:
             pckt_info.append((int(adl.start), adl.data()))
 
-        audio_data = gpu.fill_audio_gaps(pckt_info,
-                                         dtu.seconds_to_microseconds(1 / frst_audio.srate_hz)
-                                         )
+        audio_data = gpu.fill_audio_gaps(pckt_info, dtu.seconds_to_microseconds(1 / frst_audio.srate_hz))
         tbl = audio_data.create_timestamps()
-        frst_audio = PyarrowSummary(frst_audio.name, frst_audio.stype, frst_audio.start, frst_audio.srate_hz,
-                                    frst_audio.fdir, tbl.num_rows, frst_audio.smint_s, frst_audio.sstd_s,
-                                    tbl)
+        frst_audio = PyarrowSummary(
+            frst_audio.name,
+            frst_audio.stype,
+            frst_audio.start,
+            frst_audio.srate_hz,
+            frst_audio.fdir,
+            tbl.num_rows,
+            frst_audio.smint_s,
+            frst_audio.sstd_s,
+            tbl,
+        )
         if not use_mem:
             frst_audio.write_data(True)
 
         self.gaps = audio_data.gaps
         self.summaries = self.get_non_audio_list()
         self.add_summary(frst_audio)
 
@@ -251,23 +239,32 @@
                 if len(timestamps) > 1:
                     mnint = dtu.microseconds_to_seconds(float(np.mean(np.diff(timestamps))))
                     stdint = dtu.microseconds_to_seconds(float(np.std(np.diff(timestamps))))
                 else:
                     mnint = np.nan
                     stdint = np.nan
                 if not combined_mint + combined_std > mnint > combined_mint - combined_std:
-                    self.errors.append(f"Mean interval s of combined {styp.name} sensor does not match the "
-                                       f"compilation of individual mean interval s per packet.  Will use compilation "
-                                       f"of individual values.")
+                    self.errors.append(
+                        f"Mean interval s of combined {styp.name} sensor does not match the "
+                        f"compilation of individual mean interval s per packet.  Will use compilation "
+                        f"of individual values."
+                    )
                     mnint = combined_mint
                     stdint = combined_std
-                single_smry = PyarrowSummary(first_summary.name, styp, first_summary.start,
-                                             1 / mnint, first_summary.fdir, tbl.num_rows, mnint, stdint,
-                                             first_summary.data() if first_summary.check_data() else None
-                                             )
+                single_smry = PyarrowSummary(
+                    first_summary.name,
+                    styp,
+                    first_summary.start,
+                    1 / mnint,
+                    first_summary.fdir,
+                    tbl.num_rows,
+                    mnint,
+                    stdint,
+                    first_summary.data() if first_summary.check_data() else None,
+                )
                 self.summaries.append(single_smry)
 
     def merge_summaries_of_type(self, stype: SensorType):
         """
         combines and replaces multiple summaries of one SensorType into a single one
 
         *caution: using this on an audio sensor may cause data validation issues*
@@ -290,18 +287,25 @@
             if first_summary.check_data():
                 first_summary._data = tbl
             else:
                 pq.write_table(tbl, first_summary.file_name())
                 os.remove(smrys.file_name())
         mnint = dtu.microseconds_to_seconds(float(np.mean(np.diff(tbl["timestamps"].to_numpy()))))
         stdint = dtu.microseconds_to_seconds(float(np.std(np.diff(tbl["timestamps"].to_numpy()))))
-        single_smry = PyarrowSummary(first_summary.name, first_summary.stype, first_summary.start,
-                                     1 / mnint, first_summary.fdir, tbl.num_rows, mnint, stdint,
-                                     first_summary.data() if first_summary.check_data() else None
-                                     )
+        single_smry = PyarrowSummary(
+            first_summary.name,
+            first_summary.stype,
+            first_summary.start,
+            1 / mnint,
+            first_summary.fdir,
+            tbl.num_rows,
+            mnint,
+            stdint,
+            first_summary.data() if first_summary.check_data() else None,
+        )
         self.summaries = other_smrs
         self.summaries.append(single_smry)
 
     def merge_all_summaries(self):
         """
         merge all PyarrowSummary with the same sensor type into single PyarrowSummary per type
         """
@@ -350,31 +354,31 @@
 
 def stream_to_pyarrow(packets: List[RedvoxPacketM], out_dir: Optional[str] = None) -> AggregateSummary:
     """
     stream the packets to parquet files for later processing.
 
     :param packets: redvox packets to convert
     :param out_dir: optional directory to write the pyarrow files to; if None, don't write files.  default None
-    :return: summary of the sensors, their data and their file locations if possible
+    :return: AggregateSummary of the sensors' metadata, data, and location of the data if written to disk
     """
     summary = AggregateSummary()
     for k in map(packet_to_pyarrow, packets, repeat(out_dir)):
         for t in k.summaries:
             summary.add_summary(t)
 
     return summary
 
 
 def packet_to_pyarrow(packet: RedvoxPacketM, out_dir: Optional[str] = None) -> AggregateSummary:
     """
-    gets non-audio sensor information by writing it into folders with the sensor names to the out_dir
+    gets non-audio sensor information by keeping it memory or writing it into folders named with the sensor names
 
     :param packet: packet to extract data from
     :param out_dir: optional directory to write the pyarrow files to; if None, don't write files.  default None
-    :return: sensor type: sensor name, start_timestamp, sample rate (if fixed, np.nan otherwise)
+    :return: AggregateSummary of the sensors' metadata, data, and location of the data if written to disk
     """
     result = AggregateSummary()
     packet_start = int(packet.timing_information.packet_start_mach_timestamp)
     funcs = [
         load_apim_audio,
         load_apim_compressed_audio,
         load_apim_image,
@@ -412,36 +416,46 @@
 
     :param packet: packet with data to load
     :return: audio sensor type, name,  data and sample rate
     """
     if srupa.__has_sensor(packet, srupa.__AUDIO_FIELD_NAME):
         audio_sensor: RedvoxPacketM.Sensors.Audio = packet.sensors.audio
         return PyarrowSummary(
-            audio_sensor.sensor_description, srupa.SensorType.AUDIO, np.nan, audio_sensor.sample_rate, "",
-            int(audio_sensor.samples.value_statistics.count), 1./audio_sensor.sample_rate, 0.,
-            pa.Table.from_pydict({"microphone": np.array(audio_sensor.samples.values)})
+            audio_sensor.sensor_description,
+            srupa.SensorType.AUDIO,
+            np.nan,
+            audio_sensor.sample_rate,
+            "",
+            int(audio_sensor.samples.value_statistics.count),
+            1.0 / audio_sensor.sample_rate,
+            0.0,
+            pa.Table.from_pydict({"microphone": np.array(audio_sensor.samples.values)}),
         )
     return None
 
 
 def load_apim_compressed_audio(packet: RedvoxPacketM) -> Optional[PyarrowSummary]:
     """
     load compressed audio data from a single redvox packet
 
     :param packet: packet with data to load
     :return: compressed audio sensor data if it exists, None otherwise
     """
     if srupa.__has_sensor(packet, srupa.__COMPRESSED_AUDIO_FIELD_NAME):
-        comp_audio: RedvoxPacketM.Sensors.CompressedAudio = (
-            packet.sensors.compressed_audio
-        )
+        comp_audio: RedvoxPacketM.Sensors.CompressedAudio = packet.sensors.compressed_audio
         return PyarrowSummary(
-            comp_audio.sensor_description, srupa.SensorType.COMPRESSED_AUDIO, np.nan,
-            comp_audio.sample_rate, "", np.nan, 1./comp_audio.sample_rate, 0.,
-            srupa.apim_compressed_audio_to_pyarrow(comp_audio)
+            comp_audio.sensor_description,
+            srupa.SensorType.COMPRESSED_AUDIO,
+            np.nan,
+            comp_audio.sample_rate,
+            "",
+            np.nan,
+            1.0 / comp_audio.sample_rate,
+            0.0,
+            srupa.apim_compressed_audio_to_pyarrow(comp_audio),
         )
     return None
 
 
 def load_apim_image(packet: RedvoxPacketM) -> Optional[PyarrowSummary]:
     """
     load image data from a single redvox packet
@@ -450,23 +464,30 @@
     :return: image sensor data if it exists, None otherwise
     """
     if srupa.__has_sensor(packet, srupa.__IMAGE_FIELD_NAME):
         image_sensor: RedvoxPacketM.Sensors.Image = packet.sensors.image
         timestamps = image_sensor.timestamps.timestamps
         additional_inputs = packet.station_information.app_settings.additional_input_sensors
         if RedvoxPacketM.StationInformation.AppSettings.InputSensor.IMAGE_PER_SECOND in additional_inputs:
-            sample_rate = 1.
+            sample_rate = 1.0
         # elif RedvoxPacketM.StationInformation.AppSettings.InputSensor.IMAGE_PER_PACKET in additional_inputs:
         else:
             sample_rate = 1 / srupa.__packet_duration_s(packet)
         # else:
         #   sample_rate = np.nan
         return PyarrowSummary(
-            image_sensor.sensor_description, srupa.SensorType.IMAGE, np.nan, sample_rate, "",
-            len(timestamps), 1./sample_rate, 0., srupa.apim_image_to_pyarrow(image_sensor)
+            image_sensor.sensor_description,
+            srupa.SensorType.IMAGE,
+            np.nan,
+            sample_rate,
+            "",
+            len(timestamps),
+            1.0 / sample_rate,
+            0.0,
+            srupa.apim_image_to_pyarrow(image_sensor),
         )
     return None
 
 
 def load_apim_location(packet: RedvoxPacketM) -> Optional[PyarrowSummary]:
     """
     load location data from a single packet
@@ -479,18 +500,25 @@
         timestamps = loc.timestamps.timestamps
         if len(timestamps) > 0:
             if len(timestamps) > 1:
                 m_intv = dtu.microseconds_to_seconds(float(np.mean(np.diff(timestamps))))
                 intv_std = dtu.microseconds_to_seconds(float(np.std(np.diff(timestamps))))
             else:
                 m_intv = srupa.__packet_duration_s(packet)
-                intv_std = 0.
+                intv_std = 0.0
             return PyarrowSummary(
-                loc.sensor_description, srupa.SensorType.LOCATION, np.nan, np.nan, "",
-                len(timestamps), m_intv, intv_std, srupa.apim_location_to_pyarrow(loc)
+                loc.sensor_description,
+                srupa.SensorType.LOCATION,
+                np.nan,
+                np.nan,
+                "",
+                len(timestamps),
+                m_intv,
+                intv_std,
+                srupa.apim_location_to_pyarrow(loc),
             )
     return None
 
 
 def load_apim_best_location(packet: RedvoxPacketM) -> Optional[PyarrowSummary]:
     """
     load best location data from a single redvox packet
@@ -504,69 +532,84 @@
             best_loc: RedvoxPacketM.Sensors.Location.BestLocation
             if loc.HasField("last_best_location"):
                 best_loc = loc.last_best_location
             else:
                 best_loc = loc.overall_best_location
             packet_len_s = srupa.__packet_duration_s(packet)
             return PyarrowSummary(
-                loc.sensor_description, srupa.SensorType.BEST_LOCATION, np.nan,
-                1./packet_len_s, "", 1, packet_len_s, 0.,
-                srupa.apim_best_location_to_pyarrow(best_loc,
-                                                    packet.timing_information.packet_start_mach_timestamp),
+                loc.sensor_description,
+                srupa.SensorType.BEST_LOCATION,
+                np.nan,
+                1.0 / packet_len_s,
+                "",
+                1,
+                packet_len_s,
+                0.0,
+                srupa.apim_best_location_to_pyarrow(best_loc, packet.timing_information.packet_start_mach_timestamp),
             )
     return None
 
 
 def load_apim_health(packet: RedvoxPacketM) -> Optional[PyarrowSummary]:
     """
     load station health data from a single redvox packet
 
     :param packet: packet with data to load
     :return: station health data if it exists, None otherwise
     """
-    metrics: RedvoxPacketM.StationInformation.StationMetrics = (
-        packet.station_information.station_metrics
-    )
+    metrics: RedvoxPacketM.StationInformation.StationMetrics = packet.station_information.station_metrics
     timestamps = metrics.timestamps.timestamps
     rate = packet.station_information.app_settings.metrics_rate
     if rate == RedvoxPacketM.StationInformation.MetricsRate.ONCE_PER_SECOND:
         sample_rate = 1
     elif rate == RedvoxPacketM.StationInformation.MetricsRate.ONCE_PER_PACKET:
         sample_rate = 1 / srupa.__packet_duration_s(packet)
     else:
         sample_rate = np.nan
     if len(timestamps) > 0:
         return PyarrowSummary(
-            "station health", srupa.SensorType.STATION_HEALTH, np.nan, sample_rate, "",
-            len(timestamps), 1./sample_rate, 0., srupa.apim_health_to_pyarrow(metrics)
+            "station health",
+            srupa.SensorType.STATION_HEALTH,
+            np.nan,
+            sample_rate,
+            "",
+            len(timestamps),
+            1.0 / sample_rate,
+            0.0,
+            srupa.apim_health_to_pyarrow(metrics),
         )
     return None
 
 
 def load_single(
-        packet: RedvoxPacketM,
-        sensor_type: srupa.SensorType,
+    packet: RedvoxPacketM,
+    sensor_type: srupa.SensorType,
 ) -> Optional[PyarrowSummary]:
     field_name: str = srupa.__SENSOR_TYPE_TO_FIELD_NAME[sensor_type]
-    sensor_fn: Optional[
-        Callable[[RedvoxPacketM], srupa.Sensor]
-    ] = srupa.__SENSOR_TYPE_TO_SENSOR_FN[sensor_type]
+    sensor_fn: Optional[Callable[[RedvoxPacketM], srupa.Sensor]] = srupa.__SENSOR_TYPE_TO_SENSOR_FN[sensor_type]
     if srupa.__has_sensor(packet, field_name) and sensor_fn is not None:
         sensor = sensor_fn(packet)
         t = sensor.timestamps.timestamps
         if len(t) > 1:
             m_intv = dtu.microseconds_to_seconds(float(np.mean(np.diff(t))))
             intv_std = dtu.microseconds_to_seconds(float(np.std(np.diff(t))))
         else:
             m_intv = srupa.__packet_duration_s(packet)
-            intv_std = 0.
+            intv_std = 0.0
         if len(t) > 0:
             return PyarrowSummary(
-                sensor.sensor_description, sensor_type, np.nan, np.nan, "",
-                len(t), m_intv, intv_std, srupa.read_apim_single_sensor(sensor, field_name)
+                sensor.sensor_description,
+                sensor_type,
+                np.nan,
+                np.nan,
+                "",
+                len(t),
+                m_intv,
+                intv_std,
+                srupa.read_apim_single_sensor(sensor, field_name),
             )
     return None
 
 
 def load_apim_pressure(packet: RedvoxPacketM) -> Optional[PyarrowSummary]:
     """
     load pressure data from a single redvox packet
@@ -614,51 +657,58 @@
     :param packet: packet with data to load
     :return: relative humidity sensor data if it exists, None otherwise
     """
     return load_single(packet, srupa.SensorType.RELATIVE_HUMIDITY)
 
 
 def load_xyz(
-        packet: RedvoxPacketM,
-        sensor_type: srupa.SensorType,
+    packet: RedvoxPacketM,
+    sensor_type: srupa.SensorType,
 ) -> Optional[PyarrowSummary]:
     field_name: str = srupa.__SENSOR_TYPE_TO_FIELD_NAME[sensor_type]
-    sensor_fn: Optional[
-        Callable[[RedvoxPacketM], srupa.Sensor]
-    ] = srupa.__SENSOR_TYPE_TO_SENSOR_FN[sensor_type]
+    sensor_fn: Optional[Callable[[RedvoxPacketM], srupa.Sensor]] = srupa.__SENSOR_TYPE_TO_SENSOR_FN[sensor_type]
     if srupa.__has_sensor(packet, field_name) and sensor_fn is not None:
         sensor = sensor_fn(packet)
         t = sensor.timestamps.timestamps
         if len(t) > 1:
             m_intv = dtu.microseconds_to_seconds(float(np.mean(np.diff(t))))
             intv_std = dtu.microseconds_to_seconds(float(np.std(np.diff(t))))
         else:
             m_intv = srupa.__packet_duration_s(packet)
-            intv_std = 0.
+            intv_std = 0.0
         if len(t) > 0:
             # read packet.station_information.app_settings.additional_input_sensors for fast sensors
             # rename if needed
             return PyarrowSummary(
-                sensor.sensor_description, sensor_type, np.nan, np.nan, "",
-                len(t), m_intv, intv_std, srupa.read_apim_xyz_sensor(sensor, field_name)
+                sensor.sensor_description,
+                sensor_type,
+                np.nan,
+                np.nan,
+                "",
+                len(t),
+                m_intv,
+                intv_std,
+                srupa.read_apim_xyz_sensor(sensor, field_name),
             )
     return None
 
 
 def load_apim_accelerometer(packet: RedvoxPacketM) -> Optional[PyarrowSummary]:
     """
     load accelerometer data from a single redvox packet
 
     :param packet: packet with data to load
     :return: accelerometer sensor data if it exists, None otherwise
     """
     return load_xyz(packet, srupa.SensorType.ACCELEROMETER)
 
 
-def load_apim_magnetometer(packet: RedvoxPacketM,) -> Optional[PyarrowSummary]:
+def load_apim_magnetometer(
+    packet: RedvoxPacketM,
+) -> Optional[PyarrowSummary]:
     """
     load magnetometer data from a single redvox packet
 
     :param packet: packet with data to load
     :return: magnetometer sensor data if it exists, None otherwise
     """
     return load_xyz(packet, srupa.SensorType.MAGNETOMETER)
```

### Comparing `redvox-3.4.2/redvox/common/parallel_utils.py` & `redvox-3.5.0/redvox/common/parallel_utils.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/common/run_me.py` & `redvox-3.5.0/redvox/common/run_me.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/common/sensor_data.py` & `redvox-3.5.0/redvox/common/sensor_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import pyarrow as pa
 import pyarrow.compute as pc
 import pyarrow.dataset as ds
 import pyarrow.parquet as pq
 
 import redvox.common.sensor_io as io
 import redvox.common.date_time_utils as dtu
-from redvox.common.io import FileSystemSaveMode, FileSystemWriter as Fsw
+from redvox.common.io import FileSystemSaveMode, FileSystemWriter as Fsw, get_json_file, json_file_to_dict
 from redvox.common import offset_model as om
 from redvox.common.errors import RedVoxExceptions
 from redvox.common.gap_and_pad_utils import calc_evenly_sampled_timestamps, AudioWithGaps
 from redvox.api1000.wrapped_redvox_packet.station_information import (
     NetworkType,
     PowerState,
     CellServiceState,
@@ -28,22 +28,24 @@
     ScreenState,
 )
 from redvox.api1000.wrapped_redvox_packet.sensors.location import LocationProvider
 from redvox.api1000.wrapped_redvox_packet.sensors.image import ImageCodec
 from redvox.api1000.wrapped_redvox_packet.sensors.audio import AudioCodec
 
 # function used to translate values of enumerated columns
-COLUMN_TO_ENUM_FN = {"location_provider": lambda l: LocationProvider(l).name,
-                     "image_codec": lambda l: ImageCodec(l).name,
-                     "audio_codec": lambda l: AudioCodec(l).name,
-                     "network_type": lambda l: NetworkType(l).name,
-                     "power_state": lambda l: PowerState(l).name,
-                     "cell_service": lambda l: CellServiceState(l).name,
-                     "wifi_wake_lock": lambda l: WifiWakeLock(l).name,
-                     "screen_state": lambda l: ScreenState(l).name}
+COLUMN_TO_ENUM_FN = {
+    "location_provider": lambda l: LocationProvider(l).name,
+    "image_codec": lambda l: ImageCodec(l).name,
+    "audio_codec": lambda l: AudioCodec(l).name,
+    "network_type": lambda l: NetworkType(l).name,
+    "power_state": lambda l: PowerState(l).name,
+    "cell_service": lambda l: CellServiceState(l).name,
+    "wifi_wake_lock": lambda l: WifiWakeLock(l).name,
+    "screen_state": lambda l: ScreenState(l).name,
+}
 # columns that cannot be interpolated
 NON_INTERPOLATED_COLUMNS = ["compressed_audio", "image"]
 # columns that are not numeric but can be interpolated
 NON_NUMERIC_COLUMNS = list(COLUMN_TO_ENUM_FN.keys())
 
 
 class SensorType(enum.Enum):
@@ -68,31 +70,27 @@
     PROXIMITY = 14  # on, off, cm
     RELATIVE_HUMIDITY = 15  # percentage
     ROTATION_VECTOR = 16  # Unitless
     INFRARED = 17  # this is proximity
     STATION_HEALTH = 18
     # Health sensors: battery charge and current level, phone internal temperature, network source and strength,
     # available RAM of the system, cell service status, amount of hard disk space left, power charging state
-    # wifi lock state, cpu utilization, screen state, and screen brightness
+    # Wi-Fi lock state, cpu utilization, screen state, and screen brightness
     BEST_LOCATION = 19  # See standard
     VELOCITY = 20  # m/s
 
     @staticmethod
     def type_from_str(type_str: str) -> "SensorType":
         """
         converts a string to a sensor type
 
         :param type_str: string to convert
         :return: a sensor type, UNKNOWN_SENSOR is the default for invalid inputs
         """
-        if (
-                type_str.lower() == "audio"
-                or type_str.lower() == "mic"
-                or type_str.lower() == "microphone"
-        ):
+        if type_str.lower() == "audio" or type_str.lower() == "mic" or type_str.lower() == "microphone":
             return SensorType.AUDIO
         elif type_str.lower() == "accelerometer" or type_str.lower() == "accel":
             return SensorType.ACCELEROMETER
         elif type_str.lower() == "ambient_temperature":
             return SensorType.AMBIENT_TEMPERATURE
         elif type_str.lower() == "compressed_audio":
             return SensorType.COMPRESSED_AUDIO
@@ -100,32 +98,25 @@
             return SensorType.GRAVITY
         elif type_str.lower() == "gyroscope" or type_str.lower() == "gyro":
             return SensorType.GYROSCOPE
         elif type_str.lower() == "image":
             return SensorType.IMAGE
         elif type_str.lower() == "light":
             return SensorType.LIGHT
-        elif (
-                type_str.lower() == "linear_acceleration"
-                or type_str.lower() == "linear_accel"
-        ):
+        elif type_str.lower() == "linear_acceleration" or type_str.lower() == "linear_accel":
             return SensorType.LINEAR_ACCELERATION
         elif type_str.lower() == "location" or type_str.lower() == "loc":
             return SensorType.LOCATION
         elif type_str.lower() == "best_location" or type_str.lower() == "best_loc":
             return SensorType.BEST_LOCATION
         elif type_str.lower() == "magnetometer" or type_str.lower() == "mag":
             return SensorType.MAGNETOMETER
         elif type_str.lower() == "orientation":
             return SensorType.ORIENTATION
-        elif (
-                type_str.lower() == "pressure"
-                or type_str.lower() == "bar"
-                or type_str.lower() == "barometer"
-        ):
+        elif type_str.lower() == "pressure" or type_str.lower() == "bar" or type_str.lower() == "barometer":
             return SensorType.PRESSURE
         elif type_str.lower() == "proximity" or type_str.lower() == "infrared":
             return SensorType.PROXIMITY
         elif type_str.lower() == "relative_humidity":
             return SensorType.RELATIVE_HUMIDITY
         elif type_str.lower() == "rotation_vector":
             return SensorType.ROTATION_VECTOR
@@ -165,30 +156,30 @@
 
         _fs_writer: FileSystemWriter, handles file system i/o parameters
 
         _data: pyarrow Table, used to store the data when it's not written to the disk.  default None
     """
 
     def __init__(
-            self,
-            sensor_name: str,
-            sensor_data: Optional[pa.Table] = None,
-            sensor_type: SensorType = SensorType.UNKNOWN_SENSOR,
-            sample_rate_hz: float = np.nan,
-            sample_interval_s: float = np.nan,
-            sample_interval_std_s: float = np.nan,
-            is_sample_rate_fixed: bool = False,
-            are_timestamps_altered: bool = False,
-            calculate_stats: bool = False,
-            use_offset_model_for_correction: bool = False,
-            save_data: bool = False,
-            base_dir: str = ".",
-            gaps: Optional[List[Tuple[float, float]]] = None,
-            show_errors: bool = False,
-            use_temp_dir: bool = False
+        self,
+        sensor_name: str,
+        sensor_data: Optional[pa.Table] = None,
+        sensor_type: SensorType = SensorType.UNKNOWN_SENSOR,
+        sample_rate_hz: float = np.nan,
+        sample_interval_s: float = np.nan,
+        sample_interval_std_s: float = np.nan,
+        is_sample_rate_fixed: bool = False,
+        are_timestamps_altered: bool = False,
+        calculate_stats: bool = False,
+        use_offset_model_for_correction: bool = False,
+        save_data: bool = False,
+        base_dir: str = ".",
+        gaps: Optional[List[Tuple[float, float]]] = None,
+        show_errors: bool = False,
+        use_temp_dir: bool = False,
     ):
         """
         initialize the sensor data with params
 
         :param sensor_name: name of the sensor.  REQUIRED
         :param sensor_type: enumerated type of the sensor, default SensorType.UNKNOWN_SENSOR
         :param sensor_data: Optional pyarrow table with the timestamps and sensor data;
@@ -231,65 +222,69 @@
             save_mode = FileSystemSaveMode.MEM
         self._fs_writer = Fsw("", "parquet", base_dir, save_mode)
         self._gaps: List[Tuple] = gaps if gaps else []
         set_data_as_sensor_data = True
         if sensor_data is not None:
             if "timestamps" not in sensor_data.schema.names:
                 self._errors.append('must have a column titled "timestamps"')
-            elif sensor_data['timestamps'].length() > 0:
+            elif sensor_data["timestamps"].length() > 0:
                 set_data_as_sensor_data = False
-                if calculate_stats and np.isnan(sample_interval_s) and np.isnan(sample_rate_hz) \
-                        and np.isnan(sample_interval_std_s):
+                if calculate_stats:
                     self.organize_and_update_stats(sensor_data)
                 elif sensor_data["timestamps"].length() > 1:
                     self.sort_by_data_timestamps(sensor_data)
                 else:
                     self.write_pyarrow_table(sensor_data)
         if set_data_as_sensor_data:
             self._data = sensor_data
         if show_errors:
             self.print_errors()
 
     def __repr__(self):
-        return f"name: {self.name}, " \
-               f"type: {self._type.value}, " \
-               f"num_samples: {self.num_samples()}, " \
-               f"sample_rate_hz: {self._sample_rate_hz}, " \
-               f"sample_interval_s: {self._sample_interval_s}, " \
-               f"sample_interval_std_s: {self._sample_interval_std_s}, " \
-               f"is_sample_rate_fixed: {self._is_sample_rate_fixed}, " \
-               f"timestamps_altered: {self._timestamps_altered}, " \
-               f"use_offset_model: {self._use_offset_model}, " \
-               f"gaps: {[g for g in self._gaps]}"
+        return (
+            f"name: {self.name}, "
+            f"type: {self._type.value}, "
+            f"num_samples: {self.num_samples()}, "
+            f"sample_rate_hz: {self._sample_rate_hz}, "
+            f"sample_interval_s: {self._sample_interval_s}, "
+            f"sample_interval_std_s: {self._sample_interval_std_s}, "
+            f"is_sample_rate_fixed: {self._is_sample_rate_fixed}, "
+            f"timestamps_altered: {self._timestamps_altered}, "
+            f"use_offset_model: {self._use_offset_model}, "
+            f"gaps: {[g for g in self._gaps]}"
+        )
 
     def __str__(self):
-        return f"name: {self.name}, " \
-               f"type: {self._type.name}, " \
-               f"num_samples: {self.num_samples()}, " \
-               f"sample_rate_hz: {self._sample_rate_hz}, " \
-               f"sample_interval_s: {self._sample_interval_s}, " \
-               f"sample_interval_std_s: {self._sample_interval_std_s}, " \
-               f"is_sample_rate_fixed: {self._is_sample_rate_fixed}, " \
-               f"timestamps_altered: {self._timestamps_altered}, " \
-               f"use_offset_model: {self._use_offset_model}"
+        return (
+            f"name: {self.name}, "
+            f"type: {self._type.name}, "
+            f"num_samples: {self.num_samples()}, "
+            f"sample_rate_hz: {self._sample_rate_hz}, "
+            f"sample_interval_s: {self._sample_interval_s}, "
+            f"sample_interval_std_s: {self._sample_interval_std_s}, "
+            f"is_sample_rate_fixed: {self._is_sample_rate_fixed}, "
+            f"timestamps_altered: {self._timestamps_altered}, "
+            f"use_offset_model: {self._use_offset_model}"
+        )
 
     @staticmethod
     def from_dir(
-            sensor_name: str,
-            data_path: str,
-            sensor_type: SensorType = SensorType.UNKNOWN_SENSOR,
-            sample_rate_hz: float = np.nan,
-            sample_interval_s: float = np.nan,
-            sample_interval_std_s: float = np.nan,
-            is_sample_rate_fixed: bool = False,
-            are_timestamps_altered: bool = False,
-            calculate_stats: bool = False,
-            use_offset_model_for_correction: bool = False,
-            save_data: bool = False,
-            use_temp_dir: bool = False) -> "SensorData":
+        sensor_name: str,
+        data_path: str,
+        sensor_type: SensorType = SensorType.UNKNOWN_SENSOR,
+        sample_rate_hz: float = np.nan,
+        sample_interval_s: float = np.nan,
+        sample_interval_std_s: float = np.nan,
+        is_sample_rate_fixed: bool = False,
+        are_timestamps_altered: bool = False,
+        calculate_stats: bool = False,
+        use_offset_model_for_correction: bool = False,
+        save_data: bool = False,
+        use_temp_dir: bool = False,
+    ) -> "SensorData":
         """
         init but with a path to directory containing parquet file(s) instead of a table of data
 
         :param sensor_name: name of the sensor
         :param data_path: path to the directory containing the parquet files
         :param sensor_type: enumerated type of the sensor, default SensorType.UNKNOWN_SENSOR
         :param sample_rate_hz: sample rate in hz of the data, default np.nan
@@ -302,36 +297,46 @@
                                 default False
         :param use_offset_model_for_correction: if True, use an offset model to correct timestamps, otherwise
                                                 use the best known offset.  default False
         :param save_data: if True, save the data of the sensor to disk, otherwise use a temporary dir.  default False
         :param use_temp_dir: if True, save the data using a temporary directory.  default False
         :return: SensorData object
         """
-        result = SensorData(sensor_name,
-                            ds.dataset(data_path, format="parquet", exclude_invalid_files=True).to_table(),
-                            sensor_type, sample_rate_hz, sample_interval_s, sample_interval_std_s,
-                            is_sample_rate_fixed, are_timestamps_altered, calculate_stats,
-                            use_offset_model_for_correction, save_data, data_path, use_temp_dir=use_temp_dir)
+        result = SensorData(
+            sensor_name,
+            ds.dataset(data_path, format="parquet", exclude_invalid_files=True).to_table(),
+            sensor_type,
+            sample_rate_hz,
+            sample_interval_s,
+            sample_interval_std_s,
+            is_sample_rate_fixed,
+            are_timestamps_altered,
+            calculate_stats,
+            use_offset_model_for_correction,
+            save_data,
+            data_path,
+            use_temp_dir=use_temp_dir,
+        )
         return result
 
     @staticmethod
     def from_dict(
-            sensor_name: str,
-            sensor_data: Dict,
-            sensor_type: SensorType = SensorType.UNKNOWN_SENSOR,
-            sample_rate_hz: float = np.nan,
-            sample_interval_s: float = np.nan,
-            sample_interval_std_s: float = np.nan,
-            is_sample_rate_fixed: bool = False,
-            are_timestamps_altered: bool = False,
-            calculate_stats: bool = False,
-            use_offset_model_for_correction: bool = False,
-            save_data: bool = False,
-            arrow_dir: str = "",
-            use_temp_dir: bool = False
+        sensor_name: str,
+        sensor_data: Dict,
+        sensor_type: SensorType = SensorType.UNKNOWN_SENSOR,
+        sample_rate_hz: float = np.nan,
+        sample_interval_s: float = np.nan,
+        sample_interval_std_s: float = np.nan,
+        is_sample_rate_fixed: bool = False,
+        are_timestamps_altered: bool = False,
+        calculate_stats: bool = False,
+        use_offset_model_for_correction: bool = False,
+        save_data: bool = False,
+        arrow_dir: str = "",
+        use_temp_dir: bool = False,
     ) -> "SensorData":
         """
         init but with a dictionary
 
         :param sensor_name: name of the sensor
         :param sensor_type: enumerated type of the sensor, default SensorType.UNKNOWN_SENSOR
         :param sensor_data: dict with the timestamps and sensor data; first column is always the timestamps,
@@ -348,18 +353,29 @@
                                                 use the best known offset.  default False
         :param save_data: if True, save the data of the sensor to disk, otherwise use a temporary dir.  default False
         :param arrow_dir: directory to save pyarrow table, default "" (current dir).  default temporary dir if not
                             saving data
         :param use_temp_dir: If True, use a temporary directory to save the data.  default False
         :return: SensorData object
         """
-        return SensorData(sensor_name, pa.Table.from_pydict(sensor_data), sensor_type, sample_rate_hz,
-                          sample_interval_s, sample_interval_std_s, is_sample_rate_fixed, are_timestamps_altered,
-                          calculate_stats, use_offset_model_for_correction, save_data, arrow_dir,
-                          use_temp_dir=use_temp_dir)
+        return SensorData(
+            sensor_name,
+            pa.Table.from_pydict(sensor_data),
+            sensor_type,
+            sample_rate_hz,
+            sample_interval_s,
+            sample_interval_std_s,
+            is_sample_rate_fixed,
+            are_timestamps_altered,
+            calculate_stats,
+            use_offset_model_for_correction,
+            save_data,
+            arrow_dir,
+            use_temp_dir=use_temp_dir,
+        )
 
     def save(self, file_name: Optional[str] = None) -> Optional[Path]:
         """
         Saves the sensor to disk.  Does nothing if saving is not enabled
 
         :param file_name: Optional file name to save as.  Do not include a file extension.  Default None
                             If None, a default file name is created using this format:
@@ -371,15 +387,15 @@
         return None
 
     def load(self, in_dir: str) -> "SensorData":
         """
         :param in_dir: structured directory with json metadata file to load
         :return: SensorData using data from files
         """
-        file = io.get_json_file(in_dir)
+        file = get_json_file(in_dir)
         if file is None:
             st = SensorData("LoadError")
             st.append_error("File to load Sensor not found.")
             return self
         else:
             return self.from_json_file(in_dir, file)
 
@@ -612,25 +628,17 @@
         :param ptable: pyarrow table to update
         :return: updated version of self
         """
         self.sort_by_data_timestamps(ptable)
         if not self._is_sample_rate_fixed:
             if self.num_samples() > 1:
                 timestamp_diffs = np.diff(self.data_timestamps())
-                self._sample_interval_s = dtu.microseconds_to_seconds(
-                    float(np.mean(timestamp_diffs))
-                )
-                self._sample_interval_std_s = dtu.microseconds_to_seconds(
-                    float(np.std(timestamp_diffs))
-                )
-                self._sample_rate_hz = (
-                    np.nan
-                    if self.is_sample_interval_invalid()
-                    else 1 / self._sample_interval_s
-                )
+                self._sample_interval_s = dtu.microseconds_to_seconds(float(np.mean(timestamp_diffs)))
+                self._sample_interval_std_s = dtu.microseconds_to_seconds(float(np.std(timestamp_diffs)))
+                self._sample_rate_hz = np.nan if self.is_sample_interval_invalid() else 1 / self._sample_interval_s
             else:
                 self._sample_interval_s = np.nan
                 self._sample_interval_std_s = np.nan
                 self._sample_rate_hz = np.nan
         return self
 
     def append_sensor(self, new_sensor: "SensorData", recalculate_stats: bool = False) -> "SensorData":
@@ -646,29 +654,30 @@
         _arrow: pa.Table = pa.concat_tables([self.pyarrow_table(), new_sensor.pyarrow_table()])
         if recalculate_stats and not self._is_sample_rate_fixed:
             self.organize_and_update_stats(_arrow)
         else:
             self.write_pyarrow_table(_arrow)
         return self
 
-    def append_data(
-            self, new_data: List[np.array], recalculate_stats: bool = False
-    ) -> "SensorData":
+    def append_data(self, new_data: List[np.array], recalculate_stats: bool = False) -> "SensorData":
         """
         append the new data to the dataframe, update the sensor's stats on demand if it doesn't have a fixed
             sample rate, then return the updated object
 
         :param new_data: list of arrays containing data to add to the sensor's dataframe
         :param recalculate_stats: if True and the sensor does not have a fixed sample rate, sort the timestamps,
                                     recalculate the sample rate, interval, and interval std dev, default False
         :return: the updated object
         """
-        _arrow = pa.concat_tables([self.pyarrow_table(),
-                                   pa.Table.from_arrays(arrays=[pa.array(s) for s in new_data],
-                                                        names=self.data_channels())])
+        _arrow = pa.concat_tables(
+            [
+                self.pyarrow_table(),
+                pa.Table.from_arrays(arrays=[pa.array(s) for s in new_data], names=self.data_channels()),
+            ]
+        )
         if recalculate_stats and not self._is_sample_rate_fixed:
             self.organize_and_update_stats(_arrow)
         else:
             self.write_pyarrow_table(_arrow)
         return self
 
     def is_sample_interval_invalid(self) -> bool:
@@ -801,30 +810,33 @@
 
     def update_data_timestamps(self, offset_model: om.OffsetModel):
         """
         updates the timestamps of the data points
 
         :param offset_model: model used to update the timestamps
         """
-        slope = dtu.seconds_to_microseconds(self._sample_interval_s) * (1 + offset_model.slope) \
-            if self._use_offset_model else dtu.seconds_to_microseconds(self._sample_interval_s)
+        slope = (
+            dtu.seconds_to_microseconds(self._sample_interval_s) * (1 + offset_model.slope)
+            if self._use_offset_model
+            else dtu.seconds_to_microseconds(self._sample_interval_s)
+        )
         if self._type == SensorType.AUDIO:
             # use the model to update the first timestamp or add the best offset (model's intercept value)
             timestamps = pa.array(
                 calc_evenly_sampled_timestamps(
                     offset_model.update_time(self.unaltered_data_timestamps()[0], self._use_offset_model),
                     self.num_samples(),
-                    slope))
+                    slope,
+                )
+            )
         else:
-            timestamps = pa.array(offset_model.update_timestamps(self.unaltered_data_timestamps(),
-                                                                 self._use_offset_model))
-        # old_name = self.full_path()
+            timestamps = pa.array(
+                offset_model.update_timestamps(self.unaltered_data_timestamps(), self._use_offset_model)
+            )
         self.write_pyarrow_table(self.pyarrow_table().set_column(0, "timestamps", timestamps))
-        # self.set_file_name()
-        # os.rename(old_name, self.full_path())
         time_diffs = np.floor(np.diff(self.data_timestamps()))
         if len(time_diffs) > 1:
             self._sample_interval_s = dtu.microseconds_to_seconds(slope)
             if self._sample_interval_s > 0:
                 self._sample_rate_hz = 1 / self._sample_interval_s
                 self._sample_interval_std_s = dtu.microseconds_to_seconds(float(np.std(time_diffs)))
         self._timestamps_altered = True
@@ -833,16 +845,17 @@
         """
         converts all timestamps in the sensor to the original values from the data
         """
         timestamps = self.unaltered_data_timestamps()
         self.write_pyarrow_table(self.pyarrow_table().set_column(0, "timestamps", timestamps))
         self._timestamps_altered = False
 
-    def interpolate(self, interpolate_timestamp: float, first_point: int, second_point: int = 0,
-                    copy: bool = True) -> pa.Table:
+    def interpolate(
+        self, interpolate_timestamp: float, first_point: int, second_point: int = 0, copy: bool = True
+    ) -> pa.Table:
         """
         interpolates two points at the chosen timestamp.  If copy is true, copies the values of the closest point,
         otherwise interpolates any numerical value.  Non-numeric values are set to a copy of the closest point.
 
         :param interpolate_timestamp: timestamp to interpolate other values
         :param first_point: index of first point
         :param second_point: delta to second point, default 0 (same as first point)
@@ -850,24 +863,24 @@
                         Default True
         :return: pyarrow Table of interpolated points
         """
         start_point = self.pyarrow_table().slice(first_point, 1).to_pydict()
         if not copy and second_point:
             i_p = {}
             end_point = self.pyarrow_table().slice(first_point + second_point, 1).to_pydict()
-            first_closer = \
-                np.abs(start_point[0] - interpolate_timestamp) \
-                <= np.abs(end_point[0] - interpolate_timestamp)
+            first_closer = np.abs(start_point[0] - interpolate_timestamp) <= np.abs(
+                end_point[0] - interpolate_timestamp
+            )
             for col in self.pyarrow_table().schema.names:
                 # process each column independently into new table object
                 if col not in NON_INTERPOLATED_COLUMNS + NON_NUMERIC_COLUMNS:
                     numeric_diff = end_point[col] - start_point[col]
-                    numeric_diff = \
-                        (numeric_diff / numeric_diff["timestamps"]) * \
-                        (interpolate_timestamp - start_point[col]) + start_point[col]
+                    numeric_diff = (numeric_diff / numeric_diff["timestamps"]) * (
+                        interpolate_timestamp - start_point[col]
+                    ) + start_point[col]
                     i_p[col] = numeric_diff
                 elif col in NON_NUMERIC_COLUMNS:
                     if first_closer:
                         i_p[col] = start_point[col]
                     else:
                         i_p[col] = end_point[col]
         else:
@@ -887,15 +900,15 @@
             "sample_interval_s": self._sample_interval_s,
             "sample_interval_std_s": self._sample_interval_std_s,
             "is_sample_rate_fixed": self._is_sample_rate_fixed,
             "timestamps_altered": self._timestamps_altered,
             "use_offset_model": self._use_offset_model,
             "gaps": self._gaps,
             "base_dir": os.path.basename(self._fs_writer.save_dir()),
-            "errors": self._errors.as_dict()
+            "errors": self._errors.as_dict(),
         }
 
     def to_json(self) -> str:
         """
         :return: sensor as json string
         """
         return io.to_json(self)
@@ -918,25 +931,33 @@
         convert contents of json file to Sensor
 
         :param file_dir: full path to containing directory for the file
         :param file_name: optional name of file and extension to load data from; if not specified, finds the first one
         :return: SensorData object
         """
         if file_name is None:
-            file_name = io.get_json_file(file_dir)
+            file_name = get_json_file(file_dir)
             if file_name is None:
                 result = SensorData("Empty")
                 result.append_error("JSON file to load Sensor from not found.")
                 return result
-        json_data = io.json_file_to_dict(os.path.join(file_dir, file_name))
+        json_data = json_file_to_dict(os.path.join(file_dir, file_name))
         if "name" in json_data.keys():
-            result = SensorData.from_dir(json_data["name"], file_dir, SensorType[json_data["type"]],
-                                         json_data["sample_rate_hz"], json_data["sample_interval_s"],
-                                         json_data["sample_interval_std_s"], json_data["is_sample_rate_fixed"],
-                                         json_data["timestamps_altered"], False, json_data["use_offset_model"])
+            result = SensorData.from_dir(
+                json_data["name"],
+                file_dir,
+                SensorType[json_data["type"]],
+                json_data["sample_rate_hz"],
+                json_data["sample_interval_s"],
+                json_data["sample_interval_std_s"],
+                json_data["is_sample_rate_fixed"],
+                json_data["timestamps_altered"],
+                False,
+                json_data["use_offset_model"],
+            )
             result.set_errors(RedVoxExceptions.from_dict(json_data["errors"]))
             result.set_save_to_disk(True)
             result.set_file_name()
             result.set_gaps(json_data["gaps"])
         else:
             result = SensorData("Empty")
             result.append_error(f"Loading from {file_name} failed; missing Sensor name.")
@@ -966,15 +987,15 @@
                 SensorType.GYROSCOPE: GyroscopeSensor,
                 SensorType.MAGNETOMETER: MagnetometerSensor,
                 SensorType.ORIENTATION: OrientationSensor,
                 SensorType.GRAVITY: GravitySensor,
                 SensorType.LINEAR_ACCELERATION: LinearAccelerationSensor,
                 SensorType.ROTATION_VECTOR: RotationVectorSensor,
                 SensorType.VELOCITY: VelocitySensor,
-                SensorType.UNKNOWN_SENSOR: SensorData
+                SensorType.UNKNOWN_SENSOR: SensorData,
             }
             self.__class__ = sensor_class_from_type[self._type]
         return self
 
     def set_errors(self, errors: RedVoxExceptions):
         """
         sets the errors of the Sensor
@@ -1000,45 +1021,65 @@
         self._gaps = gaps
 
 
 class AudioSensor(SensorData):
     """
     Audio specific functions
     """
-    def __init__(self, sensor_name: str,
-                 sensor_data: Optional[pa.Table] = None,
-                 sample_rate_hz: float = np.nan,
-                 sample_interval_s: float = np.nan,
-                 sample_interval_std_s: float = np.nan,
-                 is_sample_rate_fixed: bool = False,
-                 are_timestamps_altered: bool = False,
-                 calculate_stats: bool = False,
-                 use_offset_model_for_correction: bool = False,
-                 save_data: bool = False,
-                 base_dir: str = ".",
-                 gaps: Optional[List[Tuple[float, float]]] = None,
-                 show_errors: bool = False,
-                 use_temp_dir: bool = False):
-        super().__init__(sensor_name, sensor_data, SensorType.AUDIO, sample_rate_hz, sample_interval_s,
-                         sample_interval_std_s, is_sample_rate_fixed, are_timestamps_altered, calculate_stats,
-                         use_offset_model_for_correction, save_data, base_dir, gaps, show_errors, use_temp_dir)
+
+    def __init__(
+        self,
+        sensor_name: str,
+        sensor_data: Optional[pa.Table] = None,
+        sample_rate_hz: float = np.nan,
+        sample_interval_s: float = np.nan,
+        sample_interval_std_s: float = np.nan,
+        is_sample_rate_fixed: bool = False,
+        are_timestamps_altered: bool = False,
+        calculate_stats: bool = False,
+        use_offset_model_for_correction: bool = False,
+        save_data: bool = False,
+        base_dir: str = ".",
+        gaps: Optional[List[Tuple[float, float]]] = None,
+        show_errors: bool = False,
+        use_temp_dir: bool = False,
+    ):
+        super().__init__(
+            sensor_name,
+            sensor_data,
+            SensorType.AUDIO,
+            sample_rate_hz,
+            sample_interval_s,
+            sample_interval_std_s,
+            is_sample_rate_fixed,
+            are_timestamps_altered,
+            calculate_stats,
+            use_offset_model_for_correction,
+            save_data,
+            base_dir,
+            gaps,
+            show_errors,
+            use_temp_dir,
+        )
 
     @staticmethod
-    def from_metadata(sensor_name: str,
-                      data: AudioWithGaps,
-                      sample_rate_hz: float = np.nan,
-                      sample_interval_s: float = np.nan,
-                      sample_interval_std_s: float = np.nan,
-                      is_sample_rate_fixed: bool = False,
-                      are_timestamps_altered: bool = False,
-                      calculate_stats: bool = False,
-                      use_offset_model_for_correction: bool = False,
-                      save_data: bool = False,
-                      base_dir: str = ".",
-                      use_temp_dir: bool = False) -> "SensorData":
+    def from_metadata(
+        sensor_name: str,
+        data: AudioWithGaps,
+        sample_rate_hz: float = np.nan,
+        sample_interval_s: float = np.nan,
+        sample_interval_std_s: float = np.nan,
+        is_sample_rate_fixed: bool = False,
+        are_timestamps_altered: bool = False,
+        calculate_stats: bool = False,
+        use_offset_model_for_correction: bool = False,
+        save_data: bool = False,
+        base_dir: str = ".",
+        use_temp_dir: bool = False,
+    ) -> "SensorData":
         """
         init but using metadata
 
         :param sensor_name: name of the sensor
         :param data: the metadata used to create the sensor
         :param sample_rate_hz: sample rate in hz of the data, default np.nan
         :param sample_interval_s: sample interval in seconds of the data, default np.nan
@@ -1052,1253 +1093,1570 @@
                                                 use the best known offset.  default False
         :param save_data: if True, save the data of the sensor to disk, otherwise use a temporary dir.  default False
         :param base_dir: directory to save pyarrow table, default "." (current dir).  internally uses a temporary
                             dir if not saving data
         :param use_temp_dir: if True, save the data using a temporary directory.  default False
         :return: SensorData object
         """
-        return SensorData(sensor_name, data.create_timestamps(),
-                          SensorType.AUDIO, sample_rate_hz, sample_interval_s, sample_interval_std_s,
-                          is_sample_rate_fixed, are_timestamps_altered, calculate_stats,
-                          use_offset_model_for_correction, save_data, base_dir, use_temp_dir=use_temp_dir)
+        return SensorData(
+            sensor_name,
+            data.create_timestamps(),
+            SensorType.AUDIO,
+            sample_rate_hz,
+            sample_interval_s,
+            sample_interval_std_s,
+            is_sample_rate_fixed,
+            are_timestamps_altered,
+            calculate_stats,
+            use_offset_model_for_correction,
+            save_data,
+            base_dir,
+            use_temp_dir=use_temp_dir,
+        )
 
     def get_microphone_data(self) -> np.array:
         """
         :return: audio data as numpy array
         """
-        return super().get_data_channel('microphone')
+        return super().get_data_channel("microphone")
 
     def get_valid_microphone_data(self) -> np.array:
         """
         :return: non-nan audio data as numpy array
         """
-        return super().get_valid_data_channel_values('microphone')
+        return super().get_valid_data_channel_values("microphone")
 
 
 class CompressedAudioSensor(SensorData):
     """
     Compressed audio specific functions
     """
-    def __init__(self, sensor_name: str,
-                 sensor_data: Optional[pa.Table] = None,
-                 sample_rate_hz: float = np.nan,
-                 sample_interval_s: float = np.nan,
-                 sample_interval_std_s: float = np.nan,
-                 is_sample_rate_fixed: bool = False,
-                 are_timestamps_altered: bool = False,
-                 calculate_stats: bool = False,
-                 use_offset_model_for_correction: bool = False,
-                 save_data: bool = False,
-                 base_dir: str = ".",
-                 gaps: Optional[List[Tuple[float, float]]] = None,
-                 show_errors: bool = False):
-        super().__init__(sensor_name, sensor_data, SensorType.COMPRESSED_AUDIO, sample_rate_hz, sample_interval_s,
-                         sample_interval_std_s, is_sample_rate_fixed, are_timestamps_altered, calculate_stats,
-                         use_offset_model_for_correction, save_data, base_dir, gaps, show_errors)
+
+    def __init__(
+        self,
+        sensor_name: str,
+        sensor_data: Optional[pa.Table] = None,
+        sample_rate_hz: float = np.nan,
+        sample_interval_s: float = np.nan,
+        sample_interval_std_s: float = np.nan,
+        is_sample_rate_fixed: bool = False,
+        are_timestamps_altered: bool = False,
+        calculate_stats: bool = False,
+        use_offset_model_for_correction: bool = False,
+        save_data: bool = False,
+        base_dir: str = ".",
+        gaps: Optional[List[Tuple[float, float]]] = None,
+        show_errors: bool = False,
+    ):
+        super().__init__(
+            sensor_name,
+            sensor_data,
+            SensorType.COMPRESSED_AUDIO,
+            sample_rate_hz,
+            sample_interval_s,
+            sample_interval_std_s,
+            is_sample_rate_fixed,
+            are_timestamps_altered,
+            calculate_stats,
+            use_offset_model_for_correction,
+            save_data,
+            base_dir,
+            gaps,
+            show_errors,
+        )
 
     def get_compressed_audio_data(self) -> np.array:
         """
         :return: compressed audio data as numpy array
         """
-        return super().get_data_channel('compressed_audio')
+        return super().get_data_channel("compressed_audio")
 
     def get_valid_compressed_audio_data(self) -> np.array:
         """
         :return: non-nan compressed audio data as numpy array
         """
-        return super().get_valid_data_channel_values('compressed_audio')
+        return super().get_valid_data_channel_values("compressed_audio")
 
     def get_audio_codec_data(self) -> List[str]:
         """
         :return: audio codec as list of strings
         """
-        return super()._get_non_numeric_data_channel('audio_codec')
+        return super()._get_non_numeric_data_channel("audio_codec")
 
     def _get_valid_audio_codec_data(self) -> List[str]:
         """
         NOT IMPLEMENTED
         :return: non-nan audio codec as list of strings
         """
         pass
         # return super().get_valid_data_channel_values('audio_codec')
 
 
 class ImageSensor(SensorData):
     """
     Image specific functions
     """
-    def __init__(self, sensor_name: str,
-                 sensor_data: Optional[pa.Table] = None,
-                 sample_rate_hz: float = np.nan,
-                 sample_interval_s: float = np.nan,
-                 sample_interval_std_s: float = np.nan,
-                 is_sample_rate_fixed: bool = False,
-                 are_timestamps_altered: bool = False,
-                 calculate_stats: bool = False,
-                 use_offset_model_for_correction: bool = False,
-                 save_data: bool = False,
-                 base_dir: str = ".",
-                 gaps: Optional[List[Tuple[float, float]]] = None,
-                 show_errors: bool = False):
-        super().__init__(sensor_name, sensor_data, SensorType.IMAGE, sample_rate_hz, sample_interval_s,
-                         sample_interval_std_s, is_sample_rate_fixed, are_timestamps_altered, calculate_stats,
-                         use_offset_model_for_correction, save_data, base_dir, gaps, show_errors)
+
+    def __init__(
+        self,
+        sensor_name: str,
+        sensor_data: Optional[pa.Table] = None,
+        sample_rate_hz: float = np.nan,
+        sample_interval_s: float = np.nan,
+        sample_interval_std_s: float = np.nan,
+        is_sample_rate_fixed: bool = False,
+        are_timestamps_altered: bool = False,
+        calculate_stats: bool = False,
+        use_offset_model_for_correction: bool = False,
+        save_data: bool = False,
+        base_dir: str = ".",
+        gaps: Optional[List[Tuple[float, float]]] = None,
+        show_errors: bool = False,
+    ):
+        super().__init__(
+            sensor_name,
+            sensor_data,
+            SensorType.IMAGE,
+            sample_rate_hz,
+            sample_interval_s,
+            sample_interval_std_s,
+            is_sample_rate_fixed,
+            are_timestamps_altered,
+            calculate_stats,
+            use_offset_model_for_correction,
+            save_data,
+            base_dir,
+            gaps,
+            show_errors,
+        )
 
     def get_image_data(self) -> np.array:
         """
         :return: image data as numpy array
         """
-        return super().get_data_channel('image')
+        return super().get_data_channel("image")
 
     def get_valid_image_data(self) -> np.array:
         """
         :return: non-nan image data as numpy array
         """
-        return super().get_valid_data_channel_values('image')
+        return super().get_valid_data_channel_values("image")
 
     def get_image_codec_data(self) -> List[str]:
         """
         :return: image codec as list of strings
         """
-        return super()._get_non_numeric_data_channel('image_codec')
+        return super()._get_non_numeric_data_channel("image_codec")
 
     def get_valid_image_codec_data(self) -> List[str]:
         """
         NOT IMPLEMENTED
         :return: non-nan image codec as list of strings
         """
         pass
         # return super().get_valid_data_channel_values('image_codec')
 
 
 class PressureSensor(SensorData):
     """
     Pressure specific functions
     """
-    def __init__(self, sensor_name: str,
-                 sensor_data: Optional[pa.Table] = None,
-                 sample_rate_hz: float = np.nan,
-                 sample_interval_s: float = np.nan,
-                 sample_interval_std_s: float = np.nan,
-                 is_sample_rate_fixed: bool = False,
-                 are_timestamps_altered: bool = False,
-                 calculate_stats: bool = False,
-                 use_offset_model_for_correction: bool = False,
-                 save_data: bool = False,
-                 base_dir: str = ".",
-                 gaps: Optional[List[Tuple[float, float]]] = None,
-                 show_errors: bool = False):
-        super().__init__(sensor_name, sensor_data, SensorType.PRESSURE, sample_rate_hz, sample_interval_s,
-                         sample_interval_std_s, is_sample_rate_fixed, are_timestamps_altered, calculate_stats,
-                         use_offset_model_for_correction, save_data, base_dir, gaps, show_errors)
+
+    def __init__(
+        self,
+        sensor_name: str,
+        sensor_data: Optional[pa.Table] = None,
+        sample_rate_hz: float = np.nan,
+        sample_interval_s: float = np.nan,
+        sample_interval_std_s: float = np.nan,
+        is_sample_rate_fixed: bool = False,
+        are_timestamps_altered: bool = False,
+        calculate_stats: bool = False,
+        use_offset_model_for_correction: bool = False,
+        save_data: bool = False,
+        base_dir: str = ".",
+        gaps: Optional[List[Tuple[float, float]]] = None,
+        show_errors: bool = False,
+    ):
+        super().__init__(
+            sensor_name,
+            sensor_data,
+            SensorType.PRESSURE,
+            sample_rate_hz,
+            sample_interval_s,
+            sample_interval_std_s,
+            is_sample_rate_fixed,
+            are_timestamps_altered,
+            calculate_stats,
+            use_offset_model_for_correction,
+            save_data,
+            base_dir,
+            gaps,
+            show_errors,
+        )
 
     def get_pressure_data(self) -> np.array:
         """
         :return: pressure data as numpy array
         """
-        return super().get_data_channel('pressure')
+        return super().get_data_channel("pressure")
 
     def get_valid_pressure_data(self) -> np.array:
         """
         :return: non-nan pressure data as numpy array
         """
-        return super().get_valid_data_channel_values('pressure')
+        return super().get_valid_data_channel_values("pressure")
 
 
 class LightSensor(SensorData):
     """
     Light specific functions
     """
-    def __init__(self, sensor_name: str,
-                 sensor_data: Optional[pa.Table] = None,
-                 sample_rate_hz: float = np.nan,
-                 sample_interval_s: float = np.nan,
-                 sample_interval_std_s: float = np.nan,
-                 is_sample_rate_fixed: bool = False,
-                 are_timestamps_altered: bool = False,
-                 calculate_stats: bool = False,
-                 use_offset_model_for_correction: bool = False,
-                 save_data: bool = False,
-                 base_dir: str = ".",
-                 gaps: Optional[List[Tuple[float, float]]] = None,
-                 show_errors: bool = False):
-        super().__init__(sensor_name, sensor_data, SensorType.LIGHT, sample_rate_hz, sample_interval_s,
-                         sample_interval_std_s, is_sample_rate_fixed, are_timestamps_altered, calculate_stats,
-                         use_offset_model_for_correction, save_data, base_dir, gaps, show_errors)
+
+    def __init__(
+        self,
+        sensor_name: str,
+        sensor_data: Optional[pa.Table] = None,
+        sample_rate_hz: float = np.nan,
+        sample_interval_s: float = np.nan,
+        sample_interval_std_s: float = np.nan,
+        is_sample_rate_fixed: bool = False,
+        are_timestamps_altered: bool = False,
+        calculate_stats: bool = False,
+        use_offset_model_for_correction: bool = False,
+        save_data: bool = False,
+        base_dir: str = ".",
+        gaps: Optional[List[Tuple[float, float]]] = None,
+        show_errors: bool = False,
+    ):
+        super().__init__(
+            sensor_name,
+            sensor_data,
+            SensorType.LIGHT,
+            sample_rate_hz,
+            sample_interval_s,
+            sample_interval_std_s,
+            is_sample_rate_fixed,
+            are_timestamps_altered,
+            calculate_stats,
+            use_offset_model_for_correction,
+            save_data,
+            base_dir,
+            gaps,
+            show_errors,
+        )
 
     def get_light_data(self) -> np.array:
         """
         :return: light data as numpy array
         """
-        return super().get_data_channel('light')
+        return super().get_data_channel("light")
 
     def get_valid_light_data(self) -> np.array:
         """
         :return: non-nan light data as numpy array
         """
-        return super().get_valid_data_channel_values('light')
+        return super().get_valid_data_channel_values("light")
 
 
 class ProximitySensor(SensorData):
     """
     Proximity specific functions
     """
-    def __init__(self, sensor_name: str,
-                 sensor_data: Optional[pa.Table] = None,
-                 sample_rate_hz: float = np.nan,
-                 sample_interval_s: float = np.nan,
-                 sample_interval_std_s: float = np.nan,
-                 is_sample_rate_fixed: bool = False,
-                 are_timestamps_altered: bool = False,
-                 calculate_stats: bool = False,
-                 use_offset_model_for_correction: bool = False,
-                 save_data: bool = False,
-                 base_dir: str = ".",
-                 gaps: Optional[List[Tuple[float, float]]] = None,
-                 show_errors: bool = False):
-        super().__init__(sensor_name, sensor_data, SensorType.PROXIMITY, sample_rate_hz, sample_interval_s,
-                         sample_interval_std_s, is_sample_rate_fixed, are_timestamps_altered, calculate_stats,
-                         use_offset_model_for_correction, save_data, base_dir, gaps, show_errors)
+
+    def __init__(
+        self,
+        sensor_name: str,
+        sensor_data: Optional[pa.Table] = None,
+        sample_rate_hz: float = np.nan,
+        sample_interval_s: float = np.nan,
+        sample_interval_std_s: float = np.nan,
+        is_sample_rate_fixed: bool = False,
+        are_timestamps_altered: bool = False,
+        calculate_stats: bool = False,
+        use_offset_model_for_correction: bool = False,
+        save_data: bool = False,
+        base_dir: str = ".",
+        gaps: Optional[List[Tuple[float, float]]] = None,
+        show_errors: bool = False,
+    ):
+        super().__init__(
+            sensor_name,
+            sensor_data,
+            SensorType.PROXIMITY,
+            sample_rate_hz,
+            sample_interval_s,
+            sample_interval_std_s,
+            is_sample_rate_fixed,
+            are_timestamps_altered,
+            calculate_stats,
+            use_offset_model_for_correction,
+            save_data,
+            base_dir,
+            gaps,
+            show_errors,
+        )
 
     def get_proximity_data(self) -> np.array:
         """
         :return: proximity data as numpy array
         """
-        return super().get_data_channel('proximity')
+        return super().get_data_channel("proximity")
 
     def get_valid_proximity_data(self) -> np.array:
         """
         :return: non-nan proximity data as numpy array
         """
-        return super().get_valid_data_channel_values('proximity')
+        return super().get_valid_data_channel_values("proximity")
 
 
 class AmbientTemperatureSensor(SensorData):
     """
     Ambient temperature specific functions
     """
-    def __init__(self, sensor_name: str,
-                 sensor_data: Optional[pa.Table] = None,
-                 sample_rate_hz: float = np.nan,
-                 sample_interval_s: float = np.nan,
-                 sample_interval_std_s: float = np.nan,
-                 is_sample_rate_fixed: bool = False,
-                 are_timestamps_altered: bool = False,
-                 calculate_stats: bool = False,
-                 use_offset_model_for_correction: bool = False,
-                 save_data: bool = False,
-                 base_dir: str = ".",
-                 gaps: Optional[List[Tuple[float, float]]] = None,
-                 show_errors: bool = False):
-        super().__init__(sensor_name, sensor_data, SensorType.AMBIENT_TEMPERATURE, sample_rate_hz, sample_interval_s,
-                         sample_interval_std_s, is_sample_rate_fixed, are_timestamps_altered, calculate_stats,
-                         use_offset_model_for_correction, save_data, base_dir, gaps, show_errors)
+
+    def __init__(
+        self,
+        sensor_name: str,
+        sensor_data: Optional[pa.Table] = None,
+        sample_rate_hz: float = np.nan,
+        sample_interval_s: float = np.nan,
+        sample_interval_std_s: float = np.nan,
+        is_sample_rate_fixed: bool = False,
+        are_timestamps_altered: bool = False,
+        calculate_stats: bool = False,
+        use_offset_model_for_correction: bool = False,
+        save_data: bool = False,
+        base_dir: str = ".",
+        gaps: Optional[List[Tuple[float, float]]] = None,
+        show_errors: bool = False,
+    ):
+        super().__init__(
+            sensor_name,
+            sensor_data,
+            SensorType.AMBIENT_TEMPERATURE,
+            sample_rate_hz,
+            sample_interval_s,
+            sample_interval_std_s,
+            is_sample_rate_fixed,
+            are_timestamps_altered,
+            calculate_stats,
+            use_offset_model_for_correction,
+            save_data,
+            base_dir,
+            gaps,
+            show_errors,
+        )
 
     def get_ambient_temperature_data(self) -> np.array:
         """
         :return: ambient temperature data as numpy array
         """
-        return super().get_data_channel('ambient_temperature')
+        return super().get_data_channel("ambient_temperature")
 
     def get_valid_ambient_temperature_data(self) -> np.array:
         """
         :return: non-nan ambient temperature data as numpy array
         """
-        return super().get_valid_data_channel_values('ambient_temperature')
+        return super().get_valid_data_channel_values("ambient_temperature")
 
 
 class RelativeHumiditySensor(SensorData):
     """
     Relative humidity specific functions
     """
-    def __init__(self, sensor_name: str,
-                 sensor_data: Optional[pa.Table] = None,
-                 sample_rate_hz: float = np.nan,
-                 sample_interval_s: float = np.nan,
-                 sample_interval_std_s: float = np.nan,
-                 is_sample_rate_fixed: bool = False,
-                 are_timestamps_altered: bool = False,
-                 calculate_stats: bool = False,
-                 use_offset_model_for_correction: bool = False,
-                 save_data: bool = False,
-                 base_dir: str = ".",
-                 gaps: Optional[List[Tuple[float, float]]] = None,
-                 show_errors: bool = False):
-        super().__init__(sensor_name, sensor_data, SensorType.RELATIVE_HUMIDITY, sample_rate_hz, sample_interval_s,
-                         sample_interval_std_s, is_sample_rate_fixed, are_timestamps_altered, calculate_stats,
-                         use_offset_model_for_correction, save_data, base_dir, gaps, show_errors)
+
+    def __init__(
+        self,
+        sensor_name: str,
+        sensor_data: Optional[pa.Table] = None,
+        sample_rate_hz: float = np.nan,
+        sample_interval_s: float = np.nan,
+        sample_interval_std_s: float = np.nan,
+        is_sample_rate_fixed: bool = False,
+        are_timestamps_altered: bool = False,
+        calculate_stats: bool = False,
+        use_offset_model_for_correction: bool = False,
+        save_data: bool = False,
+        base_dir: str = ".",
+        gaps: Optional[List[Tuple[float, float]]] = None,
+        show_errors: bool = False,
+    ):
+        super().__init__(
+            sensor_name,
+            sensor_data,
+            SensorType.RELATIVE_HUMIDITY,
+            sample_rate_hz,
+            sample_interval_s,
+            sample_interval_std_s,
+            is_sample_rate_fixed,
+            are_timestamps_altered,
+            calculate_stats,
+            use_offset_model_for_correction,
+            save_data,
+            base_dir,
+            gaps,
+            show_errors,
+        )
 
     def get_relative_humidity_data(self) -> np.array:
         """
         :return: relative humidity data as numpy array
         """
-        return super().get_data_channel('relative_humidity')
+        return super().get_data_channel("relative_humidity")
 
     def get_valid_relative_humidity_data(self) -> np.array:
         """
         :return: non-nan relative humidity data as numpy array
         """
-        return super().get_valid_data_channel_values('relative_humidity')
+        return super().get_valid_data_channel_values("relative_humidity")
 
 
 class AccelerometerSensor(SensorData):
     """
     Accelerometer specific functions
     """
-    def __init__(self, sensor_name: str,
-                 sensor_data: Optional[pa.Table] = None,
-                 sample_rate_hz: float = np.nan,
-                 sample_interval_s: float = np.nan,
-                 sample_interval_std_s: float = np.nan,
-                 is_sample_rate_fixed: bool = False,
-                 are_timestamps_altered: bool = False,
-                 calculate_stats: bool = False,
-                 use_offset_model_for_correction: bool = False,
-                 save_data: bool = False,
-                 base_dir: str = ".",
-                 gaps: Optional[List[Tuple[float, float]]] = None,
-                 show_errors: bool = False):
-        super().__init__(sensor_name, sensor_data, SensorType.ACCELEROMETER, sample_rate_hz, sample_interval_s,
-                         sample_interval_std_s, is_sample_rate_fixed, are_timestamps_altered, calculate_stats,
-                         use_offset_model_for_correction, save_data, base_dir, gaps, show_errors)
+
+    def __init__(
+        self,
+        sensor_name: str,
+        sensor_data: Optional[pa.Table] = None,
+        sample_rate_hz: float = np.nan,
+        sample_interval_s: float = np.nan,
+        sample_interval_std_s: float = np.nan,
+        is_sample_rate_fixed: bool = False,
+        are_timestamps_altered: bool = False,
+        calculate_stats: bool = False,
+        use_offset_model_for_correction: bool = False,
+        save_data: bool = False,
+        base_dir: str = ".",
+        gaps: Optional[List[Tuple[float, float]]] = None,
+        show_errors: bool = False,
+    ):
+        super().__init__(
+            sensor_name,
+            sensor_data,
+            SensorType.ACCELEROMETER,
+            sample_rate_hz,
+            sample_interval_s,
+            sample_interval_std_s,
+            is_sample_rate_fixed,
+            are_timestamps_altered,
+            calculate_stats,
+            use_offset_model_for_correction,
+            save_data,
+            base_dir,
+            gaps,
+            show_errors,
+        )
 
     def get_accelerometer_x_data(self) -> np.array:
         """
         :return: accelerometer x channel data as numpy array
         """
-        return super().get_data_channel('accelerometer_x')
+        return super().get_data_channel("accelerometer_x")
 
     def get_valid_accelerometer_x_data(self) -> np.array:
         """
         :return: non-nan accelerometer x channel data as numpy array
         """
-        return super().get_valid_data_channel_values('accelerometer_x')
+        return super().get_valid_data_channel_values("accelerometer_x")
 
     def get_accelerometer_y_data(self) -> np.array:
         """
         :return: accelerometer y channel data as numpy array
         """
-        return super().get_data_channel('accelerometer_y')
+        return super().get_data_channel("accelerometer_y")
 
     def get_valid_accelerometer_y_data(self) -> np.array:
         """
         :return: non-nan accelerometer y channel data as numpy array
         """
-        return super().get_valid_data_channel_values('accelerometer_y')
+        return super().get_valid_data_channel_values("accelerometer_y")
 
     def get_accelerometer_z_data(self) -> np.array:
         """
         :return: accelerometer z channel data as numpy array
         """
-        return super().get_data_channel('accelerometer_z')
+        return super().get_data_channel("accelerometer_z")
 
     def get_valid_accelerometer_z_data(self) -> np.array:
         """
         :return: non-nan accelerometer z channel data as numpy array
         """
-        return super().get_valid_data_channel_values('accelerometer_z')
+        return super().get_valid_data_channel_values("accelerometer_z")
 
 
 class MagnetometerSensor(SensorData):
     """
     Magnetometer specific functions
     """
-    def __init__(self, sensor_name: str,
-                 sensor_data: Optional[pa.Table] = None,
-                 sample_rate_hz: float = np.nan,
-                 sample_interval_s: float = np.nan,
-                 sample_interval_std_s: float = np.nan,
-                 is_sample_rate_fixed: bool = False,
-                 are_timestamps_altered: bool = False,
-                 calculate_stats: bool = False,
-                 use_offset_model_for_correction: bool = False,
-                 save_data: bool = False,
-                 base_dir: str = ".",
-                 gaps: Optional[List[Tuple[float, float]]] = None,
-                 show_errors: bool = False):
-        super().__init__(sensor_name, sensor_data, SensorType.MAGNETOMETER, sample_rate_hz, sample_interval_s,
-                         sample_interval_std_s, is_sample_rate_fixed, are_timestamps_altered, calculate_stats,
-                         use_offset_model_for_correction, save_data, base_dir, gaps, show_errors)
+
+    def __init__(
+        self,
+        sensor_name: str,
+        sensor_data: Optional[pa.Table] = None,
+        sample_rate_hz: float = np.nan,
+        sample_interval_s: float = np.nan,
+        sample_interval_std_s: float = np.nan,
+        is_sample_rate_fixed: bool = False,
+        are_timestamps_altered: bool = False,
+        calculate_stats: bool = False,
+        use_offset_model_for_correction: bool = False,
+        save_data: bool = False,
+        base_dir: str = ".",
+        gaps: Optional[List[Tuple[float, float]]] = None,
+        show_errors: bool = False,
+    ):
+        super().__init__(
+            sensor_name,
+            sensor_data,
+            SensorType.MAGNETOMETER,
+            sample_rate_hz,
+            sample_interval_s,
+            sample_interval_std_s,
+            is_sample_rate_fixed,
+            are_timestamps_altered,
+            calculate_stats,
+            use_offset_model_for_correction,
+            save_data,
+            base_dir,
+            gaps,
+            show_errors,
+        )
 
     def get_magnetometer_x_data(self) -> np.array:
         """
         :return: magnetometer x channel data as numpy array
         """
-        return super().get_data_channel('magnetometer_x')
+        return super().get_data_channel("magnetometer_x")
 
     def get_valid_magnetometer_x_data(self) -> np.array:
         """
         :return: non-nan magnetometer x channel data as numpy array
         """
-        return super().get_valid_data_channel_values('magnetometer_x')
+        return super().get_valid_data_channel_values("magnetometer_x")
 
     def get_magnetometer_y_data(self) -> np.array:
         """
         :return: magnetometer y channel data as numpy array
         """
-        return super().get_data_channel('magnetometer_y')
+        return super().get_data_channel("magnetometer_y")
 
     def get_valid_magnetometer_y_data(self) -> np.array:
         """
         :return: non-nan magnetometer y channel data as numpy array
         """
-        return super().get_valid_data_channel_values('magnetometer_y')
+        return super().get_valid_data_channel_values("magnetometer_y")
 
     def get_magnetometer_z_data(self) -> np.array:
         """
         :return: magnetometer z channel data as numpy array
         """
-        return super().get_data_channel('magnetometer_z')
+        return super().get_data_channel("magnetometer_z")
 
     def get_valid_magnetometer_z_data(self) -> np.array:
         """
         :return: non-nan magnetometer z channel data as numpy array
         """
-        return super().get_valid_data_channel_values('magnetometer_z')
+        return super().get_valid_data_channel_values("magnetometer_z")
 
 
 class LinearAccelerationSensor(SensorData):
     """
     Linear acceleration specific functions
     """
-    def __init__(self, sensor_name: str,
-                 sensor_data: Optional[pa.Table] = None,
-                 sample_rate_hz: float = np.nan,
-                 sample_interval_s: float = np.nan,
-                 sample_interval_std_s: float = np.nan,
-                 is_sample_rate_fixed: bool = False,
-                 are_timestamps_altered: bool = False,
-                 calculate_stats: bool = False,
-                 use_offset_model_for_correction: bool = False,
-                 save_data: bool = False,
-                 base_dir: str = ".",
-                 gaps: Optional[List[Tuple[float, float]]] = None,
-                 show_errors: bool = False):
-        super().__init__(sensor_name, sensor_data, SensorType.LINEAR_ACCELERATION, sample_rate_hz, sample_interval_s,
-                         sample_interval_std_s, is_sample_rate_fixed, are_timestamps_altered, calculate_stats,
-                         use_offset_model_for_correction, save_data, base_dir, gaps, show_errors)
+
+    def __init__(
+        self,
+        sensor_name: str,
+        sensor_data: Optional[pa.Table] = None,
+        sample_rate_hz: float = np.nan,
+        sample_interval_s: float = np.nan,
+        sample_interval_std_s: float = np.nan,
+        is_sample_rate_fixed: bool = False,
+        are_timestamps_altered: bool = False,
+        calculate_stats: bool = False,
+        use_offset_model_for_correction: bool = False,
+        save_data: bool = False,
+        base_dir: str = ".",
+        gaps: Optional[List[Tuple[float, float]]] = None,
+        show_errors: bool = False,
+    ):
+        super().__init__(
+            sensor_name,
+            sensor_data,
+            SensorType.LINEAR_ACCELERATION,
+            sample_rate_hz,
+            sample_interval_s,
+            sample_interval_std_s,
+            is_sample_rate_fixed,
+            are_timestamps_altered,
+            calculate_stats,
+            use_offset_model_for_correction,
+            save_data,
+            base_dir,
+            gaps,
+            show_errors,
+        )
 
     def get_linear_acceleration_x_data(self) -> np.array:
         """
         :return: linear acceleration x channel data as numpy array
         """
-        return super().get_data_channel('linear_acceleration_x')
+        return super().get_data_channel("linear_acceleration_x")
 
     def get_valid_linear_acceleration_x_data(self) -> np.array:
         """
         :return: non-nan linear acceleration x channel data as numpy array
         """
-        return super().get_valid_data_channel_values('linear_acceleration_x')
+        return super().get_valid_data_channel_values("linear_acceleration_x")
 
     def get_linear_acceleration_y_data(self) -> np.array:
         """
         :return: linear acceleration y channel data as numpy array
         """
-        return super().get_data_channel('linear_acceleration_y')
+        return super().get_data_channel("linear_acceleration_y")
 
     def get_valid_linear_acceleration_y_data(self) -> np.array:
         """
         :return: non-nan linear acceleration y channel data as numpy array
         """
-        return super().get_valid_data_channel_values('linear_acceleration_y')
+        return super().get_valid_data_channel_values("linear_acceleration_y")
 
     def get_linear_acceleration_z_data(self) -> np.array:
         """
         :return: linear acceleration z channel data as numpy array
         """
-        return super().get_data_channel('linear_acceleration_z')
+        return super().get_data_channel("linear_acceleration_z")
 
     def get_valid_linear_acceleration_z_data(self) -> np.array:
         """
         :return: non-nan linear acceleration z channel data as numpy array
         """
-        return super().get_valid_data_channel_values('linear_acceleration_z')
+        return super().get_valid_data_channel_values("linear_acceleration_z")
 
 
 class OrientationSensor(SensorData):
     """
     Orientation specific functions
     """
-    def __init__(self, sensor_name: str,
-                 sensor_data: Optional[pa.Table] = None,
-                 sample_rate_hz: float = np.nan,
-                 sample_interval_s: float = np.nan,
-                 sample_interval_std_s: float = np.nan,
-                 is_sample_rate_fixed: bool = False,
-                 are_timestamps_altered: bool = False,
-                 calculate_stats: bool = False,
-                 use_offset_model_for_correction: bool = False,
-                 save_data: bool = False,
-                 base_dir: str = ".",
-                 gaps: Optional[List[Tuple[float, float]]] = None,
-                 show_errors: bool = False):
-        super().__init__(sensor_name, sensor_data, SensorType.ORIENTATION, sample_rate_hz, sample_interval_s,
-                         sample_interval_std_s, is_sample_rate_fixed, are_timestamps_altered, calculate_stats,
-                         use_offset_model_for_correction, save_data, base_dir, gaps, show_errors)
+
+    def __init__(
+        self,
+        sensor_name: str,
+        sensor_data: Optional[pa.Table] = None,
+        sample_rate_hz: float = np.nan,
+        sample_interval_s: float = np.nan,
+        sample_interval_std_s: float = np.nan,
+        is_sample_rate_fixed: bool = False,
+        are_timestamps_altered: bool = False,
+        calculate_stats: bool = False,
+        use_offset_model_for_correction: bool = False,
+        save_data: bool = False,
+        base_dir: str = ".",
+        gaps: Optional[List[Tuple[float, float]]] = None,
+        show_errors: bool = False,
+    ):
+        super().__init__(
+            sensor_name,
+            sensor_data,
+            SensorType.ORIENTATION,
+            sample_rate_hz,
+            sample_interval_s,
+            sample_interval_std_s,
+            is_sample_rate_fixed,
+            are_timestamps_altered,
+            calculate_stats,
+            use_offset_model_for_correction,
+            save_data,
+            base_dir,
+            gaps,
+            show_errors,
+        )
 
     def get_orientation_x_data(self) -> np.array:
         """
         :return: orientation x channel data as numpy array
         """
-        return super().get_data_channel('orientation_x')
+        return super().get_data_channel("orientation_x")
 
     def get_valid_orientation_x_data(self) -> np.array:
         """
         :return: non-nan orientation x channel data as numpy array
         """
-        return super().get_valid_data_channel_values('orientation_x')
+        return super().get_valid_data_channel_values("orientation_x")
 
     def get_orientation_y_data(self) -> np.array:
         """
         :return: orientation y channel data as numpy array
         """
-        return super().get_data_channel('orientation_y')
+        return super().get_data_channel("orientation_y")
 
     def get_valid_orientation_y_data(self) -> np.array:
         """
         :return: non-nan orientation y channel data as numpy array
         """
-        return super().get_valid_data_channel_values('orientation_y')
+        return super().get_valid_data_channel_values("orientation_y")
 
     def get_orientation_z_data(self) -> np.array:
         """
         :return: orientation z channel data as numpy array
         """
-        return super().get_data_channel('orientation_z')
+        return super().get_data_channel("orientation_z")
 
     def get_valid_orientation_z_data(self) -> np.array:
         """
         :return: non-nan orientation z channel data as numpy array
         """
-        return super().get_valid_data_channel_values('orientation_z')
+        return super().get_valid_data_channel_values("orientation_z")
 
 
 class RotationVectorSensor(SensorData):
     """
     Rotation vector specific functions
     """
-    def __init__(self, sensor_name: str,
-                 sensor_data: Optional[pa.Table] = None,
-                 sample_rate_hz: float = np.nan,
-                 sample_interval_s: float = np.nan,
-                 sample_interval_std_s: float = np.nan,
-                 is_sample_rate_fixed: bool = False,
-                 are_timestamps_altered: bool = False,
-                 calculate_stats: bool = False,
-                 use_offset_model_for_correction: bool = False,
-                 save_data: bool = False,
-                 base_dir: str = ".",
-                 gaps: Optional[List[Tuple[float, float]]] = None,
-                 show_errors: bool = False):
-        super().__init__(sensor_name, sensor_data, SensorType.ROTATION_VECTOR, sample_rate_hz, sample_interval_s,
-                         sample_interval_std_s, is_sample_rate_fixed, are_timestamps_altered, calculate_stats,
-                         use_offset_model_for_correction, save_data, base_dir, gaps, show_errors)
+
+    def __init__(
+        self,
+        sensor_name: str,
+        sensor_data: Optional[pa.Table] = None,
+        sample_rate_hz: float = np.nan,
+        sample_interval_s: float = np.nan,
+        sample_interval_std_s: float = np.nan,
+        is_sample_rate_fixed: bool = False,
+        are_timestamps_altered: bool = False,
+        calculate_stats: bool = False,
+        use_offset_model_for_correction: bool = False,
+        save_data: bool = False,
+        base_dir: str = ".",
+        gaps: Optional[List[Tuple[float, float]]] = None,
+        show_errors: bool = False,
+    ):
+        super().__init__(
+            sensor_name,
+            sensor_data,
+            SensorType.ROTATION_VECTOR,
+            sample_rate_hz,
+            sample_interval_s,
+            sample_interval_std_s,
+            is_sample_rate_fixed,
+            are_timestamps_altered,
+            calculate_stats,
+            use_offset_model_for_correction,
+            save_data,
+            base_dir,
+            gaps,
+            show_errors,
+        )
 
     def get_rotation_vector_x_data(self) -> np.array:
         """
         :return: rotation vector x channel data as numpy array
         """
-        return super().get_data_channel('rotation_vector_x')
+        return super().get_data_channel("rotation_vector_x")
 
     def get_valid_rotation_vector_x_data(self) -> np.array:
         """
         :return: non-nan rotation vector x channel data as numpy array
         """
-        return super().get_valid_data_channel_values('rotation_vector_x')
+        return super().get_valid_data_channel_values("rotation_vector_x")
 
     def get_rotation_vector_y_data(self) -> np.array:
         """
         :return: rotation vector y channel data as numpy array
         """
-        return super().get_data_channel('rotation_vector_y')
+        return super().get_data_channel("rotation_vector_y")
 
     def get_valid_rotation_vector_y_data(self) -> np.array:
         """
         :return: non-nan rotation vector y channel data as numpy array
         """
-        return super().get_valid_data_channel_values('rotation_vector_y')
+        return super().get_valid_data_channel_values("rotation_vector_y")
 
     def get_rotation_vector_z_data(self) -> np.array:
         """
         :return: rotation vector z channel data as numpy array
         """
-        return super().get_data_channel('rotation_vector_z')
+        return super().get_data_channel("rotation_vector_z")
 
     def get_valid_rotation_vector_z_data(self) -> np.array:
         """
         :return: non-nan rotation vector z channel data as numpy array
         """
-        return super().get_valid_data_channel_values('rotation_vector_z')
+        return super().get_valid_data_channel_values("rotation_vector_z")
 
 
 class VelocitySensor(SensorData):
     """
     Rotation vector specific functions
     """
-    def __init__(self, sensor_name: str,
-                 sensor_data: Optional[pa.Table] = None,
-                 sample_rate_hz: float = np.nan,
-                 sample_interval_s: float = np.nan,
-                 sample_interval_std_s: float = np.nan,
-                 is_sample_rate_fixed: bool = False,
-                 are_timestamps_altered: bool = False,
-                 calculate_stats: bool = False,
-                 use_offset_model_for_correction: bool = False,
-                 save_data: bool = False,
-                 base_dir: str = ".",
-                 gaps: Optional[List[Tuple[float, float]]] = None,
-                 show_errors: bool = False):
-        super().__init__(sensor_name, sensor_data, SensorType.Velocity, sample_rate_hz, sample_interval_s,
-                         sample_interval_std_s, is_sample_rate_fixed, are_timestamps_altered, calculate_stats,
-                         use_offset_model_for_correction, save_data, base_dir, gaps, show_errors)
+
+    def __init__(
+        self,
+        sensor_name: str,
+        sensor_data: Optional[pa.Table] = None,
+        sample_rate_hz: float = np.nan,
+        sample_interval_s: float = np.nan,
+        sample_interval_std_s: float = np.nan,
+        is_sample_rate_fixed: bool = False,
+        are_timestamps_altered: bool = False,
+        calculate_stats: bool = False,
+        use_offset_model_for_correction: bool = False,
+        save_data: bool = False,
+        base_dir: str = ".",
+        gaps: Optional[List[Tuple[float, float]]] = None,
+        show_errors: bool = False,
+    ):
+        super().__init__(
+            sensor_name,
+            sensor_data,
+            SensorType.VELOCITY,
+            sample_rate_hz,
+            sample_interval_s,
+            sample_interval_std_s,
+            is_sample_rate_fixed,
+            are_timestamps_altered,
+            calculate_stats,
+            use_offset_model_for_correction,
+            save_data,
+            base_dir,
+            gaps,
+            show_errors,
+        )
 
     def get_velocity_x_data(self) -> np.array:
         """
         :return: velocity x channel data as numpy array
         """
-        return super().get_data_channel('velocity_x')
+        return super().get_data_channel("velocity_x")
 
     def get_valid_velocity_x_data(self) -> np.array:
         """
         :return: non-nan velocity x channel data as numpy array
         """
-        return super().get_valid_data_channel_values('velocity_x')
+        return super().get_valid_data_channel_values("velocity_x")
 
     def get_velocity_y_data(self) -> np.array:
         """
         :return: velocity y channel data as numpy array
         """
-        return super().get_data_channel('velocity_y')
+        return super().get_data_channel("velocity_y")
 
     def get_valid_velocity_y_data(self) -> np.array:
         """
         :return: non-nan velocity y channel data as numpy array
         """
-        return super().get_valid_data_channel_values('velocity_y')
+        return super().get_valid_data_channel_values("velocity_y")
 
     def get_velocity_z_data(self) -> np.array:
         """
         :return: velocity z channel data as numpy array
         """
-        return super().get_data_channel('velocity_z')
+        return super().get_data_channel("velocity_z")
 
     def get_valid_velocity_z_data(self) -> np.array:
         """
         :return: non-nan velocity z channel data as numpy array
         """
-        return super().get_valid_data_channel_values('velocity_z')
+        return super().get_valid_data_channel_values("velocity_z")
 
 
 class GyroscopeSensor(SensorData):
     """
     Gyroscope specific functions
     """
-    def __init__(self, sensor_name: str,
-                 sensor_data: Optional[pa.Table] = None,
-                 sample_rate_hz: float = np.nan,
-                 sample_interval_s: float = np.nan,
-                 sample_interval_std_s: float = np.nan,
-                 is_sample_rate_fixed: bool = False,
-                 are_timestamps_altered: bool = False,
-                 calculate_stats: bool = False,
-                 use_offset_model_for_correction: bool = False,
-                 save_data: bool = False,
-                 base_dir: str = ".",
-                 gaps: Optional[List[Tuple[float, float]]] = None,
-                 show_errors: bool = False):
-        super().__init__(sensor_name, sensor_data, SensorType.GYROSCOPE, sample_rate_hz, sample_interval_s,
-                         sample_interval_std_s, is_sample_rate_fixed, are_timestamps_altered, calculate_stats,
-                         use_offset_model_for_correction, save_data, base_dir, gaps, show_errors)
+
+    def __init__(
+        self,
+        sensor_name: str,
+        sensor_data: Optional[pa.Table] = None,
+        sample_rate_hz: float = np.nan,
+        sample_interval_s: float = np.nan,
+        sample_interval_std_s: float = np.nan,
+        is_sample_rate_fixed: bool = False,
+        are_timestamps_altered: bool = False,
+        calculate_stats: bool = False,
+        use_offset_model_for_correction: bool = False,
+        save_data: bool = False,
+        base_dir: str = ".",
+        gaps: Optional[List[Tuple[float, float]]] = None,
+        show_errors: bool = False,
+    ):
+        super().__init__(
+            sensor_name,
+            sensor_data,
+            SensorType.GYROSCOPE,
+            sample_rate_hz,
+            sample_interval_s,
+            sample_interval_std_s,
+            is_sample_rate_fixed,
+            are_timestamps_altered,
+            calculate_stats,
+            use_offset_model_for_correction,
+            save_data,
+            base_dir,
+            gaps,
+            show_errors,
+        )
 
     def get_gyroscope_x_data(self) -> np.array:
         """
         :return: gyroscope x channel data as numpy array
         """
-        return super().get_data_channel('gyroscope_x')
+        return super().get_data_channel("gyroscope_x")
 
     def get_valid_gyroscope_x_data(self) -> np.array:
         """
         :return: non-nan gyroscope x channel data as numpy array
         """
-        return super().get_valid_data_channel_values('gyroscope_x')
+        return super().get_valid_data_channel_values("gyroscope_x")
 
     def get_gyroscope_y_data(self) -> np.array:
         """
         :return: gyroscope y channel data as numpy array
         """
-        return super().get_data_channel('gyroscope_y')
+        return super().get_data_channel("gyroscope_y")
 
     def get_valid_gyroscope_y_data(self) -> np.array:
         """
         :return: non-nan gyroscope y channel data as numpy array
         """
-        return super().get_valid_data_channel_values('gyroscope_y')
+        return super().get_valid_data_channel_values("gyroscope_y")
 
     def get_gyroscope_z_data(self) -> np.array:
         """
         :return: gyroscope z channel data as numpy array
         """
-        return super().get_data_channel('gyroscope_z')
+        return super().get_data_channel("gyroscope_z")
 
     def get_valid_gyroscope_z_data(self) -> np.array:
         """
         :return: non-nan gyroscope z channel data as numpy array
         """
-        return super().get_valid_data_channel_values('gyroscope_z')
+        return super().get_valid_data_channel_values("gyroscope_z")
 
 
 class GravitySensor(SensorData):
     """
     Gravity specific functions
     """
-    def __init__(self, sensor_name: str,
-                 sensor_data: Optional[pa.Table] = None,
-                 sample_rate_hz: float = np.nan,
-                 sample_interval_s: float = np.nan,
-                 sample_interval_std_s: float = np.nan,
-                 is_sample_rate_fixed: bool = False,
-                 are_timestamps_altered: bool = False,
-                 calculate_stats: bool = False,
-                 use_offset_model_for_correction: bool = False,
-                 save_data: bool = False,
-                 base_dir: str = ".",
-                 gaps: Optional[List[Tuple[float, float]]] = None,
-                 show_errors: bool = False):
-        super().__init__(sensor_name, sensor_data, SensorType.GRAVITY, sample_rate_hz, sample_interval_s,
-                         sample_interval_std_s, is_sample_rate_fixed, are_timestamps_altered, calculate_stats,
-                         use_offset_model_for_correction, save_data, base_dir, gaps, show_errors)
+
+    def __init__(
+        self,
+        sensor_name: str,
+        sensor_data: Optional[pa.Table] = None,
+        sample_rate_hz: float = np.nan,
+        sample_interval_s: float = np.nan,
+        sample_interval_std_s: float = np.nan,
+        is_sample_rate_fixed: bool = False,
+        are_timestamps_altered: bool = False,
+        calculate_stats: bool = False,
+        use_offset_model_for_correction: bool = False,
+        save_data: bool = False,
+        base_dir: str = ".",
+        gaps: Optional[List[Tuple[float, float]]] = None,
+        show_errors: bool = False,
+    ):
+        super().__init__(
+            sensor_name,
+            sensor_data,
+            SensorType.GRAVITY,
+            sample_rate_hz,
+            sample_interval_s,
+            sample_interval_std_s,
+            is_sample_rate_fixed,
+            are_timestamps_altered,
+            calculate_stats,
+            use_offset_model_for_correction,
+            save_data,
+            base_dir,
+            gaps,
+            show_errors,
+        )
 
     def get_gravity_x_data(self) -> np.array:
         """
         :return: gravity x channel data as numpy array
         """
-        return super().get_data_channel('gravity_x')
+        return super().get_data_channel("gravity_x")
 
     def get_valid_gravity_x_data(self) -> np.array:
         """
         :return: non-nan gravity x channel data as numpy array
         """
-        return super().get_valid_data_channel_values('gravity_x')
+        return super().get_valid_data_channel_values("gravity_x")
 
     def get_gravity_y_data(self) -> np.array:
         """
         :return: gravity y channel data as numpy array
         """
-        return super().get_data_channel('gravity_y')
+        return super().get_data_channel("gravity_y")
 
     def get_valid_gravity_y_data(self) -> np.array:
         """
         :return: non-nan gravity y channel data as numpy array
         """
-        return super().get_valid_data_channel_values('gravity_y')
+        return super().get_valid_data_channel_values("gravity_y")
 
     def get_gravity_z_data(self) -> np.array:
         """
         :return: gravity z channel data as numpy array
         """
-        return super().get_data_channel('gravity_z')
+        return super().get_data_channel("gravity_z")
 
     def get_valid_gravity_z_data(self) -> np.array:
         """
         :return: non-nan gravity z channel data as numpy array
         """
-        return super().get_valid_data_channel_values('gravity_z')
+        return super().get_valid_data_channel_values("gravity_z")
 
 
 class LocationSensor(SensorData):
     """
     Location specific functions
     """
-    def __init__(self, sensor_name: str,
-                 sensor_data: Optional[pa.Table] = None,
-                 sample_rate_hz: float = np.nan,
-                 sample_interval_s: float = np.nan,
-                 sample_interval_std_s: float = np.nan,
-                 is_sample_rate_fixed: bool = False,
-                 are_timestamps_altered: bool = False,
-                 calculate_stats: bool = False,
-                 use_offset_model_for_correction: bool = False,
-                 save_data: bool = False,
-                 base_dir: str = ".",
-                 gaps: Optional[List[Tuple[float, float]]] = None,
-                 show_errors: bool = False):
-        super().__init__(sensor_name, sensor_data, SensorType.LOCATION, sample_rate_hz, sample_interval_s,
-                         sample_interval_std_s, is_sample_rate_fixed, are_timestamps_altered, calculate_stats,
-                         use_offset_model_for_correction, save_data, base_dir, gaps, show_errors)
+
+    def __init__(
+        self,
+        sensor_name: str,
+        sensor_data: Optional[pa.Table] = None,
+        sample_rate_hz: float = np.nan,
+        sample_interval_s: float = np.nan,
+        sample_interval_std_s: float = np.nan,
+        is_sample_rate_fixed: bool = False,
+        are_timestamps_altered: bool = False,
+        calculate_stats: bool = False,
+        use_offset_model_for_correction: bool = False,
+        save_data: bool = False,
+        base_dir: str = ".",
+        gaps: Optional[List[Tuple[float, float]]] = None,
+        show_errors: bool = False,
+    ):
+        super().__init__(
+            sensor_name,
+            sensor_data,
+            SensorType.LOCATION,
+            sample_rate_hz,
+            sample_interval_s,
+            sample_interval_std_s,
+            is_sample_rate_fixed,
+            are_timestamps_altered,
+            calculate_stats,
+            use_offset_model_for_correction,
+            save_data,
+            base_dir,
+            gaps,
+            show_errors,
+        )
 
     def get_gps_timestamps_data(self) -> np.array:
         """
         :return: gps timestamps as numpy array
         """
-        return super().get_data_channel('gps_timestamps')
+        return super().get_data_channel("gps_timestamps")
 
     def get_valid_gps_timestamps_data(self) -> np.array:
         """
         :return: non-nan gps timestamps as numpy array
         """
-        return super().get_valid_data_channel_values('gps_timestamps')
+        return super().get_valid_data_channel_values("gps_timestamps")
 
     def get_latitude_data(self) -> np.array:
         """
         :return: latitude data as numpy array
         """
-        return super().get_data_channel('latitude')
+        return super().get_data_channel("latitude")
 
     def get_valid_latitude_data(self) -> np.array:
         """
         :return: non-nan latitude data as numpy array
         """
-        return super().get_valid_data_channel_values('latitude')
+        return super().get_valid_data_channel_values("latitude")
 
     def get_longitude_data(self) -> np.array:
         """
         :return: longitude data as numpy array
         """
-        return super().get_data_channel('longitude')
+        return super().get_data_channel("longitude")
 
     def get_valid_longitude_data(self) -> np.array:
         """
         :return: non-nan longitude data as numpy array
         """
-        return super().get_valid_data_channel_values('longitude')
+        return super().get_valid_data_channel_values("longitude")
 
     def get_altitude_data(self) -> np.array:
         """
         :return: altitude data as numpy array
         """
-        return super().get_data_channel('altitude')
+        return super().get_data_channel("altitude")
 
     def get_valid_altitude_data(self) -> np.array:
         """
         :return: non-nan altitude data as numpy array
         """
-        return super().get_valid_data_channel_values('altitude')
+        return super().get_valid_data_channel_values("altitude")
 
     def get_speed_data(self) -> np.array:
         """
         :return: speed data as numpy array
         """
-        return super().get_data_channel('speed')
+        return super().get_data_channel("speed")
 
     def get_valid_speed_data(self) -> np.array:
         """
         :return: non-nan speed data as numpy array
         """
-        return super().get_valid_data_channel_values('speed')
+        return super().get_valid_data_channel_values("speed")
 
     def get_bearing_data(self) -> np.array:
         """
         :return: bearing data as numpy array
         """
-        return super().get_data_channel('bearing')
+        return super().get_data_channel("bearing")
 
     def get_valid_bearing_data(self) -> np.array:
         """
         :return: non-nan bearing data as numpy array
         """
-        return super().get_valid_data_channel_values('bearing')
+        return super().get_valid_data_channel_values("bearing")
 
     def get_horizontal_accuracy_data(self) -> np.array:
         """
         :return: horizontal accuracy data as numpy array
         """
-        return super().get_data_channel('horizontal_accuracy')
+        return super().get_data_channel("horizontal_accuracy")
 
     def get_valid_horizontal_accuracy_data(self) -> np.array:
         """
         :return: non-nan horizontal accuracy data as numpy array
         """
-        return super().get_valid_data_channel_values('horizontal_accuracy')
+        return super().get_valid_data_channel_values("horizontal_accuracy")
 
     def get_vertical_accuracy_data(self) -> np.array:
         """
         :return: vertical accuracy data as numpy array
         """
-        return super().get_data_channel('vertical_accuracy')
+        return super().get_data_channel("vertical_accuracy")
 
     def get_valid_vertical_accuracy_data(self) -> np.array:
         """
         :return: non-nan vertical accuracy data as numpy array
         """
-        return super().get_valid_data_channel_values('vertical_accuracy')
+        return super().get_valid_data_channel_values("vertical_accuracy")
 
     def get_speed_accuracy_data(self) -> np.array:
         """
         :return: speed accuracy data as numpy array
         """
-        return super().get_data_channel('speed_accuracy')
+        return super().get_data_channel("speed_accuracy")
 
     def get_valid_speed_accuracy_data(self) -> np.array:
         """
         :return: non-nan speed accuracy data as numpy array
         """
-        return super().get_valid_data_channel_values('speed_accuracy')
+        return super().get_valid_data_channel_values("speed_accuracy")
 
     def get_bearing_accuracy_data(self) -> np.array:
         """
         :return: bearing accuracy data as numpy array
         """
-        return super().get_data_channel('bearing_accuracy')
+        return super().get_data_channel("bearing_accuracy")
 
     def get_valid_bearing_accuracy_data(self) -> np.array:
         """
         :return: non-nan bearing accuracy data as numpy array
         """
-        return super().get_valid_data_channel_values('bearing_accuracy')
+        return super().get_valid_data_channel_values("bearing_accuracy")
 
     def get_location_provider_data(self) -> List[str]:
         """
         :return: location provider data as list of strings
         """
-        return super()._get_non_numeric_data_channel('location_provider')
+        return super()._get_non_numeric_data_channel("location_provider")
 
     def get_valid_location_provider_data(self) -> List[str]:
         """
         NOT IMPLEMENTED
         :return: non-nan location provider data as list of strings
         """
         pass
         # return super().get_valid_data_channel_values('location_provider')
 
 
 class BestLocationSensor(SensorData):
     """
     Best-location specific functions
     """
-    def __init__(self, sensor_name: str,
-                 sensor_data: Optional[pa.Table] = None,
-                 sample_rate_hz: float = np.nan,
-                 sample_interval_s: float = np.nan,
-                 sample_interval_std_s: float = np.nan,
-                 is_sample_rate_fixed: bool = False,
-                 are_timestamps_altered: bool = False,
-                 calculate_stats: bool = False,
-                 use_offset_model_for_correction: bool = False,
-                 save_data: bool = False,
-                 base_dir: str = ".",
-                 gaps: Optional[List[Tuple[float, float]]] = None,
-                 show_errors: bool = False):
-        super().__init__(sensor_name, sensor_data, SensorType.BEST_LOCATION, sample_rate_hz, sample_interval_s,
-                         sample_interval_std_s, is_sample_rate_fixed, are_timestamps_altered, calculate_stats,
-                         use_offset_model_for_correction, save_data, base_dir, gaps, show_errors)
+
+    def __init__(
+        self,
+        sensor_name: str,
+        sensor_data: Optional[pa.Table] = None,
+        sample_rate_hz: float = np.nan,
+        sample_interval_s: float = np.nan,
+        sample_interval_std_s: float = np.nan,
+        is_sample_rate_fixed: bool = False,
+        are_timestamps_altered: bool = False,
+        calculate_stats: bool = False,
+        use_offset_model_for_correction: bool = False,
+        save_data: bool = False,
+        base_dir: str = ".",
+        gaps: Optional[List[Tuple[float, float]]] = None,
+        show_errors: bool = False,
+    ):
+        super().__init__(
+            sensor_name,
+            sensor_data,
+            SensorType.BEST_LOCATION,
+            sample_rate_hz,
+            sample_interval_s,
+            sample_interval_std_s,
+            is_sample_rate_fixed,
+            are_timestamps_altered,
+            calculate_stats,
+            use_offset_model_for_correction,
+            save_data,
+            base_dir,
+            gaps,
+            show_errors,
+        )
 
     def get_gps_timestamps_data(self) -> np.array:
         """
         :return: gps timestamps as numpy array
         """
-        return super().get_data_channel('gps_timestamps')
+        return super().get_data_channel("gps_timestamps")
 
     def get_valid_gps_timestamps_data(self) -> np.array:
         """
         :return: non-nan gps timestamps as numpy array
         """
-        return super().get_valid_data_channel_values('gps_timestamps')
+        return super().get_valid_data_channel_values("gps_timestamps")
 
     def get_latitude_data(self) -> np.array:
         """
         :return: latitude data as numpy array
         """
-        return super().get_data_channel('latitude')
+        return super().get_data_channel("latitude")
 
     def get_valid_latitude_data(self) -> np.array:
         """
         :return: non-nan latitude data as numpy array
         """
-        return super().get_valid_data_channel_values('latitude')
+        return super().get_valid_data_channel_values("latitude")
 
     def get_longitude_data(self) -> np.array:
         """
         :return: longitude data as numpy array
         """
-        return super().get_data_channel('longitude')
+        return super().get_data_channel("longitude")
 
     def get_valid_longitude_data(self) -> np.array:
         """
         :return: non-nan longitude data as numpy array
         """
-        return super().get_valid_data_channel_values('longitude')
+        return super().get_valid_data_channel_values("longitude")
 
     def get_altitude_data(self) -> np.array:
         """
         :return: altitude data as numpy array
         """
-        return super().get_data_channel('altitude')
+        return super().get_data_channel("altitude")
 
     def get_valid_altitude_data(self) -> np.array:
         """
         :return: non-nan altitude data as numpy array
         """
-        return super().get_valid_data_channel_values('altitude')
+        return super().get_valid_data_channel_values("altitude")
 
     def get_speed_data(self) -> np.array:
         """
         :return: speed data as numpy array
         """
-        return super().get_data_channel('speed')
+        return super().get_data_channel("speed")
 
     def get_valid_speed_data(self) -> np.array:
         """
         :return: non-nan speed data as numpy array
         """
-        return super().get_valid_data_channel_values('speed')
+        return super().get_valid_data_channel_values("speed")
 
     def get_bearing_data(self) -> np.array:
         """
         :return: bearing data as numpy array
         """
-        return super().get_data_channel('bearing')
+        return super().get_data_channel("bearing")
 
     def get_valid_bearing_data(self) -> np.array:
         """
         :return: non-nan bearing data as numpy array
         """
-        return super().get_valid_data_channel_values('bearing')
+        return super().get_valid_data_channel_values("bearing")
 
     def get_horizontal_accuracy_data(self) -> np.array:
         """
         :return: horizontal accuracy data as numpy array
         """
-        return super().get_data_channel('horizontal_accuracy')
+        return super().get_data_channel("horizontal_accuracy")
 
     def get_valid_horizontal_accuracy_data(self) -> np.array:
         """
         :return: non-nan horizontal accuracy data as numpy array
         """
-        return super().get_valid_data_channel_values('horizontal_accuracy')
+        return super().get_valid_data_channel_values("horizontal_accuracy")
 
     def get_vertical_accuracy_data(self) -> np.array:
         """
         :return: vertical accuracy data as numpy array
         """
-        return super().get_data_channel('vertical_accuracy')
+        return super().get_data_channel("vertical_accuracy")
 
     def get_valid_vertical_accuracy_data(self) -> np.array:
         """
         :return: non-nan vertical accuracy data as numpy array
         """
-        return super().get_valid_data_channel_values('vertical_accuracy')
+        return super().get_valid_data_channel_values("vertical_accuracy")
 
     def get_speed_accuracy_data(self) -> np.array:
         """
         :return: speed accuracy data as numpy array
         """
-        return super().get_data_channel('speed_accuracy')
+        return super().get_data_channel("speed_accuracy")
 
     def get_valid_speed_accuracy_data(self) -> np.array:
         """
         :return: non-nan speed accuracy data as numpy array
         """
-        return super().get_valid_data_channel_values('speed_accuracy')
+        return super().get_valid_data_channel_values("speed_accuracy")
 
     def get_bearing_accuracy_data(self) -> np.array:
         """
         :return: bearing accuracy data as numpy array
         """
-        return super().get_data_channel('bearing_accuracy')
+        return super().get_data_channel("bearing_accuracy")
 
     def get_valid_bearing_accuracy_data(self) -> np.array:
         """
         :return: non-nan bearing accuracy data as numpy array
         """
-        return super().get_valid_data_channel_values('bearing_accuracy')
+        return super().get_valid_data_channel_values("bearing_accuracy")
 
     def get_location_provider_data(self) -> List[str]:
         """
         :return: location provider data as list of strings
         """
-        return super()._get_non_numeric_data_channel('location_provider')
+        return super()._get_non_numeric_data_channel("location_provider")
 
     def get_valid_location_provider_data(self) -> List[str]:
         """
         NOT IMPLEMENTED
         :return: non-nan location provider data as list of strings
         """
         pass
         # return super().get_valid_data_channel_values('location_provider')
 
 
 class StationHealthSensor(SensorData):
     """
     Station Health specific functions
     """
-    def __init__(self, sensor_name: str,
-                 sensor_data: Optional[pa.Table] = None,
-                 sample_rate_hz: float = np.nan,
-                 sample_interval_s: float = np.nan,
-                 sample_interval_std_s: float = np.nan,
-                 is_sample_rate_fixed: bool = False,
-                 are_timestamps_altered: bool = False,
-                 calculate_stats: bool = False,
-                 use_offset_model_for_correction: bool = False,
-                 save_data: bool = False,
-                 base_dir: str = ".",
-                 gaps: Optional[List[Tuple[float, float]]] = None,
-                 show_errors: bool = False):
-        super().__init__(sensor_name, sensor_data, SensorType.STATION_HEALTH, sample_rate_hz, sample_interval_s,
-                         sample_interval_std_s, is_sample_rate_fixed, are_timestamps_altered, calculate_stats,
-                         use_offset_model_for_correction, save_data, base_dir, gaps, show_errors)
+
+    def __init__(
+        self,
+        sensor_name: str,
+        sensor_data: Optional[pa.Table] = None,
+        sample_rate_hz: float = np.nan,
+        sample_interval_s: float = np.nan,
+        sample_interval_std_s: float = np.nan,
+        is_sample_rate_fixed: bool = False,
+        are_timestamps_altered: bool = False,
+        calculate_stats: bool = False,
+        use_offset_model_for_correction: bool = False,
+        save_data: bool = False,
+        base_dir: str = ".",
+        gaps: Optional[List[Tuple[float, float]]] = None,
+        show_errors: bool = False,
+    ):
+        super().__init__(
+            sensor_name,
+            sensor_data,
+            SensorType.STATION_HEALTH,
+            sample_rate_hz,
+            sample_interval_s,
+            sample_interval_std_s,
+            is_sample_rate_fixed,
+            are_timestamps_altered,
+            calculate_stats,
+            use_offset_model_for_correction,
+            save_data,
+            base_dir,
+            gaps,
+            show_errors,
+        )
 
     def get_battery_charge_remaining_data(self) -> np.array:
         """
         :return: battery charge remaining data as numpy array
         """
-        return super().get_data_channel('battery_charge_remaining')
+        return super().get_data_channel("battery_charge_remaining")
 
     def get_valid_battery_charge_remaining_data(self) -> np.array:
         """
         :return: non-nan battery charge remaining data as numpy array
         """
-        return super().get_valid_data_channel_values('battery_charge_remaining')
+        return super().get_valid_data_channel_values("battery_charge_remaining")
 
     def get_battery_current_strength_data(self) -> np.array:
         """
         :return: battery current strength data as numpy array
         """
-        return super().get_data_channel('battery_current_strength')
+        return super().get_data_channel("battery_current_strength")
 
     def get_valid_battery_current_strength_data(self) -> np.array:
         """
         :return: non-nan battery current strength data as numpy array
         """
-        return super().get_valid_data_channel_values('battery_current_strength')
+        return super().get_valid_data_channel_values("battery_current_strength")
 
     def get_internal_temp_c_data(self) -> np.array:
         """
         :return: internal temperature celsius data as numpy array
         """
-        return super().get_data_channel('internal_temp_c')
+        return super().get_data_channel("internal_temp_c")
 
     def get_valid_internal_temp_c_data(self) -> np.array:
         """
         :return: non-nan internal temperature celsius data as numpy array
         """
-        return super().get_valid_data_channel_values('internal_temp_c')
+        return super().get_valid_data_channel_values("internal_temp_c")
 
     def get_network_type_data(self) -> List[str]:
         """
         :return: network type data as list of strings
         """
-        return super()._get_non_numeric_data_channel('network_type')
+        return super()._get_non_numeric_data_channel("network_type")
 
     def get_valid_network_type_data(self) -> List[str]:
         """
         NOT IMPLEMENTED
         :return: non-nan network type data as list of strings
         """
         pass
         # return super().get_valid_data_channel_values('network_type')
 
     def get_network_strength_data(self) -> np.array:
         """
         :return: network strength data as numpy array
         """
-        return super().get_data_channel('network_strength')
+        return super().get_data_channel("network_strength")
 
     def get_valid_network_strength_data(self) -> np.array:
         """
         :return: non-nan network strength data as numpy array
         """
-        return super().get_valid_data_channel_values('network_strength')
+        return super().get_valid_data_channel_values("network_strength")
 
     def get_power_state_data(self) -> List[str]:
         """
         :return: power state data as list of strings
         """
-        return super()._get_non_numeric_data_channel('power_state')
+        return super()._get_non_numeric_data_channel("power_state")
 
     def get_valid_power_state_data(self) -> List[str]:
         """
         NOT IMPLEMENTED
         :return: non-nan power state data as list of strings
         """
         pass
         # return super().get_valid_data_channel_values('power_state')
 
     def get_avail_ram_data(self) -> np.array:
         """
         :return: available RAM data as numpy array
         """
-        return super().get_data_channel('avail_ram')
+        return super().get_data_channel("avail_ram")
 
     def get_valid_avail_ram_data(self) -> np.array:
         """
         :return: non-nan available RAM data as numpy array
         """
-        return super().get_valid_data_channel_values('avail_ram')
+        return super().get_valid_data_channel_values("avail_ram")
 
     def get_avail_disk_data(self) -> np.array:
         """
         :return: available disk space data as numpy array
         """
-        return super().get_data_channel('avail_disk')
+        return super().get_data_channel("avail_disk")
 
     def get_valid_avail_disk_data(self) -> np.array:
         """
         :return: non-nan available disk space data as numpy array
         """
-        return super().get_valid_data_channel_values('avail_disk')
+        return super().get_valid_data_channel_values("avail_disk")
 
     def get_cell_service_data(self) -> List[str]:
         """
         :return: cell service data as list of strings
         """
-        return super()._get_non_numeric_data_channel('cell_service')
+        return super()._get_non_numeric_data_channel("cell_service")
 
     def get_valid_cell_service_data(self) -> List[str]:
         """
         NOT IMPLEMENTED
         :return: non-nan cell service data as list of strings
         """
         pass
         # return super().get_valid_data_channel_values('cell_service')
 
     def get_cpu_utilization_data(self) -> np.array:
         """
         :return: CPU utilization data as numpy array
         """
-        return super().get_data_channel('cpu_utilization')
+        return super().get_data_channel("cpu_utilization")
 
     def get_valid_cpu_utilization_data(self) -> np.array:
         """
         :return: non-nan CPU utilization data as numpy array
         """
-        return super().get_valid_data_channel_values('cpu_utilization')
+        return super().get_valid_data_channel_values("cpu_utilization")
 
     def get_wifi_wake_lock_data(self) -> List[str]:
         """
-        :return: wifi wake lock data as list of strings
+        :return: Wi-Fi wake lock data as list of strings
         """
-        return super()._get_non_numeric_data_channel('wifi_wake_lock')
+        return super()._get_non_numeric_data_channel("wifi_wake_lock")
 
     def get_valid_wifi_wake_lock_data(self) -> List[str]:
         """
         NOT IMPLEMENTED
-        :return: non-nan wifi wake lock data as list of strings
+        :return: non-nan Wi-Fi wake lock data as list of strings
         """
         pass
         # return super().get_valid_data_channel_values('wifi_wake_lock')
 
     def get_screen_state_data(self) -> List[str]:
         """
         :return: screen state data as list of strings
         """
-        return super()._get_non_numeric_data_channel('screen_state')
+        return super()._get_non_numeric_data_channel("screen_state")
 
     def get_valid_screen_state_data(self) -> List[str]:
         """
         NOT IMPLEMENTED
         :return: non-nan screen state data as list of strings
         """
         pass
         # return super().get_valid_data_channel_values('screen_state')
 
     def get_screen_brightness_data(self) -> np.array:
         """
         :return: screen brightness data as numpy array
         """
-        return super().get_data_channel('screen_brightness')
+        return super().get_data_channel("screen_brightness")
 
     def get_valid_screen_brightness_data(self) -> np.array:
         """
         :return: non-nan screen brightness data as numpy array
         """
-        return super().get_valid_data_channel_values('screen_brightness')
+        return super().get_valid_data_channel_values("screen_brightness")
```

### Comparing `redvox-3.4.2/redvox/common/sensor_io.py` & `redvox-3.5.0/redvox/common/sensor_io.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,40 +4,35 @@
 from pathlib import Path
 import json
 from typing import (
     Optional,
     TYPE_CHECKING,
 )
 
-from redvox.common.io import json_to_dict, json_file_to_dict, get_json_file
-
 if TYPE_CHECKING:
     from redvox.common.sensor_data import SensorData
 
 
-def to_json(sensor: "SensorData",) -> str:
+def to_json(
+    sensor: "SensorData",
+) -> str:
     """
     :return: sensor as json string
     """
     return json.dumps(sensor.as_dict())
 
 
-def to_json_file(sensor: "SensorData",
-                 file_name: Optional[str] = None) -> Path:
+def to_json_file(sensor: "SensorData", file_name: Optional[str] = None) -> Path:
     """
     saves the sensor as json and data in the same directory.
 
     :param sensor: SensorData to save
     :param file_name: the optional base file name.  Do not include a file extension.
                         If None, a default file name is created using this format:
                         [sensor_type]_[first_timestamp].json
     :return: path to json file
     """
-    _file_name: str = (
-        file_name
-        if file_name is not None
-        else sensor.file_name()
-    )
+    _file_name: str = file_name if file_name is not None else sensor.file_name()
     file_path: Path = sensor.fs_writer().json_path()
     with open(file_path, "w") as f_p:
         f_p.write(to_json(sensor))
         return file_path.resolve(False)
```

### Comparing `redvox-3.4.2/redvox/common/sensor_reader_utils.py` & `redvox-3.5.0/redvox/common/sensor_reader_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 This module loads sensor data from Redvox packets
 """
 
 from typing import Callable, Dict, List, Optional, Tuple, Union
 
 import numpy as np
+
 # noinspection Mypy
 import pyarrow as pa
 
 import redvox.api1000.proto.redvox_api_m_pb2 as api_m
 from redvox.common import date_time_utils as dtu
 from redvox.common.sensor_data import SensorData, SensorType
 
@@ -144,20 +145,16 @@
     SensorType.RELATIVE_HUMIDITY: lambda packet: packet.sensors.relative_humidity,
     SensorType.ROTATION_VECTOR: lambda packet: packet.sensors.rotation_vector,
     SensorType.INFRARED: lambda packet: packet.sensors.proximity,
     SensorType.VELOCITY: lambda packet: packet.sensors.velocity,
 }
 
 
-def __has_sensor(
-        data: Union[api_m.RedvoxPacketM, api_m.RedvoxPacketM.Sensors], field_name: str
-) -> bool:
+def __has_sensor(data: Union[api_m.RedvoxPacketM, api_m.RedvoxPacketM.Sensors], field_name: str) -> bool:
     """
-    Returns true if the given packet or sensors instance contains the valid sensor.
-
     :param data: Either a packet or a packet's sensors message.
     :param field_name: The name of the sensor being checked.
     :return: True if the sensor exists, False otherwise.
     """
     if isinstance(data, api_m.RedvoxPacketM):
         # noinspection Mypy,PyTypeChecker
         return data.sensors.HasField(field_name)
@@ -167,73 +164,61 @@
         return data.HasField(field_name)
 
     return False
 
 
 def __packet_duration_s(packet: api_m.RedvoxPacketM) -> float:
     """
-    Returns the packet duration in seconds.
-
     :param packet: The packet to calculate the duration for.
     :return: The packet duration in seconds.
     """
     return len(packet.sensors.audio.samples.values) / packet.sensors.audio.sample_rate
 
 
 def __packet_duration_us(packet: api_m.RedvoxPacketM) -> float:
     """
-    Returns the packet duration in microseconds.
-
     :param packet: The packet to calculate the duration for.
     :return: The packet duration in microseconds.
     """
     return __packet_duration_s(packet) * 1_000_000.0
 
 
-def __stats_for_sensor_per_packet_per_second(num_packets: int,
-                                             packet_dur_s: float,
-                                             timestamps: np.array) -> Tuple[float, float, float]:
+def __stats_for_sensor_per_packet_per_second(
+    num_packets: int, packet_dur_s: float, timestamps: np.array
+) -> Tuple[float, float, float]:
     """
     Sensor being evaluated must either have 1/packet or 1/second sample rate
 
     :param num_packets: number of packets to calculate stats for
     :param packet_dur_s: duration of packet in seconds
-    :param timestamps: timestamps of the samples
+    :param timestamps: timestamps of the data
     :return: sample rate in hz, sample interval in seconds, and sample interval std deviation
     """
     if len(timestamps) != num_packets:
         sample_rate = 1.0
     else:
         sample_rate = 1 / packet_dur_s
     sample_interval = 1 / sample_rate
     sample_interval_std = (
-        dtu.microseconds_to_seconds(float(np.std(np.diff(timestamps))))
-        if len(timestamps) > 1
-        else np.nan
+        dtu.microseconds_to_seconds(float(np.std(np.diff(timestamps)))) if len(timestamps) > 1 else np.nan
     )
     return sample_rate, sample_interval, sample_interval_std
 
 
-def get_empty_sensor(
-        name: str, sensor_type: SensorType = SensorType.UNKNOWN_SENSOR
-) -> SensorData:
+def get_empty_sensor(name: str, sensor_type: SensorType = SensorType.UNKNOWN_SENSOR) -> SensorData:
     """
-    create a sensor data object with no data
-
     :param name: name of the sensor
     :param sensor_type: type of the sensor to create, default SensorType.UNKNOWN_SENSOR
-    :return: empty sensor
+    :return: empty sensor with no data
     """
     return SensorData(name, pa.Table.from_pydict({"timestamps": []}), sensor_type)
 
 
 def get_sensor_description(sensor: Sensor) -> str:
     """
-    read the sensor's description from the sensor
-
     :param sensor: the sensor to read the description from
     :return: the sensor's description
     """
     return sensor.sensor_description
 
 
 def get_sample_statistics(data_df: pa.Table) -> Tuple[float, float, float]:
@@ -243,31 +228,25 @@
     :param data_df: the dataframe containing timestamps to calculate statistics from
     :return: a Tuple containing the sample rate, interval and interval std dev
     """
     sample_interval: float
     sample_interval_std: float
     timestamps: np.array = data_df["timestamps"].to_numpy()
     if timestamps.size > 1:
-        sample_interval = dtu.microseconds_to_seconds(
-            float(np.mean(np.diff(timestamps)))
-        )
-        sample_interval_std = dtu.microseconds_to_seconds(
-            float(np.std(np.diff(timestamps)))
-        )
+        sample_interval = dtu.microseconds_to_seconds(float(np.mean(np.diff(timestamps))))
+        sample_interval_std = dtu.microseconds_to_seconds(float(np.std(np.diff(timestamps))))
     else:
         sample_interval = np.nan
         sample_interval_std = np.nan
     return 1.0 / sample_interval, sample_interval, sample_interval_std
 
 
-def read_apim_xyz_sensor(
-        sensor: api_m.RedvoxPacketM.Sensors.Xyz, column_id: str
-) -> pa.Table:
+def read_apim_xyz_sensor(sensor: api_m.RedvoxPacketM.Sensors.Xyz, column_id: str) -> pa.Table:
     """
-    read a sensor that has xyz data channels from an api M data packet
+    read a sensor that has xyz data channels from an api M data packet.
     raises Attribute Error if sensor does not contain xyz channels
 
     :param sensor: the xyz api M sensor to read
     :param column_id: string, used to name the columns
     :return: dictionary representing the data in the sensor
     """
     timestamps: np.ndarray = np.array(sensor.timestamps.timestamps)
@@ -276,32 +255,34 @@
             "timestamps",
             "unaltered_timestamps",
             f"{column_id}_x",
             f"{column_id}_y",
             f"{column_id}_z",
         ]
         return pa.Table.from_pydict(
-            dict(zip(columns, [timestamps,
-                               timestamps,
-                               np.array(sensor.x_samples.values),
-                               np.array(sensor.y_samples.values),
-                               np.array(sensor.z_samples.values),
-                               ]
-                     )
-                 )
+            dict(
+                zip(
+                    columns,
+                    [
+                        timestamps,
+                        timestamps,
+                        np.array(sensor.x_samples.values),
+                        np.array(sensor.y_samples.values),
+                        np.array(sensor.z_samples.values),
+                    ],
+                )
+            )
         )
     except AttributeError:
         raise
 
 
-def read_apim_single_sensor(
-        sensor: api_m.RedvoxPacketM.Sensors.Single, column_id: str
-) -> pa.Table:
+def read_apim_single_sensor(sensor: api_m.RedvoxPacketM.Sensors.Single, column_id: str) -> pa.Table:
     """
-    read a sensor that has a single data channel from an api M data packet
+    read a sensor that has a single data channel from an api M data packet.
     raises Attribute Error if sensor does not contain exactly one data channel
 
     :param sensor: the single channel api M sensor to read
     :param column_id: string, used to name the columns
     :return: pyarrow table representing the data in the sensor
     """
     timestamps: np.ndarray = np.array(sensor.timestamps.timestamps)
@@ -310,77 +291,77 @@
         return pa.Table.from_pydict(dict(zip(columns, [timestamps, timestamps, np.array(sensor.samples.values)])))
     except AttributeError:
         raise
 
 
 def apim_compressed_audio_to_pyarrow(comp_audio: api_m.RedvoxPacketM.Sensors.CompressedAudio) -> pa.Table:
     """
-    :param comp_audio: compressed audio sensor to convert to pyarrow table
+    :param comp_audio: compressed audio sensor to convert
     :return: pyarrow table representation of compressed audio data
     """
     return pa.Table.from_pydict(
-        dict(zip(COMPRESSED_AUDIO_COLUMNS,
-                 [
-                     comp_audio.first_sample_timestamp,
-                     comp_audio.first_sample_timestamp,
-                     np.array(list(comp_audio.audio_bytes)),
-                     comp_audio.audio_codec,
-                 ]
-                 )
-             )
+        dict(
+            zip(
+                COMPRESSED_AUDIO_COLUMNS,
+                [
+                    comp_audio.first_sample_timestamp,
+                    comp_audio.first_sample_timestamp,
+                    np.array(list(comp_audio.audio_bytes)),
+                    comp_audio.audio_codec,
+                ],
+            )
+        )
     )
 
 
 def apim_image_to_pyarrow(image_sensor: api_m.RedvoxPacketM.Sensors.Image) -> pa.Table:
     """
-    :param image_sensor: image sensor to convert to pyarrow table
+    :param image_sensor: image sensor to convert
     :return: pyarrow table representation of image data
     """
     timestamps = image_sensor.timestamps.timestamps
     codecs = np.full(len(timestamps), image_sensor.image_codec)
-    return pa.Table.from_pydict(
-        dict(zip(IMAGE_COLUMNS,
-                 [timestamps, timestamps, image_sensor.samples, codecs]
-                 )
-             )
-    )
+    return pa.Table.from_pydict(dict(zip(IMAGE_COLUMNS, [timestamps, timestamps, image_sensor.samples, codecs])))
 
 
-def apim_best_location_to_pyarrow(best_loc: api_m.RedvoxPacketM.Sensors.Location.BestLocation,
-                                  packet_start_timestamp: float) -> pa.Table:
+def apim_best_location_to_pyarrow(
+    best_loc: api_m.RedvoxPacketM.Sensors.Location.BestLocation, packet_start_timestamp: float
+) -> pa.Table:
     """
     :param best_loc: best location to convert to pyarrow table
     :param packet_start_timestamp: timestamp of packet's first sample
-    :return: pyarrow table representation of best location data
+    :return: pyarrow table representation of the best location data
     """
     return pa.Table.from_pydict(
-        dict(zip(LOCATION_COLUMNS,
-                 [
-                     [packet_start_timestamp],
-                     [best_loc.latitude_longitude_timestamp.mach],
-                     [best_loc.latitude_longitude_timestamp.gps],
-                     [best_loc.latitude],
-                     [best_loc.longitude],
-                     [best_loc.altitude],
-                     [best_loc.speed],
-                     [best_loc.bearing],
-                     [best_loc.horizontal_accuracy],
-                     [best_loc.vertical_accuracy],
-                     [best_loc.speed_accuracy],
-                     [best_loc.bearing_accuracy],
-                     [best_loc.location_provider],
-                 ]
-                 )
-             )
+        dict(
+            zip(
+                LOCATION_COLUMNS,
+                [
+                    [packet_start_timestamp],
+                    [best_loc.latitude_longitude_timestamp.mach],
+                    [best_loc.latitude_longitude_timestamp.gps],
+                    [best_loc.latitude],
+                    [best_loc.longitude],
+                    [best_loc.altitude],
+                    [best_loc.speed],
+                    [best_loc.bearing],
+                    [best_loc.horizontal_accuracy],
+                    [best_loc.vertical_accuracy],
+                    [best_loc.speed_accuracy],
+                    [best_loc.bearing_accuracy],
+                    [best_loc.location_provider],
+                ],
+            )
+        )
     )
 
 
 def apim_location_to_pyarrow(loc: api_m.RedvoxPacketM.Sensors.Location) -> pa.Table:
     """
-    :param loc: location sensor to convert to pyarrow table
+    :param loc: location sensor to convert
     :return: pyarrow table representation of location data
     """
     timestamps = loc.timestamps.timestamps
     gps_timestamps = loc.timestamps_gps.timestamps
     lat_samples = loc.latitude_samples.values
     lon_samples = loc.longitude_samples.values
     alt_samples = loc.altitude_samples.values
@@ -401,22 +382,25 @@
         data_for_df[5].append(np.nan if len(alt_samples) <= i else alt_samples[i])
         data_for_df[6].append(np.nan if len(spd_samples) <= i else spd_samples[i])
         data_for_df[7].append(np.nan if len(bear_samples) <= i else bear_samples[i])
         data_for_df[8].append(np.nan if len(hor_acc_samples) <= i else hor_acc_samples[i])
         data_for_df[9].append(np.nan if len(vert_acc_samples) <= i else vert_acc_samples[i])
         data_for_df[10].append(np.nan if len(spd_acc_samples) <= i else spd_acc_samples[i])
         data_for_df[11].append(np.nan if len(bear_acc_samples) <= i else bear_acc_samples[i])
-        data_for_df[12].append(api_m.RedvoxPacketM.Sensors.Location.LocationProvider.UNKNOWN
-                               if len(loc_prov_samples) <= i else loc_prov_samples[i])
+        data_for_df[12].append(
+            api_m.RedvoxPacketM.Sensors.Location.LocationProvider.UNKNOWN
+            if len(loc_prov_samples) <= i
+            else loc_prov_samples[i]
+        )
     return pa.Table.from_pydict(dict(zip(LOCATION_COLUMNS, data_for_df)))
 
 
 def apim_health_to_pyarrow(metrics: api_m.RedvoxPacketM.StationInformation.StationMetrics) -> pa.Table:
     """
-    :param metrics: station metrics to convert to pyarrow table
+    :param metrics: station metrics to convert
     :return: pyarrow table representation of station metrics data
     """
     timestamps = metrics.timestamps.timestamps
     bat_samples = metrics.battery.values
     bat_cur_samples = metrics.battery_current.values
     temp_samples = metrics.temperature.values
     net_samples = metrics.network_type
@@ -432,23 +416,38 @@
     data_for_df = [], [], [], [], [], [], [], [], [], [], [], [], [], [], []
     for i in range(len(timestamps)):
         data_for_df[0].append(timestamps[i])
         data_for_df[1].append(timestamps[i])
         data_for_df[2].append(np.nan if len(bat_samples) < i + 1 else bat_samples[i])
         data_for_df[3].append(np.nan if len(bat_cur_samples) < i + 1 else bat_cur_samples[i])
         data_for_df[4].append(np.nan if len(temp_samples) < i + 1 else temp_samples[i])
-        data_for_df[5].append(api_m.RedvoxPacketM.StationInformation.StationMetrics.NetworkType.UNKNOWN_NETWORK
-                              if len(net_samples) < i + 1 else net_samples[i])
+        data_for_df[5].append(
+            api_m.RedvoxPacketM.StationInformation.StationMetrics.NetworkType.UNKNOWN_NETWORK
+            if len(net_samples) < i + 1
+            else net_samples[i]
+        )
         data_for_df[6].append(np.nan if len(net_str_samples) < i + 1 else net_str_samples[i])
-        data_for_df[7].append(api_m.RedvoxPacketM.StationInformation.StationMetrics.PowerState.UNKNOWN_POWER_STATE
-                              if len(pow_samples) < i + 1 else pow_samples[i])
+        data_for_df[7].append(
+            api_m.RedvoxPacketM.StationInformation.StationMetrics.PowerState.UNKNOWN_POWER_STATE
+            if len(pow_samples) < i + 1
+            else pow_samples[i]
+        )
         data_for_df[8].append(np.nan if len(avail_ram_samples) < i + 1 else avail_ram_samples[i])
         data_for_df[9].append(np.nan if len(avail_disk_samples) < i + 1 else avail_disk_samples[i])
-        data_for_df[10].append(api_m.RedvoxPacketM.StationInformation.StationMetrics.CellServiceState.UNKNOWN
-                               if len(cell_samples) < i + 1 else cell_samples[i])
+        data_for_df[10].append(
+            api_m.RedvoxPacketM.StationInformation.StationMetrics.CellServiceState.UNKNOWN
+            if len(cell_samples) < i + 1
+            else cell_samples[i]
+        )
         data_for_df[11].append(np.nan if len(cpu_util_samples) < i + 1 else cpu_util_samples[i])
-        data_for_df[12].append(api_m.RedvoxPacketM.StationInformation.StationMetrics.WifiWakeLock.NONE
-                               if len(wake_lock_samples) < i + 1 else wake_lock_samples[i])
-        data_for_df[13].append(api_m.RedvoxPacketM.StationInformation.StationMetrics.ScreenState.UNKNOWN_SCREEN_STATE
-                               if len(screen_state_samples) < i + 1 else screen_state_samples[i])
+        data_for_df[12].append(
+            api_m.RedvoxPacketM.StationInformation.StationMetrics.WifiWakeLock.NONE
+            if len(wake_lock_samples) < i + 1
+            else wake_lock_samples[i]
+        )
+        data_for_df[13].append(
+            api_m.RedvoxPacketM.StationInformation.StationMetrics.ScreenState.UNKNOWN_SCREEN_STATE
+            if len(screen_state_samples) < i + 1
+            else screen_state_samples[i]
+        )
         data_for_df[14].append(np.nan if len(screen_bright_samples) < i + 1 else screen_bright_samples[i])
     return pa.Table.from_pydict(dict(zip(STATION_HEALTH_COLUMNS, data_for_df)))
```

### Comparing `redvox-3.4.2/redvox/common/session_io.py` & `redvox-3.5.0/redvox/common/session_io.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,93 +5,73 @@
 import json
 import pickle
 from typing import (
     Optional,
     TYPE_CHECKING,
 )
 
-from redvox.common.io import get_json_file, json_file_to_dict, json_to_dict
-
 
 if TYPE_CHECKING:
     from redvox.common.session_model import SessionModel
 
 
 def session_model_to_json(session: "SessionModel") -> str:
     """
     :return: station as json string
     """
     return json.dumps(session.as_dict())
 
 
-def session_model_to_json_file(session: "SessionModel",
-                               out_dir: str = ".",
-                               file_name: Optional[str] = None) -> Path:
+def session_model_to_json_file(session: "SessionModel", out_dir: str = ".", file_name: Optional[str] = None) -> Path:
     """
     saves the SessionModel as json.
 
     :param session: SessionModel to save
     :param out_dir: path to save file at.  Defaults to "." (current directory)
     :param file_name: the optional base file name.  Do NOT include a file extension.
                         If None, uses the default [id]_[startdate].json
     :return: path to json file
     """
-    _file_name: str = (
-        file_name
-        if file_name is not None
-        else session.default_json_file_name()
-    ) + ".json"
+    _file_name: str = (file_name if file_name is not None else session.default_file_name()) + ".json"
 
     file_path: Path = Path(out_dir).joinpath(_file_name)
     with open(file_path, "w") as f_p:
         f_p.write(session_model_to_json(session))
         return file_path.resolve(False)
 
 
 def session_model_dict_from_json(json_str: str) -> dict:
     """
-    Convert a json file to a dictionary that can create a SessionModel
-
     :param json_str: string of json to read
     :return: dictionary of SessionModel from json
     """
     return json.loads(json_str)
 
 
 def session_model_dict_from_json_file(file_path: str) -> dict:
     """
-    Read the contents of a json file and convert it into a dictionary of a SessionModel
-
     :param file_path: full path to the file, including file name and extension
-    :return: dictionary of SessionModel from json
+    :return: dictionary of SessionModel from json file
     """
     with open(file_path, "r") as f_p:
         return session_model_dict_from_json(f_p.read())
 
 
-def compress_session_model(
-        session: "SessionModel",
-        base_dir: str = ".",
-        file_name: Optional[str] = None
-) -> Path:
+def compress_session_model(session: "SessionModel", base_dir: str = ".", file_name: Optional[str] = None) -> Path:
     """
     Compresses a SessionModel to a pkl file.
 
     :param session: The SessionModel to compress.
     :param base_dir: The base directory to write the serialized file to (default=.).
     :param file_name: The optional file name. Do not include the extension (it's always gonna be .pkl).
                       If None, a default filename with the following format is used: [id]_[start_ts]_model.pkl
     :return: The path to the written compressed file.
     """
 
-    _file_name: str = (
-        file_name
-        if file_name is not None
-        else f"{session.id}_{int(session.start_date)}_model"
-    ) + ".pkl"
+    _file_name: str = (file_name if file_name is not None else session.default_file_name()) + ".pkl"
 
     file_path: Path = Path(base_dir).joinpath(_file_name)
 
     with open(file_path, "wb") as compressed_out:
         pickle.dump(session, compressed_out)
         compressed_out.flush()
         return file_path.resolve(False)
@@ -101,8 +81,8 @@
     """
     Decompresses and deserializes a SessionModel written to disk.
 
     :param path: Path to the serialized and compressed SessionModel.
     :return: An instance of a SessionModel.
     """
     with open(path, "rb") as compressed_in:
-        return pickle.load(compressed_in)
+        return pickle.load(compressed_in)
```

### Comparing `redvox-3.4.2/redvox/common/session_model_utils.py` & `redvox-3.5.0/redvox/common/session_model.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,403 +1,404 @@
-from typing import List, Optional, Tuple
-from dataclasses import dataclass
+import os.path
+from pathlib import Path
+from typing import Dict, List, Optional
 
 import numpy as np
 
+import redvox
+import redvox.api1000.proto.redvox_api_m_pb2 as api_m
+import redvox.common.date_time_utils as dtu
+import redvox.common.session_io as s_io
+import redvox.common.session_model_utils as smu
+from redvox.cloud import session_model_api as cloud_sm
+from redvox.common.errors import RedVoxError, RedVoxExceptions
+
+
+SESSION_VERSION = "2023-06-28"  # Version of the SessionModel
+CLIENT_NAME = "redvox-sdk/session_model"  # Name of the client used to create the SessionModel
+CLIENT_VERSION = SESSION_VERSION  # Version of the client used to create the SessionModel
+APP_NAME = "RedVox"  # Default name of the app
+DAILY_SESSION_NAME = "Day"  # Identifier for day-long dynamic sessions
+HOURLY_SESSION_NAME = "Hour"  # Identifier for hour-long dynamic sessions
 
-@dataclass
-class LocationStat:
-    """
-    Stores the stats of a single location source.
-
-    Variance and standard deviation tuples are optional arguments and will be set to 0 if none are given.
-    If one is given when initialized, but not the other, the proper relational function will be applied to the
-    existing value to get the other.
-
-    If both are given, nothing is done to either value; we assume the user has provided the correct values.
-
-    properties:
-        source_name: str, name of the source of the location data.  Default empty string
-
-        count: int, number of data points for that source.  Default 0
 
-        means: Tuple of float, the mean of the latitude, longitude, and altitude.  Default tuple of np.nan
+class SessionModel:
+    """
+    SDK version of Session from the cloud API
+    """
 
-        variance: Optional Tuple of float, the variance of the latitude, longitude, and altitude.  Default tuple of 0
+    def __init__(
+        self, session: Optional[cloud_sm.Session] = None, dynamic: Optional[Dict[str, cloud_sm.DynamicSession]] = None
+    ):
+        self.cloud_session: Optional[cloud_sm.Session] = session
+        self.dynamic_sessions: Dict[str, cloud_sm.DynamicSession] = {} if dynamic is None else dynamic
+        self._sdk_version: str = redvox.VERSION
+        self._errors: RedVoxExceptions = RedVoxExceptions("SessionModel")
 
-        std_dev: Optional Tuple of float, the standard deviations of latitude, longitude, and altitude.
-        Default tuple of 0.
-    """
-    source_name: str = ""
-    count: int = 0
-    means: Tuple[float, float, float] = (np.nan, np.nan, np.nan)
-    variance: Optional[Tuple[float, float, float]] = None
-    std_dev: Optional[Tuple[float, float, float]] = None
-
-    def __post_init__(self):
-        """
-        ensures the variance and std_dev values are correctly set
-        """
-        if self.variance is None and self.std_dev:
-            self.variance = (self.std_dev[0] * self.std_dev[0],
-                             self.std_dev[1] * self.std_dev[1],
-                             self.std_dev[2] * self.std_dev[2])
-        elif self.std_dev is None and self.variance:
-            self.std_dev = tuple(np.sqrt(self.variance))
-        elif self.std_dev is None and self.variance is None:
-            self.variance = (0., 0., 0.)
-            self.std_dev = (0., 0., 0.)
-
-    def __str__(self):
-        return f"source_name: {self.source_name}, " \
-               f"count: {self.count}, " \
-               f"means (lat, lon, alt): {self.means}, " \
-               f"std_dev (lat, lon, alt): {self.std_dev}, " \
-               f"variance (lat, lon, alt): {self.variance}"
+    def __repr__(self):
+        return (
+            f"cloud_session: {self.cloud_session}, "
+            f"dynamic_sessions: {self.dynamic_sessions}, "
+            f"sdk_version: {self._sdk_version}"
+            f"errors: {self._errors}"
+        )
 
     def as_dict(self) -> dict:
         """
-        :return: LocationStat as a dictionary
+        :return: SessionModel as dictionary
         """
         return {
-            "source_name": self.source_name,
-            "count": self.count,
-            "means": self.means,
-            "variance": self.variance,
-            "std_dev": self.std_dev,
+            "cloud_session": self.cloud_session.to_dict(),
+            "dynamic_sessions": {n: m.to_dict() for n, m in self.dynamic_sessions.items()},
         }
 
     @staticmethod
-    def from_dict(data: dict) -> "LocationStat":
+    def from_dict(dictionary: Dict) -> "SessionModel":
         """
-        LocationStat from dictionary
-        :param data: dictionary of LocationStat values
+        :param dictionary: dictionary to read from
+        :return: SessionModel from the dict
         """
-        return LocationStat(data["source_name"], data["count"], data["means"], data["variance"], data["std_dev"])
+        return SessionModel(
+            cloud_sm.Session.from_dict(dictionary["cloud_session"]),
+            {n: cloud_sm.DynamicSession.from_dict(m) for n, m in dictionary["dynamic_sessions"].items()},
+        )
 
+    def compress(self, out_dir: str = ".") -> Path:
+        """
+        Compresses this SessionModel to a file at out_dir.
+        Uses the id and start_ts to name the file.
 
-class LocationStats:
-    """
-    Stores the stats of all locations
+        :param out_dir: Directory to save file to.  Default "." (current directory)
+        :return: The path to the written file.
+        """
+        return s_io.compress_session_model(self, out_dir)
 
-    protected:
-        _location_stats: all the location stats, default empty list
-    """
-    def __init__(self, loc_stats: Optional[List[LocationStat]] = None):
+    def save(self, out_type: str = "json", out_dir: str = ".") -> Path:
         """
-        initialize the stats
+        Save the SessionModel to disk.  Options for out_type are "json" for JSON file and "pkl" for .pkl file.
+        Defaults to "json".  File will be named after id and start_ts of the SessionModel
 
-        :param loc_stats: the list of stats to start with, default None
+        :param out_type: "json" for JSON file and "pkl" for .pkl file
+        :param out_dir: Directory to save file to.  Default "." (current directory)
+        :return: path to saved file
         """
-        self._location_stats: List[LocationStat] = [] if loc_stats is None else loc_stats
+        if out_type == "pkl":
+            return self.compress(out_dir)
+        return s_io.session_model_to_json_file(self, out_dir)
 
-    def __repr__(self):
-        return f"_location_stats: {[n for n in self._location_stats]}"
+    @staticmethod
+    def load(file_path: str) -> "SessionModel":
+        """
+        Load only works on a JSON or .pkl file.
 
-    def __str__(self):
-        return f"stats: {[n.__str__() for n in self._location_stats]}"
+        :param file_path: full name and path to the SessionModel file
+        :return: SessionModel from a JSON or .pkl file.
+        """
+        ext = os.path.splitext(file_path)[1]
+        if ext == ".json":
+            return SessionModel.from_dict(s_io.session_model_dict_from_json_file(file_path))
+        elif ext == ".pkl":
+            return s_io.decompress_session_model(file_path)
+        else:
+            raise ValueError(f"{file_path} has unknown file extension; this function only accepts json and pkl files.")
 
-    def as_dict(self) -> dict:
+    def default_file_name(self) -> str:
         """
-        :return: LocationStats as a dictionary
+        :return: Default file name as [id]_[start_ts]_model, with start_ts as integer of microseconds
+                    since epoch UTC.  File extension NOT included.
         """
-        return {"location_stats": [n.as_dict() for n in self._location_stats]}
+        return (
+            f"{self.cloud_session.id}_"
+            f"{0 if np.isnan(self.cloud_session.start_ts) else self.cloud_session.start_ts}_model"
+        )
 
     @staticmethod
-    def from_dict(data: dict) -> "LocationStats":
+    def create_from_packet(packet: api_m.RedvoxPacketM) -> "SessionModel":
         """
-        Read LocationData from a LocationStats dictionary
-
-        :param data: dictionary to read from
+        :param packet: API M packet of data to read
+        :return: Session using the data from the packet
         """
-        return LocationStats([LocationStat.from_dict(n) for n in data["location_stats"]])
+        try:
+            duration = (
+                packet.timing_information.packet_end_mach_timestamp
+                - packet.timing_information.packet_start_mach_timestamp
+            )
+            all_sensors = smu.get_all_sensors_in_packet(packet)
+            sensors = [cloud_sm.Sensor(s[0], s[1], smu.add_to_stats(s[2])) for s in all_sensors]
+            local_ts = smu.get_local_timesync(packet)
+            if local_ts is None:
+                raise RedVoxError(
+                    f"Unable to find timing data for station {packet.station_information.id}.\n"
+                    f"Timing is required to complete SessionModel.\nNow Quitting."
+                )
+            fst_lst = cloud_sm.FirstLastBufTimeSync([], smu.NUM_BUFFER_POINTS, [], smu.NUM_BUFFER_POINTS)
+            for f in local_ts[5]:
+                smu.add_to_fst_buffer(fst_lst.fst, fst_lst.fst_max_size, f.ts, f)
+                smu.add_to_lst_buffer(fst_lst.lst, fst_lst.lst_max_size, f.ts, f)
+            timing = cloud_sm.Timing(local_ts[0], local_ts[1], local_ts[2], local_ts[3], local_ts[4], fst_lst)
+            result = SessionModel(
+                cloud_sm.Session(
+                    id=packet.station_information.id,
+                    uuid=packet.station_information.uuid,
+                    desc=packet.station_information.description,
+                    start_ts=int(packet.timing_information.app_start_mach_timestamp),
+                    client=CLIENT_NAME,
+                    client_ver=CLIENT_VERSION,
+                    session_ver=SESSION_VERSION,
+                    app=APP_NAME,
+                    api=int(packet.api),
+                    sub_api=int(packet.sub_api),
+                    make=packet.station_information.make,
+                    model=packet.station_information.model,
+                    app_ver=packet.station_information.app_version,
+                    owner=packet.station_information.auth_id,
+                    private=packet.station_information.is_private,
+                    packet_dur=duration,
+                    sensors=sensors,
+                    n_pkts=1,
+                    timing=timing,
+                    sub=[],
+                )
+            )
+            result.sub = [result.add_dynamic_day(packet)]
+        except Exception as e:
+            # result = SessionModel(station_description=f"FAILED: {e}")
+            raise e
+        return result
 
-    def add_loc_stat(self, new_loc: LocationStat):
+    @staticmethod
+    def create_from_stream(data_stream: List[api_m.RedvoxPacketM]) -> "SessionModel":
         """
-        adds a LocationStat to the stats
-
-        :param new_loc: LocationStat to add
+        :param data_stream: list of API M packets from a single station to read
+        :return: SessionModel using the data packets from the stream
         """
-        self._location_stats.append(new_loc)
+        p1 = data_stream.pop(0)
+        model = SessionModel.create_from_packet(p1)
+        for p in data_stream:
+            model.add_data_from_packet(p)
+        data_stream.insert(0, p1)
+        return model
+
+    def add_data_from_packet(self, packet: api_m.RedvoxPacketM):
+        """
+        Adds the data from the packet to the SessionModel.
+        If the packet doesn't match the key of the SessionModel, writes an error and no data is added
+
+        :param packet: packet to add
+        """
+        if (
+            self.cloud_session.session_key() != f"{packet.station_information.id}:{packet.station_information.uuid}:"
+            f"{int(packet.timing_information.app_start_mach_timestamp)}"
+        ):
+            self._errors.append(
+                "Attempted to add packet with invalid key: "
+                f"{packet.station_information.id}:{packet.station_information.uuid}:"
+                f"{int(packet.timing_information.app_start_mach_timestamp)}"
+            )
+            return
+        local_ts = smu.get_local_timesync(packet)
+        if local_ts is None:
+            self._errors.append(
+                f"Timesync doesn't exist in packet starting at "
+                f"{packet.timing_information.packet_start_mach_timestamp}."
+            )
+        else:
+            timing = self.cloud_session.timing
+            for f in local_ts[5]:
+                smu.add_to_fst_buffer(timing.fst_lst.fst, timing.fst_lst.fst_max_size, f.ts, f)
+                smu.add_to_lst_buffer(timing.fst_lst.lst, timing.fst_lst.lst_max_size, f.ts, f)
+            timing.n_ex += local_ts[2]
+            timing.mean_lat = (timing.mean_lat * self.cloud_session.n_pkts + local_ts[3]) / (
+                self.cloud_session.n_pkts + 1
+            )
+            timing.mean_off = (timing.mean_off * self.cloud_session.n_pkts + local_ts[4]) / (
+                self.cloud_session.n_pkts + 1
+            )
+            if local_ts[0] < timing.first_data_ts:
+                timing.first_data_ts = local_ts[0]
+            if local_ts[1] > timing.last_data_ts:
+                timing.last_data_ts = local_ts[1]
+        all_sensors = smu.get_all_sensors_in_packet(packet)
+        for s in all_sensors:
+            sensor = self.get_sensor(s[0], s[1])
+            if sensor is not None:
+                sensor.sample_rate_stats = smu.add_to_stats(s[2], sensor.sample_rate_stats)
+            else:
+                self.cloud_session.sensors.append(cloud_sm.Sensor(s[0], s[1], smu.add_to_stats(s[2])))
+        self.add_dynamic_day(packet)
+        self.cloud_session.n_pkts += 1
+
+    def add_dynamic_hour(self, data: dict, packet_start: float, session_key: str) -> str:
+        """
+        Add (or update an existing session if key exists) a dynamic session with length of 1 hour using a single packet
+
+        :param data: dictionary of data to add
+        :param packet_start: starting timestamp of the packet in microseconds since epoch UTC
+        :param session_key: the session key of the parent Session
+        :return: the key to the new dynamic session
+        """
+        start_dt = dtu.datetime_from_epoch_microseconds_utc(packet_start)
+        hour_start_dt = dtu.datetime(start_dt.year, start_dt.month, start_dt.day, start_dt.hour)
+        hour_end_ts = int(dtu.datetime_to_epoch_microseconds_utc(hour_start_dt + dtu.timedelta(hours=1)))
+        hour_start_ts = int(dtu.datetime_to_epoch_microseconds_utc(hour_start_dt))
+        key = f"{session_key}:{hour_start_ts}:{hour_end_ts}"
+        if key in self.dynamic_sessions.keys():
+            self._update_dynamic_session(key, data, [f"{packet_start}"])
+        else:
+            self.dynamic_sessions[key] = cloud_sm.DynamicSession(
+                1,
+                smu.add_location_data(data["location"]),
+                smu.add_to_stats(data["battery"]),
+                smu.add_to_stats(data["temperature"]),
+                session_key,
+                hour_start_ts,
+                hour_end_ts,
+                HOURLY_SESSION_NAME,
+                [f"{packet_start}"],
+            )
+        return key
+
+    def add_dynamic_day(self, packet: api_m.RedvoxPacketM) -> str:
+        """
+        Add (or update an existing session if key exists) a dynamic session with length of 1 day using a single packet
+
+        :param packet: packet to read data from
+        :return: the key to the new or updated dynamic session
+        """
+        data = smu.get_dynamic_data(packet)
+        start_dt = dtu.datetime_from_epoch_microseconds_utc(packet.timing_information.packet_start_mach_timestamp)
+        day_start_dt = dtu.datetime(start_dt.year, start_dt.month, start_dt.day)
+        day_end_ts = int(dtu.datetime_to_epoch_microseconds_utc(day_start_dt + dtu.timedelta(days=1)))
+        day_start_ts = int(dtu.datetime_to_epoch_microseconds_utc(day_start_dt))
+        session_key = (
+            f"{packet.station_information.id}:{packet.station_information.uuid}:"
+            f"{packet.timing_information.app_start_mach_timestamp}"
+        )
+        key = f"{session_key}:{day_start_ts}:{day_end_ts}"
+        hourly_key = self.add_dynamic_hour(data, packet.timing_information.packet_start_mach_timestamp, session_key)
+        if key in self.dynamic_sessions.keys():
+            self._update_dynamic_session(key, data, [hourly_key])
+        else:
+            self.dynamic_sessions[key] = cloud_sm.DynamicSession(
+                1,
+                smu.add_location_data(data["location"]),
+                smu.add_to_stats(data["battery"]),
+                smu.add_to_stats(data["temperature"]),
+                session_key,
+                day_start_ts,
+                day_end_ts,
+                DAILY_SESSION_NAME,
+                [hourly_key],
+            )
+        return key
+
+    def _update_dynamic_session(self, key: str, data: Dict, sub: List[str]):
+        """
+        update a dynamic session with a given key.
+
+        :param key: key to the dynamic session
+        :param data: dictionary of data to add
+        :param sub: the list of keys that the dynamic session is linked to
+        """
+        if key not in self.dynamic_sessions.keys():
+            self._errors.append(f"Attempted to update non-existent key: {key}.")
+        else:
+            dyn_sess = self.dynamic_sessions[key]
+            dyn_sess.n_pkts += 1
+            dyn_sess.location = smu.add_location_data(data["location"], dyn_sess.location)
+            dyn_sess.battery = smu.add_to_stats(data["battery"], dyn_sess.battery)
+            dyn_sess.temperature = smu.add_to_stats(data["temperature"], dyn_sess.temperature)
+            for s in sub:
+                if s in self.dynamic_sessions.keys():
+                    self._update_dynamic_session(s, data, self.dynamic_sessions[s].sub)
 
-    def get_all_stats(self) -> List[LocationStat]:
+    def sdk_version(self) -> str:
         """
-        :return: all location stats
+        :return: sdk version used to create the SessionModel
         """
-        return self._location_stats.copy()
+        return self._sdk_version
 
-    def get_sources(self) -> List[str]:
+    def num_sensors(self) -> int:
         """
-        :return: the sources of all location stats
+        :return: number of sensors in the Session
         """
-        return [n.source_name for n in self._location_stats]
+        return len(self.cloud_session.sensors)
 
-    def get_stats_for_source(self, source: str) -> Optional[LocationStat]:
+    def get_sensor_names(self) -> List[str]:
         """
-        :param source: source name to get
-        :return: LocationStat of source requested or None if source doesn't exist
+        :return: number of sensors in the Session
         """
-        for n in self._location_stats:
-            if n.source_name == source:
-                return n
-        return None
+        return [n.name for n in self.cloud_session.sensors]
 
-    def has_source(self, source: str) -> bool:
+    def get_sensor(self, name: str, desc: Optional[str] = None) -> Optional[cloud_sm.Sensor]:
         """
-        :param source: the source name to check for
-        :return: True if the source name is in the stats, False otherwise
+        :param name: name of the sensor to get
+        :param desc: Optional description of the sensor to get.  If None, will get the first sensor that
+                        matches the name given.  Default None.
+        :return: the first sensor that matches the name and description given or None if sensor was not found
         """
-        for n in self._location_stats:
-            if n.source_name == source:
-                return True
-        return False
-
-    def add_count_by_source(self, source: str, val_to_add: int) -> Optional[LocationStat]:
-        """
-        :param source: the source name to update count for
-        :param val_to_add: the number of new points to add to the count
-        :return: the LocationStat with the same source name as the input, or None if the source doesn't exist
-        """
-        for n in self._location_stats:
-            if n.source_name == source:
-                n.count += val_to_add
-                return n
+        for s in self.cloud_session.sensors:
+            if s.name == name:
+                if desc is None or s.description == desc:
+                    return s
         return None
 
-    def add_means_by_source(self, source: str, val_to_add: int,
-                            means_to_add: Tuple[float, float, float]) -> Optional[LocationStat]:
+    def audio_sample_rate_nominal_hz(self) -> float:
         """
-        :param source: the source name to update count and means for
-        :param val_to_add: the number of new points to add to the count
-        :param means_to_add: the means of the location to add
-        :return: the updated LocationStat with the same source name as the input, or None if the source doesn't exist
-        """
-        for n in self._location_stats:
-            if n.source_name == source:
-                n.count += val_to_add
-                n.means = tuple(map(lambda i, j: i + ((j - i) / n.count), n.means, means_to_add))
-                return n
-        return None
-
-    @staticmethod
-    def _update_variances(num_old_samples: int, old_vari: float, old_mean: float,
-                          num_new_samples: int, new_vari: float, new_mean: float) -> float:
+        :return: number of sensors in the Session
         """
-        adds new variance to old variance to get variance of total set
-
-        :param num_old_samples: number of old samples
-        :param old_vari: old variance
-        :param num_new_samples: number of new samples
-        :param new_vari: new variance
-        :return: variance of total set
-        """
-        if num_old_samples + num_new_samples == 0:
-            return 0.
-        combined_mean = (num_old_samples * old_mean + num_new_samples * new_mean) / (num_old_samples + num_new_samples)
-        return ((num_old_samples * (old_vari + np.power((old_mean - combined_mean), 2))
-                 + num_new_samples * (new_vari + np.power((new_mean - combined_mean), 2)))
-                / (num_old_samples + num_new_samples))
-
-    def add_variance_by_source(self, source: str, val_to_add: int,
-                               means_to_add: Tuple[float, float, float],
-                               varis_to_add: Tuple[float, float, float]) -> LocationStat:
-        """
-        Adds data to a LocationStat with the same source, or creates a new LocationStat if source is not found.
-
-        :param source: the source name to update count, means, and std dev for
-        :param val_to_add: the number of new points to add to the count
-        :param means_to_add: the means of the location to add
-        :param varis_to_add: the variances of the location to add
-        :return: the updated LocationStat with the same source name as the input
-        """
-        n = self.get_stats_for_source(source)
-        if n is None:
-            self.add_loc_stat(LocationStat(source, val_to_add, means_to_add, varis_to_add))
-            return self._location_stats[-1]
-        else:
-            n.variance = (self._update_variances(n.count, n.variance[0], n.means[0],
-                                                 val_to_add, varis_to_add[0], means_to_add[0]),
-                          self._update_variances(n.count, n.variance[1], n.means[1],
-                                                 val_to_add, varis_to_add[1], means_to_add[1]),
-                          self._update_variances(n.count, n.variance[2], n.means[2],
-                                                 val_to_add, varis_to_add[2], means_to_add[2]))
-            n.std_dev = tuple(np.sqrt(n.variance))
-            self.add_means_by_source(source, val_to_add, means_to_add)
-            return n
-
-    def add_std_dev_by_source(self, source: str, val_to_add: int,
-                              means_to_add: Tuple[float, float, float],
-                              stds_to_add: Tuple[float, float, float]) -> LocationStat:
-        """
-        Adds data to a LocationStat with the same source, or creates a new LocationStat if source is not found.
-
-        :param source: the source name to update count, means, and std dev for
-        :param val_to_add: the number of new points to add to the count
-        :param means_to_add: the means of the location to add
-        :param stds_to_add: the std devs of the location to add
-        :return: the updated LocationStat with the same source name as the input
-        """
-        return self.add_variance_by_source(source, val_to_add, means_to_add,
-                                           (stds_to_add[0]*stds_to_add[0],
-                                            stds_to_add[1]*stds_to_add[1],
-                                            stds_to_add[2]*stds_to_add[2]))
+        for n in self.cloud_session.sensors:
+            if n.name == "audio":
+                return n.sample_rate_stats.welford.mean
 
-
-class CircularQueue:
-    """
-    Holds data in a fixed size queue that overwrites the oldest entry if allowed.
-
-    Properties:
-        capacity: int, size of the queue
-
-        data: List, the actual data being stored
-
-        head: int, index of the head of the queue.  Default 0
-
-        tail: int, index of the tail of the queue.  Default -1
-
-        size: int, number of actual data points in the queue.  Default 0.  Cannot be more than capacity.
-
-        debug: bool, if True, will output additional messages when errors occur.  Default False
-    """
-    def __init__(self, capacity: int, debug: bool = False):
+    def get_daily_dynamic_sessions(self) -> List[cloud_sm.DynamicSession]:
         """
-        Initialize the queue.
-        Remember to only put the same type of data points into the queue.
-
-        :param capacity: size of the queue
-        :param debug: if True, output additional messages when errors occur, default False
+        :return: all day-long dynamic sessions in the Session
         """
-        self.capacity: int = capacity
-        self.data: List = [None] * capacity
-        self.head: int = 0
-        self.tail: int = -1
-        self.size: int = 0
-        self.debug: bool = debug
-
-    def __repr__(self):
-        return f"capacity: {self.capacity}, " \
-               f"head: {self.head}, " \
-               f"tail: {self.tail}, " \
-               f"size: {self.size}, " \
-               f"data: {self.data}"
-
-    def __str__(self):
-        return f"capacity: {self.capacity}, " \
-               f"head: {self.head}, " \
-               f"tail: {self.tail}, " \
-               f"size: {self.size}, " \
-               f"data: {self.look_at_data()}"
+        return [n for n in self.dynamic_sessions.values() if n.dur == DAILY_SESSION_NAME]
 
-    def as_dict(self) -> dict:
+    def get_hourly_dynamic_sessions(self) -> List[cloud_sm.DynamicSession]:
         """
-        :return: CircularQueue as a dictionary
+        :return: all hour-long dynamic sessions in the Session
         """
-        return {
-            "capacity": self.capacity,
-            "head": self.head,
-            "tail": self.tail,
-            "size": self.size,
-            "data": self.data
-        }
+        return [n for n in self.dynamic_sessions.values() if n.dur == HOURLY_SESSION_NAME]
 
-    @staticmethod
-    def from_dict(data: dict) -> "CircularQueue":
+    def print_errors(self):
         """
-        :param data: dictionary to read from
-        :return: CircularQueue defined by the dictionary
+        print all errors encountered by the SessionModel
         """
-        result = CircularQueue(data["capacity"])
-        result.head = data["head"]
-        result.tail = data["tail"]
-        result.size = data["size"]
-        result.data = data["data"]
-        return result
+        self._errors.print()
 
-    def _update_index(self, index: int):
-        return (index + 1) % self.capacity
 
-    def is_full(self) -> bool:
-        return self.size == self.capacity
+class LocalSessionModels:
+    """
+    SDK version of SessionModelsResp from the cloud API
+    """
 
-    def is_empty(self) -> bool:
-        return self.size == 0
+    def __init__(self):
+        self.sessions: Dict[str, SessionModel] = {}
 
-    def add(self, data: any, limit_size: bool = False):
+    def add_packet(self, packet: api_m.RedvoxPacketM) -> str:
         """
-        adds data to the buffer.  Overwrites values unless limit_size is True
+        add a packet to one of the models, or make a new one
 
-        :param data: data to add
-        :param limit_size: if True, will not overwrite data if the buffer is full
-        """
-        if limit_size and self.is_full():
-            if self.debug:
-                print("Cannot add to full buffer.")
+        :param packet: packet of data to add.
+        :return: key of new or updated packet
+        """
+        key = (
+            f"{packet.station_information.id}:{packet.station_information.uuid}:"
+            f"{int(packet.timing_information.app_start_mach_timestamp)}"
+        )
+        if key not in self.sessions.keys():
+            self.sessions[key] = SessionModel.create_from_packet(packet)
         else:
-            self.tail = self._update_index(self.tail)
-            self.data[self.tail] = data
-            self.size = int(np.minimum(self.size + 1, self.capacity))
-            if self.size == self.capacity and self.tail == self.head:
-                self.head = self._update_index(self.head)
-
-    def remove(self) -> any:
-        """
-        removes the head of the queue
-
-        :return: data removed from the queue
-        """
-        if self.is_empty():
-            if self.debug:
-                print("Cannot remove from empty buffer.")
-            return None
-        result = self.data[self.head]
-        self.head = self._update_index(self.head)
-        self.size -= 1
-        return result
-
-    def peek(self) -> any:
-        """
-        :return: the data at the head index
-        """
-        if self.is_empty():
-            if self.debug:
-                print("Cannot look at empty buffer.")
-            return None
-        return self.data[self.head]
-
-    def peek_tail(self) -> any:
-        """
-        :return: the data at the tail index
-        """
-        if self.is_empty():
-            if self.debug:
-                print("Cannot look at empty buffer.")
-            return None
-        return self.data[self.tail]
-
-    def peek_index(self, index: int) -> any:
-        """
-        converts the index to be within the buffer's capacity if necessary
+            self.sessions[key].add_data_from_packet(packet)
+        return self.sessions[key].cloud_session.session_key()
 
-        :param index: index to look at
-        :return: element at index
+    def get_session(self, key: str) -> Optional[SessionModel]:
         """
-        if self.is_empty():
-            if self.debug:
-                print("Cannot look at empty buffer.")
-            return None
-        return self.data[index % self.capacity]
-
-    def look_at_data(self) -> List:
-        """
-        :return: all data in the queue as a list
+        :param key: key of SessionModel to get
+        :return: SessionModel that matches the given key or None
         """
-        if self.is_empty():
-            if self.debug:
-                print("Buffer is empty.")
-            return []
-        index = self.head
-        result = []
-        for i in range(self.size):
-            result.append(self.data[index])
-            index = self._update_index(index)
-        return result
+        if key in self.sessions.keys():
+            return self.sessions[key]
+        return None
```

### Comparing `redvox-3.4.2/redvox/common/station.py` & `redvox-3.5.0/redvox/common/station.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,40 +8,43 @@
 from pathlib import Path
 
 import numpy as np
 import pyarrow.dataset as ds
 import pyarrow as pa
 
 from redvox.common import station_io as io
-from redvox.common.io import FileSystemWriter as Fsw, FileSystemSaveMode, Index
+from redvox.common.io import FileSystemWriter as Fsw, FileSystemSaveMode, Index, get_json_file, json_file_to_dict
 from redvox.common import sensor_data as sd
 from redvox.common import station_utils as st_utils
+from redvox.common.offset_model import OffsetModel, GPS_LATENCY_MICROS
 from redvox.common.timesync import TimeSync
 from redvox.common.errors import RedVoxExceptions
 import redvox.api1000.proto.redvox_api_m_pb2 as api_m
 from redvox.common import packet_to_pyarrow as ptp
 from redvox.common import gap_and_pad_utils as gpu
-from redvox.common.date_time_utils import datetime_from_epoch_microseconds_utc,\
-    seconds_to_microseconds as s_to_us
+from redvox.common.date_time_utils import datetime_from_epoch_microseconds_utc, seconds_to_microseconds as s_to_us
 from redvox.common.event_stream import EventStreams
 
 
 STATION_ID_LENGTH = 10  # the length of a station ID string
 
 
 class Station:
     """
-    generic station for api-independent stuff; uses API M as the core data object since its quite versatile
-    In order for a list of data to be a station, all of the data packets must:
+    generic station for api-independent stuff; uses API M as the core data object since it's quite versatile
+
+    In order for a list of data to be a station, all the data packets must:
         * Have the same station id
         * Have the same station uuid
         * Have the same start date
         * Have the same audio sample rate
         * Have the same metadata
+
     Generally speaking, stations can be uniquely identified with a minimum of three values: id, uuid, and start date
+
     Properties:
         _data: list of sensor data associated with the station, default empty list
 
         _metadata: StationMetadata consistent across all packets, default empty StationMetadata
 
         _packet_metadata: list of StationPacketMetadata that changes from packet to packet, default empty list
 
@@ -74,23 +77,23 @@
 
         _fs_writer: FileSystemWriter, handles file system i/o parameters
 
         _errors: RedvoxExceptions, errors encountered by the Station
     """
 
     def __init__(
-            self,
-            station_id: str = "",
-            uuid: str = "",
-            start_timestamp: float = np.nan,
-            correct_timestamps: bool = False,
-            use_model_correction: bool = True,
-            base_dir: str = ".",
-            save_data: bool = False,
-            use_temp_dir: bool = False
+        self,
+        station_id: str = "",
+        uuid: str = "",
+        start_timestamp: float = np.nan,
+        correct_timestamps: bool = False,
+        use_model_correction: bool = True,
+        base_dir: str = ".",
+        save_data: bool = False,
+        use_temp_dir: bool = False,
     ):
         """
         initialize Station
 
         :param station_id: string id of the station; defined by users of the station, default ""
         :param uuid: string uuid of the station; automatically created by the station, default ""
         :param start_timestamp: timestamp in epoch UTC when station was started, default np.nan
@@ -110,59 +113,165 @@
         self._packet_metadata: List[st_utils.StationPacketMetadata] = []
         self._errors: RedVoxExceptions = RedVoxExceptions("Station")
         self._first_data_timestamp = np.nan
         self._last_data_timestamp = np.nan
         self._audio_sample_rate_nominal_hz = np.nan
         self._is_audio_scrambled = False
         self._timesync_data = TimeSync()
+        self._gps_offset_model = OffsetModel.empty_model()
         self._is_timestamps_updated = False
         if save_data:
             save_mode = FileSystemSaveMode.DISK
         elif use_temp_dir:
             save_mode = FileSystemSaveMode.TEMP
         else:
             save_mode = FileSystemSaveMode.MEM
         self._fs_writer = Fsw("", "", base_dir, save_mode)
         self._event_data = EventStreams()
 
         self._data: List[sd.SensorData] = []
         self._gaps: List[Tuple[float, float]] = []
 
     def __repr__(self):
-        return f"id: {self._id}, " \
-               f"uuid: {self._uuid}, " \
-               f"start_date: {self._start_date}, " \
-               f"use_model_correction: {self._use_model_correction}, " \
-               f"is_timestamps_updated: {self._is_timestamps_updated}, " \
-               f"metadata: {self._metadata.__repr__()}, " \
-               f"packet_metadata: {[p.__repr__() for p in self._packet_metadata]}, " \
-               f"audio_sample_rate_hz: {self._audio_sample_rate_nominal_hz}, " \
-               f"is_audio_scrambled: {self._is_audio_scrambled}, " \
-               f"timesync: {self._timesync_data.__repr__()}, " \
-               f"event_data: {self.event_data().__repr__()}, " \
-               f"gaps: {[g for g in self._gaps]}"
+        return (
+            f"id: {self._id}, "
+            f"uuid: {self._uuid}, "
+            f"start_date: {self._start_date}, "
+            f"use_model_correction: {self._use_model_correction}, "
+            f"is_timestamps_updated: {self._is_timestamps_updated}, "
+            f"metadata: {self._metadata.__repr__()}, "
+            f"packet_metadata: {[p.__repr__() for p in self._packet_metadata]}, "
+            f"audio_sample_rate_hz: {self._audio_sample_rate_nominal_hz}, "
+            f"is_audio_scrambled: {self._is_audio_scrambled}, "
+            f"timesync: {self._timesync_data.__repr__()}, "
+            f"gps_offset_model: {self._gps_offset_model.__repr__()}, "
+            f"event_data: {self.event_data().__repr__()}, "
+            f"gaps: {[g for g in self._gaps]}"
+        )
         # "data": [d.__repr__() for d in self._data],
 
     def __str__(self):
-        start_date = np.nan if np.isnan(self._start_date) \
-            else datetime_from_epoch_microseconds_utc(self._start_date).strftime('%Y-%m-%dT%H:%M:%S.%fZ')
-        return f"id: {self._id}, " \
-               f"uuid: {self._uuid}, " \
-               f"start_date: {start_date}, " \
-               f"use_model_correction: {self._use_model_correction}, " \
-               f"is_timestamps_updated: {self._is_timestamps_updated}, " \
-               f"metadata: {self._metadata.__str__()}, " \
-               f"audio_sample_rate_hz: {self._audio_sample_rate_nominal_hz}, " \
-               f"is_audio_scrambled: {self._is_audio_scrambled}, " \
-               f"timesync: {self._timesync_data.__str__()}, " \
-               f"event_data: {self.event_data().__str__()}, " \
-               f"gaps: {[g for g in self._gaps]}"
+        start_date = (
+            np.nan
+            if np.isnan(self._start_date)
+            else datetime_from_epoch_microseconds_utc(self._start_date).strftime("%Y-%m-%dT%H:%M:%S.%fZ")
+        )
+        return (
+            f"id: {self._id}, "
+            f"uuid: {self._uuid}, "
+            f"start_date: {start_date}, "
+            f"use_model_correction: {self._use_model_correction}, "
+            f"is_timestamps_updated: {self._is_timestamps_updated}, "
+            f"metadata: {self._metadata.__str__()}, "
+            f"audio_sample_rate_hz: {self._audio_sample_rate_nominal_hz}, "
+            f"is_audio_scrambled: {self._is_audio_scrambled}, "
+            f"timesync: {self._timesync_data.__str__()}, "
+            f"gps_offset_model: {self._gps_offset_model.__str__()}, "
+            f"event_data: {self.event_data().__str__()}, "
+            f"gaps: {[g for g in self._gaps]}"
+        )
         # "packet_metadata": [p.__str__() for p in self._packet_metadata],
         # "data": [d.__str__() for d in self._data]
 
+    def as_dict(self) -> dict:
+        """
+        :return: station as dictionary
+        """
+        return {
+            "id": self._id,
+            "uuid": self._uuid,
+            "start_date": self._start_date,
+            "base_dir": os.path.basename(self.save_dir()),
+            "use_model_correction": self._use_model_correction,
+            "is_audio_scrambled": self._is_audio_scrambled,
+            "is_timestamps_updated": self._is_timestamps_updated,
+            "audio_sample_rate_nominal_hz": self._audio_sample_rate_nominal_hz,
+            "first_data_timestamp": self._first_data_timestamp,
+            "last_data_timestamp": self._last_data_timestamp,
+            "metadata": self._metadata.as_dict(),
+            "packet_metadata": [p.as_dict() for p in self._packet_metadata],
+            "gps_offset_model": self._gps_offset_model.as_dict(),
+            "gaps": self._gaps,
+            "errors": self._errors.as_dict(),
+            "sensors": [s.type().name for s in self._data]
+            # "event_data": self._event_data.as_dict()
+        }
+
+    def default_station_json_file_name(self) -> str:
+        """
+        :return: default station json file name (id_startdate), with startdate as integer of microseconds
+                    since epoch UTC
+        """
+        return f"{self._id}_{0 if np.isnan(self._start_date) else int(self._start_date)}"
+
+    def to_json_file(self, file_name: Optional[str] = None) -> Path:
+        """
+        saves the station as json in station.base_dir, then creates directories and the json for the metadata
+        and data in the same base_dir.
+
+        :param file_name: the optional base file name.  Do not include a file extension.
+                            If None, a default file name is created using this format:
+                            [station_id]_[start_date].json
+        :return: path to json file
+        """
+        return io.to_json_file(self, file_name)
+
+    @staticmethod
+    def from_json_file(file_dir: str, file_name: Optional[str] = None) -> "Station":
+        """
+        convert contents of json file to Station
+
+        :param file_dir: full path to containing directory for the file
+        :param file_name: name of file and extension to load data from.  if not given, will use the first .json file
+                            in the file_dir
+        :return: Station object
+        """
+        if file_name is None:
+            file_name = get_json_file(file_dir)
+            if file_name is None:
+                result = Station("Empty")
+                result.append_error("File to load Sensor from not found.")
+                return result
+        json_data = json_file_to_dict(os.path.join(file_dir, file_name))
+        if "id" in json_data.keys() and "start_date" in json_data.keys():
+            result = Station(
+                json_data["id"],
+                json_data["uuid"],
+                json_data["start_date"],
+                use_model_correction=json_data["use_model_correction"],
+            )
+            result._fs_writer.file_name = json_data["base_dir"]
+            result._gps_offset_model = (
+                OffsetModel.from_dict(json_data["gps_offset_model"])
+                if "gps_offset_model" in json_data.keys()
+                else OffsetModel.empty_model()
+            )
+            result.set_save_mode(FileSystemSaveMode.DISK)
+            result.set_audio_scrambled(json_data["is_audio_scrambled"])
+            result.set_timestamps_updated(json_data["is_timestamps_updated"])
+            result.set_audio_sample_rate_hz(json_data["audio_sample_rate_nominal_hz"])
+            result.set_metadata(st_utils.StationMetadata.from_dict(json_data["metadata"]))
+            result.set_packet_metadata(
+                [st_utils.StationPacketMetadata.from_dict(p) for p in json_data["packet_metadata"]]
+            )
+            result.set_gaps(json_data["gaps"])
+            result.set_errors(RedVoxExceptions.from_dict(json_data["errors"]))
+            for s in json_data["sensors"]:
+                result._data.append(sd.SensorData.from_json_file(os.path.join(file_dir, s)))
+            ts_file_name = get_json_file(os.path.join(file_dir, "timesync"))
+            result.set_timesync_data(TimeSync.from_json_file(os.path.join(file_dir, "timesync", ts_file_name)))
+            ev_file_name = get_json_file(os.path.join(file_dir, "events"))
+            result.set_event_data(EventStreams.from_json_file(os.path.join(file_dir, "events"), ev_file_name))
+            result.update_first_and_last_data_timestamps()
+        else:
+            result = Station()
+            result.append_error(f"Missing id and start date to identify station in {file_name}")
+
+        return result
+
     def data(self) -> List[sd.SensorData]:
         """
         :return: the sensors of the station as a list
         """
         return self._data
 
     def get_sensors(self) -> List[str]:
@@ -247,127 +356,145 @@
 
     @staticmethod
     def load(in_dir: str = "") -> "Station":
         """
         :param in_dir: structured directory with json metadata file to load
         :return: Station using data from files
         """
-        file = io.get_json_file(in_dir)
+        file = get_json_file(in_dir)
         if file is None:
             st = Station("LoadError")
             st.append_error("File to load Station not found.")
             return st
         else:
             return Station.from_json_file(in_dir, file)
 
     @staticmethod
-    def create_from_indexes(indexes: List[Index],
-                            correct_timestamps: bool = False,
-                            use_model_correction: bool = True,
-                            base_out_dir: str = ".",
-                            save_output: bool = False,
-                            use_temp_dir: bool = False) -> "Station":
+    def create_from_indexes(
+        indexes: List[Index],
+        correct_timestamps: bool = False,
+        use_model_correction: bool = True,
+        base_out_dir: str = ".",
+        save_output: bool = False,
+        use_temp_dir: bool = False,
+    ) -> "Station":
         """
         Use a list of Indexes to create a Station
 
         :param indexes: List of indexes to use
         :param correct_timestamps: if True, correct timestamps, default False
         :param use_model_correction: if True, correct timestamps using offset model, default True
         :param base_out_dir: directory to save output files to, if saving to disk.  default "." (current directory)
         :param save_output: if True, save output to disk, default False
         :param use_temp_dir: if True, use a temporary directory, default False
         :return: Station using data from the files in the list of indexes.
         """
-        station = Station(correct_timestamps=correct_timestamps, use_model_correction=use_model_correction,
-                          base_dir=base_out_dir, save_data=save_output, use_temp_dir=use_temp_dir)
+        station = Station(
+            correct_timestamps=correct_timestamps,
+            use_model_correction=use_model_correction,
+            base_dir=base_out_dir,
+            save_data=save_output,
+            use_temp_dir=use_temp_dir,
+        )
         station.load_from_indexes(indexes)
         return station
 
     def load_from_indexes(self, indexes: List[Index]):
         """
         fill station using data from a list of Indexes
 
         :param indexes: List of indexes of the files to read
         """
         self._load_metadata_from_packet(indexes[0].read_first_packet())
         self._timesync_data.arrow_dir = os.path.join(self.save_dir(), "timesync")
-        self._timesync_data.arrow_file = \
-            f"timesync_{0 if np.isnan(self._start_date) else int(self._start_date)}"
+        self._timesync_data.arrow_file = f"timesync_{0 if np.isnan(self._start_date) else int(self._start_date)}"
         all_summaries = ptp.AggregateSummary()
         self._event_data.set_save_dir(os.path.join(self.save_dir(), "events"))
         for idx in indexes:
             pkts = idx.read_contents()
             self._packet_metadata.extend([st_utils.StationPacketMetadata(packet) for packet in pkts])
             self._timesync_data.append_timesync_arrow(TimeSync().from_raw_packets(pkts))
             self._event_data.read_from_packets_list(pkts)
             all_summaries.add_aggregate_summary(
-                ptp.stream_to_pyarrow(pkts, self._fs_writer.get_temp() if self.is_save_to_disk() else None))
+                ptp.stream_to_pyarrow(pkts, self._fs_writer.get_temp() if self.is_save_to_disk() else None)
+            )
         all_summaries.merge_all_summaries()
         self._set_pyarrow_sensors(all_summaries)
         if self._correct_timestamps:
             self.update_timestamps()
 
     @staticmethod
-    def create_from_packets(packets: List[api_m.RedvoxPacketM],
-                            correct_timestamps: bool = False,
-                            use_model_correction: bool = True,
-                            base_out_dir: str = ".",
-                            save_output: bool = False,
-                            use_temp_dir: bool = False) -> "Station":
+    def create_from_packets(
+        packets: List[api_m.RedvoxPacketM],
+        correct_timestamps: bool = False,
+        use_model_correction: bool = True,
+        base_out_dir: str = ".",
+        save_output: bool = False,
+        use_temp_dir: bool = False,
+    ) -> "Station":
         """
         Use a list of Redvox packets to create a Station
 
         :param packets: API M redvox packets with data to load
         :param correct_timestamps: if True, correct timestamps as soon as possible.  Default False
         :param use_model_correction: if True, use OffsetModel functions for time correction, add OffsetModel
                                         best offset (intercept value) otherwise.  Default True
         :param base_out_dir: directory to save parquet files, default "." (current directory)
         :param save_output: if True, save the parquet files to base_out_dir, otherwise delete them.  default False
         :param use_temp_dir: if True, save the parquet files to a temp dir.  default False
         :return: Station using data from redvox packets.
         """
-        station = Station(correct_timestamps=correct_timestamps, use_model_correction=use_model_correction,
-                          base_dir=base_out_dir, save_data=save_output, use_temp_dir=use_temp_dir)
+        station = Station(
+            correct_timestamps=correct_timestamps,
+            use_model_correction=use_model_correction,
+            base_dir=base_out_dir,
+            save_data=save_output,
+            use_temp_dir=use_temp_dir,
+        )
         station.load_data_from_packets(packets)
         return station
 
     @staticmethod
-    def create_from_metadata(packet: api_m.RedvoxPacketM,
-                             use_model_correction: bool = True,
-                             base_out_dir: str = ".",
-                             save_output: bool = False,
-                             use_temp_dir: bool = False) -> "Station":
+    def create_from_metadata(
+        packet: api_m.RedvoxPacketM,
+        use_model_correction: bool = True,
+        base_out_dir: str = ".",
+        save_output: bool = False,
+        use_temp_dir: bool = False,
+    ) -> "Station":
         """
         create a station using metadata from a packet.  There will be no sensor or timing data added.
 
         :param packet: API M redvox packet to load metadata from
         :param use_model_correction: if True, use OffsetModel functions for time correction, add OffsetModel
                                         best offset (intercept value) otherwise.  Default True
         :param base_out_dir: directory to save parquet files, default "." (current directory)
         :param save_output: if True, save the parquet files to base_out_dir, otherwise delete them.  default False
         :param use_temp_dir: if True, save the parquet files to a temp dir.  default False
         :return: Station without any sensor or timing
         """
-        station = Station(use_model_correction=use_model_correction, base_dir=base_out_dir,
-                          save_data=save_output, use_temp_dir=use_temp_dir)
+        station = Station(
+            use_model_correction=use_model_correction,
+            base_dir=base_out_dir,
+            save_data=save_output,
+            use_temp_dir=use_temp_dir,
+        )
         station._load_metadata_from_packet(packet)
         return station
 
     def load_data_from_packets(self, packets: List[api_m.RedvoxPacketM]):
         """
         fill station with data from packets
 
         :param packets: API M redvox packets with data to load
         """
         if packets and st_utils.validate_station_key_list(packets, self._errors):
             # noinspection Mypy
             self._load_metadata_from_packet(packets[0])
-            self._packet_metadata = [
-                st_utils.StationPacketMetadata(packet) for packet in packets
-            ]
+            self._packet_metadata = [st_utils.StationPacketMetadata(packet) for packet in packets]
             self._timesync_data = TimeSync().from_raw_packets(packets)
             self._timesync_data.arrow_dir = os.path.join(self.save_dir(), "timesync")
             self._timesync_data.arrow_file = f"timesync_{0 if np.isnan(self._start_date) else int(self._start_date)}"
             summaries = ptp.stream_to_pyarrow(packets, self._fs_writer.get_temp() if self.is_save_to_disk() else None)
             summaries.merge_all_summaries()
             self._set_pyarrow_sensors(summaries)
             if self._correct_timestamps:
@@ -377,22 +504,20 @@
 
     def _load_metadata_from_packet(self, packet: api_m.RedvoxPacketM):
         """
         sets metadata that applies to the entire station from a single packet
 
         :param packet: API-M redvox packet to load metadata from
         """
-        # self.id = packet.station_information.id
         self._id = packet.station_information.id.zfill(STATION_ID_LENGTH)
         self._uuid = packet.station_information.uuid
         self._start_date = packet.timing_information.app_start_mach_timestamp
         if self._start_date < 0:
             self._errors.append(
-                f"Station {self._id} has station start date before epoch.  "
-                f"Station start date reset to np.nan"
+                f"Station {self._id} has station start date before epoch.  " f"Station start date reset to np.nan"
             )
             self._start_date = np.nan
         self._metadata = st_utils.StationMetadata("Redvox", packet)
         if isinstance(packet, api_m.RedvoxPacketM) and packet.sensors.HasField("audio"):
             self._audio_sample_rate_nominal_hz = packet.sensors.audio.sample_rate
             self._is_audio_scrambled = packet.sensors.audio.is_scrambled
         else:
@@ -494,17 +619,17 @@
     def append_station(self, new_station: "Station"):
         """
         append a new station to the current station; does nothing if keys do not match
 
         :param new_station: Station to append to current station
         """
         if (
-                self.get_key() is not None
-                and new_station.get_key() == self.get_key()
-                and self._metadata.validate_metadata(new_station._metadata)
+            self.get_key() is not None
+            and new_station.get_key() == self.get_key()
+            and self._metadata.validate_metadata(new_station._metadata)
         ):
             self._errors.extend_error(new_station.errors())
             self.append_station_data(new_station._data)
             self._packet_metadata.extend(new_station._packet_metadata)
             self._sort_metadata_packets()
             self._timesync_data.append_timesync_arrow(new_station._timesync_data)
             if not hasattr(self, "_event_data"):
@@ -561,34 +686,30 @@
         """
         adds a sensor to the sensor data dictionary
 
         :param sensor_type: the type of sensor to add
         :param sensor: the sensor data to add
         """
         if sensor_type in self.get_station_sensor_types():
-            raise ValueError(
-                f"Cannot add sensor type ({sensor_type.name}) that already exists in packet!"
-            )
+            raise ValueError(f"Cannot add sensor type ({sensor_type.name}) that already exists in packet!")
         else:
             self._data.append(sensor)
 
     def get_num_packets(self) -> int:
         """
         :return: number of packets used to create station
         """
         return len(self._packet_metadata)
 
     def get_mean_packet_duration(self) -> float:
         """
         :return: mean duration of packets in microseconds
         """
         return float(
-            np.mean(
-                [tsd.packet_end_mach_timestamp - tsd.packet_start_mach_timestamp for tsd in self._packet_metadata]
-            )
+            np.mean([tsd.packet_end_mach_timestamp - tsd.packet_start_mach_timestamp for tsd in self._packet_metadata])
         )
 
     def get_mean_packet_audio_samples(self) -> float:
         """
         calculate the mean number of audio samples per packet using the
           number of audio sensor's data points and the number of packets
 
@@ -618,17 +739,15 @@
 
     def audio_sensor(self) -> Optional[sd.AudioSensor]:
         """
         :return: audio sensor if it exists, None otherwise
         """
         return self.get_sensor_by_type(sd.SensorType.AUDIO)
 
-    def set_audio_sensor(
-            self, audio_sensor: Optional[sd.AudioSensor] = None
-    ) -> "Station":
+    def set_audio_sensor(self, audio_sensor: Optional[sd.AudioSensor] = None) -> "Station":
         """
         sets the audio sensor; can remove audio sensor by passing None
 
         :param audio_sensor: the SensorData to set or None
         :return: the edited Station
         """
         if self.has_audio_sensor():
@@ -652,17 +771,15 @@
 
     def location_sensor(self) -> Optional[sd.LocationSensor]:
         """
         :return: location sensor if it exists, None otherwise
         """
         return self.get_sensor_by_type(sd.SensorType.LOCATION)
 
-    def set_location_sensor(
-            self, loc_sensor: Optional[sd.LocationSensor] = None
-    ) -> "Station":
+    def set_location_sensor(self, loc_sensor: Optional[sd.LocationSensor] = None) -> "Station":
         """
         sets the location sensor; can remove location sensor by passing None
 
         :param loc_sensor: the SensorData to set or None
         :return: the edited Station
         """
         if self.has_location_sensor():
@@ -686,17 +803,15 @@
 
     def best_location_sensor(self) -> Optional[sd.BestLocationSensor]:
         """
         :return: best location sensor if it exists, None otherwise
         """
         return self.get_sensor_by_type(sd.SensorType.BEST_LOCATION)
 
-    def set_best_location_sensor(
-            self, best_loc_sensor: Optional[sd.BestLocationSensor] = None
-    ) -> "Station":
+    def set_best_location_sensor(self, best_loc_sensor: Optional[sd.BestLocationSensor] = None) -> "Station":
         """
         sets the best location sensor; can remove location sensor by passing None
 
         :param best_loc_sensor: the SensorData to set or None
         :return: the edited Station
         """
         if self.has_best_location_sensor():
@@ -720,17 +835,15 @@
 
     def accelerometer_sensor(self) -> Optional[sd.AccelerometerSensor]:
         """
         :return: accelerometer sensor if it exists, None otherwise
         """
         return self.get_sensor_by_type(sd.SensorType.ACCELEROMETER)
 
-    def set_accelerometer_sensor(
-            self, acc_sensor: Optional[sd.AccelerometerSensor] = None
-    ) -> "Station":
+    def set_accelerometer_sensor(self, acc_sensor: Optional[sd.AccelerometerSensor] = None) -> "Station":
         """
         sets the accelerometer sensor; can remove accelerometer sensor by passing None
 
         :param acc_sensor: the SensorData to set or None
         :return: the edited Station
         """
         if self.has_accelerometer_sensor():
@@ -754,17 +867,15 @@
 
     def magnetometer_sensor(self) -> Optional[sd.MagnetometerSensor]:
         """
         :return: magnetometer sensor if it exists, None otherwise
         """
         return self.get_sensor_by_type(sd.SensorType.MAGNETOMETER)
 
-    def set_magnetometer_sensor(
-            self, mag_sensor: Optional[sd.MagnetometerSensor] = None
-    ) -> "Station":
+    def set_magnetometer_sensor(self, mag_sensor: Optional[sd.MagnetometerSensor] = None) -> "Station":
         """
         sets the magnetometer sensor; can remove magnetometer sensor by passing None
 
         :param mag_sensor: the SensorData to set or None
         :return: the edited Station
         """
         if self.has_magnetometer_sensor():
@@ -788,17 +899,15 @@
 
     def gyroscope_sensor(self) -> Optional[sd.GyroscopeSensor]:
         """
         :return: gyroscope sensor if it exists, None otherwise
         """
         return self.get_sensor_by_type(sd.SensorType.GYROSCOPE)
 
-    def set_gyroscope_sensor(
-            self, gyro_sensor: Optional[sd.GyroscopeSensor] = None
-    ) -> "Station":
+    def set_gyroscope_sensor(self, gyro_sensor: Optional[sd.GyroscopeSensor] = None) -> "Station":
         """
         sets the gyroscope sensor; can remove gyroscope sensor by passing None
 
         :param gyro_sensor: the SensorData to set or None
         :return: the edited Station
         """
         if self.has_gyroscope_sensor():
@@ -822,17 +931,15 @@
 
     def pressure_sensor(self) -> Optional[sd.PressureSensor]:
         """
         :return: pressure sensor if it exists, None otherwise
         """
         return self.get_sensor_by_type(sd.SensorType.PRESSURE)
 
-    def set_pressure_sensor(
-            self, pressure_sensor: Optional[sd.PressureSensor] = None
-    ) -> "Station":
+    def set_pressure_sensor(self, pressure_sensor: Optional[sd.PressureSensor] = None) -> "Station":
         """
         sets the pressure sensor; can remove pressure sensor by passing None
 
         :param pressure_sensor: the SensorData to set or None
         :return: the edited Station
         """
         if self.has_pressure_sensor():
@@ -855,17 +962,15 @@
 
     def barometer_sensor(self) -> Optional[sd.PressureSensor]:
         """
         :return: barometer (pressure) sensor if it exists, None otherwise
         """
         return self.pressure_sensor()
 
-    def set_barometer_sensor(
-            self, bar_sensor: Optional[sd.PressureSensor] = None
-    ) -> "Station":
+    def set_barometer_sensor(self, bar_sensor: Optional[sd.PressureSensor] = None) -> "Station":
         """
         sets the barometer (pressure) sensor; can remove barometer sensor by passing None
 
         :param bar_sensor: the SensorData to set or None
         :return: the edited station
         """
         return self.set_pressure_sensor(bar_sensor)
@@ -885,17 +990,15 @@
 
     def light_sensor(self) -> Optional[sd.LightSensor]:
         """
         :return: light sensor if it exists, None otherwise
         """
         return self.get_sensor_by_type(sd.SensorType.LIGHT)
 
-    def set_light_sensor(
-            self, light_sensor: Optional[sd.LightSensor] = None
-    ) -> "Station":
+    def set_light_sensor(self, light_sensor: Optional[sd.LightSensor] = None) -> "Station":
         """
         sets the light sensor; can remove light sensor by passing None
 
         :param light_sensor: the SensorData to set or None
         :return: the edited Station
         """
         if self.has_light_sensor():
@@ -918,17 +1021,15 @@
 
     def infrared_sensor(self) -> Optional[sd.ProximitySensor]:
         """
         :return: infrared (proximity) sensor if it exists, None otherwise
         """
         return self.proximity_sensor()
 
-    def set_infrared_sensor(
-            self, infrd_sensor: Optional[sd.ProximitySensor] = None
-    ) -> "Station":
+    def set_infrared_sensor(self, infrd_sensor: Optional[sd.ProximitySensor] = None) -> "Station":
         """
         sets the infrared sensor; can remove infrared sensor by passing None
 
         :param infrd_sensor: the SensorData to set or None
         :return: the edited Station
         """
         return self.set_proximity_sensor(infrd_sensor)
@@ -948,17 +1049,15 @@
 
     def proximity_sensor(self) -> Optional[sd.ProximitySensor]:
         """
         :return: proximity sensor if it exists, None otherwise
         """
         return self.get_sensor_by_type(sd.SensorType.PROXIMITY)
 
-    def set_proximity_sensor(
-            self, proximity_sensor: Optional[sd.ProximitySensor] = None
-    ) -> "Station":
+    def set_proximity_sensor(self, proximity_sensor: Optional[sd.ProximitySensor] = None) -> "Station":
         """
         sets the proximity sensor; can remove proximity sensor by passing None
 
         :param proximity_sensor: the SensorData to set or None
         :return: the edited Station
         """
         if self.has_proximity_sensor():
@@ -1015,15 +1114,15 @@
     def ambient_temperature_sensor(self) -> Optional[sd.AmbientTemperatureSensor]:
         """
         :return: ambient temperature sensor if it exists, None otherwise
         """
         return self.get_sensor_by_type(sd.SensorType.AMBIENT_TEMPERATURE)
 
     def set_ambient_temperature_sensor(
-            self, amb_temp_sensor: Optional[sd.AmbientTemperatureSensor] = None
+        self, amb_temp_sensor: Optional[sd.AmbientTemperatureSensor] = None
     ) -> "Station":
         """
         sets the ambient temperature sensor; can remove ambient temperature sensor by passing None
 
         :param amb_temp_sensor: the SensorData to set or None
         :return: the edited Station
         """
@@ -1048,17 +1147,15 @@
 
     def relative_humidity_sensor(self) -> Optional[sd.RelativeHumiditySensor]:
         """
         :return: relative humidity sensor if it exists, None otherwise
         """
         return self.get_sensor_by_type(sd.SensorType.RELATIVE_HUMIDITY)
 
-    def set_relative_humidity_sensor(
-            self, rel_hum_sensor: Optional[sd.RelativeHumiditySensor] = None
-    ) -> "Station":
+    def set_relative_humidity_sensor(self, rel_hum_sensor: Optional[sd.RelativeHumiditySensor] = None) -> "Station":
         """
         sets the relative humidity sensor; can remove relative humidity sensor by passing None
 
         :param rel_hum_sensor: the SensorData to set or None
         :return: the edited Station
         """
         if self.has_relative_humidity_sensor():
@@ -1082,17 +1179,15 @@
 
     def gravity_sensor(self) -> Optional[sd.GravitySensor]:
         """
         :return: gravity sensor if it exists, None otherwise
         """
         return self.get_sensor_by_type(sd.SensorType.GRAVITY)
 
-    def set_gravity_sensor(
-            self, grav_sensor: Optional[sd.GravitySensor] = None
-    ) -> "Station":
+    def set_gravity_sensor(self, grav_sensor: Optional[sd.GravitySensor] = None) -> "Station":
         """
         sets the gravity sensor; can remove gravity sensor by passing None
 
         :param grav_sensor: the SensorData to set or None
         :return: the edited Station
         """
         if self.has_gravity_sensor():
@@ -1116,17 +1211,15 @@
 
     def linear_acceleration_sensor(self) -> Optional[sd.LinearAccelerationSensor]:
         """
         :return: linear acceleration sensor if it exists, None otherwise
         """
         return self.get_sensor_by_type(sd.SensorType.LINEAR_ACCELERATION)
 
-    def set_linear_acceleration_sensor(
-            self, lin_acc_sensor: Optional[sd.LinearAccelerationSensor] = None
-    ) -> "Station":
+    def set_linear_acceleration_sensor(self, lin_acc_sensor: Optional[sd.LinearAccelerationSensor] = None) -> "Station":
         """
         sets the linear acceleration sensor; can remove linear acceleration sensor by passing None
 
         :param lin_acc_sensor: the SensorData to set or None
         :return: the edited Station
         """
         if self.has_linear_acceleration_sensor():
@@ -1150,17 +1243,15 @@
 
     def orientation_sensor(self) -> Optional[sd.OrientationSensor]:
         """
         :return: orientation sensor if it exists, None otherwise
         """
         return self.get_sensor_by_type(sd.SensorType.ORIENTATION)
 
-    def set_orientation_sensor(
-            self, orientation_sensor: Optional[sd.OrientationSensor] = None
-    ) -> "Station":
+    def set_orientation_sensor(self, orientation_sensor: Optional[sd.OrientationSensor] = None) -> "Station":
         """
         sets the orientation sensor; can remove orientation sensor by passing None
 
         :param orientation_sensor: the SensorData to set or None
         :return: the edited Station
         """
         if self.has_orientation_sensor():
@@ -1184,17 +1275,15 @@
 
     def rotation_vector_sensor(self) -> Optional[sd.RotationVectorSensor]:
         """
         :return: rotation vector sensor if it exists, None otherwise
         """
         return self.get_sensor_by_type(sd.SensorType.ROTATION_VECTOR)
 
-    def set_rotation_vector_sensor(
-            self, rot_vec_sensor: Optional[sd.RotationVectorSensor] = None
-    ) -> "Station":
+    def set_rotation_vector_sensor(self, rot_vec_sensor: Optional[sd.RotationVectorSensor] = None) -> "Station":
         """
         sets the rotation vector sensor; can remove rotation vector sensor by passing None
 
         :param rot_vec_sensor: the SensorData to set or None
         :return: the edited DataPacket
         """
         if self.has_rotation_vector_sensor():
@@ -1218,17 +1307,15 @@
 
     def compressed_audio_sensor(self) -> Optional[sd.CompressedAudioSensor]:
         """
         :return: compressed audio sensor if it exists, None otherwise
         """
         return self.get_sensor_by_type(sd.SensorType.COMPRESSED_AUDIO)
 
-    def set_compressed_audio_sensor(
-            self, comp_audio_sensor: Optional[sd.CompressedAudioSensor] = None
-    ) -> "Station":
+    def set_compressed_audio_sensor(self, comp_audio_sensor: Optional[sd.CompressedAudioSensor] = None) -> "Station":
         """
         sets the compressed audio sensor; can remove compressed audio sensor by passing None
 
         :param comp_audio_sensor: the SensorData to set or None
         :return: the edited DataPacket
         """
         if self.has_compressed_audio_sensor():
@@ -1252,17 +1339,15 @@
 
     def health_sensor(self) -> Optional[sd.StationHealthSensor]:
         """
         :return: station health sensor (station metrics) if it exists, None otherwise
         """
         return self.get_sensor_by_type(sd.SensorType.STATION_HEALTH)
 
-    def set_health_sensor(
-            self, health_sensor: Optional[sd.StationHealthSensor] = None
-    ) -> "Station":
+    def set_health_sensor(self, health_sensor: Optional[sd.StationHealthSensor] = None) -> "Station":
         """
         sets the health sensor; can remove health sensor by passing None
 
         :param health_sensor: the SensorData to set or None
         :return: the edited DataPacket
         """
         if self.has_health_sensor():
@@ -1285,15 +1370,15 @@
         """
         return self._gaps
 
     def event_data(self) -> EventStreams:
         """
         :return: all EventStreams in the Station
         """
-        return self._event_data if hasattr(self, '_event_data') else None
+        return self._event_data if hasattr(self, "_event_data") else None
 
     def set_event_data(self, data: EventStreams):
         """
         set the station's event data
 
         :param data: EventStreams object to set
         """
@@ -1318,75 +1403,120 @@
         fix any problems with the data in data_table due to app/OS version
 
         :param sensor_type: type of sensor
         :param data_table: the data to edit
         :return: updated table
         """
         # iOS accelerometer recorded values in G's instead of m/s2 before app version 4.1.x
-        if sensor_type == sd.SensorType.ACCELEROMETER and self.metadata().os == st_utils.OsType["IOS"] \
-                and (self._app_version_major()[0] < 4 or
-                     (self._app_version_major()[0] == 4 and self._app_version_major()[1] == 0)):
-            data_table = data_table.set_column(2, "accelerometer_x",
-                                               pa.array(data_table["accelerometer_x"].to_numpy() * -9.8))
-            data_table = data_table.set_column(3, "accelerometer_y",
-                                               pa.array(data_table["accelerometer_y"].to_numpy() * -9.8))
-            data_table = data_table.set_column(4, "accelerometer_z",
-                                               pa.array(data_table["accelerometer_z"].to_numpy() * -9.8))
+        if (
+            sensor_type == sd.SensorType.ACCELEROMETER
+            and self.metadata().os == st_utils.OsType["IOS"]
+            and (
+                self._app_version_major()[0] < 4
+                or (self._app_version_major()[0] == 4 and self._app_version_major()[1] == 0)
+            )
+        ):
+            data_table = data_table.set_column(
+                2, "accelerometer_x", pa.array(data_table["accelerometer_x"].to_numpy() * -9.8)
+            )
+            data_table = data_table.set_column(
+                3, "accelerometer_y", pa.array(data_table["accelerometer_y"].to_numpy() * -9.8)
+            )
+            data_table = data_table.set_column(
+                4, "accelerometer_z", pa.array(data_table["accelerometer_z"].to_numpy() * -9.8)
+            )
         return data_table
 
     def _set_pyarrow_sensors(self, sensor_summaries: ptp.AggregateSummary):
         """
         create sensors using pyarrow functions to convert summaries to tables and metadata
 
         :param sensor_summaries: summaries of sensor data that can be used to create sensors
         """
         audio_summary = sensor_summaries.get_audio()
         if audio_summary:
             # fuse audio into a single result
             self._gaps = sensor_summaries.gaps
-            self._data.append(sd.AudioSensor(audio_summary[0].name, audio_summary[0].data(), audio_summary[0].srate_hz,
-                                             1 / audio_summary[0].srate_hz, 0., True,
-                                             use_offset_model_for_correction=self._use_model_correction,
-                                             base_dir=self.get_save_dir_sensor(sd.SensorType.AUDIO),
-                                             save_data=self._fs_writer.is_save_disk()))
+            self._data.append(
+                sd.AudioSensor(
+                    audio_summary[0].name,
+                    audio_summary[0].data(),
+                    audio_summary[0].srate_hz,
+                    1 / audio_summary[0].srate_hz,
+                    0.0,
+                    True,
+                    use_offset_model_for_correction=self._use_model_correction,
+                    base_dir=self.get_save_dir_sensor(sd.SensorType.AUDIO),
+                    save_data=self._fs_writer.is_save_disk(),
+                )
+            )
             self.update_first_and_last_data_timestamps()
             for snr, sdata in sensor_summaries.get_non_audio().items():
                 if self._fs_writer.is_save_disk():
                     data_table = ds.dataset(sdata[0].fdir, format="parquet", exclude_invalid_files=True).to_table()
                 else:
                     data_table = sdata[0].data()
                     for i in range(1, len(sdata)):
                         data_table = pa.concat_tables([data_table, sdata[i].data()])
                 data_table = self._fix_sensor_data(snr, data_table)
                 if np.isnan(sdata[0].srate_hz):
                     timestamps = data_table["timestamps"].to_numpy()
-                    d, g = gpu.fill_gaps(
-                        data_table,
-                        self._gaps,
-                        float(np.mean(np.diff(timestamps))) if len(timestamps) > 1 else np.nan, "copy")
-                    new_sensor = sd.SensorData(
-                        sensor_name=sdata[0].name, sensor_data=d, gaps=g, save_data=self._fs_writer.is_save_disk(),
-                        sensor_type=snr, calculate_stats=True, is_sample_rate_fixed=False,
-                        use_offset_model_for_correction=self._use_model_correction,
-                        base_dir=self.get_save_dir_sensor(sdata[0].stype))
+                    interval_micros = float(np.mean(np.diff(timestamps))) if len(timestamps) > 1 else np.nan
+                    calculate_stats = True
+                    s_rate = np.nan
+                    s_intv = np.nan
+                    s_intv_std = np.nan
+                    fixed_rate = False
                 else:
-                    d, g = gpu.fill_gaps(
-                        data_table,
-                        self._gaps,
-                        s_to_us(sdata[0].smint_s), "copy")
-                    new_sensor = sd.SensorData(
-                            sensor_name=sdata[0].name, sensor_data=d, gaps=g, save_data=self._fs_writer.is_save_disk(),
-                            sensor_type=snr, sample_rate_hz=sdata[0].srate_hz, sample_interval_s=1/sdata[0].srate_hz,
-                            sample_interval_std_s=0., is_sample_rate_fixed=True,
-                            use_offset_model_for_correction=self._use_model_correction,
-                            base_dir=self.get_save_dir_sensor(sdata[0].stype))
+                    interval_micros = s_to_us(sdata[0].smint_s)
+                    calculate_stats = False
+                    s_rate = sdata[0].srate_hz
+                    s_intv = 1 / sdata[0].srate_hz
+                    s_intv_std = 0.0
+                    fixed_rate = True
+                d, g = gpu.fill_gaps(data_table, self._gaps, interval_micros, "copy")
+                new_sensor = sd.SensorData(
+                    sensor_name=sdata[0].name,
+                    sensor_data=d,
+                    gaps=g,
+                    save_data=self._fs_writer.is_save_disk(),
+                    sensor_type=snr,
+                    calculate_stats=calculate_stats,
+                    sample_rate_hz=s_rate,
+                    sample_interval_s=s_intv,
+                    sample_interval_std_s=s_intv_std,
+                    is_sample_rate_fixed=fixed_rate,
+                    use_offset_model_for_correction=self._use_model_correction,
+                    base_dir=self.get_save_dir_sensor(sdata[0].stype),
+                )
                 self._data.append(new_sensor.class_from_type())
+            self._set_gps_offset()
         else:
             self._errors.append("Audio Sensor expected, but does not exist.")
 
+    def _set_gps_offset(self):
+        """
+        uses the Station's location sensor to set the gps offset.
+        """
+        if self.has_location_data():
+            loc_sensor = self.location_sensor()
+        elif self.has_best_location_data():
+            loc_sensor = self.best_location_sensor()
+        else:
+            self._errors.append("No location data to set GPS offset.")
+            return
+        gps_timestamps = loc_sensor.get_gps_timestamps_data()
+        gps_offsets = gps_timestamps - loc_sensor.data_timestamps() + GPS_LATENCY_MICROS
+        if all(np.nan_to_num(gps_offsets) == 0.0):
+            self._errors.append("Location data is all invalid, cannot set GPS offset.")
+            return
+        self._gps_offset_model = OffsetModel(
+            np.empty(0), gps_offsets, gps_timestamps, gps_timestamps[0], gps_timestamps[-1]
+        )
+
     def _app_version_major(self) -> Tuple[int, int]:
         """
         :return: tuple of app version to 2 significant version numbers (i.e: version number x.y.z returns x and y)
         """
         nums = self.metadata().app_version.split(".")
         if self.metadata().os == st_utils.OsType["IOS"]:
             nums[1] = nums[1].split(" ")[0]
@@ -1462,14 +1592,20 @@
         """
         set the timesync data for the station
 
         :param timesync: timesync data
         """
         self._timesync_data = timesync
 
+    def gps_offset_model(self) -> OffsetModel:
+        """
+        :return: the gps offset model
+        """
+        return self._gps_offset_model
+
     def errors(self) -> RedVoxExceptions:
         """
         :return: errors of the station
         """
         return self._errors
 
     def set_errors(self, errors: RedVoxExceptions):
@@ -1479,14 +1615,15 @@
         :param errors: errors to set
         """
         self._errors = errors
 
     def append_error(self, error: str):
         """
         add an error to the station
+
         :param error: error to add
         """
         self._errors.append(error)
 
     def print_errors(self):
         """
         prints all errors in Station
@@ -1542,157 +1679,86 @@
         """
         :param use_temp_dir: if True, use temp dir to save data.  default False
         """
         self._fs_writer.set_use_temp(use_temp_dir)
         for snr in self._data:
             snr.set_use_temp_dir(use_temp_dir)
 
+    def use_timesync_for_correction(self) -> bool:
+        """
+        Note: This function means nothing if the station is not set to correct timestamps
+
+        :return: True if timesync is used for correction, False if GPS is used instead.
+        """
+        if np.isnan(self._timesync_data.mean_latency()) or self._timesync_data.best_offset() == 0.0:
+            return False
+        return True
+
     def update_timestamps(self) -> "Station":
         """
         updates the timestamps in the station using the offset model
+
+        :return: updated Station
         """
-        if self._is_timestamps_updated:
-            self._errors.append("Timestamps already corrected!")
-        elif self._correct_timestamps:
-            self._start_date = self._timesync_data.offset_model().update_time(
-                self._start_date, self._use_model_correction
-            )
+        if not self._is_timestamps_updated and self._correct_timestamps:
+            if self.use_timesync_for_correction():
+                offset_model = self._timesync_data.offset_model()
+            else:
+                offset_model = self._gps_offset_model
+            self._start_date = offset_model.update_time(self._start_date, self._use_model_correction)
+            for sensor in self._data:
+                sensor.update_data_timestamps(offset_model)
+            for packet in self._packet_metadata:
+                packet.update_timestamps(offset_model, self._use_model_correction)
+            for g in range(len(self._gaps)):
+                self._gaps[g] = (offset_model.update_time(self._gaps[g][0]), offset_model.update_time(self._gaps[g][1]))
+            if hasattr(self, "_event_data"):
+                self._event_data.update_timestamps(offset_model, self.use_model_correction())
             if self._fs_writer.file_name != self._get_id_key():
                 if self._fs_writer.is_save_disk():
                     old_name = self.save_dir()
                     self.set_save_dir(self._fs_writer.base_dir)
                     if old_name != "." and os.path.exists(old_name):
                         os.rename(old_name, self.save_dir())
                 else:
                     self._fs_writer.file_name = self._get_id_key()
-            for sensor in self._data:
-                sensor.update_data_timestamps(self._timesync_data.offset_model())
-            for packet in self._packet_metadata:
-                packet.update_timestamps(self._timesync_data.offset_model(), self._use_model_correction)
-            for g in range(len(self._gaps)):
-                self._gaps[g] = (self._timesync_data.offset_model().update_time(self._gaps[g][0]),
-                                 self._timesync_data.offset_model().update_time(self._gaps[g][1]))
-            if hasattr(self, "_event_data"):
-                self._event_data.update_timestamps(self._timesync_data.offset_model(), self.use_model_correction())
             self.update_first_and_last_data_timestamps()
             self._timesync_data.arrow_file = f"timesync_{0 if np.isnan(self._start_date) else int(self._start_date)}"
             self._is_timestamps_updated = True
-        else:
-            self._errors.append("Attempted to correct timestamps, but correction not enabled.")
         return self
 
     def undo_update_timestamps(self) -> "Station":
         """
         undoes non-sensor timestamp updates of the timestamps in the station using the offset model
         sensors already have unaltered timestamps
+
+        :return: updated Station
         """
-        if not self._is_timestamps_updated:
-            self._errors.append("Timestamps already not corrected!")
-        else:
-            self._start_date = self._timesync_data.offset_model().get_original_time(
-                self._start_date, self._use_model_correction
-            )
+        if self._is_timestamps_updated:
+            if self.use_timesync_for_correction():
+                offset_model = self._timesync_data.offset_model()
+            else:
+                offset_model = self._gps_offset_model
+            self._start_date = offset_model.get_original_time(self._start_date, self._use_model_correction)
+            for sensor in self._data:
+                sensor.set_original_timestamps()
+            for packet in self._packet_metadata:
+                packet.original_timestamps(offset_model, self._use_model_correction)
+            for g in range(len(self._gaps)):
+                self._gaps[g] = (
+                    offset_model.get_original_time(self._gaps[g][0]),
+                    offset_model.get_original_time(self._gaps[g][1]),
+                )
+            if hasattr(self, "_event_data"):
+                self._event_data.original_timestamps(offset_model, self.use_model_correction())
             if self._fs_writer.file_name != self._get_id_key():
                 if self._fs_writer.is_save_disk():
                     old_name = self.save_dir()
                     self.set_save_dir(self._fs_writer.base_dir)
                     if old_name != "." and os.path.exists(old_name):
                         os.rename(old_name, self.save_dir())
                 else:
                     self._fs_writer.file_name = self._get_id_key()
-            for sensor in self._data:
-                sensor.set_original_timestamps()
-            for packet in self._packet_metadata:
-                packet.original_timestamps(self._timesync_data.offset_model(), self._use_model_correction)
-            for g in range(len(self._gaps)):
-                self._gaps[g] = (self._timesync_data.offset_model().get_original_time(self._gaps[g][0]),
-                                 self._timesync_data.offset_model().get_original_time(self._gaps[g][1]))
-            if hasattr(self, "_event_data"):
-                self._event_data.original_timestamps(self._timesync_data.offset_model(), self.use_model_correction())
             self.update_first_and_last_data_timestamps()
             self._timesync_data.arrow_file = f"timesync_{0 if np.isnan(self._start_date) else int(self._start_date)}"
-            self._is_timestamps_updated = True
+            self._is_timestamps_updated = False
         return self
-
-    def as_dict(self) -> dict:
-        """
-        :return: station as dictionary
-        """
-        return {
-            "id": self._id,
-            "uuid": self._uuid,
-            "start_date": self._start_date,
-            "base_dir": os.path.basename(self.save_dir()),
-            "use_model_correction": self._use_model_correction,
-            "is_audio_scrambled": self._is_audio_scrambled,
-            "is_timestamps_updated": self._is_timestamps_updated,
-            "audio_sample_rate_nominal_hz": self._audio_sample_rate_nominal_hz,
-            "first_data_timestamp": self._first_data_timestamp,
-            "last_data_timestamp": self._last_data_timestamp,
-            "metadata": self._metadata.as_dict(),
-            "packet_metadata": [p.as_dict() for p in self._packet_metadata],
-            "gaps": self._gaps,
-            "errors": self._errors.as_dict(),
-            "sensors": [s.type().name for s in self._data]
-            # "event_data": self._event_data.as_dict()
-        }
-
-    def default_station_json_file_name(self) -> str:
-        """
-        :return: default station json file name (id_startdate), with startdate as integer of microseconds
-                    since epoch UTC
-        """
-        return f"{self._id}_{0 if np.isnan(self._start_date) else int(self._start_date)}"
-
-    def to_json_file(self, file_name: Optional[str] = None) -> Path:
-        """
-        saves the station as json in station.base_dir, then creates directories and the json for the metadata
-        and data in the same base_dir.
-
-        :param file_name: the optional base file name.  Do not include a file extension.
-                            If None, a default file name is created using this format:
-                            [station_id]_[start_date].json
-        :return: path to json file
-        """
-        return io.to_json_file(self, file_name)
-
-    @staticmethod
-    def from_json_file(file_dir: str, file_name: Optional[str] = None) -> "Station":
-        """
-        convert contents of json file to Station
-
-        :param file_dir: full path to containing directory for the file
-        :param file_name: name of file and extension to load data from
-        :return: Station object
-        """
-        if file_name is None:
-            file_name = io.get_json_file(file_dir)
-            if file_name is None:
-                result = Station("Empty")
-                result.append_error("File to load Sensor from not found.")
-                return result
-        json_data = io.json_file_to_dict(os.path.join(file_dir, file_name))
-        if "id" in json_data.keys() and "start_date" in json_data.keys():
-            result = Station(json_data["id"], json_data["uuid"], json_data["start_date"],
-                             use_model_correction=json_data["use_model_correction"])
-            result._fs_writer.file_name = json_data["base_dir"]
-            result.set_save_mode(FileSystemSaveMode.DISK)
-            result.set_audio_scrambled(json_data["is_audio_scrambled"])
-            result.set_timestamps_updated(json_data["is_timestamps_updated"])
-            result.set_audio_sample_rate_hz(json_data["audio_sample_rate_nominal_hz"])
-            result.set_metadata(st_utils.StationMetadata.from_dict(json_data["metadata"]))
-            result.set_packet_metadata(
-                [st_utils.StationPacketMetadata.from_dict(p) for p in json_data["packet_metadata"]])
-            result.set_gaps(json_data["gaps"])
-            result.set_errors(RedVoxExceptions.from_dict(json_data["errors"]))
-            for s in json_data["sensors"]:
-                result._data.append(sd.SensorData.from_json_file(os.path.join(file_dir, s)))
-            ts_file_name = io.get_json_file(os.path.join(file_dir, "timesync"))
-            result.set_timesync_data(TimeSync.from_json_file(os.path.join(file_dir, "timesync", ts_file_name)))
-            ev_file_name = io.get_json_file(os.path.join(file_dir, "events"))
-            result.set_event_data(EventStreams.from_json_file(os.path.join(file_dir, "events"), ev_file_name))
-            result.update_first_and_last_data_timestamps()
-        else:
-            result = Station()
-            result.append_error(f"Missing id and start date to identify station in {file_name}")
-
-        return result
```

### Comparing `redvox-3.4.2/redvox/common/station_io.py` & `redvox-3.5.0/redvox/common/station_io.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,53 +5,46 @@
 import json
 import os
 from typing import (
     Optional,
     TYPE_CHECKING,
 )
 
-from redvox.common.io import get_json_file, json_file_to_dict, json_to_dict
-
 
 if TYPE_CHECKING:
     from redvox.common.station import Station
 
 
-def to_json(station: "Station",) -> str:
+def to_json(
+    station: "Station",
+) -> str:
     """
     :return: station as json string
     """
     return json.dumps(station.as_dict())
 
 
-def to_json_file(station: "Station",
-                 file_name: Optional[str] = None) -> Path:
+def to_json_file(station: "Station", file_name: Optional[str] = None) -> Path:
     """
     saves the station as json and data in the same directory.
 
     :param station: Station to save
     :param file_name: the optional base file name.  Do not include a file extension.
                         If None, uses the default [id]_[startdate].json
     :return: path to json file
     """
-    _file_name: str = (
-        file_name
-        if file_name is not None
-        else station.default_station_json_file_name()
-    )
+    _file_name: str = file_name if file_name is not None else station.default_station_json_file_name()
 
     # write the sensor objects, using the default values
     for datas in station.data():
         datas.to_json_file()
 
-    # ts_dir = os.path.join(station.save_dir(), "timesync")
     os.makedirs(station.timesync_data().arrow_dir, exist_ok=True)
     station.timesync_data().to_json_file()
 
-    # ev_dir = os.path.join(station.save_dir(), "events")
     os.makedirs(station.get_event_data_dir(), exist_ok=True)
     station.event_data().to_json_file(station.get_event_data_dir())
 
     file_path: Path = Path(station.save_dir()).joinpath(station.fs_writer().json_file_name())
     with open(file_path, "w") as f_p:
         f_p.write(to_json(station))
         return file_path.resolve(False)
```

### Comparing `redvox-3.4.2/redvox/common/station_model.py` & `redvox-3.5.0/redvox/common/station_model.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,123 +1,130 @@
-from typing import List
-
-import numpy as np
-
-import redvox
-from redvox.common.session_model import SessionModel
-from redvox.common.date_time_utils import datetime_from_epoch_microseconds_utc
-
-
-class StationModel:
-    """
-    Model for a station.  Does not include data.
-
-    Properties:
-        id: string, the id of the station.  Users can change this
-
-        uuid: string, the uuid of the station.  This is set by the app when it is installed on a device
-
-        audio_sample_rate_hz: int, the audio sample rate in hz of the station
-
-        sessions: List of SessionModel: the sessions used to create the StationModel
-
-        app: string, name of the app
-
-        app_version: string, version of the app
-
-        api: float, the api version of the data
-
-        sub_api: float, the sub api of the data
-
-        make: string, make of the station
-
-        model: string, model of the station
-
-        num_sessions: int, number of sessions in the model
-
-        sdk_version: string, version of SDK used to create the model
-
-        start_date: float, timestamp of first station data point in microseconds since epoch UTC
-
-        end_date: float, timestamp of last station data point in microseconds since epoch UTC
-
-        changelog: List of str, list of all changes to station during lifetime
-    """
-    def __init__(self,
-                 station_id: str = "",
-                 uuid: str = "",
-                 app_name: str = "Redvox",
-                 api: float = np.nan,
-                 sub_api: float = np.nan,
-                 make: str = "",
-                 model: str = "",
-                 app_version: str = "",
-                 start_date: float = np.nan,
-                 end_date: float = np.nan
-                 ):
-        self.id: str = station_id
-        self.uuid: str = uuid
-        self.app_name: str = app_name
-        self.api: float = api
-        self.sub_api: float = sub_api
-        self.make: str = make
-        self.model: str = model
-        self.app_version: str = app_version
-        self.num_sessions: int = 0
-        self.sdk_version: str = redvox.version()
-        self.start_date: float = start_date
-        self.end_date: float = end_date
-        self.changelog: List[str] = []
-
-    def add_session(self, session: SessionModel):
-        """
-        Add a new session to the StationModel.  id and uuid must match; no change if no match
-
-        :param session: Session to add
-        """
-        if self.id == session.id and self.uuid == session.uuid:
-            self.num_sessions += 1
-            if self.start_date > session.start_date:
-                self.start_date = session.start_date
-            if self.end_date < session.last_data_timestamp:
-                self.end_date = session.last_data_timestamp
-            first_timestamp = np.nan if np.isnan(session.first_data_timestamp) \
-                else datetime_from_epoch_microseconds_utc(
-                session.first_data_timestamp).strftime('%Y-%m-%dT%H:%M:%S.%fZ')
-            last_timestamp = np.nan if np.isnan(session.last_data_timestamp) \
-                else datetime_from_epoch_microseconds_utc(
-                session.last_data_timestamp).strftime('%Y-%m-%dT%H:%M:%S.%fZ')
-            self.changelog.append(f"session from {first_timestamp}: {last_timestamp}")
-
-    @staticmethod
-    def create_from_session(session: SessionModel) -> "StationModel":
-        """
-        Create StationModel from a single session
-
-        :param session: SessionModel to create StationModel from
-        :return: StationModel
-        """
-        try:
-            result = StationModel(session.id, session.uuid, session.app_name, session.api, session.sub_api,
-                                  session.make, session.model, session.app_version, session.start_date,
-                                  session.last_data_timestamp
-                                  )
-        except Exception as e:
-            raise e
-        return result
-
-    @staticmethod
-    def create_from_sessions(sessions: List[SessionModel]) -> "StationModel":
-        """
-        create StationModel from a list of sessions.  Uses the first SessionModel as the base for the StationModel,
-        and will ignore any SessionModel that does not align with the first SessionModel
-
-        :param sessions: sessions to create StationModel from
-        :return: StationModel
-        """
-        p1 = sessions.pop(0)
-        model = StationModel.create_from_session(p1)
-        for p in sessions:
-            model.add_session(p)
-        sessions.insert(0, p1)
-        return model
+"""
+Prototype class
+In Development
+
+Class representing the Station information that can be used to convert Station into another format.
+"""
+
+# from typing import List
+#
+# import numpy as np
+#
+# import redvox
+# from redvox.common.session_model import SessionModel
+# from redvox.common.date_time_utils import datetime_from_epoch_microseconds_utc
+#
+#
+# class StationModel:
+#     """
+#     Model for a station.  Does not include data.
+#
+#     Properties:
+#         id: string, the id of the station.  Users can change this
+#
+#         uuid: string, the uuid of the station.  This is set by the app when it is installed on a device
+#
+#         audio_sample_rate_hz: int, the audio sample rate in hz of the station
+#
+#         sessions: List of SessionModel: the sessions used to create the StationModel
+#
+#         app: string, name of the app
+#
+#         app_version: string, version of the app
+#
+#         api: float, the api version of the data
+#
+#         sub_api: float, the sub api of the data
+#
+#         make: string, make of the station
+#
+#         model: string, model of the station
+#
+#         num_sessions: int, number of sessions in the model
+#
+#         sdk_version: string, version of SDK used to create the model
+#
+#         start_date: float, timestamp of first station data point in microseconds since epoch UTC
+#
+#         end_date: float, timestamp of last station data point in microseconds since epoch UTC
+#
+#         changelog: List of str, list of all changes to station during lifetime
+#     """
+#     def __init__(self,
+#                  station_id: str = "",
+#                  uuid: str = "",
+#                  app_name: str = "Redvox",
+#                  api: float = np.nan,
+#                  sub_api: float = np.nan,
+#                  make: str = "",
+#                  model: str = "",
+#                  app_version: str = "",
+#                  start_date: float = np.nan,
+#                  end_date: float = np.nan
+#                  ):
+#         self.id: str = station_id
+#         self.uuid: str = uuid
+#         self.app_name: str = app_name
+#         self.api: float = api
+#         self.sub_api: float = sub_api
+#         self.make: str = make
+#         self.model: str = model
+#         self.app_version: str = app_version
+#         self.num_sessions: int = 0
+#         self.sdk_version: str = redvox.version()
+#         self.start_date: float = start_date
+#         self.end_date: float = end_date
+#         self.changelog: List[str] = []
+#
+#     def add_session(self, session: SessionModel):
+#         """
+#         Add a new session to the StationModel.  id and uuid must match; no change if no match
+#
+#         :param session: Session to add
+#         """
+#         if self.id == session.id and self.uuid == session.uuid:
+#             self.num_sessions += 1
+#             if self.start_date > session.start_date:
+#                 self.start_date = session.start_date
+#             if self.end_date < session.last_data_timestamp:
+#                 self.end_date = session.last_data_timestamp
+#             first_timestamp = np.nan if np.isnan(session.first_data_timestamp) \
+#                 else datetime_from_epoch_microseconds_utc(
+#                 session.first_data_timestamp).strftime('%Y-%m-%dT%H:%M:%S.%fZ')
+#             last_timestamp = np.nan if np.isnan(session.last_data_timestamp) \
+#                 else datetime_from_epoch_microseconds_utc(
+#                 session.last_data_timestamp).strftime('%Y-%m-%dT%H:%M:%S.%fZ')
+#             self.changelog.append(f"session from {first_timestamp}: {last_timestamp}")
+#
+#     @staticmethod
+#     def create_from_session(session: SessionModel) -> "StationModel":
+#         """
+#         Create StationModel from a single session
+#
+#         :param session: SessionModel to create StationModel from
+#         :return: StationModel
+#         """
+#         try:
+#             result = StationModel(session.id, session.uuid, session.app_name, session.api, session.sub_api,
+#                                   session.make, session.model, session.app_version, session.start_date,
+#                                   session.last_data_timestamp
+#                                   )
+#         except Exception as e:
+#             raise e
+#         return result
+#
+#     @staticmethod
+#     def create_from_sessions(sessions: List[SessionModel]) -> "StationModel":
+#         """
+#         create StationModel from a list of sessions.  Uses the first SessionModel as the base for the StationModel,
+#         and will ignore any SessionModel that does not align with the first SessionModel
+#
+#         :param sessions: sessions to create StationModel from
+#         :return: StationModel
+#         """
+#         p1 = sessions.pop(0)
+#         model = StationModel.create_from_session(p1)
+#         for p in sessions:
+#             model.add_session(p)
+#         sessions.insert(0, p1)
+#         return model
```

### Comparing `redvox-3.4.2/redvox/common/station_utils.py` & `redvox-3.5.0/redvox/common/station_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 """
 Defines generic station metadata for API-independent analysis
 all timestamps are floats in microseconds unless otherwise stated
 """
 from dataclasses import dataclass
+from dataclasses_json import dataclass_json
 from typing import Tuple, Optional, List, Dict
 
 import numpy as np
 
 from redvox.common.offset_model import OffsetModel
 from redvox.api1000.wrapped_redvox_packet.station_information import OsType
 from redvox.api1000.wrapped_redvox_packet.timing_information import TimingScoreMethod
 from redvox.common.errors import RedVoxExceptions
 import redvox.api1000.proto.redvox_api_m_pb2 as api_m
 
 
-def validate_station_key_list(
-    data_packets: List[api_m.RedvoxPacketM], errors: RedVoxExceptions
-) -> bool:
+def validate_station_key_list(data_packets: List[api_m.RedvoxPacketM], errors: RedVoxExceptions) -> bool:
     """
     Checks for consistency in the data packets.  Returns False if discrepancies are found.
     If debug is True, will output the discrepancies.
 
     :param data_packets: list of RedvoxPacketM to look at
     :param errors: RedVoxExceptions detailing errors found while validating
     :return: True if no discrepancies found.  False otherwise
@@ -39,15 +38,15 @@
                 t.station_information.make,
                 t.station_information.model,
                 t.station_information.os,
                 t.station_information.os_version,
                 t.station_information.app_version,
                 t.station_information.is_private,
                 len(t.sensors.audio.samples.values) / t.sensors.audio.sample_rate,
-                ]
+            ]
             for t in data_packets
         ]
     )
 
     k: Dict[str, np.ndarray] = {
         "ids": j[0],
         "uuids": j[1],
@@ -75,21 +74,25 @@
     if my_errors.get_num_errors() > 0:
         errors.extend_error(my_errors)
         return False
 
     return True  # if here, everything is consistent
 
 
+@dataclass_json
 @dataclass
 class StationKey:
     """
     A set of values that uniquely define a station
+
     Properties:
         id: str, id of the station
+
         uuid: str, uuid of the station
+
         start_timestamp_micros: float, starting time of the station in microseconds since epoch UTC
     """
 
     id: str
     uuid: str
     start_timestamp_micros: float
 
@@ -98,36 +101,39 @@
 
     def get_key(self) -> Tuple[str, str, float]:
         """
         :return: the key as a tuple
         """
         return self.id, self.uuid, self.start_timestamp_micros
 
-    def check_key(self, station_id: Optional[str] = None, station_uuid: Optional[str] = None,
-                  start_timestamp: Optional[float] = None) -> bool:
+    def check_key(
+        self,
+        station_id: Optional[str] = None,
+        station_uuid: Optional[str] = None,
+        start_timestamp: Optional[float] = None,
+    ) -> bool:
         """
         check if the key has the values specified.  If the parameter is None, any value will match.
         Note that NAN is a valid value for start_timestamps, but any station with start_timestamp = NAN
         will not match any value, including another NAN.
 
         :param station_id: station id, default None
         :param station_uuid: station uuid, default None
         :param start_timestamp: station start timestamp in microseconds since UTC epoch, default None
         :return: True if all parameters match key values
         """
         if station_id is not None and station_id != self.id:
-            # print(f"Id {station_id} does not equal station's id: {self.id}")
             return False
         if station_uuid is not None and station_uuid != self.uuid:
-            # print(f"Uuid {station_uuid} does not equal station's uuid: {self.uuid}")
             return False
-        if start_timestamp is not None and (start_timestamp != self.start_timestamp_micros
-                                            or np.isnan(start_timestamp) or np.isnan(self.start_timestamp_micros)):
-            # print(f"Start timestamp {start_timestamp} does not equal station's "
-            #       f"start timestamp: {self.start_timestamp_micros}")
+        if start_timestamp is not None and (
+            start_timestamp != self.start_timestamp_micros
+            or np.isnan(start_timestamp)
+            or np.isnan(self.start_timestamp_micros)
+        ):
             return False
         return True
 
     def compare_key(self, other_key: "StationKey") -> bool:
         """
         compare key to another station's key
 
@@ -136,26 +142,38 @@
         """
         return self.check_key(other_key.id, other_key.uuid, other_key.start_timestamp_micros)
 
 
 class StationMetadata:
     """
     A container for all the packet metadata consistent across all packets
+
     Properties:
         api: float, api version, default np.nan
+
         sub_api: float, sub api version, default np.nan
+
         make: str, station make, default empty string
+
         model: str, station model, default empty string
+
         os: OsType enum, station OS, default OsType.UNKNOWN_OS
+
         os_version: str, station OS version, default empty string
+
         app: str, station app, default empty string
+
         app_version: str, station app version, default empty string
+
         is_private: bool, is station data private, default False
+
         packet_duration_s: float, duration of the packet in seconds, default np.nan
+
         station_description: str, description of the station, default empty string
+
         other_metadata: dict, str: str of other metadata from the packet, default empty list
     """
 
     def __init__(self, app: str = "", packet: Optional[api_m.RedvoxPacketM] = None):
         """
         initialize the metadata
 
@@ -169,74 +187,75 @@
             self.sub_api = packet.sub_api
             self.make = packet.station_information.make
             self.model = packet.station_information.model
             self.os: OsType = OsType(packet.station_information.os)
             self.os_version = packet.station_information.os_version
             self.app_version = packet.station_information.app_version
             self.is_private = packet.station_information.is_private
-            self.packet_duration_s = (
-                    len(packet.sensors.audio.samples.values)
-                    / packet.sensors.audio.sample_rate
-            )
+            self.packet_duration_s = len(packet.sensors.audio.samples.values) / packet.sensors.audio.sample_rate
             self.station_description = packet.station_information.description
         else:
             self.api = np.nan
             self.sub_api = np.nan
             self.make = ""
             self.model = ""
             self.os: OsType = OsType["UNKNOWN_OS"]
             self.os_version = ""
             self.app_version = ""
             self.is_private = False
             self.packet_duration_s = np.nan
             self.station_description = ""
 
     def __repr__(self):
-        return f"app: {self.app}, " \
-               f"api: {self.api}, " \
-               f"sub_api: {self.sub_api}, " \
-               f"make: {self.make}, " \
-               f"model: {self.model}, " \
-               f"os: {self.os.value}, " \
-               f"os_version: {self.os_version}, " \
-               f"app_version: {self.app_version}, " \
-               f"is_private: {self.is_private}, " \
-               f"packet_duration_s: {self.packet_duration_s}, " \
-               f"station_description: {self.station_description}"
+        return (
+            f"app: {self.app}, "
+            f"api: {self.api}, "
+            f"sub_api: {self.sub_api}, "
+            f"make: {self.make}, "
+            f"model: {self.model}, "
+            f"os: {self.os.value}, "
+            f"os_version: {self.os_version}, "
+            f"app_version: {self.app_version}, "
+            f"is_private: {self.is_private}, "
+            f"packet_duration_s: {self.packet_duration_s}, "
+            f"station_description: {self.station_description}"
+        )
 
     def __str__(self):
-        return f"app: {self.app}, " \
-               f"api: {self.api}, " \
-               f"sub_api: {self.sub_api}, " \
-               f"make: {self.make}, " \
-               f"model: {self.model}, " \
-               f"os: {self.os.name}, " \
-               f"os_version: {self.os_version}, " \
-               f"app_version: {self.app_version}, " \
-               f"is_private: {self.is_private}, " \
-               f"packet_duration_s: {self.packet_duration_s}, " \
-               f"station_description: {self.station_description}"
+        return (
+            f"app: {self.app}, "
+            f"api: {self.api}, "
+            f"sub_api: {self.sub_api}, "
+            f"make: {self.make}, "
+            f"model: {self.model}, "
+            f"os: {self.os.name}, "
+            f"os_version: {self.os_version}, "
+            f"app_version: {self.app_version}, "
+            f"is_private: {self.is_private}, "
+            f"packet_duration_s: {self.packet_duration_s}, "
+            f"station_description: {self.station_description}"
+        )
 
     def validate_metadata(self, other_metadata: "StationMetadata") -> bool:
         """
         :param other_metadata: another StationMetadata object to compare
         :return: True if other_metadata is equal to the calling metadata
         """
         return (
-                self.app == other_metadata.app
-                and self.api == other_metadata.api
-                and self.sub_api == other_metadata.sub_api
-                and self.make == other_metadata.make
-                and self.model == other_metadata.model
-                and self.os == other_metadata.os
-                and self.os_version == other_metadata.os_version
-                and self.app_version == other_metadata.app_version
-                and self.is_private == other_metadata.is_private
-                and self.packet_duration_s == other_metadata.packet_duration_s
-                and self.station_description == other_metadata.station_description
+            self.app == other_metadata.app
+            and self.api == other_metadata.api
+            and self.sub_api == other_metadata.sub_api
+            and self.make == other_metadata.make
+            and self.model == other_metadata.model
+            and self.os == other_metadata.os
+            and self.os_version == other_metadata.os_version
+            and self.app_version == other_metadata.app_version
+            and self.is_private == other_metadata.is_private
+            and self.packet_duration_s == other_metadata.packet_duration_s
+            and self.station_description == other_metadata.station_description
         )
 
     def as_dict(self) -> dict:
         """
         :return: dictionary representation of the metadata
         """
         return {
@@ -247,15 +266,15 @@
             "model": self.model,
             "os": self.os.name,
             "os_version": self.os_version,
             "app_version": self.app_version,
             "is_private": self.is_private,
             "packet_duration_s": self.packet_duration_s,
             "station_description": self.station_description,
-            "other_metadata": self.other_metadata
+            "other_metadata": self.other_metadata,
         }
 
     @staticmethod
     def from_dict(md_dict: dict) -> "StationMetadata":
         """
         :param md_dict: metadata dictionary
         :return: StationMetadata from dictionary
@@ -304,55 +323,51 @@
         """
         initialize the metadata
 
         :param packet: Optional RedvoxPacketM to read data from
         """
         self.other_metadata = {}
         if packet:
-            self.packet_start_mach_timestamp = (
-                packet.timing_information.packet_start_mach_timestamp
-            )
-            self.packet_end_mach_timestamp = (
-                packet.timing_information.packet_end_mach_timestamp
-            )
-            self.packet_start_os_timestamp = (
-                packet.timing_information.packet_start_os_timestamp
-            )
-            self.packet_end_os_timestamp = (
-                packet.timing_information.packet_end_os_timestamp
-            )
+            self.packet_start_mach_timestamp = packet.timing_information.packet_start_mach_timestamp
+            self.packet_end_mach_timestamp = packet.timing_information.packet_end_mach_timestamp
+            self.packet_start_os_timestamp = packet.timing_information.packet_start_os_timestamp
+            self.packet_end_os_timestamp = packet.timing_information.packet_end_os_timestamp
             self.server_packet_receive_timestamp = packet.timing_information.server_acquisition_arrival_timestamp
             self.timing_info_score = packet.timing_information.score
             self.timing_score_method = TimingScoreMethod(packet.timing_information.score_method)
         else:
             self.packet_start_mach_timestamp = np.nan
             self.packet_end_mach_timestamp = np.nan
             self.packet_start_os_timestamp = np.nan
             self.packet_end_os_timestamp = np.nan
             self.server_packet_receive_timestamp = np.nan
             self.timing_info_score = np.nan
             self.timing_score_method = TimingScoreMethod["UNKNOWN"]
 
     def __repr__(self):
-        return f"packet_start_mach_timestamp: {self.packet_start_mach_timestamp}, " \
-               f"packet_end_mach_timestamp: {self.packet_end_mach_timestamp}, " \
-               f"packet_start_os_timestamp: {self.packet_start_os_timestamp}, " \
-               f"packet_end_os_timestamp: {self.packet_end_os_timestamp}, " \
-               f"server_packet_receive_timestamp: {self.server_packet_receive_timestamp}, " \
-               f"timing_info_score: {self.timing_info_score}, " \
-               f"timing_score_method: {self.timing_score_method.value}"
+        return (
+            f"packet_start_mach_timestamp: {self.packet_start_mach_timestamp}, "
+            f"packet_end_mach_timestamp: {self.packet_end_mach_timestamp}, "
+            f"packet_start_os_timestamp: {self.packet_start_os_timestamp}, "
+            f"packet_end_os_timestamp: {self.packet_end_os_timestamp}, "
+            f"server_packet_receive_timestamp: {self.server_packet_receive_timestamp}, "
+            f"timing_info_score: {self.timing_info_score}, "
+            f"timing_score_method: {self.timing_score_method.value}"
+        )
 
     def __str__(self):
-        return f"packet_start_mach_timestamp: {self.packet_start_mach_timestamp}, " \
-               f"packet_end_mach_timestamp: {self.packet_end_mach_timestamp}, " \
-               f"packet_start_os_timestamp: {self.packet_start_os_timestamp}, " \
-               f"packet_end_os_timestamp: {self.packet_end_os_timestamp}, " \
-               f"server_packet_receive_timestamp: {self.server_packet_receive_timestamp}, " \
-               f"timing_info_score: {self.timing_info_score}, " \
-               f"timing_score_method: {self.timing_score_method.name}"
+        return (
+            f"packet_start_mach_timestamp: {self.packet_start_mach_timestamp}, "
+            f"packet_end_mach_timestamp: {self.packet_end_mach_timestamp}, "
+            f"packet_start_os_timestamp: {self.packet_start_os_timestamp}, "
+            f"packet_end_os_timestamp: {self.packet_end_os_timestamp}, "
+            f"server_packet_receive_timestamp: {self.server_packet_receive_timestamp}, "
+            f"timing_info_score: {self.timing_info_score}, "
+            f"timing_score_method: {self.timing_score_method.name}"
+        )
 
     def update_timestamps(self, om: OffsetModel, use_model_function: bool = True):
         """
         updates the timestamps in the metadata using the offset model
 
         :param om: OffsetModel to apply to data
         :param use_model_function: if True, use the offset model's correction function to correct time,
@@ -384,15 +399,15 @@
             "packet_start_mach_timestamp": self.packet_start_mach_timestamp,
             "packet_end_mach_timestamp": self.packet_end_mach_timestamp,
             "packet_start_os_timestamp": self.packet_start_os_timestamp,
             "packet_end_os_timestamp": self.packet_end_os_timestamp,
             "server_packet_receive_timestamp": self.server_packet_receive_timestamp,
             "timing_info_score": self.timing_info_score,
             "timing_score_method": self.timing_score_method.name,
-            "other_metadata": self.other_metadata
+            "other_metadata": self.other_metadata,
         }
 
     @staticmethod
     def from_dict(pmd_dict: dict) -> "StationPacketMetadata":
         """
         :param pmd_dict: dictionary with StationPacketMetadata
         :return: StationPacketMetadata from dictionary
@@ -401,11 +416,11 @@
         result.other_metadata = pmd_dict["other_metadata"]
         result.packet_start_mach_timestamp = pmd_dict["packet_start_mach_timestamp"]
         result.packet_end_mach_timestamp = pmd_dict["packet_end_mach_timestamp"]
         result.packet_start_os_timestamp = pmd_dict["packet_start_os_timestamp"]
         result.packet_end_os_timestamp = pmd_dict["packet_end_os_timestamp"]
         result.server_packet_receive_timestamp = pmd_dict["server_packet_receive_timestamp"]
         result.timing_info_score = pmd_dict["timing_info_score"]
-        result.timing_score_method = TimingScoreMethod[pmd_dict["timing_score_method"]
-                                                       if "timing_score_method" in pmd_dict.keys()
-                                                       else "UNKNOWN"]
+        result.timing_score_method = TimingScoreMethod[
+            pmd_dict["timing_score_method"] if "timing_score_method" in pmd_dict.keys() else "UNKNOWN"
+        ]
         return result
```

### Comparing `redvox-3.4.2/redvox/common/stats_helper.py` & `redvox-3.5.0/redvox/common/stats_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,24 +6,28 @@
 from typing import List, Union
 
 import numpy as np
 
 
 class StatsContainer:
     """
-    Helper class to compute statistics for a set of objects
-    Stores the mean, std dev, number of data points (count), and best value per set object
+    Helper class to compute statistics for a set of objects.
+    Stores the mean, std dev, number of data points (count), and best value per set object.
     Calculates mean of means, mean of variance, variance of means, total variance,
     and total std dev for the set of objects
 
     Properties:
         mean_array: the mean of each object in the set
+
         std_dev_array: the std_dev of each object in the set
+
         count_array: the number of elements in each object in the set
+
         best_value: the best value to represent the set
+
         container_id: a string that identifies the StatsContainer
     """
 
     def __init__(self, container_id: str) -> None:
         """
         Initialize the StatsContainer
 
@@ -40,17 +44,15 @@
         :return: mean of all means
         """
         # convert non-numbers to 0s
         counts: np.ndarray = np.nan_to_num(self.count_array)
         if np.sum(counts) == 0:
             return np.nan
         # weight each mean by the number of elements in it
-        total_means: np.ndarray = np.prod(
-            [np.nan_to_num(self.mean_array), counts], axis=0
-        )
+        total_means: np.ndarray = np.prod([np.nan_to_num(self.mean_array), counts], axis=0)
         # if sum(counts) is 0, change sum(counts) to 1 to avoid divide by 0 errors
         return np.sum(total_means) / np.sum(counts)
 
     def mean_of_variance(self) -> float:
         """
         :return: mean of the variances
         """
@@ -68,17 +70,15 @@
         """
         :return: variance of the means
         """
         counts: np.ndarray = np.nan_to_num(self.count_array)
         if np.sum(counts) == 0:
             return np.nan
         # get the difference of individual means and total mean
-        mean_vars: np.ndarray = np.subtract(
-            np.nan_to_num(self.mean_array), self.mean_of_means()
-        )
+        mean_vars: np.ndarray = np.subtract(np.nan_to_num(self.mean_array), self.mean_of_means())
         # square the differences then weight them by number of elements
         total: np.ndarray = np.prod([mean_vars, mean_vars, counts], axis=0)
         # if sum(counts) is 0, change sum(counts) to 1 to avoid divide by 0 errors
         return np.sum(total) / np.sum(counts)
 
     def total_variance(self) -> float:
         """
```

### Comparing `redvox-3.4.2/redvox/common/timesync.py` & `redvox-3.5.0/redvox/common/timesync.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 Modules for extracting time synchronization statistics for API 900 and 1000 data.
-Currently uses API M packets due to versatility of the packet.
+Expects API M packets due to versatility of the packet.
 Also includes functions for correcting time arrays.
 ALL timestamps in microseconds unless otherwise stated
 """
 
 from functools import reduce
 from typing import List, Optional, Union
 from pathlib import Path
@@ -12,22 +12,21 @@
 
 # noinspection Mypy
 import numpy as np
 import pyarrow as pa
 import pyarrow.dataset as ds
 
 import redvox.common.timesync_io as io
+from redvox.common.io import json_file_to_dict
 import redvox.api900.lib.api900_pb2 as api900_pb2
 from redvox.api1000.proto.redvox_api_m_pb2 import RedvoxPacketM
 from redvox.api900.lib.api900_pb2 import RedvoxPacket
 import redvox.api900.reader_utils as util_900
 from redvox.common.offset_model import OffsetModel
-from redvox.common import (
-    tri_message_stats as tms,
-)
+from redvox.common import tri_message_stats as tms
 
 
 class TimeSync:
     """
     Stores latencies, offsets, and other timesync related information about a single station
     ALL timestamps in microseconds unless otherwise stated
     Timestamps are never updated from the raw values provided from the data
@@ -67,30 +66,30 @@
 
         _arrow_dir: str, directory to save arrow file in, default "." (current dir)
 
         _arrow_file: str, base name of file to save data as, default "timesync"
     """
 
     def __init__(
-            self,
-            time_sync_exchanges_list: Optional[List[float]] = None,
-            latencies: Optional[np.ndarray] = None,
-            best_latency: float = np.nan,
-            mean_latency: float = np.nan,
-            latency_std: float = np.nan,
-            offsets: Optional[np.ndarray] = None,
-            best_offset: float = 0.0,
-            mean_offset: float = np.nan,
-            offset_std: float = np.nan,
-            data_start: float = np.nan,
-            data_end: float = np.nan,
-            best_latency_index: int = np.nan,
-            best_array_index: int = 0,
-            arrow_dir: str = ".",
-            arrow_file_name: str = "timesync"
+        self,
+        time_sync_exchanges_list: Optional[List[float]] = None,
+        latencies: Optional[np.ndarray] = None,
+        best_latency: float = np.nan,
+        mean_latency: float = np.nan,
+        latency_std: float = np.nan,
+        offsets: Optional[np.ndarray] = None,
+        best_offset: float = 0.0,
+        mean_offset: float = np.nan,
+        offset_std: float = np.nan,
+        data_start: float = np.nan,
+        data_end: float = np.nan,
+        best_latency_index: int = np.nan,
+        best_array_index: int = 0,
+        arrow_dir: str = ".",
+        arrow_file_name: str = "timesync",
     ):
         """
         Initialize properties
 
         :param time_sync_exchanges_list: optional timesync exchanges of the packet as a flat list, default None
         :param latencies: optional arrays of latencies from exchanges; must be two equal length arrays, default None
         :param best_latency: the best latency of set, default np.nan
@@ -98,16 +97,16 @@
         :param latency_std: the standard deviation of all latencies, default np.nan
         :param offsets: optional arrays of offsets from exchanges; must be two equal length arrays, default None
         :param best_offset: the best offset of the packet, default 0.0
         :param mean_offset: the mean of all offsets, default np.nan
         :param offset_std: the standard deviation of all offsets, default np.nan
         :param data_start: the start timestamp of the data, default np.nan
         :param data_end: the end timestamp of the data, default np.nan
-        :param best_latency_index: index of best latency in latencies array, default np.nan
-        :param best_array_index: index of best latency array; must be either 1 (first array) or 3 (second array),
+        :param best_latency_index: index of the best latency in latencies array, default np.nan
+        :param best_array_index: index of the best latency array; must be either 1 (first array) or 3 (second array),
                                     any other value is invalid, default 0
         :param arrow_dir: directory to save timesync data in, default "."
         :param arrow_file_name: name of file to save timesync data as.  do not include extensions.  default "timesync"
         """
         self._latencies: np.ndarray = latencies
         self._best_latency: float = best_latency
         self._mean_latency: float = mean_latency
@@ -124,42 +123,45 @@
         self.arrow_file: str = arrow_file_name
 
         if time_sync_exchanges_list is None or len(time_sync_exchanges_list) < 1:
             self._time_sync_exchanges_list = [[], [], [], [], [], []]
             self._best_exchange_index_list = []
             self._offset_model: OffsetModel = OffsetModel.empty_model()
         else:
-            self._time_sync_exchanges_list = np.transpose([
-                time_sync_exchanges_list[i: i + 6]
-                for i in range(0, len(time_sync_exchanges_list), 6)
-            ])
+            self._time_sync_exchanges_list = np.transpose(
+                [time_sync_exchanges_list[i : i + 6] for i in range(0, len(time_sync_exchanges_list), 6)]
+            )
             if self._latencies is None:
                 if not np.isnan(self._data_start):
                     self._data_start = self.get_exchange_timestamps(4)[0]
                 if not np.isnan(self._data_end):
                     self._data_end = self.get_exchange_timestamps(5)[-1]
                 self._stats_from_exchanges()
 
     def __repr__(self):
-        return f"best_latency_index: {self._best_latency_index}, " \
-               f"best_latency: {self._best_latency}, " \
-               f"mean_latency: {self._mean_latency}, " \
-               f"latency_std: {self._latency_std}, " \
-               f"best_offset: {self._best_offset}, " \
-               f"mean_offset: {self._mean_offset}, " \
-               f"offset_std: {self._offset_std}"
+        return (
+            f"best_latency_index: {self._best_latency_index}, "
+            f"best_latency: {self._best_latency}, "
+            f"mean_latency: {self._mean_latency}, "
+            f"latency_std: {self._latency_std}, "
+            f"best_offset: {self._best_offset}, "
+            f"mean_offset: {self._mean_offset}, "
+            f"offset_std: {self._offset_std}"
+        )
 
     def __str__(self):
-        return f"best_latency_index: {self._best_latency_index}, " \
-               f"best_latency: {self._best_latency}, " \
-               f"mean_latency: {self._mean_latency}, " \
-               f"latency_std: {self._latency_std}, " \
-               f"best_offset: {self._best_offset}, " \
-               f"mean_offset: {self._mean_offset}, " \
-               f"offset_std: {self._offset_std}"
+        return (
+            f"best_latency_index: {self._best_latency_index}, "
+            f"best_latency: {self._best_latency}, "
+            f"mean_latency: {self._mean_latency}, "
+            f"latency_std: {self._latency_std}, "
+            f"best_offset: {self._best_offset}, "
+            f"mean_offset: {self._mean_offset}, "
+            f"offset_std: {self._offset_std}"
+        )
 
     def as_dict(self) -> dict:
         """
         :return: TimeSync as a dictionary
         """
         return {
             "best_latency_index": self._best_latency_index,
@@ -169,15 +171,15 @@
             "latency_std": self._latency_std,
             "best_offset": self._best_offset,
             "mean_offset": self._mean_offset,
             "offset_std": self._offset_std,
             "data_start": self._data_start,
             "data_end": self._data_end,
             "arrow_dir": self.arrow_dir,
-            "arrow_file_name": self.arrow_file
+            "arrow_file_name": self.arrow_file,
         }
 
     def to_json(self):
         """
         :return: TimeSync as json string
         """
         return io.to_json(self)
@@ -197,25 +199,47 @@
     def from_json_file(file_path: str) -> "TimeSync":
         """
         convert contents of json file to TimeSync data
 
         :param file_path: full path of file to load data from.
         :return: TimeSyncArrow object
         """
-        json_data = io.json_file_to_dict(file_path)
-        data = ds.dataset(os.path.join(json_data["arrow_dir"], json_data["arrow_file_name"] + ".parquet"),
-                          format="parquet", exclude_invalid_files=True).to_table()
-        result = TimeSync(None, np.array((data["latencies1"], data["latencies3"])),
-                          json_data["best_latency"], json_data["mean_latency"], json_data["latency_std"],
-                          np.array((data["offsets1"], data["offsets3"])),
-                          json_data["best_offset"], json_data["mean_offset"], json_data["offset_std"],
-                          json_data["data_start"], json_data["data_end"], json_data["best_latency_index"],
-                          json_data["best_msg_array_index"], json_data["arrow_dir"], json_data["arrow_file_name"])
-        result.set_sync_exchanges([data["a1"].to_numpy(), data["a2"].to_numpy(), data["a3"].to_numpy(),
-                                   data["b1"].to_numpy(), data["b2"].to_numpy(), data["b3"].to_numpy()])
+        json_data = json_file_to_dict(file_path)
+        data = ds.dataset(
+            os.path.join(json_data["arrow_dir"], json_data["arrow_file_name"] + ".parquet"),
+            format="parquet",
+            exclude_invalid_files=True,
+        ).to_table()
+        result = TimeSync(
+            None,
+            np.array((data["latencies1"], data["latencies3"])),
+            json_data["best_latency"],
+            json_data["mean_latency"],
+            json_data["latency_std"],
+            np.array((data["offsets1"], data["offsets3"])),
+            json_data["best_offset"],
+            json_data["mean_offset"],
+            json_data["offset_std"],
+            json_data["data_start"],
+            json_data["data_end"],
+            json_data["best_latency_index"],
+            json_data["best_msg_array_index"],
+            json_data["arrow_dir"],
+            json_data["arrow_file_name"],
+        )
+        result.set_sync_exchanges(
+            [
+                data["a1"].to_numpy(),
+                data["a2"].to_numpy(),
+                data["a3"].to_numpy(),
+                data["b1"].to_numpy(),
+                data["b2"].to_numpy(),
+                data["b3"].to_numpy(),
+            ]
+        )
         return result
 
     @staticmethod
     def from_dict(ts_dict: dict, tse_data: List) -> "TimeSync":
         """
         create TimeSync frp, dictionary
 
@@ -225,26 +249,28 @@
         """
         return TimeSync(tse_data, ts_dict["best_latency"], ts_dict["best_offset"])
 
     def data_as_pyarrow(self) -> pa.Table:
         """
         :return: convert timesync exchanges, latencies, and offsets into a pyarrow table
         """
-        return pa.Table.from_pydict({
-            "a1": self._time_sync_exchanges_list[0],
-            "a2": self._time_sync_exchanges_list[1],
-            "a3": self._time_sync_exchanges_list[2],
-            "b1": self._time_sync_exchanges_list[3],
-            "b2": self._time_sync_exchanges_list[4],
-            "b3": self._time_sync_exchanges_list[5],
-            "latencies1": self._latencies[0],
-            "latencies3": self._latencies[1],
-            "offsets1": self._offsets[0],
-            "offsets3": self._offsets[1]
-        })
+        return pa.Table.from_pydict(
+            {
+                "a1": self._time_sync_exchanges_list[0],
+                "a2": self._time_sync_exchanges_list[1],
+                "a3": self._time_sync_exchanges_list[2],
+                "b1": self._time_sync_exchanges_list[3],
+                "b2": self._time_sync_exchanges_list[4],
+                "b3": self._time_sync_exchanges_list[5],
+                "latencies1": self._latencies[0],
+                "latencies3": self._latencies[1],
+                "offsets1": self._offsets[0],
+                "offsets3": self._offsets[1],
+            }
+        )
 
     def _stats_from_exchanges(self):
         """
         Compute the tri-message stats from the data
         """
         if self.num_tri_messages() < 1:
             self._latencies = np.array(([], []))
@@ -269,17 +295,21 @@
                 np.array(self._time_sync_exchanges_list[3]),
                 np.array(self._time_sync_exchanges_list[4]),
                 np.array(self._time_sync_exchanges_list[5]),
             )
             self._latencies = np.array((tse.latency1, tse.latency3))
             self._offsets = np.array((tse.offset1, tse.offset3))
             if not np.isnan(self._data_start) and not np.isnan(self._data_end):
-                self._offset_model = OffsetModel(self._latencies.flatten(), self._offsets.flatten(),
-                                                 self.get_device_exchanges_timestamps(),
-                                                 self._data_start, self._data_end)
+                self._offset_model = OffsetModel(
+                    self._latencies.flatten(),
+                    self._offsets.flatten(),
+                    self.get_device_exchanges_timestamps(),
+                    self._data_start,
+                    self._data_end,
+                )
                 # Compute the statistics for latency using the model
                 self._mean_latency = self._offset_model.mean_latency
                 self._latency_std = self._offset_model.std_dev_latency
             else:
                 self._offset_model = OffsetModel.empty_model()
                 # Compute the statistics for latency using the exchanges
                 self._mean_latency = np.mean([*self._latencies[0], *self._latencies[1]])
@@ -337,37 +367,43 @@
 
     def append_timesync_arrow(self, new_data: "TimeSync"):
         """
         adds timesync data from new_data to current
 
         :param new_data: another TimeSyncArrow object
         """
-        self._time_sync_exchanges_list[0] = np.append(self._time_sync_exchanges_list[0],
-                                                      new_data._time_sync_exchanges_list[0])
-        self._time_sync_exchanges_list[1] = np.append(self._time_sync_exchanges_list[1],
-                                                      new_data._time_sync_exchanges_list[1])
-        self._time_sync_exchanges_list[2] = np.append(self._time_sync_exchanges_list[2],
-                                                      new_data._time_sync_exchanges_list[2])
-        self._time_sync_exchanges_list[3] = np.append(self._time_sync_exchanges_list[3],
-                                                      new_data._time_sync_exchanges_list[3])
-        self._time_sync_exchanges_list[4] = np.append(self._time_sync_exchanges_list[4],
-                                                      new_data._time_sync_exchanges_list[4])
-        self._time_sync_exchanges_list[5] = np.append(self._time_sync_exchanges_list[5],
-                                                      new_data._time_sync_exchanges_list[5])
+        self._time_sync_exchanges_list[0] = np.append(
+            self._time_sync_exchanges_list[0], new_data._time_sync_exchanges_list[0]
+        )
+        self._time_sync_exchanges_list[1] = np.append(
+            self._time_sync_exchanges_list[1], new_data._time_sync_exchanges_list[1]
+        )
+        self._time_sync_exchanges_list[2] = np.append(
+            self._time_sync_exchanges_list[2], new_data._time_sync_exchanges_list[2]
+        )
+        self._time_sync_exchanges_list[3] = np.append(
+            self._time_sync_exchanges_list[3], new_data._time_sync_exchanges_list[3]
+        )
+        self._time_sync_exchanges_list[4] = np.append(
+            self._time_sync_exchanges_list[4], new_data._time_sync_exchanges_list[4]
+        )
+        self._time_sync_exchanges_list[5] = np.append(
+            self._time_sync_exchanges_list[5], new_data._time_sync_exchanges_list[5]
+        )
         if np.isnan(self._data_start):
             self._data_start = new_data._data_start
         elif not np.isnan(new_data._data_start):
             self._data_start = np.min([self._data_start, new_data._data_start])
         if np.isnan(self._data_end):
             self._data_end = new_data._data_end
         elif not np.isnan(new_data._data_end):
             self._data_end = np.max([self._data_end, new_data._data_end])
         self._stats_from_exchanges()
 
-    def from_raw_packets(self, packets: List[Union[RedvoxPacketM, RedvoxPacket]]) -> 'TimeSync':
+    def from_raw_packets(self, packets: List[Union[RedvoxPacketM, RedvoxPacket]]) -> "TimeSync":
         """
         converts packets into TimeSyncData objects, then performs analysis
 
         :param packets: list of RedvoxPacketM and RedvoxPacket to convert
         :return: modified version of self
         """
         all_exchanges: List[float] = []
@@ -379,28 +415,32 @@
             self._data_end = packets[-1].timing_information.packet_end_mach_timestamp
         else:
             self._data_end = packets[-1].app_file_start_timestamp_machine
 
         packet: Union[RedvoxPacketM, RedvoxPacket]
         for packet in packets:
             if isinstance(packet, RedvoxPacketM):
-                all_exchanges.extend(reduce(lambda acc, ex: acc + [ex.a1, ex.a2, ex.a3, ex.b1, ex.b2, ex.b3],
-                                            packet.timing_information.synch_exchanges,
-                                            []))
+                all_exchanges.extend(
+                    reduce(
+                        lambda acc, ex: acc + [ex.a1, ex.a2, ex.a3, ex.b1, ex.b2, ex.b3],
+                        packet.timing_information.synch_exchanges,
+                        [],
+                    )
+                )
             else:
                 # Get synch exchanges
                 ch: api900_pb2.UnevenlySampledChannel
                 for ch in packet.unevenly_sampled_channels:
                     if api900_pb2.TIME_SYNCHRONIZATION in ch.channel_types:
                         all_exchanges.extend(util_900.extract_payload(ch))
 
         if len(all_exchanges) > 0:
-            self._time_sync_exchanges_list = np.transpose([
-                all_exchanges[i: i + 6] for i in range(0, len(all_exchanges), 6)
-            ])
+            self._time_sync_exchanges_list = np.transpose(
+                [all_exchanges[i : i + 6] for i in range(0, len(all_exchanges), 6)]
+            )
             self._stats_from_exchanges()
         return self
 
     def sync_exchanges(self) -> np.ndarray:
         """
         :return: time sync exchanges
         """
@@ -438,15 +478,15 @@
         """
         :return: standard deviation of latency
         """
         return self._latency_std
 
     def best_latency_index(self) -> int:
         """
-        :return: index/position of best latency or np.nan if no best latency exists
+        :return: index/position of the best latency or np.nan if no best latency exists
         """
         return self._best_latency_index
 
     def best_latency_per_exchange(self) -> np.array:
         """
         :return: the best latency per sync exchange as a numpy array
         """
```

### Comparing `redvox-3.4.2/redvox/common/timesync_io.py` & `redvox-3.5.0/redvox/common/timesync_io.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,41 @@
 """
 This module provides IO primitives for working with timesync data.
 """
 from pathlib import Path
 import json
 from typing import (
-    Dict,
     Optional,
     TYPE_CHECKING,
 )
 
-from redvox.common.io import json_file_to_dict
-
 import pyarrow.parquet as pq
 
 
 if TYPE_CHECKING:
     from redvox.common.timesync import TimeSync
 
 
-def to_json(timesync: "TimeSync",) -> str:
+def to_json(
+    timesync: "TimeSync",
+) -> str:
     """
     :return: timesync as json string
     """
     return json.dumps(timesync.as_dict())
 
 
-def to_json_file(timesync: "TimeSync",
-                 file_name: Optional[str] = None) -> Path:
+def to_json_file(timesync: "TimeSync", file_name: Optional[str] = None) -> Path:
     """
     saves the timesync as json and data in the same directory.
 
     :param timesync: TimeSync to save
     :param file_name: the optional base file name.  Do not include a file extension.
                         If None, uses the timesync's file name.
     :return: path to json file
     """
-    _file_name: str = (
-        file_name
-        if file_name is not None
-        else timesync.arrow_file
-    )
+    _file_name: str = file_name if file_name is not None else timesync.arrow_file
     file_path: Path = Path(timesync.arrow_dir).joinpath(f"{_file_name}.json")
-    pq.write_table(timesync.data_as_pyarrow(),
-                   Path(timesync.arrow_dir).joinpath(f"{_file_name}.parquet"))
+    pq.write_table(timesync.data_as_pyarrow(), Path(timesync.arrow_dir).joinpath(f"{_file_name}.parquet"))
     with open(file_path, "w") as f_p:
         f_p.write(to_json(timesync))
         return file_path.resolve(False)
```

### Comparing `redvox-3.4.2/redvox/common/tri_message_stats.py` & `redvox-3.5.0/redvox/common/tri_message_stats.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,27 +11,39 @@
 # noinspection Mypy
 import numpy as np
 
 
 class TriMessageStats:
     """
     Stores statistics about the tri-message exchanges
+
     ALL timestamps in microseconds
+
     Properties:
         packet_id: an identifier for the packet that contains the data.  Used for reporting purposes
+
         latency1: latencies measured by timestamps 1 and 2
+
         latency3: latencies measured by timestamps 2 and 3
+
         offset1: offsets measured by timestamps 1 and 2
+
         offset3: offsets measured by timestamps 2 and 3
+
         best_latency: minimum latency that meets all criteria, default np.nan
+
         best_offset: best offset that meets all criteria, default 0.0
+
         best_latency_array_index: index of which latency array has the best latency, valid values are either 1 or 3,
                                     all other values are invalid, default 0
-        best_latency_index: index in latency array with best latency, default None
+
+        best_latency_index: index in latency array with the best latency, default None
+
         best_latency_per_exchange_index_array: the index of which latency array has the best latency, per each exchange
+
         num_messages: number of tri-message exchanges
     """
 
     def __init__(
         self,
         packet_id: Union[str, int],
         a1: np.ndarray,
@@ -51,17 +63,15 @@
         :param b1: array of device timestamp 1
         :param b2: array of device timestamp 2
         :param b3: array of device timestamp 3
         """
         self.packet_id: Union[str, int] = packet_id
         self.num_messages: int = len(a1)
         # compute latencies and offsets
-        latencies_tuple: Tuple[np.ndarray, np.ndarray] = latencies(
-            a1, a2, a3, b1, b2, b3
-        )
+        latencies_tuple: Tuple[np.ndarray, np.ndarray] = latencies(a1, a2, a3, b1, b2, b3)
         self.latency1: np.ndarray = latencies_tuple[0]
         self.latency3: np.ndarray = latencies_tuple[1]
         offsets_tuple: Tuple[np.ndarray, np.ndarray] = offsets(a1, a2, a3, b1, b2, b3)
         self.offset1: np.ndarray = offsets_tuple[0]
         self.offset3: np.ndarray = offsets_tuple[1]
 
         self.best_latency: float = np.nan
@@ -71,15 +81,15 @@
 
         self.find_best_latency()
         self.find_best_offset()
         self.best_latency_per_exchange_index_array: List[int] = self.find_best_exchange_latencies_index()
 
     def find_best_latency(self) -> None:
         """
-        Finds the best latency among the latencies
+        Finds and sets the best latency among the latencies.  Update is done in place, nothing is returned.
         """
         if all(np.nan_to_num(self.latency1) == 0.0) or all(np.nan_to_num(self.latency3) == 0.0):
             # all latencies for one of the arrays is zero, the data is untrustworthy.  set the defaults
             self.best_latency = np.nan
             self.best_latency_array_index = None
             self.best_latency_index = None
         else:
@@ -94,20 +104,18 @@
             else:
                 self.best_latency = d3_min
                 self.best_latency_array_index = 3
                 self.best_latency_index = int(np.where(self.latency3 == d3_min)[0][0])
 
     def find_best_offset(self) -> None:
         """
-        Finds the best offset among the offsets
+        Finds and sets the best offset among the offsets.  Update is done in place, nothing is returned.
         """
-        # if no best latency, find it
         if self.best_latency is None:
             self.find_best_latency()
-        # best latency = best offset, if best latency is still None, best offset is 0.0
         if self.best_latency_array_index == 1:
             self.best_offset = self.offset1[self.best_latency_index]
         elif self.best_latency_array_index == 3:
             self.best_offset = self.offset3[self.best_latency_index]
         else:
             self.best_offset = 0.0
 
@@ -123,74 +131,69 @@
         a2_coeffs: np.ndarray,
         a3_coeffs: np.ndarray,
         b1_coeffs: np.ndarray,
         b2_coeffs: np.ndarray,
         b3_coeffs: np.ndarray,
     ) -> None:
         """
-        set the latency and find the best latency
+        set the latency, then find the best latency.  Update is done in place, nothing is returned.
 
-        :param a1_coeffs: server timestamp 1
-        :param a2_coeffs: server timestamp 2
-        :param a3_coeffs: server timestamp 3
-        :param b1_coeffs: device timestamp 1
-        :param b2_coeffs: device timestamp 2
-        :param b3_coeffs: device timestamp 3
+        :param a1_coeffs: server timestamps 1
+        :param a2_coeffs: server timestamps 2
+        :param a3_coeffs: server timestamps 3
+        :param b1_coeffs: device timestamps 1
+        :param b2_coeffs: device timestamps 2
+        :param b3_coeffs: device timestamps 3
         """
         # compute latencies
-        self.latency1, self.latency3 = latencies(
-            a1_coeffs, a2_coeffs, a3_coeffs, b1_coeffs, b2_coeffs, b3_coeffs
-        )
+        self.latency1, self.latency3 = latencies(a1_coeffs, a2_coeffs, a3_coeffs, b1_coeffs, b2_coeffs, b3_coeffs)
         self.find_best_latency()
 
     def set_offset(
         self,
         a1_coeffs: np.ndarray,
         a2_coeffs: np.ndarray,
         a3_coeffs: np.ndarray,
         b1_coeffs: np.ndarray,
         b2_coeffs: np.ndarray,
         b3_coeffs: np.ndarray,
     ) -> None:
         """
-        set the offset and find the best offset
+        set the offset then find the best offset.  Update is done in place, nothing is returned.
 
-        :param a1_coeffs: server timestamp 1
-        :param a2_coeffs: server timestamp 2
-        :param a3_coeffs: server timestamp 3
-        :param b1_coeffs: device timestamp 1
-        :param b2_coeffs: device timestamp 2
-        :param b3_coeffs: device timestamp 3
-        """
-        # compute offsets
-        self.offset1, self.offset3 = offsets(
-            a1_coeffs, a2_coeffs, a3_coeffs, b1_coeffs, b2_coeffs, b3_coeffs
-        )
+        :param a1_coeffs: server timestamps 1
+        :param a2_coeffs: server timestamps 2
+        :param a3_coeffs: server timestamps 3
+        :param b1_coeffs: device timestamps 1
+        :param b2_coeffs: device timestamps 2
+        :param b3_coeffs: device timestamps 3
+        """
+        self.offset1, self.offset3 = offsets(a1_coeffs, a2_coeffs, a3_coeffs, b1_coeffs, b2_coeffs, b3_coeffs)
         self.find_best_offset()
 
 
 def latencies(
     a1_coeffs: np.ndarray,
     a2_coeffs: np.ndarray,
     a3_coeffs: np.ndarray,
     b1_coeffs: np.ndarray,
     b2_coeffs: np.ndarray,
     b3_coeffs: np.ndarray,
 ) -> Tuple[np.ndarray, np.ndarray]:
     """
     Compute latencies in microseconds based on message exchange timestamps.
 
-    Parameters
-    ----------
-    a1_coeffs, ... b3_coeffs: tri-message timestamps as loaded in transmit_receive_timestamps_microsec
-
-    Returns
-    -------
-    d1_coeffs: array of server round trip latencies in microseconds
-    d3_coeffs: array of device round trip latencies in microseconds
+    :param a1_coeffs: server timestamps 1
+    :param a2_coeffs: server timestamps 2
+    :param a3_coeffs: server timestamps 3
+    :param b1_coeffs: device timestamps 1
+    :param b2_coeffs: device timestamps 2
+    :param b3_coeffs: device timestamps 3
+    :return: tuple of nd.arrays; the array of server round trip latencies in microseconds and
+                the array of device round trip latencies in microseconds
     """
     # Compute latencies in microseconds
     d1_coeffs: np.ndarray = 0.5 * ((a2_coeffs - a1_coeffs) - (b2_coeffs - b1_coeffs))
     d3_coeffs: np.ndarray = 0.5 * ((b3_coeffs - b2_coeffs) - (a3_coeffs - a2_coeffs))
 
     # convert negative latencies to nan.  negative latencies should not exist naturally
     d1_coeffs[d1_coeffs < 0] = np.nan
@@ -206,42 +209,31 @@
     b1_coeffs: np.ndarray,
     b2_coeffs: np.ndarray,
     b3_coeffs: np.ndarray,
 ) -> Tuple[np.ndarray, np.ndarray]:
     """
     Compute offsets in microseconds based on message exchange timestamps.
 
-    Parameters
-    ----------
-    a1_coeffs, ... b3_coeffs: tri-message timestamps as loaded in transmit_receive_timestamps_microsec
-
-    Returns
-    -------
-    o1_coeffs: array of server round trip latencies in microseconds
-    o3_coeffs: array of device round trip latencies in microseconds
+    :param a1_coeffs: server timestamps 1
+    :param a2_coeffs: server timestamps 2
+    :param a3_coeffs: server timestamps 3
+    :param b1_coeffs: device timestamps 1
+    :param b2_coeffs: device timestamps 2
+    :param b3_coeffs: device timestamps 3
+    :return: tuple of nd.arrays; the array of server round trip offsets in microseconds and
+                the array of device round trip offsets in microseconds
     """
     # assume the generic equation f = a - b + d
     # where d is latency, f is offset, b is machine time and a is time sync server time
     # refer to latency equations above for definitions of d1_coeffs and d3_coeffs
     # with latency d1_coeffs, the equation is f1 = a1_coeffs - b1_coeffs + d1_coeffs
     # with latency d3_coeffs, the equation is f3 = a3_coeffs - b3_coeffs + d3_coeffs
     # In the absence of latency, offset can be calculated this way:
-    # o1_coeffs = (a1_coeffs - b1_coeffs + a2_coeffs - b2_coeffs) / 2.
-    # o3_coeffs = (a3_coeffs - b3_coeffs + a2_coeffs - b2_coeffs) / 2.
-    # get latencies
-    # latencies_tuple: Tuple[np.ndarray, np.ndarray] = latencies(
-    #    a1_coeffs, a2_coeffs, a3_coeffs, b1_coeffs, b2_coeffs, b3_coeffs
-    # )
-    # d1_coeffs: np.ndarray = latencies_tuple[0]
-    # d3_coeffs: np.ndarray = latencies_tuple[1]
-    # use latency to compute offset in microseconds
-    # o1_coeffs: np.ndarray = a1_coeffs - b1_coeffs + d1_coeffs
-    o1_coeffs: np.ndarray = (a1_coeffs - b1_coeffs + a2_coeffs - b2_coeffs) / 2
-    o3_coeffs: np.ndarray = (a3_coeffs - b3_coeffs + a2_coeffs - b2_coeffs) / 2
-    # o3_coeffs: np.ndarray = a3_coeffs - b3_coeffs + d3_coeffs
+    o1_coeffs: np.ndarray = (a1_coeffs - b1_coeffs + a2_coeffs - b2_coeffs) / 2.0
+    o3_coeffs: np.ndarray = (a3_coeffs - b3_coeffs + a2_coeffs - b2_coeffs) / 2.0
 
     return o1_coeffs, o3_coeffs
 
 
 def validate_timestamps(
     a1_coeffs: np.ndarray,
     a2_coeffs: np.ndarray,
@@ -250,23 +242,21 @@
     b2_coeffs: np.ndarray,
     b3_coeffs: np.ndarray,
 ) -> Tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray]:
     """
     it's possible some of the tri-message values are duplicated; the duplicates and other invalid times
     must be removed.
 
-       Parameters
-       -------
-       a1_coeffs, a2_coeffs, a3_coeffs, b1_coeffs, b2_coeffs, b3_coeffs: arrays of message exchange timestamps
-
-       Returns
-       -------
-       a1_coeffs[valid_indices], a2_coeffs[valid_indices], a3_coeffs[valid_indices],
-       b1_coeffs[valid_indices], b2_coeffs[valid_indices], b3_coeffs[valid_indices]:
-       arrays of valid message exchange timestamps
+    :param a1_coeffs: server timestamps 1
+    :param a2_coeffs: server timestamps 2
+    :param a3_coeffs: server timestamps 3
+    :param b1_coeffs: device timestamps 1
+    :param b2_coeffs: device timestamps 2
+    :param b3_coeffs: device timestamps 3
+    :return: tuple of 6 ndarrays; each array will be the same length and contain only valid entries in the exchanges.
     """
     num_timestamps = len(a1_coeffs)
     # if length is 1 or less, no need to validate, just return all the values
     if num_timestamps <= 1:
         return a1_coeffs, a2_coeffs, a3_coeffs, b1_coeffs, b2_coeffs, b3_coeffs
     # if here, there's more than 1 exchange to check
     valid_times: List[Dict] = [{}, {}, {}, {}, {}, {}]
@@ -318,38 +308,24 @@
 
     Returns
     -------
     a1_coeffs, a2_coeffs, a3_coeffs, b1_coeffs, b2_coeffs, b3_coeffs: arrays of message exchange timestamps
     """
 
     if len(coeffs) % 6 != 0:
-        raise Exception(
-            "Tri-Message contains partial exchange, unsafe to use it for computations."
-        )
+        raise Exception("Tri-Message contains partial exchange, unsafe to use it for computations.")
 
     # Timing coefficients
     step: int = 6  # each tri-message exchange contains 6 timestamps, 3 from server and 3 from device
     stop: int = int(len(coeffs) / 6) * step
 
-    a1_coeffs: np.ndarray = coeffs[
-        0:stop:step
-    ]  # server first transmit timestamps in epoch microseconds
-    a2_coeffs: np.ndarray = coeffs[
-        1:stop:step
-    ]  # server first receive timestamps in epoch microseconds
-    a3_coeffs: np.ndarray = coeffs[
-        2:stop:step
-    ]  # server second transmit timestamps in epoch microseconds
-    b1_coeffs: np.ndarray = coeffs[
-        3:stop:step
-    ]  # device first receive timestamps in mach microseconds
-    b2_coeffs: np.ndarray = coeffs[
-        4:stop:step
-    ]  # device first transmit timestamps in mach microseconds
-    b3_coeffs: np.ndarray = coeffs[
-        5:stop:step
-    ]  # device second receive timestamps in mach microseconds
+    a1_coeffs: np.ndarray = coeffs[0:stop:step]  # server first transmit timestamps in epoch microseconds
+    a2_coeffs: np.ndarray = coeffs[1:stop:step]  # server first receive timestamps in epoch microseconds
+    a3_coeffs: np.ndarray = coeffs[2:stop:step]  # server second transmit timestamps in epoch microseconds
+    b1_coeffs: np.ndarray = coeffs[3:stop:step]  # device first receive timestamps in mach microseconds
+    b2_coeffs: np.ndarray = coeffs[4:stop:step]  # device first transmit timestamps in mach microseconds
+    b3_coeffs: np.ndarray = coeffs[5:stop:step]  # device second receive timestamps in mach microseconds
 
     # make sure each tri-message exchange contains 6 timestamps (done with modulo check above)
     # assert len(a1_coeffs) == len(a2_coeffs) == len(a3_coeffs) == len(b1_coeffs) == len(b2_coeffs) == len(b3_coeffs)
 
     return a1_coeffs, a2_coeffs, a3_coeffs, b1_coeffs, b2_coeffs, b3_coeffs
```

### Comparing `redvox-3.4.2/redvox/common/versioning.py` & `redvox-3.5.0/redvox/common/versioning.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox/settings.py` & `redvox-3.5.0/redvox/settings.py`

 * *Files identical despite different names*

### Comparing `redvox-3.4.2/redvox.egg-info/PKG-INFO` & `redvox-3.5.0/redvox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redvox
-Version: 3.4.2
+Version: 3.5.0
 Summary: Library for working with RedVox files. 
 Author-email: "RedVox, Inc" <support@redvox.io>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `redvox-3.4.2/redvox.egg-info/SOURCES.txt` & `redvox-3.5.0/redvox.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 redvox/api1000/common/typing.py
 redvox/api1000/gui/__init__.py
 redvox/api1000/gui/image_viewer.py
 redvox/api1000/proto/__init__.py
 redvox/api1000/proto/redvox_api_m_pb2.py
 redvox/api1000/wrapped_redvox_packet/__init__.py
 redvox/api1000/wrapped_redvox_packet/event_streams.py
+redvox/api1000/wrapped_redvox_packet/ml.py
 redvox/api1000/wrapped_redvox_packet/station_information.py
 redvox/api1000/wrapped_redvox_packet/timing_information.py
 redvox/api1000/wrapped_redvox_packet/wrapped_packet.py
 redvox/api1000/wrapped_redvox_packet/sensors/__init__.py
 redvox/api1000/wrapped_redvox_packet/sensors/audio.py
 redvox/api1000/wrapped_redvox_packet/sensors/image.py
 redvox/api1000/wrapped_redvox_packet/sensors/location.py
@@ -87,14 +88,15 @@
 redvox/cloud/data_api.py
 redvox/cloud/data_client.py
 redvox/cloud/data_io.py
 redvox/cloud/errors.py
 redvox/cloud/metadata_api.py
 redvox/cloud/query_timing_correction.py
 redvox/cloud/routes.py
+redvox/cloud/session_model_api.py
 redvox/cloud/station_stats.py
 redvox/cloud/subscription.py
 redvox/common/__init__.py
 redvox/common/api_conversions.py
 redvox/common/api_reader.py
 redvox/common/api_reader_dw.py
 redvox/common/constants.py
```

