# Comparing `tmp/ringity-0.3a2.tar.gz` & `tmp/ringity-0.3a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ringity-0.3a2.tar", last modified: Fri Feb 24 10:06:17 2023, max compression
+gzip compressed data, was "ringity-0.3a3.tar", last modified: Tue Jul 11 21:12:26 2023, max compression
```

## Comparing `ringity-0.3a2.tar` & `ringity-0.3a3.tar`

### file list

```diff
@@ -1,62 +1,75 @@
-drwxr-xr-x   0 markusyoussef   (501) staff       (20)        0 2023-02-24 10:06:17.459186 ringity-0.3a2/
--rw-r--r--   0 markusyoussef   (501) staff       (20)     1074 2022-09-14 13:31:49.000000 ringity-0.3a2/LICENSE.txt
--rw-r--r--   0 markusyoussef   (501) staff       (20)     3243 2023-02-24 10:06:17.460412 ringity-0.3a2/PKG-INFO
--rw-r--r--   0 markusyoussef   (501) staff       (20)     2624 2022-09-14 13:31:49.000000 ringity-0.3a2/README.rst
--rw-r--r--   0 markusyoussef   (501) staff       (20)      164 2023-01-21 23:44:19.000000 ringity-0.3a2/pyproject.toml
-drwxr-xr-x   0 markusyoussef   (501) staff       (20)        0 2023-02-24 10:06:17.369484 ringity-0.3a2/ringity/
--rw-r--r--   0 markusyoussef   (501) staff       (20)     1631 2023-02-24 09:59:35.000000 ringity-0.3a2/ringity/__init__.py
-drwxr-xr-x   0 markusyoussef   (501) staff       (20)        0 2023-02-24 10:06:17.379465 ringity-0.3a2/ringity/_legacy/
--rw-r--r--   0 markusyoussef   (501) staff       (20)      200 2023-01-21 23:44:19.000000 ringity-0.3a2/ringity/_legacy/__init__.py
--rw-r--r--   0 markusyoussef   (501) staff       (20)    13801 2023-01-21 23:44:19.000000 ringity-0.3a2/ringity/_legacy/legacy_network_model.py
-drwxr-xr-x   0 markusyoussef   (501) staff       (20)        0 2023-02-24 10:06:17.394317 ringity-0.3a2/ringity/classes/
--rw-r--r--   0 markusyoussef   (501) staff       (20)        0 2022-09-14 13:31:49.000000 ringity-0.3a2/ringity/classes/__init__.py
--rw-r--r--   0 markusyoussef   (501) staff       (20)    17647 2022-09-14 13:31:49.000000 ringity-0.3a2/ringity/classes/_distns.py
--rw-r--r--   0 markusyoussef   (501) staff       (20)     1547 2022-09-14 13:31:49.000000 ringity-0.3a2/ringity/classes/exceptions.py
--rw-r--r--   0 markusyoussef   (501) staff       (20)      553 2022-09-14 13:31:49.000000 ringity-0.3a2/ringity/classes/legacy.py
--rw-r--r--   0 markusyoussef   (501) staff       (20)     6113 2023-01-21 23:44:19.000000 ringity-0.3a2/ringity/classes/modelparameterbuilder.py
--rw-r--r--   0 markusyoussef   (501) staff       (20)    11906 2023-01-21 23:44:19.000000 ringity-0.3a2/ringity/classes/networkbuilder.py
--rw-r--r--   0 markusyoussef   (501) staff       (20)    12335 2023-01-21 23:44:19.000000 ringity-0.3a2/ringity/classes/pdiagram.py
-drwxr-xr-x   0 markusyoussef   (501) staff       (20)        0 2023-02-24 10:06:17.408446 ringity-0.3a2/ringity/core/
--rw-r--r--   0 markusyoussef   (501) staff       (20)      928 2023-01-21 23:44:19.000000 ringity-0.3a2/ringity/core/__init__.py
--rw-r--r--   0 markusyoussef   (501) staff       (20)     7232 2023-01-21 23:44:19.000000 ringity-0.3a2/ringity/core/data2metric.py
--rw-r--r--   0 markusyoussef   (501) staff       (20)     4992 2023-01-21 23:44:19.000000 ringity-0.3a2/ringity/core/metric2ringscore.py
--rw-r--r--   0 markusyoussef   (501) staff       (20)     1502 2023-01-21 23:44:19.000000 ringity-0.3a2/ringity/core/phomology.py
--rw-r--r--   0 markusyoussef   (501) staff       (20)    11214 2023-01-21 23:44:19.000000 ringity-0.3a2/ringity/core/pipeline.py
--rw-r--r--   0 markusyoussef   (501) staff       (20)      440 2023-01-21 23:44:19.000000 ringity-0.3a2/ringity/core/statistics.py
-drwxr-xr-x   0 markusyoussef   (501) staff       (20)        0 2023-02-24 10:06:17.420834 ringity-0.3a2/ringity/generators/
--rw-r--r--   0 markusyoussef   (501) staff       (20)      435 2023-02-22 17:00:35.000000 ringity-0.3a2/ringity/generators/__init__.py
--rw-r--r--   0 markusyoussef   (501) staff       (20)     9261 2023-02-22 17:00:35.000000 ringity-0.3a2/ringity/generators/geometric_networks.py
--rw-r--r--   0 markusyoussef   (501) staff       (20)     2491 2023-01-21 23:44:19.000000 ringity-0.3a2/ringity/generators/network_models.py
--rw-r--r--   0 markusyoussef   (501) staff       (20)      445 2023-01-21 23:44:19.000000 ringity-0.3a2/ringity/generators/pdiagrams.py
--rw-r--r--   0 markusyoussef   (501) staff       (20)     4823 2023-01-24 10:14:42.000000 ringity-0.3a2/ringity/generators/point_clouds.py
-drwxr-xr-x   0 markusyoussef   (501) staff       (20)        0 2023-02-24 10:06:17.431289 ringity-0.3a2/ringity/generators/utils/
--rw-r--r--   0 markusyoussef   (501) staff       (20)        0 2023-01-21 23:44:19.000000 ringity-0.3a2/ringity/generators/utils/__init__.py
--rw-r--r--   0 markusyoussef   (501) staff       (20)      105 2023-01-21 23:44:19.000000 ringity-0.3a2/ringity/generators/utils/defaults.py
--rw-r--r--   0 markusyoussef   (501) staff       (20)    14290 2023-01-21 23:44:19.000000 ringity-0.3a2/ringity/generators/utils/distribution_functions.py
--rw-r--r--   0 markusyoussef   (501) staff       (20)     9488 2023-01-21 23:44:19.000000 ringity-0.3a2/ringity/generators/utils/param_utils.py
--rw-r--r--   0 markusyoussef   (501) staff       (20)     3879 2023-01-21 23:44:19.000000 ringity-0.3a2/ringity/generators/utils/transformations.py
-drwxr-xr-x   0 markusyoussef   (501) staff       (20)        0 2023-02-24 10:06:17.435522 ringity-0.3a2/ringity/networkmeasures/
--rw-r--r--   0 markusyoussef   (501) staff       (20)        0 2023-01-21 23:44:19.000000 ringity-0.3a2/ringity/networkmeasures/__init__.py
--rw-r--r--   0 markusyoussef   (501) staff       (20)     7777 2023-01-21 23:44:19.000000 ringity-0.3a2/ringity/networkmeasures/centralities.py
--rw-r--r--   0 markusyoussef   (501) staff       (20)     1423 2023-01-21 23:44:19.000000 ringity-0.3a2/ringity/networkmeasures/graphlet_coefficients.py
-drwxr-xr-x   0 markusyoussef   (501) staff       (20)        0 2023-02-24 10:06:17.447810 ringity-0.3a2/ringity/plotting/
--rw-r--r--   0 markusyoussef   (501) staff       (20)      411 2023-01-21 23:44:19.000000 ringity-0.3a2/ringity/plotting/__init__.py
--rw-r--r--   0 markusyoussef   (501) staff       (20)     4584 2023-01-21 23:44:19.000000 ringity-0.3a2/ringity/plotting/_plotly.py
--rw-r--r--   0 markusyoussef   (501) staff       (20)     3928 2023-01-21 23:44:19.000000 ringity-0.3a2/ringity/plotting/animation.py
--rw-r--r--   0 markusyoussef   (501) staff       (20)     6835 2023-02-22 17:36:32.000000 ringity-0.3a2/ringity/plotting/plot_functions.py
--rw-r--r--   0 markusyoussef   (501) staff       (20)     1512 2023-01-21 23:44:19.000000 ringity-0.3a2/ringity/plotting/singlecell.py
--rw-r--r--   0 markusyoussef   (501) staff       (20)      832 2023-01-21 23:44:19.000000 ringity-0.3a2/ringity/plotting/styling.py
-drwxr-xr-x   0 markusyoussef   (501) staff       (20)        0 2023-02-24 10:06:17.450745 ringity-0.3a2/ringity/readwrite/
--rw-r--r--   0 markusyoussef   (501) staff       (20)        0 2022-09-14 13:31:49.000000 ringity-0.3a2/ringity/readwrite/__init__.py
--rw-r--r--   0 markusyoussef   (501) staff       (20)     2064 2023-01-31 22:30:52.000000 ringity-0.3a2/ringity/readwrite/pdiagrams.py
-drwxr-xr-x   0 markusyoussef   (501) staff       (20)        0 2023-02-24 10:06:17.456787 ringity-0.3a2/ringity/singlecell/
--rw-r--r--   0 markusyoussef   (501) staff       (20)      151 2023-02-06 22:32:59.000000 ringity-0.3a2/ringity/singlecell/__init__.py
--rw-r--r--   0 markusyoussef   (501) staff       (20)     1495 2023-01-21 23:44:19.000000 ringity-0.3a2/ringity/singlecell/genesets.py
--rw-r--r--   0 markusyoussef   (501) staff       (20)     4839 2023-02-06 22:39:27.000000 ringity-0.3a2/ringity/singlecell/singlecell.py
-drwxr-xr-x   0 markusyoussef   (501) staff       (20)        0 2023-02-24 10:06:17.374552 ringity-0.3a2/ringity.egg-info/
--rw-r--r--   0 markusyoussef   (501) staff       (20)     3243 2023-02-24 10:06:17.000000 ringity-0.3a2/ringity.egg-info/PKG-INFO
--rw-r--r--   0 markusyoussef   (501) staff       (20)     1514 2023-02-24 10:06:17.000000 ringity-0.3a2/ringity.egg-info/SOURCES.txt
--rw-r--r--   0 markusyoussef   (501) staff       (20)        1 2023-02-24 10:06:17.000000 ringity-0.3a2/ringity.egg-info/dependency_links.txt
--rw-r--r--   0 markusyoussef   (501) staff       (20)       38 2023-02-24 10:06:17.000000 ringity-0.3a2/ringity.egg-info/requires.txt
--rw-r--r--   0 markusyoussef   (501) staff       (20)        8 2023-02-24 10:06:17.000000 ringity-0.3a2/ringity.egg-info/top_level.txt
--rw-r--r--   0 markusyoussef   (501) staff       (20)      834 2023-02-24 10:06:17.462803 ringity-0.3a2/setup.cfg
+drwxr-xr-x   0 markusyoussef   (501) staff       (20)        0 2023-07-11 21:12:26.003778 ringity-0.3a3/
+-rw-r--r--   0 markusyoussef   (501) staff       (20)     1074 2022-09-14 13:31:49.000000 ringity-0.3a3/LICENSE.txt
+-rw-r--r--   0 markusyoussef   (501) staff       (20)     3243 2023-07-11 21:12:26.003845 ringity-0.3a3/PKG-INFO
+-rw-r--r--   0 markusyoussef   (501) staff       (20)     2624 2023-05-02 14:02:01.000000 ringity-0.3a3/README.rst
+-rw-r--r--   0 markusyoussef   (501) staff       (20)      196 2023-05-02 14:11:25.000000 ringity-0.3a3/pyproject.toml
+drwxr-xr-x   0 markusyoussef   (501) staff       (20)        0 2023-07-11 21:12:25.991781 ringity-0.3a3/ringity/
+-rw-r--r--   0 markusyoussef   (501) staff       (20)     1565 2023-07-11 21:06:51.000000 ringity-0.3a3/ringity/__init__.py
+drwxr-xr-x   0 markusyoussef   (501) staff       (20)        0 2023-07-11 21:12:25.993069 ringity-0.3a3/ringity/_legacy/
+-rw-r--r--   0 markusyoussef   (501) staff       (20)      200 2023-05-02 14:02:01.000000 ringity-0.3a3/ringity/_legacy/__init__.py
+-rw-r--r--   0 markusyoussef   (501) staff       (20)    13801 2023-05-02 14:02:01.000000 ringity-0.3a3/ringity/_legacy/legacy_network_model.py
+drwxr-xr-x   0 markusyoussef   (501) staff       (20)        0 2023-07-11 21:12:25.994586 ringity-0.3a3/ringity/classes/
+-rw-r--r--   0 markusyoussef   (501) staff       (20)        0 2023-05-02 12:55:33.000000 ringity-0.3a3/ringity/classes/__init__.py
+-rw-r--r--   0 markusyoussef   (501) staff       (20)    17647 2023-05-02 14:02:01.000000 ringity-0.3a3/ringity/classes/_distns.py
+-rw-r--r--   0 markusyoussef   (501) staff       (20)     1547 2023-05-02 14:02:01.000000 ringity-0.3a3/ringity/classes/exceptions.py
+-rw-r--r--   0 markusyoussef   (501) staff       (20)      553 2023-05-02 14:02:01.000000 ringity-0.3a3/ringity/classes/legacy.py
+-rw-r--r--   0 markusyoussef   (501) staff       (20)     6113 2023-05-02 14:02:01.000000 ringity-0.3a3/ringity/classes/modelparameterbuilder.py
+-rw-r--r--   0 markusyoussef   (501) staff       (20)    11906 2023-05-02 14:02:01.000000 ringity-0.3a3/ringity/classes/networkbuilder.py
+-rw-r--r--   0 markusyoussef   (501) staff       (20)    12640 2023-05-08 20:57:13.000000 ringity-0.3a3/ringity/classes/pdiagram.py
+drwxr-xr-x   0 markusyoussef   (501) staff       (20)        0 2023-07-11 21:12:25.995805 ringity-0.3a3/ringity/generators/
+-rw-r--r--   0 markusyoussef   (501) staff       (20)      374 2023-06-16 15:24:39.000000 ringity-0.3a3/ringity/generators/__init__.py
+-rw-r--r--   0 markusyoussef   (501) staff       (20)     9261 2023-05-02 14:11:25.000000 ringity-0.3a3/ringity/generators/geometric_networks.py
+-rw-r--r--   0 markusyoussef   (501) staff       (20)      445 2023-05-02 14:02:01.000000 ringity-0.3a3/ringity/generators/pdiagrams.py
+-rw-r--r--   0 markusyoussef   (501) staff       (20)     4823 2023-05-02 14:02:01.000000 ringity-0.3a3/ringity/generators/point_clouds.py
+drwxr-xr-x   0 markusyoussef   (501) staff       (20)        0 2023-07-11 21:12:25.996599 ringity-0.3a3/ringity/generators/utils/
+-rw-r--r--   0 markusyoussef   (501) staff       (20)        0 2023-05-02 14:02:01.000000 ringity-0.3a3/ringity/generators/utils/__init__.py
+-rw-r--r--   0 markusyoussef   (501) staff       (20)      105 2023-05-02 14:02:01.000000 ringity-0.3a3/ringity/generators/utils/defaults.py
+-rw-r--r--   0 markusyoussef   (501) staff       (20)    14290 2023-05-02 14:02:01.000000 ringity-0.3a3/ringity/generators/utils/distribution_functions.py
+-rw-r--r--   0 markusyoussef   (501) staff       (20)     9488 2023-05-02 14:02:01.000000 ringity-0.3a3/ringity/generators/utils/param_utils.py
+-rw-r--r--   0 markusyoussef   (501) staff       (20)     3879 2023-05-02 14:02:01.000000 ringity-0.3a3/ringity/generators/utils/transformations.py
+drwxr-xr-x   0 markusyoussef   (501) staff       (20)        0 2023-07-11 21:12:25.997192 ringity-0.3a3/ringity/networkmeasures/
+-rw-r--r--   0 markusyoussef   (501) staff       (20)        0 2023-05-02 14:02:01.000000 ringity-0.3a3/ringity/networkmeasures/__init__.py
+-rw-r--r--   0 markusyoussef   (501) staff       (20)     7817 2023-06-16 15:34:00.000000 ringity-0.3a3/ringity/networkmeasures/centralities.py
+-rw-r--r--   0 markusyoussef   (501) staff       (20)     1423 2023-05-02 14:02:01.000000 ringity-0.3a3/ringity/networkmeasures/graphlet_coefficients.py
+drwxr-xr-x   0 markusyoussef   (501) staff       (20)        0 2023-07-11 21:12:25.999123 ringity-0.3a3/ringity/networkmodel/
+-rw-r--r--   0 markusyoussef   (501) staff       (20)     2492 2023-06-16 15:23:52.000000 ringity-0.3a3/ringity/networkmodel/__init__.py
+-rw-r--r--   0 markusyoussef   (501) staff       (20)    17898 2023-06-24 13:45:38.000000 ringity-0.3a3/ringity/networkmodel/distributions.py
+-rw-r--r--   0 markusyoussef   (501) staff       (20)     6109 2023-05-02 14:11:25.000000 ringity-0.3a3/ringity/networkmodel/modelparameterbuilder.py
+-rw-r--r--   0 markusyoussef   (501) staff       (20)    11753 2023-06-24 13:52:21.000000 ringity-0.3a3/ringity/networkmodel/networkbuilder.py
+-rw-r--r--   0 markusyoussef   (501) staff       (20)     9655 2023-06-17 04:15:50.000000 ringity-0.3a3/ringity/networkmodel/param_utils.py
+-rw-r--r--   0 markusyoussef   (501) staff       (20)     4026 2023-06-17 12:51:31.000000 ringity-0.3a3/ringity/networkmodel/transformations.py
+drwxr-xr-x   0 markusyoussef   (501) staff       (20)        0 2023-07-11 21:12:26.000339 ringity-0.3a3/ringity/plotting/
+-rw-r--r--   0 markusyoussef   (501) staff       (20)      411 2023-05-02 14:02:01.000000 ringity-0.3a3/ringity/plotting/__init__.py
+-rw-r--r--   0 markusyoussef   (501) staff       (20)     4584 2023-05-02 14:02:01.000000 ringity-0.3a3/ringity/plotting/_plotly.py
+-rw-r--r--   0 markusyoussef   (501) staff       (20)     3928 2023-05-02 14:02:01.000000 ringity-0.3a3/ringity/plotting/animation.py
+-rw-r--r--   0 markusyoussef   (501) staff       (20)     6835 2023-05-02 14:11:25.000000 ringity-0.3a3/ringity/plotting/plot_functions.py
+-rw-r--r--   0 markusyoussef   (501) staff       (20)     1512 2023-05-02 14:02:01.000000 ringity-0.3a3/ringity/plotting/singlecell.py
+-rw-r--r--   0 markusyoussef   (501) staff       (20)      832 2023-05-02 14:02:01.000000 ringity-0.3a3/ringity/plotting/styling.py
+drwxr-xr-x   0 markusyoussef   (501) staff       (20)        0 2023-07-11 21:12:26.000615 ringity-0.3a3/ringity/readwrite/
+-rw-r--r--   0 markusyoussef   (501) staff       (20)        0 2023-05-02 14:02:01.000000 ringity-0.3a3/ringity/readwrite/__init__.py
+-rw-r--r--   0 markusyoussef   (501) staff       (20)     2064 2023-05-02 14:11:25.000000 ringity-0.3a3/ringity/readwrite/pdiagrams.py
+drwxr-xr-x   0 markusyoussef   (501) staff       (20)        0 2023-07-11 21:12:26.001932 ringity-0.3a3/ringity/ringscore/
+-rw-r--r--   0 markusyoussef   (501) staff       (20)      948 2023-06-16 15:31:26.000000 ringity-0.3a3/ringity/ringscore/__init__.py
+-rw-r--r--   0 markusyoussef   (501) staff       (20)     7232 2023-05-02 14:02:01.000000 ringity-0.3a3/ringity/ringscore/data2metric.py
+-rw-r--r--   0 markusyoussef   (501) staff       (20)     4992 2023-05-02 14:02:01.000000 ringity-0.3a3/ringity/ringscore/metric2ringscore.py
+-rw-r--r--   0 markusyoussef   (501) staff       (20)     1502 2023-05-02 14:02:01.000000 ringity-0.3a3/ringity/ringscore/phomology.py
+-rw-r--r--   0 markusyoussef   (501) staff       (20)    11706 2023-06-16 15:31:40.000000 ringity-0.3a3/ringity/ringscore/pipeline.py
+-rw-r--r--   0 markusyoussef   (501) staff       (20)     1481 2023-07-07 11:38:21.000000 ringity-0.3a3/ringity/ringscore/statistics.py
+drwxr-xr-x   0 markusyoussef   (501) staff       (20)        0 2023-07-11 21:12:26.002503 ringity-0.3a3/ringity/singlecell/
+-rw-r--r--   0 markusyoussef   (501) staff       (20)      151 2023-05-02 14:02:01.000000 ringity-0.3a3/ringity/singlecell/__init__.py
+-rw-r--r--   0 markusyoussef   (501) staff       (20)     1495 2023-05-02 14:02:01.000000 ringity-0.3a3/ringity/singlecell/genesets.py
+-rw-r--r--   0 markusyoussef   (501) staff       (20)     4839 2023-05-02 14:11:25.000000 ringity-0.3a3/ringity/singlecell/singlecell.py
+drwxr-xr-x   0 markusyoussef   (501) staff       (20)        0 2023-07-11 21:12:26.003444 ringity-0.3a3/ringity/userclasses/
+-rw-r--r--   0 markusyoussef   (501) staff       (20)        0 2023-05-02 14:11:25.000000 ringity-0.3a3/ringity/userclasses/__init__.py
+-rw-r--r--   0 markusyoussef   (501) staff       (20)    17651 2023-05-02 14:11:25.000000 ringity-0.3a3/ringity/userclasses/_distns.py
+-rw-r--r--   0 markusyoussef   (501) staff       (20)     1547 2023-05-02 14:11:25.000000 ringity-0.3a3/ringity/userclasses/exceptions.py
+-rw-r--r--   0 markusyoussef   (501) staff       (20)     2332 2023-05-02 14:11:25.000000 ringity-0.3a3/ringity/userclasses/formulas.py
+-rw-r--r--   0 markusyoussef   (501) staff       (20)      553 2023-05-02 14:11:25.000000 ringity-0.3a3/ringity/userclasses/legacy.py
+-rw-r--r--   0 markusyoussef   (501) staff       (20)    12473 2023-06-16 15:32:07.000000 ringity-0.3a3/ringity/userclasses/pdiagram.py
+drwxr-xr-x   0 markusyoussef   (501) staff       (20)        0 2023-07-11 21:12:25.992510 ringity-0.3a3/ringity.egg-info/
+-rw-r--r--   0 markusyoussef   (501) staff       (20)     3243 2023-07-11 21:12:25.000000 ringity-0.3a3/ringity.egg-info/PKG-INFO
+-rw-r--r--   0 markusyoussef   (501) staff       (20)     1930 2023-07-11 21:12:25.000000 ringity-0.3a3/ringity.egg-info/SOURCES.txt
+-rw-r--r--   0 markusyoussef   (501) staff       (20)        1 2023-07-11 21:12:25.000000 ringity-0.3a3/ringity.egg-info/dependency_links.txt
+-rw-r--r--   0 markusyoussef   (501) staff       (20)       56 2023-07-11 21:12:25.000000 ringity-0.3a3/ringity.egg-info/requires.txt
+-rw-r--r--   0 markusyoussef   (501) staff       (20)        8 2023-07-11 21:12:25.000000 ringity-0.3a3/ringity.egg-info/top_level.txt
+-rw-r--r--   0 markusyoussef   (501) staff       (20)      854 2023-07-11 21:12:26.004208 ringity-0.3a3/setup.cfg
```

### Comparing `ringity-0.3a2/LICENSE.txt` & `ringity-0.3a3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ringity-0.3a2/PKG-INFO` & `ringity-0.3a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ringity
-Version: 0.3a2
+Version: 0.3a3
 Summary: ringity package
 Home-page: https://github.com/ClusterDuck123/ringity
 Author: Markus K. Youssef
 Author-email: mk.youssef@hotmail.com
 Project-URL: Bug Tracker, https://github.com/kiri93/ringity/issues
 Project-URL: Lab Origin, https://menchelab.com
 Keywords: network ring circular tda
```

### Comparing `ringity-0.3a2/README.rst` & `ringity-0.3a3/README.rst`

 * *Files identical despite different names*

### Comparing `ringity-0.3a2/ringity/__init__.py` & `ringity-0.3a3/ringity/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 name = "ringity"
 __author__ = "M. K. Youssef, et al."
-__version__ = "0.3a2"
+__version__ = "0.3a3"
 
 # FUNCTIONS
-from ringity.core import (
+from ringity.ringscore import (
                     pdiagram, 
                     pdiagram_from_network,
                     pdiagram_from_point_cloud,
                     pdiagram_from_distance_matrix,
                     
                     ring_score,
                     ring_score_from_network,
@@ -20,20 +20,17 @@
                     pwdistance,
                     pwdistance_from_network,
                     pwdistance_from_point_cloud,
                     pwdistance_from_adjacency_matrix
                     )
 
 # MODULES
-from ringity.core import (statistics)
+from ringity.ringscore import (statistics)
 
-from ringity.generators import (
-                    random_pdgm,
-                    network_model,
-                    )
+from ringity.networkmodel import network_model
 import ringity.generators.geometric_networks as geometric_networks
 
 from ringity.plotting import (
                         plot,
                         plot_X,
                         plot_nx,
                         plot_dgm,
```

### Comparing `ringity-0.3a2/ringity/_legacy/legacy_network_model.py` & `ringity-0.3a3/ringity/_legacy/legacy_network_model.py`

 * *Files identical despite different names*

### Comparing `ringity-0.3a2/ringity/classes/_distns.py` & `ringity-0.3a3/ringity/classes/_distns.py`

 * *Files identical despite different names*

### Comparing `ringity-0.3a2/ringity/classes/exceptions.py` & `ringity-0.3a3/ringity/classes/exceptions.py`

 * *Files identical despite different names*

### Comparing `ringity-0.3a2/ringity/classes/legacy.py` & `ringity-0.3a3/ringity/classes/legacy.py`

 * *Files identical despite different names*

### Comparing `ringity-0.3a2/ringity/classes/modelparameterbuilder.py` & `ringity-0.3a3/ringity/classes/modelparameterbuilder.py`

 * *Files identical despite different names*

### Comparing `ringity-0.3a2/ringity/classes/networkbuilder.py` & `ringity-0.3a3/ringity/classes/networkbuilder.py`

 * *Files identical despite different names*

### Comparing `ringity-0.3a2/ringity/classes/pdiagram.py` & `ringity-0.3a3/ringity/userclasses/pdiagram.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import warnings
 import numpy as np
 import ringity as rng
 
 from itertools import compress
 from collections.abc import MutableMapping
-from ringity.core.metric2ringscore import ring_score_from_sequence
-from ringity.classes.exceptions import (
+from ringity.ringscore.metric2ringscore import ring_score_from_sequence
+from ringity.userclasses.exceptions import (
                                     SchroedingersException,
                                     TimeParadoxError,
                                     EndOfTimeError,
                                     SettingPersistenceError)
 
 # =============================================================================
 #  ------------------------------- DgmPt CLASS -------------------------------
@@ -162,14 +162,16 @@
     @property
     def deaths(self):
         births, deaths = zip(*self)
         return np.array(deaths)
 
     @property
     def plengths(self):
+        if len(self) == 0:
+            return np.array([])
         return self.deaths - self.births
 
     @property
     def pratios(self):
         return self.deaths / self.births
 
     @property
@@ -198,34 +200,36 @@
     def score(self):
         warnings.warn("The property `score` is depricated! "
                       "Please use the method `ring_score` instead.",
                       DeprecationWarning, stacklevel = 2)
         return self.ring_score()
 
 # -------------------------------- Methods ---------------------------------
-    def psequence(self, normalisation = 'diameter'):
+    def psequence(self, normalisation = 'signal'):
         """Return 1-dimensional transformation of persistence diagram.
 
         Parameters
         ----------
         normalisation : str, optional
-            Acceptable normalisation: `diameter`, `signal`. By default 'diameter'.
+            Acceptable normalisation: `diameter`, `signal`. By default 'signal'.
 
         Returns
         -------
         np.array
             Persistence sequence.
 
         Raises
         ------
         ValueError
             If `normalisation` is not known.
         """        
         pseq = self.plengths
 
+        if len(pseq) == 0:
+            return pseq
         if normalisation is None:
             return pseq
         elif normalisation.lower() == 'diameter':
             return pseq/self.diameter
         elif normalisation.lower() == 'signal':
             return pseq/self.signal
         else:
@@ -236,15 +240,15 @@
         return other
     
     def append(self, item):
         list.append(self, PDiagramPoint(item))
         self.sort(reverse=True)
 
     def trimmed(self, length = None):
-        if length is None:
+        if length is None or length == np.inf:
             return self[self > 0]
 
         if length <= len(self):
             return self[:length]
 
         else:
             other = self.copy()
@@ -259,15 +263,15 @@
         return np.array(self)
 
 # ---------------------------- Function calls -----------------------------
     def ring_score(self, 
                 flavour = 'geometric', 
                 nb_pers = None, 
                 exponent = 2):
-        return ring_score_from_sequence(self.sequence,
+        return ring_score_from_sequence(self.psequence(),
                                         flavour = flavour,
                                         nb_pers = nb_pers,
                                         exponent = exponent)
 
     def plot(self, 
             ax = None, 
             return_artist_obj = False,
```

### Comparing `ringity-0.3a2/ringity/core/__init__.py` & `ringity-0.3a3/ringity/ringscore/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #FUNCTIONS
-from ringity.core.pipeline import (
+from ringity.ringscore.pipeline import (
                     pdiagram, 
                     pdiagram_from_network,
                     pdiagram_from_point_cloud,
                     pdiagram_from_distance_matrix,
                     
                     ring_score,
                     ring_score_from_network,
                     ring_score_from_point_cloud,
                     ring_score_from_distance_matrix,
 
                     ring_score_from_pdiagram
                     )
-from ringity.core.metric2ringscore import ring_score_from_sequence
-from ringity.core.data2metric import (
+from ringity.ringscore.metric2ringscore import ring_score_from_sequence
+from ringity.ringscore.data2metric import (
                                 pwdistance,
                                 pwdistance_from_network,
                                 pwdistance_from_point_cloud,
                                 pwdistance_from_adjacency_matrix)
 
 
 # MODULES
-import ringity.core.statistics as statistics
+import ringity.ringscore.statistics as statistics
 import ringity.singlecell.singlecell as singlecell
```

### Comparing `ringity-0.3a2/ringity/core/data2metric.py` & `ringity-0.3a3/ringity/ringscore/data2metric.py`

 * *Files identical despite different names*

### Comparing `ringity-0.3a2/ringity/core/metric2ringscore.py` & `ringity-0.3a3/ringity/ringscore/metric2ringscore.py`

 * *Files identical despite different names*

### Comparing `ringity-0.3a2/ringity/core/phomology.py` & `ringity-0.3a3/ringity/ringscore/phomology.py`

 * *Files identical despite different names*

### Comparing `ringity-0.3a2/ringity/core/pipeline.py` & `ringity-0.3a3/ringity/ringscore/pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 from ringity.classes.pdiagram import PDiagram
-from ringity.core.metric2ringscore import ring_score_from_sequence
-from ringity.core.data2metric import pwdistance_from_network, pwdistance_from_point_cloud
+from ringity.ringscore.metric2ringscore import ring_score_from_sequence
+from ringity.ringscore.data2metric import pwdistance_from_network, pwdistance_from_point_cloud
 
 from gtda.homology import VietorisRipsPersistence # WE SHOULD GET RID OF THIS IMPORT HERE
 from scipy.spatial.distance import is_valid_dm
 
 import numpy as np
 import networkx as nx
 import scipy.sparse
 
-# -----------------------------------------------------------------------------    
+# -----------------------------------------------------------------------------
 # -------------------- GENERIC PDIAGRAM AND SCORE FUNCTION --------------------
-# ----------------------------------------------------------------------------- 
+# -----------------------------------------------------------------------------
 def ring_score(arg,
             argtype = None,
             flavour = 'geometric',
             exponent = 2,
             nb_pers = np.inf,
             verbose = False,
             **kwargs):
     """Calculate pdiagram from given data structures.
 
     Generic function to calculate ring score by calling another appropriate
     ring score function:
         - If ``arg`` is a networkx graph, it will call ``ring_score_from_network``.
-        - If ``arg`` is a ringity persistence diagram, it will call 
+        - If ``arg`` is a ringity persistence diagram, it will call
         ``ring_score_from_persistence_diagram``.
-        - If ``arg`` is a numpy array or sparse matrix the paramter ``argtype`` 
+        - If ``arg`` is a numpy array or sparse matrix the paramter ``argtype``
         specifies how to interpret the data and which ring-score function to call.
-        
+
     Note: All functions eventually call ``ring_score_from_sequence``.
-    
+
     Parameters
     ----------
     arg : numpy array, sparse matrix, networkx graph or ringity persistence
     diagram.
 
     Returns
     -------
@@ -58,23 +58,23 @@
             verbose = False,
             **kwargs):
     """Calculate ring score from given data structures.
 
     Generic function to calculate persistence diagram by calling another appropriate
     pdiagram function:
         - If ``arg`` is a networkx graph, it will call ``pdiagram_from_network``.
-        - If ``arg`` is a ringity persistence diagram, it will call 
+        - If ``arg`` is a ringity persistence diagram, it will call
         ``pdiagram_from_persistence_diagram``.
-        - If ``arg`` is a numpy array or sparse matrix the paramter ``argtype`` 
-        specifies how to interpret the data and which ring-score function to call. 
+        - If ``arg`` is a numpy array or sparse matrix the paramter ``argtype``
+        specifies how to interpret the data and which ring-score function to call.
         ``None`` will try to guess weather the ``arg`` looks like a ``point cloud`` or a
-        ``distance matrix``. 
-        
+        ``distance matrix``.
+
     Note: All functions eventually call ``pdiagram_from_sequence``.
-    
+
     Parameters
     ----------
     arg : numpy array, sparse matrix, networkx graph or ringity persistence
     diagram.
 
     Returns
     -------
@@ -99,18 +99,18 @@
             pdgm  = pdiagram_from_distance_matrix(arg, **kwargs)
         else:
             raise Exception(f"Argtype `{argtype} unknown.")
     else:
         raise Exception(f"Data structure `{type(arg)} unknown.")
 
     return pdgm
-                                                        
-# -----------------------------------------------------------------------------    
+
+# -----------------------------------------------------------------------------
 # --------------------- DATA SPECIFIC RING SCORE FUNCTIONS --------------------
-# -----------------------------------------------------------------------------     
+# -----------------------------------------------------------------------------
 def ring_score_from_point_cloud(X,
                             flavour = 'geometric',
                             exponent = 2,
                             nb_pers = np.inf,
                             persistence = 'VietorisRipsPersistence',
                             metric = 'euclidean',
                             metric_params = {},
@@ -132,16 +132,16 @@
                                 metric_params = metric_params,
                                 dim = dim,
                                 **kwargs)
     return ring_score_from_pdiagram(pdgm,
                                 flavour = flavour,
                                 exponent = exponent,
                                 nb_pers = nb_pers)
-    
-                                               
+
+
 def ring_score_from_network(G,
                         flavour = 'geometric',
                         exponent = 2,
                         nb_pers = np.inf,
                         persistence = 'VietorisRipsPersistence',
                         metric = 'net_flow',
                         metric_params = {},
@@ -163,16 +163,16 @@
                             metric_params = metric_params,
                             dim = dim,
                             **kwargs)
     return ring_score_from_pdiagram(pdgm,
                                 flavour = flavour,
                                 exponent = exponent,
                                 nb_pers = nb_pers)
-                                    
-                                    
+
+
 def ring_score_from_distance_matrix(D,
                                 persistence = 'VietorisRipsPersistence',
                                 dim = 1,
                                 nb_pers = np.inf,
                                 exponent = 2,
                                 flavour = 'geometric',
                                 **kwargs):
@@ -193,80 +193,100 @@
     flavour : str, optional
         _description_, by default 'geometric'
 
     Returns
     -------
     _type_
         _description_
-    """                                
-    
+    """
+
     pdgm = pdiagram_from_distance_matrix(D,
                                     persistence = persistence,
                                     dim = dim,
                                     **kwargs)
     return ring_score_from_pdiagram(pdgm,
                                     flavour = flavour,
                                     exponent = exponent,
                                     nb_pers = nb_pers)
-                            
-                                    
+
+
 def ring_score_from_pdiagram(pdgm,
+                             score_type = 'length',
                              flavour = 'geometric',
                              nb_pers = np.inf,
                              exponent = 2):
     """Calculates ring-score from a PDiagram object."""
-    return ring_score_from_sequence(pdgm.sequence,
-                                    flavour = flavour,
-                                    nb_pers = nb_pers,
-                                    exponent = exponent)
-                                               
-# -----------------------------------------------------------------------------    
+    trimmed_pdgm = pdgm.trimmed(nb_pers)
+
+    if score_type == 'length':
+        score = ring_score_from_sequence(trimmed_pdgm.plengths,
+                                         flavour = flavour,
+                                         nb_pers = nb_pers,
+                                         exponent = exponent)
+    elif score_type == 'ratio':
+        score = ring_score_from_sequence(trimmed_pdgm.pratios,
+                                            flavour = flavour,
+                                            nb_pers = nb_pers,
+                                            exponent = exponent)
+    elif score_type == 'diameter':
+        score = ring_score_from_sequence(trimmed_pdgm.plengths,
+                                         flavour = flavour,
+                                         nb_pers = nb_pers,
+                                         exponent = exponent)
+        score *= trimmed_pdgm.signal/trimmed_pdgm.diameter * (2/np.sqrt(3))
+
+    else:
+        raise Exception(f"Score type `{score_type}` unknown.")
+
+    return score
+
+# -----------------------------------------------------------------------------
 # ----------------------- PERSISTENCE DIAGRAM FUNCTIONS -----------------------
-# ----------------------------------------------------------------------------- 
+# -----------------------------------------------------------------------------
 def pdiagram_from_point_cloud(X,
                             metric = 'euclidean',
                             dim = 1,
                             persistence = 'VietorisRipsPersistence',
                             **kwargs):
     """Constructs a PDiagram object from a point cloud.
-    
+
     This function wraps persistent homolgy calculation from giotto-tda."""
-    
+
     if persistence == 'VietorisRipsPersistence':
-        D = pwdistance_from_point_cloud(X, 
+        D = pwdistance_from_point_cloud(X,
                                         metric = metric)
-        pdgm = pdiagram_from_distance_matrix(D, 
+        pdgm = pdiagram_from_distance_matrix(D,
                                         dim = dim,
                                         persistence = persistence,
                                         kwargs = kwargs)
-    return pdgm   
-    
-    
-def pdiagram_from_network(G, 
-                        metric = 'net_flow', 
+    return pdgm
+
+
+def pdiagram_from_network(G,
+                        metric = 'net_flow',
                         use_weights = None,
                         store_weights = None,
                         new_weight_name = None,
                         overwrite_weights = False,
                         verbose = False,
                         **kwargs):
     """Constructs a PDiagram object from a networkx graph.
 
-    This function is not available yet. NEEDS TESTING!!!! 
+    This function is not available yet. NEEDS TESTING!!!!
 
     Parameters
     ----------
     G : _type_
         _description_
     metric : str, optional
         _description_, by default 'net_flow'
     use_weights : bool, optional
         _description_, by default None
     store_weights : bool, optional
-        Weights will only be stored if a centrality measure is 
+        Weights will only be stored if a centrality measure is
         used for distance calculations! By default None.
     new_weight_name : _type_, optional
         _description_, by default None
     overwrite_weights : bool, optional
         _description_, by default False
     verbose : bool, optional
         _description_, by default False
@@ -275,21 +295,21 @@
     -------
     _type_
         _description_
     """
 
     D = pwdistance_from_network(G, metric = metric, verbose = verbose)
     return pdiagram_from_distance_matrix(D)
-    
-def pdiagram_from_distance_matrix(D, 
+
+def pdiagram_from_distance_matrix(D,
                                 persistence = 'VietorisRipsPersistence',
                                 dim = 1,
                                 **kwargs):
     """Constructs a PDiagram object from a distance matrix.
     """
     if persistence == 'VietorisRipsPersistence':
         VR = VietorisRipsPersistence(metric = "precomputed",
                                      homology_dimensions = tuple(range(dim+1)))
         pdgm = VR.fit_transform([D])[0]
-    return PDiagram.from_gtda(pdgm, 
-                        dim = dim, 
-                        diameter = D.max())
+    return PDiagram.from_gtda(pdgm,
+                        dim = dim,
+                        diameter = D.max())
```

### Comparing `ringity-0.3a2/ringity/generators/geometric_networks.py` & `ringity-0.3a3/ringity/generators/geometric_networks.py`

 * *Files identical despite different names*

### Comparing `ringity-0.3a2/ringity/generators/network_models.py` & `ringity-0.3a3/ringity/networkmodel/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import networkx as nx
 
 from scipy.spatial.distance import squareform
-from ringity.classes.networkbuilder import NetworkBuilder
-from ringity.generators.utils.param_utils import parse_canonical_parameters
+from ringity.networkmodel.networkbuilder import NetworkBuilder
+from ringity.networkmodel.param_utils import parse_canonical_parameters
 
 def network_model(N,
                   response = None,
                   coupling = None,
                   density = None,
                   rate = None,
                   beta = None,
```

### Comparing `ringity-0.3a2/ringity/generators/point_clouds.py` & `ringity-0.3a3/ringity/generators/point_clouds.py`

 * *Files identical despite different names*

### Comparing `ringity-0.3a2/ringity/generators/utils/distribution_functions.py` & `ringity-0.3a3/ringity/generators/utils/distribution_functions.py`

 * *Files identical despite different names*

### Comparing `ringity-0.3a2/ringity/generators/utils/param_utils.py` & `ringity-0.3a3/ringity/generators/utils/param_utils.py`

 * *Files identical despite different names*

### Comparing `ringity-0.3a2/ringity/generators/utils/transformations.py` & `ringity-0.3a3/ringity/generators/utils/transformations.py`

 * *Files identical despite different names*

### Comparing `ringity-0.3a2/ringity/networkmeasures/centralities.py` & `ringity-0.3a3/ringity/networkmeasures/centralities.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,17 @@
     if not nx.is_connected(G):
         raise DisconnectedGraphError
 
     # The exact sparse representation is irrelevant from a speed
     # perspective, but differs in the implementation below.
     A_coo = nx.to_scipy_sparse_array(G, format = 'coo')
 
+    if not isinstance(A_coo.dtype, np.float64):
+        A_coo = A_coo.astype(np.float64)
+
     # Inverted Laplacian is going to be dense anyways.
     # So there is no harm in working with dense matrices here.
     L = -A_coo.toarray()
     np.fill_diagonal(L, A_coo.sum(axis = 1))
 
     # Removing first (or any other) row and corresponding column from the
     # Laplacian matrix leads to an invertible matrix if the graph is connected.
@@ -144,15 +147,14 @@
 def laplace(A):
     n, m = A.shape
     diags = A.sum(axis=1)
     D = scipy.sparse.spdiags(diags.flatten(), [0], m, n)
     return D - A
 
 def oriented_incidence_matrix(A):
-    assert type(A) == scipy.sparse.csr.csr_matrix
     N = A.shape[0]
     E = int(A.nnz/2)
     B = scipy.sparse.lil_matrix((E, N))
 
     edges = edge_extractor(A)
 
     for ei, (u,v) in enumerate(edges):
```

### Comparing `ringity-0.3a2/ringity/networkmeasures/graphlet_coefficients.py` & `ringity-0.3a3/ringity/networkmeasures/graphlet_coefficients.py`

 * *Files identical despite different names*

### Comparing `ringity-0.3a2/ringity/plotting/_plotly.py` & `ringity-0.3a3/ringity/plotting/_plotly.py`

 * *Files identical despite different names*

### Comparing `ringity-0.3a2/ringity/plotting/animation.py` & `ringity-0.3a3/ringity/plotting/animation.py`

 * *Files identical despite different names*

### Comparing `ringity-0.3a2/ringity/plotting/plot_functions.py` & `ringity-0.3a3/ringity/plotting/plot_functions.py`

 * *Files identical despite different names*

### Comparing `ringity-0.3a2/ringity/plotting/singlecell.py` & `ringity-0.3a3/ringity/plotting/singlecell.py`

 * *Files identical despite different names*

### Comparing `ringity-0.3a2/ringity/plotting/styling.py` & `ringity-0.3a3/ringity/plotting/styling.py`

 * *Files identical despite different names*

### Comparing `ringity-0.3a2/ringity/readwrite/pdiagrams.py` & `ringity-0.3a3/ringity/readwrite/pdiagrams.py`

 * *Files identical despite different names*

### Comparing `ringity-0.3a2/ringity/singlecell/genesets.py` & `ringity-0.3a3/ringity/singlecell/genesets.py`

 * *Files identical despite different names*

### Comparing `ringity-0.3a2/ringity/singlecell/singlecell.py` & `ringity-0.3a3/ringity/singlecell/singlecell.py`

 * *Files identical despite different names*

### Comparing `ringity-0.3a2/ringity.egg-info/PKG-INFO` & `ringity-0.3a3/ringity.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ringity
-Version: 0.3a2
+Version: 0.3a3
 Summary: ringity package
 Home-page: https://github.com/ClusterDuck123/ringity
 Author: Markus K. Youssef
 Author-email: mk.youssef@hotmail.com
 Project-URL: Bug Tracker, https://github.com/kiri93/ringity/issues
 Project-URL: Lab Origin, https://menchelab.com
 Keywords: network ring circular tda
```

### Comparing `ringity-0.3a2/ringity.egg-info/SOURCES.txt` & `ringity-0.3a3/ringity.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -13,37 +13,48 @@
 ringity/classes/__init__.py
 ringity/classes/_distns.py
 ringity/classes/exceptions.py
 ringity/classes/legacy.py
 ringity/classes/modelparameterbuilder.py
 ringity/classes/networkbuilder.py
 ringity/classes/pdiagram.py
-ringity/core/__init__.py
-ringity/core/data2metric.py
-ringity/core/metric2ringscore.py
-ringity/core/phomology.py
-ringity/core/pipeline.py
-ringity/core/statistics.py
 ringity/generators/__init__.py
 ringity/generators/geometric_networks.py
-ringity/generators/network_models.py
 ringity/generators/pdiagrams.py
 ringity/generators/point_clouds.py
 ringity/generators/utils/__init__.py
 ringity/generators/utils/defaults.py
 ringity/generators/utils/distribution_functions.py
 ringity/generators/utils/param_utils.py
 ringity/generators/utils/transformations.py
 ringity/networkmeasures/__init__.py
 ringity/networkmeasures/centralities.py
 ringity/networkmeasures/graphlet_coefficients.py
+ringity/networkmodel/__init__.py
+ringity/networkmodel/distributions.py
+ringity/networkmodel/modelparameterbuilder.py
+ringity/networkmodel/networkbuilder.py
+ringity/networkmodel/param_utils.py
+ringity/networkmodel/transformations.py
 ringity/plotting/__init__.py
 ringity/plotting/_plotly.py
 ringity/plotting/animation.py
 ringity/plotting/plot_functions.py
 ringity/plotting/singlecell.py
 ringity/plotting/styling.py
 ringity/readwrite/__init__.py
 ringity/readwrite/pdiagrams.py
+ringity/ringscore/__init__.py
+ringity/ringscore/data2metric.py
+ringity/ringscore/metric2ringscore.py
+ringity/ringscore/phomology.py
+ringity/ringscore/pipeline.py
+ringity/ringscore/statistics.py
 ringity/singlecell/__init__.py
 ringity/singlecell/genesets.py
-ringity/singlecell/singlecell.py
+ringity/singlecell/singlecell.py
+ringity/userclasses/__init__.py
+ringity/userclasses/_distns.py
+ringity/userclasses/exceptions.py
+ringity/userclasses/formulas.py
+ringity/userclasses/legacy.py
+ringity/userclasses/pdiagram.py
```

### Comparing `ringity-0.3a2/setup.cfg` & `ringity-0.3a3/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 include_package_data = True
 install_requires = 
 	matplotlib
 	networkx
 	numba
 	wheel
 	scipy
+	pandas
+	giotto-tda
 
 [options.package_data]
 * = *.txt, *.rst
 ringity = data/*.csv
 
 [egg_info]
 tag_build =
```

