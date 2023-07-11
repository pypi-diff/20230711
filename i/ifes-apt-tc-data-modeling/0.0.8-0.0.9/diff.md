# Comparing `tmp/ifes_apt_tc_data_modeling-0.0.8.tar.gz` & `tmp/ifes_apt_tc_data_modeling-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifes_apt_tc_data_modeling-0.0.8.tar", last modified: Wed May  3 08:16:00 2023, max compression
+gzip compressed data, was "ifes_apt_tc_data_modeling-0.0.9.tar", last modified: Tue Jul 11 08:34:10 2023, max compression
```

## Comparing `ifes_apt_tc_data_modeling-0.0.8.tar` & `ifes_apt_tc_data_modeling-0.0.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-05-03 08:16:00.466841 ifes_apt_tc_data_modeling-0.0.8/
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    11358 2023-01-13 23:09:44.000000 ifes_apt_tc_data_modeling-0.0.8/LICENSE.txt
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    22620 2023-05-03 08:16:00.466841 ifes_apt_tc_data_modeling-0.0.8/PKG-INFO
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     9003 2023-04-28 12:07:31.000000 ifes_apt_tc_data_modeling-0.0.8/README.md
-drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-05-03 08:16:00.456841 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      668 2023-03-20 08:50:24.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/__init__.py
-drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-05-03 08:16:00.456841 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/apt/
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      668 2023-03-20 09:06:23.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/apt/__init__.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     4093 2023-05-02 08:53:17.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/apt/apt6_headers.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    11504 2023-05-03 08:04:23.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/apt/apt6_reader.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    19741 2023-05-02 08:53:17.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/apt/apt6_sections.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    34086 2023-05-02 08:53:17.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/apt/apt6_sections_branches.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     1572 2023-05-02 08:53:17.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/apt/apt6_utils.py
-drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-05-03 08:16:00.456841 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/epos/
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      668 2023-03-20 09:03:51.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/epos/__init__.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     7524 2023-05-02 09:14:22.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/epos/epos_reader.py
-drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-05-03 08:16:00.456841 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/fig/
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      668 2023-03-20 08:58:26.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/fig/__init__.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     5774 2023-05-02 09:14:22.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/fig/fig_reader.py
-drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-05-03 08:16:00.456841 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/nexus/
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      668 2023-03-20 08:59:34.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/nexus/__init__.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     1604 2023-05-02 08:53:17.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/nexus/nx_field.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     7995 2023-05-02 09:14:22.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/nexus/nx_ion.py
-drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-05-03 08:16:00.456841 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/pos/
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      663 2023-03-20 08:58:38.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/pos/__init__.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     3207 2023-05-02 09:14:22.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/pos/pos_reader.py
-drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-05-03 08:16:00.456841 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/rng/
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      668 2023-03-20 08:58:26.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/rng/__init__.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     8079 2023-05-02 09:14:22.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/rng/rng_reader.py
-drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-05-03 08:16:00.456841 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/rrng/
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      663 2023-03-20 08:58:13.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/rrng/__init__.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     9241 2023-05-02 09:14:22.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/rrng/rrng_reader.py
-drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-05-03 08:16:00.466841 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/utils/
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      668 2023-03-20 08:50:24.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/utils/__init__.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     1354 2023-05-02 08:53:17.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/utils/definitions.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     1732 2023-05-02 08:53:17.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/utils/mmapped_io.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    17104 2023-05-02 09:14:22.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/utils/molecular_ions.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)   164819 2023-03-20 08:50:51.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/utils/nist_isotope_data.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     1272 2023-05-02 08:53:17.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/utils/string_handling.py
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     8572 2023-05-02 09:14:22.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/utils/utils.py
-drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-05-03 08:16:00.456841 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling.egg-info/
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    22620 2023-05-03 08:16:00.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling.egg-info/PKG-INFO
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     1496 2023-05-03 08:16:00.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling.egg-info/SOURCES.txt
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)        1 2023-05-03 08:16:00.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling.egg-info/dependency_links.txt
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      139 2023-05-03 08:16:00.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling.egg-info/requires.txt
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)       26 2023-05-03 08:16:00.000000 ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling.egg-info/top_level.txt
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     1051 2023-05-03 08:14:00.000000 ifes_apt_tc_data_modeling-0.0.8/pyproject.toml
--rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)       38 2023-05-03 08:16:00.466841 ifes_apt_tc_data_modeling-0.0.8/setup.cfg
+drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-07-11 08:34:10.359054 ifes_apt_tc_data_modeling-0.0.9/
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    11358 2023-07-11 07:37:20.000000 ifes_apt_tc_data_modeling-0.0.9/LICENSE.txt
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    23089 2023-07-11 08:34:10.359054 ifes_apt_tc_data_modeling-0.0.9/PKG-INFO
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     9472 2023-07-11 08:29:59.000000 ifes_apt_tc_data_modeling-0.0.9/README.md
+drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-07-11 08:34:10.349054 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      668 2023-07-11 07:37:20.000000 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/__init__.py
+drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-07-11 08:34:10.359054 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/apt/
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      668 2023-07-11 07:37:20.000000 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/apt/__init__.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     4093 2023-07-11 07:37:20.000000 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/apt/apt6_headers.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    11504 2023-07-11 07:37:20.000000 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/apt/apt6_reader.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    19741 2023-07-11 07:37:20.000000 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/apt/apt6_sections.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    34086 2023-07-11 07:37:20.000000 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/apt/apt6_sections_branches.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     1572 2023-07-11 07:37:20.000000 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/apt/apt6_utils.py
+drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-07-11 08:34:10.359054 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/epos/
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      668 2023-07-11 07:37:20.000000 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/epos/__init__.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     7524 2023-07-11 07:37:20.000000 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/epos/epos_reader.py
+drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-07-11 08:34:10.359054 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/fig/
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      668 2023-07-11 07:37:20.000000 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/fig/__init__.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     5774 2023-07-11 07:37:20.000000 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/fig/fig_reader.py
+drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-07-11 08:34:10.359054 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/nexus/
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      668 2023-07-11 07:37:20.000000 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/nexus/__init__.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     1604 2023-07-11 07:37:20.000000 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/nexus/nx_field.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     7995 2023-07-11 07:37:20.000000 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/nexus/nx_ion.py
+drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-07-11 08:34:10.359054 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/pos/
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      663 2023-07-11 07:37:20.000000 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/pos/__init__.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     3207 2023-07-11 07:37:20.000000 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/pos/pos_reader.py
+drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-07-11 08:34:10.359054 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/rng/
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      668 2023-07-11 07:37:20.000000 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/rng/__init__.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     8079 2023-07-11 07:37:20.000000 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/rng/rng_reader.py
+drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-07-11 08:34:10.359054 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/rrng/
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      663 2023-07-11 07:37:20.000000 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/rrng/__init__.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     9241 2023-07-11 07:37:20.000000 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/rrng/rrng_reader.py
+drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-07-11 08:34:10.359054 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/utils/
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      668 2023-07-11 07:37:20.000000 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/utils/__init__.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     1354 2023-07-11 07:37:20.000000 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/utils/definitions.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     1732 2023-07-11 07:37:20.000000 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/utils/mmapped_io.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    17104 2023-07-11 07:37:20.000000 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/utils/molecular_ions.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)   164819 2023-07-11 07:37:20.000000 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/utils/nist_isotope_data.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     1272 2023-07-11 07:37:20.000000 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/utils/string_handling.py
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     8572 2023-07-11 07:37:20.000000 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/utils/utils.py
+drwxr-xr-x   0 mkuehbach  (1000) mkuehbach  (1000)        0 2023-07-11 08:34:10.349054 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling.egg-info/
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)    23089 2023-07-11 08:34:10.000000 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling.egg-info/PKG-INFO
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     1496 2023-07-11 08:34:10.000000 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling.egg-info/SOURCES.txt
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)        1 2023-07-11 08:34:10.000000 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling.egg-info/dependency_links.txt
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)      146 2023-07-11 08:34:10.000000 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling.egg-info/requires.txt
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)       26 2023-07-11 08:34:10.000000 ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling.egg-info/top_level.txt
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)     1057 2023-07-11 08:28:51.000000 ifes_apt_tc_data_modeling-0.0.9/pyproject.toml
+-rw-r--r--   0 mkuehbach  (1000) mkuehbach  (1000)       38 2023-07-11 08:34:10.359054 ifes_apt_tc_data_modeling-0.0.9/setup.cfg
```

### Comparing `ifes_apt_tc_data_modeling-0.0.8/LICENSE.txt` & `ifes_apt_tc_data_modeling-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.8/PKG-INFO` & `ifes_apt_tc_data_modeling-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifes_apt_tc_data_modeling
-Version: 0.0.8
+Version: 0.0.9
 Summary: Foster exchange about data models and work towards clear specifications of file formats and data models in the research field of atom probe microscopy.
 Author: The NOMAD Authors
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -218,168 +218,171 @@
 
 # atomprobe-data-modeling
 
 ## Mission:
 Foster exchange about data models and work towards specifications
 of file formats from the research field of atom probe microscopy.
 
-## Documentation of file formats and data models in atom probe status quo
-Detailed technical specifications of the file formats and data models are not
-available for all formats in the field of atom probe microscopy.
-A practical solution to address this limitation so far has been that scientists collect
-examples in respective formats, so-called instances, and inspect and share these.
-Based on this reverse engineering, individual atom probers have contributed to formulate
-what can be considered likely candidates of the specification for several file formats.
-This worked especially well for the POS and ePOS formats.
-
-Pieces of information about file formats are reported in the literature in e.g.
-books by D. Larson et al. and B. Gault et al. Atom probers like D. Haley have contributed
-substantially to make the community aware of existent limitations and these
-reverse engineering practices. AMETEK/Cameca is the key technology partner in atom probe.
-The company has created an open file format called APT which improves the accessibility of
-specific numerical data and some metadata. Individuals like M. Kühbach have driven the
-implementation and communication of parsers for this APT file format.
-
-Nowadays there is an increased interest and demand placed on atom probers by the funding
-agencies that researchers should and have to make their research data management and data
-stewardship better matching and more completely aligned to the aims and practices of
-F.A.I.R. research principles. Therefore, it is useful to exchange more details about
-data models and file formats as otherwise it is not foreseeable how atom probe data
-can be made really interoperable with electronic lab notebooks, research data management
-systems (RDMS), and related software tools.
-
-In light of these challenges, the idea of understanding formats just by examples,
-showed to be a slow and error-prone route as e.g. source code and workflows which have
-been useed to write such files, and the associated input, workflow, and provenance information
-might have been or not captured or/and the specific software tool(s) used might not have been
-shared or made accessible for reviewing and analyzing their functions.
-
-## Benefit and Next Steps
-You can easily imagine that the more people will support us with this work the
-more complete our understanding and knowledge about the available file formats
-in atom probe microscopy can and will become. This can help all of us in the
-long run to build software tools which are more reliable and thrustworthy and
-also technically more robust when it comes to parse research data - irrespective
-from which tools these come or how you would like to used these data further
-throughout your journey of digitalizing your atom probe research.
-
-The Python parsers in this repository are meant as a motivation to offer
-immediate benefit to users. The collection of examples and technical discussions
-via issues serves the more long-term aim. This is to arrive at a detailed technical
-specification rather than more robust parsers only so that atom probe data can be
-exchanged across tools irrespective of their formatting.
-
-# Getting started as developer
-
+# Getting started
 You should create a virtual environment. We tested on Ubuntu with Python 3.8.
 Newer versions of Python should work similarly when using the desired version tag.
 
 If you don't have Python 3.8 installed on your computer, follow these commands:
 ```
 sudo add-apt-repository ppa:deadsnakes/ppa
 sudo apt install python3.8 python3-dev libpython3.8-dev python3.8-venv
 ```
 
-In some cases when using Python3.8 it was necessary to install python-numpy in others
-not. So consider this if you run into issues when continuing this manual.
+In some cases when using Python3.8, it was necessary to install python-numpy.
+Please consider this if you run into issues when continuing with this manual.
 The following steps will install the ifes_apt_tc_data_modeling module in the
 latest version.
 
 ```
 mkdir <your-brand-new-folder>
 cd <your-brand-new-folder>
 pip install virtualenv
 virtualenv --python=python3.8 .py38
 source .py38/bin/activate
 
 git clone git@github.com:atomprobe-tc/ifes_apt_tc_data_modeling.git
 cd ifes_apt_tc_data_modeling
 python -m pip install --upgrade pip
+python -m pip install pip-tools
 python -m pip install -e .
-python -m pip install -e ".[dev]"
 python -m pip list
 ```
 
-You can find instructions about how to use this tool in the tests/data jupyter notebook.
-This notebook can be started from the command line inside the ifes_apt_tc_data_modeling
-directory simply by calling.
+## Additional steps to do when working with jupyter notebooks
+By default the functionalities are offered as a library for Python programmers.
+For developers and users who would like to try using the library a convenient
+way is via jupyter notebooks. You can find instructions about how to use this tool
+in the tests/data jupyter notebook. This notebook can be started from the command
+line inside the ifes_apt_tc_data_modeling directory simply by calling.
+If you would like to use a jupyter notebook jupyter has to be installed as
+it will not be installed by default. To achieve this perform the following actions:
 
 ```
+python -m pip install -e ".[dev]"
+python -m pip list
+
 jupyter-lab
 ```
 
+## Documentation of file formats and data models in atom probe status quo
+Detailed technical specifications of the file formats and data models are not available for
+most formats in the field of atom probe microscopy. A practical solution to address this 
+limitation has been so far that scientists collect example files formatted in respective formats.
+
+These so-called instances were inspected and shared with colleagues. In summary, individual
+atom probers have contributed to formulate what can be considered likely candidates
+of specifications for several file formats via reverse engineering.
+This worked especially well for the POS and ePOS formats.
+
+Pieces of information about file formats were reported in the literature (e.g.
+the books by D. Larson et al. and B. Gault et al.). Atom probers like D. Haley have contributed
+substantially to make the community aware of existent limitations and these reverse engineering
+practices. AMETEK/Cameca is the key technology partner in atom probe. They have developed
+an open file format called APT which improves the accessibility of specific numerical data and
+some metadata. Individuals like M. Kühbach have driven the implementation and communication of
+parsers for this APT file format.
+
+Nowadays there is an increased interest and demand placed on atom probers by the funding agencies
+that researchers should or even have to make their research data management and data stewardship
+better matching and more completely aligned to the aims and practices of the F.A.I.R.
+principles of data stewardship. Therefore, it is useful to exchange more details about
+data models and file formats. Otherwise, it is not foreseeable how atom probe data can be made
+really interoperable with electronic lab notebooks, research data management
+systems (RDMS), and related software tools for data analyses.
+
+In light of these challenges, the idea of understanding formats just by examples, showed to be a
+slow and error-prone route as e.g. source code and workflows which have been useed to write such
+files, and the associated input, workflow, and provenance information has typically not been captured.
+Or the specific software tool(s) used might not have been shared or made accessible for review
+by the atom probe community.
+
+## Benefit and Next Steps
+You can easily imagine that the more people will support this work the more complete a public
+understanding and knowledge about the available file formats in atom probe microscopy will become.
+This can help all of us in the long run to build software tools which are more reliable, yield
+thrustworthy results and are technically more robust when it comes to parsing research data.
+Irrespective from which tools these data and metadata come or how one would like to used these data.
+
+The Python parsers in this repository are meant as a motivation to offer immediate benefit for users.
+The collection of examples and technical discussions via issues serves the more long-term aim.
+This is to arrive at a detailed technical specification rather than having more robust parsers only
+so that atom probe data can be exchanged across tools irrespective of their formatting.
 
 ## Support us with this work
 Thank you very much for supporting this activity and your time.
 
 ## Feedback, questions
 Feel free to drop us a message via creating an issue or commenting on one.
 Feel invited to use the resources in this repository.
 
 ## Where to place your examples?
 There is a *examples_with_provenance* and *examples_without_provenance*
 sub-directory for each file format.
 
 When you do know with which software and measured dataset you have created a file,
 you should share the file and these pieces of information (software version). Do so by
-naming at least the respective raw files. Ideally you share the examples via offering
+naming at least the respective raw files. Ideally, you share the examples via offering
 a link to an external data repository such as Zenodo or other providers. This not only
 avoids that this repository would get too much filled up with binary data.
 Also it enables you to share clearly under which license you would like make your
 example(s) accessible.
 
 ## Provenance if possible, plain examples if in doubt
 Use the *examples_with_provenance* sub-directory. With this it is at least possible
 to reproduce the file creation. A practical solution is to share (by uploading)
 the screenshot of the complete IVAS/APSuite version info screen, including
-the APSuite version, the CernRoot version, the CamecaRoot version, and the versions
+the APSuite version, the CERN Root version, the CamecaRoot version, and the versions
 of libraries used by APSuite. This can help other atom probers and AMETEK/Cameca
-to improve their software as it enables them to identify inconsistencies
-or bugs eventually easier.
+to improve their software as it will enable them to identify inconsistencies.
 
 Atom probers should be aware that file formats like POS, ePOS, or APT are neither
 raw data nor follow a clear technical documentation. Therefore, all current file
-formats are not meeting the FAIR principles.ey specified. Instead, refer to RRAW,
-STR, RHIT and/or HITS files. Ideally, you add unique identifiers (such as SHA256
-checksums) for each raw file. A documentation how you can do this was issued by 
-your IFES APT TC colleagues [(How to hash your data)](https://github.com/oxfordAPT/hashlist).
-
-If you cannot provide such detailed pieces of information to your work you can
-still participate and support us a lot if you share your knowledge by adding at
-least a link to a repository or file share with content in the relevant atom-probe
--specific file formats.
+formats are not meeting the FAIR principles. Instead, share RRAW, STR, RHIT, and HITS files.
+Ideally, you add unique identifiers (such as SHA256 checksums) for each file.
+A documentation how you can do this was issued by your IFES APT TC colleagues
+[(How to hash your data)](https://github.com/oxfordAPT/hashlist).
+
+If you cannot provide such detailed pieces of information, you can still participate
+and support us a lot if you share your knowledge by adding at least a link to a repository
+or file share with content in the relevant atom-probe-specific file formats.
+
 In this case, please use the *examples_without_provenance* directory.
 While these examples are stripped of the context in which they were created
 and used (provenance information), these examples can still be very useful
-to run the file formats parsers against to make the parsers more robust.
+to run the file formats parsers against to make the parsers more robust, i.e.
+that these can pick up formatting issues and act accordingly.
 
 # Background information
-File formats, data models, in (almost every) research field may not be 
-fully documented. A checklist of the necessary pieces of information and 
-documentation required to call a data model, data schema, and/or file format
-fully documented in accordance with the FAIR data and research software stewardship
-principles is given below:
+File formats, data models, in (almost every) research field may not be fully documented.
+A checklist of the necessary pieces of information and documentation required to call a
+data model, data schema, and/or file format fully documented in accordance with the
+FAIR data and research software stewardship principles is given below:
 
 1. Each piece of information (bit/byte) is documented.
 2. This documentation fulfills the FAIR principles, i.e.
    [Wilkinson et al., 2016](https://doi.org/10.1038/sdata.2016.18) and
    [Barker et al., 2022](https://doi.org/10.1038/s41597-022-01710-x)
    For binary files, tools like [kaitai struct](https://kaitai.io/) offer a
    solution to describe the exact binary information content in a data
    item. This can be a file but also the storage of a database entry or the
-   response of a call to an API.  Let alone the binary structure is insufficient,
-   tough.
+   response of a call to an API.
+   Let alone the binary structure is insufficient tough.
 3. To each piece of information there has to exist also a parameterized description,
    what this piece of information conceptually means. One way to arrive at such
    description is to use a data schema or ontology.
    It is important to mention that the concepts in this schema/ontology have
    unique identifier so that each data item/piece of information is identifiable
    as an instance of an entry in a database or a knowledge graph.
    This holds independently of which research data management system
    or electronic lab notebook is used.
-4. In addition, it is very useful that timestamps are associated with 
-   each data item (ISO8061 with time zone information) so that it is possible
-   to create a timeline of the context in which and when the e.g. file was created.
+4. In addition, it is very useful if timestamps are associated with each data item
+   (ISO8061 including time zone information) so that it is possible to create a
+   timeline of the context in which and when the e.g. file was created.
 
 The first and second point is known as a specification, while the third and fourth
 point emphasize that the contextualization and provenance is key to make a
 specification complete and useful.
```

### Comparing `ifes_apt_tc_data_modeling-0.0.8/README.md` & `ifes_apt_tc_data_modeling-0.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,167 +1,170 @@
 # atomprobe-data-modeling
 
 ## Mission:
 Foster exchange about data models and work towards specifications
 of file formats from the research field of atom probe microscopy.
 
-## Documentation of file formats and data models in atom probe status quo
-Detailed technical specifications of the file formats and data models are not
-available for all formats in the field of atom probe microscopy.
-A practical solution to address this limitation so far has been that scientists collect
-examples in respective formats, so-called instances, and inspect and share these.
-Based on this reverse engineering, individual atom probers have contributed to formulate
-what can be considered likely candidates of the specification for several file formats.
-This worked especially well for the POS and ePOS formats.
-
-Pieces of information about file formats are reported in the literature in e.g.
-books by D. Larson et al. and B. Gault et al. Atom probers like D. Haley have contributed
-substantially to make the community aware of existent limitations and these
-reverse engineering practices. AMETEK/Cameca is the key technology partner in atom probe.
-The company has created an open file format called APT which improves the accessibility of
-specific numerical data and some metadata. Individuals like M. Kühbach have driven the
-implementation and communication of parsers for this APT file format.
-
-Nowadays there is an increased interest and demand placed on atom probers by the funding
-agencies that researchers should and have to make their research data management and data
-stewardship better matching and more completely aligned to the aims and practices of
-F.A.I.R. research principles. Therefore, it is useful to exchange more details about
-data models and file formats as otherwise it is not foreseeable how atom probe data
-can be made really interoperable with electronic lab notebooks, research data management
-systems (RDMS), and related software tools.
-
-In light of these challenges, the idea of understanding formats just by examples,
-showed to be a slow and error-prone route as e.g. source code and workflows which have
-been useed to write such files, and the associated input, workflow, and provenance information
-might have been or not captured or/and the specific software tool(s) used might not have been
-shared or made accessible for reviewing and analyzing their functions.
-
-## Benefit and Next Steps
-You can easily imagine that the more people will support us with this work the
-more complete our understanding and knowledge about the available file formats
-in atom probe microscopy can and will become. This can help all of us in the
-long run to build software tools which are more reliable and thrustworthy and
-also technically more robust when it comes to parse research data - irrespective
-from which tools these come or how you would like to used these data further
-throughout your journey of digitalizing your atom probe research.
-
-The Python parsers in this repository are meant as a motivation to offer
-immediate benefit to users. The collection of examples and technical discussions
-via issues serves the more long-term aim. This is to arrive at a detailed technical
-specification rather than more robust parsers only so that atom probe data can be
-exchanged across tools irrespective of their formatting.
-
-# Getting started as developer
-
+# Getting started
 You should create a virtual environment. We tested on Ubuntu with Python 3.8.
 Newer versions of Python should work similarly when using the desired version tag.
 
 If you don't have Python 3.8 installed on your computer, follow these commands:
 ```
 sudo add-apt-repository ppa:deadsnakes/ppa
 sudo apt install python3.8 python3-dev libpython3.8-dev python3.8-venv
 ```
 
-In some cases when using Python3.8 it was necessary to install python-numpy in others
-not. So consider this if you run into issues when continuing this manual.
+In some cases when using Python3.8, it was necessary to install python-numpy.
+Please consider this if you run into issues when continuing with this manual.
 The following steps will install the ifes_apt_tc_data_modeling module in the
 latest version.
 
 ```
 mkdir <your-brand-new-folder>
 cd <your-brand-new-folder>
 pip install virtualenv
 virtualenv --python=python3.8 .py38
 source .py38/bin/activate
 
 git clone git@github.com:atomprobe-tc/ifes_apt_tc_data_modeling.git
 cd ifes_apt_tc_data_modeling
 python -m pip install --upgrade pip
+python -m pip install pip-tools
 python -m pip install -e .
-python -m pip install -e ".[dev]"
 python -m pip list
 ```
 
-You can find instructions about how to use this tool in the tests/data jupyter notebook.
-This notebook can be started from the command line inside the ifes_apt_tc_data_modeling
-directory simply by calling.
+## Additional steps to do when working with jupyter notebooks
+By default the functionalities are offered as a library for Python programmers.
+For developers and users who would like to try using the library a convenient
+way is via jupyter notebooks. You can find instructions about how to use this tool
+in the tests/data jupyter notebook. This notebook can be started from the command
+line inside the ifes_apt_tc_data_modeling directory simply by calling.
+If you would like to use a jupyter notebook jupyter has to be installed as
+it will not be installed by default. To achieve this perform the following actions:
 
 ```
+python -m pip install -e ".[dev]"
+python -m pip list
+
 jupyter-lab
 ```
 
+## Documentation of file formats and data models in atom probe status quo
+Detailed technical specifications of the file formats and data models are not available for
+most formats in the field of atom probe microscopy. A practical solution to address this 
+limitation has been so far that scientists collect example files formatted in respective formats.
+
+These so-called instances were inspected and shared with colleagues. In summary, individual
+atom probers have contributed to formulate what can be considered likely candidates
+of specifications for several file formats via reverse engineering.
+This worked especially well for the POS and ePOS formats.
+
+Pieces of information about file formats were reported in the literature (e.g.
+the books by D. Larson et al. and B. Gault et al.). Atom probers like D. Haley have contributed
+substantially to make the community aware of existent limitations and these reverse engineering
+practices. AMETEK/Cameca is the key technology partner in atom probe. They have developed
+an open file format called APT which improves the accessibility of specific numerical data and
+some metadata. Individuals like M. Kühbach have driven the implementation and communication of
+parsers for this APT file format.
+
+Nowadays there is an increased interest and demand placed on atom probers by the funding agencies
+that researchers should or even have to make their research data management and data stewardship
+better matching and more completely aligned to the aims and practices of the F.A.I.R.
+principles of data stewardship. Therefore, it is useful to exchange more details about
+data models and file formats. Otherwise, it is not foreseeable how atom probe data can be made
+really interoperable with electronic lab notebooks, research data management
+systems (RDMS), and related software tools for data analyses.
+
+In light of these challenges, the idea of understanding formats just by examples, showed to be a
+slow and error-prone route as e.g. source code and workflows which have been useed to write such
+files, and the associated input, workflow, and provenance information has typically not been captured.
+Or the specific software tool(s) used might not have been shared or made accessible for review
+by the atom probe community.
+
+## Benefit and Next Steps
+You can easily imagine that the more people will support this work the more complete a public
+understanding and knowledge about the available file formats in atom probe microscopy will become.
+This can help all of us in the long run to build software tools which are more reliable, yield
+thrustworthy results and are technically more robust when it comes to parsing research data.
+Irrespective from which tools these data and metadata come or how one would like to used these data.
+
+The Python parsers in this repository are meant as a motivation to offer immediate benefit for users.
+The collection of examples and technical discussions via issues serves the more long-term aim.
+This is to arrive at a detailed technical specification rather than having more robust parsers only
+so that atom probe data can be exchanged across tools irrespective of their formatting.
 
 ## Support us with this work
 Thank you very much for supporting this activity and your time.
 
 ## Feedback, questions
 Feel free to drop us a message via creating an issue or commenting on one.
 Feel invited to use the resources in this repository.
 
 ## Where to place your examples?
 There is a *examples_with_provenance* and *examples_without_provenance*
 sub-directory for each file format.
 
 When you do know with which software and measured dataset you have created a file,
 you should share the file and these pieces of information (software version). Do so by
-naming at least the respective raw files. Ideally you share the examples via offering
+naming at least the respective raw files. Ideally, you share the examples via offering
 a link to an external data repository such as Zenodo or other providers. This not only
 avoids that this repository would get too much filled up with binary data.
 Also it enables you to share clearly under which license you would like make your
 example(s) accessible.
 
 ## Provenance if possible, plain examples if in doubt
 Use the *examples_with_provenance* sub-directory. With this it is at least possible
 to reproduce the file creation. A practical solution is to share (by uploading)
 the screenshot of the complete IVAS/APSuite version info screen, including
-the APSuite version, the CernRoot version, the CamecaRoot version, and the versions
+the APSuite version, the CERN Root version, the CamecaRoot version, and the versions
 of libraries used by APSuite. This can help other atom probers and AMETEK/Cameca
-to improve their software as it enables them to identify inconsistencies
-or bugs eventually easier.
+to improve their software as it will enable them to identify inconsistencies.
 
 Atom probers should be aware that file formats like POS, ePOS, or APT are neither
 raw data nor follow a clear technical documentation. Therefore, all current file
-formats are not meeting the FAIR principles.ey specified. Instead, refer to RRAW,
-STR, RHIT and/or HITS files. Ideally, you add unique identifiers (such as SHA256
-checksums) for each raw file. A documentation how you can do this was issued by 
-your IFES APT TC colleagues [(How to hash your data)](https://github.com/oxfordAPT/hashlist).
-
-If you cannot provide such detailed pieces of information to your work you can
-still participate and support us a lot if you share your knowledge by adding at
-least a link to a repository or file share with content in the relevant atom-probe
--specific file formats.
+formats are not meeting the FAIR principles. Instead, share RRAW, STR, RHIT, and HITS files.
+Ideally, you add unique identifiers (such as SHA256 checksums) for each file.
+A documentation how you can do this was issued by your IFES APT TC colleagues
+[(How to hash your data)](https://github.com/oxfordAPT/hashlist).
+
+If you cannot provide such detailed pieces of information, you can still participate
+and support us a lot if you share your knowledge by adding at least a link to a repository
+or file share with content in the relevant atom-probe-specific file formats.
+
 In this case, please use the *examples_without_provenance* directory.
 While these examples are stripped of the context in which they were created
 and used (provenance information), these examples can still be very useful
-to run the file formats parsers against to make the parsers more robust.
+to run the file formats parsers against to make the parsers more robust, i.e.
+that these can pick up formatting issues and act accordingly.
 
 # Background information
-File formats, data models, in (almost every) research field may not be 
-fully documented. A checklist of the necessary pieces of information and 
-documentation required to call a data model, data schema, and/or file format
-fully documented in accordance with the FAIR data and research software stewardship
-principles is given below:
+File formats, data models, in (almost every) research field may not be fully documented.
+A checklist of the necessary pieces of information and documentation required to call a
+data model, data schema, and/or file format fully documented in accordance with the
+FAIR data and research software stewardship principles is given below:
 
 1. Each piece of information (bit/byte) is documented.
 2. This documentation fulfills the FAIR principles, i.e.
    [Wilkinson et al., 2016](https://doi.org/10.1038/sdata.2016.18) and
    [Barker et al., 2022](https://doi.org/10.1038/s41597-022-01710-x)
    For binary files, tools like [kaitai struct](https://kaitai.io/) offer a
    solution to describe the exact binary information content in a data
    item. This can be a file but also the storage of a database entry or the
-   response of a call to an API.  Let alone the binary structure is insufficient,
-   tough.
+   response of a call to an API.
+   Let alone the binary structure is insufficient tough.
 3. To each piece of information there has to exist also a parameterized description,
    what this piece of information conceptually means. One way to arrive at such
    description is to use a data schema or ontology.
    It is important to mention that the concepts in this schema/ontology have
    unique identifier so that each data item/piece of information is identifiable
    as an instance of an entry in a database or a knowledge graph.
    This holds independently of which research data management system
    or electronic lab notebook is used.
-4. In addition, it is very useful that timestamps are associated with 
-   each data item (ISO8061 with time zone information) so that it is possible
-   to create a timeline of the context in which and when the e.g. file was created.
+4. In addition, it is very useful if timestamps are associated with each data item
+   (ISO8061 including time zone information) so that it is possible to create a
+   timeline of the context in which and when the e.g. file was created.
 
 The first and second point is known as a specification, while the third and fourth
 point emphasize that the contextualization and provenance is key to make a
 specification complete and useful.
```

### Comparing `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/__init__.py` & `ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/apt/__init__.py` & `ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/apt/__init__.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/apt/apt6_headers.py` & `ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/apt/apt6_headers.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/apt/apt6_reader.py` & `ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/apt/apt6_reader.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/apt/apt6_sections.py` & `ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/apt/apt6_sections.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/apt/apt6_sections_branches.py` & `ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/apt/apt6_sections_branches.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/apt/apt6_utils.py` & `ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/apt/apt6_utils.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/epos/__init__.py` & `ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/epos/__init__.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/epos/epos_reader.py` & `ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/epos/epos_reader.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/fig/__init__.py` & `ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/fig/__init__.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/fig/fig_reader.py` & `ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/fig/fig_reader.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/nexus/__init__.py` & `ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/nexus/__init__.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/nexus/nx_field.py` & `ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/nexus/nx_field.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/nexus/nx_ion.py` & `ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/nexus/nx_ion.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/pos/__init__.py` & `ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/pos/__init__.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/pos/pos_reader.py` & `ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/pos/pos_reader.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/rng/__init__.py` & `ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/rng/__init__.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/rng/rng_reader.py` & `ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/rng/rng_reader.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/rrng/__init__.py` & `ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/rrng/__init__.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/rrng/rrng_reader.py` & `ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/rrng/rrng_reader.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/utils/__init__.py` & `ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/utils/definitions.py` & `ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/utils/mmapped_io.py` & `ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/utils/mmapped_io.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/utils/molecular_ions.py` & `ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/utils/molecular_ions.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/utils/nist_isotope_data.py` & `ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/utils/nist_isotope_data.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/utils/string_handling.py` & `ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/utils/string_handling.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling/utils/utils.py` & `ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling/utils/utils.py`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling.egg-info/PKG-INFO` & `ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifes-apt-tc-data-modeling
-Version: 0.0.8
+Version: 0.0.9
 Summary: Foster exchange about data models and work towards clear specifications of file formats and data models in the research field of atom probe microscopy.
 Author: The NOMAD Authors
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -218,168 +218,171 @@
 
 # atomprobe-data-modeling
 
 ## Mission:
 Foster exchange about data models and work towards specifications
 of file formats from the research field of atom probe microscopy.
 
-## Documentation of file formats and data models in atom probe status quo
-Detailed technical specifications of the file formats and data models are not
-available for all formats in the field of atom probe microscopy.
-A practical solution to address this limitation so far has been that scientists collect
-examples in respective formats, so-called instances, and inspect and share these.
-Based on this reverse engineering, individual atom probers have contributed to formulate
-what can be considered likely candidates of the specification for several file formats.
-This worked especially well for the POS and ePOS formats.
-
-Pieces of information about file formats are reported in the literature in e.g.
-books by D. Larson et al. and B. Gault et al. Atom probers like D. Haley have contributed
-substantially to make the community aware of existent limitations and these
-reverse engineering practices. AMETEK/Cameca is the key technology partner in atom probe.
-The company has created an open file format called APT which improves the accessibility of
-specific numerical data and some metadata. Individuals like M. Kühbach have driven the
-implementation and communication of parsers for this APT file format.
-
-Nowadays there is an increased interest and demand placed on atom probers by the funding
-agencies that researchers should and have to make their research data management and data
-stewardship better matching and more completely aligned to the aims and practices of
-F.A.I.R. research principles. Therefore, it is useful to exchange more details about
-data models and file formats as otherwise it is not foreseeable how atom probe data
-can be made really interoperable with electronic lab notebooks, research data management
-systems (RDMS), and related software tools.
-
-In light of these challenges, the idea of understanding formats just by examples,
-showed to be a slow and error-prone route as e.g. source code and workflows which have
-been useed to write such files, and the associated input, workflow, and provenance information
-might have been or not captured or/and the specific software tool(s) used might not have been
-shared or made accessible for reviewing and analyzing their functions.
-
-## Benefit and Next Steps
-You can easily imagine that the more people will support us with this work the
-more complete our understanding and knowledge about the available file formats
-in atom probe microscopy can and will become. This can help all of us in the
-long run to build software tools which are more reliable and thrustworthy and
-also technically more robust when it comes to parse research data - irrespective
-from which tools these come or how you would like to used these data further
-throughout your journey of digitalizing your atom probe research.
-
-The Python parsers in this repository are meant as a motivation to offer
-immediate benefit to users. The collection of examples and technical discussions
-via issues serves the more long-term aim. This is to arrive at a detailed technical
-specification rather than more robust parsers only so that atom probe data can be
-exchanged across tools irrespective of their formatting.
-
-# Getting started as developer
-
+# Getting started
 You should create a virtual environment. We tested on Ubuntu with Python 3.8.
 Newer versions of Python should work similarly when using the desired version tag.
 
 If you don't have Python 3.8 installed on your computer, follow these commands:
 ```
 sudo add-apt-repository ppa:deadsnakes/ppa
 sudo apt install python3.8 python3-dev libpython3.8-dev python3.8-venv
 ```
 
-In some cases when using Python3.8 it was necessary to install python-numpy in others
-not. So consider this if you run into issues when continuing this manual.
+In some cases when using Python3.8, it was necessary to install python-numpy.
+Please consider this if you run into issues when continuing with this manual.
 The following steps will install the ifes_apt_tc_data_modeling module in the
 latest version.
 
 ```
 mkdir <your-brand-new-folder>
 cd <your-brand-new-folder>
 pip install virtualenv
 virtualenv --python=python3.8 .py38
 source .py38/bin/activate
 
 git clone git@github.com:atomprobe-tc/ifes_apt_tc_data_modeling.git
 cd ifes_apt_tc_data_modeling
 python -m pip install --upgrade pip
+python -m pip install pip-tools
 python -m pip install -e .
-python -m pip install -e ".[dev]"
 python -m pip list
 ```
 
-You can find instructions about how to use this tool in the tests/data jupyter notebook.
-This notebook can be started from the command line inside the ifes_apt_tc_data_modeling
-directory simply by calling.
+## Additional steps to do when working with jupyter notebooks
+By default the functionalities are offered as a library for Python programmers.
+For developers and users who would like to try using the library a convenient
+way is via jupyter notebooks. You can find instructions about how to use this tool
+in the tests/data jupyter notebook. This notebook can be started from the command
+line inside the ifes_apt_tc_data_modeling directory simply by calling.
+If you would like to use a jupyter notebook jupyter has to be installed as
+it will not be installed by default. To achieve this perform the following actions:
 
 ```
+python -m pip install -e ".[dev]"
+python -m pip list
+
 jupyter-lab
 ```
 
+## Documentation of file formats and data models in atom probe status quo
+Detailed technical specifications of the file formats and data models are not available for
+most formats in the field of atom probe microscopy. A practical solution to address this 
+limitation has been so far that scientists collect example files formatted in respective formats.
+
+These so-called instances were inspected and shared with colleagues. In summary, individual
+atom probers have contributed to formulate what can be considered likely candidates
+of specifications for several file formats via reverse engineering.
+This worked especially well for the POS and ePOS formats.
+
+Pieces of information about file formats were reported in the literature (e.g.
+the books by D. Larson et al. and B. Gault et al.). Atom probers like D. Haley have contributed
+substantially to make the community aware of existent limitations and these reverse engineering
+practices. AMETEK/Cameca is the key technology partner in atom probe. They have developed
+an open file format called APT which improves the accessibility of specific numerical data and
+some metadata. Individuals like M. Kühbach have driven the implementation and communication of
+parsers for this APT file format.
+
+Nowadays there is an increased interest and demand placed on atom probers by the funding agencies
+that researchers should or even have to make their research data management and data stewardship
+better matching and more completely aligned to the aims and practices of the F.A.I.R.
+principles of data stewardship. Therefore, it is useful to exchange more details about
+data models and file formats. Otherwise, it is not foreseeable how atom probe data can be made
+really interoperable with electronic lab notebooks, research data management
+systems (RDMS), and related software tools for data analyses.
+
+In light of these challenges, the idea of understanding formats just by examples, showed to be a
+slow and error-prone route as e.g. source code and workflows which have been useed to write such
+files, and the associated input, workflow, and provenance information has typically not been captured.
+Or the specific software tool(s) used might not have been shared or made accessible for review
+by the atom probe community.
+
+## Benefit and Next Steps
+You can easily imagine that the more people will support this work the more complete a public
+understanding and knowledge about the available file formats in atom probe microscopy will become.
+This can help all of us in the long run to build software tools which are more reliable, yield
+thrustworthy results and are technically more robust when it comes to parsing research data.
+Irrespective from which tools these data and metadata come or how one would like to used these data.
+
+The Python parsers in this repository are meant as a motivation to offer immediate benefit for users.
+The collection of examples and technical discussions via issues serves the more long-term aim.
+This is to arrive at a detailed technical specification rather than having more robust parsers only
+so that atom probe data can be exchanged across tools irrespective of their formatting.
 
 ## Support us with this work
 Thank you very much for supporting this activity and your time.
 
 ## Feedback, questions
 Feel free to drop us a message via creating an issue or commenting on one.
 Feel invited to use the resources in this repository.
 
 ## Where to place your examples?
 There is a *examples_with_provenance* and *examples_without_provenance*
 sub-directory for each file format.
 
 When you do know with which software and measured dataset you have created a file,
 you should share the file and these pieces of information (software version). Do so by
-naming at least the respective raw files. Ideally you share the examples via offering
+naming at least the respective raw files. Ideally, you share the examples via offering
 a link to an external data repository such as Zenodo or other providers. This not only
 avoids that this repository would get too much filled up with binary data.
 Also it enables you to share clearly under which license you would like make your
 example(s) accessible.
 
 ## Provenance if possible, plain examples if in doubt
 Use the *examples_with_provenance* sub-directory. With this it is at least possible
 to reproduce the file creation. A practical solution is to share (by uploading)
 the screenshot of the complete IVAS/APSuite version info screen, including
-the APSuite version, the CernRoot version, the CamecaRoot version, and the versions
+the APSuite version, the CERN Root version, the CamecaRoot version, and the versions
 of libraries used by APSuite. This can help other atom probers and AMETEK/Cameca
-to improve their software as it enables them to identify inconsistencies
-or bugs eventually easier.
+to improve their software as it will enable them to identify inconsistencies.
 
 Atom probers should be aware that file formats like POS, ePOS, or APT are neither
 raw data nor follow a clear technical documentation. Therefore, all current file
-formats are not meeting the FAIR principles.ey specified. Instead, refer to RRAW,
-STR, RHIT and/or HITS files. Ideally, you add unique identifiers (such as SHA256
-checksums) for each raw file. A documentation how you can do this was issued by 
-your IFES APT TC colleagues [(How to hash your data)](https://github.com/oxfordAPT/hashlist).
-
-If you cannot provide such detailed pieces of information to your work you can
-still participate and support us a lot if you share your knowledge by adding at
-least a link to a repository or file share with content in the relevant atom-probe
--specific file formats.
+formats are not meeting the FAIR principles. Instead, share RRAW, STR, RHIT, and HITS files.
+Ideally, you add unique identifiers (such as SHA256 checksums) for each file.
+A documentation how you can do this was issued by your IFES APT TC colleagues
+[(How to hash your data)](https://github.com/oxfordAPT/hashlist).
+
+If you cannot provide such detailed pieces of information, you can still participate
+and support us a lot if you share your knowledge by adding at least a link to a repository
+or file share with content in the relevant atom-probe-specific file formats.
+
 In this case, please use the *examples_without_provenance* directory.
 While these examples are stripped of the context in which they were created
 and used (provenance information), these examples can still be very useful
-to run the file formats parsers against to make the parsers more robust.
+to run the file formats parsers against to make the parsers more robust, i.e.
+that these can pick up formatting issues and act accordingly.
 
 # Background information
-File formats, data models, in (almost every) research field may not be 
-fully documented. A checklist of the necessary pieces of information and 
-documentation required to call a data model, data schema, and/or file format
-fully documented in accordance with the FAIR data and research software stewardship
-principles is given below:
+File formats, data models, in (almost every) research field may not be fully documented.
+A checklist of the necessary pieces of information and documentation required to call a
+data model, data schema, and/or file format fully documented in accordance with the
+FAIR data and research software stewardship principles is given below:
 
 1. Each piece of information (bit/byte) is documented.
 2. This documentation fulfills the FAIR principles, i.e.
    [Wilkinson et al., 2016](https://doi.org/10.1038/sdata.2016.18) and
    [Barker et al., 2022](https://doi.org/10.1038/s41597-022-01710-x)
    For binary files, tools like [kaitai struct](https://kaitai.io/) offer a
    solution to describe the exact binary information content in a data
    item. This can be a file but also the storage of a database entry or the
-   response of a call to an API.  Let alone the binary structure is insufficient,
-   tough.
+   response of a call to an API.
+   Let alone the binary structure is insufficient tough.
 3. To each piece of information there has to exist also a parameterized description,
    what this piece of information conceptually means. One way to arrive at such
    description is to use a data schema or ontology.
    It is important to mention that the concepts in this schema/ontology have
    unique identifier so that each data item/piece of information is identifiable
    as an instance of an entry in a database or a knowledge graph.
    This holds independently of which research data management system
    or electronic lab notebook is used.
-4. In addition, it is very useful that timestamps are associated with 
-   each data item (ISO8061 with time zone information) so that it is possible
-   to create a timeline of the context in which and when the e.g. file was created.
+4. In addition, it is very useful if timestamps are associated with each data item
+   (ISO8061 including time zone information) so that it is possible to create a
+   timeline of the context in which and when the e.g. file was created.
 
 The first and second point is known as a specification, while the third and fourth
 point emphasize that the contextualization and provenance is key to make a
 specification complete and useful.
```

### Comparing `ifes_apt_tc_data_modeling-0.0.8/ifes_apt_tc_data_modeling.egg-info/SOURCES.txt` & `ifes_apt_tc_data_modeling-0.0.9/ifes_apt_tc_data_modeling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ifes_apt_tc_data_modeling-0.0.8/pyproject.toml` & `ifes_apt_tc_data_modeling-0.0.9/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ifes_apt_tc_data_modeling"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
     { name = "The NOMAD Authors" },
 ]
 description = "Foster exchange about data models and work towards clear specifications of file formats and data models in the research field of atom probe microscopy."
 readme = "README.md"
 license = { file = "LICENSE.txt" }
 requires-python = ">=3.8,<3.11"
@@ -19,20 +19,20 @@
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "h5py>=3.6.0",
     "numpy>=1.21.2",
     "pandas>=1.3.2",
-    "ase==3.19.0",
-    "radioactivedecay>=0.4.16",
-    "jupyterlab_h5web>=6.6.1",
-    "jupyterlab>=3.5.2,<3.6.0"
+    "ase>=3.19.0",
+    "radioactivedecay>=0.4.16"
 ]
 
 [project.optional-dependencies]
 dev = [
-    "twine",
+    "twine>=4.0.2",
+    "jupyterlab_h5web>=6.6.1",
+    "jupyterlab>=3.5.2,<3.6.0"
 ]
 
 # [tool.setuptools]
 # packages = ["apt", "epos", "nexus", "pos", "rng", "rrng", "fig", "utils"]
```

