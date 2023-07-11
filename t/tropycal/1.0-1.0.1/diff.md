# Comparing `tmp/tropycal-1.0.tar.gz` & `tmp/tropycal-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tropycal-1.0.tar", last modified: Sun Jul  2 19:56:54 2023, max compression
+gzip compressed data, was "tropycal-1.0.1.tar", last modified: Tue Jul 11 20:23:31 2023, max compression
```

## Comparing `tropycal-1.0.tar` & `tropycal-1.0.1.tar`

### file list

```diff
@@ -1,162 +1,162 @@
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-02 19:56:54.559933 tropycal-1.0/
--rw-r--r--   0 tomerburg   (501) staff       (20)       66 2022-10-12 23:32:59.000000 tropycal-1.0/.gitattributes
--rw-r--r--   0 tomerburg   (501) staff       (20)      113 2022-10-12 23:32:59.000000 tropycal-1.0/.gitignore
--rw-r--r--   0 tomerburg   (501) staff       (20)     2485 2022-10-12 23:32:59.000000 tropycal-1.0/.travis.yml
--rw-r--r--   0 tomerburg   (501) staff       (20)     1057 2022-10-12 23:32:59.000000 tropycal-1.0/LICENSE
--rw-r--r--   0 tomerburg   (501) staff       (20)       16 2022-10-12 23:32:59.000000 tropycal-1.0/MANIFEST.in
--rw-r--r--   0 tomerburg   (501) staff       (20)     5060 2023-07-02 19:56:54.560047 tropycal-1.0/PKG-INFO
--rw-r--r--   0 tomerburg   (501) staff       (20)     4366 2023-07-02 19:56:43.000000 tropycal-1.0/README.md
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-02 19:56:54.498901 tropycal-1.0/ci/
--rw-r--r--   0 tomerburg   (501) staff       (20)     4452 2022-10-12 23:32:59.000000 tropycal-1.0/ci/deploy_key.enc
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-02 19:56:54.502188 tropycal-1.0/docs/
--rw-r--r--   0 tomerburg   (501) staff       (20)      642 2022-12-11 19:25:29.000000 tropycal-1.0/docs/Makefile
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-02 19:56:54.524254 tropycal-1.0/docs/_static/
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-02 19:56:54.525757 tropycal-1.0/docs/_static/css/
--rw-r--r--   0 tomerburg   (501) staff       (20)     3275 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_static/css/badge_only.css
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-02 19:56:54.539221 tropycal-1.0/docs/_static/css/fonts/
--rw-r--r--   0 tomerburg   (501) staff       (20)    87624 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0 tomerburg   (501) staff       (20)    67312 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0 tomerburg   (501) staff       (20)    86288 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0 tomerburg   (501) staff       (20)    66444 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0 tomerburg   (501) staff       (20)   165742 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0 tomerburg   (501) staff       (20)   444379 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0 tomerburg   (501) staff       (20)   165548 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 tomerburg   (501) staff       (20)    98024 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0 tomerburg   (501) staff       (20)    77160 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 tomerburg   (501) staff       (20)   323344 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0 tomerburg   (501) staff       (20)   193308 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0 tomerburg   (501) staff       (20)   309728 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_static/css/fonts/lato-bold.woff
--rw-r--r--   0 tomerburg   (501) staff       (20)   184912 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0 tomerburg   (501) staff       (20)   328412 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0 tomerburg   (501) staff       (20)   195704 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0 tomerburg   (501) staff       (20)   309192 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_static/css/fonts/lato-normal.woff
--rw-r--r--   0 tomerburg   (501) staff       (20)   182708 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0 tomerburg   (501) staff       (20)   135191 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_static/css/theme.css
--rw-r--r--   0 tomerburg   (501) staff       (20)   530613 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_static/dorian.png
--rw-r--r--   0 tomerburg   (501) staff       (20)   665534 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_static/grid_example_1.png
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-02 19:56:54.540112 tropycal-1.0/docs/_static/js/
--rw-r--r--   0 tomerburg   (501) staff       (20)      934 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_static/js/badge_only.js
--rw-r--r--   0 tomerburg   (501) staff       (20)     5023 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_static/js/theme.js
--rw-r--r--   0 tomerburg   (501) staff       (20)    11979 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_static/logo.png
--rw-r--r--   0 tomerburg   (501) staff       (20)    94302 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_static/logo_32.ico
--rw-r--r--   0 tomerburg   (501) staff       (20)   566670 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_static/michael_example_1.png
--rw-r--r--   0 tomerburg   (501) staff       (20)   612897 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_static/michael_example_2.png
--rw-r--r--   0 tomerburg   (501) staff       (20)   565722 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_static/michael_example_3.png
--rw-r--r--   0 tomerburg   (501) staff       (20)   583690 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_static/michael_example_4.png
--rw-r--r--   0 tomerburg   (501) staff       (20)   446960 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_static/storm_example_1.png
--rw-r--r--   0 tomerburg   (501) staff       (20)   401309 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_static/storm_example_2.png
--rw-r--r--   0 tomerburg   (501) staff       (20)   398432 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_static/storm_example_3.png
--rw-r--r--   0 tomerburg   (501) staff       (20)      328 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_static/theme_override.css
--rw-r--r--   0 tomerburg   (501) staff       (20)   726348 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_static/tornado_example_1.png
--rw-r--r--   0 tomerburg   (501) staff       (20)   307446 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_static/tornado_example_2.png
--rw-r--r--   0 tomerburg   (501) staff       (20)   172063 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_static/tornado_example_3.png
--rw-r--r--   0 tomerburg   (501) staff       (20)   152687 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_static/tornado_example_5.png
--rw-r--r--   0 tomerburg   (501) staff       (20)   277793 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_static/trackdataset_example_1.png
--rw-r--r--   0 tomerburg   (501) staff       (20)   357620 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_static/trackdataset_example_2.png
--rw-r--r--   0 tomerburg   (501) staff       (20)   245771 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_static/trackdataset_example_3.png
--rw-r--r--   0 tomerburg   (501) staff       (20)   217745 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_static/trackdataset_example_4.png
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-02 19:56:54.493476 tropycal-1.0/docs/_templates/
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-02 19:56:54.541432 tropycal-1.0/docs/_templates/autosummary/
--rw-r--r--   0 tomerburg   (501) staff       (20)      181 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_templates/autosummary/base.rst
--rw-r--r--   0 tomerburg   (501) staff       (20)      699 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0 tomerburg   (501) staff       (20)     1210 2022-10-12 23:32:59.000000 tropycal-1.0/docs/_templates/autosummary/module.rst
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-02 19:56:54.541638 tropycal-1.0/docs/_templates/overrides/
--rw-r--r--   0 tomerburg   (501) staff       (20)      772 2023-07-02 19:56:43.000000 tropycal-1.0/docs/_templates/overrides/tropycal.utils.rst
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-02 19:56:54.542014 tropycal-1.0/docs/api/
--rw-r--r--   0 tomerburg   (501) staff       (20)      698 2023-07-02 19:56:43.000000 tropycal-1.0/docs/api/index.rst
--rw-r--r--   0 tomerburg   (501) staff       (20)     7515 2023-07-02 19:56:43.000000 tropycal-1.0/docs/conf.py
--rw-r--r--   0 tomerburg   (501) staff       (20)     6077 2022-10-12 23:32:59.000000 tropycal-1.0/docs/data.rst
--rw-r--r--   0 tomerburg   (501) staff       (20)     1619 2023-07-02 19:56:43.000000 tropycal-1.0/docs/index.rst
--rw-r--r--   0 tomerburg   (501) staff       (20)      935 2022-10-12 23:32:59.000000 tropycal-1.0/docs/install.rst
--rw-r--r--   0 tomerburg   (501) staff       (20)     1108 2022-10-12 23:32:59.000000 tropycal-1.0/docs/make.bat
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-02 19:56:54.542842 tropycal-1.0/docs/options/
--rw-r--r--   0 tomerburg   (501) staff       (20)     2094 2022-12-09 19:59:04.000000 tropycal-1.0/docs/options/domain.rst
--rw-r--r--   0 tomerburg   (501) staff       (20)      102 2022-10-12 23:32:59.000000 tropycal-1.0/docs/options/gridded_stats.rst
--rw-r--r--   0 tomerburg   (501) staff       (20)    10181 2022-12-09 19:59:04.000000 tropycal-1.0/docs/options/map_prop.rst
--rw-r--r--   0 tomerburg   (501) staff       (20)       76 2022-10-12 23:32:59.000000 tropycal-1.0/docs/requirements.txt
--rw-r--r--   0 tomerburg   (501) staff       (20)      554 2022-10-12 23:32:59.000000 tropycal-1.0/docs/sample_usage.rst
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-02 19:56:54.543577 tropycal-1.0/docs/samples/
--rw-r--r--   0 tomerburg   (501) staff       (20)     6253 2022-10-12 23:32:59.000000 tropycal-1.0/docs/samples/tracks.TrackDataset.rst
--rw-r--r--   0 tomerburg   (501) staff       (20)    10328 2022-10-12 23:32:59.000000 tropycal-1.0/docs/samples/tracks.storm.rst
--rw-r--r--   0 tomerburg   (501) staff       (20)     4359 2022-10-12 23:32:59.000000 tropycal-1.0/docs/samples/tracks.tornado.rst
--rw-r--r--   0 tomerburg   (501) staff       (20)      505 2022-12-09 19:59:04.000000 tropycal-1.0/docs/support.rst
--rw-r--r--   0 tomerburg   (501) staff       (20)      114 2022-12-15 14:18:51.000000 tropycal-1.0/docs/test.py
--rw-r--r--   0 tomerburg   (501) staff       (20)     7375 2022-10-12 23:32:59.000000 tropycal-1.0/docs/tropycal_full_logo.png
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-02 19:56:54.546879 tropycal-1.0/examples/
--rw-r--r--   0 tomerburg   (501) staff       (20)       96 2022-10-12 23:32:59.000000 tropycal-1.0/examples/README.txt
--rw-r--r--   0 tomerburg   (501) staff       (20)     5534 2023-06-28 02:18:34.000000 tropycal-1.0/examples/analogs.py
--rw-r--r--   0 tomerburg   (501) staff       (20)    10897 2023-07-02 19:56:43.000000 tropycal-1.0/examples/cartopy.py
--rw-r--r--   0 tomerburg   (501) staff       (20)     6171 2023-06-28 02:18:34.000000 tropycal-1.0/examples/customize_storm.py
--rw-r--r--   0 tomerburg   (501) staff       (20)     6297 2023-06-28 02:18:34.000000 tropycal-1.0/examples/realtime.py
--rw-r--r--   0 tomerburg   (501) staff       (20)     7105 2023-06-28 02:18:34.000000 tropycal-1.0/examples/recon.py
--rw-r--r--   0 tomerburg   (501) staff       (20)     4456 2023-07-02 19:56:43.000000 tropycal-1.0/examples/ships.py
--rw-r--r--   0 tomerburg   (501) staff       (20)     5164 2023-06-28 02:18:34.000000 tropycal-1.0/examples/tc_rainfall.py
--rw-r--r--   0 tomerburg   (501) staff       (20)     8733 2023-07-02 19:56:43.000000 tropycal-1.0/examples/tracks.TrackDataset.py
--rw-r--r--   0 tomerburg   (501) staff       (20)     2757 2023-07-02 19:56:43.000000 tropycal-1.0/examples/tracks.season.py
--rw-r--r--   0 tomerburg   (501) staff       (20)     7465 2023-06-28 02:18:34.000000 tropycal-1.0/examples/tracks.storm.py
--rw-r--r--   0 tomerburg   (501) staff       (20)     4451 2023-06-28 02:18:34.000000 tropycal-1.0/examples/tracks.tornado.py
--rw-r--r--   0 tomerburg   (501) staff       (20)      995 2023-07-02 19:56:54.560435 tropycal-1.0/setup.cfg
--rw-r--r--   0 tomerburg   (501) staff       (20)      121 2023-07-02 19:56:43.000000 tropycal-1.0/setup.py
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-02 19:56:54.494749 tropycal-1.0/src/
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-02 19:56:54.547950 tropycal-1.0/src/tropycal/
--rw-r--r--   0 tomerburg   (501) staff       (20)      159 2022-12-15 14:18:51.000000 tropycal-1.0/src/tropycal/__init__.py
--rw-r--r--   0 tomerburg   (501) staff       (20)      447 2022-12-15 14:18:51.000000 tropycal-1.0/src/tropycal/_version.py
--rw-r--r--   0 tomerburg   (501) staff       (20)     5103 2023-07-02 19:56:43.000000 tropycal-1.0/src/tropycal/constants.py
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-02 19:56:54.549367 tropycal-1.0/src/tropycal/plot/
--rw-r--r--   0 tomerburg   (501) staff       (20)       23 2023-07-02 19:56:43.000000 tropycal-1.0/src/tropycal/plot/__init__.py
--rw-r--r--   0 tomerburg   (501) staff       (20)    14158 2023-07-02 19:56:43.000000 tropycal-1.0/src/tropycal/plot/plot.py
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-02 19:56:54.550651 tropycal-1.0/src/tropycal/rain/
--rw-r--r--   0 tomerburg   (501) staff       (20)      184 2023-07-02 19:56:43.000000 tropycal-1.0/src/tropycal/rain/__init__.py
--rw-r--r--   0 tomerburg   (501) staff       (20)    11110 2023-07-02 19:56:43.000000 tropycal-1.0/src/tropycal/rain/dataset.py
--rw-r--r--   0 tomerburg   (501) staff       (20)    27902 2023-07-02 19:56:43.000000 tropycal-1.0/src/tropycal/rain/plot.py
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-02 19:56:54.552048 tropycal-1.0/src/tropycal/realtime/
--rw-r--r--   0 tomerburg   (501) staff       (20)      132 2023-07-02 19:56:43.000000 tropycal-1.0/src/tropycal/realtime/__init__.py
--rw-r--r--   0 tomerburg   (501) staff       (20)    37999 2023-07-02 19:56:43.000000 tropycal-1.0/src/tropycal/realtime/realtime.py
--rw-r--r--   0 tomerburg   (501) staff       (20)    47715 2023-07-02 19:56:43.000000 tropycal-1.0/src/tropycal/realtime/storm.py
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-02 19:56:54.553976 tropycal-1.0/src/tropycal/recon/
--rw-r--r--   0 tomerburg   (501) staff       (20)      240 2023-07-02 19:56:43.000000 tropycal-1.0/src/tropycal/recon/__init__.py
--rw-r--r--   0 tomerburg   (501) staff       (20)   122579 2023-07-02 19:56:43.000000 tropycal-1.0/src/tropycal/recon/dataset.py
--rw-r--r--   0 tomerburg   (501) staff       (20)    39097 2023-07-02 19:56:43.000000 tropycal-1.0/src/tropycal/recon/plot.py
--rw-r--r--   0 tomerburg   (501) staff       (20)    39275 2023-07-02 19:56:43.000000 tropycal-1.0/src/tropycal/recon/realtime.py
--rw-r--r--   0 tomerburg   (501) staff       (20)    63621 2023-07-02 19:56:43.000000 tropycal-1.0/src/tropycal/recon/tools.py
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-02 19:56:54.554550 tropycal-1.0/src/tropycal/ships/
--rw-r--r--   0 tomerburg   (501) staff       (20)       85 2023-07-02 19:56:43.000000 tropycal-1.0/src/tropycal/ships/__init__.py
--rw-r--r--   0 tomerburg   (501) staff       (20)    15819 2023-07-02 19:56:43.000000 tropycal-1.0/src/tropycal/ships/ships.py
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-02 19:56:54.555486 tropycal-1.0/src/tropycal/tornado/
--rw-r--r--   0 tomerburg   (501) staff       (20)      176 2023-07-02 19:56:43.000000 tropycal-1.0/src/tropycal/tornado/__init__.py
--rw-r--r--   0 tomerburg   (501) staff       (20)    15765 2023-07-02 19:56:43.000000 tropycal-1.0/src/tropycal/tornado/dataset.py
--rw-r--r--   0 tomerburg   (501) staff       (20)     8853 2023-07-02 19:56:43.000000 tropycal-1.0/src/tropycal/tornado/plot.py
--rw-r--r--   0 tomerburg   (501) staff       (20)     1941 2023-07-02 19:56:43.000000 tropycal-1.0/src/tropycal/tornado/tools.py
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-02 19:56:54.557065 tropycal-1.0/src/tropycal/tracks/
--rw-r--r--   0 tomerburg   (501) staff       (20)      224 2023-07-02 19:56:43.000000 tropycal-1.0/src/tropycal/tracks/__init__.py
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-02 19:56:54.557705 tropycal-1.0/src/tropycal/tracks/data/
--rw-r--r--   0 tomerburg   (501) staff       (20)     1249 2023-07-02 19:56:43.000000 tropycal-1.0/src/tropycal/tracks/data/catarina.csv
--rw-r--r--   0 tomerburg   (501) staff       (20)     1924 2023-07-02 19:56:43.000000 tropycal-1.0/src/tropycal/tracks/data/pacific_2006.csv
--rw-r--r--   0 tomerburg   (501) staff       (20)   213770 2023-07-02 19:56:43.000000 tropycal-1.0/src/tropycal/tracks/dataset.py
--rw-r--r--   0 tomerburg   (501) staff       (20)   129964 2023-07-02 19:56:43.000000 tropycal-1.0/src/tropycal/tracks/plot.py
--rw-r--r--   0 tomerburg   (501) staff       (20)    20570 2023-07-02 19:56:43.000000 tropycal-1.0/src/tropycal/tracks/season.py
--rw-r--r--   0 tomerburg   (501) staff       (20)   123468 2023-07-02 19:56:43.000000 tropycal-1.0/src/tropycal/tracks/storm.py
--rw-r--r--   0 tomerburg   (501) staff       (20)    31259 2023-07-02 19:56:43.000000 tropycal-1.0/src/tropycal/tracks/tools.py
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-02 19:56:54.558530 tropycal-1.0/src/tropycal/utils/
--rw-r--r--   0 tomerburg   (501) staff       (20)      132 2022-10-12 23:32:59.000000 tropycal-1.0/src/tropycal/utils/__init__.py
--rw-r--r--   0 tomerburg   (501) staff       (20)    10482 2023-07-02 19:56:43.000000 tropycal-1.0/src/tropycal/utils/cartopy_utils.py
--rw-r--r--   0 tomerburg   (501) staff       (20)    11465 2023-07-02 19:56:43.000000 tropycal-1.0/src/tropycal/utils/colors.py
--rw-r--r--   0 tomerburg   (501) staff       (20)    71423 2023-07-02 19:56:43.000000 tropycal-1.0/src/tropycal/utils/generic_utils.py
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-02 19:56:54.548800 tropycal-1.0/src/tropycal.egg-info/
--rw-r--r--   0 tomerburg   (501) staff       (20)     5060 2023-07-02 19:56:54.000000 tropycal-1.0/src/tropycal.egg-info/PKG-INFO
--rw-r--r--   0 tomerburg   (501) staff       (20)     3897 2023-07-02 19:56:54.000000 tropycal-1.0/src/tropycal.egg-info/SOURCES.txt
--rw-r--r--   0 tomerburg   (501) staff       (20)        1 2023-07-02 19:56:54.000000 tropycal-1.0/src/tropycal.egg-info/dependency_links.txt
--rw-r--r--   0 tomerburg   (501) staff       (20)      119 2023-07-02 19:56:54.000000 tropycal-1.0/src/tropycal.egg-info/requires.txt
--rw-r--r--   0 tomerburg   (501) staff       (20)        9 2023-07-02 19:56:54.000000 tropycal-1.0/src/tropycal.egg-info/top_level.txt
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-02 19:56:54.496365 tropycal-1.0/tests/
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-02 19:56:54.558986 tropycal-1.0/tests/data/
--rw-r--r--   0 tomerburg   (501) staff       (20)   136603 2023-07-02 19:56:43.000000 tropycal-1.0/tests/data/sample_hurdat.txt
--rw-r--r--   0 tomerburg   (501) staff       (20)      782 2023-07-02 19:56:43.000000 tropycal-1.0/tests/data/sample_storm.txt
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-02 19:56:54.559148 tropycal-1.0/tests/ships/
--rw-r--r--   0 tomerburg   (501) staff       (20)     3566 2023-07-02 19:56:43.000000 tropycal-1.0/tests/ships/test_ships.py
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-02 19:56:54.559629 tropycal-1.0/tests/tracks/
--rw-r--r--   0 tomerburg   (501) staff       (20)     4840 2023-07-02 19:56:43.000000 tropycal-1.0/tests/tracks/test_dataset.py
--rw-r--r--   0 tomerburg   (501) staff       (20)     1599 2023-07-02 19:56:43.000000 tropycal-1.0/tests/tracks/test_season.py
--rw-r--r--   0 tomerburg   (501) staff       (20)     6755 2023-07-02 19:56:43.000000 tropycal-1.0/tests/tracks/test_storm.py
-drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-02 19:56:54.559784 tropycal-1.0/tests/utils/
--rw-r--r--   0 tomerburg   (501) staff       (20)    19452 2023-07-02 19:56:43.000000 tropycal-1.0/tests/utils/test_utils.py
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.578859 tropycal-1.0.1/
+-rw-r--r--   0 tomerburg   (501) staff       (20)       66 2023-07-02 20:17:03.000000 tropycal-1.0.1/.gitattributes
+-rw-r--r--   0 tomerburg   (501) staff       (20)      113 2023-07-02 20:17:03.000000 tropycal-1.0.1/.gitignore
+-rw-r--r--   0 tomerburg   (501) staff       (20)     2485 2023-07-02 20:17:03.000000 tropycal-1.0.1/.travis.yml
+-rw-r--r--   0 tomerburg   (501) staff       (20)     1057 2023-07-02 20:17:03.000000 tropycal-1.0.1/LICENSE
+-rw-r--r--   0 tomerburg   (501) staff       (20)       16 2023-07-02 20:17:03.000000 tropycal-1.0.1/MANIFEST.in
+-rw-r--r--   0 tomerburg   (501) staff       (20)     5064 2023-07-11 20:23:31.578991 tropycal-1.0.1/PKG-INFO
+-rw-r--r--   0 tomerburg   (501) staff       (20)     4368 2023-07-11 20:14:34.000000 tropycal-1.0.1/README.md
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.507597 tropycal-1.0.1/ci/
+-rw-r--r--   0 tomerburg   (501) staff       (20)     4452 2023-07-02 20:17:03.000000 tropycal-1.0.1/ci/deploy_key.enc
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.510573 tropycal-1.0.1/docs/
+-rw-r--r--   0 tomerburg   (501) staff       (20)      642 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/Makefile
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.534414 tropycal-1.0.1/docs/_static/
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.535685 tropycal-1.0.1/docs/_static/css/
+-rw-r--r--   0 tomerburg   (501) staff       (20)     3275 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/css/badge_only.css
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.553894 tropycal-1.0.1/docs/_static/css/fonts/
+-rw-r--r--   0 tomerburg   (501) staff       (20)    87624 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-r--r--   0 tomerburg   (501) staff       (20)    67312 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-r--r--   0 tomerburg   (501) staff       (20)    86288 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-r--r--   0 tomerburg   (501) staff       (20)    66444 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-r--r--   0 tomerburg   (501) staff       (20)   165742 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/css/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 tomerburg   (501) staff       (20)   444379 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 tomerburg   (501) staff       (20)   165548 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/css/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 tomerburg   (501) staff       (20)    98024 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/css/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 tomerburg   (501) staff       (20)    77160 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/css/fonts/fontawesome-webfont.woff2
+-rw-r--r--   0 tomerburg   (501) staff       (20)   323344 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/css/fonts/lato-bold-italic.woff
+-rw-r--r--   0 tomerburg   (501) staff       (20)   193308 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/css/fonts/lato-bold-italic.woff2
+-rw-r--r--   0 tomerburg   (501) staff       (20)   309728 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/css/fonts/lato-bold.woff
+-rw-r--r--   0 tomerburg   (501) staff       (20)   184912 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/css/fonts/lato-bold.woff2
+-rw-r--r--   0 tomerburg   (501) staff       (20)   328412 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/css/fonts/lato-normal-italic.woff
+-rw-r--r--   0 tomerburg   (501) staff       (20)   195704 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/css/fonts/lato-normal-italic.woff2
+-rw-r--r--   0 tomerburg   (501) staff       (20)   309192 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/css/fonts/lato-normal.woff
+-rw-r--r--   0 tomerburg   (501) staff       (20)   182708 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/css/fonts/lato-normal.woff2
+-rw-r--r--   0 tomerburg   (501) staff       (20)   135191 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/css/theme.css
+-rw-r--r--   0 tomerburg   (501) staff       (20)   530613 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/dorian.png
+-rw-r--r--   0 tomerburg   (501) staff       (20)   665534 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/grid_example_1.png
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.554759 tropycal-1.0.1/docs/_static/js/
+-rw-r--r--   0 tomerburg   (501) staff       (20)      934 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/js/badge_only.js
+-rw-r--r--   0 tomerburg   (501) staff       (20)     5023 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/js/theme.js
+-rw-r--r--   0 tomerburg   (501) staff       (20)    11979 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/logo.png
+-rw-r--r--   0 tomerburg   (501) staff       (20)    94302 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/logo_32.ico
+-rw-r--r--   0 tomerburg   (501) staff       (20)   566670 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/michael_example_1.png
+-rw-r--r--   0 tomerburg   (501) staff       (20)   612897 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/michael_example_2.png
+-rw-r--r--   0 tomerburg   (501) staff       (20)   565722 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/michael_example_3.png
+-rw-r--r--   0 tomerburg   (501) staff       (20)   583690 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/michael_example_4.png
+-rw-r--r--   0 tomerburg   (501) staff       (20)   446960 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/storm_example_1.png
+-rw-r--r--   0 tomerburg   (501) staff       (20)   401309 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/storm_example_2.png
+-rw-r--r--   0 tomerburg   (501) staff       (20)   398432 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/storm_example_3.png
+-rw-r--r--   0 tomerburg   (501) staff       (20)      328 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/theme_override.css
+-rw-r--r--   0 tomerburg   (501) staff       (20)   726348 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/tornado_example_1.png
+-rw-r--r--   0 tomerburg   (501) staff       (20)   307446 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/tornado_example_2.png
+-rw-r--r--   0 tomerburg   (501) staff       (20)   172063 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/tornado_example_3.png
+-rw-r--r--   0 tomerburg   (501) staff       (20)   152687 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/tornado_example_5.png
+-rw-r--r--   0 tomerburg   (501) staff       (20)   277793 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/trackdataset_example_1.png
+-rw-r--r--   0 tomerburg   (501) staff       (20)   357620 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/trackdataset_example_2.png
+-rw-r--r--   0 tomerburg   (501) staff       (20)   245771 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/trackdataset_example_3.png
+-rw-r--r--   0 tomerburg   (501) staff       (20)   217745 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_static/trackdataset_example_4.png
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.501813 tropycal-1.0.1/docs/_templates/
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.555634 tropycal-1.0.1/docs/_templates/autosummary/
+-rw-r--r--   0 tomerburg   (501) staff       (20)      181 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 tomerburg   (501) staff       (20)      699 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 tomerburg   (501) staff       (20)     1210 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_templates/autosummary/module.rst
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.555894 tropycal-1.0.1/docs/_templates/overrides/
+-rw-r--r--   0 tomerburg   (501) staff       (20)      772 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/_templates/overrides/tropycal.utils.rst
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.556150 tropycal-1.0.1/docs/api/
+-rw-r--r--   0 tomerburg   (501) staff       (20)      698 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/api/index.rst
+-rw-r--r--   0 tomerburg   (501) staff       (20)     7517 2023-07-11 20:15:12.000000 tropycal-1.0.1/docs/conf.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)     6077 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/data.rst
+-rw-r--r--   0 tomerburg   (501) staff       (20)     1622 2023-07-11 20:16:05.000000 tropycal-1.0.1/docs/index.rst
+-rw-r--r--   0 tomerburg   (501) staff       (20)      935 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/install.rst
+-rw-r--r--   0 tomerburg   (501) staff       (20)     1108 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/make.bat
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.556950 tropycal-1.0.1/docs/options/
+-rw-r--r--   0 tomerburg   (501) staff       (20)     2094 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/options/domain.rst
+-rw-r--r--   0 tomerburg   (501) staff       (20)      102 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/options/gridded_stats.rst
+-rw-r--r--   0 tomerburg   (501) staff       (20)    10181 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/options/map_prop.rst
+-rw-r--r--   0 tomerburg   (501) staff       (20)       76 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/requirements.txt
+-rw-r--r--   0 tomerburg   (501) staff       (20)      554 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/sample_usage.rst
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.558647 tropycal-1.0.1/docs/samples/
+-rw-r--r--   0 tomerburg   (501) staff       (20)     6253 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/samples/tracks.TrackDataset.rst
+-rw-r--r--   0 tomerburg   (501) staff       (20)    10328 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/samples/tracks.storm.rst
+-rw-r--r--   0 tomerburg   (501) staff       (20)     4359 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/samples/tracks.tornado.rst
+-rw-r--r--   0 tomerburg   (501) staff       (20)      505 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/support.rst
+-rw-r--r--   0 tomerburg   (501) staff       (20)      114 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/test.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)     7375 2023-07-02 20:17:03.000000 tropycal-1.0.1/docs/tropycal_full_logo.png
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.561911 tropycal-1.0.1/examples/
+-rw-r--r--   0 tomerburg   (501) staff       (20)       96 2023-07-02 20:17:03.000000 tropycal-1.0.1/examples/README.txt
+-rw-r--r--   0 tomerburg   (501) staff       (20)     5534 2023-07-02 20:17:03.000000 tropycal-1.0.1/examples/analogs.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)    10897 2023-07-02 20:17:03.000000 tropycal-1.0.1/examples/cartopy.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)     6171 2023-07-02 20:17:03.000000 tropycal-1.0.1/examples/customize_storm.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)     6297 2023-07-02 20:17:03.000000 tropycal-1.0.1/examples/realtime.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)     7105 2023-07-02 20:17:03.000000 tropycal-1.0.1/examples/recon.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)     4456 2023-07-02 20:17:03.000000 tropycal-1.0.1/examples/ships.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)     5164 2023-07-02 20:17:03.000000 tropycal-1.0.1/examples/tc_rainfall.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)     8733 2023-07-02 20:17:03.000000 tropycal-1.0.1/examples/tracks.TrackDataset.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)     2757 2023-07-02 20:17:03.000000 tropycal-1.0.1/examples/tracks.season.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)     7465 2023-07-02 20:17:03.000000 tropycal-1.0.1/examples/tracks.storm.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)     4451 2023-07-02 20:17:03.000000 tropycal-1.0.1/examples/tracks.tornado.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)      997 2023-07-11 20:23:31.579309 tropycal-1.0.1/setup.cfg
+-rw-r--r--   0 tomerburg   (501) staff       (20)      121 2023-07-02 20:17:03.000000 tropycal-1.0.1/setup.py
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.502295 tropycal-1.0.1/src/
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.562511 tropycal-1.0.1/src/tropycal/
+-rw-r--r--   0 tomerburg   (501) staff       (20)      159 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/__init__.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)      447 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/_version.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)     5103 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/constants.py
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.563526 tropycal-1.0.1/src/tropycal/plot/
+-rw-r--r--   0 tomerburg   (501) staff       (20)       23 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/plot/__init__.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)    14158 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/plot/plot.py
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.564048 tropycal-1.0.1/src/tropycal/rain/
+-rw-r--r--   0 tomerburg   (501) staff       (20)      184 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/rain/__init__.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)    11110 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/rain/dataset.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)    27902 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/rain/plot.py
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.565214 tropycal-1.0.1/src/tropycal/realtime/
+-rw-r--r--   0 tomerburg   (501) staff       (20)      132 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/realtime/__init__.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)    37999 2023-07-11 15:17:41.000000 tropycal-1.0.1/src/tropycal/realtime/realtime.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)    47725 2023-07-11 18:29:30.000000 tropycal-1.0.1/src/tropycal/realtime/storm.py
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.568758 tropycal-1.0.1/src/tropycal/recon/
+-rw-r--r--   0 tomerburg   (501) staff       (20)      240 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/recon/__init__.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)   122736 2023-07-02 22:24:35.000000 tropycal-1.0.1/src/tropycal/recon/dataset.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)    39124 2023-07-02 22:16:19.000000 tropycal-1.0.1/src/tropycal/recon/plot.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)    39275 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/recon/realtime.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)    63621 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/recon/tools.py
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.570000 tropycal-1.0.1/src/tropycal/ships/
+-rw-r--r--   0 tomerburg   (501) staff       (20)       85 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/ships/__init__.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)    16078 2023-07-11 19:09:00.000000 tropycal-1.0.1/src/tropycal/ships/ships.py
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.570762 tropycal-1.0.1/src/tropycal/tornado/
+-rw-r--r--   0 tomerburg   (501) staff       (20)      176 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/tornado/__init__.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)    15765 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/tornado/dataset.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)     8853 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/tornado/plot.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)     1941 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/tornado/tools.py
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.574048 tropycal-1.0.1/src/tropycal/tracks/
+-rw-r--r--   0 tomerburg   (501) staff       (20)      224 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/tracks/__init__.py
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.574495 tropycal-1.0.1/src/tropycal/tracks/data/
+-rw-r--r--   0 tomerburg   (501) staff       (20)     1249 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/tracks/data/catarina.csv
+-rw-r--r--   0 tomerburg   (501) staff       (20)     1924 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/tracks/data/pacific_2006.csv
+-rw-r--r--   0 tomerburg   (501) staff       (20)   213904 2023-07-06 23:31:07.000000 tropycal-1.0.1/src/tropycal/tracks/dataset.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)   130072 2023-07-10 15:18:51.000000 tropycal-1.0.1/src/tropycal/tracks/plot.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)    20570 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/tracks/season.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)   123426 2023-07-11 16:57:39.000000 tropycal-1.0.1/src/tropycal/tracks/storm.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)    31259 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/tracks/tools.py
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.575624 tropycal-1.0.1/src/tropycal/utils/
+-rw-r--r--   0 tomerburg   (501) staff       (20)      132 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/utils/__init__.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)    10482 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/utils/cartopy_utils.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)    11465 2023-07-02 20:17:03.000000 tropycal-1.0.1/src/tropycal/utils/colors.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)    72336 2023-07-11 18:33:59.000000 tropycal-1.0.1/src/tropycal/utils/generic_utils.py
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.563157 tropycal-1.0.1/src/tropycal.egg-info/
+-rw-r--r--   0 tomerburg   (501) staff       (20)     5064 2023-07-11 20:23:31.000000 tropycal-1.0.1/src/tropycal.egg-info/PKG-INFO
+-rw-r--r--   0 tomerburg   (501) staff       (20)     3897 2023-07-11 20:23:31.000000 tropycal-1.0.1/src/tropycal.egg-info/SOURCES.txt
+-rw-r--r--   0 tomerburg   (501) staff       (20)        1 2023-07-11 20:23:31.000000 tropycal-1.0.1/src/tropycal.egg-info/dependency_links.txt
+-rw-r--r--   0 tomerburg   (501) staff       (20)      119 2023-07-11 20:23:31.000000 tropycal-1.0.1/src/tropycal.egg-info/requires.txt
+-rw-r--r--   0 tomerburg   (501) staff       (20)        9 2023-07-11 20:23:31.000000 tropycal-1.0.1/src/tropycal.egg-info/top_level.txt
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.503196 tropycal-1.0.1/tests/
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.576777 tropycal-1.0.1/tests/data/
+-rw-r--r--   0 tomerburg   (501) staff       (20)   136603 2023-07-02 20:17:03.000000 tropycal-1.0.1/tests/data/sample_hurdat.txt
+-rw-r--r--   0 tomerburg   (501) staff       (20)      782 2023-07-02 20:17:03.000000 tropycal-1.0.1/tests/data/sample_storm.txt
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.577356 tropycal-1.0.1/tests/ships/
+-rw-r--r--   0 tomerburg   (501) staff       (20)     3566 2023-07-02 20:17:03.000000 tropycal-1.0.1/tests/ships/test_ships.py
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.578460 tropycal-1.0.1/tests/tracks/
+-rw-r--r--   0 tomerburg   (501) staff       (20)     4840 2023-07-02 20:17:03.000000 tropycal-1.0.1/tests/tracks/test_dataset.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)     1599 2023-07-02 20:17:03.000000 tropycal-1.0.1/tests/tracks/test_season.py
+-rw-r--r--   0 tomerburg   (501) staff       (20)     6755 2023-07-02 20:17:03.000000 tropycal-1.0.1/tests/tracks/test_storm.py
+drwxr-xr-x   0 tomerburg   (501) staff       (20)        0 2023-07-11 20:23:31.578681 tropycal-1.0.1/tests/utils/
+-rw-r--r--   0 tomerburg   (501) staff       (20)    19452 2023-07-02 20:17:03.000000 tropycal-1.0.1/tests/utils/test_utils.py
```

### Comparing `tropycal-1.0/.travis.yml` & `tropycal-1.0.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/LICENSE` & `tropycal-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/PKG-INFO` & `tropycal-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tropycal
-Version: 1.0
+Version: 1.0.1
 Summary: Package for retrieving and analyzing tropical cyclone data
 Home-page: https://github.com/tropycal/tropycal
 Author: Tomer Burg, Sam Lillo
 Project-URL: Documentation, https://tropycal.github.io/tropycal/
 Project-URL: Source Code, https://github.com/tropycal/tropycal
 Keywords: meteorology,weather
 Platform: any
@@ -18,15 +18,15 @@
 License-File: LICENSE
 
 # Tropycal
 Tropycal is a Python package intended to simplify the process of retrieving and analyzing tropical cyclone data, both for past storms and in real time, and is geared towards the research and operational meteorology sectors.
 
 Tropycal can read in HURDAT2 and IBTrACS reanalysis data and operational National Hurricane Center (NHC) Best Track data and conform them to the same format, which can be used to perform climatological, seasonal and individual storm analyses. For each individual storm, operational NHC and model forecasts, aircraft reconnaissance data, rainfall data, and any associated tornado activity can be retrieved and plotted.
 
-The latest version of Tropycal is v1.0.
+The latest version of Tropycal is v1.0.1.
 
 ## Installation
 
 
 ### Conda
 
 The currently recommended method of installation is via conda:
```

### Comparing `tropycal-1.0/README.md` & `tropycal-1.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Tropycal
 Tropycal is a Python package intended to simplify the process of retrieving and analyzing tropical cyclone data, both for past storms and in real time, and is geared towards the research and operational meteorology sectors.
 
 Tropycal can read in HURDAT2 and IBTrACS reanalysis data and operational National Hurricane Center (NHC) Best Track data and conform them to the same format, which can be used to perform climatological, seasonal and individual storm analyses. For each individual storm, operational NHC and model forecasts, aircraft reconnaissance data, rainfall data, and any associated tornado activity can be retrieved and plotted.
 
-The latest version of Tropycal is v1.0.
+The latest version of Tropycal is v1.0.1.
 
 ## Installation
 
 
 ### Conda
 
 The currently recommended method of installation is via conda:
```

### Comparing `tropycal-1.0/ci/deploy_key.enc` & `tropycal-1.0.1/ci/deploy_key.enc`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/Makefile` & `tropycal-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_static/css/badge_only.css` & `tropycal-1.0.1/docs/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_static/css/fonts/Roboto-Slab-Bold.woff` & `tropycal-1.0.1/docs/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_static/css/fonts/Roboto-Slab-Bold.woff2` & `tropycal-1.0.1/docs/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_static/css/fonts/Roboto-Slab-Regular.woff` & `tropycal-1.0.1/docs/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_static/css/fonts/Roboto-Slab-Regular.woff2` & `tropycal-1.0.1/docs/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_static/css/fonts/fontawesome-webfont.eot` & `tropycal-1.0.1/docs/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_static/css/fonts/fontawesome-webfont.svg` & `tropycal-1.0.1/docs/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_static/css/fonts/fontawesome-webfont.ttf` & `tropycal-1.0.1/docs/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_static/css/fonts/fontawesome-webfont.woff` & `tropycal-1.0.1/docs/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_static/css/fonts/fontawesome-webfont.woff2` & `tropycal-1.0.1/docs/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_static/css/fonts/lato-bold-italic.woff` & `tropycal-1.0.1/docs/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_static/css/fonts/lato-bold-italic.woff2` & `tropycal-1.0.1/docs/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_static/css/fonts/lato-bold.woff` & `tropycal-1.0.1/docs/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_static/css/fonts/lato-bold.woff2` & `tropycal-1.0.1/docs/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_static/css/fonts/lato-normal-italic.woff` & `tropycal-1.0.1/docs/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_static/css/fonts/lato-normal-italic.woff2` & `tropycal-1.0.1/docs/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_static/css/fonts/lato-normal.woff` & `tropycal-1.0.1/docs/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_static/css/fonts/lato-normal.woff2` & `tropycal-1.0.1/docs/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_static/css/theme.css` & `tropycal-1.0.1/docs/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_static/dorian.png` & `tropycal-1.0.1/docs/_static/dorian.png`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_static/grid_example_1.png` & `tropycal-1.0.1/docs/_static/grid_example_1.png`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_static/js/badge_only.js` & `tropycal-1.0.1/docs/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_static/js/theme.js` & `tropycal-1.0.1/docs/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_static/logo.png` & `tropycal-1.0.1/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_static/logo_32.ico` & `tropycal-1.0.1/docs/_static/logo_32.ico`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_static/michael_example_1.png` & `tropycal-1.0.1/docs/_static/michael_example_1.png`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_static/michael_example_2.png` & `tropycal-1.0.1/docs/_static/michael_example_2.png`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_static/michael_example_3.png` & `tropycal-1.0.1/docs/_static/michael_example_3.png`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_static/michael_example_4.png` & `tropycal-1.0.1/docs/_static/michael_example_4.png`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_static/storm_example_1.png` & `tropycal-1.0.1/docs/_static/storm_example_1.png`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_static/storm_example_2.png` & `tropycal-1.0.1/docs/_static/storm_example_2.png`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_static/storm_example_3.png` & `tropycal-1.0.1/docs/_static/storm_example_3.png`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_static/tornado_example_1.png` & `tropycal-1.0.1/docs/_static/tornado_example_1.png`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_static/tornado_example_2.png` & `tropycal-1.0.1/docs/_static/tornado_example_2.png`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_static/tornado_example_3.png` & `tropycal-1.0.1/docs/_static/tornado_example_3.png`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_static/tornado_example_5.png` & `tropycal-1.0.1/docs/_static/tornado_example_5.png`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_static/trackdataset_example_1.png` & `tropycal-1.0.1/docs/_static/trackdataset_example_1.png`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_static/trackdataset_example_2.png` & `tropycal-1.0.1/docs/_static/trackdataset_example_2.png`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_static/trackdataset_example_3.png` & `tropycal-1.0.1/docs/_static/trackdataset_example_3.png`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_static/trackdataset_example_4.png` & `tropycal-1.0.1/docs/_static/trackdataset_example_4.png`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_templates/autosummary/class.rst` & `tropycal-1.0.1/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_templates/autosummary/module.rst` & `tropycal-1.0.1/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/_templates/overrides/tropycal.utils.rst` & `tropycal-1.0.1/docs/_templates/overrides/tropycal.utils.rst`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/api/index.rst` & `tropycal-1.0.1/docs/api/index.rst`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/conf.py` & `tropycal-1.0.1/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 project = 'tropycal'
 copyright = '2023, Tropycal Developers'
 author = 'Tropycal Developers'
 
 # The short X.Y version
 version = ''
 # The full version, including alpha/beta/rc tags
-release = '1.0'
+release = '1.0.1'
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 needs_sphinx = '2.1'
```

### Comparing `tropycal-1.0/docs/data.rst` & `tropycal-1.0.1/docs/data.rst`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/index.rst` & `tropycal-1.0.1/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
    api/index
    sample_usage
    data
 
 Latest Version
 ==============
 
-The latest version of Tropycal as of 2 July 2023 is v1.0. This documentation is valid for the latest version of Tropycal.
+The latest version of Tropycal as of 11 July 2023 is v1.0.1. This documentation is valid for the latest version of Tropycal.
 
 Indices and tables
 ==================
 
 * :ref:`genindex`
 * :ref:`modindex`
 * :ref:`search`
```

### Comparing `tropycal-1.0/docs/install.rst` & `tropycal-1.0.1/docs/install.rst`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/make.bat` & `tropycal-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/options/domain.rst` & `tropycal-1.0.1/docs/options/domain.rst`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/options/map_prop.rst` & `tropycal-1.0.1/docs/options/map_prop.rst`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/sample_usage.rst` & `tropycal-1.0.1/docs/sample_usage.rst`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/samples/tracks.TrackDataset.rst` & `tropycal-1.0.1/docs/samples/tracks.TrackDataset.rst`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/samples/tracks.storm.rst` & `tropycal-1.0.1/docs/samples/tracks.storm.rst`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/samples/tracks.tornado.rst` & `tropycal-1.0.1/docs/samples/tracks.tornado.rst`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/docs/tropycal_full_logo.png` & `tropycal-1.0.1/docs/tropycal_full_logo.png`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/examples/analogs.py` & `tropycal-1.0.1/examples/analogs.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/examples/cartopy.py` & `tropycal-1.0.1/examples/cartopy.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/examples/customize_storm.py` & `tropycal-1.0.1/examples/customize_storm.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/examples/realtime.py` & `tropycal-1.0.1/examples/realtime.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/examples/recon.py` & `tropycal-1.0.1/examples/recon.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/examples/ships.py` & `tropycal-1.0.1/examples/ships.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/examples/tc_rainfall.py` & `tropycal-1.0.1/examples/tc_rainfall.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/examples/tracks.TrackDataset.py` & `tropycal-1.0.1/examples/tracks.TrackDataset.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/examples/tracks.season.py` & `tropycal-1.0.1/examples/tracks.season.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/examples/tracks.storm.py` & `tropycal-1.0.1/examples/tracks.storm.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/examples/tracks.tornado.py` & `tropycal-1.0.1/examples/tracks.tornado.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/setup.cfg` & `tropycal-1.0.1/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tropycal
-version = 1.0
+version = 1.0.1
 description = Package for retrieving and analyzing tropical cyclone data
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Tomer Burg, Sam Lillo
 platform = any
 keywords = meteorology, weather
 classifiers =
```

### Comparing `tropycal-1.0/src/tropycal/constants.py` & `tropycal-1.0.1/src/tropycal/constants.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/src/tropycal/plot/plot.py` & `tropycal-1.0.1/src/tropycal/plot/plot.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/src/tropycal/rain/dataset.py` & `tropycal-1.0.1/src/tropycal/rain/dataset.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/src/tropycal/rain/plot.py` & `tropycal-1.0.1/src/tropycal/rain/plot.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/src/tropycal/realtime/realtime.py` & `tropycal-1.0.1/src/tropycal/realtime/realtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -699,15 +699,15 @@
 
                 # Match to existing invests
                 distances = [great_circle((lat, lon), (self.data[storm_id]['lat'][-1],
                                           self.data[storm_id]['lon'][-1])).miles for storm_id in self.data.keys()]
                 min_distance = np.min(distances)
                 idx = distances.index(min_distance)
                 storm_id = [k for k in self.data.keys()][idx]
-                if min_distance <= 150:
+                if min_distance <= 400:
                     self.data[storm_id]['prob_2day'] = prob_2day
                     self.data[storm_id]['prob_7day'] = prob_7day
                     self.data[storm_id]['risk_2day'] = risk_2day
                     self.data[storm_id]['risk_7day'] = risk_7day
 
         except:
```

### Comparing `tropycal-1.0/src/tropycal/realtime/storm.py` & `tropycal-1.0.1/src/tropycal/realtime/storm.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,16 +105,16 @@
             end_time = 'N/A'
             max_wind = 'N/A'
             min_mslp = 'N/A'
         else:
             time_tropical = np.array(self.dict['time'])[idx]
             start_time = time_tropical[0].strftime("%H00 UTC %d %B %Y")
             end_time = time_tropical[-1].strftime("%H00 UTC %d %B %Y")
-            max_wind = 'N/A' if all_nan(np.array(self.dict['vmax'])[idx]) else np.nanmax(np.array(self.dict['vmax'])[idx])
-            min_mslp = 'N/A' if all_nan(np.array(self.dict['mslp'])[idx]) else np.nanmin(np.array(self.dict['mslp'])[idx])
+            max_wind = 'N/A' if all_nan(np.array(self.dict['vmax'])[idx]) else int(np.nanmax(np.array(self.dict['vmax'])[idx]))
+            min_mslp = 'N/A' if all_nan(np.array(self.dict['mslp'])[idx]) else int(np.nanmin(np.array(self.dict['mslp'])[idx]))
         summary_keys = {
             'Maximum Wind': f"{max_wind} knots",
             'Minimum Pressure': f"{min_mslp} hPa",
             'Start Time': start_time,
             'End Time': end_time,
         }
```

### Comparing `tropycal-1.0/src/tropycal/recon/dataset.py` & `tropycal-1.0.1/src/tropycal/recon/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1495,14 +1495,18 @@
         # --------------------------------------------------------------------------------------
 
         # Generate left and right title strings
         title_left, title_right = hovmoller_plot_title(
             self.storm, Hov_dict, varname)
         ax.set_title(title_left, loc='left', fontsize=16, fontweight='bold')
         ax.set_title(title_right, loc='right', fontsize=12)
+        
+        # Add plot credit
+        ax.text(0.02, 0.02, 'Plot generated by Tropycal',
+                ha='left', va='bottom', transform=ax.transAxes)
 
         # Return axis
         return ax
 
     def plot_maps(self, time=None, varname='wspd', recon_stats=None, domain="dynamic",
                   window=6, align='center', radlim=None, ax=None, cartopy_proj=None, save_dir=None, **kwargs):
         r"""
```

### Comparing `tropycal-1.0/src/tropycal/recon/plot.py` & `tropycal-1.0.1/src/tropycal/recon/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -920,15 +920,15 @@
         try:
             ax2.text(
                 0, .05, f'\nDeep Layer Mean Wind: {deg2dir(data["DLMdir"])} at {int(data["DLMspd"])} kt', va='top', fontsize=12)
         except:
             ax2.text(0, .05, f'\nDeep Layer Mean Wind: N/A',
                      va='top', fontsize=12)
 
-        ax2.set_title('Generated using Tropycal \n', fontsize=12,
+        ax2.set_title('Generated using Tropycal\nInspired by Tropical Tidbits', fontsize=12,
                       fontweight='bold', color='0.7', loc='right')
 
         cellText = np.array([[f'{int(i)} hPa' for i, j in zip(dfwind['pres'], dfwind['wspd']) if not np.isnan(j)],
                              [f'{deg2dir(j)} at {int(i)} kt' for i, j in zip(dfwind['wspd'], dfwind['wdir']) if not np.isnan(i)]]).T
         colLabels = ['Pressure', 'Wind']
         colors = [['w', cellcolor(cmap_wind(i / 200), i)]
                   for i in dfwind['wspd'] if not np.isnan(i)]
```

### Comparing `tropycal-1.0/src/tropycal/recon/realtime.py` & `tropycal-1.0.1/src/tropycal/recon/realtime.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/src/tropycal/recon/tools.py` & `tropycal-1.0.1/src/tropycal/recon/tools.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/src/tropycal/ships/ships.py` & `tropycal-1.0.1/src/tropycal/ships/ships.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,16 +14,19 @@
     r"""
     Initializes an instance of Ships.
     
     Parameters
     ----------
     content : str
         SHIPS file content. If initialized via a ``tropycal.tracks.Storm`` object, this does not need to be provided.
+    
+    Other Parameters
+    ----------------
     storm_name : str, optional
-        Storm name to associate with this SHIPS data. If initialized via a ``tropycal.tracks.Storm`` object, this does not need to be provided.
+        If provided, overrides storm name from SHIPS text data with the provided storm name.
     
     Returns
     -------
     tropycal.ships.Ships
         Instance of a Ships object.
     
     Notes
@@ -90,22 +93,17 @@
     def __init__(self, content, storm_name=None, forecast_init=None):
         
         ships = ships_parser(content)
         self.dict = ships['data']
         self.dict_ri = ships['data_ri']
         self.attrs = ships['data_attrs']
         
-        # Add storm name if provided
-        self.attrs['storm_name'] = 'UNKNOWN'
+        # Override storm name if requested
         if storm_name is not None: self.attrs['storm_name'] = storm_name
 
-        # Add forecast initialization if provided
-        self.attrs['forecast_init'] = np.nan
-        if forecast_init is not None: self.attrs['forecast_init'] = forecast_init
-
         # Set data variables as attributes of this object
         for key in self.dict:
             self[key] = np.array(self.dict[key])
     
     def get_variables(self):
         r"""
         Return list of available forecast variables.
@@ -238,16 +236,21 @@
             Matplotlib figure containing multiple axes.
         """
 
         # Create the figure and gridspec
         fig = plt.figure(figsize=(9,6),dpi=200)
         gs = gridspec.GridSpec(6, 32)
 
-        # Left column
-        proj = ccrs.PlateCarree()
+        # Left column & format Cartopy projection
+        plot_lon = np.copy(self.lon)
+        if np.nanmax(self.lon) > 150 or np.nanmin(self.lon) < -150:
+            proj = ccrs.PlateCarree(central_longitude = 180.0)
+            plot_lon[plot_lon < 0] += 360.0
+        else:
+            proj = ccrs.PlateCarree()
         ax1 = plt.subplot(gs[:3, :14])
         ax2 = plt.subplot(gs[3:, :14], projection=proj)
 
         # Right column
         ax3 = plt.subplot(gs[:1, 16:])
         ax4 = plt.subplot(gs[1:2, 16:])
         ax5 = plt.subplot(gs[2:3, 16:])
@@ -315,16 +318,16 @@
         table.set_fontsize(8)
         table.scale(1, 1.5)
         table.auto_set_column_width(range(len(data[0])))
 
         # ================================================================================================
 
         # Plot forecast
-        ax2.plot(self.lon, self.lat, color='k', linewidth=1.5, transform=ccrs.PlateCarree())
-        for i_lon, i_lat, i_vmax, i_type in zip(self.lon, self.lat, self.vmax_land_kt, self.storm_type):
+        ax2.plot(plot_lon, self.lat, color='k', linewidth=1.5, transform=ccrs.PlateCarree())
+        for i_lon, i_lat, i_vmax, i_type in zip(plot_lon, self.lat, self.vmax_land_kt, self.storm_type):
             if True in [np.isnan(i) for i in [i_lon, i_lat, i_vmax]]: continue
             marker_type = 'o' if i_type == 'TROP' else '^'
             marker_size = 9 if i_type == 'TROP' else 8
             ax2.plot(i_lon, i_lat, marker_type, mfc=get_colors_sshws(i_vmax),
                      mec='k', mew=0.5, ms=marker_size, transform=ccrs.PlateCarree())
             if i_type != 'TROP': continue
             category = str(wind_to_category(i_vmax))
@@ -336,26 +339,30 @@
 
         # Plot coastlines and political boundaries
         ax2.add_feature(cfeature.STATES.with_scale('50m'), linewidths=0.25, linestyle='solid', edgecolor='#444')
         ax2.add_feature(cfeature.BORDERS.with_scale('50m'), linewidths=0.5, linestyle='solid', edgecolor='#444')
         ax2.add_feature(cfeature.COASTLINE.with_scale('50m'), linewidths=0.5, linestyle='solid', edgecolor='#444')
         ax2.add_feature(cfeature.LAND.with_scale('50m'), facecolor='#EEEEEE', edgecolor='face')
 
-        plot_domain = dynamic_map_extent(np.nanmin(self.lon),
-                                         np.nanmax(self.lon),
+        plot_domain = dynamic_map_extent(np.nanmin(plot_lon),
+                                         np.nanmax(plot_lon),
                                          np.nanmin(self.lat),
                                          np.nanmax(self.lat))
         ax2.set_extent(plot_domain)
 
         # Add lat/lon labels
         gl = ax2.gridlines(draw_labels=True, linewidth=0.5, color='gray', alpha=0.5, linestyle='dashed')
         gl.top_labels = False
         gl.right_labels = False
         gl.xlabel_style = {'size': 8}
         gl.ylabel_style = {'size': 8}
+        
+        # Add plot credit
+        ax2.text(0.02, 0.98, "Plot generated by Tropycal\nInspired by Deelan Jariwala",
+                 fontsize=8, alpha=0.6, ha='left', va='top', transform=ax2.transAxes)
 
         # ================================================================================================
 
         # Set grid
         ax3.grid(linestyle='dotted')
         ax3.set_xticks(range(0,max(self.fhr)+1,24))
         ax3.set_xticklabels([])
@@ -424,11 +431,11 @@
         # Set grid
         ax8.grid(linestyle='dotted')
         ax8.set_xticks(range(0,max(self.fhr)+1,24))
         ax8.tick_params(axis='both', labelsize=8)
         ax8.set_xlim(0,max(self.fhr))
 
         # Plot heat potential
-        ax8.plot(self.fhr, self.heat_content, color='purple', label='Heat Content')
+        ax8.plot(self.fhr, self.heat_content, color='purple', label=r'Heat Content (KJ/cm$^2$)')
         ax8.legend(fontsize=7)
 
         return fig
```

### Comparing `tropycal-1.0/src/tropycal/tornado/dataset.py` & `tropycal-1.0.1/src/tropycal/tornado/dataset.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/src/tropycal/tornado/plot.py` & `tropycal-1.0.1/src/tropycal/tornado/plot.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/src/tropycal/tornado/tools.py` & `tropycal-1.0.1/src/tropycal/tornado/tools.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/src/tropycal/tracks/data/catarina.csv` & `tropycal-1.0.1/src/tropycal/tracks/data/catarina.csv`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/src/tropycal/tracks/data/pacific_2006.csv` & `tropycal-1.0.1/src/tropycal/tracks/data/pacific_2006.csv`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/src/tropycal/tracks/dataset.py` & `tropycal-1.0.1/src/tropycal/tracks/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -467,22 +467,19 @@
                 self.data[current_id]['type'].append(storm_type)
                 self.data[current_id]['lat'].append(lat)
                 self.data[current_id]['lon'].append(lon)
                 self.data[current_id]['vmax'].append(vmax)
                 self.data[current_id]['mslp'].append(mslp)
 
                 # Add basin
-                origin_basin = add_basin + ''
-                if add_basin == 'east_pacific':
-                    check_basin = get_basin(
-                        self.data[current_id]['lat'][0], self.data[current_id]['lon'][0], add_basin)
-                    if check_basin != add_basin:
-                        origin_basin = 'north_atlantic'
-                self.data[current_id]['wmo_basin'].append(
-                    get_basin(lat, lon, origin_basin))
+                previous_basin = add_basin + ''
+                if len(self.data[current_id]['wmo_basin']) > 0:
+                    previous_basin = self.data[current_id]['wmo_basin'][-1]
+                if previous_basin not in constants.NHC_BASINS: previous_basin = 'east_pacific'
+                self.data[current_id]['wmo_basin'].append(get_basin(lat, lon, previous_basin))
 
                 # Calculate ACE & append to storm total
                 if not np.isnan(vmax):
                     ace = accumulated_cyclone_energy(vmax)
                     if hhmm in constants.STANDARD_HOURS and storm_type in constants.NAMED_TROPICAL_STORM_TYPES:
                         self.data[current_id]['ace'] += np.round(ace, 4)
 
@@ -707,14 +704,18 @@
 
                 # Calculate ACE & append to storm total
                 if not np.isnan(btk_wind):
                     ace = accumulated_cyclone_energy(btk_wind)
                     if btk_type in constants.NAMED_TROPICAL_STORM_TYPES:
                         self.data[stormid]['ace'] += np.round(ace, 4)
 
+            # Fix name for unnamed storms
+            if name.upper() == 'INVEST' and True in np.isin(self.data[stormid]['type'], list(constants.TROPICAL_STORM_TYPES)):
+                name = 'UNNAMED'
+            
             # Add storm name
             self.data[stormid]['name'] = name
 
         # Determine time elapsed
         time_elapsed = dt.now() - start_time
         tsec = str(round(time_elapsed.total_seconds(), 2))
         print(f"--> Completed reading in best track data ({tsec} seconds)")
```

### Comparing `tropycal-1.0/src/tropycal/tracks/plot.py` & `tropycal-1.0.1/src/tropycal/tracks/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -2423,16 +2423,17 @@
                         plot_coords.append(
                             (bounds[0] + bounds[2]) * 0.5)  # lon
                         plot_coords.append(bounds[1])  # lat
                         plot_coords.append(record.attributes['GENPROB'])
                     else:
                         found_areas = []
                         for i_record, i_point in zip(shapefiles['points'].records(), shapefiles['points'].geometries()):
-                            found_areas.append(i_record.attributes['AREA'])
-                        if 'AREA' in record.attributes.keys() and record.attributes['AREA'] not in found_areas:
+                            found_areas.append([i_record.attributes['BASIN'],i_record.attributes['AREA']])
+                        check_area = [record.attributes['BASIN'],record.attributes['AREA']]
+                        if 'AREA' in record.attributes.keys() and check_area not in found_areas:
                             bounds = record.geometry.bounds
                             plot_coords.append(
                                 (bounds[0] + bounds[2]) * 0.5)  # lon
                             plot_coords.append(bounds[1])  # lat
                             if two_prop['days'] == 2:
                                 plot_coords.append(
                                     record.attributes['PROB2DAY'])
```

### Comparing `tropycal-1.0/src/tropycal/tracks/season.py` & `tropycal-1.0.1/src/tropycal/tracks/season.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/src/tropycal/tracks/storm.py` & `tropycal-1.0.1/src/tropycal/tracks/storm.py`

 * *Files 0% similar despite different names*

```diff
@@ -2897,15 +2897,15 @@
             content = read_url(url, split=False, subsplit=False)
             if len(content) < 10:
                 warnings.warn('Improper SHIPS entry for this time. Returning a value of None.')
                 return None
         except:
             raise ValueError('SHIPS data is unavailable for the requested storm or time.')
 
-        return Ships(content, storm_name=self.name, forecast_init=time)
+        return Ships(content)
 
     def get_archer(self):
         r"""
         Retrieves satellite-derived ARCHER track data for this storm, if available.
 
         Returns
         -------
```

### Comparing `tropycal-1.0/src/tropycal/tracks/tools.py` & `tropycal-1.0.1/src/tropycal/tracks/tools.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/src/tropycal/utils/cartopy_utils.py` & `tropycal-1.0.1/src/tropycal/utils/cartopy_utils.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/src/tropycal/utils/colors.py` & `tropycal-1.0.1/src/tropycal/utils/colors.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/src/tropycal/utils/generic_utils.py` & `tropycal-1.0.1/src/tropycal/utils/generic_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1352,14 +1352,28 @@
             line_subset_3 = float((line.split('mean (')[1]).split('%')[0])
         else:
             line_subset_3 = float((line.split('mean(')[1]).split('%')[0])
         return line_subset_1, line_subset_2, line_subset_3
 
     content = content.split('\n')
     for line in content:
+        
+        # Attempt to retrieve storm name and forecast init
+        if len(line.strip()) > 5 and line.strip()[0] == '*' and 'UTC' in line and 'storm_name' not in data_attrs:
+            line_array = line.split()
+            data_attrs['forecast_init'] = dt.strptime(f'{line_array[3]} {line_array[4]}','%m/%d/%y %H')
+            storm_name = line_array[1]
+            if storm_name.upper() in ['UNNAMED', 'INVEST', 'UNKNOWN']:
+                # Determine suffix
+                storm_id = line_array[2]
+                storm_suffix = storm_id[1]
+                if storm_id[0] in ['C', 'E', 'W', 'I', 'S']:
+                    storm_suffix = storm_id[0]
+                storm_name = f'{(line_array[2])[2:4]}{storm_suffix}'
+            data_attrs['storm_name'] = storm_name
 
         # Parse first group into dict
         first_group = {
             'TIME (HR)': ['fhr',int],
             'LAT (DEG N)': ['lat',float],
             'LONG(DEG W)': ['lon',float],
             'V (KT) NO LAND': ['vmax_noland_kt',int],
@@ -1531,16 +1545,15 @@
     # Define empty array
     return_arr = np.zeros((lats2d.shape))
 
     # Calculate distance from lat/lon at each gridpoint
     r_earth = 6.371 * 10**6
     dlat = np.subtract(np.radians(lats2d), np.radians(lat))
     dlon = np.subtract(np.radians(lons2d), np.radians(lon))
-    a = np.sin(dlat/2) * np.sin(dlat/2) + np.cos(np.radians(lats2d)) * \
-        np.cos(np.radians(lat)) * np.sin(dlon/2) * np.sin(dlon/2)
+    a = np.sin(dlat/2) * np.sin(dlat/2) + np.cos(np.radians(lats2d)) * np.cos(np.radians(lat)) * np.sin(dlon/2) * np.sin(dlon/2)
     c = 2 * np.arctan(np.sqrt(a), np.sqrt(1-a))
     dist = (r_earth * c)/1000.0
 
     return return_arr, dist
 
 
 def add_radius(lats2d, lons2d, lat, lon, rad):
@@ -1572,16 +1585,15 @@
     return_arr = np.zeros((lats2d.shape))
 
     # Calculate distance from lat/lon at each gridpoint
     r_earth = 6.371 * 10**6
     dlat = np.subtract(np.radians(lats2d), np.radians(lat))
     dlon = np.subtract(np.radians(lons2d), np.radians(lon))
 
-    a = np.sin(dlat*0.5) * np.sin(dlat*0.5) + np.cos(np.radians(lats2d)) * \
-        np.cos(np.radians(lat)) * np.sin(dlon*0.5) * np.sin(dlon*0.5)
+    a = np.sin(dlat*0.5) * np.sin(dlat*0.5) + np.cos(np.radians(lats2d)) * np.cos(np.radians(lat)) * np.sin(dlon*0.5) * np.sin(dlon*0.5)
     c = 2 * np.arctan(np.sqrt(a), np.sqrt(1-a))
     dist = (r_earth * c) * 0.001
 
     # Mask out values less than radius
     return_arr[dist > rad] = 0
     return_arr[dist <= rad] = 1
     return return_arr
@@ -1627,18 +1639,20 @@
             new_lats = np.arange(np.round(lat-5), 0+res, res)
     new_lons = np.arange(np.round(lon-10), np.round(lon+10+res), res)
     new_lons_2d, new_lats_2d = np.meshgrid(new_lons, new_lats)
     new_arr, new_dist = calc_distance(new_lats_2d, new_lons_2d, lat, lon)
 
     return_arr = plug_array(new_arr, return_arr, {
                             'lat': new_lats, 'lon': new_lons}, {'lat': lats, 'lon': lons})
+    return_dist = plug_array(new_dist, dist, {'lat': new_lats, 'lon': new_lons}, {
+                             'lat': lats, 'lon': lons})
 
     # Mask out values less than radius
-    return_arr[dist > rad] = 0
-    return_arr[dist <= rad] = 1
+    return_arr[return_dist > rad] = 0
+    return_arr[return_dist <= rad] = 1
     return return_arr
 
 
 def all_nan(arr):
     r"""
     Determine whether the entire array is filled with NaNs.
```

### Comparing `tropycal-1.0/src/tropycal.egg-info/PKG-INFO` & `tropycal-1.0.1/src/tropycal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tropycal
-Version: 1.0
+Version: 1.0.1
 Summary: Package for retrieving and analyzing tropical cyclone data
 Home-page: https://github.com/tropycal/tropycal
 Author: Tomer Burg, Sam Lillo
 Project-URL: Documentation, https://tropycal.github.io/tropycal/
 Project-URL: Source Code, https://github.com/tropycal/tropycal
 Keywords: meteorology,weather
 Platform: any
@@ -18,15 +18,15 @@
 License-File: LICENSE
 
 # Tropycal
 Tropycal is a Python package intended to simplify the process of retrieving and analyzing tropical cyclone data, both for past storms and in real time, and is geared towards the research and operational meteorology sectors.
 
 Tropycal can read in HURDAT2 and IBTrACS reanalysis data and operational National Hurricane Center (NHC) Best Track data and conform them to the same format, which can be used to perform climatological, seasonal and individual storm analyses. For each individual storm, operational NHC and model forecasts, aircraft reconnaissance data, rainfall data, and any associated tornado activity can be retrieved and plotted.
 
-The latest version of Tropycal is v1.0.
+The latest version of Tropycal is v1.0.1.
 
 ## Installation
 
 
 ### Conda
 
 The currently recommended method of installation is via conda:
```

### Comparing `tropycal-1.0/src/tropycal.egg-info/SOURCES.txt` & `tropycal-1.0.1/src/tropycal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/tests/data/sample_hurdat.txt` & `tropycal-1.0.1/tests/data/sample_hurdat.txt`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/tests/data/sample_storm.txt` & `tropycal-1.0.1/tests/data/sample_storm.txt`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/tests/ships/test_ships.py` & `tropycal-1.0.1/tests/ships/test_ships.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/tests/tracks/test_dataset.py` & `tropycal-1.0.1/tests/tracks/test_dataset.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/tests/tracks/test_season.py` & `tropycal-1.0.1/tests/tracks/test_season.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/tests/tracks/test_storm.py` & `tropycal-1.0.1/tests/tracks/test_storm.py`

 * *Files identical despite different names*

### Comparing `tropycal-1.0/tests/utils/test_utils.py` & `tropycal-1.0.1/tests/utils/test_utils.py`

 * *Files identical despite different names*

