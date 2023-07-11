# Comparing `tmp/ephysiopy-1.9.22.tar.gz` & `tmp/ephysiopy-1.9.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ephysiopy-1.9.22.tar", last modified: Tue Jul  4 12:58:23 2023, max compression
+gzip compressed data, was "ephysiopy-1.9.23.tar", last modified: Mon Jul 10 14:35:49 2023, max compression
```

## Comparing `ephysiopy-1.9.22.tar` & `ephysiopy-1.9.23.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:58:23.482486 ephysiopy-1.9.22/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-04 12:58:23.482486 ephysiopy-1.9.22/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:58:23.478486 ephysiopy-1.9.22/ephysiopy/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:58:23.478486 ephysiopy-1.9.22/ephysiopy/axona/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/axona/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19336 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/axona/axonaIO.py
--rw-r--r--   0 runner    (1001) docker     (123)    11999 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/axona/file_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/axona/tetrode_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/axona/tintcolours.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:58:23.478486 ephysiopy-1.9.22/ephysiopy/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34668 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/common/binning.py
--rw-r--r--   0 runner    (1001) docker     (123)    21358 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/common/ephys_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    40221 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/common/fieldcalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/common/gridcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/common/mle_von_mises_vals.py
--rw-r--r--   0 runner    (1001) docker     (123)    49500 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/common/phasecoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    24931 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/common/rhythmicity.py
--rw-r--r--   0 runner    (1001) docker     (123)    28784 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/common/spikecalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/common/statscalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/common/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:58:23.478486 ephysiopy-1.9.22/ephysiopy/format_converters/
--rw-r--r--   0 runner    (1001) docker     (123)    19711 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/format_converters/OE_Axona.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/format_converters/OE_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/format_converters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:58:23.478486 ephysiopy-1.9.22/ephysiopy/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24089 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/io/recording.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:58:23.482486 ephysiopy-1.9.22/ephysiopy/openephys2py/
--rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/openephys2py/KiloSort.py
--rw-r--r--   0 runner    (1001) docker     (123)    10799 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/openephys2py/OESettings.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/openephys2py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:58:23.482486 ephysiopy-1.9.22/ephysiopy/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-04 12:58:16.000000 ephysiopy-1.9.22/ephysiopy/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-04 12:58:17.000000 ephysiopy-1.9.22/ephysiopy/tests/test_axona_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-04 12:58:17.000000 ephysiopy-1.9.22/ephysiopy/tests/test_axona_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-04 12:58:17.000000 ephysiopy-1.9.22/ephysiopy/tests/test_binning.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-04 12:58:17.000000 ephysiopy-1.9.22/ephysiopy/tests/test_dacq2py.py
--rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-07-04 12:58:17.000000 ephysiopy-1.9.22/ephysiopy/tests/test_ephys_generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-07-04 12:58:17.000000 ephysiopy-1.9.22/ephysiopy/tests/test_fieldcalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-04 12:58:17.000000 ephysiopy-1.9.22/ephysiopy/tests/test_gridcell.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-04 12:58:17.000000 ephysiopy-1.9.22/ephysiopy/tests/test_openephys.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-07-04 12:58:17.000000 ephysiopy-1.9.22/ephysiopy/tests/test_phasecoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-04 12:58:17.000000 ephysiopy-1.9.22/ephysiopy/tests/test_rhythmicity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-07-04 12:58:17.000000 ephysiopy-1.9.22/ephysiopy/tests/test_spikecalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-04 12:58:17.000000 ephysiopy-1.9.22/ephysiopy/tests/test_statscalcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-04 12:58:17.000000 ephysiopy-1.9.22/ephysiopy/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:58:23.482486 ephysiopy-1.9.22/ephysiopy/visualise/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 12:58:17.000000 ephysiopy-1.9.22/ephysiopy/visualise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32324 2023-07-04 12:58:17.000000 ephysiopy-1.9.22/ephysiopy/visualise/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 12:58:23.478486 ephysiopy-1.9.22/ephysiopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-04 12:58:23.000000 ephysiopy-1.9.22/ephysiopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-04 12:58:23.000000 ephysiopy-1.9.22/ephysiopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 12:58:23.000000 ephysiopy-1.9.22/ephysiopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-04 12:58:23.000000 ephysiopy-1.9.22/ephysiopy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-04 12:58:23.000000 ephysiopy-1.9.22/ephysiopy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-04 12:58:23.482486 ephysiopy-1.9.22/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-04 12:58:17.000000 ephysiopy-1.9.22/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:35:49.865101 ephysiopy-1.9.23/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-10 14:35:42.000000 ephysiopy-1.9.23/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-10 14:35:42.000000 ephysiopy-1.9.23/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-10 14:35:49.865101 ephysiopy-1.9.23/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-10 14:35:42.000000 ephysiopy-1.9.23/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:35:49.861101 ephysiopy-1.9.23/ephysiopy/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-10 14:35:42.000000 ephysiopy-1.9.23/ephysiopy/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-10 14:35:42.000000 ephysiopy-1.9.23/ephysiopy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:35:49.861101 ephysiopy-1.9.23/ephysiopy/axona/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:35:42.000000 ephysiopy-1.9.23/ephysiopy/axona/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19336 2023-07-10 14:35:42.000000 ephysiopy-1.9.23/ephysiopy/axona/axonaIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11999 2023-07-10 14:35:42.000000 ephysiopy-1.9.23/ephysiopy/axona/file_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-10 14:35:42.000000 ephysiopy-1.9.23/ephysiopy/axona/tetrode_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-10 14:35:42.000000 ephysiopy-1.9.23/ephysiopy/axona/tintcolours.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:35:49.861101 ephysiopy-1.9.23/ephysiopy/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:35:42.000000 ephysiopy-1.9.23/ephysiopy/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34668 2023-07-10 14:35:42.000000 ephysiopy-1.9.23/ephysiopy/common/binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21358 2023-07-10 14:35:42.000000 ephysiopy-1.9.23/ephysiopy/common/ephys_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40221 2023-07-10 14:35:42.000000 ephysiopy-1.9.23/ephysiopy/common/fieldcalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-07-10 14:35:42.000000 ephysiopy-1.9.23/ephysiopy/common/gridcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-07-10 14:35:42.000000 ephysiopy-1.9.23/ephysiopy/common/mle_von_mises_vals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49500 2023-07-10 14:35:42.000000 ephysiopy-1.9.23/ephysiopy/common/phasecoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24931 2023-07-10 14:35:42.000000 ephysiopy-1.9.23/ephysiopy/common/rhythmicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28776 2023-07-10 14:35:42.000000 ephysiopy-1.9.23/ephysiopy/common/spikecalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-07-10 14:35:42.000000 ephysiopy-1.9.23/ephysiopy/common/statscalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-07-10 14:35:42.000000 ephysiopy-1.9.23/ephysiopy/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:35:49.861101 ephysiopy-1.9.23/ephysiopy/format_converters/
+-rw-r--r--   0 runner    (1001) docker     (123)    19711 2023-07-10 14:35:42.000000 ephysiopy-1.9.23/ephysiopy/format_converters/OE_Axona.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-07-10 14:35:42.000000 ephysiopy-1.9.23/ephysiopy/format_converters/OE_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:35:42.000000 ephysiopy-1.9.23/ephysiopy/format_converters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:35:49.861101 ephysiopy-1.9.23/ephysiopy/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:35:42.000000 ephysiopy-1.9.23/ephysiopy/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25074 2023-07-10 14:35:42.000000 ephysiopy-1.9.23/ephysiopy/io/recording.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:35:49.861101 ephysiopy-1.9.23/ephysiopy/openephys2py/
+-rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-07-10 14:35:42.000000 ephysiopy-1.9.23/ephysiopy/openephys2py/KiloSort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12293 2023-07-10 14:35:42.000000 ephysiopy-1.9.23/ephysiopy/openephys2py/OESettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:35:42.000000 ephysiopy-1.9.23/ephysiopy/openephys2py/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:35:49.865101 ephysiopy-1.9.23/ephysiopy/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:35:42.000000 ephysiopy-1.9.23/ephysiopy/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-07-10 14:35:42.000000 ephysiopy-1.9.23/ephysiopy/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-07-10 14:35:43.000000 ephysiopy-1.9.23/ephysiopy/tests/test_axona_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-10 14:35:43.000000 ephysiopy-1.9.23/ephysiopy/tests/test_axona_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-10 14:35:43.000000 ephysiopy-1.9.23/ephysiopy/tests/test_binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-10 14:35:43.000000 ephysiopy-1.9.23/ephysiopy/tests/test_dacq2py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9325 2023-07-10 14:35:43.000000 ephysiopy-1.9.23/ephysiopy/tests/test_ephys_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-07-10 14:35:43.000000 ephysiopy-1.9.23/ephysiopy/tests/test_fieldcalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-10 14:35:43.000000 ephysiopy-1.9.23/ephysiopy/tests/test_gridcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-10 14:35:43.000000 ephysiopy-1.9.23/ephysiopy/tests/test_openephys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-07-10 14:35:43.000000 ephysiopy-1.9.23/ephysiopy/tests/test_phasecoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-10 14:35:43.000000 ephysiopy-1.9.23/ephysiopy/tests/test_rhythmicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-07-10 14:35:43.000000 ephysiopy-1.9.23/ephysiopy/tests/test_spikecalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-10 14:35:43.000000 ephysiopy-1.9.23/ephysiopy/tests/test_statscalcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-10 14:35:43.000000 ephysiopy-1.9.23/ephysiopy/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:35:49.865101 ephysiopy-1.9.23/ephysiopy/visualise/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 14:35:43.000000 ephysiopy-1.9.23/ephysiopy/visualise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32382 2023-07-10 14:35:43.000000 ephysiopy-1.9.23/ephysiopy/visualise/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 14:35:49.861101 ephysiopy-1.9.23/ephysiopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-10 14:35:49.000000 ephysiopy-1.9.23/ephysiopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-10 14:35:49.000000 ephysiopy-1.9.23/ephysiopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 14:35:49.000000 ephysiopy-1.9.23/ephysiopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-10 14:35:49.000000 ephysiopy-1.9.23/ephysiopy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 14:35:49.000000 ephysiopy-1.9.23/ephysiopy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-10 14:35:49.865101 ephysiopy-1.9.23/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-10 14:35:43.000000 ephysiopy-1.9.23/setup.py
```

### Comparing `ephysiopy-1.9.22/LICENSE` & `ephysiopy-1.9.23/LICENSE`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.22/PKG-INFO` & `ephysiopy-1.9.23/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ephysiopy
-Version: 1.9.22
+Version: 1.9.23
 Summary: Analysis of electrophysiology data
 Home-page: https://github.com/rhayman/ephysiopy
 Author: Robin Hayman
 Author-email: robin.hayman@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ephysiopy-1.9.22/README.md` & `ephysiopy-1.9.23/README.md`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.22/ephysiopy/axona/axonaIO.py` & `ephysiopy-1.9.23/ephysiopy/axona/axonaIO.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.22/ephysiopy/axona/file_headers.py` & `ephysiopy-1.9.23/ephysiopy/axona/file_headers.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.22/ephysiopy/axona/tetrode_dict.py` & `ephysiopy-1.9.23/ephysiopy/axona/tetrode_dict.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.22/ephysiopy/axona/tintcolours.py` & `ephysiopy-1.9.23/ephysiopy/axona/tintcolours.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.22/ephysiopy/common/binning.py` & `ephysiopy-1.9.23/ephysiopy/common/binning.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.22/ephysiopy/common/ephys_generic.py` & `ephysiopy-1.9.23/ephysiopy/common/ephys_generic.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.22/ephysiopy/common/fieldcalcs.py` & `ephysiopy-1.9.23/ephysiopy/common/fieldcalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.22/ephysiopy/common/gridcell.py` & `ephysiopy-1.9.23/ephysiopy/common/gridcell.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.22/ephysiopy/common/mle_von_mises_vals.py` & `ephysiopy-1.9.23/ephysiopy/common/mle_von_mises_vals.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.22/ephysiopy/common/phasecoding.py` & `ephysiopy-1.9.23/ephysiopy/common/phasecoding.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.22/ephysiopy/common/rhythmicity.py` & `ephysiopy-1.9.23/ephysiopy/common/rhythmicity.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.22/ephysiopy/common/spikecalcs.py` & `ephysiopy-1.9.23/ephysiopy/common/spikecalcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,23 +228,24 @@
         mask = np.logical_and(bins > 0, bins < n)
         return np.mean(counts[mask[1:]])
 
     def xcorr(
             self, x1: np.ndarray, x2=None,
             Trange=None, **kwargs) -> np.ndarray:
         """
-        Calculates the histogram of the ISIs in x1 or x1 vs x2
+        Calculates the ISIs in x1 or x1 vs x2 within a 
+        given range
 
         Parameters
         ----------
         x1, x2 : array_like
             The times of the spikes emitted by the cluster(s)
-            NB must be signed int to accomodate negative times
+            Assumed to be in milliseconds
         Trange : array_like
-            Range of times to bin up. Defaults to [-500, +500] in ms
+            Range of times to bin up in ms. Defaults to [-500, +500]
 
         Returns
         -------
         y : np.ndarray
             The time differences between spike times in x1 over the range
             of times defined Trange
         """
```

### Comparing `ephysiopy-1.9.22/ephysiopy/common/statscalcs.py` & `ephysiopy-1.9.23/ephysiopy/common/statscalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.22/ephysiopy/common/utils.py` & `ephysiopy-1.9.23/ephysiopy/common/utils.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.22/ephysiopy/format_converters/OE_Axona.py` & `ephysiopy-1.9.23/ephysiopy/format_converters/OE_Axona.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.22/ephysiopy/format_converters/OE_numpy.py` & `ephysiopy-1.9.23/ephysiopy/format_converters/OE_numpy.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.22/ephysiopy/io/recording.py` & `ephysiopy-1.9.23/ephysiopy/io/recording.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import abc
 import os
+import re
 import warnings
 from enum import Enum
 from pathlib import Path, PurePath
 from typing import NoReturn
 
 import h5py
 import numpy as np
@@ -33,21 +34,26 @@
 def memmapBinaryFile(path2file: str, n_channels=384, **kwargs) -> np.ndarray:
     """
     Returns a numpy memmap of the int16 data in the
     file path2file, if present
     """
     import os
 
+    if("data_type" in kwargs.keys()):
+        data_type = kwargs["data_type"]
+    else:
+        data_type = np.int16
+
     if os.path.exists(path2file):
         # make sure n_channels is int as could be str
         n_channels = int(n_channels)
         status = os.stat(path2file)
         n_samples = int(status.st_size / (2.0 * n_channels))
         mmap = np.memmap(
-            path2file, np.int16, "r", 0, (n_channels, n_samples), order="F"
+            path2file, data_type, "r", 0, (n_channels, n_samples), order="F"
         )
         return mmap
     else:
         return np.empty(0)
 
 
 def loadTrackingPluginData(pname: Path) -> np.ndarray:
@@ -354,24 +360,27 @@
 
 
 class OpenEphysBase(TrialInterface):
     def __init__(self, pname: Path, **kwargs) -> None:
         super().__init__(pname, **kwargs)
         setattr(self, "sync_message_file", None)
         self.load_settings()
-        record_methods = ["Acquisition Board",
-                          "Neuropix-PXI", "Sources/Neuropix-PXI",
-                          "Rhythm FPGA", "Sources/Rhythm FPGA"]
-        rec_method = [i for i in self.settings.processors.keys()
-                      if i in record_methods][0]
+        # The numbers after the strings in this list are the node id's 
+        # in openephys
+        record_methods = ["Acquisition Board [0-9][0-9][0-9]",
+                          "Neuropix-PXI [0-9][0-9][0-9]",
+                          "Sources/Neuropix-PXI [0-9][0-9][0-9]",
+                          "Rhythm FPGA [0-9][0-9][0-9]",
+                          "Sources/Rhythm FPGA [0-9][0-9][0-9]"]
+        rec_method = [re.search(m,k).string for k in self.settings.processors.keys() 
+                       for m in record_methods if re.search(m,k) is not None][0]
         if 'Sources/' in rec_method:
-            tmp_rec_method = rec_method.lstrip('Sources/')
-            self.rec_kind = Xml2RecordingKind[tmp_rec_method]
-        else:
-            self.rec_kind = Xml2RecordingKind[rec_method]
+            rec_method = rec_method.lstrip('Sources/')
+        
+        self.rec_kind = Xml2RecordingKind[rec_method.rpartition(" ")[0]]
 
         # Attempt to find the files contained in the parent directory
         # related to the recording with the default experiment and
         # recording name
         self.find_files(pname)
         self.sample_rate = None
         self.sample_rate = self.settings.processors[rec_method].sample_rate
@@ -511,15 +520,26 @@
                 "Could not find the pos data. \
                 Make sure there is a pos_data folder with data_array.npy \
                 and timestamps.npy in"
             )
         self.recording_start_time = recording_start_time
 
     def load_ttl(self, *args, **kwargs):
-        pass
+        ttl_ts = np.load(os.path.join(self.path2EventsData, "timestamps.npy"))
+        states = np.load(os.path.join(self.path2EventsData, "states.npy"))
+        if "StimControl_id" in kwargs.keys():
+            stim_id = kwargs['StimControl_id']
+            duration = getattr(self.settings.processors[stim_id], "Duration")
+            setattr(self, "stim_duration", int(duration))
+        if "TTL_channel_number" in kwargs.keys():
+            chan = kwargs["TTL_channel_number"]
+            high_ttl = ttl_ts[states==chan]
+            # get into ms
+            high_ttl = high_ttl * 1000.
+            setattr(self, "ttl_timestamps", high_ttl)
 
     def find_files(
         self,
         pname_root: str,
         experiment_name: str = "experiment1",
         rec_name: str = "recording1",
     ):
```

### Comparing `ephysiopy-1.9.22/ephysiopy/openephys2py/KiloSort.py` & `ephysiopy-1.9.23/ephysiopy/openephys2py/KiloSort.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.22/ephysiopy/openephys2py/OESettings.py` & `ephysiopy-1.9.23/ephysiopy/openephys2py/OESettings.py`

 * *Files 18% similar despite different names*

```diff
@@ -245,14 +245,59 @@
     subChannels: List[int] = field(default_factory=List)
     subChannelsThresh: List[int] = field(default_factory=List)
     subChannelsActive: List[int] = field(default_factory=List)
     prePeakSamples: int = field(default=8)
     postPeakSamples: int = field(default=32)
 
 
+class AbstractProcessorFactory():
+    def create_pos_tracker(self):
+        return PosTracker()
+    def create_rhythm_fpga(self):
+        return RhythmFPGA()
+    def create_neuropix_pxi(self):
+        return NeuropixPXI()
+    def create_acquisition_board(self):
+        return AcquisitionBoard()
+    def create_spike_sorter(self):
+        return SpikeSorter()
+    def create_track_me(self):
+        return TrackMe()
+    def create_record_node(self):
+        return RecordNode()
+    def create_stim_control(self):
+        return StimControl()
+    def create_oe_plugin(self):
+        return OEPlugin()
+    
+
+class ProcessorFactory():
+    factory = AbstractProcessorFactory()
+    def create_processor(self, proc_name: str):
+        if "Pos Tracker" in proc_name or "PosTracker" in proc_name:
+            return self.factory.create_pos_tracker()
+        elif "Rhythm" in proc_name:
+            return self.factory.create_rhythm_fpga()
+        elif "Neuropix-PXI" in proc_name:
+            return self.factory.create_neuropix_pxi()
+        elif "Acquisition Board" in proc_name:
+            return self.factory.create_acquisition_board()
+        elif "Spike Sorter" in proc_name:
+            return self.factory.create_spike_sorter()
+        elif "TrackMe" in proc_name:
+            return self.factory.create_track_me()
+        elif "Record Node" in proc_name:
+            return self.factory.create_record_node()
+        elif "StimControl" in proc_name:
+            return self.factory.create_stim_control()
+        else:
+            return self.factory.create_oe_plugin()
+    
+        
+
 def recurseNode(
                 node: xml.etree.ElementTree.Element,
                 func: Callable,
                 cls: dataclass):
     """
     Recursive function that applies func to each node
     """
@@ -264,44 +309,43 @@
         return
 
 
 def addValues2Class(node: xml.etree.ElementTree.Element, cls: dataclass):
     for i in node.items():
         if hasattr(cls, i[0]):
             setattr(cls, i[0], i[1])
+        if i == "GLOBAL_PARAMETERS":
+            print(i)
     if hasattr(cls, "channel_info") and node.tag == "CHANNEL":
         if cls.channel_info is None:
             cls.channel_info = list()
         chan = Channel()
         recurseNode(node, addValues2Class, chan)
         cls.channel_info.append(chan)
     if hasattr(cls, "stream") and node.tag == "STREAM":
         if cls.stream is None:
             cls.stream = Stream()
         recurseNode(node, addValues2Class, cls.stream)
-
+    
 
 class OEStructure(object):
     """
     Loads up the structure.oebin file for openephys flat binary
     format recordings
     """
 
-    def __init__(self, pname: str):
+    def __init__(self, fname: str):
         self.filename = []
         self.data = []
         import json
         import os
 
-        for d, _, f in os.walk(pname):
-            for ff in f:
-                if "structure.oebin" in ff:
-                    self.filename.append(os.path.join(d, ff))
-                    with open(os.path.join(d, ff), "r") as f:
-                        self.data.append(json.load(f))
+        self.filename.append(fname)
+        with open(fname, "r") as f:
+            self.data.append(json.load(f))
 
 
 class Settings(object):
     """
     Groups together the other classes in this module and does the actual
     parsing of the settings.xml file
 
@@ -329,15 +373,16 @@
             ("Pos Tracker", PosTracker()),
             ("PosTracker", PosTracker()),
             ("Rhythm FPGA", RhythmFPGA()),
             ("Neuropix-PXI", NeuropixPXI()),
             ("Acquisition Board", AcquisitionBoard()),
             ("Spike Sorter", SpikeSorter()),
             ("TrackMe", TrackMe()),
-            ("Record Node", RecordNode())
+            ("Record Node", RecordNode()),
+            ("StimControl", StimControl())
         ])
         self.processors = OrderedDict()
         self.record_nodes = OrderedDict()
         self.tracker_params = {}
         self.stimcontrol_params = {}
         self.load()
         self.parse()
@@ -353,33 +398,34 @@
         """
         Parses the basic information about the processors in the
         open-ephys signal chain and as described in the settings.xml
         file(s)
         """
         if self.tree is None:
             self.load()
+        processor_factory = ProcessorFactory()
         # quick hack to deal with flat binary format that has no settings.xml
         if self.tree is not None:
             for elem in self.tree.iter("PROCESSOR"):
                 i_proc = elem.get("name")
                 if "/" in i_proc:
                     i_proc = i_proc.split("/")[-1]
-                if i_proc == "Record Node":  # special as could be > 1
-                    recNode = RecordNode()
-                    recurseNode(elem, addValues2Class, recNode)
-                    if recNode.nodeId is not None:
-                        self.record_nodes[i_proc + " " + recNode.nodeId] = recNode
+                new_processor = processor_factory.create_processor(i_proc)
+                recurseNode(elem, addValues2Class, new_processor)
+                if i_proc == "Record Node":
+                    if new_processor.nodeId is not None:
+                        self.record_nodes[i_proc + " " + new_processor.nodeId] = new_processor
                     else:
-                        self.record_nodes[i_proc] = recNode
-                elif i_proc in self.possible_processors.keys():
-                    self.processors[i_proc] = self.possible_processors[i_proc]
-                    recurseNode(elem, addValues2Class, self.processors[i_proc])
+                        self.record_nodes[i_proc] = new_processor
                 else:
-                    self.processors[i_proc] = OEPlugin()
-                    recurseNode(elem, addValues2Class, self.processors[i_proc])
+                    if new_processor.nodeId is not None:
+                        self.processors[i_proc + " " + new_processor.nodeId] = new_processor
+                    else:
+                        self.processors[i_proc] = new_processor
+                
 
     def parseStimControl(self):
         """
         Parses information attached to the StimControl module I wrote
         """
         if len(self.processors) == 0:
             self.parse()
```

### Comparing `ephysiopy-1.9.22/ephysiopy/tests/conftest.py` & `ephysiopy-1.9.23/ephysiopy/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.22/ephysiopy/tests/test_axona_headers.py` & `ephysiopy-1.9.23/ephysiopy/tests/test_axona_headers.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.22/ephysiopy/tests/test_axona_io.py` & `ephysiopy-1.9.23/ephysiopy/tests/test_axona_io.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.22/ephysiopy/tests/test_binning.py` & `ephysiopy-1.9.23/ephysiopy/tests/test_binning.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.22/ephysiopy/tests/test_dacq2py.py` & `ephysiopy-1.9.23/ephysiopy/tests/test_dacq2py.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.22/ephysiopy/tests/test_ephys_generic.py` & `ephysiopy-1.9.23/ephysiopy/tests/test_ephys_generic.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.22/ephysiopy/tests/test_fieldcalcs.py` & `ephysiopy-1.9.23/ephysiopy/tests/test_fieldcalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.22/ephysiopy/tests/test_gridcell.py` & `ephysiopy-1.9.23/ephysiopy/tests/test_gridcell.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.22/ephysiopy/tests/test_phasecoding.py` & `ephysiopy-1.9.23/ephysiopy/tests/test_phasecoding.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.22/ephysiopy/tests/test_rhythmicity.py` & `ephysiopy-1.9.23/ephysiopy/tests/test_rhythmicity.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.22/ephysiopy/tests/test_spikecalcs.py` & `ephysiopy-1.9.23/ephysiopy/tests/test_spikecalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.22/ephysiopy/tests/test_statscalcs.py` & `ephysiopy-1.9.23/ephysiopy/tests/test_statscalcs.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.22/ephysiopy/tests/test_utils.py` & `ephysiopy-1.9.23/ephysiopy/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.22/ephysiopy/visualise/plotting.py` & `ephysiopy-1.9.23/ephysiopy/visualise/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -371,28 +371,31 @@
         divider = make_axes_locatable(axScatter)
         axScatter.set_xticks((dt[0], 0, dt[1]))
         axScatter.set_xticklabels((str(dt[0]), '0', str(dt[1])))
         axHistx = divider.append_axes("top", 0.95, pad=0.2, sharex=axScatter,
                                       transform=axScatter.transAxes)
         scattTrans = transforms.blended_transform_factory(axScatter.transData,
                                                           axScatter.transAxes)
-        stim_pwidth = int(self.settings['stim_pwidth'])
+        stim_pwidth = getattr(self, "stim_duration", None)
+        if stim_pwidth is None:
+            raise ValueError("stim duration is None")
+
         axScatter.add_patch(
             Rectangle(
-                (0, 0), width=stim_pwidth/1000., height=1,
+                (0, 0), width=stim_pwidth, height=1,
                 transform=scattTrans,
                 color=[0, 0, 1], alpha=0.5))
         histTrans = transforms.blended_transform_factory(axHistx.transData,
                                                          axHistx.transAxes)
-        axHistx.add_patch(Rectangle((0, 0), width=stim_pwidth/1000., height=1,
+        axHistx.add_patch(Rectangle((0, 0), width=stim_pwidth, height=1,
                           transform=histTrans,
                           color=[0, 0, 1], alpha=0.5))
         axScatter.set_ylabel('Laser stimulation events', labelpad=-18.5)
         axScatter.set_xlabel('Time to stimulus onset(ms)')
-        nStms = int(self.STM['num_stm_samples'])
+        nStms = len(on_good)
         axScatter.set_ylim(0, nStms)
         # Label only the min and max of the y-axis
         ylabels = axScatter.get_yticklabels()
         for i in range(1, len(ylabels)-1):
             ylabels[i].set_visible(False)
         yticks = axScatter.get_yticklines()
         for i in range(1, len(yticks)-1):
```

### Comparing `ephysiopy-1.9.22/ephysiopy.egg-info/PKG-INFO` & `ephysiopy-1.9.23/ephysiopy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ephysiopy
-Version: 1.9.22
+Version: 1.9.23
 Summary: Analysis of electrophysiology data
 Home-page: https://github.com/rhayman/ephysiopy
 Author: Robin Hayman
 Author-email: robin.hayman@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ephysiopy-1.9.22/ephysiopy.egg-info/SOURCES.txt` & `ephysiopy-1.9.23/ephysiopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ephysiopy-1.9.22/setup.py` & `ephysiopy-1.9.23/setup.py`

 * *Files identical despite different names*

