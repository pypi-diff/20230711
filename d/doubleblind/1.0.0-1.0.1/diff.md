# Comparing `tmp/doubleblind-1.0.0.tar.gz` & `tmp/doubleblind-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doubleblind-1.0.0.tar", last modified: Sun Jul  2 19:09:52 2023, max compression
+gzip compressed data, was "doubleblind-1.0.1.tar", last modified: Tue Jul 11 10:42:06 2023, max compression
```

## Comparing `doubleblind-1.0.0.tar` & `doubleblind-1.0.1.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxrwxrwx   0        0        0        0 2023-07-02 19:09:52.148347 doubleblind-1.0.0/
--rw-rw-rw-   0        0        0       90 2023-07-02 18:56:15.000000 doubleblind-1.0.0/HISTORY.rst
--rw-rw-rw-   0        0        0     1090 2023-05-12 11:45:24.000000 doubleblind-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      355 2023-05-14 10:35:08.000000 doubleblind-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5666 2023-07-02 19:09:52.147471 doubleblind-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3235 2023-05-15 20:59:15.000000 doubleblind-1.0.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-02 19:09:51.840599 doubleblind-1.0.0/build/
-drwxrwxrwx   0        0        0        0 2023-07-02 19:09:51.841134 doubleblind-1.0.0/build/lib/
-drwxrwxrwx   0        0        0        0 2023-07-02 19:09:51.880906 doubleblind-1.0.0/build/lib/doubleblind/
--rw-rw-rw-   0        0        0    15406 2023-05-13 14:16:15.000000 doubleblind-1.0.0/build/lib/doubleblind/favicon.ico
--rw-rw-rw-   0        0        0    52999 2023-05-13 14:14:46.000000 doubleblind-1.0.0/build/lib/doubleblind/splash.png
--rw-rw-rw-   0        0        0    53768 2023-05-13 14:14:17.000000 doubleblind-1.0.0/build/lib/doubleblind/splash_transparent.png
-drwxrwxrwx   0        0        0        0 2023-07-02 19:09:51.844181 doubleblind-1.0.0/docs/
-drwxrwxrwx   0        0        0        0 2023-07-02 19:09:51.846171 doubleblind-1.0.0/docs/build/
-drwxrwxrwx   0        0        0        0 2023-07-02 19:09:52.000124 doubleblind-1.0.0/docs/build/_sources/
--rw-rw-rw-   0        0        0      181 2023-05-15 20:35:38.000000 doubleblind-1.0.0/docs/build/_sources/doubleblind.blinding.GenericCoder.__init__.rst.txt
--rw-rw-rw-   0        0        0      164 2023-05-15 20:35:38.000000 doubleblind-1.0.0/docs/build/_sources/doubleblind.blinding.GenericCoder.blind.rst.txt
--rw-rw-rw-   0        0        0      460 2023-05-15 20:35:34.000000 doubleblind-1.0.0/docs/build/_sources/doubleblind.blinding.GenericCoder.rst.txt
--rw-rw-rw-   0        0        0      170 2023-05-15 20:35:38.000000 doubleblind-1.0.0/docs/build/_sources/doubleblind.blinding.GenericCoder.unblind.rst.txt
--rw-rw-rw-   0        0        0      175 2023-05-15 20:35:38.000000 doubleblind-1.0.0/docs/build/_sources/doubleblind.blinding.ImageCoder.__init__.rst.txt
--rw-rw-rw-   0        0        0      158 2023-05-15 20:35:38.000000 doubleblind-1.0.0/docs/build/_sources/doubleblind.blinding.ImageCoder.blind.rst.txt
--rw-rw-rw-   0        0        0      473 2023-05-15 20:35:34.000000 doubleblind-1.0.0/docs/build/_sources/doubleblind.blinding.ImageCoder.rst.txt
--rw-rw-rw-   0        0        0      164 2023-05-15 20:35:38.000000 doubleblind-1.0.0/docs/build/_sources/doubleblind.blinding.ImageCoder.unblind.rst.txt
--rw-rw-rw-   0        0        0      169 2023-05-15 20:35:38.000000 doubleblind-1.0.0/docs/build/_sources/doubleblind.blinding.VSICoder.__init__.rst.txt
--rw-rw-rw-   0        0        0      152 2023-05-15 20:35:38.000000 doubleblind-1.0.0/docs/build/_sources/doubleblind.blinding.VSICoder.blind.rst.txt
--rw-rw-rw-   0        0        0      432 2023-05-15 20:35:34.000000 doubleblind-1.0.0/docs/build/_sources/doubleblind.blinding.VSICoder.rst.txt
--rw-rw-rw-   0        0        0      158 2023-05-15 20:35:38.000000 doubleblind-1.0.0/docs/build/_sources/doubleblind.blinding.VSICoder.unblind.rst.txt
--rw-rw-rw-   0        0        0      272 2023-05-15 20:24:16.000000 doubleblind-1.0.0/docs/build/_sources/doubleblind.blinding.rst.txt
--rw-rw-rw-   0        0        0       30 2023-05-15 20:30:53.000000 doubleblind-1.0.0/docs/build/_sources/history.rst.txt
--rw-rw-rw-   0        0        0      890 2023-05-15 20:58:17.000000 doubleblind-1.0.0/docs/build/_sources/index.rst.txt
--rw-rw-rw-   0        0        0     4841 2023-05-15 20:30:29.000000 doubleblind-1.0.0/docs/build/_sources/installation.rst.txt
--rw-rw-rw-   0        0        0       30 2019-07-11 11:49:50.000000 doubleblind-1.0.0/docs/build/_sources/readme.rst.txt
--rw-rw-rw-   0        0        0     3404 2023-07-02 18:55:20.000000 doubleblind-1.0.0/docs/build/_sources/user_guide.rst.txt
-drwxrwxrwx   0        0        0        0 2023-07-02 19:09:51.904805 doubleblind-1.0.0/docs/build/_static/
--rw-rw-rw-   0        0        0     1005 2023-05-15 20:19:07.000000 doubleblind-1.0.0/docs/build/_static/api_reference.rst
--rw-rw-rw-   0        0        0    53768 2023-05-13 14:14:17.000000 doubleblind-1.0.0/docs/build/_static/doubleblind.png
--rw-rw-rw-   0        0        0    15406 2023-05-13 14:16:15.000000 doubleblind-1.0.0/docs/build/_static/favicon.ico
--rw-rw-rw-   0        0        0      286 2023-05-14 14:35:23.000000 doubleblind-1.0.0/docs/build/_static/file.png
--rw-rw-rw-   0        0        0       90 2023-05-14 14:35:23.000000 doubleblind-1.0.0/docs/build/_static/minus.png
--rw-rw-rw-   0        0        0       90 2023-05-14 14:35:23.000000 doubleblind-1.0.0/docs/build/_static/plus.png
--rw-rw-rw-   0        0        0      695 2023-05-14 14:42:26.000000 doubleblind-1.0.0/docs/build/_static/py.png
-drwxrwxrwx   0        0        0        0 2023-07-02 19:09:52.008121 doubleblind-1.0.0/docs/source/
-drwxrwxrwx   0        0        0        0 2023-07-02 19:09:51.952471 doubleblind-1.0.0/docs/source/_static/
--rw-rw-rw-   0        0        0     1005 2023-05-15 20:19:07.000000 doubleblind-1.0.0/docs/source/_static/api_reference.rst
--rw-rw-rw-   0        0        0     3153 2023-05-15 20:33:11.000000 doubleblind-1.0.0/docs/source/conf.py
--rw-rw-rw-   0        0        0      181 2023-05-15 20:35:38.000000 doubleblind-1.0.0/docs/source/doubleblind.blinding.GenericCoder.__init__.rst
--rw-rw-rw-   0        0        0      164 2023-05-15 20:35:38.000000 doubleblind-1.0.0/docs/source/doubleblind.blinding.GenericCoder.blind.rst
--rw-rw-rw-   0        0        0      460 2023-05-15 20:35:34.000000 doubleblind-1.0.0/docs/source/doubleblind.blinding.GenericCoder.rst
--rw-rw-rw-   0        0        0      170 2023-05-15 20:35:38.000000 doubleblind-1.0.0/docs/source/doubleblind.blinding.GenericCoder.unblind.rst
--rw-rw-rw-   0        0        0      175 2023-05-15 20:35:38.000000 doubleblind-1.0.0/docs/source/doubleblind.blinding.ImageCoder.__init__.rst
--rw-rw-rw-   0        0        0      158 2023-05-15 20:35:38.000000 doubleblind-1.0.0/docs/source/doubleblind.blinding.ImageCoder.blind.rst
--rw-rw-rw-   0        0        0      473 2023-05-15 20:35:34.000000 doubleblind-1.0.0/docs/source/doubleblind.blinding.ImageCoder.rst
--rw-rw-rw-   0        0        0      164 2023-05-15 20:35:38.000000 doubleblind-1.0.0/docs/source/doubleblind.blinding.ImageCoder.unblind.rst
--rw-rw-rw-   0        0        0      169 2023-05-15 20:35:38.000000 doubleblind-1.0.0/docs/source/doubleblind.blinding.VSICoder.__init__.rst
--rw-rw-rw-   0        0        0      152 2023-05-15 20:35:38.000000 doubleblind-1.0.0/docs/source/doubleblind.blinding.VSICoder.blind.rst
--rw-rw-rw-   0        0        0      432 2023-05-15 20:35:34.000000 doubleblind-1.0.0/docs/source/doubleblind.blinding.VSICoder.rst
--rw-rw-rw-   0        0        0      158 2023-05-15 20:35:38.000000 doubleblind-1.0.0/docs/source/doubleblind.blinding.VSICoder.unblind.rst
--rw-rw-rw-   0        0        0      272 2023-05-15 20:34:50.000000 doubleblind-1.0.0/docs/source/doubleblind.blinding.rst
--rw-rw-rw-   0        0        0    53768 2023-05-13 14:14:17.000000 doubleblind-1.0.0/docs/source/doubleblind.png
--rw-rw-rw-   0        0        0    15406 2023-05-13 14:16:15.000000 doubleblind-1.0.0/docs/source/favicon.ico
--rw-rw-rw-   0        0        0       30 2023-05-15 20:30:53.000000 doubleblind-1.0.0/docs/source/history.rst
--rw-rw-rw-   0        0        0      890 2023-05-15 20:58:17.000000 doubleblind-1.0.0/docs/source/index.rst
--rw-rw-rw-   0        0        0     4841 2023-05-15 20:30:29.000000 doubleblind-1.0.0/docs/source/installation.rst
--rw-rw-rw-   0        0        0       30 2019-07-11 11:49:50.000000 doubleblind-1.0.0/docs/source/readme.rst
--rw-rw-rw-   0        0        0     3404 2023-07-02 18:55:20.000000 doubleblind-1.0.0/docs/source/user_guide.rst
-drwxrwxrwx   0        0        0        0 2023-07-02 19:09:52.047431 doubleblind-1.0.0/doubleblind/
--rw-rw-rw-   0        0        0       71 2023-05-12 20:05:44.000000 doubleblind-1.0.0/doubleblind/__init__.py
--rw-rw-rw-   0        0        0    11330 2023-06-03 10:22:45.000000 doubleblind-1.0.0/doubleblind/blinding.py
--rw-rw-rw-   0        0        0     1574 2023-05-16 14:33:38.000000 doubleblind-1.0.0/doubleblind/editing.py
--rw-rw-rw-   0        0        0     1563 2023-05-14 10:02:35.000000 doubleblind-1.0.0/doubleblind/favicon.icns
--rw-rw-rw-   0        0        0    15406 2023-05-13 14:16:15.000000 doubleblind-1.0.0/doubleblind/favicon.ico
--rw-rw-rw-   0        0        0    20365 2023-07-02 18:21:24.000000 doubleblind-1.0.0/doubleblind/gui.py
--rw-rw-rw-   0        0        0     1515 2023-05-16 18:13:59.000000 doubleblind-1.0.0/doubleblind/gui_style.py
--rw-rw-rw-   0        0        0      769 2023-05-14 13:21:37.000000 doubleblind-1.0.0/doubleblind/main.py
--rw-rw-rw-   0        0        0      838 2023-05-13 14:59:20.000000 doubleblind-1.0.0/doubleblind/parametric_style.qss
--rw-rw-rw-   0        0        0    52999 2023-05-13 14:14:46.000000 doubleblind-1.0.0/doubleblind/splash.png
--rw-rw-rw-   0        0        0    53768 2023-05-13 14:14:17.000000 doubleblind-1.0.0/doubleblind/splash_transparent.png
--rw-rw-rw-   0        0        0     3117 2023-06-03 10:22:45.000000 doubleblind-1.0.0/doubleblind/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-02 19:09:52.058729 doubleblind-1.0.0/doubleblind.egg-info/
--rw-rw-rw-   0        0        0     5666 2023-07-02 19:09:49.000000 doubleblind-1.0.0/doubleblind.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4961 2023-07-02 19:09:51.000000 doubleblind-1.0.0/doubleblind.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-02 19:09:49.000000 doubleblind-1.0.0/doubleblind.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-07-02 19:09:49.000000 doubleblind-1.0.0/doubleblind.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       57 2023-07-02 19:09:49.000000 doubleblind-1.0.0/doubleblind.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-02 19:09:49.000000 doubleblind-1.0.0/doubleblind.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2880 2023-07-02 19:09:32.000000 doubleblind-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      225 2023-05-16 18:39:17.000000 doubleblind-1.0.0/requirements_dev.txt
--rw-rw-rw-   0        0        0       42 2023-07-02 19:09:52.148347 doubleblind-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-02 19:09:52.073476 doubleblind-1.0.0/tests/
-drwxrwxrwx   0        0        0        0 2023-07-02 19:09:52.079208 doubleblind-1.0.0/tests/.pytest_cache/
--rw-rw-rw-   0        0        0       39 2023-05-15 09:11:55.000000 doubleblind-1.0.0/tests/.pytest_cache/.gitignore
--rw-rw-rw-   0        0        0      191 2023-05-15 09:11:55.000000 doubleblind-1.0.0/tests/.pytest_cache/CACHEDIR.TAG
--rw-rw-rw-   0        0        0      310 2023-05-15 09:11:55.000000 doubleblind-1.0.0/tests/.pytest_cache/README.md
-drwxrwxrwx   0        0        0        0 2023-07-02 19:09:51.850688 doubleblind-1.0.0/tests/.pytest_cache/v/
-drwxrwxrwx   0        0        0        0 2023-07-02 19:09:52.084221 doubleblind-1.0.0/tests/.pytest_cache/v/cache/
--rw-rw-rw-   0        0        0     4681 2023-05-16 20:52:36.000000 doubleblind-1.0.0/tests/.pytest_cache/v/cache/lastfailed
--rw-rw-rw-   0        0        0    10152 2023-05-16 20:52:36.000000 doubleblind-1.0.0/tests/.pytest_cache/v/cache/nodeids
--rw-rw-rw-   0        0        0        2 2023-05-16 20:52:36.000000 doubleblind-1.0.0/tests/.pytest_cache/v/cache/stepwise
--rw-rw-rw-   0        0        0     2661 2023-05-15 19:35:42.000000 doubleblind-1.0.0/tests/__init__.py
--rw-rw-rw-   0        0        0       88 2023-02-01 15:09:59.000000 doubleblind-1.0.0/tests/conftest.py
--rw-rw-rw-   0        0        0    15588 2023-05-16 20:51:51.000000 doubleblind-1.0.0/tests/test_blinding.py
--rw-rw-rw-   0        0        0     3069 2023-05-16 14:36:19.000000 doubleblind-1.0.0/tests/test_editing.py
-drwxrwxrwx   0        0        0        0 2023-07-02 19:09:51.852868 doubleblind-1.0.0/tests/test_files/
-drwxrwxrwx   0        0        0        0 2023-07-02 19:09:52.117142 doubleblind-1.0.0/tests/test_files/root_dir/
--rw-rw-rw-   0        0        0       64 2023-05-15 19:12:33.000000 doubleblind-1.0.0/tests/test_files/root_dir/dont_map.txt
--rw-rw-rw-   0        0        0    10018 2023-05-15 19:13:18.000000 doubleblind-1.0.0/tests/test_files/root_dir/test workbook.xlsx
--rw-rw-rw-   0        0        0       64 2023-05-15 19:24:03.000000 doubleblind-1.0.0/tests/test_files/root_dir/unmodified_file.txt
-drwxrwxrwx   0        0        0        0 2023-07-02 19:09:52.145508 doubleblind-1.0.0/tests/test_files/unblind_additionals_truth/
--rw-rw-rw-   0        0        0       64 2023-05-15 19:12:33.000000 doubleblind-1.0.0/tests/test_files/unblind_additionals_truth/dont_map.txt
--rw-rw-rw-   0        0        0       64 2023-05-15 19:13:50.000000 doubleblind-1.0.0/tests/test_files/unblind_additionals_truth/dont_map_unblinded.txt
--rw-rw-rw-   0        0        0    10018 2023-05-15 19:13:18.000000 doubleblind-1.0.0/tests/test_files/unblind_additionals_truth/test workbook.xlsx
--rw-rw-rw-   0        0        0     5658 2023-05-15 19:53:13.000000 doubleblind-1.0.0/tests/test_files/unblind_additionals_truth/test workbook_unblinded.xlsx
--rw-rw-rw-   0        0        0       64 2023-05-15 19:24:03.000000 doubleblind-1.0.0/tests/test_files/unblind_additionals_truth/unmodified_file.txt
--rw-rw-rw-   0        0        0     4005 2023-05-16 19:41:00.000000 doubleblind-1.0.0/tests/test_gui.py
--rw-rw-rw-   0        0        0     3636 2023-05-16 18:42:02.000000 doubleblind-1.0.0/tests/test_gui_style.py
--rw-rw-rw-   0        0        0     2175 2023-05-15 10:10:28.000000 doubleblind-1.0.0/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:42:06.561483 doubleblind-1.0.1/
+-rw-rw-rw-   0        0        0      194 2023-07-11 10:34:57.000000 doubleblind-1.0.1/HISTORY.rst
+-rw-rw-rw-   0        0        0     1090 2023-05-12 11:45:24.000000 doubleblind-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      355 2023-05-14 10:35:08.000000 doubleblind-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5666 2023-07-11 10:42:06.561483 doubleblind-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3235 2023-05-15 20:59:15.000000 doubleblind-1.0.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-11 10:42:06.340201 doubleblind-1.0.1/build/
+drwxrwxrwx   0        0        0        0 2023-07-11 10:42:06.341200 doubleblind-1.0.1/build/lib/
+drwxrwxrwx   0        0        0        0 2023-07-11 10:42:06.371133 doubleblind-1.0.1/build/lib/doubleblind/
+-rw-rw-rw-   0        0        0    15406 2023-05-13 14:16:15.000000 doubleblind-1.0.1/build/lib/doubleblind/favicon.ico
+-rw-rw-rw-   0        0        0    52999 2023-05-13 14:14:46.000000 doubleblind-1.0.1/build/lib/doubleblind/splash.png
+-rw-rw-rw-   0        0        0    53768 2023-05-13 14:14:17.000000 doubleblind-1.0.1/build/lib/doubleblind/splash_transparent.png
+drwxrwxrwx   0        0        0        0 2023-07-11 10:42:06.342851 doubleblind-1.0.1/docs/
+drwxrwxrwx   0        0        0        0 2023-07-11 10:42:06.344812 doubleblind-1.0.1/docs/build/
+drwxrwxrwx   0        0        0        0 2023-07-11 10:42:06.464992 doubleblind-1.0.1/docs/build/_sources/
+-rw-rw-rw-   0        0        0      181 2023-05-15 20:35:38.000000 doubleblind-1.0.1/docs/build/_sources/doubleblind.blinding.GenericCoder.__init__.rst.txt
+-rw-rw-rw-   0        0        0      164 2023-05-15 20:35:38.000000 doubleblind-1.0.1/docs/build/_sources/doubleblind.blinding.GenericCoder.blind.rst.txt
+-rw-rw-rw-   0        0        0      460 2023-05-15 20:35:34.000000 doubleblind-1.0.1/docs/build/_sources/doubleblind.blinding.GenericCoder.rst.txt
+-rw-rw-rw-   0        0        0      170 2023-05-15 20:35:38.000000 doubleblind-1.0.1/docs/build/_sources/doubleblind.blinding.GenericCoder.unblind.rst.txt
+-rw-rw-rw-   0        0        0      175 2023-05-15 20:35:38.000000 doubleblind-1.0.1/docs/build/_sources/doubleblind.blinding.ImageCoder.__init__.rst.txt
+-rw-rw-rw-   0        0        0      158 2023-05-15 20:35:38.000000 doubleblind-1.0.1/docs/build/_sources/doubleblind.blinding.ImageCoder.blind.rst.txt
+-rw-rw-rw-   0        0        0      473 2023-05-15 20:35:34.000000 doubleblind-1.0.1/docs/build/_sources/doubleblind.blinding.ImageCoder.rst.txt
+-rw-rw-rw-   0        0        0      164 2023-05-15 20:35:38.000000 doubleblind-1.0.1/docs/build/_sources/doubleblind.blinding.ImageCoder.unblind.rst.txt
+-rw-rw-rw-   0        0        0      169 2023-05-15 20:35:38.000000 doubleblind-1.0.1/docs/build/_sources/doubleblind.blinding.VSICoder.__init__.rst.txt
+-rw-rw-rw-   0        0        0      152 2023-05-15 20:35:38.000000 doubleblind-1.0.1/docs/build/_sources/doubleblind.blinding.VSICoder.blind.rst.txt
+-rw-rw-rw-   0        0        0      432 2023-05-15 20:35:34.000000 doubleblind-1.0.1/docs/build/_sources/doubleblind.blinding.VSICoder.rst.txt
+-rw-rw-rw-   0        0        0      158 2023-05-15 20:35:38.000000 doubleblind-1.0.1/docs/build/_sources/doubleblind.blinding.VSICoder.unblind.rst.txt
+-rw-rw-rw-   0        0        0      272 2023-05-15 20:24:16.000000 doubleblind-1.0.1/docs/build/_sources/doubleblind.blinding.rst.txt
+-rw-rw-rw-   0        0        0       30 2023-05-15 20:30:53.000000 doubleblind-1.0.1/docs/build/_sources/history.rst.txt
+-rw-rw-rw-   0        0        0      890 2023-05-15 20:58:17.000000 doubleblind-1.0.1/docs/build/_sources/index.rst.txt
+-rw-rw-rw-   0        0        0     4841 2023-05-15 20:30:29.000000 doubleblind-1.0.1/docs/build/_sources/installation.rst.txt
+-rw-rw-rw-   0        0        0       30 2019-07-11 11:49:50.000000 doubleblind-1.0.1/docs/build/_sources/readme.rst.txt
+-rw-rw-rw-   0        0        0     3404 2023-07-02 18:55:20.000000 doubleblind-1.0.1/docs/build/_sources/user_guide.rst.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 10:42:06.384169 doubleblind-1.0.1/docs/build/_static/
+-rw-rw-rw-   0        0        0     1005 2023-05-15 20:19:07.000000 doubleblind-1.0.1/docs/build/_static/api_reference.rst
+-rw-rw-rw-   0        0        0    53768 2023-05-13 14:14:17.000000 doubleblind-1.0.1/docs/build/_static/doubleblind.png
+-rw-rw-rw-   0        0        0    15406 2023-05-13 14:16:15.000000 doubleblind-1.0.1/docs/build/_static/favicon.ico
+-rw-rw-rw-   0        0        0      286 2023-05-14 14:35:23.000000 doubleblind-1.0.1/docs/build/_static/file.png
+-rw-rw-rw-   0        0        0       90 2023-05-14 14:35:23.000000 doubleblind-1.0.1/docs/build/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2023-05-14 14:35:23.000000 doubleblind-1.0.1/docs/build/_static/plus.png
+-rw-rw-rw-   0        0        0      695 2023-05-14 14:42:26.000000 doubleblind-1.0.1/docs/build/_static/py.png
+drwxrwxrwx   0        0        0        0 2023-07-11 10:42:06.472748 doubleblind-1.0.1/docs/source/
+drwxrwxrwx   0        0        0        0 2023-07-11 10:42:06.423141 doubleblind-1.0.1/docs/source/_static/
+-rw-rw-rw-   0        0        0     1005 2023-05-15 20:19:07.000000 doubleblind-1.0.1/docs/source/_static/api_reference.rst
+-rw-rw-rw-   0        0        0     3153 2023-07-11 10:41:22.000000 doubleblind-1.0.1/docs/source/conf.py
+-rw-rw-rw-   0        0        0      181 2023-05-15 20:35:38.000000 doubleblind-1.0.1/docs/source/doubleblind.blinding.GenericCoder.__init__.rst
+-rw-rw-rw-   0        0        0      164 2023-05-15 20:35:38.000000 doubleblind-1.0.1/docs/source/doubleblind.blinding.GenericCoder.blind.rst
+-rw-rw-rw-   0        0        0      460 2023-05-15 20:35:34.000000 doubleblind-1.0.1/docs/source/doubleblind.blinding.GenericCoder.rst
+-rw-rw-rw-   0        0        0      170 2023-05-15 20:35:38.000000 doubleblind-1.0.1/docs/source/doubleblind.blinding.GenericCoder.unblind.rst
+-rw-rw-rw-   0        0        0      175 2023-05-15 20:35:38.000000 doubleblind-1.0.1/docs/source/doubleblind.blinding.ImageCoder.__init__.rst
+-rw-rw-rw-   0        0        0      158 2023-05-15 20:35:38.000000 doubleblind-1.0.1/docs/source/doubleblind.blinding.ImageCoder.blind.rst
+-rw-rw-rw-   0        0        0      473 2023-05-15 20:35:34.000000 doubleblind-1.0.1/docs/source/doubleblind.blinding.ImageCoder.rst
+-rw-rw-rw-   0        0        0      164 2023-05-15 20:35:38.000000 doubleblind-1.0.1/docs/source/doubleblind.blinding.ImageCoder.unblind.rst
+-rw-rw-rw-   0        0        0      169 2023-05-15 20:35:38.000000 doubleblind-1.0.1/docs/source/doubleblind.blinding.VSICoder.__init__.rst
+-rw-rw-rw-   0        0        0      152 2023-05-15 20:35:38.000000 doubleblind-1.0.1/docs/source/doubleblind.blinding.VSICoder.blind.rst
+-rw-rw-rw-   0        0        0      432 2023-05-15 20:35:34.000000 doubleblind-1.0.1/docs/source/doubleblind.blinding.VSICoder.rst
+-rw-rw-rw-   0        0        0      158 2023-05-15 20:35:38.000000 doubleblind-1.0.1/docs/source/doubleblind.blinding.VSICoder.unblind.rst
+-rw-rw-rw-   0        0        0      272 2023-05-15 20:34:50.000000 doubleblind-1.0.1/docs/source/doubleblind.blinding.rst
+-rw-rw-rw-   0        0        0    53768 2023-05-13 14:14:17.000000 doubleblind-1.0.1/docs/source/doubleblind.png
+-rw-rw-rw-   0        0        0    15406 2023-05-13 14:16:15.000000 doubleblind-1.0.1/docs/source/favicon.ico
+-rw-rw-rw-   0        0        0       30 2023-05-15 20:30:53.000000 doubleblind-1.0.1/docs/source/history.rst
+-rw-rw-rw-   0        0        0      890 2023-05-15 20:58:17.000000 doubleblind-1.0.1/docs/source/index.rst
+-rw-rw-rw-   0        0        0     4841 2023-05-15 20:30:29.000000 doubleblind-1.0.1/docs/source/installation.rst
+-rw-rw-rw-   0        0        0       30 2019-07-11 11:49:50.000000 doubleblind-1.0.1/docs/source/readme.rst
+-rw-rw-rw-   0        0        0     3404 2023-07-02 18:55:20.000000 doubleblind-1.0.1/docs/source/user_guide.rst
+drwxrwxrwx   0        0        0        0 2023-07-11 10:42:06.508612 doubleblind-1.0.1/doubleblind/
+-rw-rw-rw-   0        0        0       71 2023-07-11 10:41:22.000000 doubleblind-1.0.1/doubleblind/__init__.py
+-rw-rw-rw-   0        0        0    11330 2023-06-03 10:22:45.000000 doubleblind-1.0.1/doubleblind/blinding.py
+-rw-rw-rw-   0        0        0     1574 2023-05-16 14:33:38.000000 doubleblind-1.0.1/doubleblind/editing.py
+-rw-rw-rw-   0        0        0     1563 2023-05-14 10:02:35.000000 doubleblind-1.0.1/doubleblind/favicon.icns
+-rw-rw-rw-   0        0        0    15406 2023-05-13 14:16:15.000000 doubleblind-1.0.1/doubleblind/favicon.ico
+-rw-rw-rw-   0        0        0    20340 2023-07-11 10:18:40.000000 doubleblind-1.0.1/doubleblind/gui.py
+-rw-rw-rw-   0        0        0     1515 2023-05-16 18:13:59.000000 doubleblind-1.0.1/doubleblind/gui_style.py
+-rw-rw-rw-   0        0        0      769 2023-05-14 13:21:37.000000 doubleblind-1.0.1/doubleblind/main.py
+-rw-rw-rw-   0        0        0      838 2023-05-13 14:59:20.000000 doubleblind-1.0.1/doubleblind/parametric_style.qss
+-rw-rw-rw-   0        0        0    52999 2023-05-13 14:14:46.000000 doubleblind-1.0.1/doubleblind/splash.png
+-rw-rw-rw-   0        0        0    53768 2023-05-13 14:14:17.000000 doubleblind-1.0.1/doubleblind/splash_transparent.png
+-rw-rw-rw-   0        0        0     3117 2023-06-03 10:22:45.000000 doubleblind-1.0.1/doubleblind/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:42:06.519659 doubleblind-1.0.1/doubleblind.egg-info/
+-rw-rw-rw-   0        0        0     5666 2023-07-11 10:42:03.000000 doubleblind-1.0.1/doubleblind.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4961 2023-07-11 10:42:06.000000 doubleblind-1.0.1/doubleblind.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 10:42:03.000000 doubleblind-1.0.1/doubleblind.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-07-11 10:42:03.000000 doubleblind-1.0.1/doubleblind.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       57 2023-07-11 10:42:03.000000 doubleblind-1.0.1/doubleblind.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-11 10:42:03.000000 doubleblind-1.0.1/doubleblind.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2880 2023-07-11 10:41:22.000000 doubleblind-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0      225 2023-05-16 18:39:17.000000 doubleblind-1.0.1/requirements_dev.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 10:42:06.561483 doubleblind-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-11 10:42:06.532523 doubleblind-1.0.1/tests/
+drwxrwxrwx   0        0        0        0 2023-07-11 10:42:06.538526 doubleblind-1.0.1/tests/.pytest_cache/
+-rw-rw-rw-   0        0        0       39 2023-05-15 09:11:55.000000 doubleblind-1.0.1/tests/.pytest_cache/.gitignore
+-rw-rw-rw-   0        0        0      191 2023-05-15 09:11:55.000000 doubleblind-1.0.1/tests/.pytest_cache/CACHEDIR.TAG
+-rw-rw-rw-   0        0        0      310 2023-05-15 09:11:55.000000 doubleblind-1.0.1/tests/.pytest_cache/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 10:42:06.347841 doubleblind-1.0.1/tests/.pytest_cache/v/
+drwxrwxrwx   0        0        0        0 2023-07-11 10:42:06.543528 doubleblind-1.0.1/tests/.pytest_cache/v/cache/
+-rw-rw-rw-   0        0        0     4681 2023-05-16 20:52:36.000000 doubleblind-1.0.1/tests/.pytest_cache/v/cache/lastfailed
+-rw-rw-rw-   0        0        0    10152 2023-05-16 20:52:36.000000 doubleblind-1.0.1/tests/.pytest_cache/v/cache/nodeids
+-rw-rw-rw-   0        0        0        2 2023-05-16 20:52:36.000000 doubleblind-1.0.1/tests/.pytest_cache/v/cache/stepwise
+-rw-rw-rw-   0        0        0     2661 2023-05-15 19:35:42.000000 doubleblind-1.0.1/tests/__init__.py
+-rw-rw-rw-   0        0        0       88 2023-02-01 15:09:59.000000 doubleblind-1.0.1/tests/conftest.py
+-rw-rw-rw-   0        0        0    15588 2023-05-16 20:51:51.000000 doubleblind-1.0.1/tests/test_blinding.py
+-rw-rw-rw-   0        0        0     3069 2023-05-16 14:36:19.000000 doubleblind-1.0.1/tests/test_editing.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:42:06.349849 doubleblind-1.0.1/tests/test_files/
+drwxrwxrwx   0        0        0        0 2023-07-11 10:42:06.549489 doubleblind-1.0.1/tests/test_files/root_dir/
+-rw-rw-rw-   0        0        0       64 2023-05-15 19:12:33.000000 doubleblind-1.0.1/tests/test_files/root_dir/dont_map.txt
+-rw-rw-rw-   0        0        0    10018 2023-05-15 19:13:18.000000 doubleblind-1.0.1/tests/test_files/root_dir/test workbook.xlsx
+-rw-rw-rw-   0        0        0       64 2023-05-15 19:24:03.000000 doubleblind-1.0.1/tests/test_files/root_dir/unmodified_file.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 10:42:06.559484 doubleblind-1.0.1/tests/test_files/unblind_additionals_truth/
+-rw-rw-rw-   0        0        0       64 2023-05-15 19:12:33.000000 doubleblind-1.0.1/tests/test_files/unblind_additionals_truth/dont_map.txt
+-rw-rw-rw-   0        0        0       64 2023-05-15 19:13:50.000000 doubleblind-1.0.1/tests/test_files/unblind_additionals_truth/dont_map_unblinded.txt
+-rw-rw-rw-   0        0        0    10018 2023-05-15 19:13:18.000000 doubleblind-1.0.1/tests/test_files/unblind_additionals_truth/test workbook.xlsx
+-rw-rw-rw-   0        0        0     5658 2023-05-15 19:53:13.000000 doubleblind-1.0.1/tests/test_files/unblind_additionals_truth/test workbook_unblinded.xlsx
+-rw-rw-rw-   0        0        0       64 2023-05-15 19:24:03.000000 doubleblind-1.0.1/tests/test_files/unblind_additionals_truth/unmodified_file.txt
+-rw-rw-rw-   0        0        0     4005 2023-05-16 19:41:00.000000 doubleblind-1.0.1/tests/test_gui.py
+-rw-rw-rw-   0        0        0     3636 2023-05-16 18:42:02.000000 doubleblind-1.0.1/tests/test_gui_style.py
+-rw-rw-rw-   0        0        0     2175 2023-05-15 10:10:28.000000 doubleblind-1.0.1/tests/test_utils.py
```

### Comparing `doubleblind-1.0.0/LICENSE` & `doubleblind-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `doubleblind-1.0.0/PKG-INFO` & `doubleblind-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doubleblind
-Version: 1.0.0
+Version: 1.0.1
 Summary: Automatically and reversibly replace file names with random strings to help experimenters quantify microscopy experiments blindly and maintain experimental integrity.
 Author-email: Guy Teichman <guyteichman@gmail.com>
 Maintainer-email: Guy Teichman <guyteichman@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Guy Teichman
```

### Comparing `doubleblind-1.0.0/README.rst` & `doubleblind-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `doubleblind-1.0.0/build/lib/doubleblind/favicon.ico` & `doubleblind-1.0.1/build/lib/doubleblind/favicon.ico`

 * *Files identical despite different names*

### Comparing `doubleblind-1.0.0/build/lib/doubleblind/splash.png` & `doubleblind-1.0.1/build/lib/doubleblind/splash.png`

 * *Files identical despite different names*

### Comparing `doubleblind-1.0.0/build/lib/doubleblind/splash_transparent.png` & `doubleblind-1.0.1/build/lib/doubleblind/splash_transparent.png`

 * *Files identical despite different names*

### Comparing `doubleblind-1.0.0/docs/build/_sources/index.rst.txt` & `doubleblind-1.0.1/docs/build/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `doubleblind-1.0.0/docs/build/_sources/installation.rst.txt` & `doubleblind-1.0.1/docs/build/_sources/installation.rst.txt`

 * *Files identical despite different names*

### Comparing `doubleblind-1.0.0/docs/build/_sources/user_guide.rst.txt` & `doubleblind-1.0.1/docs/build/_sources/user_guide.rst.txt`

 * *Files identical despite different names*

### Comparing `doubleblind-1.0.0/docs/build/_static/api_reference.rst` & `doubleblind-1.0.1/docs/build/_static/api_reference.rst`

 * *Files identical despite different names*

### Comparing `doubleblind-1.0.0/docs/build/_static/doubleblind.png` & `doubleblind-1.0.1/docs/build/_static/doubleblind.png`

 * *Files identical despite different names*

### Comparing `doubleblind-1.0.0/docs/build/_static/favicon.ico` & `doubleblind-1.0.1/docs/build/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `doubleblind-1.0.0/docs/build/_static/py.png` & `doubleblind-1.0.1/docs/build/_static/py.png`

 * *Files identical despite different names*

### Comparing `doubleblind-1.0.0/docs/source/_static/api_reference.rst` & `doubleblind-1.0.1/docs/source/_static/api_reference.rst`

 * *Files identical despite different names*

### Comparing `doubleblind-1.0.0/docs/source/conf.py` & `doubleblind-1.0.1/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'DoubleBlind'
 copyright = '2023, Guy Teichman'
 author = 'Guy Teichman'
 
 # The full version, including alpha/beta/rc tags
-release = '1.0.0'
+release = '1.0.1'
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = ['sphinx.ext.autodoc', 'sphinx.ext.autosummary', 'sphinx.ext.doctest']
```

### Comparing `doubleblind-1.0.0/docs/source/doubleblind.png` & `doubleblind-1.0.1/docs/source/doubleblind.png`

 * *Files identical despite different names*

### Comparing `doubleblind-1.0.0/docs/source/favicon.ico` & `doubleblind-1.0.1/docs/source/favicon.ico`

 * *Files identical despite different names*

### Comparing `doubleblind-1.0.0/docs/source/index.rst` & `doubleblind-1.0.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `doubleblind-1.0.0/docs/source/installation.rst` & `doubleblind-1.0.1/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `doubleblind-1.0.0/docs/source/user_guide.rst` & `doubleblind-1.0.1/docs/source/user_guide.rst`

 * *Files identical despite different names*

### Comparing `doubleblind-1.0.0/doubleblind/blinding.py` & `doubleblind-1.0.1/doubleblind/blinding.py`

 * *Files identical despite different names*

### Comparing `doubleblind-1.0.0/doubleblind/editing.py` & `doubleblind-1.0.1/doubleblind/editing.py`

 * *Files identical despite different names*

### Comparing `doubleblind-1.0.0/doubleblind/favicon.icns` & `doubleblind-1.0.1/doubleblind/favicon.icns`

 * *Files identical despite different names*

### Comparing `doubleblind-1.0.0/doubleblind/favicon.ico` & `doubleblind-1.0.1/doubleblind/favicon.ico`

 * *Files identical despite different names*

### Comparing `doubleblind-1.0.0/doubleblind/gui.py` & `doubleblind-1.0.1/doubleblind/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -358,16 +358,15 @@
         msg.setWindowTitle('Data blinded')
         msg.setText('Data was blinded successfully!')
         msg.exec()
 
 
 class DecodeTab(TabPage):
     PARAM_DESCS = TabPage.PARAM_DESCS.copy()
-    PARAM_DESCS[0] = ('file_types', 'File types to un-blind:',
-                       'Choose the type of files you want to un-blind. '),
+    PARAM_DESCS[0] = ('file_types', 'File types to un-blind:', 'Choose the type of files you want to un-blind. ')
     PARAM_DESCS.pop(3)
     PARAM_DESCS[3] = ('other_files', 'Replace blinded names in more files:\n(optional)',
                       'Folder with additional files (such as tables with quantification results) '
                       'which contain the blinded names. \n'
                       'DoubleBlind will look for the blinded names in these files, '
                       'and replace them with the original names. ')
```

### Comparing `doubleblind-1.0.0/doubleblind/gui_style.py` & `doubleblind-1.0.1/doubleblind/gui_style.py`

 * *Files identical despite different names*

### Comparing `doubleblind-1.0.0/doubleblind/main.py` & `doubleblind-1.0.1/doubleblind/main.py`

 * *Files identical despite different names*

### Comparing `doubleblind-1.0.0/doubleblind/parametric_style.qss` & `doubleblind-1.0.1/doubleblind/parametric_style.qss`

 * *Files identical despite different names*

### Comparing `doubleblind-1.0.0/doubleblind/splash.png` & `doubleblind-1.0.1/doubleblind/splash.png`

 * *Files identical despite different names*

### Comparing `doubleblind-1.0.0/doubleblind/splash_transparent.png` & `doubleblind-1.0.1/doubleblind/splash_transparent.png`

 * *Files identical despite different names*

### Comparing `doubleblind-1.0.0/doubleblind/utils.py` & `doubleblind-1.0.1/doubleblind/utils.py`

 * *Files identical despite different names*

### Comparing `doubleblind-1.0.0/doubleblind.egg-info/PKG-INFO` & `doubleblind-1.0.1/doubleblind.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doubleblind
-Version: 1.0.0
+Version: 1.0.1
 Summary: Automatically and reversibly replace file names with random strings to help experimenters quantify microscopy experiments blindly and maintain experimental integrity.
 Author-email: Guy Teichman <guyteichman@gmail.com>
 Maintainer-email: Guy Teichman <guyteichman@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Guy Teichman
```

### Comparing `doubleblind-1.0.0/doubleblind.egg-info/SOURCES.txt` & `doubleblind-1.0.1/doubleblind.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `doubleblind-1.0.0/pyproject.toml` & `doubleblind-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "doubleblind"  # Required
-version = "1.0.0"  # Required
+version = "1.0.1"  # Required
 description = "Automatically and reversibly replace file names with random strings to help experimenters quantify microscopy experiments blindly and maintain experimental integrity."
 readme = "README.rst" # Optional
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 keywords = ["microscopy", "blinding", "double-blind", "experiment", "rename"]
 authors = [{ name = "Guy Teichman", email = "guyteichman@gmail.com" }]
 maintainers = [{ name = "Guy Teichman", email = "guyteichman@gmail.com" }]
```

### Comparing `doubleblind-1.0.0/tests/.pytest_cache/v/cache/lastfailed` & `doubleblind-1.0.1/tests/.pytest_cache/v/cache/lastfailed`

 * *Files identical despite different names*

### Comparing `doubleblind-1.0.0/tests/.pytest_cache/v/cache/nodeids` & `doubleblind-1.0.1/tests/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `doubleblind-1.0.0/tests/__init__.py` & `doubleblind-1.0.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `doubleblind-1.0.0/tests/test_blinding.py` & `doubleblind-1.0.1/tests/test_blinding.py`

 * *Files identical despite different names*

### Comparing `doubleblind-1.0.0/tests/test_editing.py` & `doubleblind-1.0.1/tests/test_editing.py`

 * *Files identical despite different names*

### Comparing `doubleblind-1.0.0/tests/test_files/root_dir/test workbook.xlsx` & `doubleblind-1.0.1/tests/test_files/root_dir/test workbook.xlsx`

 * *Files identical despite different names*

### Comparing `doubleblind-1.0.0/tests/test_files/unblind_additionals_truth/test workbook.xlsx` & `doubleblind-1.0.1/tests/test_files/unblind_additionals_truth/test workbook.xlsx`

 * *Files identical despite different names*

### Comparing `doubleblind-1.0.0/tests/test_files/unblind_additionals_truth/test workbook_unblinded.xlsx` & `doubleblind-1.0.1/tests/test_files/unblind_additionals_truth/test workbook_unblinded.xlsx`

 * *Files identical despite different names*

### Comparing `doubleblind-1.0.0/tests/test_gui.py` & `doubleblind-1.0.1/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `doubleblind-1.0.0/tests/test_gui_style.py` & `doubleblind-1.0.1/tests/test_gui_style.py`

 * *Files identical despite different names*

### Comparing `doubleblind-1.0.0/tests/test_utils.py` & `doubleblind-1.0.1/tests/test_utils.py`

 * *Files identical despite different names*

