# Comparing `tmp/wwvb-3.0.4.tar.gz` & `tmp/wwvb-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwvb-3.0.4.tar", last modified: Sun May  7 19:41:40 2023, max compression
+gzip compressed data, was "wwvb-3.0.5.tar", last modified: Tue Jul 11 15:12:50 2023, max compression
```

## Comparing `wwvb-3.0.4.tar` & `wwvb-3.0.5.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 19:41:40.649159 wwvb-3.0.4/
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-05-07 19:41:12.000000 wwvb-3.0.4/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 19:41:40.641159 wwvb-3.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 19:41:40.641159 wwvb-3.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-05-07 19:41:12.000000 wwvb-3.0.4/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-05-07 19:41:12.000000 wwvb-3.0.4/.github/workflows/cron.yml
--rw-r--r--   0 runner    (1001) docker     (122)      875 2023-05-07 19:41:12.000000 wwvb-3.0.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1722 2023-05-07 19:41:12.000000 wwvb-3.0.4/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (122)      221 2023-05-07 19:41:12.000000 wwvb-3.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      844 2023-05-07 19:41:12.000000 wwvb-3.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      244 2023-05-07 19:41:12.000000 wwvb-3.0.4/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 19:41:40.641159 wwvb-3.0.4/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (122)    10280 2023-05-07 19:41:12.000000 wwvb-3.0.4/LICENSES/Apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)     7048 2023-05-07 19:41:12.000000 wwvb-3.0.4/LICENSES/CC0-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)    34670 2023-05-07 19:41:12.000000 wwvb-3.0.4/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1211 2023-05-07 19:41:12.000000 wwvb-3.0.4/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-05-07 19:41:12.000000 wwvb-3.0.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)    10180 2023-05-07 19:41:40.649159 wwvb-3.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     9406 2023-05-07 19:41:12.000000 wwvb-3.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 19:41:40.641159 wwvb-3.0.4/_static/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-07 19:41:12.000000 wwvb-3.0.4/_static/.empty
--rw-r--r--   0 runner    (1001) docker     (122)    13365 2023-05-07 19:41:12.000000 wwvb-3.0.4/adafruit_datetime.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-07 19:41:12.000000 wwvb-3.0.4/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2653 2023-05-07 19:41:12.000000 wwvb-3.0.4/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      412 2023-05-07 19:41:12.000000 wwvb-3.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      441 2023-05-07 19:41:12.000000 wwvb-3.0.4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1196 2023-05-07 19:41:40.649159 wwvb-3.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 19:41:40.641159 wwvb-3.0.4/src/
--rw-r--r--   0 runner    (1001) docker     (122)     5718 2023-05-07 19:41:12.000000 wwvb-3.0.4/src/uwwvb.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 19:41:40.645159 wwvb-3.0.4/src/wwvb/
--rw-r--r--   0 runner    (1001) docker     (122)    30051 2023-05-07 19:41:12.000000 wwvb-3.0.4/src/wwvb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-07 19:41:40.000000 wwvb-3.0.4/src/wwvb/__version__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2851 2023-05-07 19:41:12.000000 wwvb-3.0.4/src/wwvb/decode.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      889 2023-05-07 19:41:12.000000 wwvb-3.0.4/src/wwvb/dut1table.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3893 2023-05-07 19:41:12.000000 wwvb-3.0.4/src/wwvb/gen.py
--rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-05-07 19:41:12.000000 wwvb-3.0.4/src/wwvb/iersdata.py
--rw-r--r--   0 runner    (1001) docker     (122)     2394 2023-05-07 19:41:12.000000 wwvb-3.0.4/src/wwvb/iersdata_dist.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-07 19:41:12.000000 wwvb-3.0.4/src/wwvb/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     8524 2023-05-07 19:41:12.000000 wwvb-3.0.4/src/wwvb/testcli.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2637 2023-05-07 19:41:12.000000 wwvb-3.0.4/src/wwvb/testdaylight.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1750 2023-05-07 19:41:12.000000 wwvb-3.0.4/src/wwvb/testls.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1103 2023-05-07 19:41:12.000000 wwvb-3.0.4/src/wwvb/testpm.py
--rw-r--r--   0 runner    (1001) docker     (122)     8590 2023-05-07 19:41:12.000000 wwvb-3.0.4/src/wwvb/testuwwvb.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    16504 2023-05-07 19:41:12.000000 wwvb-3.0.4/src/wwvb/testwwvb.py
--rw-r--r--   0 runner    (1001) docker     (122)      299 2023-05-07 19:41:12.000000 wwvb-3.0.4/src/wwvb/tz.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     7501 2023-05-07 19:41:12.000000 wwvb-3.0.4/src/wwvb/updateiers.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3344 2023-05-07 19:41:12.000000 wwvb-3.0.4/src/wwvb/wwvbtk.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 19:41:40.645159 wwvb-3.0.4/src/wwvb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    10180 2023-05-07 19:41:40.000000 wwvb-3.0.4/src/wwvb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1391 2023-05-07 19:41:40.000000 wwvb-3.0.4/src/wwvb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-07 19:41:40.000000 wwvb-3.0.4/src/wwvb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      179 2023-05-07 19:41:40.000000 wwvb-3.0.4/src/wwvb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      106 2023-05-07 19:41:40.000000 wwvb-3.0.4/src/wwvb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-07 19:41:40.000000 wwvb-3.0.4/src/wwvb.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-07 19:41:40.649159 wwvb-3.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      694 2023-05-07 19:41:12.000000 wwvb-3.0.4/tests/1998leapsecond
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-05-07 19:41:12.000000 wwvb-3.0.4/tests/2012leapsecond
--rw-r--r--   0 runner    (1001) docker     (122)     1599 2023-05-07 19:41:12.000000 wwvb-3.0.4/tests/all-headers
--rw-r--r--   0 runner    (1001) docker     (122)     5136 2023-05-07 19:41:12.000000 wwvb-3.0.4/tests/bar
--rw-r--r--   0 runner    (1001) docker     (122)     1719 2023-05-07 19:41:12.000000 wwvb-3.0.4/tests/both
--rw-r--r--   0 runner    (1001) docker     (122)      939 2023-05-07 19:41:12.000000 wwvb-3.0.4/tests/cradek
--rw-r--r--   0 runner    (1001) docker     (122)      941 2023-05-07 19:41:12.000000 wwvb-3.0.4/tests/duration
--rw-r--r--   0 runner    (1001) docker     (122)      940 2023-05-07 19:41:12.000000 wwvb-3.0.4/tests/enddst-phase
--rw-r--r--   0 runner    (1001) docker     (122)      940 2023-05-07 19:41:12.000000 wwvb-3.0.4/tests/enddst-phase-2
--rw-r--r--   0 runner    (1001) docker     (122)      459 2023-05-07 19:41:12.000000 wwvb-3.0.4/tests/endleapyear
--rw-r--r--   0 runner    (1001) docker     (122)      382 2023-05-07 19:41:12.000000 wwvb-3.0.4/tests/leapday1
--rw-r--r--   0 runner    (1001) docker     (122)      382 2023-05-07 19:41:12.000000 wwvb-3.0.4/tests/leapday28
--rw-r--r--   0 runner    (1001) docker     (122)      382 2023-05-07 19:41:12.000000 wwvb-3.0.4/tests/leapday29
--rw-r--r--   0 runner    (1001) docker     (122)      691 2023-05-07 19:41:12.000000 wwvb-3.0.4/tests/negleapsecond
--rw-r--r--   0 runner    (1001) docker     (122)      536 2023-05-07 19:41:12.000000 wwvb-3.0.4/tests/nextdst
--rw-r--r--   0 runner    (1001) docker     (122)      536 2023-05-07 19:41:12.000000 wwvb-3.0.4/tests/nextst
--rw-r--r--   0 runner    (1001) docker     (122)      382 2023-05-07 19:41:12.000000 wwvb-3.0.4/tests/nonleapday1
--rw-r--r--   0 runner    (1001) docker     (122)      382 2023-05-07 19:41:12.000000 wwvb-3.0.4/tests/nonleapday28
--rw-r--r--   0 runner    (1001) docker     (122)      940 2023-05-07 19:41:12.000000 wwvb-3.0.4/tests/phase
--rw-r--r--   0 runner    (1001) docker     (122)      536 2023-05-07 19:41:12.000000 wwvb-3.0.4/tests/startdst
--rw-r--r--   0 runner    (1001) docker     (122)      940 2023-05-07 19:41:12.000000 wwvb-3.0.4/tests/startdst-phase
--rw-r--r--   0 runner    (1001) docker     (122)      940 2023-05-07 19:41:12.000000 wwvb-3.0.4/tests/startdst-phase-2
--rw-r--r--   0 runner    (1001) docker     (122)      459 2023-05-07 19:41:12.000000 wwvb-3.0.4/tests/startleapyear
--rw-r--r--   0 runner    (1001) docker     (122)      536 2023-05-07 19:41:12.000000 wwvb-3.0.4/tests/startst
--rw-r--r--   0 runner    (1001) docker     (122)      921 2023-05-07 19:41:12.000000 wwvb-3.0.4/tests/y2k
--rw-r--r--   0 runner    (1001) docker     (122)      921 2023-05-07 19:41:12.000000 wwvb-3.0.4/tests/y2k-1
--rw-r--r--   0 runner    (1001) docker     (122)      613 2023-05-07 19:41:12.000000 wwvb-3.0.4/tests/y2k1
--rw-r--r--   0 runner    (1001) docker     (122)      613 2023-05-07 19:41:12.000000 wwvb-3.0.4/tests/y2k1-1
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:12:50.253451 wwvb-3.0.5/
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-07-11 15:12:24.000000 wwvb-3.0.5/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:12:50.245451 wwvb-3.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:12:50.249451 wwvb-3.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-07-11 15:12:24.000000 wwvb-3.0.5/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-07-11 15:12:24.000000 wwvb-3.0.5/.github/workflows/cron.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      875 2023-07-11 15:12:24.000000 wwvb-3.0.5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1722 2023-07-11 15:12:24.000000 wwvb-3.0.5/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-07-11 15:12:24.000000 wwvb-3.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      844 2023-07-11 15:12:24.000000 wwvb-3.0.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      244 2023-07-11 15:12:24.000000 wwvb-3.0.5/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:12:50.249451 wwvb-3.0.5/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (122)    10280 2023-07-11 15:12:24.000000 wwvb-3.0.5/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     7048 2023-07-11 15:12:24.000000 wwvb-3.0.5/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    34670 2023-07-11 15:12:24.000000 wwvb-3.0.5/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1211 2023-07-11 15:12:24.000000 wwvb-3.0.5/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-07-11 15:12:24.000000 wwvb-3.0.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)    10180 2023-07-11 15:12:50.253451 wwvb-3.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     9406 2023-07-11 15:12:24.000000 wwvb-3.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:12:50.249451 wwvb-3.0.5/_static/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-11 15:12:24.000000 wwvb-3.0.5/_static/.empty
+-rw-r--r--   0 runner    (1001) docker     (122)    13365 2023-07-11 15:12:24.000000 wwvb-3.0.5/adafruit_datetime.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-11 15:12:24.000000 wwvb-3.0.5/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2653 2023-07-11 15:12:24.000000 wwvb-3.0.5/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      412 2023-07-11 15:12:24.000000 wwvb-3.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      486 2023-07-11 15:12:24.000000 wwvb-3.0.5/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1196 2023-07-11 15:12:50.253451 wwvb-3.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:12:50.249451 wwvb-3.0.5/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     5718 2023-07-11 15:12:24.000000 wwvb-3.0.5/src/uwwvb.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:12:50.249451 wwvb-3.0.5/src/wwvb/
+-rw-r--r--   0 runner    (1001) docker     (122)    30051 2023-07-11 15:12:24.000000 wwvb-3.0.5/src/wwvb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-07-11 15:12:50.000000 wwvb-3.0.5/src/wwvb/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2851 2023-07-11 15:12:24.000000 wwvb-3.0.5/src/wwvb/decode.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      889 2023-07-11 15:12:24.000000 wwvb-3.0.5/src/wwvb/dut1table.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3893 2023-07-11 15:12:24.000000 wwvb-3.0.5/src/wwvb/gen.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-07-11 15:12:24.000000 wwvb-3.0.5/src/wwvb/iersdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2394 2023-07-11 15:12:24.000000 wwvb-3.0.5/src/wwvb/iersdata_dist.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-11 15:12:24.000000 wwvb-3.0.5/src/wwvb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     8524 2023-07-11 15:12:24.000000 wwvb-3.0.5/src/wwvb/testcli.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2637 2023-07-11 15:12:24.000000 wwvb-3.0.5/src/wwvb/testdaylight.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1750 2023-07-11 15:12:24.000000 wwvb-3.0.5/src/wwvb/testls.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1103 2023-07-11 15:12:24.000000 wwvb-3.0.5/src/wwvb/testpm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8590 2023-07-11 15:12:24.000000 wwvb-3.0.5/src/wwvb/testuwwvb.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    16504 2023-07-11 15:12:24.000000 wwvb-3.0.5/src/wwvb/testwwvb.py
+-rw-r--r--   0 runner    (1001) docker     (122)      299 2023-07-11 15:12:24.000000 wwvb-3.0.5/src/wwvb/tz.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     7501 2023-07-11 15:12:24.000000 wwvb-3.0.5/src/wwvb/updateiers.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     3344 2023-07-11 15:12:24.000000 wwvb-3.0.5/src/wwvb/wwvbtk.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:12:50.253451 wwvb-3.0.5/src/wwvb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    10180 2023-07-11 15:12:50.000000 wwvb-3.0.5/src/wwvb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1391 2023-07-11 15:12:50.000000 wwvb-3.0.5/src/wwvb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-11 15:12:50.000000 wwvb-3.0.5/src/wwvb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      179 2023-07-11 15:12:50.000000 wwvb-3.0.5/src/wwvb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-07-11 15:12:50.000000 wwvb-3.0.5/src/wwvb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-07-11 15:12:50.000000 wwvb-3.0.5/src/wwvb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 15:12:50.253451 wwvb-3.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      694 2023-07-11 15:12:24.000000 wwvb-3.0.5/tests/1998leapsecond
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-11 15:12:24.000000 wwvb-3.0.5/tests/2012leapsecond
+-rw-r--r--   0 runner    (1001) docker     (122)     1599 2023-07-11 15:12:24.000000 wwvb-3.0.5/tests/all-headers
+-rw-r--r--   0 runner    (1001) docker     (122)     5136 2023-07-11 15:12:24.000000 wwvb-3.0.5/tests/bar
+-rw-r--r--   0 runner    (1001) docker     (122)     1719 2023-07-11 15:12:24.000000 wwvb-3.0.5/tests/both
+-rw-r--r--   0 runner    (1001) docker     (122)      939 2023-07-11 15:12:24.000000 wwvb-3.0.5/tests/cradek
+-rw-r--r--   0 runner    (1001) docker     (122)      941 2023-07-11 15:12:24.000000 wwvb-3.0.5/tests/duration
+-rw-r--r--   0 runner    (1001) docker     (122)      940 2023-07-11 15:12:24.000000 wwvb-3.0.5/tests/enddst-phase
+-rw-r--r--   0 runner    (1001) docker     (122)      940 2023-07-11 15:12:24.000000 wwvb-3.0.5/tests/enddst-phase-2
+-rw-r--r--   0 runner    (1001) docker     (122)      459 2023-07-11 15:12:24.000000 wwvb-3.0.5/tests/endleapyear
+-rw-r--r--   0 runner    (1001) docker     (122)      382 2023-07-11 15:12:24.000000 wwvb-3.0.5/tests/leapday1
+-rw-r--r--   0 runner    (1001) docker     (122)      382 2023-07-11 15:12:24.000000 wwvb-3.0.5/tests/leapday28
+-rw-r--r--   0 runner    (1001) docker     (122)      382 2023-07-11 15:12:24.000000 wwvb-3.0.5/tests/leapday29
+-rw-r--r--   0 runner    (1001) docker     (122)      691 2023-07-11 15:12:24.000000 wwvb-3.0.5/tests/negleapsecond
+-rw-r--r--   0 runner    (1001) docker     (122)      536 2023-07-11 15:12:24.000000 wwvb-3.0.5/tests/nextdst
+-rw-r--r--   0 runner    (1001) docker     (122)      536 2023-07-11 15:12:24.000000 wwvb-3.0.5/tests/nextst
+-rw-r--r--   0 runner    (1001) docker     (122)      382 2023-07-11 15:12:24.000000 wwvb-3.0.5/tests/nonleapday1
+-rw-r--r--   0 runner    (1001) docker     (122)      382 2023-07-11 15:12:24.000000 wwvb-3.0.5/tests/nonleapday28
+-rw-r--r--   0 runner    (1001) docker     (122)      940 2023-07-11 15:12:24.000000 wwvb-3.0.5/tests/phase
+-rw-r--r--   0 runner    (1001) docker     (122)      536 2023-07-11 15:12:24.000000 wwvb-3.0.5/tests/startdst
+-rw-r--r--   0 runner    (1001) docker     (122)      940 2023-07-11 15:12:24.000000 wwvb-3.0.5/tests/startdst-phase
+-rw-r--r--   0 runner    (1001) docker     (122)      940 2023-07-11 15:12:24.000000 wwvb-3.0.5/tests/startdst-phase-2
+-rw-r--r--   0 runner    (1001) docker     (122)      459 2023-07-11 15:12:24.000000 wwvb-3.0.5/tests/startleapyear
+-rw-r--r--   0 runner    (1001) docker     (122)      536 2023-07-11 15:12:24.000000 wwvb-3.0.5/tests/startst
+-rw-r--r--   0 runner    (1001) docker     (122)      921 2023-07-11 15:12:24.000000 wwvb-3.0.5/tests/y2k
+-rw-r--r--   0 runner    (1001) docker     (122)      921 2023-07-11 15:12:24.000000 wwvb-3.0.5/tests/y2k-1
+-rw-r--r--   0 runner    (1001) docker     (122)      613 2023-07-11 15:12:24.000000 wwvb-3.0.5/tests/y2k1
+-rw-r--r--   0 runner    (1001) docker     (122)      613 2023-07-11 15:12:24.000000 wwvb-3.0.5/tests/y2k1-1
```

### Comparing `wwvb-3.0.4/.github/workflows/codeql.yml` & `wwvb-3.0.5/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/.github/workflows/cron.yml` & `wwvb-3.0.5/.github/workflows/cron.yml`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/.github/workflows/release.yml` & `wwvb-3.0.5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/.github/workflows/test.yml` & `wwvb-3.0.5/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/.pre-commit-config.yaml` & `wwvb-3.0.5/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 # SPDX-License-Identifier: Unlicense
 
 default_language_version:
   python: python3
 
 repos:
 - repo: https://github.com/psf/black
-  rev: 23.1.0
+  rev: 23.7.0
   hooks:
   - id: black
 - repo: https://github.com/pre-commit/pre-commit-hooks
   rev: v4.4.0
   hooks:
   -   id: check-yaml
   -   id: end-of-file-fixer
       exclude: tests
   -   id: trailing-whitespace
       exclude: tests
 - repo: https://github.com/fsfe/reuse-tool
-  rev: v1.1.2
+  rev: v2.0.0
   hooks:
   - id: reuse
 - repo: https://github.com/pycqa/pylint
   rev: v2.17.1
   hooks:
   - id: pylint
     additional_dependencies: [beautifulsoup4, requests, adafruit-circuitpython-datetime, click, python-dateutil, leapseconddata]
```

### Comparing `wwvb-3.0.4/LICENSES/Apache-2.0.txt` & `wwvb-3.0.5/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/LICENSES/CC0-1.0.txt` & `wwvb-3.0.5/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/LICENSES/GPL-3.0-only.txt` & `wwvb-3.0.5/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/LICENSES/Unlicense.txt` & `wwvb-3.0.5/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/Makefile` & `wwvb-3.0.5/Makefile`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/PKG-INFO` & `wwvb-3.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwvb
-Version: 3.0.4
+Version: 3.0.5
 Summary: Generate WWVB timecodes for any desired time
 Home-page: https://github.com/jepler/wwvbpy
 Author: Jeff Epler
 Author-email: jepler@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `wwvb-3.0.4/README.md` & `wwvb-3.0.5/README.md`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/adafruit_datetime.pyi` & `wwvb-3.0.5/adafruit_datetime.pyi`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/conf.py` & `wwvb-3.0.5/conf.py`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/setup.cfg` & `wwvb-3.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/src/uwwvb.py` & `wwvb-3.0.5/src/uwwvb.py`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/src/wwvb/__init__.py` & `wwvb-3.0.5/src/wwvb/__init__.py`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/src/wwvb/decode.py` & `wwvb-3.0.5/src/wwvb/decode.py`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/src/wwvb/dut1table.py` & `wwvb-3.0.5/src/wwvb/dut1table.py`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/src/wwvb/gen.py` & `wwvb-3.0.5/src/wwvb/gen.py`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/src/wwvb/iersdata.py` & `wwvb-3.0.5/src/wwvb/iersdata.py`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/src/wwvb/iersdata_dist.py` & `wwvb-3.0.5/src/wwvb/iersdata_dist.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,9 +31,9 @@
     +g*49+f*18+p*59+o*53+n*52+m*57+l*48+k*53+j*127+i*70+h*30     # 19990303
     +r*62+q*79+p*152+o*82+n*106+m*184+l*125+k*217+j*133+i*252    # 20030402
     +h*161+g*392+f*322+e*290+n*116+m*154+l*85+k*83+j*91+i*168    # 20080312
     +h*105+g*147+f*105+e*42+o*70+n*91+m*154+l*119+k*84+j*217     # 20110511
     +i*126+h*176+g*97+f*91+e*52+o*116+n*98+m*70+l*133+k*91+j*91  # 20140507
     +i*77+h*140+g*91+f*84+e*70+d*34+n*72+m*76+l*66+k*53+j*56     # 20160831
     +i*105+h*77+g*45+q*25+p*63+o*91+n*154+m*105+l*190+k*118      # 20190501
-    +j*105+i*807+j*376+k*411+l*45+k*88+l*22+k*6+l*8+k*67         # 20240504
+    +j*105+i*807+j*376+k*710                                     # 20240706
 )
```

### Comparing `wwvb-3.0.4/src/wwvb/testcli.py` & `wwvb-3.0.5/src/wwvb/testcli.py`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/src/wwvb/testdaylight.py` & `wwvb-3.0.5/src/wwvb/testdaylight.py`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/src/wwvb/testls.py` & `wwvb-3.0.5/src/wwvb/testls.py`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/src/wwvb/testpm.py` & `wwvb-3.0.5/src/wwvb/testpm.py`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/src/wwvb/testuwwvb.py` & `wwvb-3.0.5/src/wwvb/testuwwvb.py`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/src/wwvb/testwwvb.py` & `wwvb-3.0.5/src/wwvb/testwwvb.py`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/src/wwvb/updateiers.py` & `wwvb-3.0.5/src/wwvb/updateiers.py`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/src/wwvb/wwvbtk.py` & `wwvb-3.0.5/src/wwvb/wwvbtk.py`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/src/wwvb.egg-info/PKG-INFO` & `wwvb-3.0.5/src/wwvb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwvb
-Version: 3.0.4
+Version: 3.0.5
 Summary: Generate WWVB timecodes for any desired time
 Home-page: https://github.com/jepler/wwvbpy
 Author: Jeff Epler
 Author-email: jepler@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `wwvb-3.0.4/src/wwvb.egg-info/SOURCES.txt` & `wwvb-3.0.5/src/wwvb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/tests/1998leapsecond` & `wwvb-3.0.5/tests/1998leapsecond`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/tests/all-headers` & `wwvb-3.0.5/tests/all-headers`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/tests/bar` & `wwvb-3.0.5/tests/bar`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/tests/both` & `wwvb-3.0.5/tests/both`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/tests/cradek` & `wwvb-3.0.5/tests/cradek`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/tests/duration` & `wwvb-3.0.5/tests/duration`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/tests/enddst-phase` & `wwvb-3.0.5/tests/enddst-phase`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/tests/enddst-phase-2` & `wwvb-3.0.5/tests/enddst-phase-2`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/tests/negleapsecond` & `wwvb-3.0.5/tests/negleapsecond`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/tests/nextdst` & `wwvb-3.0.5/tests/nextdst`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/tests/nextst` & `wwvb-3.0.5/tests/nextst`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/tests/phase` & `wwvb-3.0.5/tests/phase`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/tests/startdst` & `wwvb-3.0.5/tests/startdst`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/tests/startdst-phase` & `wwvb-3.0.5/tests/startdst-phase`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/tests/startdst-phase-2` & `wwvb-3.0.5/tests/startdst-phase-2`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/tests/startst` & `wwvb-3.0.5/tests/startst`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/tests/y2k` & `wwvb-3.0.5/tests/y2k`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/tests/y2k-1` & `wwvb-3.0.5/tests/y2k-1`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/tests/y2k1` & `wwvb-3.0.5/tests/y2k1`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.4/tests/y2k1-1` & `wwvb-3.0.5/tests/y2k1-1`

 * *Files identical despite different names*

