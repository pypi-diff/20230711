# Comparing `tmp/calcbench_api_client-8.2.0.tar.gz` & `tmp/calcbench_api_client-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\calcbench_api_client-8.2.0.tar", last modified: Fri Apr 28 12:58:01 2023, max compression
+gzip compressed data, was "dist\calcbench_api_client-9.0.0.tar", last modified: Mon Jul 10 23:00:32 2023, max compression
```

## Comparing `calcbench_api_client-8.2.0.tar` & `calcbench_api_client-9.0.0.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 12:58:01.503794 calcbench_api_client-8.2.0/
--rw-rw-rw-   0        0        0      288 2021-05-18 15:59:00.000000 calcbench_api_client-8.2.0/.gitignore
-drwxrwxrwx   0        0        0        0 2023-04-28 12:58:00.493781 calcbench_api_client-8.2.0/.vscode/
--rw-rw-rw-   0        0        0      478 2021-05-18 15:57:34.000000 calcbench_api_client-8.2.0/.vscode/launch.json
--rw-rw-rw-   0        0        0     1989 2023-04-28 12:58:01.500783 calcbench_api_client-8.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      985 2022-08-18 20:47:28.000000 calcbench_api_client-8.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 12:58:00.528788 calcbench_api_client-8.2.0/calcbench/
-drwxrwxrwx   0        0        0        0 2023-04-28 12:58:00.542789 calcbench_api_client-8.2.0/calcbench/.vscode/
--rw-rw-rw-   0        0        0      477 2020-03-11 15:22:24.000000 calcbench_api_client-8.2.0/calcbench/.vscode/launch.json
--rw-rw-rw-   0        0        0     1810 2023-04-28 12:57:50.000000 calcbench_api_client-8.2.0/calcbench/__init__.py
--rw-rw-rw-   0        0        0    11918 2023-03-16 20:14:00.000000 calcbench_api_client-8.2.0/calcbench/api_client.py
--rw-rw-rw-   0        0        0     2279 2023-01-24 18:56:25.000000 calcbench_api_client-8.2.0/calcbench/api_query_params.py
--rw-rw-rw-   0        0        0    15620 2021-11-18 16:53:55.000000 calcbench_api_client-8.2.0/calcbench/business_combinations.py
--rw-rw-rw-   0        0        0     3920 2021-11-18 16:53:40.000000 calcbench_api_client-8.2.0/calcbench/companies.py
--rw-rw-rw-   0        0        0    17369 2022-02-15 16:51:25.000000 calcbench_api_client-8.2.0/calcbench/dimensional.py
--rw-rw-rw-   0        0        0    18077 2022-11-02 16:00:32.000000 calcbench_api_client-8.2.0/calcbench/disclosures.py
--rw-rw-rw-   0        0        0     5478 2023-03-22 16:00:49.000000 calcbench_api_client-8.2.0/calcbench/downloaders.py
--rw-rw-rw-   0        0        0     3700 2022-05-31 19:56:12.000000 calcbench_api_client-8.2.0/calcbench/face_statements.py
--rw-rw-rw-   0        0        0    11386 2023-01-19 15:50:21.000000 calcbench_api_client-8.2.0/calcbench/filing.py
--rw-rw-rw-   0        0        0     8910 2022-07-15 14:07:23.000000 calcbench_api_client-8.2.0/calcbench/listener.py
--rw-rw-rw-   0        0        0      650 2020-12-11 14:41:26.000000 calcbench_api_client-8.2.0/calcbench/metrics.py
--rw-rw-rw-   0        0        0     3269 2022-11-07 16:43:08.000000 calcbench_api_client-8.2.0/calcbench/press_release.py
--rw-rw-rw-   0        0        0     4456 2021-11-18 17:07:01.000000 calcbench_api_client-8.2.0/calcbench/raw_numeric_XBRL.py
--rw-rw-rw-   0        0        0     5968 2022-03-18 15:19:02.000000 calcbench_api_client-8.2.0/calcbench/raw_numeric_non_XBRL.py
--rw-rw-rw-   0        0        0    18769 2023-04-28 12:56:36.000000 calcbench_api_client-8.2.0/calcbench/standardized_numeric.py
-drwxrwxrwx   0        0        0        0 2023-04-28 12:58:00.579780 calcbench_api_client-8.2.0/calcbench_api_client.egg-info/
--rw-rw-rw-   0        0        0     1989 2023-04-28 12:58:00.000000 calcbench_api_client-8.2.0/calcbench_api_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2584 2023-04-28 12:58:00.000000 calcbench_api_client-8.2.0/calcbench_api_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 12:58:00.000000 calcbench_api_client-8.2.0/calcbench_api_client.egg-info/dependency_links.txt
-drwxrwxrwx   0        0        0        0 2023-04-28 12:58:00.600779 calcbench_api_client-8.2.0/calcbench_api_client.egg-info/dist/
--rw-rw-rw-   0        0        0    68879 2022-01-27 15:55:06.000000 calcbench_api_client-8.2.0/calcbench_api_client.egg-info/dist/calcbench_api_client-5.6.1-py3-none-any.whl
--rw-rw-rw-   0        0        0   418889 2022-01-27 15:55:05.000000 calcbench_api_client-8.2.0/calcbench_api_client.egg-info/dist/calcbench_api_client-5.6.1.tar.gz
--rw-rw-rw-   0        0        0      270 2023-04-28 12:58:00.000000 calcbench_api_client-8.2.0/calcbench_api_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-28 12:58:00.000000 calcbench_api_client-8.2.0/calcbench_api_client.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-28 12:58:00.611782 calcbench_api_client-8.2.0/conda-recipe/
--rw-rw-rw-   0        0        0      909 2022-06-30 14:34:48.000000 calcbench_api_client-8.2.0/conda-recipe/meta.yaml
-drwxrwxrwx   0        0        0        0 2023-04-28 12:58:00.632779 calcbench_api_client-8.2.0/docs/
--rw-rw-rw-   0        0        0        0 2020-03-11 15:22:24.000000 calcbench_api_client-8.2.0/docs/.nojekyll
--rw-rw-rw-   0        0        0      654 2020-03-11 15:22:24.000000 calcbench_api_client-8.2.0/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-04-28 12:58:00.878780 calcbench_api_client-8.2.0/docs/html/
-drwxrwxrwx   0        0        0        0 2023-04-28 12:58:00.889785 calcbench_api_client-8.2.0/docs/html/_sources/
--rw-rw-rw-   0        0        0     1299 2023-01-26 15:56:17.000000 calcbench_api_client-8.2.0/docs/html/_sources/getting-started.rst.txt
-drwxrwxrwx   0        0        0        0 2023-04-28 12:58:01.373804 calcbench_api_client-8.2.0/docs/html/_static/
--rw-rw-rw-   0        0        0    11885 2023-04-28 12:57:11.000000 calcbench_api_client-8.2.0/docs/html/_static/alabaster.css
--rw-rw-rw-   0        0        0    15541 2023-04-28 12:57:11.000000 calcbench_api_client-8.2.0/docs/html/_static/basic.css
--rw-rw-rw-   0        0        0       42 2020-03-19 21:59:59.000000 calcbench_api_client-8.2.0/docs/html/_static/custom.css
--rw-rw-rw-   0        0        0     9630 2021-07-29 16:06:08.000000 calcbench_api_client-8.2.0/docs/html/_static/doctools.js
--rw-rw-rw-   0        0        0      361 2023-04-28 12:57:11.000000 calcbench_api_client-8.2.0/docs/html/_static/documentation_options.js
--rw-rw-rw-   0        0        0      286 2020-03-11 15:22:24.000000 calcbench_api_client-8.2.0/docs/html/_static/file.png
--rw-rw-rw-   0        0        0   278292 2020-03-11 15:22:24.000000 calcbench_api_client-8.2.0/docs/html/_static/jquery-3.2.1.js
--rw-rw-rw-   0        0        0   280364 2020-03-19 22:00:02.000000 calcbench_api_client-8.2.0/docs/html/_static/jquery-3.4.1.js
--rw-rw-rw-   0        0        0   287630 2021-07-29 16:06:09.000000 calcbench_api_client-8.2.0/docs/html/_static/jquery-3.5.1.js
--rw-rw-rw-   0        0        0    89476 2021-07-29 16:06:09.000000 calcbench_api_client-8.2.0/docs/html/_static/jquery.js
--rw-rw-rw-   0        0        0    11151 2023-04-28 12:57:11.000000 calcbench_api_client-8.2.0/docs/html/_static/language_data.js
--rw-rw-rw-   0        0        0       90 2020-03-11 15:22:24.000000 calcbench_api_client-8.2.0/docs/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2020-03-11 15:22:24.000000 calcbench_api_client-8.2.0/docs/html/_static/plus.png
--rw-rw-rw-   0        0        0     4874 2023-04-28 12:57:11.000000 calcbench_api_client-8.2.0/docs/html/_static/pygments.css
--rw-rw-rw-   0        0        0    16578 2021-07-29 16:06:09.000000 calcbench_api_client-8.2.0/docs/html/_static/searchtools.js
--rw-rw-rw-   0        0        0    68420 2021-07-29 16:06:09.000000 calcbench_api_client-8.2.0/docs/html/_static/underscore-1.13.1.js
--rw-rw-rw-   0        0        0    35168 2020-03-19 22:00:02.000000 calcbench_api_client-8.2.0/docs/html/_static/underscore-1.3.1.js
--rw-rw-rw-   0        0        0    19530 2021-07-29 16:06:09.000000 calcbench_api_client-8.2.0/docs/html/_static/underscore.js
--rw-rw-rw-   0        0        0    20664 2023-04-28 12:57:11.000000 calcbench_api_client-8.2.0/docs/html/business-combinations.html
--rw-rw-rw-   0        0        0    12664 2022-01-27 15:45:17.000000 calcbench_api_client-8.2.0/docs/html/companies.html
--rw-rw-rw-   0        0        0   116341 2023-04-28 12:57:11.000000 calcbench_api_client-8.2.0/docs/html/dimensional.html
--rw-rw-rw-   0        0        0    65621 2023-04-12 21:26:04.000000 calcbench_api_client-8.2.0/docs/html/disclosures.html
--rw-rw-rw-   0        0        0    18893 2023-04-12 21:26:04.000000 calcbench_api_client-8.2.0/docs/html/downloaders.html
--rw-rw-rw-   0        0        0    35986 2023-01-26 15:02:06.000000 calcbench_api_client-8.2.0/docs/html/face-statements.html
--rw-rw-rw-   0        0        0    46164 2023-04-28 12:57:11.000000 calcbench_api_client-8.2.0/docs/html/filings.html
--rw-rw-rw-   0        0        0   107809 2023-04-28 12:57:11.000000 calcbench_api_client-8.2.0/docs/html/genindex.html
--rw-rw-rw-   0        0        0    14252 2023-04-12 21:26:05.000000 calcbench_api_client-8.2.0/docs/html/getting-started.html
--rw-rw-rw-   0        0        0     7429 2023-04-28 12:57:11.000000 calcbench_api_client-8.2.0/docs/html/index.html
--rw-rw-rw-   0        0        0     6017 2022-01-27 15:45:17.000000 calcbench_api_client-8.2.0/docs/html/metrics.html
--rw-rw-rw-   0        0        0    37691 2023-04-28 12:57:11.000000 calcbench_api_client-8.2.0/docs/html/numeric-data.html
--rw-rw-rw-   0        0        0    20870 2023-04-12 21:26:05.000000 calcbench_api_client-8.2.0/docs/html/press-release.html
--rw-rw-rw-   0        0        0    11099 2023-01-19 19:18:13.000000 calcbench_api_client-8.2.0/docs/html/push-notification.html
--rw-rw-rw-   0        0        0     7083 2023-04-28 12:57:11.000000 calcbench_api_client-8.2.0/docs/html/py-modindex.html
--rw-rw-rw-   0        0        0    18689 2022-01-27 15:45:18.000000 calcbench_api_client-8.2.0/docs/html/raw-numeric-XBRL.html
--rw-rw-rw-   0        0        0    36953 2023-01-26 15:02:06.000000 calcbench_api_client-8.2.0/docs/html/raw-numeric-non-XBRL.html
--rw-rw-rw-   0        0        0     4370 2023-04-28 12:57:11.000000 calcbench_api_client-8.2.0/docs/html/search.html
--rw-rw-rw-   0        0        0    47468 2023-04-28 12:57:11.000000 calcbench_api_client-8.2.0/docs/html/searchindex.js
--rw-rw-rw-   0        0        0       64 2020-03-11 15:22:24.000000 calcbench_api_client-8.2.0/docs/index.html
--rwxrwxrwx   0        0        0      796 2020-03-11 15:22:24.000000 calcbench_api_client-8.2.0/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-04-28 12:58:01.498784 calcbench_api_client-8.2.0/docs/source/
--rw-rw-rw-   0        0        0      274 2021-06-24 19:28:47.000000 calcbench_api_client-8.2.0/docs/source/business-combinations.rst
--rw-rw-rw-   0        0        0      132 2021-02-22 22:31:03.000000 calcbench_api_client-8.2.0/docs/source/companies.rst
--rw-rw-rw-   0        0        0     1907 2022-01-27 15:45:13.000000 calcbench_api_client-8.2.0/docs/source/conf.py
--rw-rw-rw-   0        0        0      275 2021-10-13 15:58:17.000000 calcbench_api_client-8.2.0/docs/source/dimensional.rst
--rw-rw-rw-   0        0        0      369 2021-07-23 16:57:12.000000 calcbench_api_client-8.2.0/docs/source/disclosures.rst
--rw-rw-rw-   0        0        0      113 2022-01-13 16:45:20.000000 calcbench_api_client-8.2.0/docs/source/downloaders.rst
--rw-rw-rw-   0        0        0      176 2022-05-31 19:08:45.000000 calcbench_api_client-8.2.0/docs/source/face-statements.rst
--rw-rw-rw-   0        0        0       90 2022-01-27 17:08:05.000000 calcbench_api_client-8.2.0/docs/source/filings.rst
--rw-rw-rw-   0        0        0     1299 2023-01-26 15:56:17.000000 calcbench_api_client-8.2.0/docs/source/getting-started.rst
--rw-rw-rw-   0        0        0      669 2022-01-13 16:44:16.000000 calcbench_api_client-8.2.0/docs/source/index.rst
--rw-rw-rw-   0        0        0       70 2020-11-12 16:28:47.000000 calcbench_api_client-8.2.0/docs/source/metrics.rst
--rw-rw-rw-   0        0        0      906 2022-11-07 16:43:08.000000 calcbench_api_client-8.2.0/docs/source/numeric-data.rst
--rw-rw-rw-   0        0        0      181 2021-11-18 18:30:32.000000 calcbench_api_client-8.2.0/docs/source/press-release.rst
--rw-rw-rw-   0        0        0     1002 2020-12-11 15:03:48.000000 calcbench_api_client-8.2.0/docs/source/push-notification.rst
--rw-rw-rw-   0        0        0      208 2021-05-04 16:55:43.000000 calcbench_api_client-8.2.0/docs/source/raw-numeric-XBRL.rst
--rw-rw-rw-   0        0        0      215 2021-04-05 15:28:06.000000 calcbench_api_client-8.2.0/docs/source/raw-numeric-non-XBRL.rst
--rw-rw-rw-   0        0        0       93 2020-10-22 17:34:48.000000 calcbench_api_client-8.2.0/publish.PS1
--rw-rw-rw-   0        0        0       42 2023-04-28 12:58:01.504781 calcbench_api_client-8.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1418 2023-01-26 15:29:46.000000 calcbench_api_client-8.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 23:00:32.193814 calcbench_api_client-9.0.0/
+-rw-rw-rw-   0        0        0      288 2021-05-18 15:59:00.000000 calcbench_api_client-9.0.0/.gitignore
+drwxrwxrwx   0        0        0        0 2023-07-10 23:00:31.259295 calcbench_api_client-9.0.0/.vscode/
+-rw-rw-rw-   0        0        0      478 2021-05-18 15:57:34.000000 calcbench_api_client-9.0.0/.vscode/launch.json
+-rw-rw-rw-   0        0        0     1988 2023-07-10 23:00:32.192812 calcbench_api_client-9.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      984 2023-06-06 17:23:29.000000 calcbench_api_client-9.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-10 23:00:31.293294 calcbench_api_client-9.0.0/calcbench/
+drwxrwxrwx   0        0        0        0 2023-07-10 23:00:31.306295 calcbench_api_client-9.0.0/calcbench/.vscode/
+-rw-rw-rw-   0        0        0      477 2020-03-11 15:22:24.000000 calcbench_api_client-9.0.0/calcbench/.vscode/launch.json
+-rw-rw-rw-   0        0        0     1812 2023-07-10 22:59:47.000000 calcbench_api_client-9.0.0/calcbench/__init__.py
+-rw-rw-rw-   0        0        0    11918 2023-03-16 20:14:00.000000 calcbench_api_client-9.0.0/calcbench/api_client.py
+-rw-rw-rw-   0        0        0     2279 2023-01-24 18:56:25.000000 calcbench_api_client-9.0.0/calcbench/api_query_params.py
+-rw-rw-rw-   0        0        0    15686 2023-05-08 15:32:07.000000 calcbench_api_client-9.0.0/calcbench/business_combinations.py
+-rw-rw-rw-   0        0        0     3920 2021-11-18 16:53:40.000000 calcbench_api_client-9.0.0/calcbench/companies.py
+-rw-rw-rw-   0        0        0    17369 2022-02-15 16:51:25.000000 calcbench_api_client-9.0.0/calcbench/dimensional.py
+-rw-rw-rw-   0        0        0    18077 2022-11-02 16:00:32.000000 calcbench_api_client-9.0.0/calcbench/disclosures.py
+-rw-rw-rw-   0        0        0     5726 2023-05-31 16:10:02.000000 calcbench_api_client-9.0.0/calcbench/downloaders.py
+-rw-rw-rw-   0        0        0     3700 2022-05-31 19:56:12.000000 calcbench_api_client-9.0.0/calcbench/face_statements.py
+-rw-rw-rw-   0        0        0    11386 2023-01-19 15:50:21.000000 calcbench_api_client-9.0.0/calcbench/filing.py
+-rw-rw-rw-   0        0        0     8910 2022-07-15 14:07:23.000000 calcbench_api_client-9.0.0/calcbench/listener.py
+-rw-rw-rw-   0        0        0      650 2020-12-11 14:41:26.000000 calcbench_api_client-9.0.0/calcbench/metrics.py
+-rw-rw-rw-   0        0        0     3269 2022-11-07 16:43:08.000000 calcbench_api_client-9.0.0/calcbench/press_release.py
+-rw-rw-rw-   0        0        0     4456 2021-11-18 17:07:01.000000 calcbench_api_client-9.0.0/calcbench/raw_numeric_XBRL.py
+-rw-rw-rw-   0        0        0     5968 2022-03-18 15:19:02.000000 calcbench_api_client-9.0.0/calcbench/raw_numeric_non_XBRL.py
+-rw-rw-rw-   0        0        0    19486 2023-07-10 22:57:42.000000 calcbench_api_client-9.0.0/calcbench/standardized_numeric.py
+drwxrwxrwx   0        0        0        0 2023-07-10 23:00:31.348317 calcbench_api_client-9.0.0/calcbench_api_client.egg-info/
+-rw-rw-rw-   0        0        0     1988 2023-07-10 23:00:30.000000 calcbench_api_client-9.0.0/calcbench_api_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2584 2023-07-10 23:00:31.000000 calcbench_api_client-9.0.0/calcbench_api_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 23:00:30.000000 calcbench_api_client-9.0.0/calcbench_api_client.egg-info/dependency_links.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 23:00:31.372297 calcbench_api_client-9.0.0/calcbench_api_client.egg-info/dist/
+-rw-rw-rw-   0        0        0    68879 2022-01-27 15:55:06.000000 calcbench_api_client-9.0.0/calcbench_api_client.egg-info/dist/calcbench_api_client-5.6.1-py3-none-any.whl
+-rw-rw-rw-   0        0        0   418889 2022-01-27 15:55:05.000000 calcbench_api_client-9.0.0/calcbench_api_client.egg-info/dist/calcbench_api_client-5.6.1.tar.gz
+-rw-rw-rw-   0        0        0      270 2023-07-10 23:00:30.000000 calcbench_api_client-9.0.0/calcbench_api_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-10 23:00:30.000000 calcbench_api_client-9.0.0/calcbench_api_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 23:00:31.382298 calcbench_api_client-9.0.0/conda-recipe/
+-rw-rw-rw-   0        0        0      909 2022-06-30 14:34:48.000000 calcbench_api_client-9.0.0/conda-recipe/meta.yaml
+drwxrwxrwx   0        0        0        0 2023-07-10 23:00:31.407296 calcbench_api_client-9.0.0/docs/
+-rw-rw-rw-   0        0        0        0 2020-03-11 15:22:24.000000 calcbench_api_client-9.0.0/docs/.nojekyll
+-rw-rw-rw-   0        0        0      654 2020-03-11 15:22:24.000000 calcbench_api_client-9.0.0/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-07-10 23:00:31.629295 calcbench_api_client-9.0.0/docs/html/
+drwxrwxrwx   0        0        0        0 2023-07-10 23:00:31.633296 calcbench_api_client-9.0.0/docs/html/_sources/
+-rw-rw-rw-   0        0        0     1299 2023-01-26 15:56:17.000000 calcbench_api_client-9.0.0/docs/html/_sources/getting-started.rst.txt
+drwxrwxrwx   0        0        0        0 2023-07-10 23:00:32.075812 calcbench_api_client-9.0.0/docs/html/_static/
+-rw-rw-rw-   0        0        0    11885 2023-07-10 22:59:54.000000 calcbench_api_client-9.0.0/docs/html/_static/alabaster.css
+-rw-rw-rw-   0        0        0    15541 2023-07-10 22:59:54.000000 calcbench_api_client-9.0.0/docs/html/_static/basic.css
+-rw-rw-rw-   0        0        0       42 2020-03-19 21:59:59.000000 calcbench_api_client-9.0.0/docs/html/_static/custom.css
+-rw-rw-rw-   0        0        0     9630 2021-07-29 16:06:08.000000 calcbench_api_client-9.0.0/docs/html/_static/doctools.js
+-rw-rw-rw-   0        0        0      361 2023-07-10 22:59:54.000000 calcbench_api_client-9.0.0/docs/html/_static/documentation_options.js
+-rw-rw-rw-   0        0        0      286 2020-03-11 15:22:24.000000 calcbench_api_client-9.0.0/docs/html/_static/file.png
+-rw-rw-rw-   0        0        0   278292 2020-03-11 15:22:24.000000 calcbench_api_client-9.0.0/docs/html/_static/jquery-3.2.1.js
+-rw-rw-rw-   0        0        0   280364 2020-03-19 22:00:02.000000 calcbench_api_client-9.0.0/docs/html/_static/jquery-3.4.1.js
+-rw-rw-rw-   0        0        0   287630 2021-07-29 16:06:09.000000 calcbench_api_client-9.0.0/docs/html/_static/jquery-3.5.1.js
+-rw-rw-rw-   0        0        0    89476 2021-07-29 16:06:09.000000 calcbench_api_client-9.0.0/docs/html/_static/jquery.js
+-rw-rw-rw-   0        0        0    11151 2023-07-10 22:59:54.000000 calcbench_api_client-9.0.0/docs/html/_static/language_data.js
+-rw-rw-rw-   0        0        0       90 2020-03-11 15:22:24.000000 calcbench_api_client-9.0.0/docs/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2020-03-11 15:22:24.000000 calcbench_api_client-9.0.0/docs/html/_static/plus.png
+-rw-rw-rw-   0        0        0     4874 2023-07-10 22:59:54.000000 calcbench_api_client-9.0.0/docs/html/_static/pygments.css
+-rw-rw-rw-   0        0        0    16578 2021-07-29 16:06:09.000000 calcbench_api_client-9.0.0/docs/html/_static/searchtools.js
+-rw-rw-rw-   0        0        0    68420 2021-07-29 16:06:09.000000 calcbench_api_client-9.0.0/docs/html/_static/underscore-1.13.1.js
+-rw-rw-rw-   0        0        0    35168 2020-03-19 22:00:02.000000 calcbench_api_client-9.0.0/docs/html/_static/underscore-1.3.1.js
+-rw-rw-rw-   0        0        0    19530 2021-07-29 16:06:09.000000 calcbench_api_client-9.0.0/docs/html/_static/underscore.js
+-rw-rw-rw-   0        0        0    20866 2023-07-10 22:58:11.000000 calcbench_api_client-9.0.0/docs/html/business-combinations.html
+-rw-rw-rw-   0        0        0    12664 2022-01-27 15:45:17.000000 calcbench_api_client-9.0.0/docs/html/companies.html
+-rw-rw-rw-   0        0        0   116341 2023-07-10 22:58:11.000000 calcbench_api_client-9.0.0/docs/html/dimensional.html
+-rw-rw-rw-   0        0        0    65621 2023-04-12 21:26:04.000000 calcbench_api_client-9.0.0/docs/html/disclosures.html
+-rw-rw-rw-   0        0        0    19795 2023-07-10 22:58:11.000000 calcbench_api_client-9.0.0/docs/html/downloaders.html
+-rw-rw-rw-   0        0        0    35986 2023-01-26 15:02:06.000000 calcbench_api_client-9.0.0/docs/html/face-statements.html
+-rw-rw-rw-   0        0        0    46164 2023-07-10 22:58:11.000000 calcbench_api_client-9.0.0/docs/html/filings.html
+-rw-rw-rw-   0        0        0   107809 2023-07-10 22:59:54.000000 calcbench_api_client-9.0.0/docs/html/genindex.html
+-rw-rw-rw-   0        0        0    14252 2023-07-10 22:59:54.000000 calcbench_api_client-9.0.0/docs/html/getting-started.html
+-rw-rw-rw-   0        0        0     7429 2023-07-10 22:59:54.000000 calcbench_api_client-9.0.0/docs/html/index.html
+-rw-rw-rw-   0        0        0     6017 2022-01-27 15:45:17.000000 calcbench_api_client-9.0.0/docs/html/metrics.html
+-rw-rw-rw-   0        0        0    37966 2023-07-10 22:58:11.000000 calcbench_api_client-9.0.0/docs/html/numeric-data.html
+-rw-rw-rw-   0        0        0    20870 2023-04-12 21:26:05.000000 calcbench_api_client-9.0.0/docs/html/press-release.html
+-rw-rw-rw-   0        0        0    11099 2023-01-19 19:18:13.000000 calcbench_api_client-9.0.0/docs/html/push-notification.html
+-rw-rw-rw-   0        0        0     7083 2023-07-10 22:59:54.000000 calcbench_api_client-9.0.0/docs/html/py-modindex.html
+-rw-rw-rw-   0        0        0    18689 2022-01-27 15:45:18.000000 calcbench_api_client-9.0.0/docs/html/raw-numeric-XBRL.html
+-rw-rw-rw-   0        0        0    36953 2023-01-26 15:02:06.000000 calcbench_api_client-9.0.0/docs/html/raw-numeric-non-XBRL.html
+-rw-rw-rw-   0        0        0     4370 2023-07-10 22:59:54.000000 calcbench_api_client-9.0.0/docs/html/search.html
+-rw-rw-rw-   0        0        0    47607 2023-07-10 22:59:54.000000 calcbench_api_client-9.0.0/docs/html/searchindex.js
+-rw-rw-rw-   0        0        0       64 2020-03-11 15:22:24.000000 calcbench_api_client-9.0.0/docs/index.html
+-rwxrwxrwx   0        0        0      796 2020-03-11 15:22:24.000000 calcbench_api_client-9.0.0/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-07-10 23:00:32.189818 calcbench_api_client-9.0.0/docs/source/
+-rw-rw-rw-   0        0        0      274 2021-06-24 19:28:47.000000 calcbench_api_client-9.0.0/docs/source/business-combinations.rst
+-rw-rw-rw-   0        0        0      132 2021-02-22 22:31:03.000000 calcbench_api_client-9.0.0/docs/source/companies.rst
+-rw-rw-rw-   0        0        0     1907 2022-01-27 15:45:13.000000 calcbench_api_client-9.0.0/docs/source/conf.py
+-rw-rw-rw-   0        0        0      275 2021-10-13 15:58:17.000000 calcbench_api_client-9.0.0/docs/source/dimensional.rst
+-rw-rw-rw-   0        0        0      369 2021-07-23 16:57:12.000000 calcbench_api_client-9.0.0/docs/source/disclosures.rst
+-rw-rw-rw-   0        0        0      113 2022-01-13 16:45:20.000000 calcbench_api_client-9.0.0/docs/source/downloaders.rst
+-rw-rw-rw-   0        0        0      176 2022-05-31 19:08:45.000000 calcbench_api_client-9.0.0/docs/source/face-statements.rst
+-rw-rw-rw-   0        0        0       90 2022-01-27 17:08:05.000000 calcbench_api_client-9.0.0/docs/source/filings.rst
+-rw-rw-rw-   0        0        0     1299 2023-01-26 15:56:17.000000 calcbench_api_client-9.0.0/docs/source/getting-started.rst
+-rw-rw-rw-   0        0        0      669 2022-01-13 16:44:16.000000 calcbench_api_client-9.0.0/docs/source/index.rst
+-rw-rw-rw-   0        0        0       70 2020-11-12 16:28:47.000000 calcbench_api_client-9.0.0/docs/source/metrics.rst
+-rw-rw-rw-   0        0        0      906 2022-11-07 16:43:08.000000 calcbench_api_client-9.0.0/docs/source/numeric-data.rst
+-rw-rw-rw-   0        0        0      181 2021-11-18 18:30:32.000000 calcbench_api_client-9.0.0/docs/source/press-release.rst
+-rw-rw-rw-   0        0        0     1002 2020-12-11 15:03:48.000000 calcbench_api_client-9.0.0/docs/source/push-notification.rst
+-rw-rw-rw-   0        0        0      208 2021-05-04 16:55:43.000000 calcbench_api_client-9.0.0/docs/source/raw-numeric-XBRL.rst
+-rw-rw-rw-   0        0        0      215 2021-04-05 15:28:06.000000 calcbench_api_client-9.0.0/docs/source/raw-numeric-non-XBRL.rst
+-rw-rw-rw-   0        0        0       93 2020-10-22 17:34:48.000000 calcbench_api_client-9.0.0/publish.PS1
+-rw-rw-rw-   0        0        0       42 2023-07-10 23:00:32.193814 calcbench_api_client-9.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1418 2023-01-26 15:29:46.000000 calcbench_api_client-9.0.0/setup.py
```

### Comparing `calcbench_api_client-8.2.0/PKG-INFO` & `calcbench_api_client-9.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calcbench_api_client
-Version: 8.2.0
+Version: 9.0.0
 Summary: Client for Calcbench data.
 Home-page: https://github.com/calcbench/python_api_client
 Author: Andrew Kittredge
 Author-email: andrew@calcbench.com
 License: Apache2
 Project-URL: Documentation, http://calcbench.github.io/python_api_client/html/index.html
 Project-URL: Examples, https://github.com/calcbench/notebooks
@@ -19,40 +19,40 @@
         
         :warning: **API access is not included in the standard Calcbench subscription. Talk to us@calcbench.com before you start coding.**
         
         ## Documentation
         
         http://calcbench.github.io/python_api_client/html/index.html
         
+        ## Examples
+        
+        https://github.com/calcbench/notebooks.
+        
         ## Installation
         
             pip install calcbench-api-client
         
             conda install -c calcbench calcbench-api-client
         
         ## Credentials
         
-        Use your Calcbench username (email) and password. Get a free two week Calcbench trial @ https://www.calcbench.com/join.
-        
-        ## Examples
-        
-        https://github.com/calcbench/notebooks.
+        Use your Calcbench username (email) and password. Get a free two week Calcbench trial @ https://www.calcbench.com/join
         
         ## Support
         
         andrew@calcbench.com
         
         ## Credit
         
         @someben https://github.com/calcbench/python_api_client/commit/6c2312525fa365acc91bd8e979037fc2492845f3
         
 Keywords: finance accounting SEC 10-(K|Q)
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: Backoff
-Provides-Extra: tqdm
 Provides-Extra: BeautifulSoup
+Provides-Extra: Listener
+Provides-Extra: tqdm
 Provides-Extra: Keyring
+Provides-Extra: Backoff
 Provides-Extra: pyarrow
 Provides-Extra: Pandas
-Provides-Extra: Listener
```

### Comparing `calcbench_api_client-8.2.0/README.md` & `calcbench_api_client-9.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 
 :warning: **API access is not included in the standard Calcbench subscription. Talk to us@calcbench.com before you start coding.**
 
 ## Documentation
 
 http://calcbench.github.io/python_api_client/html/index.html
 
+## Examples
+
+https://github.com/calcbench/notebooks.
+
 ## Installation
 
     pip install calcbench-api-client
 
     conda install -c calcbench calcbench-api-client
 
 ## Credentials
 
-Use your Calcbench username (email) and password. Get a free two week Calcbench trial @ https://www.calcbench.com/join.
-
-## Examples
-
-https://github.com/calcbench/notebooks.
+Use your Calcbench username (email) and password. Get a free two week Calcbench trial @ https://www.calcbench.com/join
 
 ## Support
 
 andrew@calcbench.com
 
 ## Credit
```

### Comparing `calcbench_api_client-8.2.0/calcbench/__init__.py` & `calcbench_api_client-9.0.0/calcbench/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The "public" properties on the cb module
 
 """
-__version__ = "8.2.0"
+__version__ = "9.0.0"
 from datetime import datetime
 import logging
 from .api_client import (
     enable_backoff,
     html_diff,
     set_credentials,
     set_proxies,
@@ -59,8 +59,8 @@
     ).timetuple()
     logging.basicConfig(
         format="%(asctime)s.%(msecs)03d %(levelname)-8s %(message)s", datefmt="%H:%M:%S"
     )
     cb_logger = logging.getLogger("calcbench")
     cb_logger.setLevel(level)
 
-    return cb_logger
+    return cb_logger
```

### Comparing `calcbench_api_client-8.2.0/calcbench/api_client.py` & `calcbench_api_client-9.0.0/calcbench/api_client.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/calcbench/api_query_params.py` & `calcbench_api_client-9.0.0/calcbench/api_query_params.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/calcbench/business_combinations.py` & `calcbench_api_client-9.0.0/calcbench/business_combinations.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "Can't find pandas, won't be able to use the functions that return DataFrames."
     pass
 
 import dataclasses
 import itertools
 from dataclasses import dataclass
 from datetime import datetime
-from typing import Dict, Generator
+from typing import Dict, Generator, Optional
 from calcbench.api_query_params import CompanyIdentifiers
 
 from calcbench.standardized_numeric import StandardizedPoint
 
 from .api_client import _json_POST, _try_parse_timestamp
 
 
@@ -128,15 +128,16 @@
 ]
 
 USEFUL_LIFE_LOW_COLUMN_LABEL = "useful_life_low"
 USEFUL_LIFE_HIGH_COLUMN_LABEL = "useful_life_high"
 
 
 def business_combinations_raw(
-    company_identifiers: CompanyIdentifiers = [], accession_id: int = None
+    company_identifiers: Optional[CompanyIdentifiers] = [],
+    accession_id: Optional[int] = None,
 ) -> Generator[BusinessCombination, None, None]:
     """Purchase price allocation for mergers and acquisitions.
 
     :param company_identifiers: Companies for which to retrieve data
     :param accession_id: Calcbench accession(filing) id  for which to retrieve data.  Get data for one filing.
 
     """
@@ -145,30 +146,31 @@
         "periodParameters": {"accessionID": accession_id},
     }
     for combination in _json_POST("businessCombinations", payload):
         yield BusinessCombination(**combination)
 
 
 def business_combinations(
-    company_identifiers: CompanyIdentifiers = [], accession_id: int = None
+    company_identifiers: Optional[CompanyIdentifiers] = [],
+    accession_id: Optional[int] = None,
 ) -> "pd.DataFrame":
     """Purchase price allocation for mergers and acquisitions.
 
     Columns are standardized metrics.
 
     :param company_identifiers: Companies for which to retrieve data
     :param accession_id: Calcbench accession(filing) id  for which to retrieve data.  Get data for one filing.
 
     """
     data = business_combinations_raw(
         company_identifiers=company_identifiers, accession_id=accession_id
     )
     rows = []
     for datum in data:
-        row = {key: datum[key] for key in COLUMNS}
+        row = {key: datum.get(key) for key in COLUMNS}
         for metric in STANDARDIZED_METRICS:
             standardized_point = datum.standardized_PPA_points.get(metric)
             if standardized_point:
                 row[metric] = standardized_point.get("value")
         for asset_category in FINITE_LIVED_INTANGIBLE_ASSETS:
             intangible_category = datum.intangible_categories.get(asset_category)
             if intangible_category:
```

### Comparing `calcbench_api_client-8.2.0/calcbench/companies.py` & `calcbench_api_client-9.0.0/calcbench/companies.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/calcbench/dimensional.py` & `calcbench_api_client-9.0.0/calcbench/dimensional.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/calcbench/disclosures.py` & `calcbench_api_client-9.0.0/calcbench/disclosures.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/calcbench/downloaders.py` & `calcbench_api_client-9.0.0/calcbench/downloaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,30 +138,34 @@
     >>> )
     >>> # Read the dataset
     >>> import pyarrow.parquet as pq
     >>> import pyarrow.compute as pc
     >>> table = pq.read_table(<root_path>)
     >>> expr = pc.field("ticker") == "MSFT"
     >>> msft_data = table.filter(expr).to_pandas()
+    >>>
+    >>> # Write the data
+    >>> pq.write_table(table, "C:/Users/andre/Downloads/standardized_data.parquet")
+    >>> from pyarrow import csv
+    >>> csv.write_csv(table, "C:/Users/andre/Downloads/entire_universe_standardized_PIT.csv")
 
     """
     import pyarrow as pa
     import pyarrow.parquet as pq
 
     for argument in tqdm(list(arguments)):
         try:
-
             df = f(argument)
             if df.empty:
                 continue
         except KeyboardInterrupt:
             raise
         except Exception as e:
             tqdm.write(f"Exception getting {argument} {e}")
         else:
             table = pa.Table.from_pandas(df)
             pq.write_to_dataset(
                 table=table,
                 root_path=root_path,
                 partition_cols=partition_cols,
                 **{"allow_truncated_timestamps": True, "coerce_timestamps": "us"},
-            )
+            )
```

### Comparing `calcbench_api_client-8.2.0/calcbench/face_statements.py` & `calcbench_api_client-9.0.0/calcbench/face_statements.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/calcbench/filing.py` & `calcbench_api_client-9.0.0/calcbench/filing.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/calcbench/listener.py` & `calcbench_api_client-9.0.0/calcbench/listener.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/calcbench/metrics.py` & `calcbench_api_client-9.0.0/calcbench/metrics.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/calcbench/press_release.py` & `calcbench_api_client-9.0.0/calcbench/press_release.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/calcbench/raw_numeric_XBRL.py` & `calcbench_api_client-9.0.0/calcbench/raw_numeric_XBRL.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/calcbench/raw_numeric_non_XBRL.py` & `calcbench_api_client-9.0.0/calcbench/raw_numeric_non_XBRL.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/calcbench/standardized_numeric.py` & `calcbench_api_client-9.0.0/calcbench/standardized_numeric.py`

 * *Files 10% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     all_footnotes: bool = False,
     filing_id: Optional[int] = None,
     all_non_GAAP: bool = False,
     all_metrics: bool = False,
     pit_V2: Optional[bool] = False,
     start_date: Optional[Union[datetime, date]] = None,
     end_date: Optional[Union[datetime, date]] = None,
-    exclude_unconfirmed_preliminary: Optional[bool] = False,
+    XBRL_only: Optional[bool] = False,
 ) -> Sequence[StandardizedPoint]:
     """Standardized data.
 
     Get normalized data from Calcbench.  Each point is normalized by economic concept and time period.
 
     :param company_identifiers: a sequence of tickers (or CIK codes), eg ['msft', 'goog', 'appl']
     :param metrics: a sequence of metrics, see the full list @ https://www.calcbench.com/home/standardizedmetrics eg. ['revenue', 'accountsreceivable']
@@ -106,16 +106,15 @@
     :param year: Get data for a single year, defaults to annual data.
     :param period_type: Either "annual" or "quarterly"
     :param filing_id: Filing id for which to get data.  corresponds to the filing_id in the objects returned by the filings API.
     :param all_non_GAAP: include all non-GAAP metrics from earnings press releases such as EBITDA_NonGAAP.  This is implied when querying by `filing_id`.
     :param all_metrics: All metrics.
     :param start_date: points modified from this date (inclusive).  If no time is specified all points from that date are returned.
     :param end_date: points modified until this date (exclusive).  If not time is specified point modified prior to this date are returned.
-    :param exclude_unconfirmed_preliminary: Exclude points from press-releases or 8-Ks that have not been "confirmed" in an XBRL filing.  Preliminary points have a higher error rate than XBRL points.
-
+    :param XBRL_only: Only get data that appeared in an XBRL document.  If supplied with start_date and end_date it will filter by the "confirming" filing_id.
     """
     if [
         bool(company_identifiers),
         bool(entire_universe),
         bool(filing_id),
     ].count(True) != 1:
         raise ValueError(
@@ -254,26 +253,39 @@
                 "includeTrace": include_trace,
                 "pointInTime": point_in_time,
                 "allFootnotes": all_footnotes,
                 "allface": all_face,
                 "allNonGAAP": all_non_GAAP,
                 "allMetrics": all_metrics,
                 "pointInTimeV2": pit_V2,
-                "excludeUnconfirmedPreliminary": exclude_unconfirmed_preliminary,
                 "includePreliminary": True,  # only applies to PIT V1
             },
             "periodParameters": period_parameters,
             "companiesParameters": companies_parameters,
         }
     )
 
     return _json_POST("mappedData", payload)
 
 
-ORDERED_COLUMNS = [
+ORDERED_REGULAR_COLUMNS = [
+    "ticker",
+    "metric",
+    "fiscal_year",
+    "fiscal_period",
+    "value",
+    "CIK",
+    "calendar_year",
+    "calendar_period",
+]
+"""
+Fields returned by non-point-in-time calls
+"""
+
+ORDERED_PIT_COLUMNS = [
     "ticker",
     "metric",
     "fiscal_year",
     "fiscal_period",
     "value",
     "revision_number",
     "preliminary",
@@ -286,42 +298,53 @@
     "period_end",
     "calendar_year",
     "calendar_period",
     "filing_accession_number",
     "trace_url",
     "date_modified",
     "date_XBRL_confirmed",
+    "confirming_XBRL_filing_ID",
     "original_value",
 ]
+"""
+Fields return by point-in-time calls
+"""
 
 
-def _build_data_frame(raw_data: Sequence[StandardizedPoint]) -> "pd.DataFrame":
+def _build_data_frame(
+    raw_data: Sequence[StandardizedPoint], point_in_time: bool
+) -> "pd.DataFrame":
     """
     The order of the columns should remain constant
     """
+
     if not raw_data:
         return pd.DataFrame()
+    columns = ORDERED_PIT_COLUMNS if point_in_time else ORDERED_REGULAR_COLUMNS
     data = pd.DataFrame(raw_data)
-    new_columns = list(set(data.columns) - set(ORDERED_COLUMNS))
-    data = data.reindex(columns=ORDERED_COLUMNS + new_columns)
-    data = data.drop(columns=["trace_facts"], errors="ignore")  # type: ignore
+    if point_in_time:
+        new_columns = list(set(data.columns) - set(columns))
+        data = data.reindex(columns=columns + new_columns)
+        data = data.drop(columns=["trace_facts"], errors="ignore")  # type: ignore
+    else:
+        data = data.reindex(columns=columns)
     return data
 
 
 def standardized(
     company_identifiers: CompanyIdentifiers = [],
     metrics: Sequence[str] = [],
     fiscal_year: Optional[int] = None,
     fiscal_period: PeriodArgument = None,
     start_date: Optional[Union[datetime, date]] = None,
     end_date: Optional[Union[datetime, date]] = None,
     point_in_time: bool = False,
     filing_id: Optional[int] = None,
-    exclude_unconfirmed_preliminary: Optional[bool] = False,
     pit_V2: Optional[bool] = None,
+    XBRL_only: Optional[bool] = False,
 ):
     """Standardized Numeric Data.
 
 
 
     The data behind the multi-company page, https://www.calcbench.com/multi.
 
@@ -331,16 +354,16 @@
     :param metrics: Standardized metrics.  Full list @ https://www.calcbench.com/home/standardizedmetrics eg. ['revenue', 'accountsreceivable'].  If not specified get all metrics.
     :param fiscal_year: Fiscal year for which to get data.  If not specified get all history.
     :param fiscal_period: Fiscal period for which to get data.  If not specified get all history.
     :param start_date:  Restrict to records modified on or after (inclusive) this date/datetime
     :param end_date:  Restric to records modified prior (exclusive) thie date/datetime
     :param point_in_time: Include timestamps when data was published and revision chains.
     :param filing_id: Filing ID for which to get data.  Get all of the data reported in this filing.
-    :param exclude_unconfirmed_preliminary: Exclude points from press-releases or 8-Ks that have not been "confirmed" in an XBRL filing.  Preliminary points have a higher error rate than XBRL points.
     :param pit_V2: Defaults to True, use point in time V2, this only makes sense when point_in_time = True.  This will go away at some point.
+    :param XBRL_only: Only get data that appeared in an XBRL document.  If supplied with start_date and end_date it will filter by the "confirming" filing_id.
     :return: Dataframe
 
 
 
     Standardized data with a timestamp when it was published by Calcbench.
 
 
@@ -355,15 +378,15 @@
         Columns:
 
     ticker
        Ticker of reporting company
     metric
        The metric name, see the definitions @ https://www.calcbench.com/home/standardizedmetrics
     fiscal_period
-       fiscal_year-fiscal_period the fiscal period the value applies to.
+       fiscal_year-fiscal_period the fiscal period the value applies to.  Like "2020-0" or "2021-3".  0 indicates annual, 1,2,3,4 are quarters.
     date_reported (PIT only)
        Timestamp (EST) when Calcbench finished processing the filing from which this value was parsed.
 
        In some cases, particularly prior to 2015, this will be the filing date of the document as recorded by the SEC.  To exclude these points remove points where the hour is 0.
 
     value
        The value of the fact
@@ -372,15 +395,15 @@
     preliminary
         True indicates the number was parsed from non-XBRL 8-K or press release from the wire
     XBRL
         Indicates the number was parsed from XBRL.
 
         The case where preliminary and XBRL are both true indicates the number was first parsed from a non-XBRL document then "confirmed" in an XBRL document.
     date_XBRL_confirmed
-        Time at which the point was confirmed by an point from an XBRL filing.
+        Time at which the point was confirmed by a point from an XBRL filing.
         If the point originally came from an XBRL filing this will be the original write time.
         If this is null, for points post April 2023, the point has not been confirmed.
     period_start
        First day of the fiscal period for this fact
     period_end
        Last day of the fiscal period for this fact
     calendar_year
@@ -403,14 +426,19 @@
         URL for a page showing the source document for this value.
     original_value (PIT only)
         The value that Calcbench extracted when it first processed the filing.
 
         Post November 2022, if this differs from the value Calcbench the fact was modified by Calcbench subsequent to the filing first being processed.
     standardized_id
         A unique identifier Calcbench assigns to each standardized value.
+
+    date_XBRL_confirmed
+        The date this value was "confirmed" by an XBRL document.  For values originally appearing in press-release, this will be the date of the associated 10-K/Q.
+    confirming_XBRL_filing_ID
+        The filing_id of the XBRL document which contained this value.
     date_downloaded
         The timestamp on your computer when you downloaded this data.
 
 
 
     Usage::
 
@@ -438,18 +466,18 @@
         filing_id=filing_id,
         all_metrics=not metrics,
         use_fiscal_period=True,
         include_trace=True,
         pit_V2=pit_V2,
         start_date=start_date,
         end_date=end_date,
-        exclude_unconfirmed_preliminary=exclude_unconfirmed_preliminary,
+        XBRL_only=XBRL_only,
     )
 
-    data = _build_data_frame(data)
+    data = _build_data_frame(data, point_in_time=point_in_time)
     if data.empty:
         return data
     data["fiscal_period"] = (
         data["fiscal_year"].astype(str) + "-" + data["fiscal_period"].astype(str)
     ).astype("string")
     data = data.drop("fiscal_year", axis=1)
 
@@ -483,10 +511,11 @@
         "ticker",
         "metric",
         "fiscal_period",
     ]
     if point_in_time:
         index_columns = index_columns + ["date_reported"]
         data["date_downloaded"] = datetime.now()
+        data["preliminary_only"] = data["preliminary"] & ~data["XBRL"]
     data = data.set_index(index_columns)
     data = data.sort_index()
     return data
```

### Comparing `calcbench_api_client-8.2.0/calcbench_api_client.egg-info/PKG-INFO` & `calcbench_api_client-9.0.0/calcbench_api_client.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calcbench-api-client
-Version: 8.2.0
+Version: 9.0.0
 Summary: Client for Calcbench data.
 Home-page: https://github.com/calcbench/python_api_client
 Author: Andrew Kittredge
 Author-email: andrew@calcbench.com
 License: Apache2
 Project-URL: Documentation, http://calcbench.github.io/python_api_client/html/index.html
 Project-URL: Examples, https://github.com/calcbench/notebooks
@@ -19,40 +19,40 @@
         
         :warning: **API access is not included in the standard Calcbench subscription. Talk to us@calcbench.com before you start coding.**
         
         ## Documentation
         
         http://calcbench.github.io/python_api_client/html/index.html
         
+        ## Examples
+        
+        https://github.com/calcbench/notebooks.
+        
         ## Installation
         
             pip install calcbench-api-client
         
             conda install -c calcbench calcbench-api-client
         
         ## Credentials
         
-        Use your Calcbench username (email) and password. Get a free two week Calcbench trial @ https://www.calcbench.com/join.
-        
-        ## Examples
-        
-        https://github.com/calcbench/notebooks.
+        Use your Calcbench username (email) and password. Get a free two week Calcbench trial @ https://www.calcbench.com/join
         
         ## Support
         
         andrew@calcbench.com
         
         ## Credit
         
         @someben https://github.com/calcbench/python_api_client/commit/6c2312525fa365acc91bd8e979037fc2492845f3
         
 Keywords: finance accounting SEC 10-(K|Q)
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: Backoff
-Provides-Extra: tqdm
 Provides-Extra: BeautifulSoup
+Provides-Extra: Listener
+Provides-Extra: tqdm
 Provides-Extra: Keyring
+Provides-Extra: Backoff
 Provides-Extra: pyarrow
 Provides-Extra: Pandas
-Provides-Extra: Listener
```

### Comparing `calcbench_api_client-8.2.0/calcbench_api_client.egg-info/SOURCES.txt` & `calcbench_api_client-9.0.0/calcbench_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/calcbench_api_client.egg-info/dist/calcbench_api_client-5.6.1-py3-none-any.whl` & `calcbench_api_client-9.0.0/calcbench_api_client.egg-info/dist/calcbench_api_client-5.6.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/calcbench_api_client.egg-info/dist/calcbench_api_client-5.6.1.tar.gz` & `calcbench_api_client-9.0.0/calcbench_api_client.egg-info/dist/calcbench_api_client-5.6.1.tar.gz`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/conda-recipe/meta.yaml` & `calcbench_api_client-9.0.0/conda-recipe/meta.yaml`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/docs/Makefile` & `calcbench_api_client-9.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/docs/html/_sources/getting-started.rst.txt` & `calcbench_api_client-9.0.0/docs/html/_sources/getting-started.rst.txt`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/docs/html/_static/alabaster.css` & `calcbench_api_client-9.0.0/docs/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/docs/html/_static/basic.css` & `calcbench_api_client-9.0.0/docs/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/docs/html/_static/doctools.js` & `calcbench_api_client-9.0.0/docs/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/docs/html/_static/jquery-3.2.1.js` & `calcbench_api_client-9.0.0/docs/html/_static/jquery-3.2.1.js`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/docs/html/_static/jquery-3.4.1.js` & `calcbench_api_client-9.0.0/docs/html/_static/jquery-3.4.1.js`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/docs/html/_static/jquery-3.5.1.js` & `calcbench_api_client-9.0.0/docs/html/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/docs/html/_static/jquery.js` & `calcbench_api_client-9.0.0/docs/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/docs/html/_static/language_data.js` & `calcbench_api_client-9.0.0/docs/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/docs/html/_static/pygments.css` & `calcbench_api_client-9.0.0/docs/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/docs/html/_static/searchtools.js` & `calcbench_api_client-9.0.0/docs/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/docs/html/_static/underscore-1.13.1.js` & `calcbench_api_client-9.0.0/docs/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/docs/html/_static/underscore-1.3.1.js` & `calcbench_api_client-9.0.0/docs/html/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/docs/html/_static/underscore.js` & `calcbench_api_client-9.0.0/docs/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/docs/html/business-combinations.html` & `calcbench_api_client-9.0.0/docs/html/business-combinations.html`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 <dt class="sig sig-object py" id="calcbench.business_combinations.business_combinations">
 <span class="sig-prename descclassname"><span class="pre">calcbench.business_combinations.</span></span><span class="sig-name descname"><span class="pre">business_combinations</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">company_identifiers</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">accession_id</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#calcbench.business_combinations.business_combinations" title="Permalink to this definition">¶</a></dt>
 <dd><p>Purchase price allocation for mergers and acquisitions.</p>
 <p>Columns are standardized metrics.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters</dt>
 <dd class="field-odd"><ul class="simple">
-<li><p><strong>company_identifiers</strong> (<code class="xref py py-class docutils literal notranslate"><span class="pre">Sequence</span></code>[<code class="xref py py-data docutils literal notranslate"><span class="pre">Union</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">str</span></code>, <code class="xref py py-class docutils literal notranslate"><span class="pre">int</span></code>]]) – Companies for which to retrieve data</p></li>
+<li><p><strong>company_identifiers</strong> (<code class="xref py py-data docutils literal notranslate"><span class="pre">Optional</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">Sequence</span></code>[<code class="xref py py-data docutils literal notranslate"><span class="pre">Union</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">str</span></code>, <code class="xref py py-class docutils literal notranslate"><span class="pre">int</span></code>]]]) – Companies for which to retrieve data</p></li>
 <li><p><strong>accession_id</strong> (<code class="xref py py-data docutils literal notranslate"><span class="pre">Optional</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">int</span></code>]) – Calcbench accession(filing) id  for which to retrieve data.  Get data for one filing.</p></li>
 </ul>
 </dd>
 <dt class="field-even">Return type</dt>
 <dd class="field-even"><p><code class="xref py py-class docutils literal notranslate"><span class="pre">DataFrame</span></code></p>
 </dd>
 </dl>
@@ -151,15 +151,15 @@
 <dl class="py function">
 <dt class="sig sig-object py" id="calcbench.business_combinations.business_combinations_raw">
 <span class="sig-prename descclassname"><span class="pre">calcbench.business_combinations.</span></span><span class="sig-name descname"><span class="pre">business_combinations_raw</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">company_identifiers</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">accession_id</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#calcbench.business_combinations.business_combinations_raw" title="Permalink to this definition">¶</a></dt>
 <dd><p>Purchase price allocation for mergers and acquisitions.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters</dt>
 <dd class="field-odd"><ul class="simple">
-<li><p><strong>company_identifiers</strong> (<code class="xref py py-class docutils literal notranslate"><span class="pre">Sequence</span></code>[<code class="xref py py-data docutils literal notranslate"><span class="pre">Union</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">str</span></code>, <code class="xref py py-class docutils literal notranslate"><span class="pre">int</span></code>]]) – Companies for which to retrieve data</p></li>
+<li><p><strong>company_identifiers</strong> (<code class="xref py py-data docutils literal notranslate"><span class="pre">Optional</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">Sequence</span></code>[<code class="xref py py-data docutils literal notranslate"><span class="pre">Union</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">str</span></code>, <code class="xref py py-class docutils literal notranslate"><span class="pre">int</span></code>]]]) – Companies for which to retrieve data</p></li>
 <li><p><strong>accession_id</strong> (<code class="xref py py-data docutils literal notranslate"><span class="pre">Optional</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">int</span></code>]) – Calcbench accession(filing) id  for which to retrieve data.  Get data for one filing.</p></li>
 </ul>
 </dd>
 <dt class="field-even">Return type</dt>
 <dd class="field-even"><p><code class="xref py py-class docutils literal notranslate"><span class="pre">Generator</span></code>[<a class="reference internal" href="#calcbench.business_combinations.BusinessCombination" title="calcbench.business_combinations.BusinessCombination"><code class="xref py py-class docutils literal notranslate"><span class="pre">BusinessCombination</span></code></a>, <code class="xref py py-obj docutils literal notranslate"><span class="pre">None</span></code>, <code class="xref py py-obj docutils literal notranslate"><span class="pre">None</span></code>]</p>
 </dd>
 </dl>
```

#### html2text {}

```diff
@@ -32,26 +32,26 @@
         useful_life_upper_range: floatÂ¶
         value: floatÂ¶
   calcbench.business_combinations.business_combinations(company_identifiers=[],
   accession_id=None)Â¶
       Purchase price allocation for mergers and acquisitions.
       Columns are standardized metrics.
         Parameters
-                * company_identifiers (Sequence[Union[str, int]]) â Companies
-                  for which to retrieve data
+                * company_identifiers (Optional[Sequence[Union[str, int]]]) â
+                  Companies for which to retrieve data
                 * accession_id (Optional[int]) â Calcbench accession(filing)
                   id for which to retrieve data. Get data for one filing.
         Return type
             DataFrame
   calcbench.business_combinations.business_combinations_raw
   (company_identifiers=[], accession_id=None)Â¶
       Purchase price allocation for mergers and acquisitions.
         Parameters
-                * company_identifiers (Sequence[Union[str, int]]) â Companies
-                  for which to retrieve data
+                * company_identifiers (Optional[Sequence[Union[str, int]]]) â
+                  Companies for which to retrieve data
                 * accession_id (Optional[int]) â Calcbench accession(filing)
                   id for which to retrieve data. Get data for one filing.
         Return type
             Generator[BusinessCombination, None, None]
   calcbench.business_combinations.legacy_report(company_identifiers=[],
   accession_id=None)Â¶
       This is used by a Calcbench client that shall not be named.
```

### Comparing `calcbench_api_client-8.2.0/docs/html/companies.html` & `calcbench_api_client-9.0.0/docs/html/companies.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/docs/html/dimensional.html` & `calcbench_api_client-9.0.0/docs/html/dimensional.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/docs/html/disclosures.html` & `calcbench_api_client-9.0.0/docs/html/disclosures.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/docs/html/downloaders.html` & `calcbench_api_client-9.0.0/docs/html/downloaders.html`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,19 @@
 <span class="gp">&gt;&gt;&gt; </span><span class="p">)</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="c1"># Read the dataset</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="kn">import</span> <span class="nn">pyarrow.parquet</span> <span class="k">as</span> <span class="nn">pq</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="kn">import</span> <span class="nn">pyarrow.compute</span> <span class="k">as</span> <span class="nn">pc</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="n">table</span> <span class="o">=</span> <span class="n">pq</span><span class="o">.</span><span class="n">read_table</span><span class="p">(</span><span class="o">&lt;</span><span class="n">root_path</span><span class="o">&gt;</span><span class="p">)</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="n">expr</span> <span class="o">=</span> <span class="n">pc</span><span class="o">.</span><span class="n">field</span><span class="p">(</span><span class="s2">&quot;ticker&quot;</span><span class="p">)</span> <span class="o">==</span> <span class="s2">&quot;MSFT&quot;</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="n">msft_data</span> <span class="o">=</span> <span class="n">table</span><span class="o">.</span><span class="n">filter</span><span class="p">(</span><span class="n">expr</span><span class="p">)</span><span class="o">.</span><span class="n">to_pandas</span><span class="p">()</span>
+<span class="go">&gt;&gt;&gt;</span>
+<span class="gp">&gt;&gt;&gt; </span><span class="c1"># Write the data</span>
+<span class="gp">&gt;&gt;&gt; </span><span class="n">pq</span><span class="o">.</span><span class="n">write_table</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="s2">&quot;C:/Users/andre/Downloads/standardized_data.parquet&quot;</span><span class="p">)</span>
+<span class="gp">&gt;&gt;&gt; </span><span class="kn">from</span> <span class="nn">pyarrow</span> <span class="kn">import</span> <span class="n">csv</span>
+<span class="gp">&gt;&gt;&gt; </span><span class="n">csv</span><span class="o">.</span><span class="n">write_csv</span><span class="p">(</span><span class="n">table</span><span class="p">,</span> <span class="s2">&quot;C:/Users/andre/Downloads/entire_universe_standardized_PIT.csv&quot;</span><span class="p">)</span>
 </pre></div>
 </div>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="calcbench.downloaders.iterate_to_dataframe">
 <span class="sig-prename descclassname"><span class="pre">calcbench.downloaders.</span></span><span class="sig-name descname"><span class="pre">iterate_to_dataframe</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">arguments</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">f</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#calcbench.downloaders.iterate_to_dataframe" title="Permalink to this definition">¶</a></dt>
```

#### html2text {}

```diff
@@ -51,14 +51,21 @@
       >>> )
       >>> # Read the dataset
       >>> import pyarrow.parquet as pq
       >>> import pyarrow.compute as pc
       >>> table = pq.read_table(<root_path>)
       >>> expr = pc.field("ticker") == "MSFT"
       >>> msft_data = table.filter(expr).to_pandas()
+      >>>
+      >>> # Write the data
+      >>> pq.write_table(table, "C:/Users/andre/Downloads/
+      standardized_data.parquet")
+      >>> from pyarrow import csv
+      >>> csv.write_csv(table, "C:/Users/andre/Downloads/
+      entire_universe_standardized_PIT.csv")
   calcbench.downloaders.iterate_to_dataframe(arguments, f)Â¶
       Apply arguments to a function that returns a DataFrame append to a
       dataframe and return.
       Usage:
       >>> %pip install calcbench-api-client[Pandas,Backoff,tqdm]
       >>> from calcbench.downloaders import iterate_to_dataframe
       >>> import calcbench as cb
```

### Comparing `calcbench_api_client-8.2.0/docs/html/face-statements.html` & `calcbench_api_client-9.0.0/docs/html/face-statements.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/docs/html/filings.html` & `calcbench_api_client-9.0.0/docs/html/filings.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/docs/html/genindex.html` & `calcbench_api_client-9.0.0/docs/html/genindex.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/docs/html/getting-started.html` & `calcbench_api_client-9.0.0/docs/html/getting-started.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/docs/html/index.html` & `calcbench_api_client-9.0.0/docs/html/index.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/docs/html/metrics.html` & `calcbench_api_client-9.0.0/docs/html/metrics.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/docs/html/numeric-data.html` & `calcbench_api_client-9.0.0/docs/html/numeric-data.html`

 * *Files 7% similar despite different names*

```diff
@@ -36,31 +36,31 @@
 <h1>Standardized Numeric Financials<a class="headerlink" href="#standardized-numeric-financials" title="Permalink to this headline">¶</a></h1>
 <p>Calcbench extracts all of the GAAP numbers in section 8, face statments and footnotes, of the 10-K/Qs.  Face financials from earnings press-releases and 8-Ks are also included.</p>
 <div class="section" id="standardized">
 <h2>Standardized<a class="headerlink" href="#standardized" title="Permalink to this headline">¶</a></h2>
 <p>Calcbench standardizes +1000 metrics to handle differences in filers’s tagging.  The list of stardized points is &#64; <a class="reference external" href="https://www.calcbench.com/home/standardizedmetrics">https://www.calcbench.com/home/standardizedmetrics</a></p>
 <dl class="py function">
 <dt class="sig sig-object py" id="calcbench.standardized">
-<span class="sig-prename descclassname"><span class="pre">calcbench.</span></span><span class="sig-name descname"><span class="pre">standardized</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">company_identifiers</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">metrics</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">fiscal_year</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">fiscal_period</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">start_date</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">end_date</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">point_in_time</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">filing_id</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exclude_unconfirmed_preliminary</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">pit_V2</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#calcbench.standardized" title="Permalink to this definition">¶</a></dt>
+<span class="sig-prename descclassname"><span class="pre">calcbench.</span></span><span class="sig-name descname"><span class="pre">standardized</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">company_identifiers</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">metrics</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">fiscal_year</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">fiscal_period</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">start_date</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">end_date</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">point_in_time</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">filing_id</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">pit_V2</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">XBRL_only</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#calcbench.standardized" title="Permalink to this definition">¶</a></dt>
 <dd><p>Standardized Numeric Data.</p>
 <p>The data behind the multi-company page, <a class="reference external" href="https://www.calcbench.com/multi">https://www.calcbench.com/multi</a>.</p>
 <p>Example <a class="reference external" href="https://github.com/calcbench/notebooks/blob/master/python_client_api_demo.ipynb">https://github.com/calcbench/notebooks/blob/master/python_client_api_demo.ipynb</a></p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters</dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>company_identifiers</strong> (<code class="xref py py-class docutils literal notranslate"><span class="pre">Sequence</span></code>[<code class="xref py py-data docutils literal notranslate"><span class="pre">Union</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">str</span></code>, <code class="xref py py-class docutils literal notranslate"><span class="pre">int</span></code>]]) – Tickers/CIK codes. eg. [‘msft’, ‘goog’, ‘appl’, ‘0000066740’].  If not specified get data for all companies.</p></li>
 <li><p><strong>metrics</strong> (<code class="xref py py-class docutils literal notranslate"><span class="pre">Sequence</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">str</span></code>]) – Standardized metrics.  Full list &#64; <a class="reference external" href="https://www.calcbench.com/home/standardizedmetrics">https://www.calcbench.com/home/standardizedmetrics</a> eg. [‘revenue’, ‘accountsreceivable’].  If not specified get all metrics.</p></li>
 <li><p><strong>fiscal_year</strong> (<code class="xref py py-data docutils literal notranslate"><span class="pre">Optional</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">int</span></code>]) – Fiscal year for which to get data.  If not specified get all history.</p></li>
 <li><p><strong>fiscal_period</strong> (<code class="xref py py-data docutils literal notranslate"><span class="pre">Union</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">Period</span></code>, <code class="xref py py-data docutils literal notranslate"><span class="pre">Literal</span></code>[0, 1, 2, 3, 4], <code class="xref py py-obj docutils literal notranslate"><span class="pre">None</span></code>]) – Fiscal period for which to get data.  If not specified get all history.</p></li>
 <li><p><strong>start_date</strong> (<code class="xref py py-data docutils literal notranslate"><span class="pre">Union</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">datetime</span></code>, <code class="xref py py-class docutils literal notranslate"><span class="pre">date</span></code>, <code class="xref py py-obj docutils literal notranslate"><span class="pre">None</span></code>]) – Restrict to records modified on or after (inclusive) this date/datetime</p></li>
 <li><p><strong>end_date</strong> (<code class="xref py py-data docutils literal notranslate"><span class="pre">Union</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">datetime</span></code>, <code class="xref py py-class docutils literal notranslate"><span class="pre">date</span></code>, <code class="xref py py-obj docutils literal notranslate"><span class="pre">None</span></code>]) – Restric to records modified prior (exclusive) thie date/datetime</p></li>
 <li><p><strong>point_in_time</strong> (<code class="xref py py-class docutils literal notranslate"><span class="pre">bool</span></code>) – Include timestamps when data was published and revision chains.</p></li>
 <li><p><strong>filing_id</strong> (<code class="xref py py-data docutils literal notranslate"><span class="pre">Optional</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">int</span></code>]) – Filing ID for which to get data.  Get all of the data reported in this filing.</p></li>
-<li><p><strong>exclude_unconfirmed_preliminary</strong> (<code class="xref py py-data docutils literal notranslate"><span class="pre">Optional</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">bool</span></code>]) – Exclude points from press-releases or 8-Ks that have not been “confirmed” in an XBRL filing.  Preliminary points have a higher error rate than XBRL points.</p></li>
 <li><p><strong>pit_V2</strong> (<code class="xref py py-data docutils literal notranslate"><span class="pre">Optional</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">bool</span></code>]) – Defaults to True, use point in time V2, this only makes sense when point_in_time = True.  This will go away at some point.</p></li>
+<li><p><strong>XBRL_only</strong> (<code class="xref py py-data docutils literal notranslate"><span class="pre">Optional</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">bool</span></code>]) – Only get data that appeared in an XBRL document.  If supplied with start_date and end_date it will filter by the “confirming” filing_id.</p></li>
 </ul>
 </dd>
 <dt class="field-even">Returns</dt>
 <dd class="field-even"><p>Dataframe</p>
 </dd>
 </dl>
 <p>Standardized data with a timestamp when it was published by Calcbench.</p>
@@ -72,29 +72,29 @@
 <div><p>Columns:</p>
 </div></blockquote>
 <dl>
 <dt>ticker</dt><dd><p>Ticker of reporting company</p>
 </dd>
 <dt>metric</dt><dd><p>The metric name, see the definitions &#64; <a class="reference external" href="https://www.calcbench.com/home/standardizedmetrics">https://www.calcbench.com/home/standardizedmetrics</a></p>
 </dd>
-<dt>fiscal_period</dt><dd><p>fiscal_year-fiscal_period the fiscal period the value applies to.</p>
+<dt>fiscal_period</dt><dd><p>fiscal_year-fiscal_period the fiscal period the value applies to.  Like “2020-0” or “2021-3”.  0 indicates annual, 1,2,3,4 are quarters.</p>
 </dd>
 <dt>date_reported (PIT only)</dt><dd><p>Timestamp (EST) when Calcbench finished processing the filing from which this value was parsed.</p>
 <p>In some cases, particularly prior to 2015, this will be the filing date of the document as recorded by the SEC.  To exclude these points remove points where the hour is 0.</p>
 </dd>
 <dt>value</dt><dd><p>The value of the fact</p>
 </dd>
 <dt>revision_number</dt><dd><p>0 indicates an original, unrevised value for this fact. 1, 2, 3… indicates subsequent revisions to the fact value.  <a class="reference external" href="https://knowledge.calcbench.com/hc/en-us/search?utf8=%E2%9C%93&amp;query=revisions&amp;commit=Search">https://knowledge.calcbench.com/hc/en-us/search?utf8=%E2%9C%93&amp;query=revisions&amp;commit=Search</a></p>
 </dd>
 <dt>preliminary</dt><dd><p>True indicates the number was parsed from non-XBRL 8-K or press release from the wire</p>
 </dd>
 <dt>XBRL</dt><dd><p>Indicates the number was parsed from XBRL.</p>
 <p>The case where preliminary and XBRL are both true indicates the number was first parsed from a non-XBRL document then “confirmed” in an XBRL document.</p>
 </dd>
-<dt>date_XBRL_confirmed</dt><dd><p>Time at which the point was confirmed by an point from an XBRL filing.
+<dt>date_XBRL_confirmed</dt><dd><p>Time at which the point was confirmed by a point from an XBRL filing.
 If the point originally came from an XBRL filing this will be the original write time.
 If this is null, for points post April 2023, the point has not been confirmed.</p>
 </dd>
 <dt>period_start</dt><dd><p>First day of the fiscal period for this fact</p>
 </dd>
 <dt>period_end</dt><dd><p>Last day of the fiscal period for this fact</p>
 </dd>
@@ -116,14 +116,18 @@
 <dt>trace_url</dt><dd><p>URL for a page showing the source document for this value.</p>
 </dd>
 <dt>original_value (PIT only)</dt><dd><p>The value that Calcbench extracted when it first processed the filing.</p>
 <p>Post November 2022, if this differs from the value Calcbench the fact was modified by Calcbench subsequent to the filing first being processed.</p>
 </dd>
 <dt>standardized_id</dt><dd><p>A unique identifier Calcbench assigns to each standardized value.</p>
 </dd>
+<dt>date_XBRL_confirmed</dt><dd><p>The date this value was “confirmed” by an XBRL document.  For values originally appearing in press-release, this will be the date of the associated 10-K/Q.</p>
+</dd>
+<dt>confirming_XBRL_filing_ID</dt><dd><p>The filing_id of the XBRL document which contained this value.</p>
+</dd>
 <dt>date_downloaded</dt><dd><p>The timestamp on your computer when you downloaded this data.</p>
 </dd>
 </dl>
 <p>Usage:</p>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="gp">&gt;&gt;&gt; </span><span class="n">d</span> <span class="o">=</span> <span class="n">calcbench</span><span class="o">.</span><span class="n">standardized</span><span class="p">(</span><span class="n">company_identifiers</span><span class="o">=</span><span class="p">[</span><span class="s1">&#39;msft&#39;</span><span class="p">],</span>
 <span class="gp">&gt;&gt;&gt; </span>                                <span class="n">point_in_time</span><span class="o">=</span><span class="kc">True</span><span class="p">,)</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="p">)</span>
@@ -133,15 +137,15 @@
 <span class="gp">&gt;&gt;&gt; </span><span class="n">return_on_equity</span> <span class="o">=</span> <span class="n">d</span><span class="p">[</span><span class="s1">&#39;NetIncome&#39;</span><span class="p">]</span> <span class="o">/</span> <span class="n">d</span><span class="p">[</span><span class="s1">&#39;StockholdersEquity&#39;</span><span class="p">]</span>
 </pre></div>
 </div>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="calcbench.standardized_raw">
-<span class="sig-prename descclassname"><span class="pre">calcbench.</span></span><span class="sig-name descname"><span class="pre">standardized_raw</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">company_identifiers</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">metrics</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">start_year</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">start_period</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">end_year</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">end_period</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">entire_universe</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">point_in_time</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">include_trace</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">all_history</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">year</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">period</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">period_type</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">use_fiscal_period</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">all_face</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">all_footnotes</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">filing_id</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">all_non_GAAP</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">all_metrics</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">pit_V2</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">start_date</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">end_date</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exclude_unconfirmed_preliminary</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#calcbench.standardized_raw" title="Permalink to this definition">¶</a></dt>
+<span class="sig-prename descclassname"><span class="pre">calcbench.</span></span><span class="sig-name descname"><span class="pre">standardized_raw</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">company_identifiers</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">metrics</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">start_year</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">start_period</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">end_year</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">end_period</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">entire_universe</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">point_in_time</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">include_trace</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">all_history</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">year</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">period</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">period_type</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">use_fiscal_period</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">all_face</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">all_footnotes</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">filing_id</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">all_non_GAAP</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">all_metrics</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">pit_V2</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">start_date</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">end_date</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">XBRL_only</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#calcbench.standardized_raw" title="Permalink to this definition">¶</a></dt>
 <dd><p>Standardized data.</p>
 <p>Get normalized data from Calcbench.  Each point is normalized by economic concept and time period.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters</dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>company_identifiers</strong> (<code class="xref py py-class docutils literal notranslate"><span class="pre">Sequence</span></code>[<code class="xref py py-data docutils literal notranslate"><span class="pre">Union</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">str</span></code>, <code class="xref py py-class docutils literal notranslate"><span class="pre">int</span></code>]]) – a sequence of tickers (or CIK codes), eg [‘msft’, ‘goog’, ‘appl’]</p></li>
 <li><p><strong>metrics</strong> (<code class="xref py py-class docutils literal notranslate"><span class="pre">Sequence</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">str</span></code>]) – a sequence of metrics, see the full list &#64; <a class="reference external" href="https://www.calcbench.com/home/standardizedmetrics">https://www.calcbench.com/home/standardizedmetrics</a> eg. [‘revenue’, ‘accountsreceivable’]</p></li>
@@ -154,15 +158,15 @@
 <li><p><strong>year</strong> (<code class="xref py py-data docutils literal notranslate"><span class="pre">Optional</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">int</span></code>]) – Get data for a single year, defaults to annual data.</p></li>
 <li><p><strong>period_type</strong> (<code class="xref py py-data docutils literal notranslate"><span class="pre">Optional</span></code>[<a class="reference internal" href="#calcbench.api_query_params.PeriodType" title="calcbench.api_query_params.PeriodType"><code class="xref py py-class docutils literal notranslate"><span class="pre">PeriodType</span></code></a>]) – Either “annual” or “quarterly”</p></li>
 <li><p><strong>filing_id</strong> (<code class="xref py py-data docutils literal notranslate"><span class="pre">Optional</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">int</span></code>]) – Filing id for which to get data.  corresponds to the filing_id in the objects returned by the filings API.</p></li>
 <li><p><strong>all_non_GAAP</strong> (<code class="xref py py-class docutils literal notranslate"><span class="pre">bool</span></code>) – include all non-GAAP metrics from earnings press releases such as EBITDA_NonGAAP.  This is implied when querying by <cite>filing_id</cite>.</p></li>
 <li><p><strong>all_metrics</strong> (<code class="xref py py-class docutils literal notranslate"><span class="pre">bool</span></code>) – All metrics.</p></li>
 <li><p><strong>start_date</strong> (<code class="xref py py-data docutils literal notranslate"><span class="pre">Union</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">datetime</span></code>, <code class="xref py py-class docutils literal notranslate"><span class="pre">date</span></code>, <code class="xref py py-obj docutils literal notranslate"><span class="pre">None</span></code>]) – points modified from this date (inclusive).  If no time is specified all points from that date are returned.</p></li>
 <li><p><strong>end_date</strong> (<code class="xref py py-data docutils literal notranslate"><span class="pre">Union</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">datetime</span></code>, <code class="xref py py-class docutils literal notranslate"><span class="pre">date</span></code>, <code class="xref py py-obj docutils literal notranslate"><span class="pre">None</span></code>]) – points modified until this date (exclusive).  If not time is specified point modified prior to this date are returned.</p></li>
-<li><p><strong>exclude_unconfirmed_preliminary</strong> (<code class="xref py py-data docutils literal notranslate"><span class="pre">Optional</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">bool</span></code>]) – Exclude points from press-releases or 8-Ks that have not been “confirmed” in an XBRL filing.  Preliminary points have a higher error rate than XBRL points.</p></li>
+<li><p><strong>XBRL_only</strong> (<code class="xref py py-data docutils literal notranslate"><span class="pre">Optional</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">bool</span></code>]) – Only get data that appeared in an XBRL document.  If supplied with start_date and end_date it will filter by the “confirming” filing_id.</p></li>
 </ul>
 </dd>
 <dt class="field-even">Return type</dt>
 <dd class="field-even"><p><code class="xref py py-class docutils literal notranslate"><span class="pre">Sequence</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">StandardizedPoint</span></code>]</p>
 </dd>
 </dl>
 </dd></dl>
```

#### html2text {}

```diff
@@ -13,15 +13,15 @@
 Ks are also included.
 ***** StandardizedÂ¶ *****
 Calcbench standardizes +1000 metrics to handle differences in filersâs
 tagging. The list of stardized points is @ https://www.calcbench.com/home/
 standardizedmetrics
   calcbench.standardized(company_identifiers=[], metrics=[], fiscal_year=None,
   fiscal_period=None, start_date=None, end_date=None, point_in_time=False,
-  filing_id=None, exclude_unconfirmed_preliminary=False, pit_V2=None)Â¶
+  filing_id=None, pit_V2=None, XBRL_only=False)Â¶
       Standardized Numeric Data.
       The data behind the multi-company page, https://www.calcbench.com/multi.
       Example https://github.com/calcbench/notebooks/blob/master/
       python_client_api_demo.ipynb
         Parameters
                 * company_identifiers (Sequence[Union[str, int]]) â Tickers/
                   CIK codes. eg. [âmsftâ, âgoogâ, âapplâ,
@@ -40,21 +40,20 @@
                   records modified on or after (inclusive) this date/datetime
                 * end_date (Union[datetime, date, None]) â Restric to records
                   modified prior (exclusive) thie date/datetime
                 * point_in_time (bool) â Include timestamps when data was
                   published and revision chains.
                 * filing_id (Optional[int]) â Filing ID for which to get
                   data. Get all of the data reported in this filing.
-                * exclude_unconfirmed_preliminary (Optional[bool]) â Exclude
-                  points from press-releases or 8-Ks that have not been
-                  âconfirmedâ in an XBRL filing. Preliminary points have a
-                  higher error rate than XBRL points.
                 * pit_V2 (Optional[bool]) â Defaults to True, use point in
                   time V2, this only makes sense when point_in_time = True.
                   This will go away at some point.
+                * XBRL_only (Optional[bool]) â Only get data that appeared in
+                  an XBRL document. If supplied with start_date and end_date it
+                  will filter by the âconfirmingâ filing_id.
         Returns
             Dataframe
       Standardized data with a timestamp when it was published by Calcbench.
       A record is returned for each filing in which a metric value changed (was
       revised).
       If the company files an 8-K with revenue = $100 then a week later files a
       10-K with revenue = $100 one record will be returned for that period. It
@@ -71,14 +70,16 @@
         ticker
             Ticker of reporting company
         metric
             The metric name, see the definitions @ https://www.calcbench.com/
             home/standardizedmetrics
         fiscal_period
             fiscal_year-fiscal_period the fiscal period the value applies to.
+            Like â2020-0â or â2021-3â. 0 indicates annual, 1,2,3,4 are
+            quarters.
         date_reported (PIT only)
             Timestamp (EST) when Calcbench finished processing the filing from
             which this value was parsed.
             In some cases, particularly prior to 2015, this will be the filing
             date of the document as recorded by the SEC. To exclude these
             points remove points where the hour is 0.
         value
@@ -93,15 +94,15 @@
             release from the wire
         XBRL
             Indicates the number was parsed from XBRL.
             The case where preliminary and XBRL are both true indicates the
             number was first parsed from a non-XBRL document then
             âconfirmedâ in an XBRL document.
         date_XBRL_confirmed
-            Time at which the point was confirmed by an point from an XBRL
+            Time at which the point was confirmed by a point from an XBRL
             filing. If the point originally came from an XBRL filing this will
             be the original write time. If this is null, for points post April
             2023, the point has not been confirmed.
         period_start
             First day of the fiscal period for this fact
         period_end
             Last day of the fiscal period for this fact
@@ -131,14 +132,20 @@
             The value that Calcbench extracted when it first processed the
             filing.
             Post November 2022, if this differs from the value Calcbench the
             fact was modified by Calcbench subsequent to the filing first being
             processed.
         standardized_id
             A unique identifier Calcbench assigns to each standardized value.
+        date_XBRL_confirmed
+            The date this value was âconfirmedâ by an XBRL document. For
+            values originally appearing in press-release, this will be the date
+            of the associated 10-K/Q.
+        confirming_XBRL_filing_ID
+            The filing_id of the XBRL document which contained this value.
         date_downloaded
             The timestamp on your computer when you downloaded this data.
       Usage:
       >>> d = calcbench.standardized(company_identifiers=['msft'],
       >>>                                 point_in_time=True,)
       >>> )
       >>> # Put the data in a format amiable to arithmetic on columns
@@ -148,15 +155,15 @@
       >>> return_on_equity = d['NetIncome'] / d['StockholdersEquity']
   calcbench.standardized_raw(company_identifiers=[], metrics=[],
   start_year=None, start_period=None, end_year=None, end_period=None,
   entire_universe=False, point_in_time=False, include_trace=False,
   all_history=False, year=None, period=None, period_type=None,
   use_fiscal_period=False, all_face=False, all_footnotes=False, filing_id=None,
   all_non_GAAP=False, all_metrics=False, pit_V2=False, start_date=None,
-  end_date=None, exclude_unconfirmed_preliminary=False)Â¶
+  end_date=None, XBRL_only=False)Â¶
       Standardized data.
       Get normalized data from Calcbench. Each point is normalized by economic
       concept and time period.
         Parameters
                 * company_identifiers (Sequence[Union[str, int]]) â a
                   sequence of tickers (or CIK codes), eg [âmsftâ,
                   âgoogâ, âapplâ]
@@ -190,18 +197,17 @@
                 * all_metrics (bool) â All metrics.
                 * start_date (Union[datetime, date, None]) â points modified
                   from this date (inclusive). If no time is specified all
                   points from that date are returned.
                 * end_date (Union[datetime, date, None]) â points modified
                   until this date (exclusive). If not time is specified point
                   modified prior to this date are returned.
-                * exclude_unconfirmed_preliminary (Optional[bool]) â Exclude
-                  points from press-releases or 8-Ks that have not been
-                  âconfirmedâ in an XBRL filing. Preliminary points have a
-                  higher error rate than XBRL points.
+                * XBRL_only (Optional[bool]) â Only get data that appeared in
+                  an XBRL document. If supplied with start_date and end_date it
+                  will filter by the âconfirmingâ filing_id.
         Return type
             Sequence[StandardizedPoint]
   classcalcbench.api_query_params.Period(value)
       An enumeration.
         Annual= 0
         Failure= -1
             Should be few and far between, indicates something went wrong
```

### Comparing `calcbench_api_client-8.2.0/docs/html/press-release.html` & `calcbench_api_client-9.0.0/docs/html/press-release.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/docs/html/push-notification.html` & `calcbench_api_client-9.0.0/docs/html/push-notification.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/docs/html/py-modindex.html` & `calcbench_api_client-9.0.0/docs/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/docs/html/raw-numeric-XBRL.html` & `calcbench_api_client-9.0.0/docs/html/raw-numeric-XBRL.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/docs/html/raw-numeric-non-XBRL.html` & `calcbench_api_client-9.0.0/docs/html/raw-numeric-non-XBRL.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/docs/html/search.html` & `calcbench_api_client-9.0.0/docs/html/search.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/docs/html/searchindex.js` & `calcbench_api_client-9.0.0/docs/html/searchindex.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -698,15 +698,16 @@
         "2": [1, 2, 8, 11],
         "20": [1, 5],
         "200": 8,
         "2015": 8,
         "2017": 4,
         "2018": [1, 4],
         "2019": 11,
-        "2021": 11,
+        "2020": 8,
+        "2021": [8, 11],
         "2022": 8,
         "2023": 8,
         "20fr12g": 5,
         "21": 1,
         "22": 1,
         "223267767": 8,
         "23": 1,
@@ -822,15 +823,15 @@
         "try": 6,
         "while": [5, 8],
         A: [1, 2, 5, 8, 10, 11],
         And: 2,
         As: 2,
         At: 7,
         By: [2, 6],
-        For: [1, 2],
+        For: [1, 2, 8],
         If: [1, 3, 6, 8, 10],
         In: 8,
         Is: 4,
         It: [2, 8],
         NOT: [],
         Not: 5,
         OR: [5, 6],
@@ -877,24 +878,25 @@
         alwai: 10,
         am: 5,
         amend: 5,
         amiabl: 8,
         amount: [],
         an: [1, 2, 4, 5, 6, 8, 9, 10, 11],
         analysi: 2,
+        andr: 3,
         andrew: 6,
         ani: [1, 4, 6],
         annlrpt: 5,
         annual: [1, 2, 4, 5, 8],
         annualquarterlyreport: 5,
         anoth: [],
         apach: 2,
         api: [1, 3, 5, 6, 8, 10, 11],
         api_query_param: [1, 2, 5, 8, 11],
-        appear: [5, 11],
+        appear: [5, 8, 11],
         append: 3,
         appl: [1, 8],
         appli: [3, 8],
         applic: [1, 2],
         applymap: 2,
         april: 8,
         ar: [0, 1, 2, 5, 6, 8],
@@ -907,15 +909,15 @@
         ask: 6,
         asset: 2,
         assetsandliabilitiesatfairvalu: 1,
         assetsandliabilitiesatfairvaluelevel1: 1,
         assetsandliabilitiesatfairvaluelevel2: 1,
         assetsandliabilitiesatfairvaluelevel3: 1,
         assign: [5, 8],
-        associ: 1,
+        associ: [1, 8],
         associated_earnings_press_release_sec_url: 5,
         associated_proxy_sec_url: 5,
         attempt: 11,
         avail: 2,
         availablebreakout: 1,
         avoid: [],
         awai: 8,
@@ -981,14 +983,15 @@
         businesscombinationliabilitiesassumeddeferredrevenu: 1,
         businesscombinationliabilitiesassumedlongtermdebt: 1,
         businesscombinationpurchasepric: 1,
         businesscombinationrecognizedidentifiableassetsacquiredandliabilitiesassumedasset: 1,
         businesswirepr_filedafteran8k: 5,
         businesswirepr_replac: 5,
         bya: 1,
+        c: 3,
         calcbench: [0, 1, 2, 3, 4, 5, 6, 8, 9, 10, 11],
         calcbench_accept: 5,
         calcbench_api: 6,
         calcbench_entity_id: [1, 8],
         calcbench_finished_load: 5,
         calcbench_id: [5, 10],
         calcbench_password: 6,
@@ -1047,18 +1050,19 @@
         comprehensiveincom: 4,
         compustat: [],
         comput: [3, 8],
         concentrationriskpercentagecustom: 1,
         concentrationriskpercentagesuppli: 1,
         concept: [8, 11],
         confirm: 8,
+        confirming_xbrl_filing_id: 8,
         connect: 10,
         connection_str: 10,
         consequ: [],
-        contain: 1,
+        contain: [1, 8],
         content: 2,
         conting: 2,
         continu: 6,
         contract: 2,
         coorespond: [2, 11],
         core: 2,
         corresp: 5,
@@ -1219,37 +1223,38 @@
         end: [1, 2, 11],
         end_dat: [2, 5, 8],
         end_period: [1, 8],
         end_year: [1, 8],
         endpoint: 10,
         enterprise_valu: 0,
         entire_univers: [2, 3, 5, 8, 11],
+        entire_universe_standardized_pit: 3,
         entiti: 5,
         entity_id: [2, 5, 9],
         entity_nam: [2, 4, 5, 9, 11],
         entityid: 11,
         enumer: [1, 2, 4, 5, 8, 9, 11],
         environ: 6,
         equiti: [2, 4],
         equitymethodinvest: 1,
         equitymethodinvestmentdividendsordistribut: 1,
         equitymethodinvestmentrealizedgainlossondispos: 1,
         equival: 2,
-        error: [7, 8],
+        error: 7,
         esma: 5,
         est: [2, 8],
         estim: 3,
         etc: [4, 5, 8],
         eur: 11,
         ex: 5,
         exampl: [1, 8, 11],
         except: [6, 10],
         exclud: 8,
         exclude_error: [],
-        exclude_unconfirmed_preliminari: 8,
+        exclude_unconfirmed_preliminari: [],
         exclus: 8,
         expens: 2,
         exponenti: 6,
         expr: 3,
         extensionanchor: 11,
         extract: [8, 11],
         extract_tag: 11,
@@ -1305,15 +1310,15 @@
         filing_period: 11,
         filing_typ: [1, 2, 5, 8, 9],
         filing_year: 11,
         filingd: 11,
         filingid: 11,
         filings_datafram: 5,
         filingtyp: 5,
-        filter: 3,
+        filter: [3, 8],
         financi: 7,
         financialstatementcolumn: 4,
         finish: 8,
         finitelivedintangibleassetsaccumulatedamort: 1,
         finitelivedintangibleassetsacquir: 1,
         finitelivedintangibleassetsgross: 1,
         finitelivedintangibleassetsnet: 1,
@@ -1390,15 +1395,15 @@
         has_standardized_data: 5,
         hash: 3,
         have: [5, 6, 8],
         hc: 8,
         header: 2,
         hedg: 2,
         high: 11,
-        higher: 8,
+        higher: [],
         histori: [1, 2, 4, 8],
         home: 8,
         hour: 8,
         how: 2,
         hr: 5,
         html: 2,
         http: [1, 2, 4, 5, 6, 7, 8, 10, 11],
@@ -1489,15 +1494,15 @@
         last_quart: 8,
         latenc: 7,
         later: 8,
         leas: 2,
         legacy_report: 0,
         letter: 2,
         level: [2, 6],
-        like: [4, 10, 11],
+        like: [4, 8, 10, 11],
         line: [1, 8],
         line_item: 4,
         lineitem: 4,
         link1: 5,
         link2: 5,
         link3: 5,
         link: 4,
@@ -1695,15 +1700,15 @@
         queue: 10,
         random: 3,
         rang: 11,
         range_high: 11,
         range_high_valu: 9,
         range_low: 11,
         rare: 11,
-        rate: 8,
+        rate: [],
         rather: 1,
         raw: 7,
         raw_numeric_non_xbrl: 11,
         rawdataclaus: 11,
         rawdatanonxbrlpoint: 11,
         re: 6,
         read: 3,
@@ -1831,15 +1836,15 @@
         special_fact_typ: [4, 11],
         specif: [2, 11],
         specifi: 8,
         split: 2,
         stack: [],
         standar: [],
         standard: [0, 3, 5, 6, 7, 11],
-        standardized_data: [],
+        standardized_data: 3,
         standardized_id: 8,
         standardized_numer: [0, 1],
         standardized_pit_arrow: 3,
         standardized_ppa_point: 0,
         standardized_raw: 8,
         standardized_xbrl: [5, 10],
         standardizedmetr: 8,
@@ -1865,15 +1870,15 @@
         strftime: 11,
         string: [1, 10],
         sub_divid: 2,
         subscript: [6, 10, 11],
         subscription_nam: 10,
         subsequ: [5, 8],
         suffix: 1,
-        suppli: [1, 2],
+        suppli: [1, 2, 8],
         syntax: 2,
         system: 10,
         systemd: 10,
         t: [3, 10],
         tabl: [1, 3, 5],
         table_id: 9,
         table_list: 2,
@@ -1883,15 +1888,15 @@
         talk: [6, 8, 10],
         target: 0,
         tax: 2,
         text: [7, 9],
         text_fact_id: 4,
         textblock: 2,
         tf: 2,
-        than: [1, 8],
+        than: 1,
         thei: 5,
         thi: [0, 2, 3, 4, 5, 6, 8, 10, 11],
         thie: 8,
         thing: 2,
         this_period_revenu: 5,
         three: 8,
         ticker: [1, 2, 3, 4, 5, 8, 9, 11],
@@ -1936,15 +1941,15 @@
         url: [1, 4, 8, 9, 11],
         us: [0, 2, 3, 6, 8, 11],
         usag: [1, 2, 3, 4, 5, 6, 8, 10, 11],
         usd: 11,
         use_fiscal_period: [2, 8],
         useful_life_lower_rang: 0,
         useful_life_upper_rang: 0,
-        user: 6,
+        user: [3, 6],
         utf8: 8,
         util: 3,
         v2: 8,
         valu: [0, 1, 2, 4, 5, 8, 9, 11],
         variabl: 6,
         varieti: 11,
         verbos: 6,
@@ -1966,22 +1971,25 @@
         wire: [5, 8, 10],
         wirepr: 5,
         wirepress: [],
         word_count: 2,
         work: [],
         would: 11,
         write: [3, 8, 10],
+        write_csv: 3,
         write_index: 3,
         write_mod: 3,
+        write_t: 3,
         written: 3,
         wrong: 8,
         wrote: 8,
         www: [1, 2, 4, 5, 6, 8, 11],
         x: 5,
         xbrl: [2, 4, 5, 7, 8],
+        xbrl_onli: 8,
         xbrldisclosur: 2,
         xbrlfilingid: 11,
         y: [4, 11],
         year: [1, 2, 8, 9, 11],
         yet: [],
         you: [2, 6, 8, 10],
         your: [6, 8, 10]
```

### Comparing `calcbench_api_client-8.2.0/docs/make.bat` & `calcbench_api_client-9.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/docs/source/conf.py` & `calcbench_api_client-9.0.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/docs/source/getting-started.rst` & `calcbench_api_client-9.0.0/docs/source/getting-started.rst`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/docs/source/index.rst` & `calcbench_api_client-9.0.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/docs/source/numeric-data.rst` & `calcbench_api_client-9.0.0/docs/source/numeric-data.rst`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/docs/source/push-notification.rst` & `calcbench_api_client-9.0.0/docs/source/push-notification.rst`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-8.2.0/setup.py` & `calcbench_api_client-9.0.0/setup.py`

 * *Files identical despite different names*

