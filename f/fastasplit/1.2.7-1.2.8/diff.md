# Comparing `tmp/fastasplit-1.2.7.tar.gz` & `tmp/fastasplit-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastasplit-1.2.7.tar", last modified: Mon Jul 10 19:21:49 2023, max compression
+gzip compressed data, was "fastasplit-1.2.8.tar", last modified: Tue Jul 11 00:31:38 2023, max compression
```

## Comparing `fastasplit-1.2.7.tar` & `fastasplit-1.2.8.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 joshuabenoit   (501) staff       (20)        0 2023-07-10 19:21:49.829859 fastasplit-1.2.7/
--rw-r--r--   0 joshuabenoit   (501) staff       (20)    35149 2023-07-10 18:45:06.000000 fastasplit-1.2.7/LICENSE
--rw-r--r--   0 joshuabenoit   (501) staff       (20)     1140 2023-07-10 19:21:49.829975 fastasplit-1.2.7/PKG-INFO
--rw-r--r--   0 joshuabenoit   (501) staff       (20)      805 2023-07-10 18:45:06.000000 fastasplit-1.2.7/README.md
--rw-r--r--   0 joshuabenoit   (501) staff       (20)       80 2023-07-10 18:45:06.000000 fastasplit-1.2.7/pyproject.toml
--rw-r--r--   0 joshuabenoit   (501) staff       (20)      589 2023-07-10 19:21:49.830648 fastasplit-1.2.7/setup.cfg
-drwxr-xr-x   0 joshuabenoit   (501) staff       (20)        0 2023-07-10 19:21:49.823246 fastasplit-1.2.7/src/
-drwxr-xr-x   0 joshuabenoit   (501) staff       (20)        0 2023-07-10 19:21:49.825497 fastasplit-1.2.7/src/fastasplit/
--rw-r--r--   0 joshuabenoit   (501) staff       (20)        0 2023-07-10 18:45:06.000000 fastasplit-1.2.7/src/fastasplit/__init__.py
--rwxr-xr-x   0 joshuabenoit   (501) staff       (20)     7834 2023-07-10 18:45:06.000000 fastasplit-1.2.7/src/fastasplit/fastasplit.py
-drwxr-xr-x   0 joshuabenoit   (501) staff       (20)        0 2023-07-10 19:21:49.829551 fastasplit-1.2.7/src/fastasplit.egg-info/
--rw-r--r--   0 joshuabenoit   (501) staff       (20)     1140 2023-07-10 19:21:49.000000 fastasplit-1.2.7/src/fastasplit.egg-info/PKG-INFO
--rw-r--r--   0 joshuabenoit   (501) staff       (20)      291 2023-07-10 19:21:49.000000 fastasplit-1.2.7/src/fastasplit.egg-info/SOURCES.txt
--rw-r--r--   0 joshuabenoit   (501) staff       (20)        1 2023-07-10 19:21:49.000000 fastasplit-1.2.7/src/fastasplit.egg-info/dependency_links.txt
--rw-r--r--   0 joshuabenoit   (501) staff       (20)       58 2023-07-10 19:21:49.000000 fastasplit-1.2.7/src/fastasplit.egg-info/entry_points.txt
--rw-r--r--   0 joshuabenoit   (501) staff       (20)       11 2023-07-10 19:21:49.000000 fastasplit-1.2.7/src/fastasplit.egg-info/top_level.txt
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-07-11 00:31:38.312608 fastasplit-1.2.8/
+-rw-rw-r--   0 josh      (1000) josh      (1000)      599 2023-07-11 00:30:21.000000 fastasplit-1.2.8/CHANGELOG.md
+-rw-rw-r--   0 josh      (1000) josh      (1000)    35149 2023-07-08 02:32:46.000000 fastasplit-1.2.8/LICENSE
+-rw-rw-r--   0 josh      (1000) josh      (1000)     1740 2023-07-11 00:31:38.312608 fastasplit-1.2.8/PKG-INFO
+-rw-rw-r--   0 josh      (1000) josh      (1000)      805 2023-07-09 04:33:28.000000 fastasplit-1.2.8/README.md
+-rw-rw-r--   0 josh      (1000) josh      (1000)       80 2023-07-09 03:59:24.000000 fastasplit-1.2.8/pyproject.toml
+-rw-rw-r--   0 josh      (1000) josh      (1000)      603 2023-07-11 00:31:38.312608 fastasplit-1.2.8/setup.cfg
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-07-11 00:31:38.304608 fastasplit-1.2.8/src/
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-07-11 00:31:38.308608 fastasplit-1.2.8/src/fastasplit/
+-rw-rw-r--   0 josh      (1000) josh      (1000)        0 2023-07-09 03:59:24.000000 fastasplit-1.2.8/src/fastasplit/__init__.py
+-rwxrwxr-x   0 josh      (1000) josh      (1000)    10490 2023-07-11 00:30:21.000000 fastasplit-1.2.8/src/fastasplit/fastasplit.py
+drwxrwxr-x   0 josh      (1000) josh      (1000)        0 2023-07-11 00:31:38.312608 fastasplit-1.2.8/src/fastasplit.egg-info/
+-rw-rw-r--   0 josh      (1000) josh      (1000)     1740 2023-07-11 00:31:38.000000 fastasplit-1.2.8/src/fastasplit.egg-info/PKG-INFO
+-rw-rw-r--   0 josh      (1000) josh      (1000)      304 2023-07-11 00:31:38.000000 fastasplit-1.2.8/src/fastasplit.egg-info/SOURCES.txt
+-rw-rw-r--   0 josh      (1000) josh      (1000)        1 2023-07-11 00:31:38.000000 fastasplit-1.2.8/src/fastasplit.egg-info/dependency_links.txt
+-rw-rw-r--   0 josh      (1000) josh      (1000)       58 2023-07-11 00:31:38.000000 fastasplit-1.2.8/src/fastasplit.egg-info/entry_points.txt
+-rw-rw-r--   0 josh      (1000) josh      (1000)       11 2023-07-11 00:31:38.000000 fastasplit-1.2.8/src/fastasplit.egg-info/top_level.txt
```

### Comparing `fastasplit-1.2.7/LICENSE` & `fastasplit-1.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fastasplit-1.2.7/PKG-INFO` & `fastasplit-1.2.8/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastasplit
-Version: 1.2.7
+Version: 1.2.8
 Summary: Split fasta files
 Home-page: https://github.com/jtompkin/fastasplit
 Author: Josh Tompkin
 Author-email: tompkinjo@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -40,7 +40,46 @@
 ```bash
     fastasplit -n 10 -s sequences.fa
 ```
 Split each sequence in 'sequences.fa' into a separate file:
 ```bash
     fastasplit -e sequences.fa
 ```
+
+# Changelog
+
+## [1.0.0] - 2023-06-??
+
+### Added
+- Ability to split fasta files into n number of files
+
+## [1.1.0] - 2023-06-??
+
+### Added
+- Ability to split fasta files by number of sequences
+
+## [1.2.0] - 2023-06-??
+
+### Added
+- Ability to split each sequence in fasta file to separate file
+
+## [1.2.2] - 2023-07-??
+
+### Fixed
+- Formatting errors
+### Added
+- Checks for large numbers of output files
+
+## [1.2.6] - 2023-07-08
+
+### Changed
+- **breaking:** Now installs with pip
+
+## [1.2.7] - 2023-07-10
+
+### Added
+- Documentation for pypi
+
+## [1.2.8] - 2023-07-10
+
+### Changed
+- Formatting in source
```

### Comparing `fastasplit-1.2.7/README.md` & `fastasplit-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `fastasplit-1.2.7/setup.cfg` & `fastasplit-1.2.8/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = fastasplit
-version = 1.2.7
+version = 1.2.8
 author = Josh Tompkin
 author_email = tompkinjo@gmail.com
 description = Split fasta files
-long_description = file: README.md
+long_description = file: README.md, CHANGELOG.md
 long_description_content_type = text/markdown
 url = https://github.com/jtompkin/fastasplit
 license = GPLv3
 classifiers = 
 	Programming Language :: Python :: 3
 
 [options]
```

### Comparing `fastasplit-1.2.7/src/fastasplit.egg-info/PKG-INFO` & `fastasplit-1.2.8/src/fastasplit.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastasplit
-Version: 1.2.7
+Version: 1.2.8
 Summary: Split fasta files
 Home-page: https://github.com/jtompkin/fastasplit
 Author: Josh Tompkin
 Author-email: tompkinjo@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -40,7 +40,46 @@
 ```bash
     fastasplit -n 10 -s sequences.fa
 ```
 Split each sequence in 'sequences.fa' into a separate file:
 ```bash
     fastasplit -e sequences.fa
 ```
+
+# Changelog
+
+## [1.0.0] - 2023-06-??
+
+### Added
+- Ability to split fasta files into n number of files
+
+## [1.1.0] - 2023-06-??
+
+### Added
+- Ability to split fasta files by number of sequences
+
+## [1.2.0] - 2023-06-??
+
+### Added
+- Ability to split each sequence in fasta file to separate file
+
+## [1.2.2] - 2023-07-??
+
+### Fixed
+- Formatting errors
+### Added
+- Checks for large numbers of output files
+
+## [1.2.6] - 2023-07-08
+
+### Changed
+- **breaking:** Now installs with pip
+
+## [1.2.7] - 2023-07-10
+
+### Added
+- Documentation for pypi
+
+## [1.2.8] - 2023-07-10
+
+### Changed
+- Formatting in source
```

