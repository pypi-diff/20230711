# Comparing `tmp/joulescope-1.1.7.tar.gz` & `tmp/joulescope-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joulescope-1.1.7.tar", last modified: Thu Jun  8 17:52:09 2023, max compression
+gzip compressed data, was "joulescope-1.1.8.tar", last modified: Tue Jul 11 19:52:50 2023, max compression
```

## Comparing `joulescope-1.1.7.tar` & `joulescope-1.1.8.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:52:09.964017 joulescope-1.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    21223 2023-06-08 17:51:51.000000 joulescope-1.1.7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-06-08 17:51:51.000000 joulescope-1.1.7/CREDITS.html
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-08 17:51:51.000000 joulescope-1.1.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-08 17:51:51.000000 joulescope-1.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-06-08 17:52:09.964017 joulescope-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-08 17:51:51.000000 joulescope-1.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:52:09.944017 joulescope-1.1.7/joulescope/
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53690 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/data_recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)    25692 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/datafile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:52:09.948017 joulescope-1.1.7/joulescope/entry_points/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/entry_points/bootloader_go.py
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/entry_points/capture.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/entry_points/gpo_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/entry_points/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/entry_points/parameter_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/entry_points/program.py
--rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/entry_points/recording.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/entry_points/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/entry_points/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/entry_points/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/entry_points/stream_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/file_replace.py
--rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/jls_v2_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10713 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/parameters_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/span.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/stream_buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:52:09.948017 joulescope-1.1.7/joulescope/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15919 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/test/test_data_recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/test/test_data_recorder_downsampled.py
--rw-r--r--   0 runner    (1001) docker     (123)    10576 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/test/test_datafile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/test/test_file_replace.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/test/test_jls_v2_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/test/test_span.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/test/test_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/test/test_units.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:52:09.952017 joulescope-1.1.7/joulescope/v0/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v0/array_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    12239 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v0/bootloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v0/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)    85459 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v0/decimators.py
--rw-r--r--   0 runner    (1001) docker     (123)    56561 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v0/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)   960153 2023-06-08 17:52:06.000000 joulescope-1.1.7/joulescope/v0/filter_fir.c
--rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v0/firmware_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:52:09.956017 joulescope-1.1.7/joulescope/v0/native/
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v0/native/filter_fir.c
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v0/native/filter_fir.h
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v0/native/running_statistics.c
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v0/native/running_statistics.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:52:09.956017 joulescope-1.1.7/joulescope/v0/native/test/
--rw-r--r--   0 runner    (1001) docker     (123)    55447 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v0/native/test/acutest.h
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v0/native/test/test_filter_fir.c
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v0/notification_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)   436718 2023-06-08 17:52:06.000000 joulescope-1.1.7/joulescope/v0/pattern_buffer.c
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v0/public_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)  2678826 2023-06-08 17:52:08.000000 joulescope-1.1.7/joulescope/v0/stream_buffer.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:52:09.960018 joulescope-1.1.7/joulescope/v0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v0/test/calibration_01.dat
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v0/test/test_array_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v0/test/test_calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v0/test/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v0/test/test_filter_fir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v0/test/test_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v0/test/test_pattern_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v0/test/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)    24029 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v0/test/test_stream_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v0/test/test_view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:52:09.960018 joulescope-1.1.7/joulescope/v0/usb/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v0/usb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v0/usb/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v0/usb/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v0/usb/device_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v0/usb/hw_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v0/usb/impl_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:52:09.960018 joulescope-1.1.7/joulescope/v0/usb/libusb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v0/usb/libusb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39849 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v0/usb/libusb/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v0/usb/scan_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:52:09.960018 joulescope-1.1.7/joulescope/v0/usb/winusb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v0/usb/winusb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34585 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v0/usb/winusb/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v0/usb/winusb/kernel32.py
--rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v0/usb/winusb/setupapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v0/usb/winusb/win32_device_notify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:52:09.964017 joulescope-1.1.7/joulescope/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27796 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v1/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     7113 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v1/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v1/js110.py
--rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v1/js220.py
--rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v1/sample_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)   891864 2023-06-08 17:52:09.000000 joulescope-1.1.7/joulescope/v1/stats.c
--rw-r--r--   0 runner    (1001) docker     (123)    15931 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v1/stream_buffer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:52:09.964017 joulescope-1.1.7/joulescope/v1/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/v1/test/test_sample_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    20671 2023-06-08 17:51:51.000000 joulescope-1.1.7/joulescope/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:52:09.948017 joulescope-1.1.7/joulescope.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-06-08 17:52:09.000000 joulescope-1.1.7/joulescope.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-06-08 17:52:09.000000 joulescope-1.1.7/joulescope.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 17:52:09.000000 joulescope-1.1.7/joulescope.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-08 17:52:09.000000 joulescope-1.1.7/joulescope.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-08 17:52:09.000000 joulescope-1.1.7/joulescope.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-08 17:52:09.000000 joulescope-1.1.7/joulescope.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-08 17:51:51.000000 joulescope-1.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-08 17:52:09.964017 joulescope-1.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-06-08 17:51:51.000000 joulescope-1.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:52:50.742259 joulescope-1.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    21337 2023-07-11 19:52:32.000000 joulescope-1.1.8/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-11 19:52:32.000000 joulescope-1.1.8/CREDITS.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-11 19:52:32.000000 joulescope-1.1.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-11 19:52:32.000000 joulescope-1.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-11 19:52:50.742259 joulescope-1.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-11 19:52:32.000000 joulescope-1.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:52:50.726259 joulescope-1.1.8/joulescope/
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53690 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/data_recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25692 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/datafile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:52:50.726259 joulescope-1.1.8/joulescope/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/entry_points/bootloader_go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/entry_points/capture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/entry_points/gpo_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/entry_points/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/entry_points/parameter_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/entry_points/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/entry_points/recording.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/entry_points/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/entry_points/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/entry_points/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/entry_points/stream_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/file_replace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/jls_v2_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10713 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/parameters_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/span.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/stream_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:52:50.730259 joulescope-1.1.8/joulescope/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15919 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/test/test_data_recorder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/test/test_data_recorder_downsampled.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10576 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/test/test_datafile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/test/test_file_replace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/test/test_jls_v2_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/test/test_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/test/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/test/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:52:50.730259 joulescope-1.1.8/joulescope/v0/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v0/array_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12239 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v0/bootloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v0/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85459 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v0/decimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56561 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v0/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)   960969 2023-07-11 19:52:47.000000 joulescope-1.1.8/joulescope/v0/filter_fir.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v0/firmware_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:52:50.734259 joulescope-1.1.8/joulescope/v0/native/
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v0/native/filter_fir.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v0/native/filter_fir.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v0/native/running_statistics.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v0/native/running_statistics.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:52:50.734259 joulescope-1.1.8/joulescope/v0/native/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    55447 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v0/native/test/acutest.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v0/native/test/test_filter_fir.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v0/notification_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)   437933 2023-07-11 19:52:47.000000 joulescope-1.1.8/joulescope/v0/pattern_buffer.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v0/public_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)  2679762 2023-07-11 19:52:49.000000 joulescope-1.1.8/joulescope/v0/stream_buffer.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:52:50.734259 joulescope-1.1.8/joulescope/v0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v0/test/calibration_01.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v0/test/test_array_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v0/test/test_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v0/test/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v0/test/test_filter_fir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v0/test/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v0/test/test_pattern_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v0/test/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24029 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v0/test/test_stream_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v0/test/test_view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:52:50.738259 joulescope-1.1.8/joulescope/v0/usb/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v0/usb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v0/usb/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4973 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v0/usb/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7875 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v0/usb/device_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v0/usb/hw_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v0/usb/impl_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:52:50.738259 joulescope-1.1.8/joulescope/v0/usb/libusb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v0/usb/libusb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39849 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v0/usb/libusb/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v0/usb/scan_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:52:50.738259 joulescope-1.1.8/joulescope/v0/usb/winusb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v0/usb/winusb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34585 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v0/usb/winusb/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v0/usb/winusb/kernel32.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v0/usb/winusb/setupapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v0/usb/winusb/win32_device_notify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:52:50.742259 joulescope-1.1.8/joulescope/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27796 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v1/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7113 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v1/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v1/js110.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v1/js220.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v1/sample_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   894080 2023-07-11 19:52:50.000000 joulescope-1.1.8/joulescope/v1/stats.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15931 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v1/stream_buffer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:52:50.742259 joulescope-1.1.8/joulescope/v1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/v1/test/test_sample_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20671 2023-07-11 19:52:32.000000 joulescope-1.1.8/joulescope/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:52:50.726259 joulescope-1.1.8/joulescope.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-11 19:52:50.000000 joulescope-1.1.8/joulescope.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-11 19:52:50.000000 joulescope-1.1.8/joulescope.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 19:52:50.000000 joulescope-1.1.8/joulescope.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-11 19:52:50.000000 joulescope-1.1.8/joulescope.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-11 19:52:50.000000 joulescope-1.1.8/joulescope.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-11 19:52:50.000000 joulescope-1.1.8/joulescope.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-11 19:52:32.000000 joulescope-1.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-11 19:52:50.742259 joulescope-1.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-07-11 19:52:32.000000 joulescope-1.1.8/setup.py
```

### Comparing `joulescope-1.1.7/CHANGELOG.md` & `joulescope-1.1.8/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 
 # CHANGELOG
 
 This file contains the list of changes made to pyjoulescope.
 
 
+## 1.1.8
+
+2023 Jul 11
+
+* Fixed JlsWriter for JS220.
+* Bumped pyjoulescope_driver version from 1.3.14 to 1.3.17.
+
+
 ## 1.1.7
 
 2023 Jun 8
 
 * Added GitHub Actions build.
 * Bumped minimum python version from 3.8 to 3.9.
```

### Comparing `joulescope-1.1.7/CREDITS.html` & `joulescope-1.1.8/CREDITS.html`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/LICENSE.txt` & `joulescope-1.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/PKG-INFO` & `joulescope-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joulescope
-Version: 1.1.7
+Version: 1.1.8
 Summary: Joulescope™ host driver and utilities
 Home-page: https://joulescope.readthedocs.io
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/pyjoulescope/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `joulescope-1.1.7/README.md` & `joulescope-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/__init__.py` & `joulescope-1.1.8/joulescope/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/__main__.py` & `joulescope-1.1.8/joulescope/__main__.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/data_recorder.py` & `joulescope-1.1.8/joulescope/data_recorder.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/datafile.py` & `joulescope-1.1.8/joulescope/datafile.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/entry_points/bootloader_go.py` & `joulescope-1.1.8/joulescope/entry_points/bootloader_go.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/entry_points/capture.py` & `joulescope-1.1.8/joulescope/entry_points/capture.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/entry_points/gpo_demo.py` & `joulescope-1.1.8/joulescope/entry_points/gpo_demo.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/entry_points/info.py` & `joulescope-1.1.8/joulescope/entry_points/info.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/entry_points/parameter_set.py` & `joulescope-1.1.8/joulescope/entry_points/parameter_set.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/entry_points/program.py` & `joulescope-1.1.8/joulescope/entry_points/program.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/entry_points/recording.py` & `joulescope-1.1.8/joulescope/entry_points/recording.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/entry_points/runner.py` & `joulescope-1.1.8/joulescope/entry_points/runner.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/entry_points/scan.py` & `joulescope-1.1.8/joulescope/entry_points/scan.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/entry_points/statistics.py` & `joulescope-1.1.8/joulescope/entry_points/statistics.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/entry_points/stream_test.py` & `joulescope-1.1.8/joulescope/entry_points/stream_test.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/file_replace.py` & `joulescope-1.1.8/joulescope/file_replace.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/jls_v2_writer.py` & `joulescope-1.1.8/joulescope/jls_v2_writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -145,20 +145,21 @@
         :param stream_buffer: The :class:`StreamBuffer` instance which contains
             the new data from the Joulescope.
         :return: False to continue streaming.
         """
         # called from USB thead, keep fast!
         # long-running operations will cause sample drops
         start_id, end_id = stream_buffer.sample_id_range
-        if self._idx < end_id:
-            data = stream_buffer.samples_get(self._idx, end_id, fields=self._signals)
+        start_id = max(self._idx, start_id)
+        if start_id < end_id:
+            data = stream_buffer.samples_get(start_id, end_id, fields=self._signals)
             for s in self._signals:
                 x = np.ascontiguousarray(data['signals'][s]['value'])
                 idx = SIGNALS[s][0]
-                self._wr.fsr_f32(idx, self._idx, x)
+                self._wr.fsr_f32(idx, start_id, x)
             self._idx = end_id
         return False
 
     def fsr_f32(self, signal_name, sample_id, x):
         """Write signal data directly.
 
         :param signal_name: The signal name string.
```

### Comparing `joulescope-1.1.7/joulescope/parameter.py` & `joulescope-1.1.8/joulescope/parameter.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/parameters_v1.py` & `joulescope-1.1.8/joulescope/parameters_v1.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/span.py` & `joulescope-1.1.8/joulescope/span.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/stream_buffer.py` & `joulescope-1.1.8/joulescope/stream_buffer.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/test/test_data_recorder.py` & `joulescope-1.1.8/joulescope/test/test_data_recorder.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/test/test_data_recorder_downsampled.py` & `joulescope-1.1.8/joulescope/test/test_data_recorder_downsampled.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/test/test_datafile.py` & `joulescope-1.1.8/joulescope/test/test_datafile.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/test/test_file_replace.py` & `joulescope-1.1.8/joulescope/test/test_file_replace.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/test/test_jls_v2_writer.py` & `joulescope-1.1.8/joulescope/test/test_jls_v2_writer.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/test/test_span.py` & `joulescope-1.1.8/joulescope/test/test_span.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/test/test_time.py` & `joulescope-1.1.8/joulescope/test/test_time.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/test/test_units.py` & `joulescope-1.1.8/joulescope/test/test_units.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/time.py` & `joulescope-1.1.8/joulescope/time.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/units.py` & `joulescope-1.1.8/joulescope/units.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v0/array_storage.py` & `joulescope-1.1.8/joulescope/v0/array_storage.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v0/bootloader.py` & `joulescope-1.1.8/joulescope/v0/bootloader.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v0/calibration.py` & `joulescope-1.1.8/joulescope/v0/calibration.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v0/decimators.py` & `joulescope-1.1.8/joulescope/v0/decimators.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v0/driver.py` & `joulescope-1.1.8/joulescope/v0/driver.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v0/filter_fir.c` & `joulescope-1.1.8/joulescope/v0/filter_fir.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "joulescope/v0/native/filter_fir.h"
         ],
         "include_dirs": [
             "./joulescope/v0",
-            "/tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/core/include"
+            "/tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/core/include"
         ],
         "name": "joulescope.v0.filter_fir",
         "sources": [
             "joulescope/v0/filter_fir.pyx",
             "joulescope/v0/native/filter_fir.c"
         ]
     },
@@ -30,16 +30,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -106,15 +106,15 @@
   #if PY_VERSION_HEX < 0x03090000
     #undef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -390,17 +390,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -470,14 +467,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -1122,195 +1124,177 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":689
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":696
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":703
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":713
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
+ * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   longlong_t
- * 
- */
-typedef npy_longlong __pyx_t_5numpy_long_t;
-
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":715
- * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":717
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
+ * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":716
  * 
  * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulonglong_t
- * 
- */
-typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
-
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":719
- * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":721
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":724
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1342,42 +1326,42 @@
 /*--- Type declarations ---*/
 struct __pyx_obj_10joulescope_2v0_10filter_fir_FilterFir;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":728
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":732
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1859,14 +1843,31 @@
 #endif
 
 /* WriteUnraisableException.proto */
 static void __Pyx_WriteUnraisable(const char *name, int clineno,
                                   int lineno, const char *filename,
                                   int full_traceback, int nogil);
 
+/* AssertionsEnabled.proto */
+#define __Pyx_init_assertions_enabled()
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
+  #define __pyx_assertions_enabled() (1)
+#elif PY_VERSION_HEX < 0x03080000  ||  CYTHON_COMPILING_IN_PYPY  ||  defined(Py_LIMITED_API)
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030900A6
+  static int __pyx_assertions_enabled_flag;
+  #define __pyx_assertions_enabled() (__pyx_assertions_enabled_flag)
+  #undef __Pyx_init_assertions_enabled
+  static void __Pyx_init_assertions_enabled(void) {
+    __pyx_assertions_enabled_flag = ! _PyInterpreterState_GetConfig(__Pyx_PyThreadState_Current->interp)->optimization_level;
+  }
+#else
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#endif
+
 /* GCCDiagnostics.proto */
 #if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
 #define __Pyx_HAS_GCC_DIAGNOSTIC
 #endif
 
 /* BuildPyUnicode.proto */
 static PyObject* __Pyx_PyUnicode_BuildFromAscii(Py_ssize_t ulength, char* chars, int clength,
@@ -2124,30 +2125,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
-#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_0_29_35 {
-   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
-   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
@@ -3850,15 +3851,15 @@
  *     cdef void c_process(self, const double * x, uint32_t x_length):
  *         if x_length != self._filters_width:
  *             assert(x_length == self._filters_width)             # <<<<<<<<<<<<<<
  *             return
  *         c_filter_fir.filter_fir_single(self._filters[0], x, x_length)
  */
     #ifndef CYTHON_WITHOUT_ASSERTIONS
-    if (unlikely(!Py_OptimizeFlag)) {
+    if (unlikely(__pyx_assertions_enabled())) {
       if (unlikely(!((__pyx_v_x_length == __pyx_v_self->_filters_width) != 0))) {
         PyErr_SetNone(PyExc_AssertionError);
         __PYX_ERR(0, 89, __pyx_L1_error)
       }
     }
     #endif
 
@@ -4407,15 +4408,15 @@
   __Pyx_AddTraceback("joulescope.v0.filter_fir.FilterFir.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":734
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4424,29 +4425,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4457,15 +4458,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":737
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4474,29 +4475,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4507,15 +4508,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":740
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4524,29 +4525,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4557,15 +4558,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":743
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4574,29 +4575,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4607,15 +4608,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":746
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4624,29 +4625,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 747, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4657,212 +4658,220 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":749
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":928
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":926
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":927
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
-  (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
+  __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 927, __pyx_L1_error)
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":932
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":932
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":933
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":940
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4878,15 +4887,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -4894,84 +4903,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":939
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 942, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 939, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":940
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 943, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 940, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 944, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 941, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 944, __pyx_L5_except_error)
+      __PYX_ERR(2, 941, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4986,15 +4995,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":946
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5010,15 +5019,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5026,84 +5035,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":945
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 948, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 945, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":946
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 949, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 946, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 950, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 947, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 950, __pyx_L5_except_error)
+      __PYX_ERR(2, 947, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5118,15 +5127,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":952
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5142,15 +5151,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5158,84 +5167,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":951
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 954, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 951, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":952
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 955, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 952, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":953
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 956, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 953, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 956, __pyx_L5_except_error)
+      __PYX_ERR(2, 953, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5250,176 +5259,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":966
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":975
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":981
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":990
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":996
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":1000
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":1007
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":1014
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -12762,15 +12771,15 @@
  *     cdef _memoryviewslice memviewsliceobj
  * 
  *     assert memview.view.ndim > 0             # <<<<<<<<<<<<<<
  * 
  *     if isinstance(memview, _memoryviewslice):
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_v_memview->view.ndim > 0) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
       __PYX_ERR(1, 724, __pyx_L1_error)
     }
   }
   #endif
 
@@ -18490,15 +18499,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_10joulescope_2v0_10filter_fir_FilterFir(PyObject *o) {
   struct __pyx_obj_10joulescope_2v0_10filter_fir_FilterFir *p = (struct __pyx_obj_10joulescope_2v0_10filter_fir_FilterFir *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -18644,15 +18653,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_array(PyObject *o) {
   struct __pyx_array_obj *p = (struct __pyx_array_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
@@ -18829,15 +18838,15 @@
   p->name = Py_None; Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_Enum(PyObject *o) {
   struct __pyx_MemviewEnum_obj *p = (struct __pyx_MemviewEnum_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->name);
   (*Py_TYPE(o)->tp_free)(o);
 }
@@ -18960,15 +18969,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_memoryview(PyObject *o) {
   struct __pyx_memoryview_obj *p = (struct __pyx_memoryview_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -19213,15 +19222,15 @@
   p->from_slice.memview = NULL;
   return o;
 }
 
 static void __pyx_tp_dealloc__memoryviewslice(PyObject *o) {
   struct __pyx_memoryviewslice_obj *p = (struct __pyx_memoryviewslice_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -19506,15 +19515,15 @@
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(0, 50, __pyx_L1_error)
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 57, __pyx_L1_error)
   __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(0, 110, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 944, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 941, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(1, 134, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(1, 149, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(1, 406, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(1, 615, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(1, 834, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
@@ -19551,33 +19560,33 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(2, 944, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(2, 941, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(2, 950, __pyx_L1_error)
+  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(2, 947, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
   /* "View.MemoryView":134
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
@@ -19840,14 +19849,19 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
+  /* AssertionsEnabled.init */
+  __Pyx_init_assertions_enabled();
+
+if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
+
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_112105877 = PyInt_FromLong(112105877L); if (unlikely(!__pyx_int_112105877)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_136983863 = PyInt_FromLong(136983863L); if (unlikely(!__pyx_int_136983863)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_184977713 = PyInt_FromLong(184977713L); if (unlikely(!__pyx_int_184977713)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_neg_1 = PyInt_FromLong(-1); if (unlikely(!__pyx_int_neg_1)) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -19979,39 +19993,39 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 826, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 767, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 769, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 771, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 773, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 775, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 777, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 779, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 781, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 783, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 785, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 823, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -22874,18 +22888,18 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_0_29_35
-#define __PYX_HAVE_RT_ImportType_0_29_35
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -22931,22 +22945,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `joulescope-1.1.7/joulescope/v0/firmware_manager.py` & `joulescope-1.1.8/joulescope/v0/firmware_manager.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v0/native/filter_fir.c` & `joulescope-1.1.8/joulescope/v0/native/filter_fir.c`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v0/native/filter_fir.h` & `joulescope-1.1.8/joulescope/v0/native/filter_fir.h`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v0/native/running_statistics.c` & `joulescope-1.1.8/joulescope/v0/native/running_statistics.c`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v0/native/running_statistics.h` & `joulescope-1.1.8/joulescope/v0/native/running_statistics.h`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v0/native/test/acutest.h` & `joulescope-1.1.8/joulescope/v0/native/test/acutest.h`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v0/native/test/test_filter_fir.c` & `joulescope-1.1.8/joulescope/v0/native/test/test_filter_fir.c`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v0/notification_handler.py` & `joulescope-1.1.8/joulescope/v0/notification_handler.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v0/pattern_buffer.c` & `joulescope-1.1.8/joulescope/v0/pattern_buffer.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "/tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/core/include"
+            "/tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/core/include"
         ],
         "name": "joulescope.v0.pattern_buffer",
         "sources": [
             "joulescope/v0/pattern_buffer.pyx"
         ]
     },
     "module_name": "joulescope.v0.pattern_buffer"
@@ -27,16 +27,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -103,15 +103,15 @@
   #if PY_VERSION_HEX < 0x03090000
     #undef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -387,17 +387,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -467,14 +464,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -1047,195 +1049,177 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":689
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":696
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":703
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":713
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
+ * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   longlong_t
- * 
- */
-typedef npy_longlong __pyx_t_5numpy_long_t;
-
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":715
- * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":717
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
+ * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":716
  * 
  * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulonglong_t
- * 
- */
-typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
-
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":719
- * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":721
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":724
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1263,42 +1247,42 @@
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 struct __pyx_obj_10joulescope_2v0_14pattern_buffer_PatternBuffer;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":728
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":732
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1640,14 +1624,19 @@
         PyObject_Format(s, f))
 #else
     #define __Pyx_PyObject_FormatSimple(s, f) (\
         likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
         PyObject_Format(s, f))
 #endif
 
+/* WriteUnraisableException.proto */
+static void __Pyx_WriteUnraisable(const char *name, int clineno,
+                                  int lineno, const char *filename,
+                                  int full_traceback, int nogil);
+
 /* GetTopmostException.proto */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
 #endif
 
 /* SaveResetException.proto */
 #if CYTHON_FAST_THREAD_STATE
@@ -1696,30 +1685,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
-#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_0_29_35 {
-   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
-   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
@@ -4920,15 +4909,15 @@
   __Pyx_AddTraceback("joulescope.v0.pattern_buffer.PatternBuffer.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":734
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4937,29 +4926,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4970,15 +4959,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":737
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4987,29 +4976,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -5020,15 +5009,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":740
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -5037,29 +5026,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -5070,15 +5059,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":743
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -5087,29 +5076,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -5120,15 +5109,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":746
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -5137,29 +5126,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 747, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -5170,212 +5159,220 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":749
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":928
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":926
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":927
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
-  (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
+  __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 927, __pyx_L1_error)
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":932
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":932
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":933
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":940
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5391,15 +5388,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -5407,84 +5404,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":939
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 942, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 939, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":940
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 943, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 940, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 944, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 941, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 944, __pyx_L5_except_error)
+      __PYX_ERR(2, 941, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5499,15 +5496,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":946
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5523,15 +5520,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5539,84 +5536,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":945
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 948, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 945, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":946
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 949, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 946, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 950, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 947, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 950, __pyx_L5_except_error)
+      __PYX_ERR(2, 947, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5631,15 +5628,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":952
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5655,15 +5652,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5671,84 +5668,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":951
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 954, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 951, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":952
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 955, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 952, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":953
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 956, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 953, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(2, 956, __pyx_L5_except_error)
+      __PYX_ERR(2, 953, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5763,176 +5760,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":966
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":975
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":981
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":990
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":996
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":1000
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":1007
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":1014
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -5958,15 +5955,15 @@
   bad:
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_10joulescope_2v0_14pattern_buffer_PatternBuffer(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   (*Py_TYPE(o)->tp_free)(o);
 }
 
 static PyObject *__pyx_getprop_10joulescope_2v0_14pattern_buffer_13PatternBuffer_sample_id_max(PyObject *o, CYTHON_UNUSED void *x) {
@@ -6218,15 +6215,15 @@
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 166, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 186, __pyx_L1_error)
   __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(0, 205, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 944, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(2, 941, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
@@ -6281,33 +6278,33 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(2, 944, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(2, 941, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(2, 950, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(2, 947, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -6391,39 +6388,39 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 826, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(2, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(2, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(2, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(2, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(2, 767, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_number) __PYX_ERR(2, 769, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(2, 771, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(2, 773, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(2, 775, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(2, 777, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(2, 779, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(2, 781, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(2, 783, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_character) __PYX_ERR(2, 785, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(2, 823, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -6708,15 +6705,15 @@
  * # Licensed under the Apache License, Version 2.0 (the "License");
  */
   __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -8341,14 +8338,54 @@
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(owned_ref);
     #endif
     return (equals == Py_NE);
 #endif
 }
 
+/* WriteUnraisableException */
+  static void __Pyx_WriteUnraisable(const char *name, CYTHON_UNUSED int clineno,
+                                  CYTHON_UNUSED int lineno, CYTHON_UNUSED const char *filename,
+                                  int full_traceback, CYTHON_UNUSED int nogil) {
+    PyObject *old_exc, *old_val, *old_tb;
+    PyObject *ctx;
+    __Pyx_PyThreadState_declare
+#ifdef WITH_THREAD
+    PyGILState_STATE state;
+    if (nogil)
+        state = PyGILState_Ensure();
+    else state = (PyGILState_STATE)0;
+#endif
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrFetch(&old_exc, &old_val, &old_tb);
+    if (full_traceback) {
+        Py_XINCREF(old_exc);
+        Py_XINCREF(old_val);
+        Py_XINCREF(old_tb);
+        __Pyx_ErrRestore(old_exc, old_val, old_tb);
+        PyErr_PrintEx(1);
+    }
+    #if PY_MAJOR_VERSION < 3
+    ctx = PyString_FromString(name);
+    #else
+    ctx = PyUnicode_FromString(name);
+    #endif
+    __Pyx_ErrRestore(old_exc, old_val, old_tb);
+    if (!ctx) {
+        PyErr_WriteUnraisable(Py_None);
+    } else {
+        PyErr_WriteUnraisable(ctx);
+        Py_DECREF(ctx);
+    }
+#ifdef WITH_THREAD
+    if (nogil)
+        PyGILState_Release(state);
+#endif
+}
+
 /* GetTopmostException */
   #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem *
 __Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
 {
     _PyErr_StackItem *exc_info = tstate->exc_info;
     while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
@@ -8691,18 +8728,18 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType_0_29_35
-#define __PYX_HAVE_RT_ImportType_0_29_35
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -8748,22 +8785,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `joulescope-1.1.7/joulescope/v0/public_keys.py` & `joulescope-1.1.8/joulescope/v0/public_keys.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v0/stream_buffer.c` & `joulescope-1.1.8/joulescope/v0/stream_buffer.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "joulescope/v0/native/filter_fir.h"
         ],
         "include_dirs": [
             "./joulescope/v0",
-            "/tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/core/include"
+            "/tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/core/include"
         ],
         "name": "joulescope.v0.stream_buffer",
         "sources": [
             "joulescope/v0/stream_buffer.pyx",
             "joulescope/v0/native/running_statistics.c"
         ]
     },
@@ -30,16 +30,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -106,15 +106,15 @@
   #if PY_VERSION_HEX < 0x03090000
     #undef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -390,17 +390,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -470,14 +467,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -1129,195 +1131,177 @@
 #define __Pyx_PyGILState_Ensure PyGILState_Ensure
 #define __Pyx_PyGILState_Release PyGILState_Release
 #define __Pyx_FastGIL_Remember()
 #define __Pyx_FastGIL_Forget()
 #define __Pyx_FastGilFuncInit()
 
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":689
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":696
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":703
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":713
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
+ * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   longlong_t
- * 
- */
-typedef npy_longlong __pyx_t_5numpy_long_t;
-
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":715
- * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":717
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
+ * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":716
  * 
  * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulonglong_t
- * 
- */
-typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
-
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":719
- * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":721
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":724
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1356,42 +1340,42 @@
 struct __pyx_obj_10joulescope_2v0_13stream_buffer_DownsamplingStreamBuffer;
 struct __pyx_obj_10joulescope_2v0_13stream_buffer___pyx_scope_struct__samples_get;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":728
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":732
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2309,14 +2293,31 @@
 #define __Pyx_PyObject_DelSlice(obj, cstart, cstop, py_start, py_stop, py_slice, has_cstart, has_cstop, wraparound)\
     __Pyx_PyObject_SetSlice(obj, (PyObject*)NULL, cstart, cstop, py_start, py_stop, py_slice, has_cstart, has_cstop, wraparound)
 static CYTHON_INLINE int __Pyx_PyObject_SetSlice(
         PyObject* obj, PyObject* value, Py_ssize_t cstart, Py_ssize_t cstop,
         PyObject** py_start, PyObject** py_stop, PyObject** py_slice,
         int has_cstart, int has_cstop, int wraparound);
 
+/* AssertionsEnabled.proto */
+#define __Pyx_init_assertions_enabled()
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
+  #define __pyx_assertions_enabled() (1)
+#elif PY_VERSION_HEX < 0x03080000  ||  CYTHON_COMPILING_IN_PYPY  ||  defined(Py_LIMITED_API)
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030900A6
+  static int __pyx_assertions_enabled_flag;
+  #define __pyx_assertions_enabled() (__pyx_assertions_enabled_flag)
+  #undef __Pyx_init_assertions_enabled
+  static void __Pyx_init_assertions_enabled(void) {
+    __pyx_assertions_enabled_flag = ! _PyInterpreterState_GetConfig(__Pyx_PyThreadState_Current->interp)->optimization_level;
+  }
+#else
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#endif
+
 /* DictGetItem.proto */
 #if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
 static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key);
 #define __Pyx_PyObject_Dict_GetItem(obj, name)\
     (likely(PyDict_CheckExact(obj)) ?\
      __Pyx_PyDict_GetItem(obj, name) : PyObject_GetItem(obj, name))
 #else
@@ -2693,30 +2694,30 @@
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* SetVTable.proto */
 static int __Pyx_SetVtable(PyObject *dict, void *vtable);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
-#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_0_29_35 {
-   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
-   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* GetVTable.proto */
 static void* __Pyx_GetVtable(PyObject *dict);
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
@@ -12112,15 +12113,15 @@
  *     def __cinit__(self):
  *         self._missing_pkt = np.full((SAMPLES_PER_PACKET * 2), 0xffff, dtype=np.uint16)
  *         assert(self._missing_pkt.flags['C_CONTIGUOUS'])             # <<<<<<<<<<<<<<
  *         cdef np.uint16_t [::1] missing_pkt_c = self._missing_pkt
  *         self._missing_pkt_ptr = &missing_pkt_c[0]
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->_missing_pkt, __pyx_n_s_flags); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 355, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_t_4, __pyx_n_u_C_CONTIGUOUS); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 355, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(2, 355, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
@@ -13552,15 +13553,15 @@
  * 
  *         self.raw = np.full((length * 2), 0, dtype=np.uint16)
  *         assert(self.raw.flags['C_CONTIGUOUS'])             # <<<<<<<<<<<<<<
  *         cdef np.uint16_t [::1] raw_c = self.raw
  *         self.raw_ptr = &raw_c[0]
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     __pyx_t_10 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->raw, __pyx_n_s_flags); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 496, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_t_10, __pyx_n_u_C_CONTIGUOUS); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 496, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(2, 496, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
@@ -13648,15 +13649,15 @@
  * 
  *         self.data = np.full((length * 2), 0.0, dtype=np.float32)
  *         assert(self.data.flags['C_CONTIGUOUS'])             # <<<<<<<<<<<<<<
  *         cdef np.float32_t [::1] data_c = self.data
  *         self.data_ptr = &data_c[0]
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->data, __pyx_n_s_flags); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 501, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = __Pyx_PyObject_Dict_GetItem(__pyx_t_2, __pyx_n_u_C_CONTIGUOUS); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 501, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(2, 501, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
@@ -13742,15 +13743,15 @@
  * 
  *         self.bits = np.full(length, 0, dtype=np.uint8)
  *         assert(self.bits.flags['C_CONTIGUOUS'])             # <<<<<<<<<<<<<<
  *         cdef np.uint8_t [::1] bits_c = self.bits
  *         self.bits_ptr = &bits_c[0]
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->bits, __pyx_n_s_flags); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 506, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_1 = __Pyx_PyObject_Dict_GetItem(__pyx_t_6, __pyx_n_u_C_CONTIGUOUS); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 506, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(2, 506, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
@@ -26341,15 +26342,15 @@
  * 
  *     def __init__(self, duration, reductions, input_sampling_frequency, output_sampling_frequency):
  *         assert(sizeof(ds_value_s) == 16)             # <<<<<<<<<<<<<<
  *         if input_sampling_frequency is not None and input_sampling_frequency != 2000000:
  *             raise ValueError(f'Require 2000000 sps, provided {input_sampling_frequency}')
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!(((sizeof(struct __pyx_t_10joulescope_2v0_13stream_buffer_ds_value_s)) == 16) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
       __PYX_ERR(4, 53, __pyx_L1_error)
     }
   }
   #endif
 
@@ -36092,15 +36093,15 @@
   __pyx_L0:;
   __PYX_XDEC_MEMVIEW(&__pyx_v_s, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":734
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -36109,29 +36110,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 735, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -36142,15 +36143,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":737
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -36159,29 +36160,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 738, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -36192,15 +36193,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":740
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -36209,29 +36210,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 741, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -36242,15 +36243,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":743
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -36259,29 +36260,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 744, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -36292,15 +36293,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":746
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -36309,29 +36310,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 747, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -36342,212 +36343,220 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":749
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":928
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":926
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":927
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
-  (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
+  __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(5, 927, __pyx_L1_error)
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":932
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":932
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":933
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":940
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -36563,15 +36572,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -36579,84 +36588,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":939
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(5, 942, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(5, 939, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":940
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(5, 943, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(5, 940, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__37, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(5, 944, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__37, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(5, 941, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(5, 944, __pyx_L5_except_error)
+      __PYX_ERR(5, 941, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -36671,15 +36680,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":946
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -36695,15 +36704,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -36711,84 +36720,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":945
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(5, 948, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(5, 945, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":946
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(5, 949, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(5, 946, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__38, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(5, 950, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__38, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(5, 947, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(5, 950, __pyx_L5_except_error)
+      __PYX_ERR(5, 947, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -36803,15 +36812,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":952
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -36827,15 +36836,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -36843,84 +36852,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":951
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(5, 954, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(5, 951, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":952
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(5, 955, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(5, 952, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":953
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__38, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(5, 956, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__38, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(5, 953, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(5, 956, __pyx_L5_except_error)
+      __PYX_ERR(5, 953, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -36935,176 +36944,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":966
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":975
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":981
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":990
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":996
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":1000
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":1007
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":1014
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -44666,15 +44675,15 @@
  *     cdef _memoryviewslice memviewsliceobj
  * 
  *     assert memview.view.ndim > 0             # <<<<<<<<<<<<<<
  * 
  *     if isinstance(memview, _memoryviewslice):
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_v_memview->view.ndim > 0) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
       __PYX_ERR(0, 724, __pyx_L1_error)
     }
   }
   #endif
 
@@ -50386,15 +50395,15 @@
   bad:
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_10joulescope_2v0_13stream_buffer_RunningStatistics(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   (*Py_TYPE(o)->tp_free)(o);
 }
 
 static PyObject *__pyx_getprop_10joulescope_2v0_13stream_buffer_17RunningStatistics_mean(PyObject *o, CYTHON_UNUSED void *x) {
@@ -50547,15 +50556,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_10joulescope_2v0_13stream_buffer_RawProcessor(PyObject *o) {
   struct __pyx_obj_10joulescope_2v0_13stream_buffer_RawProcessor *p = (struct __pyx_obj_10joulescope_2v0_13stream_buffer_RawProcessor *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->_cbk_user_data);
   (*Py_TYPE(o)->tp_free)(o);
 }
@@ -50712,15 +50721,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_10joulescope_2v0_13stream_buffer_Statistics(PyObject *o) {
   struct __pyx_obj_10joulescope_2v0_13stream_buffer_Statistics *p = (struct __pyx_obj_10joulescope_2v0_13stream_buffer_Statistics *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->stats);
   (*Py_TYPE(o)->tp_free)(o);
 }
@@ -50870,15 +50879,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_10joulescope_2v0_13stream_buffer_UsbBulkProcessor(PyObject *o) {
   struct __pyx_obj_10joulescope_2v0_13stream_buffer_UsbBulkProcessor *p = (struct __pyx_obj_10joulescope_2v0_13stream_buffer_UsbBulkProcessor *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->_missing_pkt);
   Py_CLEAR(p->_cbk_user_data);
   (*Py_TYPE(o)->tp_free)(o);
@@ -51015,15 +51024,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_10joulescope_2v0_13stream_buffer_StreamBuffer(PyObject *o) {
   struct __pyx_obj_10joulescope_2v0_13stream_buffer_StreamBuffer *p = (struct __pyx_obj_10joulescope_2v0_13stream_buffer_StreamBuffer *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->_usb_bulk_processor);
   Py_CLEAR(p->_raw_processor);
   Py_CLEAR(p->raw);
@@ -51343,15 +51352,15 @@
   p->_buffer_npy = Py_None; Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_10joulescope_2v0_13stream_buffer_DownsamplingStreamBuffer(PyObject *o) {
   struct __pyx_obj_10joulescope_2v0_13stream_buffer_DownsamplingStreamBuffer *p = (struct __pyx_obj_10joulescope_2v0_13stream_buffer_DownsamplingStreamBuffer *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->_stream_buffer);
   Py_CLEAR(p->_filter_fir);
   Py_CLEAR(p->_input_npy);
@@ -51772,15 +51781,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_array(PyObject *o) {
   struct __pyx_array_obj *p = (struct __pyx_array_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
@@ -51957,15 +51966,15 @@
   p->name = Py_None; Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_Enum(PyObject *o) {
   struct __pyx_MemviewEnum_obj *p = (struct __pyx_MemviewEnum_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->name);
   (*Py_TYPE(o)->tp_free)(o);
 }
@@ -52088,15 +52097,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_memoryview(PyObject *o) {
   struct __pyx_memoryview_obj *p = (struct __pyx_memoryview_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -52341,15 +52350,15 @@
   p->from_slice.memview = NULL;
   return o;
 }
 
 static void __pyx_tp_dealloc__memoryviewslice(PyObject *o) {
   struct __pyx_memoryviewslice_obj *p = (struct __pyx_memoryviewslice_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -52870,15 +52879,15 @@
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 2, __pyx_L1_error)
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(1, 73, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(1, 200, __pyx_L1_error)
   __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(1, 421, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(2, 515, __pyx_L1_error)
   __pyx_builtin_round = __Pyx_GetBuiltinName(__pyx_n_s_round); if (!__pyx_builtin_round) __PYX_ERR(2, 662, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(5, 944, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(5, 941, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 149, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(0, 406, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(0, 615, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(0, 834, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
@@ -53197,33 +53206,33 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("self._buffer_ptr,self._input_dbl cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__34 = PyTuple_Pack(1, __pyx_kp_s_self__buffer_ptr_self__input_dbl); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__34);
   __Pyx_GIVEREF(__pyx_tuple__34);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__37 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(5, 944, __pyx_L1_error)
+  __pyx_tuple__37 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(5, 941, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__37);
   __Pyx_GIVEREF(__pyx_tuple__37);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__38 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(5, 950, __pyx_L1_error)
+  __pyx_tuple__38 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(5, 947, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__38);
   __Pyx_GIVEREF(__pyx_tuple__38);
 
   /* "View.MemoryView":134
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
@@ -53632,14 +53641,19 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
+  /* AssertionsEnabled.init */
+  __Pyx_init_assertions_enabled();
+
+if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 1, __pyx_L1_error)
+
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(2, 1, __pyx_L1_error)
   __pyx_float_0_0 = PyFloat_FromDouble(0.0); if (unlikely(!__pyx_float_0_0)) __PYX_ERR(2, 1, __pyx_L1_error)
   __pyx_float_0_1 = PyFloat_FromDouble(0.1); if (unlikely(!__pyx_float_0_1)) __PYX_ERR(2, 1, __pyx_L1_error)
   __pyx_float_1_0 = PyFloat_FromDouble(1.0); if (unlikely(!__pyx_float_1_0)) __PYX_ERR(2, 1, __pyx_L1_error)
   __pyx_float_1eneg_12 = PyFloat_FromDouble(1e-12); if (unlikely(!__pyx_float_1eneg_12)) __PYX_ERR(2, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(2, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(2, 1, __pyx_L1_error)
@@ -53889,43 +53903,43 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(6, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(6, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(5, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(5, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(5, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(5, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(5, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_number) __PYX_ERR(5, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(5, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(5, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(5, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(5, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(5, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(5, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(5, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_character) __PYX_ERR(5, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(5, 826, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(5, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(5, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(5, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(5, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(5, 767, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_number) __PYX_ERR(5, 769, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(5, 771, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(5, 773, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(5, 775, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(5, 777, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(5, 779, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(5, 781, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(5, 783, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_character) __PYX_ERR(5, 785, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(5, 823, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("joulescope.v0.filter_fir"); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_10joulescope_2v0_10filter_fir_FilterFir = __Pyx_ImportType_0_29_35(__pyx_t_1, "joulescope.v0.filter_fir", "FilterFir", sizeof(struct __pyx_obj_10joulescope_2v0_10filter_fir_FilterFir), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(struct __pyx_obj_10joulescope_2v0_10filter_fir_FilterFir),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_10joulescope_2v0_10filter_fir_FilterFir) __PYX_ERR(7, 20, __pyx_L1_error)
+  __pyx_ptype_10joulescope_2v0_10filter_fir_FilterFir = __Pyx_ImportType_0_29_36(__pyx_t_1, "joulescope.v0.filter_fir", "FilterFir", sizeof(struct __pyx_obj_10joulescope_2v0_10filter_fir_FilterFir), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_10joulescope_2v0_10filter_fir_FilterFir),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_10joulescope_2v0_10filter_fir_FilterFir) __PYX_ERR(7, 20, __pyx_L1_error)
   __pyx_vtabptr_10joulescope_2v0_10filter_fir_FilterFir = (struct __pyx_vtabstruct_10joulescope_2v0_10filter_fir_FilterFir*)__Pyx_GetVtable(__pyx_ptype_10joulescope_2v0_10filter_fir_FilterFir->tp_dict); if (unlikely(!__pyx_vtabptr_10joulescope_2v0_10filter_fir_FilterFir)) __PYX_ERR(7, 20, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -54712,15 +54726,15 @@
  * STATS_DTYPE = np.dtype({'names': NP_STATS_NAMES, 'formats': NP_STATS_FORMAT})
  * STATS_FIELD_COUNT = _STATS_FIELDS
  * assert(len(STATS_FIELD_NAMES) == STATS_FIELD_COUNT)             # <<<<<<<<<<<<<<
  * log = logging.getLogger(__name__)
  * np.import_array()  # initialize numpy
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_STATS_FIELD_NAMES); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 61, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_23 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_23 == ((Py_ssize_t)-1))) __PYX_ERR(2, 61, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_1 = PyInt_FromSsize_t(__pyx_t_23); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 61, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_STATS_FIELD_COUNT); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 61, __pyx_L1_error)
@@ -59960,18 +59974,18 @@
     return 0;
 bad:
     Py_XDECREF(ob);
     return -1;
 }
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType_0_29_35
-#define __PYX_HAVE_RT_ImportType_0_29_35
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -60017,22 +60031,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `joulescope-1.1.7/joulescope/v0/test/calibration_01.dat` & `joulescope-1.1.8/joulescope/v0/test/calibration_01.dat`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v0/test/test_array_storage.py` & `joulescope-1.1.8/joulescope/v0/test/test_array_storage.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v0/test/test_calibration.py` & `joulescope-1.1.8/joulescope/v0/test/test_calibration.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v0/test/test_device.py` & `joulescope-1.1.8/joulescope/v0/test/test_device.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v0/test/test_filter_fir.py` & `joulescope-1.1.8/joulescope/v0/test/test_filter_fir.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v0/test/test_parameter.py` & `joulescope-1.1.8/joulescope/v0/test/test_parameter.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v0/test/test_pattern_buffer.py` & `joulescope-1.1.8/joulescope/v0/test/test_pattern_buffer.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v0/test/test_stats.py` & `joulescope-1.1.8/joulescope/v0/test/test_stats.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v0/test/test_stream_buffer.py` & `joulescope-1.1.8/joulescope/v0/test/test_stream_buffer.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v0/test/test_view.py` & `joulescope-1.1.8/joulescope/v0/test/test_view.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v0/usb/__init__.py` & `joulescope-1.1.8/joulescope/v0/usb/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v0/usb/api.py` & `joulescope-1.1.8/joulescope/v0/usb/api.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v0/usb/core.py` & `joulescope-1.1.8/joulescope/v0/usb/core.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v0/usb/device_thread.py` & `joulescope-1.1.8/joulescope/v0/usb/device_thread.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v0/usb/hw_tests.py` & `joulescope-1.1.8/joulescope/v0/usb/hw_tests.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v0/usb/impl_tools.py` & `joulescope-1.1.8/joulescope/v0/usb/impl_tools.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v0/usb/libusb/device.py` & `joulescope-1.1.8/joulescope/v0/usb/libusb/device.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v0/usb/scan_info.py` & `joulescope-1.1.8/joulescope/v0/usb/scan_info.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v0/usb/winusb/device.py` & `joulescope-1.1.8/joulescope/v0/usb/winusb/device.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v0/usb/winusb/kernel32.py` & `joulescope-1.1.8/joulescope/v0/usb/winusb/kernel32.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v0/usb/winusb/setupapi.py` & `joulescope-1.1.8/joulescope/v0/usb/winusb/setupapi.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v0/usb/winusb/win32_device_notify.py` & `joulescope-1.1.8/joulescope/v0/usb/winusb/win32_device_notify.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v1/__init__.py` & `joulescope-1.1.8/joulescope/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v1/device.py` & `joulescope-1.1.8/joulescope/v1/device.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v1/driver.py` & `joulescope-1.1.8/joulescope/v1/driver.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v1/js110.py` & `joulescope-1.1.8/joulescope/v1/js110.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v1/js220.py` & `joulescope-1.1.8/joulescope/v1/js220.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v1/sample_buffer.py` & `joulescope-1.1.8/joulescope/v1/sample_buffer.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v1/stats.c` & `joulescope-1.1.8/joulescope/v1/stats.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-/* Generated by Cython 0.29.35 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "/tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/core/include"
+            "/tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/core/include"
         ],
         "name": "joulescope.v1.stats",
         "sources": [
             "joulescope/v1/stats.pyx"
         ]
     },
     "module_name": "joulescope.v1.stats"
@@ -27,16 +27,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_35"
-#define CYTHON_HEX_VERSION 0x001D23F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -103,15 +103,15 @@
   #if PY_VERSION_HEX < 0x03090000
     #undef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -387,17 +387,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -467,14 +464,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -1120,195 +1122,177 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":689
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":696
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":703
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":713
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
+ * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   longlong_t
- * 
- */
-typedef npy_longlong __pyx_t_5numpy_long_t;
-
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":715
- * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":717
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
+ * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":716
  * 
  * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulonglong_t
- * 
- */
-typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
-
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":719
- * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":721
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":724
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1339,42 +1323,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":728
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":732
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1776,14 +1760,19 @@
 #define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
 #define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
 #endif
 
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
+/* WriteUnraisableException.proto */
+static void __Pyx_WriteUnraisable(const char *name, int clineno,
+                                  int lineno, const char *filename,
+                                  int full_traceback, int nogil);
+
 /* GetTopmostException.proto */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
 #endif
 
 /* SaveResetException.proto */
 #if CYTHON_FAST_THREAD_STATE
@@ -1989,14 +1978,31 @@
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_PyList_Append(L,x) PyList_Append(L,x)
 #endif
 
+/* AssertionsEnabled.proto */
+#define __Pyx_init_assertions_enabled()
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
+  #define __pyx_assertions_enabled() (1)
+#elif PY_VERSION_HEX < 0x03080000  ||  CYTHON_COMPILING_IN_PYPY  ||  defined(Py_LIMITED_API)
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030900A6
+  static int __pyx_assertions_enabled_flag;
+  #define __pyx_assertions_enabled() (__pyx_assertions_enabled_flag)
+  #undef __Pyx_init_assertions_enabled
+  static void __Pyx_init_assertions_enabled(void) {
+    __pyx_assertions_enabled_flag = ! _PyInterpreterState_GetConfig(__Pyx_PyThreadState_Current->interp)->optimization_level;
+  }
+#else
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#endif
+
 /* None.proto */
 static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname);
 
 /* DivInt[long].proto */
 static CYTHON_INLINE long __Pyx_div_long(long, long);
 
 /* PySequenceContains.proto */
@@ -2031,30 +2037,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_35
-#define __PYX_HAVE_RT_ImportType_proto_0_29_35
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
 #if __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_0_29_35(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_0_29_35 {
-   __Pyx_ImportType_CheckSize_Error_0_29_35 = 0,
-   __Pyx_ImportType_CheckSize_Warn_0_29_35 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_0_29_35 = 2
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
@@ -3704,15 +3710,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_dtype);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":734
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3721,29 +3727,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3754,15 +3760,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":737
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3771,29 +3777,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3804,15 +3810,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":740
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3821,29 +3827,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3854,15 +3860,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":743
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3871,29 +3877,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3904,15 +3910,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":746
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3921,29 +3927,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3954,212 +3960,220 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":749
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":928
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":926
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":927
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
-  (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
+  __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 927, __pyx_L1_error)
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":932
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":932
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":933
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":940
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4175,15 +4189,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -4191,84 +4205,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":939
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 939, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":940
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 940, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 941, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 944, __pyx_L5_except_error)
+      __PYX_ERR(1, 941, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4283,15 +4297,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":946
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4307,15 +4321,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4323,84 +4337,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":945
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 945, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":946
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 946, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 947, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 950, __pyx_L5_except_error)
+      __PYX_ERR(1, 947, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4415,15 +4429,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":952
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4439,15 +4453,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4455,84 +4469,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":951
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 951, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":952
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 952, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":953
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 953, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 956, __pyx_L5_except_error)
+      __PYX_ERR(1, 953, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4547,176 +4561,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":966
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":975
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":981
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":990
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":996
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":1000
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":1007
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":1014
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -12059,15 +12073,15 @@
  *     cdef _memoryviewslice memviewsliceobj
  * 
  *     assert memview.view.ndim > 0             # <<<<<<<<<<<<<<
  * 
  *     if isinstance(memview, _memoryviewslice):
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_v_memview->view.ndim > 0) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
       __PYX_ERR(2, 724, __pyx_L1_error)
     }
   }
   #endif
 
@@ -17786,15 +17800,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_array(PyObject *o) {
   struct __pyx_array_obj *p = (struct __pyx_array_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
@@ -17971,15 +17985,15 @@
   p->name = Py_None; Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_Enum(PyObject *o) {
   struct __pyx_MemviewEnum_obj *p = (struct __pyx_MemviewEnum_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->name);
   (*Py_TYPE(o)->tp_free)(o);
 }
@@ -18102,15 +18116,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_memoryview(PyObject *o) {
   struct __pyx_memoryview_obj *p = (struct __pyx_memoryview_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -18355,15 +18369,15 @@
   p->from_slice.memview = NULL;
   return o;
 }
 
 static void __pyx_tp_dealloc__memoryviewslice(PyObject *o) {
   struct __pyx_memoryviewslice_obj *p = (struct __pyx_memoryviewslice_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -18645,15 +18659,15 @@
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {&__pyx_n_u_variance, __pyx_k_variance, sizeof(__pyx_k_variance), 0, 1, 0, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 45, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 113, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 944, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 941, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(2, 149, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(2, 152, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(2, 2, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(2, 406, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(2, 615, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(2, 834, __pyx_L1_error)
   return 0;
@@ -18661,33 +18675,33 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 944, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 941, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../../tmp/build-env-tmru47h4/lib/python3.11/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../tmp/build-env-251udsfj/lib/python3.11/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 950, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 947, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
   /* "View.MemoryView":134
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
@@ -18962,14 +18976,19 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
+  /* AssertionsEnabled.init */
+  __Pyx_init_assertions_enabled();
+
+if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
+
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_112105877 = PyInt_FromLong(112105877L); if (unlikely(!__pyx_int_112105877)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_136983863 = PyInt_FromLong(136983863L); if (unlikely(!__pyx_int_136983863)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_184977713 = PyInt_FromLong(184977713L); if (unlikely(!__pyx_int_184977713)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_neg_1 = PyInt_FromLong(-1); if (unlikely(!__pyx_int_neg_1)) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -19086,39 +19105,39 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_35(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_35); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_35(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_35(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_35); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 767, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 769, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 771, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 773, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 775, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 777, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 779, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 781, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 783, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 785, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 823, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -20350,14 +20369,54 @@
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
 
+/* WriteUnraisableException */
+static void __Pyx_WriteUnraisable(const char *name, CYTHON_UNUSED int clineno,
+                                  CYTHON_UNUSED int lineno, CYTHON_UNUSED const char *filename,
+                                  int full_traceback, CYTHON_UNUSED int nogil) {
+    PyObject *old_exc, *old_val, *old_tb;
+    PyObject *ctx;
+    __Pyx_PyThreadState_declare
+#ifdef WITH_THREAD
+    PyGILState_STATE state;
+    if (nogil)
+        state = PyGILState_Ensure();
+    else state = (PyGILState_STATE)0;
+#endif
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrFetch(&old_exc, &old_val, &old_tb);
+    if (full_traceback) {
+        Py_XINCREF(old_exc);
+        Py_XINCREF(old_val);
+        Py_XINCREF(old_tb);
+        __Pyx_ErrRestore(old_exc, old_val, old_tb);
+        PyErr_PrintEx(1);
+    }
+    #if PY_MAJOR_VERSION < 3
+    ctx = PyString_FromString(name);
+    #else
+    ctx = PyUnicode_FromString(name);
+    #endif
+    __Pyx_ErrRestore(old_exc, old_val, old_tb);
+    if (!ctx) {
+        PyErr_WriteUnraisable(Py_None);
+    } else {
+        PyErr_WriteUnraisable(ctx);
+        Py_DECREF(ctx);
+    }
+#ifdef WITH_THREAD
+    if (nogil)
+        PyGILState_Release(state);
+#endif
+}
+
 /* GetTopmostException */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem *
 __Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
 {
     _PyErr_StackItem *exc_info = tstate->exc_info;
     while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
@@ -21484,18 +21543,18 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType_0_29_35
-#define __PYX_HAVE_RT_ImportType_0_29_35
-static PyTypeObject *__Pyx_ImportType_0_29_35(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_35 check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
@@ -21541,22 +21600,22 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_35 && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_35 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
```

### Comparing `joulescope-1.1.7/joulescope/v1/stream_buffer.py` & `joulescope-1.1.8/joulescope/v1/stream_buffer.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/v1/test/test_sample_buffer.py` & `joulescope-1.1.8/joulescope/v1/test/test_sample_buffer.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope/view.py` & `joulescope-1.1.8/joulescope/view.py`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/joulescope.egg-info/PKG-INFO` & `joulescope-1.1.8/joulescope.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joulescope
-Version: 1.1.7
+Version: 1.1.8
 Summary: Joulescope™ host driver and utilities
 Home-page: https://joulescope.readthedocs.io
 Author: Jetperch LLC
 Author-email: joulescope-dev@jetperch.com
 License: Apache 2.0
 Project-URL: Bug Reports, https://github.com/jetperch/pyjoulescope/issues
 Project-URL: Funding, https://www.joulescope.com
```

### Comparing `joulescope-1.1.7/joulescope.egg-info/SOURCES.txt` & `joulescope-1.1.8/joulescope.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/pyproject.toml` & `joulescope-1.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `joulescope-1.1.7/setup.py` & `joulescope-1.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,15 +178,15 @@
 
     # See https://packaging.python.org/en/latest/requirements.html
     # https://numpy.org/neps/nep-0029-deprecation_policy.html
     install_requires=[
         'numpy',
         'psutil',
         'pyjls>=0.7.1',
-        'pyjoulescope_driver>=1.3.14',
+        'pyjoulescope_driver>=1.3.17',
         'python-dateutil>=2.7.3',
         'pymonocypher>=3.1.3.2',
         "pywin32; platform_system=='Windows'",
     ],
 
     extras_require={
         'dev': ['check-manifest', 'coverage', 'Cython', 'wheel', 'sphinx', 'myst-parser'],
```

