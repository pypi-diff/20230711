# Comparing `tmp/battetl-1.0.2.tar.gz` & `tmp/battetl-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "battetl-1.0.2.tar", last modified: Wed May 17 03:39:42 2023, max compression
+gzip compressed data, was "battetl-1.1.0.tar", last modified: Tue Jul 11 18:50:37 2023, max compression
```

## Comparing `battetl-1.0.2.tar` & `battetl-1.1.0.tar`

### file list

```diff
@@ -1,34 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 03:39:42.841215 battetl-1.0.2/
--rw-rw-rw-   0        0        0     1087 2023-04-04 20:46:42.000000 battetl-1.0.2/LICENSE
--rw-rw-rw-   0        0        0    15489 2023-05-17 03:39:42.839217 battetl-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    14936 2023-05-10 20:47:12.000000 battetl-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 03:39:42.760103 battetl-1.0.2/battetl/
--rw-rw-rw-   0        0        0     7350 2023-05-17 03:36:10.000000 battetl-1.0.2/battetl/BattETL.py
--rw-rw-rw-   0        0        0      116 2023-04-05 19:58:40.000000 battetl-1.0.2/battetl/__init__.py
--rw-rw-rw-   0        0        0     8802 2023-05-17 03:36:10.000000 battetl-1.0.2/battetl/constants.py
-drwxrwxrwx   0        0        0        0 2023-05-17 03:39:42.802620 battetl-1.0.2/battetl/extract/
--rw-rw-rw-   0        0        0    27305 2023-04-10 18:26:06.000000 battetl-1.0.2/battetl/extract/Extractor.py
--rw-rw-rw-   0        0        0       34 2023-04-05 19:58:40.000000 battetl-1.0.2/battetl/extract/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 03:39:42.813622 battetl-1.0.2/battetl/load/
--rw-rw-rw-   0        0        0    36511 2023-05-17 03:36:10.000000 battetl-1.0.2/battetl/load/Loader.py
--rw-rw-rw-   0        0        0       79 2023-04-26 18:52:26.000000 battetl-1.0.2/battetl/load/__init__.py
--rw-rw-rw-   0        0        0     6816 2023-05-17 03:36:10.000000 battetl-1.0.2/battetl/load/batt_db_test_helper.py
--rw-rw-rw-   0        0        0     1728 2023-05-10 20:47:12.000000 battetl-1.0.2/battetl/logger.py
-drwxrwxrwx   0        0        0        0 2023-05-17 03:39:42.819625 battetl-1.0.2/battetl/transform/
--rw-rw-rw-   0        0        0    26425 2023-05-17 03:36:10.000000 battetl-1.0.2/battetl/transform/Transformer.py
--rw-rw-rw-   0        0        0       38 2023-04-05 19:58:40.000000 battetl-1.0.2/battetl/transform/__init__.py
--rw-rw-rw-   0        0        0    12452 2023-04-26 18:52:26.000000 battetl-1.0.2/battetl/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-17 03:39:42.793621 battetl-1.0.2/battetl.egg-info/
--rw-rw-rw-   0        0        0    15489 2023-05-17 03:39:42.000000 battetl-1.0.2/battetl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      592 2023-05-17 03:39:42.000000 battetl-1.0.2/battetl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 03:39:42.000000 battetl-1.0.2/battetl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      171 2023-05-17 03:39:42.000000 battetl-1.0.2/battetl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-17 03:39:42.000000 battetl-1.0.2/battetl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 03:39:42.841215 battetl-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      900 2023-04-24 19:52:15.000000 battetl-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-17 03:39:42.836217 battetl-1.0.2/tests/
--rw-rw-rw-   0        0        0     4494 2023-05-17 03:36:10.000000 battetl-1.0.2/tests/test_BattETL.py
--rw-rw-rw-   0        0        0    17547 2023-04-26 18:52:26.000000 battetl-1.0.2/tests/test_Extractor.py
--rw-rw-rw-   0        0        0    26574 2023-05-17 03:36:10.000000 battetl-1.0.2/tests/test_Loader.py
--rw-rw-rw-   0        0        0    12554 2023-05-17 03:36:10.000000 battetl-1.0.2/tests/test_Transformer.py
--rw-rw-rw-   0        0        0     2532 2023-04-11 19:33:26.000000 battetl-1.0.2/tests/test_utils.py
+drwxr-xr-x   0 Benjamin   (502) staff       (20)        0 2023-07-11 18:50:37.135462 battetl-1.1.0/
+-rw-r--r--   0 Benjamin   (502) staff       (20)     1066 2023-07-10 18:08:18.000000 battetl-1.1.0/LICENSE
+-rw-r--r--   0 Benjamin   (502) staff       (20)    16509 2023-07-11 18:50:37.134989 battetl-1.1.0/PKG-INFO
+-rw-r--r--   0 Benjamin   (502) staff       (20)    15958 2023-07-11 18:30:14.000000 battetl-1.1.0/README.md
+drwxr-xr-x   0 Benjamin   (502) staff       (20)        0 2023-07-11 18:50:37.125758 battetl-1.1.0/battetl/
+-rw-r--r--   0 Benjamin   (502) staff       (20)     7528 2023-07-11 18:30:14.000000 battetl-1.1.0/battetl/BattETL.py
+-rw-r--r--   0 Benjamin   (502) staff       (20)      155 2023-07-11 18:30:14.000000 battetl-1.1.0/battetl/__init__.py
+-rw-r--r--   0 Benjamin   (502) staff       (20)     6971 2023-07-11 18:30:14.000000 battetl-1.1.0/battetl/battetl_quick.py
+-rw-r--r--   0 Benjamin   (502) staff       (20)     9627 2023-07-11 18:30:14.000000 battetl-1.1.0/battetl/constants.py
+drwxr-xr-x   0 Benjamin   (502) staff       (20)        0 2023-07-11 18:50:37.129643 battetl-1.1.0/battetl/extract/
+-rw-r--r--   0 Benjamin   (502) staff       (20)    26560 2023-07-10 18:08:18.000000 battetl-1.1.0/battetl/extract/Extractor.py
+-rw-r--r--   0 Benjamin   (502) staff       (20)       33 2023-07-10 18:08:18.000000 battetl-1.1.0/battetl/extract/__init__.py
+drwxr-xr-x   0 Benjamin   (502) staff       (20)        0 2023-07-11 18:50:37.132503 battetl-1.1.0/battetl/load/
+-rw-r--r--   0 Benjamin   (502) staff       (20)    39804 2023-07-11 18:30:14.000000 battetl-1.1.0/battetl/load/Loader.py
+-rw-r--r--   0 Benjamin   (502) staff       (20)      115 2023-07-11 18:30:14.000000 battetl-1.1.0/battetl/load/__init__.py
+-rw-r--r--   0 Benjamin   (502) staff       (20)     7341 2023-07-11 18:30:14.000000 battetl-1.1.0/battetl/load/batt_db_test_helper.py
+-rw-r--r--   0 Benjamin   (502) staff       (20)     3201 2023-07-11 18:30:14.000000 battetl-1.1.0/battetl/load/quick_loader.py
+-rw-r--r--   0 Benjamin   (502) staff       (20)     1677 2023-07-10 18:08:18.000000 battetl-1.1.0/battetl/logger.py
+drwxr-xr-x   0 Benjamin   (502) staff       (20)        0 2023-07-11 18:50:37.134052 battetl-1.1.0/battetl/transform/
+-rw-r--r--   0 Benjamin   (502) staff       (20)    29328 2023-07-11 18:30:14.000000 battetl-1.1.0/battetl/transform/Transformer.py
+-rw-r--r--   0 Benjamin   (502) staff       (20)       37 2023-07-10 18:08:18.000000 battetl-1.1.0/battetl/transform/__init__.py
+-rw-r--r--   0 Benjamin   (502) staff       (20)    13584 2023-07-11 18:30:14.000000 battetl-1.1.0/battetl/utils.py
+drwxr-xr-x   0 Benjamin   (502) staff       (20)        0 2023-07-11 18:50:37.128158 battetl-1.1.0/battetl.egg-info/
+-rw-r--r--   0 Benjamin   (502) staff       (20)    16509 2023-07-11 18:50:37.000000 battetl-1.1.0/battetl.egg-info/PKG-INFO
+-rw-r--r--   0 Benjamin   (502) staff       (20)      533 2023-07-11 18:50:37.000000 battetl-1.1.0/battetl.egg-info/SOURCES.txt
+-rw-r--r--   0 Benjamin   (502) staff       (20)        1 2023-07-11 18:50:37.000000 battetl-1.1.0/battetl.egg-info/dependency_links.txt
+-rw-r--r--   0 Benjamin   (502) staff       (20)      171 2023-07-11 18:50:37.000000 battetl-1.1.0/battetl.egg-info/requires.txt
+-rw-r--r--   0 Benjamin   (502) staff       (20)        8 2023-07-11 18:50:37.000000 battetl-1.1.0/battetl.egg-info/top_level.txt
+-rw-r--r--   0 Benjamin   (502) staff       (20)       38 2023-07-11 18:50:37.135569 battetl-1.1.0/setup.cfg
+-rw-r--r--   0 Benjamin   (502) staff       (20)      886 2023-07-11 18:30:14.000000 battetl-1.1.0/setup.py
```

### Comparing `battetl-1.0.2/LICENSE` & `battetl-1.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 BattGenie
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 BattGenie
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `battetl-1.0.2/PKG-INFO` & `battetl-1.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,329 +1,358 @@
-Metadata-Version: 2.1
-Name: battetl
-Version: 1.0.2
-Summary: A Python module for extracting, transforming, and loading battery data to a database.
-Home-page: https://github.com/BattGenie/battetl
-Author: Zander Nevitt, Bing Syuan Wang and Chintan Pathak
-Author-email: info@battgenie.life
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9, <3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/BattETL_Logo.png">
-
-# BattETL
-
-BattETL is a well-tested and an enterprise-ready python module for **E**xtracting, **T**ransforming, and **L**oading battery cycler data to a [database](https://github.com/BattGenie/battdb). BattETL can also be used just for data extraction and transformation if a database is not desired. Currently data from Maccor and Arbin cyclers are supported.
-
-<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/BattETL_Simple_System.svg">
-
-## Overview
-
-- [Motivation](#motivation)
-- [Video Guides](#video-guides)
-- [Installation](#installation)
-  - [Requirements](#requirements)
-  - [Installation Instructions](#installation-instructions)
-- [Usage](#usage)
-  - [Config File](#config-file)
-  - [Env File](#env-file)
-  - [Data Export Requirements](#data-export-requirements)
-    - [Maccor](#maccor)
-    - [Arbin](#arbin)
-- [BattETL Overview](#battetl-overview)
-  - [System Diagram](#system-diagram)
-  - [Transformer](#transformer)
-  - [Extractor](#extractor)
-  - [Loader](#loader)
-- [Testing](#testing)
-- [Troubleshooting](#troubleshooting)
-
-## Motivation
-
-### Why another battery cycler data ingesting tool?
-
-There are published [open](https://github.com/TRI-AMDD/beep) [source](https://github.com/Battery-Intelligence-Lab/galvanalyser) solutions for battery cycler data ingestion. BattETL hopes to build on these tools and adds a few conveniences to support robust data management and repeatable data analytics.
-
-### Some features of BattETL
-
-- **A relational data destination.**
-
-BattETL package is tightly coupled to the destination database it sends the data to. BattETL requires that for the battery data that is loaded to the database - the detailed metadata such as battery make and model, cycler make and model, and schedule/procedure information be also included. While these constraints (somewhat) slowdown the data ingestion process, it ensures verifiable, high-quality data persistance.
-
-- **A database that can hold *all* relevant battery test information.**
-
-Not only does the BattETL extract and store all the battery test data, it also captures the cycler schedule/procedure file. In addition to the schedule/procedure file, BattETL captures and stores all files associated with the schedule/procedure. This includes any current profiles (Maccor FastWave or Arbin current simulation files), EIS specifications, or even entire system specifications (Arbin batch files.)
-
-- **Analytics built into the transformation step.**
-
-As part of the transformation step BattETL calculates various cycle statistics (capacity, coulombic efficiency, CC/CV charge times, etc.) providing independent and supplemental cycle statistics to compliment those generated by the cycler software. These can particularly handy when easy-to-miss settings were overlooked in writing the schedule (e.g. forgetting to reset the capacity when incriminating the cycle.) Do you have some sort of hyper-boutique transformation or statistic calculation needed for a specific test? No problem. BattETL can apply user defined transformation functions too; all before the data is loaded to the database.
-
-## Video Guides
-
-The following are video guides BattETL and BattDB:
-
-- [Installation & setup](https://www.youtube.com/watch?v=tmudLhrj9xE)
-- [Design overview](https://www.youtube.com/watch?v=Y2tXInbkYF8)
-- [Demonstration](https://www.youtube.com/watch?v=3wNd3fhqBwo)
-
-## Installation
-
-A video showing how to setup and install BattETL and BattDB can be found [here](https://www.youtube.com/watch?v=tmudLhrj9xE)
-
-### Requirements
-
-#### Software Requirements
-
-- Python 3.9 or 3.10
-- The required packages are listed in the `requirements.txt` file
-
-#### Hardware Requirements
-
-Based on processing approximately 10,000 rows and 12 columns with Pandas, BattETL requires a minimum of 13MB of RAM.
-
-- RAM: 2 GB or higher.
-- Disk Space: At least 2 GB of free space is recommended to accommodate the transformed data, as well as additional space for installation and storing data. The exact amount of disk space required will depend on the size of the data being processed and the resulting intermediate results.
-
-### Installation Instructions
-
-- Install BattETL using pip:
-
-```sh
-pip install battetl
-```
-
-- Install BattETL from source code:
-
-```sh
-git clone https://github.com/BattGenie/battetl.git
-cd battetl
-pip install -r requirements.txt
-pip install .
-```
-
-> Note that if you wish to use the Load feature of BattETL it is necessary to deploy an instance of a [BattDB](https://github.com/BattGenie/battdb) database to load the data to. Follow the instructions there for deploying the database.
-
-## Usage
-
-A video demonstrating how to use BattETL and BattDB can be found [here](https://www.youtube.com/watch?v=3wNd3fhqBwo)
-
-Using BattETL as an all-in-one ETL function is as easy as:
-
-```python
-from battetl import BattETL
-
-cell = BattETL(config_path).extract().transform().load()
-```
-
-Where `config_path` is the absolute or relative path to BattETL [config file](#config-file).
-
-It is also necessary to include an [.env file](#env-file) within the working directory that contains the associated database credentials.
-
-Finally, the data must be exported from the cycler in a [specific format](#data-export-requirements)
-
-For a practical implementation of `BattETL`, please refer to the example notebook `examples/battetl_demo.ipynb` located in the `examples` directory. This notebook demonstrates how to implement `BattETL` and can serve as a useful reference for your own project.
-
-> Note that repeated calls to load test data that already exists in the database (as determined by unix timestamp) will not overwrite any existing data. Only test data after the most recent existing unix timestamp will be loaded. In the case of loading cycle statistics, any duplicate cycles that already exist in the database will be overwritten.
-
-### Config File
-
-To use BattETL it is necessary to provide a path to JSON configuration file. This config file contains paths to the relevant test data files and test metadata used for analysis and establishing database relations. An example configuration file is given within `examples/battetl_config_example.json`
-
-```json
-{
-    "timezone": "America/Los_Angeles",
-    "data_file_path": [
-        "abs/path/to/your/arbin/or/maccor/test/data/file(s).txt"
-    ],
-    "stats_file_path": [
-        "abs/path/to/your/arbin/or/maccor/test/stats/file.txt"
-    ],
-    "schedule_file_path": [
-        "abs/path/to/your/schedule/or/procedure/file(s).000"
-    ],
-    "meta_data": {
-        "test_meta": {
-            "test_name": "the_name_of_your_test",
-            "channel": 10
-        },
-        "cell": {
-            "manufacturer_sn": "0001"
-        },
-        "cell_meta": {
-            "manufacturer": "FakeMN",
-            "manufacturer_pn": "1234"
-        },
-        "schedule_meta": {
-            "schedule_name": "fake_schedule.000",
-            "cycler_make": "BattGenie"
-        },
-        "cycler": {
-            "sn": "0001"
-        },
-        "cycler_meta": {
-            "manufacturer": "BattGenie",
-            "model": "Cycler9000"
-        }
-    }
-}
-```
-
-### Env File
-
-The .env contains the associated database credentials and is formatted as follows
-
-```
-ENV=dev # dev, prod
-DB_TARGET=YOUR_DATABASE_NAME
-DB_USERNAME=YOUR_USERNAME
-DB_PASSWORD=YOUR_PASSWORD
-DB_HOSTNAME=localhost
-DB_PORT=5432
-```
-
-An example .env file is given within `examples/.env.example`
-
-### Data Export Requirements
-
-- [For Maccor Cycler](#maccor)
-- [For Arbin Cycler](#arbin)
-
-#### Maccor
-
-From the "Maccor Export" tool data should be exported as "Text Output" in a "Tab Delimited" format. The output sheets should include "Data Records" and "Cycle Statistics". The box for "Discharge Current Exported Negative" should be checked.
-
-The following columns are the minimum required for export:
-
-For Data Records:
-
-- Cycle : Header Label of Cyc#
-- Step : Header Label of Step
-- Test Time : Header Label of TestTime(s), Units of seconds
-- Step Time : Header Label of StepTime(s), Units of seconds
-- Capacity : Header Label of Capacity(Ah), Units of Amp-Hour
-- Energy : Header Label of Watt-hr, Units of Watt-hour
-- Current : Header Label of Current(A), Units of Amps
-- Voltage : Header Label of Voltage(V), Units of Volts
-- DPT Time : Header label of DPt Time
-
-<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/MaccorExport_DataRecords.png" width="85%" height="50%">
-
-For Cycle Statistics:
-
-- Cycle : Header Label of Cycle
-- Capacity Chg : Header label AH-IN, Units of Ahr
-- Capacity Dis : Header label AH-Out, Units of Ahr
-- DPT Time : Header Label of DPt Time
-
-<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/MaccorExport_CycleStats.png" width="85%" height="50%">
-
-#### Arbin
-
-Within the Arbin Export tool the "File Type" should be set to "To CSV". Within "Data Filter" the box "statistics by Cycle" should be checked along with any other data. For range filter "All" should be selected.
-
-<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/ArbinExport.jpg" width="45%" height="25%">
-
-An example notebook `battetl_demo.ipynb` that provides a tool to help generate config files is located in the `examples` directory.
-
-## BattETL Overview
-
-A video discussing the design of BattDB and BattETL can be found [here](https://www.youtube.com/watch?v=Y2tXInbkYF8)
-
-BattETL bundles together the three independent submodules:
-
-- [Extractor](#extractor) : Responsible for extractor the cycler data and schedule/procedure files.
-- [Transformer](#transformer) : Responsible for transforming cycler data
-- [Loader](#loader) : Responsible for loading data and associated data to the database.
-
-After running BattETL on a specific configuration file the following objects will be available as class variables from the instance:
-
-- `raw_test_data: pandas.DataFrame`: The raw test data exactly as it is in the generated cycler data file(s).
-- `raw_cycle_stats: pandas.DataFrame`: The raw cycle stats data exactly as it is in the generated cycler statistics file.
-- `test_data: pandas.DataFrame`: The transformed test data after normalizing units and datatype and adding a unixtime column.
-- `cycle_stats: pandas.DataFrame`: The transformed cycle stats after normalizing units, datatypes, and calculating supplemental cycle statistics.
-- `schedule: dict`: The procedure/schedule file and all associated files in a nested Dictionary.
-
-### System diagram
-
-<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/BattETL_SystemDiagram.svg">
-
-### Extractor
-
-The Extractor is an interface that allows you to extract battery test data from raw data files. You can extract test data and cycle stats data from multiple files using `data_from_files`, and extract Arbin schedules or Maccor procedures and associated files using `schedule_from_files`.
-
-For an example of the Extractor as a standalone class, see `examples/submodule_demos/Extractor_demo.ipynb`
-
-#### Functions
-
-- `data_from_files(paths: list[str])`: Extracts multiple test data files into a single pandas DataFrame.  
-- `schedule_from_files(paths: list[str])`: Extracts Arbin schedules or Maccor procedures and associated files and stores them in a dictionary.  
-- `from_pickle(path: str)`: Reads data from the passed file path and returns it as a pandas DataFrame.  
-
-#### Variables
-
-- `cycler_make: str`: Cycler make  
-- `raw_test_data_meta_data: list[dict]`: Test data meta data  
-- `raw_cycle_stats_meta_data: list[dict]`: Cycler stats meta data  
-- `raw_test_data: pandas.DataFrame`: Test data  
-- `raw_cycle_stats: pandas.DataFrame`: Cycler stats  
-- `maccor_procedure: dict`: Maccor procedure  
-- `arbin_schedule: dict`: Arbin schedule  
-
-### Transformer
-
-The Transformer is an interface that allows you to transform battery test data to the BattETL schema. By default, the time zone is set to 'America/Los_Angeles', but you can modify it to your preferred time zone using the names found in the [IANA Time Zone Database](https://www.iana.org/time-zones). In addition to the default functions provided by the Transformer, you can add your own custom functions to perform specific transformations on your data.
-
-For an example of the Extractor as a standalone class, see `examples/submodule_demos/Transformer_demo.ipynb`
-
-#### Functions
-
-- `transform_test_data(self, data: pd.DataFrame)`: Transforms test data to conform to BattETL naming and data conventions  
-- `transform_cycle_stats`: Transforms cycle stats to conform to BattETL naming and data conventions  
-
-#### Variables
-
-- `timezone: str`: Time zone strings in the IANA Time Zone Database. Used to convert to unix timestamp in seconds. Default 'America/Los_Angeles'.  
-- `user_transform_test_data`: A user defined function to transform test data. The function should take a pandas.DataFrame as input and return a pandas.DataFrame as output.  
-- `user_transform_cycle_stats`: A user defined function to transform cycle stats. The function should take a pandas.DataFrame as input and return a pandas.DataFrame as output.  
-- `test_data: pandas.DataFrame`: Transformed test data  
-- `cycle_stats: pandas.DataFrame`: Transformed cycle stats  
-
-### Loader
-
-The `load` module provides an interface to load the extracted data into a database.
-
-Note that repeated calls to load test data that already exists in the database (as determined by unix timestamp) will not overwrite any existing data. Only test data after the latest existing unix timestamp will be loaded. In the case of loading cycle statistics, any duplicate cycles that already exist in the database will be overwritten.
-
-For an example of the Extractor as a standalone class, see `examples/submodule_demos/Loader_demo.ipynb`
-
-#### Functions
-
-- `load_test_data(test_data_df)`: Loads test_data_df to `test_data` table in the specified database.  
-- `load_cycle_stats(cycle_stats_df)`: Loads cycle_stats_df to `test_data_cycle_stats` table in the specified database.  
-
-## Testing
-
-To run the test suite, use the following commands:
-
-- Run all tests: `pytest`
-- Run Maccor tests: `pytest -m maccor`
-- Run Arbin tests: `pytest -m arbin`
-- Run database specific tests: `pytest -m database`
-- Run tests other than Arbin: `pytest -m "not arbin"`
-- Run Extractor tests: `pytest tests/test_extract_data.py`
-
-To show logs while testing, add the `-o log_cli=true` flag.
-
-## Troubleshooting
-
-### pip install psycopg2 error
-
-If there is an error `Error: pg_config executable not found.` Try installing `libpq-dev` before installing `psycopg2`
-
-```sh
-sudo apt install libpq-dev
-```
+Metadata-Version: 2.1
+Name: battetl
+Version: 1.1.0
+Summary: A Python module for extracting, transforming, and loading battery data to a database.
+Home-page: https://github.com/BattGenie/battetl
+Author: Zander Nevitt, Bing Syuan Wang, Eric Ravet, and Chintan Pathak
+Author-email: info@battgenie.life
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9, <3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/BattETL_Logo.png">
+
+# BattETL
+
+BattETL is a well-tested and an enterprise-ready python module for **E**xtracting, **T**ransforming, and **L**oading battery cycler data to a [database](https://github.com/BattGenie/battdb). BattETL can also be used just for data extraction and transformation if a database is not desired. Currently data from Maccor and Arbin cyclers are supported.
+
+<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/BattETL_Simple_System.svg">
+
+## Overview
+
+- [Motivation](#motivation)
+- [Video Guides](#video-guides)
+- [Installation](#installation)
+  - [Requirements](#requirements)
+  - [Installation Instructions](#installation-instructions)
+- [Usage](#usage)
+  - [Quick Mode](#quick-mode)
+  - [Config File](#config-file)
+  - [Env File](#env-file)
+  - [Data Export Requirements](#data-export-requirements)
+    - [Maccor](#maccor)
+    - [Arbin](#arbin)
+- [BattETL Overview](#battetl-overview)
+  - [System Diagram](#system-diagram)
+  - [Transformer](#transformer)
+  - [Extractor](#extractor)
+  - [Loader](#loader)
+- [Testing](#testing)
+- [Troubleshooting](#troubleshooting)
+
+## Motivation
+
+### Why another battery cycler data ingesting tool?
+
+There are published [open](https://github.com/TRI-AMDD/beep) [source](https://github.com/Battery-Intelligence-Lab/galvanalyser) solutions for battery cycler data ingestion. BattETL hopes to build on these tools and adds a few conveniences to support robust data management and repeatable data analytics.
+
+### Some features of BattETL
+
+- **A relational data destination.**
+
+BattETL package is tightly coupled to the destination database it sends the data to. BattETL requires that for the battery data that is loaded to the database - the detailed metadata such as battery make and model, cycler make and model, and schedule/procedure information be also included. While these constraints (somewhat) slowdown the data ingestion process, it ensures verifiable, high-quality data persistance.
+
+- **A database that can hold *all* relevant battery test information.**
+
+Not only does the BattETL extract and store all the battery test data, it also captures the cycler schedule/procedure file. In addition to the schedule/procedure file, BattETL captures and stores all files associated with the schedule/procedure. This includes any current profiles (Maccor FastWave or Arbin current simulation files), EIS specifications, or even entire system specifications (Arbin batch files.)
+
+- **Analytics built into the transformation step.**
+
+As part of the transformation step BattETL calculates various cycle statistics (capacity, coulombic efficiency, CC/CV charge times, etc.) providing independent and supplemental cycle statistics to compliment those generated by the cycler software. These can particularly handy when easy-to-miss settings were overlooked in writing the schedule (e.g. forgetting to reset the capacity when incriminating the cycle.) Do you have some sort of hyper-boutique transformation or statistic calculation needed for a specific test? No problem. BattETL can apply user defined transformation functions too; all before the data is loaded to the database.
+
+## Video Guides
+
+The following are video guides BattETL and BattDB:
+
+- [Installation & setup](https://www.youtube.com/watch?v=tmudLhrj9xE)
+- [Design overview](https://www.youtube.com/watch?v=Y2tXInbkYF8)
+- [Demonstration](https://www.youtube.com/watch?v=3wNd3fhqBwo)
+
+## Installation
+
+A video showing how to setup and install BattETL and BattDB can be found [here](https://www.youtube.com/watch?v=tmudLhrj9xE)
+
+### Requirements
+
+#### Software Requirements
+
+- Python 3.9 or 3.10
+- The required packages are listed in the `requirements.txt` file
+
+#### Hardware Requirements
+
+Based on processing approximately 10,000 rows and 12 columns with Pandas, BattETL requires a minimum of 13MB of RAM.
+
+- RAM: 2 GB or higher.
+- Disk Space: At least 2 GB of free space is recommended to accommodate the transformed data, as well as additional space for installation and storing data. The exact amount of disk space required will depend on the size of the data being processed and the resulting intermediate results.
+
+### Installation Instructions
+
+- Install BattETL using pip:
+
+```sh
+pip install battetl
+```
+
+- Install BattETL from source code:
+
+```sh
+git clone https://github.com/BattGenie/battetl.git
+cd battetl
+pip install -r requirements.txt
+pip install .
+```
+
+> Note that if you wish to use the Load feature of BattETL it is necessary to deploy an instance of a [BattDB](https://github.com/BattGenie/battdb) database to load the data to. Follow the instructions there for deploying the database.
+
+## Usage
+
+A video demonstrating how to use BattETL and BattDB can be found [here](https://www.youtube.com/watch?v=3wNd3fhqBwo)
+
+Using BattETL as an all-in-one ETL function is as easy as:
+
+```python
+from battetl import BattETL
+
+cell = BattETL(config_path).extract().transform().load()
+```
+
+Where `config_path` is the absolute or relative path to BattETL [config file](#config-file).
+
+It is also necessary to include an [.env file](#env-file) within the working directory that contains the associated database credentials.
+
+Finally, the data must be exported from the cycler in a [specific format](#data-export-requirements)
+
+For a practical implementation of `BattETL`, please refer to the example notebook `examples/battetl_demo.ipynb` located in the `examples` directory. This notebook demonstrates how to implement `BattETL` and can serve as a useful reference for your own project.
+
+> Note that repeated calls to load test data that already exists in the database (as determined by unix timestamp) will not overwrite any existing data. Only test data after the most recent existing unix timestamp will be loaded. In the case of loading cycle statistics, any duplicate cycles that already exist in the database will be overwritten.
+
+### Quick Mode
+
+BattETL provides a Quick Mode, which automatically detects whether the given file is test data or test stats from a Maccor or an Arbin cycler, and uploads it to the database accordingly. Here's an example command line:
+
+```bash
+python -m battetl.battetl_quick file="TEST_DATA.txt" db_url="postgres://postgres:password@localhost:5454/battdb_quick"
+```
+
+This command relies on [BattDB](https://github.com/BattGenie/BattDB). If BattDB does not exist, a database will be created using Docker Compose and the data will be uploaded to it. The command also returns a harmonized Pandas dataframe that can be used for analysis and visualization. 
+
+### Config File
+
+To use BattETL it is necessary to provide a path to JSON configuration file. This config file contains paths to the relevant test data files and test metadata used for analysis and establishing database relations. An example configuration file is given within `examples/battetl_config_example.json`
+
+```json
+{
+    "timezone": "America/Los_Angeles",
+    "data_file_path": [
+        "abs/path/to/your/arbin/or/maccor/test/data/file(s).txt"
+    ],
+    "stats_file_path": [
+        "abs/path/to/your/arbin/or/maccor/test/stats/file.txt"
+    ],
+    "schedule_file_path": [
+        "abs/path/to/your/schedule/or/procedure/file(s).000"
+    ],
+    "meta_data": {
+        "test_meta": {
+            "test_name": "the_name_of_your_test",
+            "channel": 10
+        },
+        "cell": {
+            "manufacturer_sn": "0001"
+        },
+        "cell_meta": {
+            "manufacturer": "FakeMN",
+            "manufacturer_pn": "1234"
+        },
+        "schedule_meta": {
+            "schedule_name": "fake_schedule.000",
+            "cycler_make": "BattGenie"
+        },
+        "cycler": {
+            "sn": "0001"
+        },
+        "cycler_meta": {
+            "manufacturer": "BattGenie",
+            "model": "Cycler9000"
+        },
+        "customers": {
+            "customer_name": "FakeCustomer"
+        },
+        "projects": {
+            "project_name": "FakeProject"
+        }
+    }
+}
+```
+
+#### Cell Thermocouple (optional)
+
+If the cell has a thermocouple, it is necessary to include the following in the header of the config file:
+
+```json
+"cell_thermocouple": 1
+```
+
+where `1` corresponds to the thermocouple index in the cycler test data export, i.e `Temp 1` for Maccor and `Aux_Temperature_1 (C)` for Arbin.
+
+If no cell thermocouple value is listed, `calculated_max_charge_temp_c` and `calculated_max_discharge_temp_c` will be set to `null` in the `test_data_cycle_stats` table.
+
+### Env File
+
+The .env contains the associated database credentials and is formatted as follows
+
+```text
+ENV=dev # dev, prod
+DB_TARGET=YOUR_DATABASE_NAME
+DB_USERNAME=YOUR_USERNAME
+DB_PASSWORD=YOUR_PASSWORD
+DB_HOSTNAME=localhost
+DB_PORT=5432
+```
+
+An example .env file is given within `examples/.env.example`
+
+### Data Export Requirements
+
+- [For Maccor Cycler](#maccor)
+- [For Arbin Cycler](#arbin)
+
+#### Maccor
+
+From the "Maccor Export" tool data should be exported as "Text Output" in a "Tab Delimited" format. The output sheets should include "Data Records" and "Cycle Statistics". The box for "Discharge Current Exported Negative" should be checked.
+
+The following columns are the minimum required for export:
+
+For Data Records:
+
+- Cycle : Header Label of Cyc#
+- Step : Header Label of Step
+- Test Time : Header Label of TestTime(s), Units of seconds
+- Step Time : Header Label of StepTime(s), Units of seconds
+- Capacity : Header Label of Capacity(Ah), Units of Amp-Hour
+- Energy : Header Label of Watt-hr, Units of Watt-hour
+- Current : Header Label of Current(A), Units of Amps
+- Voltage : Header Label of Voltage(V), Units of Volts
+- DPT Time : Header label of DPt Time
+
+<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/MaccorExport_DataRecords.png" width="85%" height="50%">
+
+For Cycle Statistics:
+
+- Cycle : Header Label of Cycle
+- Capacity Chg : Header label AH-IN, Units of Ahr
+- Capacity Dis : Header label AH-Out, Units of Ahr
+- DPT Time : Header Label of DPt Time
+
+<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/MaccorExport_CycleStats.png" width="85%" height="50%">
+
+#### Arbin
+
+Within the Arbin Export tool the "File Type" should be set to "To CSV". Within "Data Filter" the box "statistics by Cycle" should be checked along with any other data. For range filter "All" should be selected.
+
+<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/ArbinExport.jpg" width="45%" height="25%">
+
+An example notebook `battetl_demo.ipynb` that provides a tool to help generate config files is located in the `examples` directory.
+
+## BattETL Overview
+
+A video discussing the design of BattDB and BattETL can be found [here](https://www.youtube.com/watch?v=Y2tXInbkYF8)
+
+BattETL bundles together the three independent submodules:
+
+- [Extractor](#extractor) : Responsible for extractor the cycler data and schedule/procedure files.
+- [Transformer](#transformer) : Responsible for transforming cycler data
+- [Loader](#loader) : Responsible for loading data and associated data to the database.
+
+After running BattETL on a specific configuration file the following objects will be available as class variables from the instance:
+
+- `raw_test_data: pandas.DataFrame`: The raw test data exactly as it is in the generated cycler data file(s).
+- `raw_cycle_stats: pandas.DataFrame`: The raw cycle stats data exactly as it is in the generated cycler statistics file.
+- `test_data: pandas.DataFrame`: The transformed test data after normalizing units and datatype and adding a unixtime column.
+- `cycle_stats: pandas.DataFrame`: The transformed cycle stats after normalizing units, datatypes, and calculating supplemental cycle statistics.
+- `schedule: dict`: The procedure/schedule file and all associated files in a nested Dictionary.
+
+### System diagram
+
+<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/BattETL_SystemDiagram.svg">
+
+### Extractor
+
+The Extractor is an interface that allows you to extract battery test data from raw data files. You can extract test data and cycle stats data from multiple files using `data_from_files`, and extract Arbin schedules or Maccor procedures and associated files using `schedule_from_files`.
+
+For an example of the Extractor as a standalone class, see `examples/submodule_demos/Extractor_demo.ipynb`
+
+#### Functions
+
+- `data_from_files(paths: list[str])`: Extracts multiple test data files into a single pandas DataFrame.  
+- `schedule_from_files(paths: list[str])`: Extracts Arbin schedules or Maccor procedures and associated files and stores them in a dictionary.  
+- `from_pickle(path: str)`: Reads data from the passed file path and returns it as a pandas DataFrame.  
+
+#### Variables
+
+- `cycler_make: str`: Cycler make  
+- `raw_test_data_meta_data: list[dict]`: Test data meta data  
+- `raw_cycle_stats_meta_data: list[dict]`: Cycler stats meta data  
+- `raw_test_data: pandas.DataFrame`: Test data  
+- `raw_cycle_stats: pandas.DataFrame`: Cycler stats  
+- `maccor_procedure: dict`: Maccor procedure  
+- `arbin_schedule: dict`: Arbin schedule  
+
+### Transformer
+
+The Transformer is an interface that allows you to transform battery test data to the BattETL schema. By default, the time zone is set to 'America/Los_Angeles', but you can modify it to your preferred time zone using the names found in the [IANA Time Zone Database](https://www.iana.org/time-zones). In addition to the default functions provided by the Transformer, you can add your own custom functions to perform specific transformations on your data.
+
+For an example of the Extractor as a standalone class, see `examples/submodule_demos/Transformer_demo.ipynb`
+
+#### Functions
+
+- `transform_test_data(self, data: pd.DataFrame)`: Transforms test data to conform to BattETL naming and data conventions  
+- `transform_cycle_stats`: Transforms cycle stats to conform to BattETL naming and data conventions  
+
+#### Variables
+
+- `timezone: str`: Time zone strings in the IANA Time Zone Database. Used to convert to unix timestamp in seconds. Default 'America/Los_Angeles'.  
+- `user_transform_test_data`: A user defined function to transform test data. The function should take a pandas.DataFrame as input and return a pandas.DataFrame as output.  
+- `user_transform_cycle_stats`: A user defined function to transform cycle stats. The function should take a pandas.DataFrame as input and return a pandas.DataFrame as output.  
+- `test_data: pandas.DataFrame`: Transformed test data  
+- `cycle_stats: pandas.DataFrame`: Transformed cycle stats  
+
+### Loader
+
+The `load` module provides an interface to load the extracted data into a database.
+
+Note that repeated calls to load test data that already exists in the database (as determined by unix timestamp) will not overwrite any existing data. Only test data after the latest existing unix timestamp will be loaded. In the case of loading cycle statistics, any duplicate cycles that already exist in the database will be overwritten.
+
+For an example of the Extractor as a standalone class, see `examples/submodule_demos/Loader_demo.ipynb`
+
+#### Functions
+
+- `load_test_data(test_data_df)`: Loads test_data_df to `test_data` table in the specified database.  
+- `load_cycle_stats(cycle_stats_df)`: Loads cycle_stats_df to `test_data_cycle_stats` table in the specified database.  
+
+## Testing
+
+To run the test suite, use the following commands:
+
+- Run all tests: `pytest`
+- Run Maccor tests: `pytest -m maccor`
+- Run Arbin tests: `pytest -m arbin`
+- Run database specific tests: `pytest -m database`
+- Run tests other than Arbin: `pytest -m "not arbin"`
+- Run Extractor tests: `pytest tests/test_extract_data.py`
+
+To show logs while testing, add the `-o log_cli=true` flag.
+
+## Troubleshooting
+
+### pip install psycopg2 error
+
+If there is an error `Error: pg_config executable not found.` Try installing `libpq-dev` before installing `psycopg2`
+
+```sh
+sudo apt install libpq-dev
+```
```

### Comparing `battetl-1.0.2/README.md` & `battetl-1.1.0/battetl.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,314 +1,358 @@
-<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/BattETL_Logo.png">
-
-# BattETL
-
-BattETL is a well-tested and an enterprise-ready python module for **E**xtracting, **T**ransforming, and **L**oading battery cycler data to a [database](https://github.com/BattGenie/battdb). BattETL can also be used just for data extraction and transformation if a database is not desired. Currently data from Maccor and Arbin cyclers are supported.
-
-<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/BattETL_Simple_System.svg">
-
-## Overview
-
-- [Motivation](#motivation)
-- [Video Guides](#video-guides)
-- [Installation](#installation)
-  - [Requirements](#requirements)
-  - [Installation Instructions](#installation-instructions)
-- [Usage](#usage)
-  - [Config File](#config-file)
-  - [Env File](#env-file)
-  - [Data Export Requirements](#data-export-requirements)
-    - [Maccor](#maccor)
-    - [Arbin](#arbin)
-- [BattETL Overview](#battetl-overview)
-  - [System Diagram](#system-diagram)
-  - [Transformer](#transformer)
-  - [Extractor](#extractor)
-  - [Loader](#loader)
-- [Testing](#testing)
-- [Troubleshooting](#troubleshooting)
-
-## Motivation
-
-### Why another battery cycler data ingesting tool?
-
-There are published [open](https://github.com/TRI-AMDD/beep) [source](https://github.com/Battery-Intelligence-Lab/galvanalyser) solutions for battery cycler data ingestion. BattETL hopes to build on these tools and adds a few conveniences to support robust data management and repeatable data analytics.
-
-### Some features of BattETL
-
-- **A relational data destination.**
-
-BattETL package is tightly coupled to the destination database it sends the data to. BattETL requires that for the battery data that is loaded to the database - the detailed metadata such as battery make and model, cycler make and model, and schedule/procedure information be also included. While these constraints (somewhat) slowdown the data ingestion process, it ensures verifiable, high-quality data persistance.
-
-- **A database that can hold *all* relevant battery test information.**
-
-Not only does the BattETL extract and store all the battery test data, it also captures the cycler schedule/procedure file. In addition to the schedule/procedure file, BattETL captures and stores all files associated with the schedule/procedure. This includes any current profiles (Maccor FastWave or Arbin current simulation files), EIS specifications, or even entire system specifications (Arbin batch files.)
-
-- **Analytics built into the transformation step.**
-
-As part of the transformation step BattETL calculates various cycle statistics (capacity, coulombic efficiency, CC/CV charge times, etc.) providing independent and supplemental cycle statistics to compliment those generated by the cycler software. These can particularly handy when easy-to-miss settings were overlooked in writing the schedule (e.g. forgetting to reset the capacity when incriminating the cycle.) Do you have some sort of hyper-boutique transformation or statistic calculation needed for a specific test? No problem. BattETL can apply user defined transformation functions too; all before the data is loaded to the database.
-
-## Video Guides
-
-The following are video guides BattETL and BattDB:
-
-- [Installation & setup](https://www.youtube.com/watch?v=tmudLhrj9xE)
-- [Design overview](https://www.youtube.com/watch?v=Y2tXInbkYF8)
-- [Demonstration](https://www.youtube.com/watch?v=3wNd3fhqBwo)
-
-## Installation
-
-A video showing how to setup and install BattETL and BattDB can be found [here](https://www.youtube.com/watch?v=tmudLhrj9xE)
-
-### Requirements
-
-#### Software Requirements
-
-- Python 3.9 or 3.10
-- The required packages are listed in the `requirements.txt` file
-
-#### Hardware Requirements
-
-Based on processing approximately 10,000 rows and 12 columns with Pandas, BattETL requires a minimum of 13MB of RAM.
-
-- RAM: 2 GB or higher.
-- Disk Space: At least 2 GB of free space is recommended to accommodate the transformed data, as well as additional space for installation and storing data. The exact amount of disk space required will depend on the size of the data being processed and the resulting intermediate results.
-
-### Installation Instructions
-
-- Install BattETL using pip:
-
-```sh
-pip install battetl
-```
-
-- Install BattETL from source code:
-
-```sh
-git clone https://github.com/BattGenie/battetl.git
-cd battetl
-pip install -r requirements.txt
-pip install .
-```
-
-> Note that if you wish to use the Load feature of BattETL it is necessary to deploy an instance of a [BattDB](https://github.com/BattGenie/battdb) database to load the data to. Follow the instructions there for deploying the database.
-
-## Usage
-
-A video demonstrating how to use BattETL and BattDB can be found [here](https://www.youtube.com/watch?v=3wNd3fhqBwo)
-
-Using BattETL as an all-in-one ETL function is as easy as:
-
-```python
-from battetl import BattETL
-
-cell = BattETL(config_path).extract().transform().load()
-```
-
-Where `config_path` is the absolute or relative path to BattETL [config file](#config-file).
-
-It is also necessary to include an [.env file](#env-file) within the working directory that contains the associated database credentials.
-
-Finally, the data must be exported from the cycler in a [specific format](#data-export-requirements)
-
-For a practical implementation of `BattETL`, please refer to the example notebook `examples/battetl_demo.ipynb` located in the `examples` directory. This notebook demonstrates how to implement `BattETL` and can serve as a useful reference for your own project.
-
-> Note that repeated calls to load test data that already exists in the database (as determined by unix timestamp) will not overwrite any existing data. Only test data after the most recent existing unix timestamp will be loaded. In the case of loading cycle statistics, any duplicate cycles that already exist in the database will be overwritten.
-
-### Config File
-
-To use BattETL it is necessary to provide a path to JSON configuration file. This config file contains paths to the relevant test data files and test metadata used for analysis and establishing database relations. An example configuration file is given within `examples/battetl_config_example.json`
-
-```json
-{
-    "timezone": "America/Los_Angeles",
-    "data_file_path": [
-        "abs/path/to/your/arbin/or/maccor/test/data/file(s).txt"
-    ],
-    "stats_file_path": [
-        "abs/path/to/your/arbin/or/maccor/test/stats/file.txt"
-    ],
-    "schedule_file_path": [
-        "abs/path/to/your/schedule/or/procedure/file(s).000"
-    ],
-    "meta_data": {
-        "test_meta": {
-            "test_name": "the_name_of_your_test",
-            "channel": 10
-        },
-        "cell": {
-            "manufacturer_sn": "0001"
-        },
-        "cell_meta": {
-            "manufacturer": "FakeMN",
-            "manufacturer_pn": "1234"
-        },
-        "schedule_meta": {
-            "schedule_name": "fake_schedule.000",
-            "cycler_make": "BattGenie"
-        },
-        "cycler": {
-            "sn": "0001"
-        },
-        "cycler_meta": {
-            "manufacturer": "BattGenie",
-            "model": "Cycler9000"
-        }
-    }
-}
-```
-
-### Env File
-
-The .env contains the associated database credentials and is formatted as follows
-
-```
-ENV=dev # dev, prod
-DB_TARGET=YOUR_DATABASE_NAME
-DB_USERNAME=YOUR_USERNAME
-DB_PASSWORD=YOUR_PASSWORD
-DB_HOSTNAME=localhost
-DB_PORT=5432
-```
-
-An example .env file is given within `examples/.env.example`
-
-### Data Export Requirements
-
-- [For Maccor Cycler](#maccor)
-- [For Arbin Cycler](#arbin)
-
-#### Maccor
-
-From the "Maccor Export" tool data should be exported as "Text Output" in a "Tab Delimited" format. The output sheets should include "Data Records" and "Cycle Statistics". The box for "Discharge Current Exported Negative" should be checked.
-
-The following columns are the minimum required for export:
-
-For Data Records:
-
-- Cycle : Header Label of Cyc#
-- Step : Header Label of Step
-- Test Time : Header Label of TestTime(s), Units of seconds
-- Step Time : Header Label of StepTime(s), Units of seconds
-- Capacity : Header Label of Capacity(Ah), Units of Amp-Hour
-- Energy : Header Label of Watt-hr, Units of Watt-hour
-- Current : Header Label of Current(A), Units of Amps
-- Voltage : Header Label of Voltage(V), Units of Volts
-- DPT Time : Header label of DPt Time
-
-<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/MaccorExport_DataRecords.png" width="85%" height="50%">
-
-For Cycle Statistics:
-
-- Cycle : Header Label of Cycle
-- Capacity Chg : Header label AH-IN, Units of Ahr
-- Capacity Dis : Header label AH-Out, Units of Ahr
-- DPT Time : Header Label of DPt Time
-
-<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/MaccorExport_CycleStats.png" width="85%" height="50%">
-
-#### Arbin
-
-Within the Arbin Export tool the "File Type" should be set to "To CSV". Within "Data Filter" the box "statistics by Cycle" should be checked along with any other data. For range filter "All" should be selected.
-
-<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/ArbinExport.jpg" width="45%" height="25%">
-
-An example notebook `battetl_demo.ipynb` that provides a tool to help generate config files is located in the `examples` directory.
-
-## BattETL Overview
-
-A video discussing the design of BattDB and BattETL can be found [here](https://www.youtube.com/watch?v=Y2tXInbkYF8)
-
-BattETL bundles together the three independent submodules:
-
-- [Extractor](#extractor) : Responsible for extractor the cycler data and schedule/procedure files.
-- [Transformer](#transformer) : Responsible for transforming cycler data
-- [Loader](#loader) : Responsible for loading data and associated data to the database.
-
-After running BattETL on a specific configuration file the following objects will be available as class variables from the instance:
-
-- `raw_test_data: pandas.DataFrame`: The raw test data exactly as it is in the generated cycler data file(s).
-- `raw_cycle_stats: pandas.DataFrame`: The raw cycle stats data exactly as it is in the generated cycler statistics file.
-- `test_data: pandas.DataFrame`: The transformed test data after normalizing units and datatype and adding a unixtime column.
-- `cycle_stats: pandas.DataFrame`: The transformed cycle stats after normalizing units, datatypes, and calculating supplemental cycle statistics.
-- `schedule: dict`: The procedure/schedule file and all associated files in a nested Dictionary.
-
-### System diagram
-
-<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/BattETL_SystemDiagram.svg">
-
-### Extractor
-
-The Extractor is an interface that allows you to extract battery test data from raw data files. You can extract test data and cycle stats data from multiple files using `data_from_files`, and extract Arbin schedules or Maccor procedures and associated files using `schedule_from_files`.
-
-For an example of the Extractor as a standalone class, see `examples/submodule_demos/Extractor_demo.ipynb`
-
-#### Functions
-
-- `data_from_files(paths: list[str])`: Extracts multiple test data files into a single pandas DataFrame.  
-- `schedule_from_files(paths: list[str])`: Extracts Arbin schedules or Maccor procedures and associated files and stores them in a dictionary.  
-- `from_pickle(path: str)`: Reads data from the passed file path and returns it as a pandas DataFrame.  
-
-#### Variables
-
-- `cycler_make: str`: Cycler make  
-- `raw_test_data_meta_data: list[dict]`: Test data meta data  
-- `raw_cycle_stats_meta_data: list[dict]`: Cycler stats meta data  
-- `raw_test_data: pandas.DataFrame`: Test data  
-- `raw_cycle_stats: pandas.DataFrame`: Cycler stats  
-- `maccor_procedure: dict`: Maccor procedure  
-- `arbin_schedule: dict`: Arbin schedule  
-
-### Transformer
-
-The Transformer is an interface that allows you to transform battery test data to the BattETL schema. By default, the time zone is set to 'America/Los_Angeles', but you can modify it to your preferred time zone using the names found in the [IANA Time Zone Database](https://www.iana.org/time-zones). In addition to the default functions provided by the Transformer, you can add your own custom functions to perform specific transformations on your data.
-
-For an example of the Extractor as a standalone class, see `examples/submodule_demos/Transformer_demo.ipynb`
-
-#### Functions
-
-- `transform_test_data(self, data: pd.DataFrame)`: Transforms test data to conform to BattETL naming and data conventions  
-- `transform_cycle_stats`: Transforms cycle stats to conform to BattETL naming and data conventions  
-
-#### Variables
-
-- `timezone: str`: Time zone strings in the IANA Time Zone Database. Used to convert to unix timestamp in seconds. Default 'America/Los_Angeles'.  
-- `user_transform_test_data`: A user defined function to transform test data. The function should take a pandas.DataFrame as input and return a pandas.DataFrame as output.  
-- `user_transform_cycle_stats`: A user defined function to transform cycle stats. The function should take a pandas.DataFrame as input and return a pandas.DataFrame as output.  
-- `test_data: pandas.DataFrame`: Transformed test data  
-- `cycle_stats: pandas.DataFrame`: Transformed cycle stats  
-
-### Loader
-
-The `load` module provides an interface to load the extracted data into a database.
-
-Note that repeated calls to load test data that already exists in the database (as determined by unix timestamp) will not overwrite any existing data. Only test data after the latest existing unix timestamp will be loaded. In the case of loading cycle statistics, any duplicate cycles that already exist in the database will be overwritten.
-
-For an example of the Extractor as a standalone class, see `examples/submodule_demos/Loader_demo.ipynb`
-
-#### Functions
-
-- `load_test_data(test_data_df)`: Loads test_data_df to `test_data` table in the specified database.  
-- `load_cycle_stats(cycle_stats_df)`: Loads cycle_stats_df to `test_data_cycle_stats` table in the specified database.  
-
-## Testing
-
-To run the test suite, use the following commands:
-
-- Run all tests: `pytest`
-- Run Maccor tests: `pytest -m maccor`
-- Run Arbin tests: `pytest -m arbin`
-- Run database specific tests: `pytest -m database`
-- Run tests other than Arbin: `pytest -m "not arbin"`
-- Run Extractor tests: `pytest tests/test_extract_data.py`
-
-To show logs while testing, add the `-o log_cli=true` flag.
-
-## Troubleshooting
-
-### pip install psycopg2 error
-
-If there is an error `Error: pg_config executable not found.` Try installing `libpq-dev` before installing `psycopg2`
-
-```sh
-sudo apt install libpq-dev
-```
+Metadata-Version: 2.1
+Name: battetl
+Version: 1.1.0
+Summary: A Python module for extracting, transforming, and loading battery data to a database.
+Home-page: https://github.com/BattGenie/battetl
+Author: Zander Nevitt, Bing Syuan Wang, Eric Ravet, and Chintan Pathak
+Author-email: info@battgenie.life
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9, <3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/BattETL_Logo.png">
+
+# BattETL
+
+BattETL is a well-tested and an enterprise-ready python module for **E**xtracting, **T**ransforming, and **L**oading battery cycler data to a [database](https://github.com/BattGenie/battdb). BattETL can also be used just for data extraction and transformation if a database is not desired. Currently data from Maccor and Arbin cyclers are supported.
+
+<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/BattETL_Simple_System.svg">
+
+## Overview
+
+- [Motivation](#motivation)
+- [Video Guides](#video-guides)
+- [Installation](#installation)
+  - [Requirements](#requirements)
+  - [Installation Instructions](#installation-instructions)
+- [Usage](#usage)
+  - [Quick Mode](#quick-mode)
+  - [Config File](#config-file)
+  - [Env File](#env-file)
+  - [Data Export Requirements](#data-export-requirements)
+    - [Maccor](#maccor)
+    - [Arbin](#arbin)
+- [BattETL Overview](#battetl-overview)
+  - [System Diagram](#system-diagram)
+  - [Transformer](#transformer)
+  - [Extractor](#extractor)
+  - [Loader](#loader)
+- [Testing](#testing)
+- [Troubleshooting](#troubleshooting)
+
+## Motivation
+
+### Why another battery cycler data ingesting tool?
+
+There are published [open](https://github.com/TRI-AMDD/beep) [source](https://github.com/Battery-Intelligence-Lab/galvanalyser) solutions for battery cycler data ingestion. BattETL hopes to build on these tools and adds a few conveniences to support robust data management and repeatable data analytics.
+
+### Some features of BattETL
+
+- **A relational data destination.**
+
+BattETL package is tightly coupled to the destination database it sends the data to. BattETL requires that for the battery data that is loaded to the database - the detailed metadata such as battery make and model, cycler make and model, and schedule/procedure information be also included. While these constraints (somewhat) slowdown the data ingestion process, it ensures verifiable, high-quality data persistance.
+
+- **A database that can hold *all* relevant battery test information.**
+
+Not only does the BattETL extract and store all the battery test data, it also captures the cycler schedule/procedure file. In addition to the schedule/procedure file, BattETL captures and stores all files associated with the schedule/procedure. This includes any current profiles (Maccor FastWave or Arbin current simulation files), EIS specifications, or even entire system specifications (Arbin batch files.)
+
+- **Analytics built into the transformation step.**
+
+As part of the transformation step BattETL calculates various cycle statistics (capacity, coulombic efficiency, CC/CV charge times, etc.) providing independent and supplemental cycle statistics to compliment those generated by the cycler software. These can particularly handy when easy-to-miss settings were overlooked in writing the schedule (e.g. forgetting to reset the capacity when incriminating the cycle.) Do you have some sort of hyper-boutique transformation or statistic calculation needed for a specific test? No problem. BattETL can apply user defined transformation functions too; all before the data is loaded to the database.
+
+## Video Guides
+
+The following are video guides BattETL and BattDB:
+
+- [Installation & setup](https://www.youtube.com/watch?v=tmudLhrj9xE)
+- [Design overview](https://www.youtube.com/watch?v=Y2tXInbkYF8)
+- [Demonstration](https://www.youtube.com/watch?v=3wNd3fhqBwo)
+
+## Installation
+
+A video showing how to setup and install BattETL and BattDB can be found [here](https://www.youtube.com/watch?v=tmudLhrj9xE)
+
+### Requirements
+
+#### Software Requirements
+
+- Python 3.9 or 3.10
+- The required packages are listed in the `requirements.txt` file
+
+#### Hardware Requirements
+
+Based on processing approximately 10,000 rows and 12 columns with Pandas, BattETL requires a minimum of 13MB of RAM.
+
+- RAM: 2 GB or higher.
+- Disk Space: At least 2 GB of free space is recommended to accommodate the transformed data, as well as additional space for installation and storing data. The exact amount of disk space required will depend on the size of the data being processed and the resulting intermediate results.
+
+### Installation Instructions
+
+- Install BattETL using pip:
+
+```sh
+pip install battetl
+```
+
+- Install BattETL from source code:
+
+```sh
+git clone https://github.com/BattGenie/battetl.git
+cd battetl
+pip install -r requirements.txt
+pip install .
+```
+
+> Note that if you wish to use the Load feature of BattETL it is necessary to deploy an instance of a [BattDB](https://github.com/BattGenie/battdb) database to load the data to. Follow the instructions there for deploying the database.
+
+## Usage
+
+A video demonstrating how to use BattETL and BattDB can be found [here](https://www.youtube.com/watch?v=3wNd3fhqBwo)
+
+Using BattETL as an all-in-one ETL function is as easy as:
+
+```python
+from battetl import BattETL
+
+cell = BattETL(config_path).extract().transform().load()
+```
+
+Where `config_path` is the absolute or relative path to BattETL [config file](#config-file).
+
+It is also necessary to include an [.env file](#env-file) within the working directory that contains the associated database credentials.
+
+Finally, the data must be exported from the cycler in a [specific format](#data-export-requirements)
+
+For a practical implementation of `BattETL`, please refer to the example notebook `examples/battetl_demo.ipynb` located in the `examples` directory. This notebook demonstrates how to implement `BattETL` and can serve as a useful reference for your own project.
+
+> Note that repeated calls to load test data that already exists in the database (as determined by unix timestamp) will not overwrite any existing data. Only test data after the most recent existing unix timestamp will be loaded. In the case of loading cycle statistics, any duplicate cycles that already exist in the database will be overwritten.
+
+### Quick Mode
+
+BattETL provides a Quick Mode, which automatically detects whether the given file is test data or test stats from a Maccor or an Arbin cycler, and uploads it to the database accordingly. Here's an example command line:
+
+```bash
+python -m battetl.battetl_quick file="TEST_DATA.txt" db_url="postgres://postgres:password@localhost:5454/battdb_quick"
+```
+
+This command relies on [BattDB](https://github.com/BattGenie/BattDB). If BattDB does not exist, a database will be created using Docker Compose and the data will be uploaded to it. The command also returns a harmonized Pandas dataframe that can be used for analysis and visualization. 
+
+### Config File
+
+To use BattETL it is necessary to provide a path to JSON configuration file. This config file contains paths to the relevant test data files and test metadata used for analysis and establishing database relations. An example configuration file is given within `examples/battetl_config_example.json`
+
+```json
+{
+    "timezone": "America/Los_Angeles",
+    "data_file_path": [
+        "abs/path/to/your/arbin/or/maccor/test/data/file(s).txt"
+    ],
+    "stats_file_path": [
+        "abs/path/to/your/arbin/or/maccor/test/stats/file.txt"
+    ],
+    "schedule_file_path": [
+        "abs/path/to/your/schedule/or/procedure/file(s).000"
+    ],
+    "meta_data": {
+        "test_meta": {
+            "test_name": "the_name_of_your_test",
+            "channel": 10
+        },
+        "cell": {
+            "manufacturer_sn": "0001"
+        },
+        "cell_meta": {
+            "manufacturer": "FakeMN",
+            "manufacturer_pn": "1234"
+        },
+        "schedule_meta": {
+            "schedule_name": "fake_schedule.000",
+            "cycler_make": "BattGenie"
+        },
+        "cycler": {
+            "sn": "0001"
+        },
+        "cycler_meta": {
+            "manufacturer": "BattGenie",
+            "model": "Cycler9000"
+        },
+        "customers": {
+            "customer_name": "FakeCustomer"
+        },
+        "projects": {
+            "project_name": "FakeProject"
+        }
+    }
+}
+```
+
+#### Cell Thermocouple (optional)
+
+If the cell has a thermocouple, it is necessary to include the following in the header of the config file:
+
+```json
+"cell_thermocouple": 1
+```
+
+where `1` corresponds to the thermocouple index in the cycler test data export, i.e `Temp 1` for Maccor and `Aux_Temperature_1 (C)` for Arbin.
+
+If no cell thermocouple value is listed, `calculated_max_charge_temp_c` and `calculated_max_discharge_temp_c` will be set to `null` in the `test_data_cycle_stats` table.
+
+### Env File
+
+The .env contains the associated database credentials and is formatted as follows
+
+```text
+ENV=dev # dev, prod
+DB_TARGET=YOUR_DATABASE_NAME
+DB_USERNAME=YOUR_USERNAME
+DB_PASSWORD=YOUR_PASSWORD
+DB_HOSTNAME=localhost
+DB_PORT=5432
+```
+
+An example .env file is given within `examples/.env.example`
+
+### Data Export Requirements
+
+- [For Maccor Cycler](#maccor)
+- [For Arbin Cycler](#arbin)
+
+#### Maccor
+
+From the "Maccor Export" tool data should be exported as "Text Output" in a "Tab Delimited" format. The output sheets should include "Data Records" and "Cycle Statistics". The box for "Discharge Current Exported Negative" should be checked.
+
+The following columns are the minimum required for export:
+
+For Data Records:
+
+- Cycle : Header Label of Cyc#
+- Step : Header Label of Step
+- Test Time : Header Label of TestTime(s), Units of seconds
+- Step Time : Header Label of StepTime(s), Units of seconds
+- Capacity : Header Label of Capacity(Ah), Units of Amp-Hour
+- Energy : Header Label of Watt-hr, Units of Watt-hour
+- Current : Header Label of Current(A), Units of Amps
+- Voltage : Header Label of Voltage(V), Units of Volts
+- DPT Time : Header label of DPt Time
+
+<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/MaccorExport_DataRecords.png" width="85%" height="50%">
+
+For Cycle Statistics:
+
+- Cycle : Header Label of Cycle
+- Capacity Chg : Header label AH-IN, Units of Ahr
+- Capacity Dis : Header label AH-Out, Units of Ahr
+- DPT Time : Header Label of DPt Time
+
+<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/MaccorExport_CycleStats.png" width="85%" height="50%">
+
+#### Arbin
+
+Within the Arbin Export tool the "File Type" should be set to "To CSV". Within "Data Filter" the box "statistics by Cycle" should be checked along with any other data. For range filter "All" should be selected.
+
+<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/ArbinExport.jpg" width="45%" height="25%">
+
+An example notebook `battetl_demo.ipynb` that provides a tool to help generate config files is located in the `examples` directory.
+
+## BattETL Overview
+
+A video discussing the design of BattDB and BattETL can be found [here](https://www.youtube.com/watch?v=Y2tXInbkYF8)
+
+BattETL bundles together the three independent submodules:
+
+- [Extractor](#extractor) : Responsible for extractor the cycler data and schedule/procedure files.
+- [Transformer](#transformer) : Responsible for transforming cycler data
+- [Loader](#loader) : Responsible for loading data and associated data to the database.
+
+After running BattETL on a specific configuration file the following objects will be available as class variables from the instance:
+
+- `raw_test_data: pandas.DataFrame`: The raw test data exactly as it is in the generated cycler data file(s).
+- `raw_cycle_stats: pandas.DataFrame`: The raw cycle stats data exactly as it is in the generated cycler statistics file.
+- `test_data: pandas.DataFrame`: The transformed test data after normalizing units and datatype and adding a unixtime column.
+- `cycle_stats: pandas.DataFrame`: The transformed cycle stats after normalizing units, datatypes, and calculating supplemental cycle statistics.
+- `schedule: dict`: The procedure/schedule file and all associated files in a nested Dictionary.
+
+### System diagram
+
+<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/BattETL_SystemDiagram.svg">
+
+### Extractor
+
+The Extractor is an interface that allows you to extract battery test data from raw data files. You can extract test data and cycle stats data from multiple files using `data_from_files`, and extract Arbin schedules or Maccor procedures and associated files using `schedule_from_files`.
+
+For an example of the Extractor as a standalone class, see `examples/submodule_demos/Extractor_demo.ipynb`
+
+#### Functions
+
+- `data_from_files(paths: list[str])`: Extracts multiple test data files into a single pandas DataFrame.  
+- `schedule_from_files(paths: list[str])`: Extracts Arbin schedules or Maccor procedures and associated files and stores them in a dictionary.  
+- `from_pickle(path: str)`: Reads data from the passed file path and returns it as a pandas DataFrame.  
+
+#### Variables
+
+- `cycler_make: str`: Cycler make  
+- `raw_test_data_meta_data: list[dict]`: Test data meta data  
+- `raw_cycle_stats_meta_data: list[dict]`: Cycler stats meta data  
+- `raw_test_data: pandas.DataFrame`: Test data  
+- `raw_cycle_stats: pandas.DataFrame`: Cycler stats  
+- `maccor_procedure: dict`: Maccor procedure  
+- `arbin_schedule: dict`: Arbin schedule  
+
+### Transformer
+
+The Transformer is an interface that allows you to transform battery test data to the BattETL schema. By default, the time zone is set to 'America/Los_Angeles', but you can modify it to your preferred time zone using the names found in the [IANA Time Zone Database](https://www.iana.org/time-zones). In addition to the default functions provided by the Transformer, you can add your own custom functions to perform specific transformations on your data.
+
+For an example of the Extractor as a standalone class, see `examples/submodule_demos/Transformer_demo.ipynb`
+
+#### Functions
+
+- `transform_test_data(self, data: pd.DataFrame)`: Transforms test data to conform to BattETL naming and data conventions  
+- `transform_cycle_stats`: Transforms cycle stats to conform to BattETL naming and data conventions  
+
+#### Variables
+
+- `timezone: str`: Time zone strings in the IANA Time Zone Database. Used to convert to unix timestamp in seconds. Default 'America/Los_Angeles'.  
+- `user_transform_test_data`: A user defined function to transform test data. The function should take a pandas.DataFrame as input and return a pandas.DataFrame as output.  
+- `user_transform_cycle_stats`: A user defined function to transform cycle stats. The function should take a pandas.DataFrame as input and return a pandas.DataFrame as output.  
+- `test_data: pandas.DataFrame`: Transformed test data  
+- `cycle_stats: pandas.DataFrame`: Transformed cycle stats  
+
+### Loader
+
+The `load` module provides an interface to load the extracted data into a database.
+
+Note that repeated calls to load test data that already exists in the database (as determined by unix timestamp) will not overwrite any existing data. Only test data after the latest existing unix timestamp will be loaded. In the case of loading cycle statistics, any duplicate cycles that already exist in the database will be overwritten.
+
+For an example of the Extractor as a standalone class, see `examples/submodule_demos/Loader_demo.ipynb`
+
+#### Functions
+
+- `load_test_data(test_data_df)`: Loads test_data_df to `test_data` table in the specified database.  
+- `load_cycle_stats(cycle_stats_df)`: Loads cycle_stats_df to `test_data_cycle_stats` table in the specified database.  
+
+## Testing
+
+To run the test suite, use the following commands:
+
+- Run all tests: `pytest`
+- Run Maccor tests: `pytest -m maccor`
+- Run Arbin tests: `pytest -m arbin`
+- Run database specific tests: `pytest -m database`
+- Run tests other than Arbin: `pytest -m "not arbin"`
+- Run Extractor tests: `pytest tests/test_extract_data.py`
+
+To show logs while testing, add the `-o log_cli=true` flag.
+
+## Troubleshooting
+
+### pip install psycopg2 error
+
+If there is an error `Error: pg_config executable not found.` Try installing `libpq-dev` before installing `psycopg2`
+
+```sh
+sudo apt install libpq-dev
+```
```

### Comparing `battetl-1.0.2/battetl/constants.py` & `battetl-1.1.0/battetl/constants.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,242 +1,287 @@
-class Constants:
-    DEFAULT_TIME_ZONE = 'America/Los_Angeles'
-
-    DATABASE_MAX_RETRIES = 10
-    DATABASE_RETRY_DELAY = 10
-    DATABASE_MAX_RETRY_DELAY = 60
-
-    MAKE_ARBIN = 'arbin'
-    MAKE_MACCOR = 'maccor'
-    DATA_TYPE_TEST_DATA = 'test_data'
-    DATA_TYPE_CYCLE_STATS = 'cycle_stats'
-
-    MACCOR_PROCEDURE_FILE_ENCODING = 'UTF-8'
-
-    MACCOR_CHARGE_STEP_NAMES = ['Charge', 'Chg Func', 'FastWave']
-    # Yes, discharge is actually misspelled in the extract procedure files
-    MACCOR_DISCHARGE_STEP_NAMES = ['Dischrge', 'Dis Func']
-
-    ARBIN_SCHEDULE_FILE_ENCODING = 'latin-1'
-
-    PREFIX_ARBIN_THERMOCOUPLE = 'aux_temperature_'
-    PREFIX_MACCOR_THERMOCOUPLE = 'temp '
-    TEMPLATE_RENAMED_THERMOCOUPLE = 'thermocouple_X_c'
-
-    COLUMNS_TEST_DATA = {
-        'test_data_id',
-        'test_id',
-        'cycle',
-        'step',
-        'test_time_s',
-        'step_time_s',
-        'current_ma',
-        'voltage_mv',
-        'recorded_datetime',
-        'unixtime_s',
-        'thermocouple_temp_c',
-        'other_details',
-    }
-    COLUMNS_CYCLE_STATS = {
-        'cycle_stats_id',
-        'test_id',
-        'cycle',
-        'test_time_s',
-        'reported_charge_capacity_mah',
-        'reported_discharge_capacity_mah',
-        'reported_charge_energy_mwh',
-        'reported_discharge_energy_mwh',
-        'reported_charge_time_s',
-        'reported_discharge_time_s',
-        'calculated_charge_capacity_mah',
-        'calculated_max_charge_temp_c',
-        'calculated_discharge_capacity_mah',
-        'calculated_max_discharge_temp_c',
-        'calculated_cc_charge_time_s',
-        'calculated_cv_charge_time_s',
-        'calculated_cc_capacity_mah',
-        'calculated_cv_capacity_mah',
-        'reported_coulombic_efficiency',
-        'calculated_coulombic_efficiency',
-        'calculated_fifty_percent_charge_time_s',
-        'calculated_eighty_percent_charge_time_s',
-        'calculated_charge_energy_mwh',
-        'calculated_discharge_energy_mwh',
-        'other_details',
-    }
-    COLUMNS_ARBIN_TEST_DATA_ONLY = {
-        'Date Time',
-        'ACR (Ohm)',
-        'dQ/dV (Ah/V)',
-        'Internal Resistance (Ohm)',
-        'dV/dQ (V/Ah)',
-        'dV/dt (V/s)',
-        'Data Point',
-    }
-    COLUMNS_ARBIN_CYCLE_STATS_ONLY = {
-        'Charge Time (s)',
-        'Date_Time',
-        'mAh/g',
-        'Coulombic Efficiency (%)',
-        'V_Max_On_Cycle (V)',
-        'Discharge Time (s)',
-    }
-    COLUMNS_MACCOR_TEST_DATA_ONLY = {
-        'Cyc#',
-        'StepTime(s)',
-        'DPt Time',
-        'Current(A)',
-        'Capacity(Ah)',
-        'Step',
-        'EV Temp',
-        'Voltage(V)',
-        'TestTime(s)',
-        'Temp 1',
-    }
-
-    COLUMNS_MACCOR_TEST_DATA_TYPE2_ONLY = {
-        'Rec',
-        'Cycle P',
-        'Cycle C',
-        'Capacity',
-        'Energy',
-        'MD',
-        'ES',
-        'DPT Time',
-    }
-
-    COLUMNS_MACCOR_CYCLE_STATS_ONLY = {
-        'T1_End',
-        'T1_Max',
-        'T1_Start',
-        'T1_Min',
-        'Cycle',
-        'Date',
-        'AH-OUT',
-        'AH-IN',
-    }
-
-    COLUMNS_TO_MILLI = {
-        # Test Data
-        'voltage_v': 'voltage_mv',
-        'current_a': 'current_ma',
-        'voltage': 'voltage_mv',
-        'current': 'current_ma',
-        'charge_capacity_ah': 'charge_capacity_mah',
-        'discharge_capacity_ah': 'discharge_capacity_mah',
-        'charge_energy_wh': 'charge_energy_mwh',
-        'discharge_energy_wh': 'discharge_energy_mwh',
-        'power_w': 'power_mw',
-        'impedance_ohm': 'impedance_mohm',
-        'capacity_ah': 'capacity_mah',
-        # Arbin Test Data
-        'arbin_charge_capacity_ah': 'arbin_charge_capacity_mah',
-        'arbin_discharge_capacity_ah': 'arbin_discharge_capacity_mah',
-        'arbin_charge_energy_wh': 'arbin_charge_energy_mwh',
-        'arbin_discharge_energy_wh': 'arbin_discharge_energy_mwh',
-        # Maccor Test Data
-        'maccor_capacity_ah': 'maccor_capacity_mah',
-        'maccor_energy_wh': 'maccor_energy_mwh',
-        'capacity': 'maccor_capacity_mah',
-        'energy': 'maccor_energy_mwh',
-        # Arbin Cycle Stats
-        'reported_charge_capacity_ah': 'reported_charge_capacity_mah',
-        'reported_discharge_capacity_ah': 'reported_discharge_capacity_mah',
-        'reported_charge_energy_wh': 'reported_charge_energy_mwh',
-        'reported_discharge_energy_wh': 'reported_discharge_energy_mwh',
-    }
-
-    COLUMNS_MAPPING_ARBIN_TEST_DATA = {
-        'Date_Time': 'recorded_datetime',
-        'Internal Resistance (Ohm)': 'impedance_ohm',
-        'Date_Time': 'recorded_datetime',
-        'Date Time': 'recorded_datetime',
-        'Data Point': 'data_point',
-        'Test Time (s)': 'test_time_s',
-        'Test Time(s)': 'test_time_s',
-        'Test_Time(s)': 'test_time_s',
-        'Step Time (s)': 'step_time_s',
-        'Step_Time(s)': 'step_time_s',
-        'Step Time(s)': 'step_time_s',
-        'Cycle Index': 'cycle',
-        'Cycle_Index': 'cycle',
-        'Step Index': 'step',
-        'Step_Index': 'step',
-        'TC_Counter1': 'tc_counter1',
-        'Voltage (V)': 'voltage_v',
-        'Voltage(V)': 'voltage_v',
-        'Current (A)': 'current_a',
-        'Current(A)': 'current_a',
-        'Charge Capacity (Ah)': 'arbin_charge_capacity_ah',
-        'Charge Capacity(Ah)': 'arbin_charge_capacity_ah',
-        'Charge_Capacity(Ah)': 'arbin_charge_capacity_ah',
-        'Discharge Capacity (Ah)': 'arbin_discharge_capacity_ah',
-        'Discharge Capacity(Ah)': 'arbin_discharge_capacity_ah',
-        'Discharge_Capacity(Ah)': 'arbin_discharge_capacity_ah',
-        'Charge Energy (Wh)': 'arbin_charge_energy_wh',
-        'Charge_Energy (Wh)': 'arbin_charge_energy_wh',
-        'Charge_Energy(Wh)': 'arbin_charge_energy_wh',
-        'Discharge Energy (Wh)': 'arbin_discharge_energy_wh',
-        'Discharge Energy(Wh)': 'arbin_discharge_energy_wh',
-        'Discharge_Energy(Wh)': 'arbin_discharge_energy_wh',
-        'Power (W)': 'power_w',
-    }
-    COLUMNS_MAPPING_ARBIN_CYCLE_STATS = {
-        'Date_Time': 'recorded_datetime',
-        'Test Time (s)': 'test_time_s',
-        'Test Time(s)': 'test_time_s',
-        'Step Time (s)': 'step_time_s',
-        'Step Time(s)': 'step_time_s',
-        'Cycle Index': 'cycle',
-        'Step Index': 'step',
-        'TC_Counter1': 'tc_counter1',
-        'Voltage(V)': 'voltage_v',
-        'Voltage (V)': 'voltage_v',
-        'Current (A)': 'current_a',
-        'Current(A)': 'current_a',
-        'Charge Capacity (Ah)': 'reported_charge_capacity_ah',
-        'Charge Capacity(Ah)': 'reported_charge_capacity_ah',
-        'Discharge Capacity (Ah)': 'reported_discharge_capacity_ah',
-        'Discharge Capacity(Ah)': 'reported_discharge_capacity_ah',
-        'Charge Time (s)': 'reported_charge_time_s',
-        'Charge Time(s)': 'reported_charge_time_s',
-        'Discharge Time (s)': 'reported_discharge_time_s',
-        'Coulombic Efficiency (%)': 'reported_coulombic_efficiency',
-        'Charge Energy (Wh)': 'reported_charge_energy_wh',
-        'Charge_Energy(Wh)': 'reported_charge_energy_wh',
-        'Discharge Energy (Wh)': 'reported_discharge_energy_wh',
-        'Discharge Energy(Wh)': 'reported_discharge_energy_wh',
-    }
-    COLUMNS_MAPPING_MACCOR_TEST_DATA = {
-        'Cyc#': 'cycle',
-        'Cycle P': 'cycle',
-        'Step': 'step',
-        'TestTime(s)': 'test_time_s',
-        'Test Time': 'test_time_s',
-        'StepTime(s)': 'step_time_s',
-        'Step Time': 'step_time_s',
-        'Capacity(Ah)': 'maccor_capacity_ah',
-        'Watt-hr': 'maccor_energy_wh',
-        'Current(A)': 'current_a',
-        'Voltage(V)': 'voltage_v',
-        'DPt Time': 'recorded_datetime',
-        'EV Temp': 'ev_temp_c',
-    }
-    COLUMNS_MAPPING_MACCOR_CYCLE_STATS = {
-        'Cycle': 'cycle',
-        'Test Time': 'test_time_s',
-        'Current': 'maccor_min_current_ma',
-        'Voltage': 'maccor_min_voltage_mv',
-        'AH-IN': 'reported_charge_capacity_ah',
-        'AH-OUT': 'reported_discharge_capacity_ah',
-        'WH-IN': 'reported_charge_energy_wh',
-        'WH-OUT': 'reported_discharge_energy_wh',
-        'T1_Start': 'maccor_charge_thermocouple_start_c',
-        'T1_End': 'maccor_charge_thermocouple_end_c',
-        'T1_Min': 'maccor_charge_thermocouple_min_c',
-        'T1_Max': 'maccor_charge_thermocouple_max_c',
-        'T1_Start.1': 'maccor_discharge_thermocouple_start_c',
-        'T1_End.1': 'maccor_discharge_thermocouple_end_c',
-        'T1_Min.1': 'maccor_discharge_thermocouple_min_c',
-        'T1_Max.1': 'maccor_discharge_thermocouple_max_c',
-        'ACR': 'acr_ohm',
-    }
+class Constants:
+    DEFAULT_TIME_ZONE = 'America/Los_Angeles'
+
+    DATABASE_MAX_RETRIES = 10
+    DATABASE_RETRY_DELAY = 10
+    DATABASE_MAX_RETRY_DELAY = 60
+
+    MAKE_ARBIN = 'arbin'
+    MAKE_MACCOR = 'maccor'
+    DATA_TYPE_TEST_DATA = 'test_data'
+    DATA_TYPE_CYCLE_STATS = 'cycle_stats'
+
+    MACCOR_PROCEDURE_FILE_ENCODING = 'UTF-8'
+
+    MACCOR_CHARGE_STEP_NAMES = ['Charge', 'Chg Func', 'FastWave']
+    # Yes, discharge is actually misspelled in the extract procedure files
+    MACCOR_DISCHARGE_STEP_NAMES = ['Dischrge', 'Dis Func']
+
+    ARBIN_SCHEDULE_FILE_ENCODING = 'latin-1'
+
+    PREFIX_ARBIN_THERMOCOUPLE = 'aux_temperature_'
+    PREFIX_MACCOR_THERMOCOUPLE = 'temp '
+    TEMPLATE_RENAMED_THERMOCOUPLE = 'thermocouple_X_c'
+
+    COLUMNS_TEST_DATA = {
+        'test_data_id',
+        'test_id',
+        'cycle',
+        'step',
+        'test_time_s',
+        'step_time_s',
+        'current_ma',
+        'voltage_mv',
+        'recorded_datetime',
+        'unixtime_s',
+        'thermocouple_temps_c',
+        'other_details',
+    }
+    COLUMNS_CYCLE_STATS = {
+        'cycle_stats_id',
+        'test_id',
+        'cycle',
+        'test_time_s',
+        'reported_charge_capacity_mah',
+        'reported_discharge_capacity_mah',
+        'reported_charge_energy_mwh',
+        'reported_discharge_energy_mwh',
+        'reported_charge_time_s',
+        'reported_discharge_time_s',
+        'calculated_charge_capacity_mah',
+        'calculated_max_charge_temp_c',
+        'calculated_discharge_capacity_mah',
+        'calculated_max_discharge_temp_c',
+        'calculated_cc_charge_time_s',
+        'calculated_cv_charge_time_s',
+        'calculated_cc_capacity_mah',
+        'calculated_cv_capacity_mah',
+        'reported_coulombic_efficiency',
+        'calculated_coulombic_efficiency',
+        'calculated_fifty_percent_charge_time_s',
+        'calculated_eighty_percent_charge_time_s',
+        'calculated_charge_energy_mwh',
+        'calculated_discharge_energy_mwh',
+        'other_details',
+    }
+    COLUMNS_ARBIN_TEST_DATA_ONLY = {
+        'Date Time',
+        'ACR (Ohm)',
+        'dQ/dV (Ah/V)',
+        'Internal Resistance (Ohm)',
+        'dV/dQ (V/Ah)',
+        'dV/dt (V/s)',
+        'Data Point',
+    }
+    COLUMNS_ARBIN_CYCLE_STATS_ONLY = {
+        'Charge Time (s)',
+        'Date_Time',
+        'mAh/g',
+        'Coulombic Efficiency (%)',
+        'V_Max_On_Cycle (V)',
+        'Discharge Time (s)',
+    }
+    COLUMNS_MACCOR_TEST_DATA_ONLY = {
+        'Cyc#',
+        'StepTime(s)',
+        'DPt Time',
+        'Current(A)',
+        'Capacity(Ah)',
+        'Step',
+        'EV Temp',
+        'Voltage(V)',
+        'TestTime(s)',
+        'Temp 1',
+    }
+
+    COLUMNS_MACCOR_TEST_DATA_TYPE2_ONLY = {
+        'Rec',
+        'Cycle P',
+        'Cycle C',
+        'Capacity',
+        'Energy',
+        'MD',
+        'ES',
+        'DPT Time',
+    }
+
+    COLUMNS_MACCOR_CYCLE_STATS_ONLY = {
+        'T1_End',
+        'T1_Max',
+        'T1_Start',
+        'T1_Min',
+        'Cycle',
+        'Date',
+        'AH-OUT',
+        'AH-IN',
+    }
+
+    COLUMNS_MACCOR_CYCLE_STATS_CUSTOMER1 = {
+        'Cycle',
+        'AH-IN',
+        'AH-OUT',
+        'T1_Start',
+        'T1_End',
+        'T1_Min',
+        'T1_Max',
+        'T1_Start',
+        'T1_End',
+        'T1_Min',
+        'T1_Max',
+        'Date',
+    }
+
+    COLUMNS_MACCOR_TEST_DATA_CUSTOMER1 = {
+        'Cyc#',
+        'Step',
+        'TestTime(s)',
+        'StepTime(s)',
+        'Capacity(Ah)',
+        'Watt-hr',
+        'Current(A)'
+        'Voltage(V)',
+        'ES',
+        'DPt Time',
+        'Volt 1',
+        'ManufacturerAccess (0x00)',
+        'AtRate (0x02)',
+        'AtRateTimeToEmpty (0x04)',
+        'Temperature (0x06)',
+        'Voltage (0x08)',
+        'BatteryStatus (0x0A)',
+        'Current (0x0C)',
+        'RemainingCapacity (0x10)',
+        'FullChargeCapacity (0x12)',
+        'AverageCurrent (0x14)',
+        'AverageTimeToEmpty (0x16)',
+        'AverageTimeToFull (0x18)',
+        'RelativeStateOfCharge (0x2C)',
+        'ChargingVoltage (0x30)',
+        'ChargingCurrent (0x32)',
+        'DesignCapacity (0x3C)',
+    }
+
+    COLUMNS_TO_MILLI = {
+        # Test Data
+        'voltage_v': 'voltage_mv',
+        'current_a': 'current_ma',
+        'voltage': 'voltage_mv',
+        'current': 'current_ma',
+        'charge_capacity_ah': 'charge_capacity_mah',
+        'discharge_capacity_ah': 'discharge_capacity_mah',
+        'charge_energy_wh': 'charge_energy_mwh',
+        'discharge_energy_wh': 'discharge_energy_mwh',
+        'power_w': 'power_mw',
+        'impedance_ohm': 'impedance_mohm',
+        'capacity_ah': 'capacity_mah',
+        # Arbin Test Data
+        'arbin_charge_capacity_ah': 'arbin_charge_capacity_mah',
+        'arbin_discharge_capacity_ah': 'arbin_discharge_capacity_mah',
+        'arbin_charge_energy_wh': 'arbin_charge_energy_mwh',
+        'arbin_discharge_energy_wh': 'arbin_discharge_energy_mwh',
+        # Maccor Test Data
+        'maccor_capacity_ah': 'maccor_capacity_mah',
+        'maccor_energy_wh': 'maccor_energy_mwh',
+        'capacity': 'maccor_capacity_mah',
+        'energy': 'maccor_energy_mwh',
+        # Arbin Cycle Stats
+        'reported_charge_capacity_ah': 'reported_charge_capacity_mah',
+        'reported_discharge_capacity_ah': 'reported_discharge_capacity_mah',
+        'reported_charge_energy_wh': 'reported_charge_energy_mwh',
+        'reported_discharge_energy_wh': 'reported_discharge_energy_mwh',
+    }
+
+    COLUMNS_MAPPING_ARBIN_TEST_DATA = {
+        'Date_Time': 'recorded_datetime',
+        'Internal Resistance (Ohm)': 'impedance_ohm',
+        'Date_Time': 'recorded_datetime',
+        'Date Time': 'recorded_datetime',
+        'Data Point': 'data_point',
+        'Test Time (s)': 'test_time_s',
+        'Test Time(s)': 'test_time_s',
+        'Test_Time(s)': 'test_time_s',
+        'Step Time (s)': 'step_time_s',
+        'Step_Time(s)': 'step_time_s',
+        'Step Time(s)': 'step_time_s',
+        'Cycle Index': 'cycle',
+        'Cycle_Index': 'cycle',
+        'Step Index': 'step',
+        'Step_Index': 'step',
+        'TC_Counter1': 'tc_counter1',
+        'Voltage (V)': 'voltage_v',
+        'Voltage(V)': 'voltage_v',
+        'Current (A)': 'current_a',
+        'Current(A)': 'current_a',
+        'Charge Capacity (Ah)': 'arbin_charge_capacity_ah',
+        'Charge Capacity(Ah)': 'arbin_charge_capacity_ah',
+        'Charge_Capacity(Ah)': 'arbin_charge_capacity_ah',
+        'Discharge Capacity (Ah)': 'arbin_discharge_capacity_ah',
+        'Discharge Capacity(Ah)': 'arbin_discharge_capacity_ah',
+        'Discharge_Capacity(Ah)': 'arbin_discharge_capacity_ah',
+        'Charge Energy (Wh)': 'arbin_charge_energy_wh',
+        'Charge_Energy (Wh)': 'arbin_charge_energy_wh',
+        'Charge_Energy(Wh)': 'arbin_charge_energy_wh',
+        'Discharge Energy (Wh)': 'arbin_discharge_energy_wh',
+        'Discharge Energy(Wh)': 'arbin_discharge_energy_wh',
+        'Discharge_Energy(Wh)': 'arbin_discharge_energy_wh',
+        'Power (W)': 'power_w',
+    }
+    COLUMNS_MAPPING_ARBIN_CYCLE_STATS = {
+        'Date_Time': 'recorded_datetime',
+        'Test Time (s)': 'test_time_s',
+        'Test Time(s)': 'test_time_s',
+        'Step Time (s)': 'step_time_s',
+        'Step Time(s)': 'step_time_s',
+        'Cycle Index': 'cycle',
+        'Step Index': 'step',
+        'TC_Counter1': 'tc_counter1',
+        'Voltage(V)': 'voltage_v',
+        'Voltage (V)': 'voltage_v',
+        'Current (A)': 'current_a',
+        'Current(A)': 'current_a',
+        'Charge Capacity (Ah)': 'reported_charge_capacity_ah',
+        'Charge Capacity(Ah)': 'reported_charge_capacity_ah',
+        'Discharge Capacity (Ah)': 'reported_discharge_capacity_ah',
+        'Discharge Capacity(Ah)': 'reported_discharge_capacity_ah',
+        'Charge Time (s)': 'reported_charge_time_s',
+        'Charge Time(s)': 'reported_charge_time_s',
+        'Discharge Time (s)': 'reported_discharge_time_s',
+        'Coulombic Efficiency (%)': 'reported_coulombic_efficiency',
+        'Charge Energy (Wh)': 'reported_charge_energy_wh',
+        'Charge_Energy(Wh)': 'reported_charge_energy_wh',
+        'Discharge Energy (Wh)': 'reported_discharge_energy_wh',
+        'Discharge Energy(Wh)': 'reported_discharge_energy_wh',
+    }
+    COLUMNS_MAPPING_MACCOR_TEST_DATA = {
+        'Cyc#': 'cycle',
+        'Cycle P': 'cycle',
+        'Step': 'step',
+        'TestTime(s)': 'test_time_s',
+        'Test Time': 'test_time_s',
+        'StepTime(s)': 'step_time_s',
+        'Step Time': 'step_time_s',
+        'Capacity(Ah)': 'maccor_capacity_ah',
+        'Watt-hr': 'maccor_energy_wh',
+        'Current(A)': 'current_a',
+        'Voltage(V)': 'voltage_v',
+        'DPt Time': 'recorded_datetime',
+        'EV Temp': 'ev_temp_c',
+    }
+    COLUMNS_MAPPING_MACCOR_CYCLE_STATS = {
+        'Cycle': 'cycle',
+        'Test Time': 'test_time_s',
+        'Current': 'maccor_min_current_ma',
+        'Voltage': 'maccor_min_voltage_mv',
+        'AH-IN': 'reported_charge_capacity_ah',
+        'AH-OUT': 'reported_discharge_capacity_ah',
+        'WH-IN': 'reported_charge_energy_wh',
+        'WH-OUT': 'reported_discharge_energy_wh',
+        'T1_Start': 'maccor_charge_thermocouple_start_c',
+        'T1_End': 'maccor_charge_thermocouple_end_c',
+        'T1_Min': 'maccor_charge_thermocouple_min_c',
+        'T1_Max': 'maccor_charge_thermocouple_max_c',
+        'T1_Start.1': 'maccor_discharge_thermocouple_start_c',
+        'T1_End.1': 'maccor_discharge_thermocouple_end_c',
+        'T1_Min.1': 'maccor_discharge_thermocouple_min_c',
+        'T1_Max.1': 'maccor_discharge_thermocouple_max_c',
+        'ACR': 'acr_ohm',
+    }
```

### Comparing `battetl-1.0.2/battetl/load/batt_db_test_helper.py` & `battetl-1.1.0/battetl/load/batt_db_test_helper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,197 +1,212 @@
-import pandas as pd
-import random
-import string
-from psycopg2 import sql
-from copy import deepcopy
-
-from .Loader import Loader
-
-
-class BattDbTestHelper(Loader):
-
-    cell_type_id = None
-    cell_id = None
-    cycler_type_id = None
-    cycle_id = None
-    schedule_id = None
-    test_id = None
-
-    def __init__(self, config: dict):
-        '''
-        Various methods to help with tests involving BattDB
-        '''
-        super().__init__(config)
-        self.config = config['meta_data']
-        assert (self._Loader__create_connection())
-
-    def create_test_db_entries(self):
-        '''
-        Creates various entries into the database that the tests assume exist. 
-        Assert to make sure the inserts actually happened. If they fail, then 
-        likely there is data in the database thats needs to be cleared. Easiest course 
-        of action in that case is rebuilding the database from scratch. 
-        '''
-        self.cell_type_id = self._Loader__insert_cell_meta()
-        assert (self.cell_type_id)
-
-        upload_dict = {**self.config['cell'],
-                       **{'cell_type_id': self.cell_type_id}}
-        self.cell_id = self._Loader__perform_insert(
-            target_table='cells', dict_to_load=upload_dict, pk_id_col='cell_id')
-        assert (self.cell_id)
-
-        self.cycler_type_id = self._Loader__perform_insert(
-            target_table='cyclers_meta', dict_to_load=self.config['cycler_meta'], pk_id_col='cycler_type_id')
-        assert (self.cycler_type_id)
-
-        upload_dict = {**self.config['cycler'],
-                       **{'cycler_type_id': self.cycler_type_id}}
-        self.cycler_id = self._Loader__perform_insert(
-            target_table='cyclers', dict_to_load=upload_dict, pk_id_col='cycler_id')
-        assert (self.cycler_id)
-
-        self.schedule_id = self._Loader__perform_insert(
-            target_table='schedule_meta', dict_to_load=self.config['schedule_meta'], pk_id_col='schedule_id')
-        assert (self.schedule_id)
-
-        upload_dict = {**self.config['test_meta'],
-                       **{'cycler_id': self.cycler_id,
-                          'schedule_id': self.schedule_id,
-                          'cell_id': self.cell_id}}
-        self.test_id = self._Loader__perform_insert(
-            target_table='test_meta', dict_to_load=upload_dict, pk_id_col='test_id')
-        assert (self.test_id)
-
-        upload_dict = {'test_id': self.test_id,
-                       'user_id': 'test_helper'}
-        self.sil_id = self._Loader__perform_insert(
-            target_table='sil_meta', dict_to_load=upload_dict, pk_id_col='sil_id')
-        assert (self.test_id)
-
-
-    def read_last_row(self, target_table: str, pk_col_name: str) -> tuple:
-        """
-        Returns the last row in the target_table, sorting off of pk_col_name.
-
-        Parameters
-        ----------
-        target_table : str
-            The table pull the last row from
-        pk_col_name : str
-            The name of the column for the primary key id.
-
-        Returns
-        -------
-        pk_id : int
-            The primary key id for the newly inserted row. Returns None if issue with inserting rows.
-        """
-        with self.conn.cursor() as cursor:
-            stmt = sql.SQL("""
-            SELECT 
-                * 
-            FROM 
-                {table}
-            ORDER BY 
-                {pk_col_name} 
-            DESC LIMIT 1;""").format(
-                table=sql.Identifier(target_table),
-                pk_col_name=sql.Identifier(pk_col_name),
-            )
-            cursor.execute(stmt)
-            last_row = cursor.fetchone()
-
-        return last_row
-
-
-    def load_df_to_db(self, df: pd.DataFrame, target_table: str) -> int:
-        """
-        Loads the passed data frame to the passed target_table in the database
-        specified in the config.
-
-        Parameters
-        ----------
-        df : pd.DataFrame
-            Data frame to load to database.
-        target_table : str
-            Table to load the data frame to.
-
-        Returns
-        -------
-        num_rows_inserted : int
-            The number of rows inserted into the target_table.
-        """
-        return self._Loader__load_dataframe(df, target_table)
-
-    def delete_test_db_entries(self):
-        '''
-        Deletes the test_db entries created in `self.create_test_db_entries`
-        '''
-        self.delete_entry(
-            'sil_meta', 'sil_id', self.sil_id)
-        self.delete_entry(
-            'test_meta', 'test_id', self.test_id)
-        self.delete_entry(
-            'cells', 'cell_id', self.cell_id)
-        self.delete_entry(
-            'cells_meta', 'cell_type_id', self.cell_type_id)
-        self.delete_entry(
-            'cyclers', 'cycler_id', self.cycler_id)
-        self.delete_entry(
-            'cyclers_meta', 'cycler_type_id', self.cycler_type_id)
-        self.delete_entry(
-            'schedule_meta', 'schedule_id', self.schedule_id)
-
-
-    def delete_entry(self, target_table, pk_col_name, pk_id):
-        '''
-        Drops an entry from a meta table.
-
-        Parameters
-        ----------
-        target_table : str
-            The name of the meta table. E.g. "cells_meta"
-        pk_col_name : str
-            The name of the primary key column. E.g. "cell_type_id"
-        pk : int
-            The primary key id number. E.g 1
-        '''
-        with self.conn.cursor() as cursor:
-            stmt = sql.SQL("""
-                DELETE FROM 
-                    {table_name}
-                WHERE 
-                    {pk_col_name} = {pk_id}
-            """).format(
-                table_name=sql.Identifier(target_table),
-                pk_col_name=sql.Identifier(pk_col_name),
-                pk_id=sql.Literal(pk_id)
-            )
-            cursor.execute(stmt)
-
-    def delete_test_data(self):
-        '''
-        Deletes all data from from data tables
-        '''
-        data_to_delete_info = [
-            ('test_data','test_id',self.test_id),
-            ('test_data_cycle_stats','test_id',self.test_id),
-            ('sil_data','sil_id',self.sil_id),
-        ]
-        for data_info in data_to_delete_info:
-            self.delete_entry(data_info[0],data_info[1],data_info[2])
-
-    def generate_random_string(self, len=20) -> str:
-        '''
-        Generates a random string of length `len`.
-
-        Parameters
-        ----------
-        len : int
-            The desired length of the random string
-
-        Returns
-        -------
-        random_string : str
-            A random string of length `len`.
-        '''
-        return (''.join(random.choice(string.ascii_letters) for i in range(len)))
+import pandas as pd
+import random
+import string
+from psycopg2 import sql
+from copy import deepcopy
+
+from .Loader import Loader
+
+
+class BattDbTestHelper(Loader):
+
+    cell_type_id = None
+    cell_id = None
+    cycler_type_id = None
+    cycle_id = None
+    schedule_id = None
+    test_id = None
+    profile_id = None
+    customer_id = None
+
+    def __init__(self, config: dict):
+        '''
+        Various methods to help with tests involving BattDB
+        '''
+        super().__init__(config)
+        self.config = config['meta_data']
+        assert (self._Loader__create_connection())
+
+    def create_test_db_entries(self):
+        '''
+        Creates various entries into the database that the tests assume exist. 
+        Assert to make sure the inserts actually happened. If they fail, then 
+        likely there is data in the database thats needs to be cleared. Easiest course 
+        of action in that case is rebuilding the database from scratch. 
+        '''
+        self.cell_type_id = self._Loader__insert_cell_meta()
+        assert (self.cell_type_id)
+
+        upload_dict = {**self.config['cell'],
+                       **{'cell_type_id': self.cell_type_id}}
+        self.cell_id = self._perform_insert(
+            target_table='cells', dict_to_load=upload_dict, pk_id_col='cell_id')
+        assert (self.cell_id)
+
+        self.cycler_type_id = self._perform_insert(
+            target_table='cyclers_meta', dict_to_load=self.config['cycler_meta'], pk_id_col='cycler_type_id')
+        assert (self.cycler_type_id)
+
+        upload_dict = {**self.config['cycler'],
+                       **{'cycler_type_id': self.cycler_type_id}}
+        self.cycler_id = self._perform_insert(
+            target_table='cyclers', dict_to_load=upload_dict, pk_id_col='cycler_id')
+        assert (self.cycler_id)
+
+        self.schedule_id = self._perform_insert(
+            target_table='schedule_meta', dict_to_load=self.config['schedule_meta'], pk_id_col='schedule_id')
+        assert (self.schedule_id)
+
+        upload_dict = {**self.config['customers']}
+        self.customer_id = self._perform_insert(
+            target_table='customers', dict_to_load=upload_dict, pk_id_col='customer_id')
+        assert (self.customer_id)
+
+        upload_dict = {**self.config['projects'],
+                       'customer_id': self.customer_id}
+        self.project_id = self._perform_insert(
+            target_table='projects', dict_to_load=upload_dict, pk_id_col='project_id')
+        assert (self.project_id)
+
+        upload_dict = {**self.config['test_meta'],
+                       **{'cycler_id': self.cycler_id,
+                          'schedule_id': self.schedule_id,
+                          'cell_id': self.cell_id}}
+        self.test_id = self._perform_insert(
+            target_table='test_meta', dict_to_load=upload_dict, pk_id_col='test_id')
+        assert (self.test_id)
+
+        upload_dict = {'test_id': self.test_id,
+                       'user_id': 'test_helper',
+                       'cell_type_id': self.cell_type_id}
+        self.sil_id = self._perform_insert(
+            target_table='sil_meta', dict_to_load=upload_dict, pk_id_col='sil_id')
+        assert (self.test_id)
+
+    def read_last_row(self, target_table: str, pk_col_name: str) -> tuple:
+        """
+        Returns the last row in the target_table, sorting off of pk_col_name.
+
+        Parameters
+        ----------
+        target_table : str
+            The table pull the last row from
+        pk_col_name : str
+            The name of the column for the primary key id.
+
+        Returns
+        -------
+        pk_id : int
+            The primary key id for the newly inserted row. Returns None if issue with inserting rows.
+        """
+        with self._conn.cursor() as cursor:
+            stmt = sql.SQL("""
+            SELECT 
+                * 
+            FROM 
+                {table}
+            ORDER BY 
+                {pk_col_name} 
+            DESC LIMIT 1;""").format(
+                table=sql.Identifier(target_table),
+                pk_col_name=sql.Identifier(pk_col_name),
+            )
+            cursor.execute(stmt)
+            last_row = cursor.fetchone()
+
+        return last_row
+
+    def load_df_to_db(self, df: pd.DataFrame, target_table: str) -> int:
+        """
+        Loads the passed data frame to the passed target_table in the database
+        specified in the config.
+
+        Parameters
+        ----------
+        df : pd.DataFrame
+            Data frame to load to database.
+        target_table : str
+            Table to load the data frame to.
+
+        Returns
+        -------
+        num_rows_inserted : int
+            The number of rows inserted into the target_table.
+        """
+        return self._load_dataframe(df, target_table)
+
+    def delete_test_db_entries(self):
+        '''
+        Deletes the test_db entries created in `self.create_test_db_entries`
+        '''
+        self.delete_entry(
+            'sil_meta', 'sil_id', self.sil_id)
+        self.delete_entry(
+            'test_meta', 'test_id', self.test_id)
+        self.delete_entry(
+            'cells', 'cell_id', self.cell_id)
+        self.delete_entry(
+            'cells_meta', 'cell_type_id', self.cell_type_id)
+        self.delete_entry(
+            'cyclers', 'cycler_id', self.cycler_id)
+        self.delete_entry(
+            'cyclers_meta', 'cycler_type_id', self.cycler_type_id)
+        self.delete_entry(
+            'schedule_meta', 'schedule_id', self.schedule_id)
+        self.delete_entry(
+            'projects', 'project_id', self.project_id)
+        self.delete_entry(
+            'customers', 'customer_id', self.customer_id)
+
+    def delete_entry(self, target_table, pk_col_name, pk_id):
+        '''
+        Drops an entry from a meta table.
+
+        Parameters
+        ----------
+        target_table : str
+            The name of the meta table. E.g. "cells_meta"
+        pk_col_name : str
+            The name of the primary key column. E.g. "cell_type_id"
+        pk : int
+            The primary key id number. E.g 1
+        '''
+        with self._conn.cursor() as cursor:
+            stmt = sql.SQL("""
+                DELETE FROM 
+                    {table_name}
+                WHERE 
+                    {pk_col_name} = {pk_id}
+            """).format(
+                table_name=sql.Identifier(target_table),
+                pk_col_name=sql.Identifier(pk_col_name),
+                pk_id=sql.Literal(pk_id)
+            )
+            cursor.execute(stmt)
+
+    def delete_test_data(self):
+        '''
+        Deletes all data from from data tables
+        '''
+        data_to_delete_info = [
+            ('test_data', 'test_id', self.test_id),
+            ('test_data_cycle_stats', 'test_id', self.test_id),
+            ('sil_data', 'sil_id', self.sil_id),
+        ]
+        for data_info in data_to_delete_info:
+            self.delete_entry(data_info[0], data_info[1], data_info[2])
+
+    def generate_random_string(self, len=20) -> str:
+        '''
+        Generates a random string of length `len`.
+
+        Parameters
+        ----------
+        len : int
+            The desired length of the random string
+
+        Returns
+        -------
+        random_string : str
+            A random string of length `len`.
+        '''
+        return (''.join(random.choice(string.ascii_letters) for i in range(len)))
```

### Comparing `battetl-1.0.2/battetl/logger.py` & `battetl-1.1.0/battetl/logger.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-"""
-BattETL logger module
-"""
-
-import os
-import logging
-import datetime
-from dotenv import load_dotenv
-from logging.handlers import RotatingFileHandler
-
-load_dotenv()
-
-LOG_MAX_SIZE = 10 * 1024 * 1024  # 10 MB
-STREAM_LOG_MAX_LENGTH = 1000
-MODULE_DIR = os.path.abspath(os.path.dirname(__file__))
-LOG_DIR = os.path.join(MODULE_DIR, "logs")
-if not os.path.isdir(LOG_DIR):
-    os.mkdir(LOG_DIR)
-LOG_FILE_NAME = 'battetl.log'
-LOG_FILE_PATH = os.path.join(LOG_DIR, LOG_FILE_NAME)
-
-# Log format
-# ----------
-# YYYY-MM-DD HH:MM:SS LEVEL [MODULE:LINENO] MESSAGE
-# asctime: Human-readable time when the LogRecord was created.
-# levelname: Text logging level for the message ('DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL').
-# module: The module (name portion of filename).
-# lineno: Source line number where the logging call was issued (if available).
-# message: The logged message.
-logger = logging.getLogger('battetl')
-
-log_format_stream = f'%(asctime)s %(levelname)s [%(module)s:%(lineno)d] %(message).{STREAM_LOG_MAX_LENGTH}s'
-formatter_stream = logging.Formatter(fmt=log_format_stream)
-handler_stream = logging.StreamHandler()
-handler_stream.setFormatter(formatter_stream)
-logger.addHandler(handler_stream)
-
-log_format_file = '%(asctime)s %(levelname)s [%(module)s:%(lineno)d] %(message)s'
-formatter_file = logging.Formatter(fmt=log_format_file)
-handler_file = RotatingFileHandler(
-    LOG_FILE_PATH, maxBytes=LOG_MAX_SIZE, backupCount=10, delay=True)
-handler_file.setFormatter(formatter_file)
-logger.addHandler(handler_file)
-
-
-# Set log level to DEBUG if ENV is dev
-env = os.getenv('ENV')
-if env == 'dev':
-    logger.setLevel(logging.DEBUG)
-else:
-    logger.setLevel(logging.INFO)
+"""
+BattETL logger module
+"""
+
+import os
+import logging
+import datetime
+from dotenv import load_dotenv
+from logging.handlers import RotatingFileHandler
+
+load_dotenv()
+
+LOG_MAX_SIZE = 10 * 1024 * 1024  # 10 MB
+STREAM_LOG_MAX_LENGTH = 1000
+MODULE_DIR = os.path.abspath(os.path.dirname(__file__))
+LOG_DIR = os.path.join(MODULE_DIR, "logs")
+if not os.path.isdir(LOG_DIR):
+    os.mkdir(LOG_DIR)
+LOG_FILE_NAME = 'battetl.log'
+LOG_FILE_PATH = os.path.join(LOG_DIR, LOG_FILE_NAME)
+
+# Log format
+# ----------
+# YYYY-MM-DD HH:MM:SS LEVEL [MODULE:LINENO] MESSAGE
+# asctime: Human-readable time when the LogRecord was created.
+# levelname: Text logging level for the message ('DEBUG', 'INFO', 'WARNING', 'ERROR', 'CRITICAL').
+# module: The module (name portion of filename).
+# lineno: Source line number where the logging call was issued (if available).
+# message: The logged message.
+logger = logging.getLogger('battetl')
+
+log_format_stream = f'%(asctime)s %(levelname)s [%(module)s:%(lineno)d] %(message).{STREAM_LOG_MAX_LENGTH}s'
+formatter_stream = logging.Formatter(fmt=log_format_stream)
+handler_stream = logging.StreamHandler()
+handler_stream.setFormatter(formatter_stream)
+logger.addHandler(handler_stream)
+
+log_format_file = '%(asctime)s %(levelname)s [%(module)s:%(lineno)d] %(message)s'
+formatter_file = logging.Formatter(fmt=log_format_file)
+handler_file = RotatingFileHandler(
+    LOG_FILE_PATH, maxBytes=LOG_MAX_SIZE, backupCount=10, delay=True)
+handler_file.setFormatter(formatter_file)
+logger.addHandler(handler_file)
+
+
+# Set log level to DEBUG if ENV is dev
+env = os.getenv('ENV')
+if env == 'dev':
+    logger.setLevel(logging.DEBUG)
+else:
+    logger.setLevel(logging.INFO)
```

### Comparing `battetl-1.0.2/battetl/transform/Transformer.py` & `battetl-1.1.0/battetl/transform/Transformer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,625 +1,699 @@
-import re
-import numpy as np
-import pandas as pd
-from typing import Callable
-
-from battetl import logger, Constants, Utils
-
-
-class Transformer:
-    def __init__(
-            self,
-            timezone: str = None,
-            user_transform_test_data: Callable[[
-                pd.DataFrame], pd.DataFrame] = None,
-            user_transform_cycle_stats: Callable[[
-                pd.DataFrame], pd.DataFrame] = None) -> None:
-        """
-        An interface to transform battery test data to BattETL schema.
-
-        Parameters
-        ----------
-        timezone : str
-            Time zone strings in the IANA Time Zone Database. Used to convert to unix timestamp
-            in seconds. Default 'America/Los_Angeles'.
-        user_transform_test_data : Callable[[pd.DataFrame], pd.DataFrame], optional
-            A user defined function to transform test data. The function should take a pandas.DataFrame
-            as input and return a pandas.DataFrame as output.
-        user_transform_cycle_stats : Callable[[pd.DataFrame], pd.DataFrame], optional
-            A user defined function to transform cycle stats. The function should take a pandas.DataFrame
-            as input and return a pandas.DataFrame as output.
-        """
-        # Default 'America/Los_Angeles'.
-        self.timezone = timezone if timezone else Constants.DEFAULT_TIME_ZONE
-        self.user_transform_test_data = user_transform_test_data
-        self.user_transform_cycle_stats = user_transform_cycle_stats
-        if self.user_transform_test_data:
-            logger.info('User defined transform_test_data function found')
-        if self.user_transform_cycle_stats:
-            logger.info('User defined transform_cycle_stats function found')
-
-        self.test_data = pd.DataFrame()
-        self.cycle_stats = pd.DataFrame()
-
-    def transform_test_data(self, data: pd.DataFrame) -> pd.DataFrame:
-        """
-        Transforms test data to conform to BattETL naming and data conventions
-
-        Parameters
-        ----------
-        data : pandas.DataFrame
-            The input DataFrame
-        schedule_steps : dict
-            A dictionary containing lists of charge (key->'chg'), discharge (key->'dsg'), and 
-            rest (key->'rst') steps from the schedule used to generate the data. Used to calculate
-            cycle level statistics (e.g. CV charge time.)
-
-        Returns
-        -------
-        df : pandas.DataFrame
-            The transformed output DataFrame
-        """
-        logger.info('Transform test data')
-
-        df = data.copy()
-        df = Utils.drop_unnamed_columns(df)
-
-        cycleMake, dataType = Utils.get_cycle_make(df.columns)
-        logger.info(f'Cycle make: {cycleMake}. Data type: {dataType}')
-
-        if cycleMake == Constants.MAKE_ARBIN and dataType == Constants.DATA_TYPE_TEST_DATA:
-            df = self.__transform_arbin_test_data(df)
-
-        if cycleMake == Constants.MAKE_MACCOR and dataType == Constants.DATA_TYPE_TEST_DATA:
-            df = self.__transform_maccor_test_data(df)
-
-        # Apply user defined transformation
-        if self.user_transform_test_data:
-            df = self.user_transform_test_data(df)
-
-        self.test_data = df
-        return df
-
-    def transform_cycle_stats(self, data: pd.DataFrame):
-        """
-        Transforms cycle stats to conform to BattETL naming and data conventions
-
-        Parameters
-        ----------
-        data : pandas.DataFrame
-            The input DataFrame
-
-        Returns
-        -------
-        df : pandas.DataFrame
-            The transformed output DataFrame
-        """
-        logger.info('Transform cycle stats')
-
-        df = data.copy()
-        df = Utils.drop_unnamed_columns(df)
-
-        cycleMake, dataType = Utils.get_cycle_make(df.columns)
-        logger.info(f'cycle make: {cycleMake}, data type: {dataType}')
-
-        if cycleMake == Constants.MAKE_ARBIN and dataType == Constants.DATA_TYPE_CYCLE_STATS:
-            df = self.__transform_arbin_cycle_stats(df)
-
-        if cycleMake == Constants.MAKE_MACCOR and dataType == Constants.DATA_TYPE_CYCLE_STATS:
-            df = self.__transform_maccor_cycle_stats(df)
-
-        # Apply user defined transformation
-        if self.user_transform_cycle_stats:
-            df = self.user_transform_cycle_stats(df)
-
-        self.cycle_stats = df
-        return df
-
-    def __transform_arbin_test_data(self, df: pd.DataFrame) -> pd.DataFrame:
-        """
-        Transforms Arbin test data to conform to BattETL naming and data conventions
-        1. Rename columns
-        2. Convert to milli
-        3. Convert datetime
-        4. Convert data type
-        5. Sort data
-
-        Parameters
-        ----------
-        df : pandas.DataFrame
-            The input DataFrame
-
-        Returns
-        -------
-        df : pandas.DataFrame
-            The transformed output DataFrame
-        """
-        df = Utils.rename_df_columns(
-            df, Constants.COLUMNS_MAPPING_ARBIN_TEST_DATA)
-        df = Utils.convert_to_milli(df)
-        df = self.__convert_datetime_unixtime(df)
-        df = self.__convert_data_type(df)
-        df = Utils.sort_dataframe(df, ['unixtime_s', 'step'])
-
-        return df
-
-    def __transform_arbin_cycle_stats(self, df: pd.DataFrame) -> pd.DataFrame:
-        """
-        Transforms Arbin cycle stats to conform to BattETL naming and data conventions
-        1. Rename columns
-        2. Convert to milli
-        3. Convert data type
-        4. Sort data
-
-        Parameters
-        ----------
-        df : pandas.DataFrame
-            The input DataFrame
-
-        Returns
-        -------
-        df : pandas.DataFrame
-            The transformed output DataFrame
-        """
-        df = Utils.rename_df_columns(
-            df, Constants.COLUMNS_MAPPING_ARBIN_CYCLE_STATS)
-        df = Utils.convert_to_milli(df)
-        df = self.__convert_data_type(df)
-        df = Utils.sort_dataframe(df, ['cycle'])
-
-        return df
-
-    def __transform_maccor_test_data(self, df: pd.DataFrame) -> pd.DataFrame:
-        """
-        Transforms Maccor test data to conform to BattETL naming and data conventions
-        1. Rename columns
-        2. Convert to milli
-        3. Convert datetime
-        4. Convert data type
-        5. Sort data
-
-        Parameters
-        ----------
-        df : pandas.DataFrame
-            The input DataFrame
-
-        Returns
-        -------
-        df : pandas.DataFrame
-            The transformed output DataFrame
-        """
-        df = Utils.rename_df_columns(
-            df, Constants.COLUMNS_MAPPING_MACCOR_TEST_DATA)
-        df = Utils.convert_to_milli(df)
-        df = self.__convert_datetime_unixtime(df)
-        df = self.__convert_data_type(df)
-
-        if 'test_time_s' in df.columns and len(df) > 0 and self.__timedelta_validation_check(df['test_time_s'][0]):
-            df = Utils.convert_timedelta_to_seconds(df, 'test_time_s')
-        if 'step_time_s' in df.columns and len(df) > 0 and self.__timedelta_validation_check(df['step_time_s'][0]):
-            df = Utils.convert_timedelta_to_seconds(df, 'step_time_s')
-
-        df = Utils.sort_dataframe(df, ['unixtime_s', 'step'])
-
-        return df
-
-    def __transform_maccor_cycle_stats(self, df: pd.DataFrame) -> pd.DataFrame:
-        """
-        Transforms Maccor cycle to conform to BattETL naming and data conventions
-        1. Rename columns
-        2. Convert to milli
-        3. Convert data type
-        4. Convert test time
-        5. Sort data
-
-        Parameters
-        ----------
-        df : pandas.DataFrame
-            The input DataFrame
-
-        Returns
-        -------
-        df : pandas.DataFrame
-            The transformed output DataFrame
-        """
-        df = Utils.rename_df_columns(
-            df, Constants.COLUMNS_MAPPING_MACCOR_CYCLE_STATS)
-        df = Utils.convert_to_milli(df)
-        df = self.__convert_data_type(df)
-
-        if 'test_time_s' in df.columns and len(df) > 0 and self.__timedelta_validation_check(df['test_time_s'][0]):
-            df = Utils.convert_timedelta_to_seconds(df, 'test_time_s')
-
-        df = Utils.sort_dataframe(df, ['cycle'])
-
-        return df
-
-    def __timedelta_validation_check(self, input_string):
-        # Check if it is like the format "1d 15:07:52.77" or "1d 15:07:52"
-        regex = re.compile(r'\d+d \d+:\d+:\d+(\.\d+)?\Z', re.I)
-        match = regex.match(str(input_string))
-        return bool(match)
-
-    def __convert_datetime_unixtime(self, df: pd.DataFrame) -> pd.DataFrame:
-        """
-        Convert datetime to UTC format and add unixtime_s column
-
-        Parameters
-        ----------
-        df : pandas.DataFrame
-            The input DataFrame
-
-        Returns
-        -------
-        df : pandas.DataFrame
-            The transformed output DataFrame
-        """
-        logger.info('Convert datetime and add unixtime_s')
-
-        df = Utils.convert_datetime(df, 'recorded_datetime', self.timezone)
-
-        # Convert to unix timestamp
-        df['unixtime_s'] = df['recorded_datetime'].astype(np.int64) // 10 ** 9
-
-        return df
-
-    def __convert_data_type(self, df: pd.DataFrame) -> pd.DataFrame:
-        """
-        Convert some data types if needed
-
-        Parameters
-        ----------
-        df : pandas.DataFrame
-            The input DataFrame
-
-        Returns
-        -------
-        df : pandas.DataFrame
-            The transformed output DataFrame
-        """
-        # Change the datatype to save on memory
-        if 'cycle' in df.columns:
-            logger.info('Convert column `cycle` to uint16')
-            df['cycle'] = df['cycle'].astype('uint16')
-        if 'stop' in df.columns:
-            logger.info('Convert column `step` to uint8')
-            df['step'] = df['step'].astype('uint8')
-
-        return df
-
-    def __harmonize_capacity(self, df: pd.DataFrame, steps: dict) -> pd.DataFrame:
-        """
-        Harmonizes capacity/energy values across cyclers by creating four new columns: `charge_capacity_mah`, 
-        `charge_energy_mwh`, `discharge_capacity_mah`, and `discharge_energy_mwh`. These columns only report 
-        capacity/energy values during corresponding charge or discharge steps. Otherwise, they will be 
-        `NaN`. The original capacity/energy reading is preserved in `cycler_charge_capacity_mah` or 
-        `cycler_charge_energy_mwh` column, where `cycler` is replaced with the name of the cycler manufacturer.
-
-        Parameters
-        ----------
-        df : pd.DataFrame
-            A pandas DataFrame containing data for single battery cycle.
-        steps : dict
-            A dictionary containing lists of charge (key->'chg'), discharge (key->'dsg'), and rest (key->'rst') steps.
-
-        Returns
-        -------
-        df : pd.DataFrame
-            A pandas DataFrame with harmonized capacity/energy values across cyclers.
-        """
-
-        if 'maccor_capacity_mah' in df:
-            df['charge_capacity_mah'] = df[df.step.isin(
-                steps['chg'])].maccor_capacity_mah
-            df['discharge_capacity_mah'] = df[df.step.isin(
-                steps['dsg'])].maccor_capacity_mah
-        if 'maccor_energy_mwh' in df:
-            df['charge_energy_mwh'] = df[df.step.isin(
-                steps['chg'])].maccor_energy_mwh
-            df['discharge_energy_mwh'] = df[df.step.isin(
-                steps['dsg'])].maccor_energy_mwh
-            # log rows and columns that be modified
-            logger.debug(
-                f'Harmonized capacity/energy values for Maccor cyclers. Modified {len(df)} rows and 4 columns.')
-            logger.debug(
-                'Added columns: charge_capacity_mah, charge_energy_mwh, discharge_capacity_mah, discharge_energy_mwh')
-        elif 'arbin_charge_capacity_mah' in df:
-            df['charge_capacity_mah'] = df[df.step.isin(
-                steps['chg'])].arbin_charge_capacity_mah
-            df['charge_energy_mwh'] = df[df.step.isin(
-                steps['chg'])].arbin_charge_energy_mwh
-            df['discharge_capacity_mah'] = df[df.step.isin(
-                steps['dsg'])].arbin_discharge_capacity_mah
-            df['discharge_energy_mwh'] = df[df.step.isin(
-                steps['dsg'])].arbin_discharge_energy_mwh
-            logger.debug(
-                f'Harmonized capacity/energy values for Arbin cyclers. Modified {len(df)} rows and 4 columns.')
-            logger.debug(
-                'Added columns: charge_capacity_mah, charge_energy_mwh, discharge_capacity_mah, discharge_energy_mwh')
-        else:
-            logger.warning("No capacity columns were found to refactor!")
-
-        return df
-
-    def calc_cycle_stats(self, steps: dict, cv_voltage_thresh_mv: float):
-        """
-        Calculates various charge and discharge statistics at the cycle level. Note this function 
-        can only be run after self.test_data exists
-
-        Parameters
-        ----------
-        steps : dict
-            A dictionary containing lists of charge (key->'chg'), discharge (key->'dsg'), and 
-            rest (key->'rst') steps.
-        cv_voltage_thresh_mv : float
-            The the voltage threshold in milli-volts above which charge is considered to be constant voltage.
-
-        Returns
-        -------
-        stats : dict
-            A dictionary containing various charge and discharge stats.
-        """
-        logger.debug(
-            f'Calculating cycle statistics with cv_voltage_thresh_mv: {cv_voltage_thresh_mv}')
-
-        if self.test_data.empty:
-            logger.error("Cannot run `calc_cycle_stats()` without test_data!")
-            return {}
-
-        self.test_data = self.__harmonize_capacity(self.test_data, steps)
-
-        # DataFrame where we will hold calculated cycle statistics for all cycles
-        df_calced_stats = pd.DataFrame(columns=['cycle'])
-
-        for cycle in range(self.test_data.cycle.head(1).item(), self.test_data.cycle.tail(1).item()+1):
-
-            cycle_data = self.test_data[self.test_data.cycle == cycle]
-            if cycle_data.empty:
-                logger.info("No cycle data for cycle " + str(cycle))
-                continue
-
-            # Calculate various charge and discharge cycle statistics.
-            stats = {'cycle': cycle}
-
-            charge_metrics = self.__calc_charge_stats(
-                cycle_data, steps['chg'], cv_voltage_thresh_mv)
-            stats.update(charge_metrics)
-
-            discharge_metrics = self.__calc_discharge_stats(
-                cycle_data, steps['dsg'])
-            stats.update(discharge_metrics)
-
-            # Calculate coulombic efficiency from the charge and discharge stats.
-            if (('calculated_charge_capacity_mah' not in stats) or
-                    ('calculated_discharge_capacity_mah' not in stats) or
-                    (stats['calculated_charge_capacity_mah'] == 0)):
-                ce = float("nan")
-                logger.info(
-                    "Unable to calculate coulombic efficiency for cycle " + str(cycle))
-            else:
-                ce = (discharge_metrics['calculated_discharge_capacity_mah']
-                      / charge_metrics['calculated_charge_capacity_mah'])
-            stats.update({'coulombic_efficiency': ce})
-
-            # Append the cycle statistics from this cycle to our cumulative DataFrame for all cycles.
-            df_calced_stats = pd.concat(
-                [df_calced_stats, pd.DataFrame(stats, index=[0])], axis=0)
-
-        if self.cycle_stats.empty:
-            self.cycle_stats = df_calced_stats
-        else:
-            self.cycle_stats = self.cycle_stats.join(
-                df_calced_stats.set_index('cycle'), on='cycle')
-
-        return self.cycle_stats
-
-    def __calc_charge_stats(self, cycle_data: pd.DataFrame, charge_steps: list, cv_voltage_thresh_mv: float) -> dict:
-        """
-        Calculates various charge stats for a single cycle of data.
-
-        Parameters
-        ----------
-        cycle_data : pd.DataFrame
-            A dataframe containing data for single battery cycle.
-        charge_steps : list
-            List of charge steps from the cycler schedule.
-        cv_voltage_thresh_mv : float
-            The the voltage threshold in milli-volts above which charge is considered to be constant voltage.
-
-        Returns
-        -------
-        stats : dict
-            A dictionary containing various charge stats.
-        """
-        logger.debug(
-            f'Calculating charge statistics with cv_voltage_thresh_mv: {cv_voltage_thresh_mv}')
-        stats = {}
-
-        # Define charge data to be where the step is a charge step.
-        chg_data = cycle_data[cycle_data.step.isin(charge_steps)]
-        if len(chg_data) < 2:
-            logger.info("No charge data for cycle " +
-                        str(cycle_data.cycle.iloc[0]))
-            return stats
-
-        ez_df = self.__ez_calc_df(
-            chg_data, charge_steps, 'charge', cv_voltage_thresh_mv)
-
-        stats['calculated_charge_capacity_mah'] = ez_df['charge_capacity_mah'].iloc[-1]
-        stats['calculated_charge_energy_mwh'] = ez_df['charge_energy_mwh'].iloc[-1]
-        stats['calculated_charge_time_s'] = ez_df['ellapsed_time_s'].iloc[-1]
-
-        stats['calculated_cc_charge_time_s'] = ez_df.cc_time_s.sum()
-        stats['calculated_cv_charge_time_s'] = ez_df.cv_time_s.sum()
-        stats['calculated_cc_capacity_mah'] = ez_df.cc_capacity_mah.sum()
-        stats['calculated_cv_capacity_mah'] = ez_df.cv_capacity_mah.sum()
-
-        # Calculate 50%/80% charge time & capacity.
-        eighty_percent_cap_mah = stats['calculated_charge_capacity_mah'] * 0.8
-        fifty_percent_cap_mah = stats['calculated_charge_capacity_mah'] * 0.5
-        try:
-            eighty_percent_cap_time_s = (ez_df[ez_df.charge_capacity_mah > eighty_percent_cap_mah].ellapsed_time_s.iloc[0]
-                                         - ez_df.ellapsed_time_s.iloc[0])
-            half_percent_cap_time_s = (ez_df[ez_df.charge_capacity_mah > fifty_percent_cap_mah].ellapsed_time_s.iloc[0]
-                                       - ez_df.ellapsed_time_s.iloc[0])
-        except:
-            eighty_percent_cap_time_s = float('nan')
-            half_percent_cap_time_s = float('nan')
-            logger.warning(
-                f'Incomplete charge data for cycle {cycle_data.cycle.iloc[0]}')
-
-        stats['calculated_fifty_percent_charge_time_s'] = half_percent_cap_time_s
-        stats['calculated_eighty_percent_charge_time_s'] = eighty_percent_cap_time_s
-
-        return stats
-
-    def __calc_discharge_stats(self, cycle_data: pd.DataFrame, discharge_steps: list) -> dict:
-        """
-        Calculates various discharge stats for a single cycle of data.
-
-        Parameters
-        ----------
-        cycle_data : pd.DataFrame
-            A dataframe containing data for single battery cycle.
-        discharge_steps : list
-            List of discharge steps from the cycler schedule.
-
-        Returns
-        -------
-        stats : dict
-            A dictionary containing various discharge stats.
-        """
-        logger.debug('Calculating discharge statistics')
-        stats = {}
-
-        # Define discharge data to be where the step is a discharge step.
-        dsg_data = cycle_data[cycle_data.step.isin(discharge_steps)]
-        if len(dsg_data) < 2:
-            logger.info("No discharge data for cycle " +
-                        str(cycle_data.cycle.iloc[0]))
-            return stats
-
-        ez_df = self.__ez_calc_df(dsg_data, discharge_steps, 'discharge')
-
-        stats['calculated_discharge_capacity_mah'] = ez_df['discharge_capacity_mah'].iloc[-1]
-        stats['calculated_discharge_energy_mwh'] = ez_df['discharge_energy_mwh'].iloc[-1]
-        stats['calculated_discharge_time_s'] = ez_df['ellapsed_time_s'].iloc[-1]
-
-        return stats
-
-    def __ez_calc_df(self, cycle_df: pd.DataFrame, steps: list, step_type: str, cv_voltage_thresh_mv=None) -> tuple:
-        """
-        Creates a DataFrame we can easily use to calculate cycle statistics.
-
-        Modifies test_data to cummulative capacity in cases where capacity is reset at each step.
-
-        Parameters
-        ----------
-        df : pd.DataFrame
-            The DataFrame use to calculate cumulative capacity.
-        steps : list
-            A list of the steps to calculate cumulative capacity for. 
-        step_type : str
-            Either 'charge' or 'discharge' depending on what type of steps we are calculating for.
-        cv_voltage_thresh_mv : float
-            The voltage threshold in mV above which charge is considered to be constant voltage.    
-
-        Returns
-        -------
-        ez_df: pd.DataFrame
-            Dataframe containing values filtered to charge steps with cumulative capacity
-            and ellapsed time calculated.
-        """
-        logger.debug(f'Calculating cumulative {step_type} capacity')
-
-        time_col = 'ellapsed_time_s'
-        volt_col = 'voltage_mv'
-        cc_time = 'cc_time_s'
-        cv_time = 'cv_time_s'
-        cc_cap = 'cc_capacity_mah'
-        cv_cap = 'cv_capacity_mah'
-        if step_type == 'charge':
-            cap_col = 'charge_capacity_mah'
-            eng_col = 'charge_energy_mwh'
-        elif step_type == 'discharge':
-            cap_col = 'discharge_capacity_mah'
-            eng_col = 'discharge_energy_mwh'
-        else:
-            logger.error(f'Unknown step type {step_type}!')
-            return pd.DataFrame()
-
-        ez_df = pd.DataFrame(
-            columns=[time_col, volt_col, cap_col, eng_col, cc_time, cv_time, cc_cap, cv_cap])
-
-        # Iterate through each charge step to calculate cumulative capacity
-
-        for i, step in enumerate(steps):
-
-            step_slice = cycle_df[cycle_df.step == step]
-            step_df = pd.DataFrame(
-                columns=[time_col, volt_col, cap_col, eng_col, cc_time, cv_time, cc_cap, cv_cap])
-
-            if step_slice.empty:
-                continue
-
-            if ez_df.empty:
-                ez_df[time_col] = step_slice['test_time_s'] - \
-                    step_slice['test_time_s'].iloc[0]
-                ez_df[volt_col] = step_slice['voltage_mv']
-                ez_df[eng_col] = step_slice[eng_col] - \
-                    step_slice[eng_col].iloc[0]
-                ez_df[cap_col] = step_slice[cap_col] - \
-                    step_slice[cap_col].iloc[0]
-                if step_type == 'charge':
-                    # if ez_df is empty, we're at beginning of a cycle and cap/step time should be reset to zero
-                    # TODO: add documentation for this
-                    delta_time = step_slice['step_time_s'] - \
-                        step_slice['step_time_s'].shift(1, fill_value=0)
-                    ez_df[cc_time] = np.where(
-                        step_slice[volt_col] < cv_voltage_thresh_mv, delta_time, 0)
-                    ez_df[cv_time] = np.where(
-                        step_slice[volt_col] >= cv_voltage_thresh_mv, delta_time, 0)
-                    delta_cap = step_slice[cap_col] - \
-                        step_slice[cap_col].shift(1, fill_value=0)
-                    ez_df[cc_cap] = np.where(
-                        step_slice[volt_col] < cv_voltage_thresh_mv, delta_cap, 0)
-                    ez_df[cv_cap] = np.where(
-                        step_slice[volt_col] >= cv_voltage_thresh_mv, delta_cap, 0)
-                # TODO: corner case of ICT will still need above logic for discharge
-                elif step_type == 'discharge':
-                    ez_df[[cc_time, cc_cap, cv_time, cv_cap]] = np.nan
-            else:
-                # This catches if capacity was reset after each step. Modifies test_data DF in place.
-                if step_slice[cap_col].iloc[0] < ez_df[cap_col].iloc[-1]:
-                    current_cycle = cycle_df.cycle.iloc[0]
-                    self.test_data.loc[self.test_data.cycle == current_cycle,
-                                       self.test_data.step == step, cap_col] += ez_df[cap_col]
-                    self.test_data.loc[self.test_data.cycle == current_cycle,
-                                       self.test_data.step == step, eng_col] += ez_df[eng_col]
-                if not ez_df.empty:
-                    # keeps running time across steps. ignoring time between steps
-                    step_df[time_col] = (
-                        step_slice['test_time_s'] - step_slice['test_time_s'].iloc[0]) + ez_df[time_col].iloc[-1]
-                # step_slice is updated with above updates to test_data because it's a slice, not copy, of test_data
-                step_df[volt_col] = step_slice[volt_col]
-                step_df[cap_col] = step_slice[cap_col]
-                step_df[eng_col] = step_slice[eng_col]
-                if step_type == 'charge':
-                    # calculate the delta time/cap for each step, sum the deltas in calc_stats() to get cycle time/cap
-                    delta_time = step_slice['step_time_s'] - \
-                        step_slice['step_time_s'].shift(1, fill_value=0)
-                    step_df[cc_time] = np.where(
-                        step_slice[volt_col] < cv_voltage_thresh_mv, delta_time, 0)
-                    step_df[cv_time] = np.where(
-                        step_slice[volt_col] >= cv_voltage_thresh_mv, delta_time, 0)
-                    delta_cap = step_slice[cap_col] - step_slice[cap_col].shift(
-                        1, fill_value=ez_df[cap_col].iloc[-1])
-                    step_df[cc_cap] = np.where(
-                        step_slice[volt_col] < cv_voltage_thresh_mv, delta_cap, 0)
-                    step_df[cv_cap] = np.where(
-                        step_slice[volt_col] >= cv_voltage_thresh_mv, delta_cap, 0)
-                elif step_type == 'discharge':
-                    step_df[[cc_time, cc_cap, cv_time, cv_cap]] = np.nan
-                ez_df = pd.concat([ez_df, step_df])
-        logger.debug(f'Finished calculating cumulative {step_type} capacity')
-        return ez_df
+import re
+import numpy as np
+import pandas as pd
+from typing import Callable
+
+from battetl import logger, Constants, Utils
+
+
+class Transformer:
+    def __init__(
+            self,
+            timezone: str = None,
+            user_transform_test_data: Callable[[
+                pd.DataFrame], pd.DataFrame] = None,
+            user_transform_cycle_stats: Callable[[
+                pd.DataFrame], pd.DataFrame] = None) -> None:
+        """
+        An interface to transform battery test data to BattETL schema.
+
+        Parameters
+        ----------
+        timezone : str
+            Time zone strings in the IANA Time Zone Database. Used to convert to unix timestamp
+            in seconds. Default 'America/Los_Angeles'.
+        user_transform_test_data : Callable[[pd.DataFrame], pd.DataFrame], optional
+            A user defined function to transform test data. The function should take a pandas.DataFrame
+            as input and return a pandas.DataFrame as output.
+        user_transform_cycle_stats : Callable[[pd.DataFrame], pd.DataFrame], optional
+            A user defined function to transform cycle stats. The function should take a pandas.DataFrame
+            as input and return a pandas.DataFrame as output.
+        """
+        # Default 'America/Los_Angeles'.
+        self.timezone = timezone if timezone else Constants.DEFAULT_TIME_ZONE
+        self.user_transform_test_data = user_transform_test_data
+        self.user_transform_cycle_stats = user_transform_cycle_stats
+        if self.user_transform_test_data:
+            logger.info('User defined transform_test_data function found')
+        if self.user_transform_cycle_stats:
+            logger.info('User defined transform_cycle_stats function found')
+
+        self.test_data = pd.DataFrame()
+        self.cycle_stats = pd.DataFrame()
+
+    def transform_test_data(self, data: pd.DataFrame) -> pd.DataFrame:
+        """
+        Transforms test data to conform to BattETL naming and data conventions
+
+        Parameters
+        ----------
+        data : pandas.DataFrame
+            The input DataFrame
+        schedule_steps : dict
+            A dictionary containing lists of charge (key->'chg'), discharge (key->'dsg'), and 
+            rest (key->'rst') steps from the schedule used to generate the data. Used to calculate
+            cycle level statistics (e.g. CV charge time.)
+
+        Returns
+        -------
+        df : pandas.DataFrame
+            The transformed output DataFrame
+        """
+        logger.info('Transform test data')
+
+        df = data.copy()
+        df = Utils.drop_unnamed_columns(df)
+        df = Utils.drop_empty_rows(df)
+
+        cycleMake, dataType = Utils.get_cycle_make(df.columns)
+        logger.info(f'Cycle make: {cycleMake}. Data type: {dataType}')
+
+        if cycleMake == Constants.MAKE_ARBIN and dataType == Constants.DATA_TYPE_TEST_DATA:
+            df = self.__transform_arbin_test_data(df)
+
+        if cycleMake == Constants.MAKE_MACCOR and dataType == Constants.DATA_TYPE_TEST_DATA:
+            df = self.__transform_maccor_test_data(df)
+
+        df = self.__consolidate_temps(df)
+
+        # Apply user defined transformation
+        if self.user_transform_test_data:
+            df = self.user_transform_test_data(df)
+
+        self.test_data = df
+        return df
+
+    def transform_cycle_stats(self, data: pd.DataFrame) -> pd.DataFrame:
+        """
+        Transforms cycle stats to conform to BattETL naming and data conventions
+
+        Parameters
+        ----------
+        data : pandas.DataFrame
+            The input DataFrame
+
+        Returns
+        -------
+        df : pandas.DataFrame
+            The transformed output DataFrame
+        """
+        logger.info('Transform cycle stats')
+
+        df = data.copy()
+        df = Utils.drop_unnamed_columns(df)
+        df = Utils.drop_empty_rows(df)
+
+        cycleMake, dataType = Utils.get_cycle_make(df.columns)
+        logger.info(f'cycle make: {cycleMake}, data type: {dataType}')
+
+        if cycleMake == Constants.MAKE_ARBIN and dataType == Constants.DATA_TYPE_CYCLE_STATS:
+            df = self.__transform_arbin_cycle_stats(df)
+
+        if cycleMake == Constants.MAKE_MACCOR and dataType == Constants.DATA_TYPE_CYCLE_STATS:
+            df = self.__transform_maccor_cycle_stats(df)
+
+        # Apply user defined transformation
+        if self.user_transform_cycle_stats:
+            df = self.user_transform_cycle_stats(df)
+
+        self.cycle_stats = df
+        return df
+
+    def __transform_arbin_test_data(self, df: pd.DataFrame) -> pd.DataFrame:
+        """
+        Transforms Arbin test data to conform to BattETL naming and data conventions
+        1. Rename columns
+        2. Convert to milli
+        3. Convert datetime
+        4. Convert data type
+        5. Sort data
+
+        Parameters
+        ----------
+        df : pandas.DataFrame
+            The input DataFrame
+
+        Returns
+        -------
+        df : pandas.DataFrame
+            The transformed output DataFrame
+        """
+        df = Utils.rename_df_columns(
+            df, Constants.COLUMNS_MAPPING_ARBIN_TEST_DATA)
+        df = Utils.convert_to_milli(df)
+        df = self.__convert_datetime_unixtime(df)
+        df = self.__convert_data_type(df)
+        df = Utils.sort_dataframe(df, ['unixtime_s', 'step'])
+
+        return df
+
+    def __transform_arbin_cycle_stats(self, df: pd.DataFrame) -> pd.DataFrame:
+        """
+        Transforms Arbin cycle stats to conform to BattETL naming and data conventions
+        1. Rename columns
+        2. Convert to milli
+        3. Convert data type
+        4. Sort data
+
+        Parameters
+        ----------
+        df : pandas.DataFrame
+            The input DataFrame
+
+        Returns
+        -------
+        df : pandas.DataFrame
+            The transformed output DataFrame
+        """
+        df = Utils.rename_df_columns(
+            df, Constants.COLUMNS_MAPPING_ARBIN_CYCLE_STATS)
+        df = Utils.convert_to_milli(df)
+        df = self.__convert_data_type(df)
+        df = Utils.sort_dataframe(df, ['cycle'])
+
+        return df
+
+    def __transform_maccor_test_data(self, df: pd.DataFrame) -> pd.DataFrame:
+        """
+        Transforms Maccor test data to conform to BattETL naming and data conventions
+        1. Rename columns
+        2. Convert to milli
+        3. Convert datetime
+        4. Convert data type
+        5. Sort data
+
+        Parameters
+        ----------
+        df : pandas.DataFrame
+            The input DataFrame
+
+        Returns
+        -------
+        df : pandas.DataFrame
+            The transformed output DataFrame
+        """
+        df = Utils.rename_df_columns(
+            df, Constants.COLUMNS_MAPPING_MACCOR_TEST_DATA)
+        df = Utils.convert_to_milli(df)
+        df = self.__convert_datetime_unixtime(df)
+        df = self.__convert_data_type(df)
+
+        if 'test_time_s' in df.columns and len(df) > 0 and self.__timedelta_validation_check(df['test_time_s'][0]):
+            df = Utils.convert_timedelta_to_seconds(df, 'test_time_s')
+        if 'step_time_s' in df.columns and len(df) > 0 and self.__timedelta_validation_check(df['step_time_s'][0]):
+            df = Utils.convert_timedelta_to_seconds(df, 'step_time_s')
+
+        df = Utils.sort_dataframe(df, ['unixtime_s', 'step'])
+
+        return df
+
+    def __transform_maccor_cycle_stats(self, df: pd.DataFrame) -> pd.DataFrame:
+        """
+        Transforms Maccor cycle to conform to BattETL naming and data conventions
+        1. Rename columns
+        2. Convert to milli
+        3. Convert data type
+        4. Convert test time
+        5. Sort data
+
+        Parameters
+        ----------
+        df : pandas.DataFrame
+            The input DataFrame
+
+        Returns
+        -------
+        df : pandas.DataFrame
+            The transformed output DataFrame
+        """
+        df = Utils.rename_df_columns(
+            df, Constants.COLUMNS_MAPPING_MACCOR_CYCLE_STATS)
+        df = Utils.convert_to_milli(df)
+        df = self.__convert_data_type(df)
+
+        if 'test_time_s' in df.columns and len(df) > 0 and self.__timedelta_validation_check(df['test_time_s'][0]):
+            df = Utils.convert_timedelta_to_seconds(df, 'test_time_s')
+
+        df = Utils.sort_dataframe(df, ['cycle'])
+
+        return df
+
+    def __timedelta_validation_check(self, input_string):
+        # Check if it is like the format "1d 15:07:52.77" or "1d 15:07:52"
+        regex = re.compile(r'\d+d \d+:\d+:\d+(\.\d+)?\Z', re.I)
+        match = regex.match(str(input_string))
+        return bool(match)
+
+    def __convert_datetime_unixtime(self, df: pd.DataFrame) -> pd.DataFrame:
+        """
+        Convert datetime to UTC format and add unixtime_s column
+
+        Parameters
+        ----------
+        df : pandas.DataFrame
+            The input DataFrame
+
+        Returns
+        -------
+        df : pandas.DataFrame
+            The transformed output DataFrame
+        """
+        logger.info('Convert datetime and add unixtime_s')
+
+        df = Utils.convert_datetime(df, 'recorded_datetime', self.timezone)
+
+        # Convert to unix timestamp
+        df['unixtime_s'] = df['recorded_datetime'].astype(np.int64) // 10 ** 9
+
+        return df
+
+    def __convert_data_type(self, df: pd.DataFrame) -> pd.DataFrame:
+        """
+        Convert some data types if needed
+
+        Parameters
+        ----------
+        df : pandas.DataFrame
+            The input DataFrame
+
+        Returns
+        -------
+        df : pandas.DataFrame
+            The transformed output DataFrame
+        """
+        # Change the datatype to save on memory
+        if 'cycle' in df.columns:
+            logger.info('Convert column `cycle` to uint16')
+            df['cycle'] = df['cycle'].astype('uint16')
+        if 'stop' in df.columns:
+            logger.info('Convert column `step` to uint8')
+            df['step'] = df['step'].astype('uint8')
+
+        # convert temperature columns to float
+        temperature_columns = df.columns[
+            df.columns.str.contains('thermocouple_')]
+        if len(temperature_columns) > 0:
+            logger.info('Convert temperature columns to float')
+            for column in temperature_columns:
+                df[column] = df[column].apply(Utils.convert_to_float)
+        return df
+
+    def __harmonize_capacity(self, df: pd.DataFrame, steps: dict) -> pd.DataFrame:
+        """
+        Harmonizes capacity/energy values across cyclers by creating four new columns: `charge_capacity_mah`, 
+        `charge_energy_mwh`, `discharge_capacity_mah`, and `discharge_energy_mwh`. These columns only report 
+        capacity/energy values during corresponding charge or discharge steps. Otherwise, they will be 
+        `NaN`. The original capacity/energy reading is preserved in `cycler_charge_capacity_mah` or 
+        `cycler_charge_energy_mwh` column, where `cycler` is replaced with the name of the cycler manufacturer.
+
+        Parameters
+        ----------
+        df : pd.DataFrame
+            A pandas DataFrame containing data for single battery cycle.
+        steps : dict
+            A dictionary containing lists of charge (key->'chg'), discharge (key->'dsg'), and rest (key->'rst') steps.
+
+        Returns
+        -------
+        df : pd.DataFrame
+            A pandas DataFrame with harmonized capacity/energy values across cyclers.
+        """
+
+        if 'maccor_capacity_mah' in df:
+            df['charge_capacity_mah'] = df[df.step.isin(
+                steps['chg'])].maccor_capacity_mah
+            df['discharge_capacity_mah'] = df[df.step.isin(
+                steps['dsg'])].maccor_capacity_mah
+        if 'maccor_energy_mwh' in df:
+            df['charge_energy_mwh'] = df[df.step.isin(
+                steps['chg'])].maccor_energy_mwh
+            df['discharge_energy_mwh'] = df[df.step.isin(
+                steps['dsg'])].maccor_energy_mwh
+            # log rows and columns that be modified
+            logger.debug(
+                f'Harmonized capacity/energy values for Maccor cyclers. Modified {len(df)} rows and 4 columns.')
+            logger.debug(
+                'Added columns: charge_capacity_mah, charge_energy_mwh, discharge_capacity_mah, discharge_energy_mwh')
+        elif 'arbin_charge_capacity_mah' in df:
+            df['charge_capacity_mah'] = df[df.step.isin(
+                steps['chg'])].arbin_charge_capacity_mah
+            df['charge_energy_mwh'] = df[df.step.isin(
+                steps['chg'])].arbin_charge_energy_mwh
+            df['discharge_capacity_mah'] = df[df.step.isin(
+                steps['dsg'])].arbin_discharge_capacity_mah
+            df['discharge_energy_mwh'] = df[df.step.isin(
+                steps['dsg'])].arbin_discharge_energy_mwh
+            logger.debug(
+                f'Harmonized capacity/energy values for Arbin cyclers. Modified {len(df)} rows and 4 columns.')
+            logger.debug(
+                'Added columns: charge_capacity_mah, charge_energy_mwh, discharge_capacity_mah, discharge_energy_mwh')
+        else:
+            logger.warning("No capacity columns were found to refactor!")
+
+        return df
+
+    def calc_cycle_stats(self, steps: dict, cv_voltage_threshold_mv: float = None, cell_thermocouple: int = None) -> pd.DataFrame:
+        """
+        Calculates various charge and discharge statistics at the cycle level. Note this function 
+        can only be run after self.test_data exists
+
+        Parameters
+        ----------
+        steps : dict
+            A dictionary containing lists of charge (key->'chg'), discharge (key->'dsg'), and 
+            rest (key->'rst') steps.
+        cv_voltage_thresh_mv : float
+            The the voltage threshold in milli-volts above which charge is considered to be constant voltage.
+        cell_thermocouple : int
+            The number (as listed in the db column) of the thermocouple  that's attached to the cell.
+
+        Returns
+        -------
+        self.cycle_stats : pd.DataFrame
+            The calculated cycle statistics for all cycles.
+        """
+        if self.test_data.empty:
+            logger.error("Cannot run `calc_cycle_stats()` without test_data!")
+            return self.cycle_stats
+
+        self.test_data = self.__harmonize_capacity(self.test_data, steps)
+
+        # DataFrame where we will hold calculated cycle statistics for all cycles
+        df_calced_stats = pd.DataFrame(columns=['cycle'])
+
+        cycle_list = self.test_data['cycle'].unique()
+        logger.info(
+            f'Calculating cycle statistics for {len(cycle_list)} cycles')
+
+        for cycle in cycle_list:
+            cycle_data = self.test_data[self.test_data.cycle == cycle]
+            if cycle_data.empty:
+                logger.info("No cycle data for cycle " + str(cycle))
+                continue
+
+            # Calculate various charge and discharge cycle statistics.
+            stats = {'cycle': cycle}
+
+            charge_metrics = self.__calc_charge_stats(
+                cycle_data, steps['chg'], cv_voltage_threshold_mv, cell_thermocouple)
+            stats.update(charge_metrics)
+
+            discharge_metrics = self.__calc_discharge_stats(
+                cycle_data, steps['dsg'], cell_thermocouple)
+            stats.update(discharge_metrics)
+
+            # Calculate coulombic efficiency from the charge and discharge stats.
+            if (('calculated_charge_capacity_mah' not in stats) or
+                    ('calculated_discharge_capacity_mah' not in stats) or
+                    (stats['calculated_charge_capacity_mah'] == 0)):
+                ce = float("nan")
+                logger.info(
+                    "Unable to calculate coulombic efficiency for cycle " + str(cycle))
+            else:
+                ce = (discharge_metrics['calculated_discharge_capacity_mah']
+                      / charge_metrics['calculated_charge_capacity_mah'])
+            stats.update({'calculated_coulombic_efficiency': ce})
+
+            # Append the cycle statistics from this cycle to our cumulative DataFrame for all cycles.
+            df_calced_stats = pd.concat(
+                [df_calced_stats, pd.DataFrame(stats, index=[0])], axis=0)
+
+        if self.cycle_stats.empty:
+            self.cycle_stats = df_calced_stats
+        else:
+            self.cycle_stats = self.cycle_stats.join(
+                df_calced_stats.set_index('cycle'), on='cycle')
+
+        return self.cycle_stats
+
+    def __calc_charge_stats(self, cycle_data: pd.DataFrame, charge_steps: list, cv_voltage_threshold_mv: float = None, cell_thermocouple: int = None) -> dict:
+        """
+        Calculates various charge stats for a single cycle of data.
+
+        Parameters
+        ----------
+        cycle_data : pd.DataFrame
+            A DataFrame containing data for single battery cycle.
+        charge_steps : list
+            List of charge steps from the cycler schedule.
+        cv_voltage_thresh_mv : float
+            The the voltage threshold in milli-volts above which charge is considered to be constant voltage.
+        cell_thermocouple : int
+            The number (as listed in the db column) of the thermocouple  that's attached to the cell.
+
+        Returns
+        -------
+        stats : dict
+            A dictionary containing various charge stats.
+        """
+        logger.debug(
+            f'Calculating charge statistics for cycle {cycle_data.cycle.iloc[0]} \
+                with {len(cycle_data)} rows and {len(charge_steps)} charge steps.')
+
+        if cv_voltage_threshold_mv:
+            logger.debug(
+                f'Using CV voltage threshold of {cv_voltage_threshold_mv} mV.')
+
+        stats = {}
+
+        # Define charge data to be where the step is a charge step.
+        chg_data = cycle_data[cycle_data.step.isin(charge_steps)]
+        if len(chg_data) < 2:
+            logger.info("No charge data for cycle " +
+                        str(cycle_data.cycle.iloc[0]))
+            return stats
+
+        ez_df = self.__ez_calc_df(
+            chg_data, charge_steps, 'charge', cv_voltage_threshold_mv)
+
+        stats['calculated_charge_capacity_mah'] = ez_df['charge_capacity_mah'].iloc[-1]
+        stats['calculated_charge_energy_mwh'] = ez_df['charge_energy_mwh'].iloc[-1]
+        stats['calculated_charge_time_s'] = ez_df['ellapsed_time_s'].iloc[-1]
+
+        stats['calculated_cc_charge_time_s'] = ez_df.cc_time_s.sum()
+        stats['calculated_cv_charge_time_s'] = ez_df.cv_time_s.sum()
+        stats['calculated_cc_capacity_mah'] = ez_df.cc_capacity_mah.sum()
+        stats['calculated_cv_capacity_mah'] = ez_df.cv_capacity_mah.sum()
+
+        # Calculate 50%/80% charge time & capacity.
+        eighty_percent_cap_mah = stats['calculated_charge_capacity_mah'] * 0.8
+        fifty_percent_cap_mah = stats['calculated_charge_capacity_mah'] * 0.5
+        try:
+            eighty_percent_cap_time_s = (ez_df[ez_df.charge_capacity_mah > eighty_percent_cap_mah].ellapsed_time_s.iloc[0]
+                                         - ez_df.ellapsed_time_s.iloc[0])
+            half_percent_cap_time_s = (ez_df[ez_df.charge_capacity_mah > fifty_percent_cap_mah].ellapsed_time_s.iloc[0]
+                                       - ez_df.ellapsed_time_s.iloc[0])
+        except:
+            eighty_percent_cap_time_s = float('nan')
+            half_percent_cap_time_s = float('nan')
+            logger.warning(
+                f'Incomplete charge data for cycle {cycle_data.cycle.iloc[0]}')
+
+        stats['calculated_fifty_percent_charge_time_s'] = half_percent_cap_time_s
+        stats['calculated_eighty_percent_charge_time_s'] = eighty_percent_cap_time_s
+
+        if cell_thermocouple:
+            logger.debug(
+                f'Using cell thermocouple {cell_thermocouple} to calculate max charge temp.')
+            thermocouple_col = f"thermocouple_{cell_thermocouple}_c"
+            try:
+                stats['calculated_max_charge_temp_c'] = chg_data.loc[:,
+                                                                     thermocouple_col].max()
+            except:
+                logger.warning(
+                    'cell_thermocouple value supplied, but not found in test_data.')
+
+        return stats
+
+    def __calc_discharge_stats(self, cycle_data: pd.DataFrame, discharge_steps: list, cell_thermocouple: int = None) -> dict:
+        """
+        Calculates various discharge stats for a single cycle of data.
+
+        Parameters
+        ----------
+        cycle_data : pd.DataFrame
+            A DataFrame containing data for single battery cycle.
+        discharge_steps : list
+            List of discharge steps from the cycler schedule.
+        cell_thermocouple : int
+            The number (as listed in the db column) of the thermocouple  that's attached to the cell.
+
+        Returns
+        -------
+        stats : dict
+            A dictionary containing various discharge stats.
+        """
+        logger.debug(
+            f'Calculating discharge statistics for cycle {cycle_data.cycle.iloc[0]} \
+                with {len(cycle_data)} rows and {len(discharge_steps)} discharge steps')
+        stats = {}
+
+        # Define discharge data to be where the step is a discharge step.
+        dsg_data = cycle_data[cycle_data.step.isin(discharge_steps)]
+        if len(dsg_data) < 2:
+            logger.info("No discharge data for cycle " +
+                        str(cycle_data.cycle.iloc[0]))
+            return stats
+
+        ez_df = self.__ez_calc_df(dsg_data, discharge_steps, 'discharge')
+
+        stats['calculated_discharge_capacity_mah'] = ez_df['discharge_capacity_mah'].iloc[-1]
+        stats['calculated_discharge_energy_mwh'] = ez_df['discharge_energy_mwh'].iloc[-1]
+        stats['calculated_discharge_time_s'] = ez_df['ellapsed_time_s'].iloc[-1]
+
+        if cell_thermocouple:
+            logger.debug(
+                f'Using cell thermocouple {cell_thermocouple} to calculate max discharge temp.')
+            thermocouple_col = f"thermocouple_{cell_thermocouple}_c"
+            try:
+                stats['calculated_max_discharge_temp_c'] = dsg_data.loc[:,
+                                                                        thermocouple_col].max()
+            except:
+                logger.warning(
+                    'cell_thermocouple value supplied, but not found in test_data.')
+        return stats
+
+    def __ez_calc_df(self, cycle_df: pd.DataFrame, steps: list, step_type: str, cv_voltage_thresh_mv: float = None) -> pd.DataFrame:
+        """
+        Creates a DataFrame we can easily use to calculate cycle statistics.
+
+        Modifies test_data to cumulative capacity in cases where capacity is reset at each step.
+
+        Parameters
+        ----------
+        df : pd.DataFrame
+            The DataFrame use to calculate cumulative capacity.
+        steps : list
+            A list of the steps to calculate cumulative capacity for. 
+        step_type : str
+            Either 'charge' or 'discharge' depending on what type of steps we are calculating for.
+        cv_voltage_thresh_mv : float
+            The voltage threshold in mV above which charge is considered to be constant voltage.    
+
+        Returns
+        -------
+        ez_df: pd.DataFrame
+            DataFrame containing values filtered to charge steps with cumulative capacity
+            and ellapsed time calculated.
+        """
+        logger.debug(
+            f'Calculating cumulative capacity with {len(cycle_df)} rows, \
+                  {len(steps)} {step_type} steps and cv_voltage_thresh_mv: {cv_voltage_thresh_mv}')
+
+        time_col = 'ellapsed_time_s'
+        volt_col = 'voltage_mv'
+        cc_time = 'cc_time_s'
+        cv_time = 'cv_time_s'
+        cc_cap = 'cc_capacity_mah'
+        cv_cap = 'cv_capacity_mah'
+        if step_type == 'charge':
+            cap_col = 'charge_capacity_mah'
+            eng_col = 'charge_energy_mwh'
+        elif step_type == 'discharge':
+            cap_col = 'discharge_capacity_mah'
+            eng_col = 'discharge_energy_mwh'
+        else:
+            logger.error(f'Unknown step type {step_type}!')
+            return pd.DataFrame()
+
+        ez_df = pd.DataFrame(
+            columns=[time_col, volt_col, cap_col, eng_col, cc_time, cv_time, cc_cap, cv_cap])
+
+        # Iterate through each charge step to calculate cumulative capacity
+        for _, step in enumerate(steps):
+
+            step_slice = cycle_df[cycle_df.step == step]
+            step_df = pd.DataFrame(
+                columns=[time_col, volt_col, cap_col, eng_col, cc_time, cv_time, cc_cap, cv_cap])
+
+            if step_slice.empty:
+                continue
+
+            if ez_df.empty:
+                ez_df[time_col] = step_slice['test_time_s'] - \
+                    step_slice['test_time_s'].iloc[0]
+                ez_df[volt_col] = step_slice['voltage_mv']
+                ez_df[eng_col] = step_slice[eng_col] - \
+                    step_slice[eng_col].iloc[0]
+                ez_df[cap_col] = step_slice[cap_col] - \
+                    step_slice[cap_col].iloc[0]
+                if step_type == 'charge' and cv_voltage_thresh_mv is not None:
+                    # if ez_df is empty, we're at beginning of a cycle and cap/step time should be reset to zero
+                    # TODO: add documentation for this
+                    delta_time = step_slice['step_time_s'] - \
+                        step_slice['step_time_s'].shift(1, fill_value=0)
+                    ez_df[cc_time] = np.where(
+                        step_slice[volt_col] < cv_voltage_thresh_mv, delta_time, 0)
+                    ez_df[cv_time] = np.where(
+                        step_slice[volt_col] >= cv_voltage_thresh_mv, delta_time, 0)
+                    delta_cap = step_slice[cap_col] - \
+                        step_slice[cap_col].shift(1, fill_value=0)
+                    ez_df[cc_cap] = np.where(
+                        step_slice[volt_col] < cv_voltage_thresh_mv, delta_cap, 0)
+                    ez_df[cv_cap] = np.where(
+                        step_slice[volt_col] >= cv_voltage_thresh_mv, delta_cap, 0)
+                # TODO: corner case of ICT will still need above logic for discharge
+                elif step_type == 'discharge':
+                    ez_df[[cc_time, cc_cap, cv_time, cv_cap]] = np.nan
+            else:
+                # This catches if capacity was reset after each step. Modifies test_data DF in place.
+                if step_slice[cap_col].iloc[0] < ez_df[cap_col].iloc[-1]:
+                    current_cycle = cycle_df.cycle.iloc[0]
+                    self.test_data.loc[
+                        (self.test_data.cycle == current_cycle) &
+                        (self.test_data.step == step),
+                        cap_col] += ez_df[cap_col]
+                    self.test_data.loc[
+                        (self.test_data.cycle == current_cycle) &
+                        (self.test_data.step == step),
+                        eng_col] += ez_df[eng_col]
+                    step_slice[cap_col] += ez_df[cap_col].iloc[-1]
+                    step_slice[eng_col] += ez_df[eng_col].iloc[-1]
+                if not ez_df.empty:
+                    # keeps running time across steps. ignoring time between steps
+                    step_df[time_col] = (
+                        step_slice['test_time_s'] - step_slice['test_time_s'].iloc[0]) + ez_df[time_col].iloc[-1]
+                # step_slice is updated with above updates to test_data because it's a slice, not copy, of test_data
+                step_df[volt_col] = step_slice[volt_col]
+                step_df[cap_col] = step_slice[cap_col]
+                step_df[eng_col] = step_slice[eng_col]
+                if step_type == 'charge' and cv_voltage_thresh_mv is not None:
+                    # calculate the delta time/cap for each step, sum the deltas in calc_stats() to get cycle time/cap
+                    delta_time = step_slice['step_time_s'] - \
+                        step_slice['step_time_s'].shift(1, fill_value=0)
+                    step_df[cc_time] = np.where(
+                        step_slice[volt_col] < cv_voltage_thresh_mv, delta_time, 0)
+                    step_df[cv_time] = np.where(
+                        step_slice[volt_col] >= cv_voltage_thresh_mv, delta_time, 0)
+                    delta_cap = step_slice[cap_col] - step_slice[cap_col].shift(
+                        1, fill_value=ez_df[cap_col].iloc[-1])
+                    step_df[cc_cap] = np.where(
+                        step_slice[volt_col] < cv_voltage_thresh_mv, delta_cap, 0)
+                    step_df[cv_cap] = np.where(
+                        step_slice[volt_col] >= cv_voltage_thresh_mv, delta_cap, 0)
+                elif step_type == 'discharge':
+                    step_df[[cc_time, cc_cap, cv_time, cv_cap]] = np.nan
+                ez_df = pd.concat([ez_df, step_df])
+        return ez_df
+
+    def __consolidate_temps(self, df):
+        '''
+        Adds thermocouple readings from each data point to an array containing all thermocouple readings.
+
+        Parameters
+        ----------
+        df : pandas.DataFrame
+            DataFrame containing test data.
+
+        Returns
+        -------
+        pd.DataFrame
+            DataFrame containing test data with thermocouple readings in an array.
+        '''
+        thermocouple_cols = [
+            col for col in df.columns if re.search('thermocouple_\d+_c', col)]
+
+        df['thermocouple_temps_c'] = df.apply(
+            lambda row: [row[col] for col in thermocouple_cols], axis=1)
+
+        return df
```

### Comparing `battetl-1.0.2/battetl/utils.py` & `battetl-1.1.0/battetl/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,399 +1,447 @@
-import os
-import re
-import json
-import yaml
-import dotenv
-import logging
-import pandas as pd
-from collections import OrderedDict
-from pydash import get, set_with, unset, merge
-
-from battetl import logger, Constants
-
-
-class Utils:
-    def load_env(env_path: str) -> None:
-        """
-        Set environment variables from .env file
-
-        Parameters
-        ----------
-        env_path : str
-            Path to .env file
-        """
-        logger.info(f'Load environment variables from {env_path}')
-        dotenv.load_dotenv(env_path, override=True)
-        # Set logger level
-        if os.getenv('ENV') == 'dev':
-            logger.info('Set logger level to DEBUG')
-            logger.setLevel(logging.DEBUG)
-
-    def load_config(config_path: str) -> dict:
-        """
-        Load config file from path
-
-        Parameters
-        ----------
-        config_path : str
-            Path to config file
-
-        Returns
-        -------
-        config : dict
-            Config file as dictionary
-        """
-        logger.info(f'Load config file from {config_path}')
-        config = None
-
-        if not os.path.exists(config_path):
-            raise FileNotFoundError(f'Config file not found at {config_path}')
-
-        try:
-            with open(config_path, 'r') as f:
-                config = json.load(f)
-                logger.info('Loaded config file as json')
-                return config
-        except json.decoder.JSONDecodeError:
-            logger.debug('Config file is not json')
-
-        try:
-            with open(config_path, 'r') as f:
-                config = yaml.load(f, Loader=yaml.SafeLoader)
-                logger.info('Loaded config file as yaml')
-                return config
-        except yaml.YAMLError:
-            logger.debug('Config file is not yaml')
-
-        # If we get here, the config file is not json or yaml
-        raise Exception('Config file is not json or yaml')
-
-    def drop_unnamed_columns(df: pd.DataFrame) -> pd.DataFrame:
-        """
-        The function drops unnamed columns from DataFrame
-
-        Parameters
-        ----------
-        df : pandas.DataFrame
-            DataFrame to drop unnamed columns from.
-
-        Returns
-        -------
-        df : pandas.DataFrame
-            Pandas DataFrame with the unnamed columns dropped.
-        """
-        logger.info('Drop unnamed columns')
-        unnamed_column_list = df.filter(like='Unnamed', axis=1).columns
-        df = Utils.drop_columns(df, unnamed_column_list)
-
-        return df
-
-    def drop_columns(df: pd.DataFrame, columns_to_drop: list[str]) -> pd.DataFrame:
-        """
-        This function drops unnamed columns from the passed DataFrame.
-
-        Parameters
-        ----------
-        df : pandas.DataFrame
-            DataFrame to drop unnamed columns from.
-        columns_to_drop : list
-            List of strings that give column names to drop
-
-        Returns
-        -------
-        df : pandas.DataFrame
-            Pandas DataFrame with the dropped columns.
-        """
-        for column in columns_to_drop:
-            if column in df.columns:
-                logger.info(f'Drop column {column}')
-                df = df.drop(columns=column)
-
-        return df
-
-    def get_cycle_make(columns: list) -> tuple[str, str]:
-        """
-        Determine the make and type of cycler.
-        Currently supported:
-        - Arbin Test Data
-        - Arbin Cycle Stats
-        - Maccor Test Data
-        - Maccor Cycle Stats
-
-        Parameters
-        ----------
-        data : list[str]
-            Original data 
-
-        Returns
-        -------
-        (str)
-            Cycle make
-        (str)
-            Data type
-        """
-        columnsSet = Utils.get_lower_strip_set(columns)
-        arbinTestDataSet = Utils.get_lower_strip_set(
-            Constants.COLUMNS_ARBIN_TEST_DATA_ONLY)
-        arbinCycleStatsSet = Utils.get_lower_strip_set(
-            Constants.COLUMNS_ARBIN_CYCLE_STATS_ONLY)
-        maccorTestDataSet = Utils.get_lower_strip_set(
-            Constants.COLUMNS_MACCOR_TEST_DATA_ONLY)
-        maccorTestDataSetType2 = Utils.get_lower_strip_set(
-            Constants.COLUMNS_MACCOR_TEST_DATA_TYPE2_ONLY)
-        maccorCycleStatsSet = Utils.get_lower_strip_set(
-            Constants.COLUMNS_MACCOR_CYCLE_STATS_ONLY)
-
-        if len(columnsSet & arbinTestDataSet) >= (len(arbinTestDataSet) / 2):
-            return Constants.MAKE_ARBIN, Constants.DATA_TYPE_TEST_DATA
-
-        if len(columnsSet & arbinCycleStatsSet) >= (len(arbinCycleStatsSet) / 2):
-            return Constants.MAKE_ARBIN, Constants.DATA_TYPE_CYCLE_STATS
-
-        if len(columnsSet & maccorTestDataSet) >= (len(maccorTestDataSet) / 2):
-            return Constants.MAKE_MACCOR, Constants.DATA_TYPE_TEST_DATA
-
-        if len(columnsSet & maccorTestDataSetType2) >= (len(maccorTestDataSetType2) / 2):
-            return Constants.MAKE_MACCOR, Constants.DATA_TYPE_TEST_DATA
-
-        if len(columnsSet & maccorCycleStatsSet) >= (len(maccorCycleStatsSet) / 2):
-            return Constants.MAKE_MACCOR, Constants.DATA_TYPE_CYCLE_STATS
-
-        return None, None
-
-    def get_lower_strip_set(data: list[str]) -> set:
-        """
-        Transform string list to lower case set
-
-        Parameters
-        ----------
-        data : list[str]
-            Original data 
-
-        Returns
-        -------
-        (set)
-            Lower case set data
-        """
-        return set([d.lower().strip().replace(' ', '').replace('_', '') for d in data])
-
-    def rename_df_columns(df: pd.DataFrame, columnsMapping: dict) -> pd.DataFrame:
-        """
-        Rename column names to BattETL format
-
-        Parameters
-        ----------
-        df : pandas.DataFrame
-            Original data
-
-        Returns
-        -------
-        df : pandas.DataFrame
-            Renamed data
-        """
-        logger.info('Rename column names to BattETL format')
-        logger.debug(f'Columns before renaming: {df.columns.values}')
-
-        # Normalize mapping data
-        mappingTable = {k.lower().strip(): v for k,
-                        v in columnsMapping.items()}
-
-        # Normalize DataFrame columns
-        df.columns = df.columns.str.lower()
-        df.columns = df.columns.str.strip()
-
-        # Rename thermocouple columns
-        for col_name in df.columns.values:
-            match_arbin = re.search(
-                Constants.PREFIX_ARBIN_THERMOCOUPLE+r'(\d)+ \(c\)', col_name)
-            match_maccor = re.search(
-                Constants.PREFIX_MACCOR_THERMOCOUPLE + r'(\d)', col_name)
-            match = (match_arbin or match_maccor)
-            if match:
-                new_col_name = Constants.TEMPLATE_RENAMED_THERMOCOUPLE.replace(
-                    'X', match.group(1))
-                df = df.rename(columns={col_name: new_col_name})
-
-        # Rename to BattETL format
-        df = df.rename(mappingTable, axis='columns')
-        logger.debug(f'Columns after renaming: {df.columns.values}')
-
-        return df
-
-    def convert_to_milli(df: pd.DataFrame) -> pd.DataFrame:
-        """
-        Convert columns to milli- and rename column name
-
-        Parameters
-        ----------
-        df : pandas.DataFrame
-            Original data 
-
-        Returns
-        -------
-        df : pandas.DataFrame
-            Converted data
-        """
-        logger.info('Convert data to milli-')
-        for column in df.columns:
-            if column in Constants.COLUMNS_TO_MILLI:
-                logger.debug(f'Converting {column}')
-                df[column] = df[column].replace(
-                    {',': ''}, regex=True).apply(pd.to_numeric, 1)
-                df[column] = df[column] * 1e3
-                columnName = Constants.COLUMNS_TO_MILLI[column]
-                logger.debug(f'Rename column name to {columnName}')
-                df = df.rename({column: columnName}, axis='columns')
-
-        return df
-
-    def sort_dataframe(df: pd.DataFrame, columns: list[str]) -> pd.DataFrame:
-        """
-        Sort pandas.DataFrame with input columns
-
-        Parameters
-        ----------
-        df : pandas.DataFrame
-            Original data 
-        columns : list[str]
-            Sort by columns
-
-        Returns
-        -------
-        df : pandas.DataFrame
-            Sorted data
-        """
-        logger.info(f'Sort DataFrame by {columns}')
-
-        df = df.sort_values(by=columns)
-        df = df.reset_index(drop=True)
-        logger.debug(f'Sorted rows: {df.shape[0]}')
-
-        return df
-
-    def convert_timedelta_to_seconds(df: pd.DataFrame, column: str) -> pd.DataFrame:
-        """
-        Convert time delta to seconds
-
-        Parameters
-        ----------
-        df : pandas.DataFrame
-            Original data 
-        column : str
-            Column to convert
-
-        Returns
-        -------
-        df : pandas.DataFrame
-            Converted data
-        """
-        logger.info(f'Convert {column} to seconds')
-
-        if column not in df.columns:
-            raise NameError(f'Can not find {column}')
-
-        df[column] = round(pd.to_timedelta(df[column]).dt.total_seconds(), 3)
-
-        return df
-
-    def convert_datetime(df: pd.DataFrame, column: str, timezone: str) -> pd.DataFrame:
-        """
-        Convert datetime to UTC format with time zone
-
-        Parameters
-        ----------
-        df : pandas.DataFrame
-            The input DataFrame
-        column : str
-            column to convert
-        timezone : str
-            Time zone strings in the IANA Time Zone Database
-
-        Returns
-        -------
-        df : pandas.DataFrame
-            Converted data
-        """
-        logger.info(f'Convert {column} to UTC with timezone {timezone}')
-
-        if column not in df.columns:
-            raise NameError(f'Can not find {column}')
-
-        df[column] = Utils.__parse_datetime(df, column)
-        df[column] = df[column].dt.tz_localize(timezone)
-        df[column] = df[column].dt.tz_convert('UTC')
-
-        return df
-
-    def __parse_datetime(df: pd.DataFrame, column: str) -> pd.DataFrame:
-        """
-        Parse datetime with default format to speed up `pandas.to_datetime`
-
-        This function speeds up the `pandas.to_datetime` process time by
-        set the date format instead of traversing each row of data.
-        The function first tries our default formats,
-        and if it doesn't work, it falls back to the original method.
-
-        Parameters
-        ----------
-        df : pandas.DataFrame
-            The input DataFrame
-        column : str
-            column to convert
-
-        Returns
-        -------
-        data : pandas.DataFrame
-            Converted data
-        """
-        format_list = [
-            '\t%m/%d/%Y %H:%M:%S.%f',
-            '%m/%d/%Y %H:%M:%S.%f',
-            '%m/%d/%Y %I:%M:%S %p',
-            '%m/%d/%Y %H:%M:%S',
-        ]
-        for format in format_list:
-            try:
-                data = pd.to_datetime(df[column], format=format)
-                logger.debug(
-                    f'Found datetime format "{format}" for column {column}')
-                return data
-            except:
-                pass
-
-        logger.debug(
-            f'Can not find format in {format_list}, use default')
-        return pd.to_datetime(df[column])
-
-
-class DashOrderedDict(OrderedDict):
-    """
-    Pulled from BEEP:
-    https://github.com/TRI-AMDD/beep/blob/master/beep/utils/__init__.py
-
-    Nested data structure with pydash enabled
-    getters and setters.  Nested values can
-    be set using dot notation, e. g.
-
-    >>> dod = DashOrderedDict()
-    >>> dod.set('key1.key2', 5)
-    >>> print(dod['key1']['key2'])
-    >>> 5
-    """
-
-    def set(self, string, value):
-        set_with(self, string, value, lambda x: OrderedDict())
-
-    def get_path(self, string, default=None):
-        return get(self, string, default=default)
-
-    def unset(self, string):
-        unset(self, string)
-
-    def merge(self, obj):
-        merge(self, obj)
-
-    def __str__(self):
-        return "{}:\n{}".format(self.__class__.__name__, json.dumps(self, indent=4))
-
-    def __repr__(self):
-        return self.__str__()
+import os
+import re
+import json
+import yaml
+import dotenv
+import logging
+import pandas as pd
+from collections import OrderedDict
+from pydash import get, set_with, unset, merge
+
+from battetl import logger, Constants
+
+
+class Utils:
+    def load_env(env_path: str) -> None:
+        """
+        Set environment variables from .env file
+
+        Parameters
+        ----------
+        env_path : str
+            Path to .env file
+        """
+        logger.info(f'Load environment variables from {env_path}')
+        dotenv.load_dotenv(env_path, override=True)
+        # Set logger level
+        if os.getenv('ENV') == 'dev':
+            logger.info('Set logger level to DEBUG')
+            logger.setLevel(logging.DEBUG)
+
+    def load_config(config_path: str) -> dict:
+        """
+        Load config file from path
+
+        Parameters
+        ----------
+        config_path : str
+            Path to config file
+
+        Returns
+        -------
+        config : dict
+            Config file as dictionary
+        """
+        logger.info(f'Load config file from {config_path}')
+        config = None
+
+        if not os.path.exists(config_path):
+            raise FileNotFoundError(f'Config file not found at {config_path}')
+
+        try:
+            with open(config_path, 'r') as f:
+                config = json.load(f)
+                logger.info('Loaded config file as json')
+                return config
+        except json.decoder.JSONDecodeError:
+            logger.debug('Config file is not json')
+
+        try:
+            with open(config_path, 'r') as f:
+                config = yaml.load(f, Loader=yaml.SafeLoader)
+                logger.info('Loaded config file as yaml')
+                return config
+        except yaml.YAMLError:
+            logger.debug('Config file is not yaml')
+
+        # If we get here, the config file is not json or yaml
+        raise Exception('Config file is not json or yaml')
+
+    def drop_unnamed_columns(df: pd.DataFrame) -> pd.DataFrame:
+        """
+        The function drops unnamed columns from DataFrame
+
+        Parameters
+        ----------
+        df : pandas.DataFrame
+            DataFrame to drop unnamed columns from.
+
+        Returns
+        -------
+        df : pandas.DataFrame
+            Pandas DataFrame with the unnamed columns dropped.
+        """
+        logger.info('Drop unnamed columns')
+        unnamed_column_list = df.filter(like='Unnamed', axis=1).columns
+        df = Utils.drop_columns(df, unnamed_column_list)
+
+        return df
+
+    def drop_columns(df: pd.DataFrame, columns_to_drop: list[str]) -> pd.DataFrame:
+        """
+        This function drops unnamed columns from the passed DataFrame.
+
+        Parameters
+        ----------
+        df : pandas.DataFrame
+            DataFrame to drop unnamed columns from.
+        columns_to_drop : list
+            List of strings that give column names to drop
+
+        Returns
+        -------
+        df : pandas.DataFrame
+            Pandas DataFrame with the dropped columns.
+        """
+        for column in columns_to_drop:
+            if column in df.columns:
+                logger.info(f'Drop column {column}')
+                df = df.drop(columns=column)
+
+        return df
+
+    def drop_empty_rows(df: pd.DataFrame) -> pd.DataFrame:
+        """
+        The function drops empty rows from DataFrame
+
+        Parameters
+        ----------
+        df : pandas.DataFrame
+            DataFrame to drop empty rows from.
+
+        Returns
+        -------
+        df : pandas.DataFrame
+            Pandas DataFrame with the empty rows dropped.
+        """
+        all_na_count = (df.isna().all(axis=1)).sum()
+        if all_na_count > 0:
+            logger.info(f'Drop {all_na_count} empty rows')
+            df = df.dropna(how='all')
+
+        return df
+
+    def get_cycle_make(columns: list) -> tuple[str, str]:
+        """
+        Determine the make and type of cycler.
+        Currently supported:
+        - Arbin Test Data
+        - Arbin Cycle Stats
+        - Maccor Test Data
+        - Maccor Cycle Stats
+
+        Parameters
+        ----------
+        data : list[str]
+            Original data 
+
+        Returns
+        -------
+        (str)
+            Cycle make
+        (str)
+            Data type
+        """
+        columnsSet = Utils.get_lower_strip_set(columns)
+        arbinTestDataSet = Utils.get_lower_strip_set(
+            Constants.COLUMNS_ARBIN_TEST_DATA_ONLY)
+        arbinCycleStatsSet = Utils.get_lower_strip_set(
+            Constants.COLUMNS_ARBIN_CYCLE_STATS_ONLY)
+        maccorTestDataSet = Utils.get_lower_strip_set(
+            Constants.COLUMNS_MACCOR_TEST_DATA_ONLY)
+        maccorTestDataSetType2 = Utils.get_lower_strip_set(
+            Constants.COLUMNS_MACCOR_TEST_DATA_TYPE2_ONLY)
+        maccorTestDataSetCustomer1 = Utils.get_lower_strip_set(
+            Constants.COLUMNS_MACCOR_TEST_DATA_CUSTOMER1)
+        maccorCycleStatsSet = Utils.get_lower_strip_set(
+            Constants.COLUMNS_MACCOR_CYCLE_STATS_ONLY)
+        maccorCycleStatsSetCustomer1 = Utils.get_lower_strip_set(
+            Constants.COLUMNS_MACCOR_CYCLE_STATS_CUSTOMER1)
+
+        if len(columnsSet & arbinTestDataSet) >= (len(arbinTestDataSet) / 2):
+            return Constants.MAKE_ARBIN, Constants.DATA_TYPE_TEST_DATA
+
+        if len(columnsSet & arbinCycleStatsSet) >= (len(arbinCycleStatsSet) / 2):
+            return Constants.MAKE_ARBIN, Constants.DATA_TYPE_CYCLE_STATS
+
+        if len(columnsSet & maccorTestDataSet) >= (len(maccorTestDataSet) / 2):
+            return Constants.MAKE_MACCOR, Constants.DATA_TYPE_TEST_DATA
+
+        if len(columnsSet & maccorTestDataSetType2) >= (len(maccorTestDataSetType2) / 2):
+            return Constants.MAKE_MACCOR, Constants.DATA_TYPE_TEST_DATA
+
+        if len(columnsSet & maccorTestDataSetCustomer1) >= (len(maccorTestDataSetCustomer1) / 2):
+            return Constants.MAKE_MACCOR, Constants.DATA_TYPE_TEST_DATA
+
+        if len(columnsSet & maccorCycleStatsSet) >= (len(maccorCycleStatsSet) / 2):
+            return Constants.MAKE_MACCOR, Constants.DATA_TYPE_CYCLE_STATS
+
+        if len(columnsSet & maccorCycleStatsSetCustomer1) >= (len(maccorCycleStatsSetCustomer1) / 2):
+            return Constants.MAKE_MACCOR, Constants.DATA_TYPE_CYCLE_STATS
+
+        return None, None
+
+    def get_lower_strip_set(data: list[str]) -> set:
+        """
+        Transform string list to lower case set
+
+        Parameters
+        ----------
+        data : list[str]
+            Original data 
+
+        Returns
+        -------
+        (set)
+            Lower case set data
+        """
+        return set([d.lower().strip().replace(' ', '').replace('_', '') for d in data])
+
+    def rename_df_columns(df: pd.DataFrame, columnsMapping: dict) -> pd.DataFrame:
+        """
+        Rename column names to BattETL format
+
+        Parameters
+        ----------
+        df : pandas.DataFrame
+            Original data
+
+        Returns
+        -------
+        df : pandas.DataFrame
+            Renamed data
+        """
+        logger.info('Rename column names to BattETL format')
+        logger.debug(f'Columns before renaming: {df.columns.values}')
+
+        # Normalize mapping data
+        mappingTable = {k.lower().strip(): v for k,
+                        v in columnsMapping.items()}
+
+        # Normalize DataFrame columns
+        df.columns = df.columns.str.lower()
+        df.columns = df.columns.str.strip()
+
+        # Rename thermocouple columns
+        for col_name in df.columns.values:
+            match_arbin = re.search(
+                Constants.PREFIX_ARBIN_THERMOCOUPLE+r'(\d)+ \(c\)', col_name)
+            match_maccor = re.search(
+                Constants.PREFIX_MACCOR_THERMOCOUPLE + r'(\d)', col_name)
+            match = (match_arbin or match_maccor)
+            if match:
+                new_col_name = Constants.TEMPLATE_RENAMED_THERMOCOUPLE.replace(
+                    'X', match.group(1))
+                df = df.rename(columns={col_name: new_col_name})
+
+        # Rename to BattETL format
+        df = df.rename(mappingTable, axis='columns')
+        logger.debug(f'Columns after renaming: {df.columns.values}')
+
+        return df
+
+    def convert_to_milli(df: pd.DataFrame) -> pd.DataFrame:
+        """
+        Convert columns to milli- and rename column name
+
+        Parameters
+        ----------
+        df : pandas.DataFrame
+            Original data 
+
+        Returns
+        -------
+        df : pandas.DataFrame
+            Converted data
+        """
+        logger.info('Convert data to milli-')
+        for column in df.columns:
+            if column in Constants.COLUMNS_TO_MILLI:
+                logger.debug(f'Converting {column}')
+                df[column] = df[column].replace(
+                    {',': ''}, regex=True).apply(pd.to_numeric, 1)
+                df[column] = df[column] * 1e3
+                columnName = Constants.COLUMNS_TO_MILLI[column]
+                logger.debug(f'Rename column name to {columnName}')
+                df = df.rename({column: columnName}, axis='columns')
+
+        return df
+
+    def sort_dataframe(df: pd.DataFrame, columns: list[str]) -> pd.DataFrame:
+        """
+        Sort pandas.DataFrame with input columns
+
+        Parameters
+        ----------
+        df : pandas.DataFrame
+            Original data 
+        columns : list[str]
+            Sort by columns
+
+        Returns
+        -------
+        df : pandas.DataFrame
+            Sorted data
+        """
+        logger.info(f'Sort DataFrame by {columns}')
+
+        df = df.sort_values(by=columns)
+        df = df.reset_index(drop=True)
+        logger.debug(f'Sorted rows: {df.shape[0]}')
+
+        return df
+
+    def convert_timedelta_to_seconds(df: pd.DataFrame, column: str) -> pd.DataFrame:
+        """
+        Convert time delta to seconds
+
+        Parameters
+        ----------
+        df : pandas.DataFrame
+            Original data 
+        column : str
+            Column to convert
+
+        Returns
+        -------
+        df : pandas.DataFrame
+            Converted data
+        """
+        logger.info(f'Convert {column} to seconds')
+
+        if column not in df.columns:
+            raise NameError(f'Can not find {column}')
+
+        df[column] = round(pd.to_timedelta(df[column]).dt.total_seconds(), 3)
+
+        return df
+
+    def convert_datetime(df: pd.DataFrame, column: str, timezone: str) -> pd.DataFrame:
+        """
+        Convert datetime to UTC format with time zone
+
+        Parameters
+        ----------
+        df : pandas.DataFrame
+            The input DataFrame
+        column : str
+            column to convert
+        timezone : str
+            Time zone strings in the IANA Time Zone Database
+
+        Returns
+        -------
+        df : pandas.DataFrame
+            Converted data
+        """
+        logger.info(f'Convert {column} to UTC with timezone {timezone}')
+
+        if column not in df.columns:
+            raise NameError(f'Can not find {column}')
+
+        df[column] = Utils.__parse_datetime(df, column)
+        df[column] = df[column].dt.tz_localize(timezone)
+        df[column] = df[column].dt.tz_convert('UTC')
+
+        return df
+
+    def __parse_datetime(df: pd.DataFrame, column: str) -> pd.DataFrame:
+        """
+        Parse datetime with default format to speed up `pandas.to_datetime`
+
+        This function speeds up the `pandas.to_datetime` process time by
+        set the date format instead of traversing each row of data.
+        The function first tries our default formats,
+        and if it doesn't work, it falls back to the original method.
+
+        Parameters
+        ----------
+        df : pandas.DataFrame
+            The input DataFrame
+        column : str
+            column to convert
+
+        Returns
+        -------
+        data : pandas.DataFrame
+            Converted data
+        """
+        format_list = [
+            '\t%m/%d/%Y %H:%M:%S.%f',
+            '%m/%d/%Y %H:%M:%S.%f',
+            '%m/%d/%Y %I:%M:%S %p',
+            '%m/%d/%Y %H:%M:%S',
+        ]
+        for format in format_list:
+            try:
+                data = pd.to_datetime(df[column], format=format)
+                logger.debug(
+                    f'Found datetime format "{format}" for column {column}')
+                return data
+            except:
+                pass
+
+        logger.debug(
+            f'Can not find format in {format_list}, use default')
+        return pd.to_datetime(df[column])
+
+    def convert_to_float(value):
+        '''
+        Converts value to float if it is a string.
+
+        Parameters
+        ----------
+        value : str or float
+            The value to convert.
+
+        Returns
+        -------
+        float
+        '''
+        if isinstance(value, str):
+            return float(value.replace(',', ''))
+        return value
+
+
+class DashOrderedDict(OrderedDict):
+    """
+    Pulled from BEEP:
+    https://github.com/TRI-AMDD/beep/blob/master/beep/utils/__init__.py
+
+    Nested data structure with pydash enabled
+    getters and setters.  Nested values can
+    be set using dot notation, e. g.
+
+    >>> dod = DashOrderedDict()
+    >>> dod.set('key1.key2', 5)
+    >>> print(dod['key1']['key2'])
+    >>> 5
+    """
+
+    def set(self, string, value):
+        set_with(self, string, value, lambda x: OrderedDict())
+
+    def get_path(self, string, default=None):
+        return get(self, string, default=default)
+
+    def unset(self, string):
+        unset(self, string)
+
+    def merge(self, obj):
+        merge(self, obj)
+
+    def __str__(self):
+        return "{}:\n{}".format(self.__class__.__name__, json.dumps(self, indent=4))
+
+    def __repr__(self):
+        return self.__str__()
```

### Comparing `battetl-1.0.2/battetl.egg-info/PKG-INFO` & `battetl-1.1.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,329 +1,343 @@
-Metadata-Version: 2.1
-Name: battetl
-Version: 1.0.2
-Summary: A Python module for extracting, transforming, and loading battery data to a database.
-Home-page: https://github.com/BattGenie/battetl
-Author: Zander Nevitt, Bing Syuan Wang and Chintan Pathak
-Author-email: info@battgenie.life
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9, <3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/BattETL_Logo.png">
-
-# BattETL
-
-BattETL is a well-tested and an enterprise-ready python module for **E**xtracting, **T**ransforming, and **L**oading battery cycler data to a [database](https://github.com/BattGenie/battdb). BattETL can also be used just for data extraction and transformation if a database is not desired. Currently data from Maccor and Arbin cyclers are supported.
-
-<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/BattETL_Simple_System.svg">
-
-## Overview
-
-- [Motivation](#motivation)
-- [Video Guides](#video-guides)
-- [Installation](#installation)
-  - [Requirements](#requirements)
-  - [Installation Instructions](#installation-instructions)
-- [Usage](#usage)
-  - [Config File](#config-file)
-  - [Env File](#env-file)
-  - [Data Export Requirements](#data-export-requirements)
-    - [Maccor](#maccor)
-    - [Arbin](#arbin)
-- [BattETL Overview](#battetl-overview)
-  - [System Diagram](#system-diagram)
-  - [Transformer](#transformer)
-  - [Extractor](#extractor)
-  - [Loader](#loader)
-- [Testing](#testing)
-- [Troubleshooting](#troubleshooting)
-
-## Motivation
-
-### Why another battery cycler data ingesting tool?
-
-There are published [open](https://github.com/TRI-AMDD/beep) [source](https://github.com/Battery-Intelligence-Lab/galvanalyser) solutions for battery cycler data ingestion. BattETL hopes to build on these tools and adds a few conveniences to support robust data management and repeatable data analytics.
-
-### Some features of BattETL
-
-- **A relational data destination.**
-
-BattETL package is tightly coupled to the destination database it sends the data to. BattETL requires that for the battery data that is loaded to the database - the detailed metadata such as battery make and model, cycler make and model, and schedule/procedure information be also included. While these constraints (somewhat) slowdown the data ingestion process, it ensures verifiable, high-quality data persistance.
-
-- **A database that can hold *all* relevant battery test information.**
-
-Not only does the BattETL extract and store all the battery test data, it also captures the cycler schedule/procedure file. In addition to the schedule/procedure file, BattETL captures and stores all files associated with the schedule/procedure. This includes any current profiles (Maccor FastWave or Arbin current simulation files), EIS specifications, or even entire system specifications (Arbin batch files.)
-
-- **Analytics built into the transformation step.**
-
-As part of the transformation step BattETL calculates various cycle statistics (capacity, coulombic efficiency, CC/CV charge times, etc.) providing independent and supplemental cycle statistics to compliment those generated by the cycler software. These can particularly handy when easy-to-miss settings were overlooked in writing the schedule (e.g. forgetting to reset the capacity when incriminating the cycle.) Do you have some sort of hyper-boutique transformation or statistic calculation needed for a specific test? No problem. BattETL can apply user defined transformation functions too; all before the data is loaded to the database.
-
-## Video Guides
-
-The following are video guides BattETL and BattDB:
-
-- [Installation & setup](https://www.youtube.com/watch?v=tmudLhrj9xE)
-- [Design overview](https://www.youtube.com/watch?v=Y2tXInbkYF8)
-- [Demonstration](https://www.youtube.com/watch?v=3wNd3fhqBwo)
-
-## Installation
-
-A video showing how to setup and install BattETL and BattDB can be found [here](https://www.youtube.com/watch?v=tmudLhrj9xE)
-
-### Requirements
-
-#### Software Requirements
-
-- Python 3.9 or 3.10
-- The required packages are listed in the `requirements.txt` file
-
-#### Hardware Requirements
-
-Based on processing approximately 10,000 rows and 12 columns with Pandas, BattETL requires a minimum of 13MB of RAM.
-
-- RAM: 2 GB or higher.
-- Disk Space: At least 2 GB of free space is recommended to accommodate the transformed data, as well as additional space for installation and storing data. The exact amount of disk space required will depend on the size of the data being processed and the resulting intermediate results.
-
-### Installation Instructions
-
-- Install BattETL using pip:
-
-```sh
-pip install battetl
-```
-
-- Install BattETL from source code:
-
-```sh
-git clone https://github.com/BattGenie/battetl.git
-cd battetl
-pip install -r requirements.txt
-pip install .
-```
-
-> Note that if you wish to use the Load feature of BattETL it is necessary to deploy an instance of a [BattDB](https://github.com/BattGenie/battdb) database to load the data to. Follow the instructions there for deploying the database.
-
-## Usage
-
-A video demonstrating how to use BattETL and BattDB can be found [here](https://www.youtube.com/watch?v=3wNd3fhqBwo)
-
-Using BattETL as an all-in-one ETL function is as easy as:
-
-```python
-from battetl import BattETL
-
-cell = BattETL(config_path).extract().transform().load()
-```
-
-Where `config_path` is the absolute or relative path to BattETL [config file](#config-file).
-
-It is also necessary to include an [.env file](#env-file) within the working directory that contains the associated database credentials.
-
-Finally, the data must be exported from the cycler in a [specific format](#data-export-requirements)
-
-For a practical implementation of `BattETL`, please refer to the example notebook `examples/battetl_demo.ipynb` located in the `examples` directory. This notebook demonstrates how to implement `BattETL` and can serve as a useful reference for your own project.
-
-> Note that repeated calls to load test data that already exists in the database (as determined by unix timestamp) will not overwrite any existing data. Only test data after the most recent existing unix timestamp will be loaded. In the case of loading cycle statistics, any duplicate cycles that already exist in the database will be overwritten.
-
-### Config File
-
-To use BattETL it is necessary to provide a path to JSON configuration file. This config file contains paths to the relevant test data files and test metadata used for analysis and establishing database relations. An example configuration file is given within `examples/battetl_config_example.json`
-
-```json
-{
-    "timezone": "America/Los_Angeles",
-    "data_file_path": [
-        "abs/path/to/your/arbin/or/maccor/test/data/file(s).txt"
-    ],
-    "stats_file_path": [
-        "abs/path/to/your/arbin/or/maccor/test/stats/file.txt"
-    ],
-    "schedule_file_path": [
-        "abs/path/to/your/schedule/or/procedure/file(s).000"
-    ],
-    "meta_data": {
-        "test_meta": {
-            "test_name": "the_name_of_your_test",
-            "channel": 10
-        },
-        "cell": {
-            "manufacturer_sn": "0001"
-        },
-        "cell_meta": {
-            "manufacturer": "FakeMN",
-            "manufacturer_pn": "1234"
-        },
-        "schedule_meta": {
-            "schedule_name": "fake_schedule.000",
-            "cycler_make": "BattGenie"
-        },
-        "cycler": {
-            "sn": "0001"
-        },
-        "cycler_meta": {
-            "manufacturer": "BattGenie",
-            "model": "Cycler9000"
-        }
-    }
-}
-```
-
-### Env File
-
-The .env contains the associated database credentials and is formatted as follows
-
-```
-ENV=dev # dev, prod
-DB_TARGET=YOUR_DATABASE_NAME
-DB_USERNAME=YOUR_USERNAME
-DB_PASSWORD=YOUR_PASSWORD
-DB_HOSTNAME=localhost
-DB_PORT=5432
-```
-
-An example .env file is given within `examples/.env.example`
-
-### Data Export Requirements
-
-- [For Maccor Cycler](#maccor)
-- [For Arbin Cycler](#arbin)
-
-#### Maccor
-
-From the "Maccor Export" tool data should be exported as "Text Output" in a "Tab Delimited" format. The output sheets should include "Data Records" and "Cycle Statistics". The box for "Discharge Current Exported Negative" should be checked.
-
-The following columns are the minimum required for export:
-
-For Data Records:
-
-- Cycle : Header Label of Cyc#
-- Step : Header Label of Step
-- Test Time : Header Label of TestTime(s), Units of seconds
-- Step Time : Header Label of StepTime(s), Units of seconds
-- Capacity : Header Label of Capacity(Ah), Units of Amp-Hour
-- Energy : Header Label of Watt-hr, Units of Watt-hour
-- Current : Header Label of Current(A), Units of Amps
-- Voltage : Header Label of Voltage(V), Units of Volts
-- DPT Time : Header label of DPt Time
-
-<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/MaccorExport_DataRecords.png" width="85%" height="50%">
-
-For Cycle Statistics:
-
-- Cycle : Header Label of Cycle
-- Capacity Chg : Header label AH-IN, Units of Ahr
-- Capacity Dis : Header label AH-Out, Units of Ahr
-- DPT Time : Header Label of DPt Time
-
-<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/MaccorExport_CycleStats.png" width="85%" height="50%">
-
-#### Arbin
-
-Within the Arbin Export tool the "File Type" should be set to "To CSV". Within "Data Filter" the box "statistics by Cycle" should be checked along with any other data. For range filter "All" should be selected.
-
-<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/ArbinExport.jpg" width="45%" height="25%">
-
-An example notebook `battetl_demo.ipynb` that provides a tool to help generate config files is located in the `examples` directory.
-
-## BattETL Overview
-
-A video discussing the design of BattDB and BattETL can be found [here](https://www.youtube.com/watch?v=Y2tXInbkYF8)
-
-BattETL bundles together the three independent submodules:
-
-- [Extractor](#extractor) : Responsible for extractor the cycler data and schedule/procedure files.
-- [Transformer](#transformer) : Responsible for transforming cycler data
-- [Loader](#loader) : Responsible for loading data and associated data to the database.
-
-After running BattETL on a specific configuration file the following objects will be available as class variables from the instance:
-
-- `raw_test_data: pandas.DataFrame`: The raw test data exactly as it is in the generated cycler data file(s).
-- `raw_cycle_stats: pandas.DataFrame`: The raw cycle stats data exactly as it is in the generated cycler statistics file.
-- `test_data: pandas.DataFrame`: The transformed test data after normalizing units and datatype and adding a unixtime column.
-- `cycle_stats: pandas.DataFrame`: The transformed cycle stats after normalizing units, datatypes, and calculating supplemental cycle statistics.
-- `schedule: dict`: The procedure/schedule file and all associated files in a nested Dictionary.
-
-### System diagram
-
-<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/BattETL_SystemDiagram.svg">
-
-### Extractor
-
-The Extractor is an interface that allows you to extract battery test data from raw data files. You can extract test data and cycle stats data from multiple files using `data_from_files`, and extract Arbin schedules or Maccor procedures and associated files using `schedule_from_files`.
-
-For an example of the Extractor as a standalone class, see `examples/submodule_demos/Extractor_demo.ipynb`
-
-#### Functions
-
-- `data_from_files(paths: list[str])`: Extracts multiple test data files into a single pandas DataFrame.  
-- `schedule_from_files(paths: list[str])`: Extracts Arbin schedules or Maccor procedures and associated files and stores them in a dictionary.  
-- `from_pickle(path: str)`: Reads data from the passed file path and returns it as a pandas DataFrame.  
-
-#### Variables
-
-- `cycler_make: str`: Cycler make  
-- `raw_test_data_meta_data: list[dict]`: Test data meta data  
-- `raw_cycle_stats_meta_data: list[dict]`: Cycler stats meta data  
-- `raw_test_data: pandas.DataFrame`: Test data  
-- `raw_cycle_stats: pandas.DataFrame`: Cycler stats  
-- `maccor_procedure: dict`: Maccor procedure  
-- `arbin_schedule: dict`: Arbin schedule  
-
-### Transformer
-
-The Transformer is an interface that allows you to transform battery test data to the BattETL schema. By default, the time zone is set to 'America/Los_Angeles', but you can modify it to your preferred time zone using the names found in the [IANA Time Zone Database](https://www.iana.org/time-zones). In addition to the default functions provided by the Transformer, you can add your own custom functions to perform specific transformations on your data.
-
-For an example of the Extractor as a standalone class, see `examples/submodule_demos/Transformer_demo.ipynb`
-
-#### Functions
-
-- `transform_test_data(self, data: pd.DataFrame)`: Transforms test data to conform to BattETL naming and data conventions  
-- `transform_cycle_stats`: Transforms cycle stats to conform to BattETL naming and data conventions  
-
-#### Variables
-
-- `timezone: str`: Time zone strings in the IANA Time Zone Database. Used to convert to unix timestamp in seconds. Default 'America/Los_Angeles'.  
-- `user_transform_test_data`: A user defined function to transform test data. The function should take a pandas.DataFrame as input and return a pandas.DataFrame as output.  
-- `user_transform_cycle_stats`: A user defined function to transform cycle stats. The function should take a pandas.DataFrame as input and return a pandas.DataFrame as output.  
-- `test_data: pandas.DataFrame`: Transformed test data  
-- `cycle_stats: pandas.DataFrame`: Transformed cycle stats  
-
-### Loader
-
-The `load` module provides an interface to load the extracted data into a database.
-
-Note that repeated calls to load test data that already exists in the database (as determined by unix timestamp) will not overwrite any existing data. Only test data after the latest existing unix timestamp will be loaded. In the case of loading cycle statistics, any duplicate cycles that already exist in the database will be overwritten.
-
-For an example of the Extractor as a standalone class, see `examples/submodule_demos/Loader_demo.ipynb`
-
-#### Functions
-
-- `load_test_data(test_data_df)`: Loads test_data_df to `test_data` table in the specified database.  
-- `load_cycle_stats(cycle_stats_df)`: Loads cycle_stats_df to `test_data_cycle_stats` table in the specified database.  
-
-## Testing
-
-To run the test suite, use the following commands:
-
-- Run all tests: `pytest`
-- Run Maccor tests: `pytest -m maccor`
-- Run Arbin tests: `pytest -m arbin`
-- Run database specific tests: `pytest -m database`
-- Run tests other than Arbin: `pytest -m "not arbin"`
-- Run Extractor tests: `pytest tests/test_extract_data.py`
-
-To show logs while testing, add the `-o log_cli=true` flag.
-
-## Troubleshooting
-
-### pip install psycopg2 error
-
-If there is an error `Error: pg_config executable not found.` Try installing `libpq-dev` before installing `psycopg2`
-
-```sh
-sudo apt install libpq-dev
-```
+<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/BattETL_Logo.png">
+
+# BattETL
+
+BattETL is a well-tested and an enterprise-ready python module for **E**xtracting, **T**ransforming, and **L**oading battery cycler data to a [database](https://github.com/BattGenie/battdb). BattETL can also be used just for data extraction and transformation if a database is not desired. Currently data from Maccor and Arbin cyclers are supported.
+
+<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/BattETL_Simple_System.svg">
+
+## Overview
+
+- [Motivation](#motivation)
+- [Video Guides](#video-guides)
+- [Installation](#installation)
+  - [Requirements](#requirements)
+  - [Installation Instructions](#installation-instructions)
+- [Usage](#usage)
+  - [Quick Mode](#quick-mode)
+  - [Config File](#config-file)
+  - [Env File](#env-file)
+  - [Data Export Requirements](#data-export-requirements)
+    - [Maccor](#maccor)
+    - [Arbin](#arbin)
+- [BattETL Overview](#battetl-overview)
+  - [System Diagram](#system-diagram)
+  - [Transformer](#transformer)
+  - [Extractor](#extractor)
+  - [Loader](#loader)
+- [Testing](#testing)
+- [Troubleshooting](#troubleshooting)
+
+## Motivation
+
+### Why another battery cycler data ingesting tool?
+
+There are published [open](https://github.com/TRI-AMDD/beep) [source](https://github.com/Battery-Intelligence-Lab/galvanalyser) solutions for battery cycler data ingestion. BattETL hopes to build on these tools and adds a few conveniences to support robust data management and repeatable data analytics.
+
+### Some features of BattETL
+
+- **A relational data destination.**
+
+BattETL package is tightly coupled to the destination database it sends the data to. BattETL requires that for the battery data that is loaded to the database - the detailed metadata such as battery make and model, cycler make and model, and schedule/procedure information be also included. While these constraints (somewhat) slowdown the data ingestion process, it ensures verifiable, high-quality data persistance.
+
+- **A database that can hold *all* relevant battery test information.**
+
+Not only does the BattETL extract and store all the battery test data, it also captures the cycler schedule/procedure file. In addition to the schedule/procedure file, BattETL captures and stores all files associated with the schedule/procedure. This includes any current profiles (Maccor FastWave or Arbin current simulation files), EIS specifications, or even entire system specifications (Arbin batch files.)
+
+- **Analytics built into the transformation step.**
+
+As part of the transformation step BattETL calculates various cycle statistics (capacity, coulombic efficiency, CC/CV charge times, etc.) providing independent and supplemental cycle statistics to compliment those generated by the cycler software. These can particularly handy when easy-to-miss settings were overlooked in writing the schedule (e.g. forgetting to reset the capacity when incriminating the cycle.) Do you have some sort of hyper-boutique transformation or statistic calculation needed for a specific test? No problem. BattETL can apply user defined transformation functions too; all before the data is loaded to the database.
+
+## Video Guides
+
+The following are video guides BattETL and BattDB:
+
+- [Installation & setup](https://www.youtube.com/watch?v=tmudLhrj9xE)
+- [Design overview](https://www.youtube.com/watch?v=Y2tXInbkYF8)
+- [Demonstration](https://www.youtube.com/watch?v=3wNd3fhqBwo)
+
+## Installation
+
+A video showing how to setup and install BattETL and BattDB can be found [here](https://www.youtube.com/watch?v=tmudLhrj9xE)
+
+### Requirements
+
+#### Software Requirements
+
+- Python 3.9 or 3.10
+- The required packages are listed in the `requirements.txt` file
+
+#### Hardware Requirements
+
+Based on processing approximately 10,000 rows and 12 columns with Pandas, BattETL requires a minimum of 13MB of RAM.
+
+- RAM: 2 GB or higher.
+- Disk Space: At least 2 GB of free space is recommended to accommodate the transformed data, as well as additional space for installation and storing data. The exact amount of disk space required will depend on the size of the data being processed and the resulting intermediate results.
+
+### Installation Instructions
+
+- Install BattETL using pip:
+
+```sh
+pip install battetl
+```
+
+- Install BattETL from source code:
+
+```sh
+git clone https://github.com/BattGenie/battetl.git
+cd battetl
+pip install -r requirements.txt
+pip install .
+```
+
+> Note that if you wish to use the Load feature of BattETL it is necessary to deploy an instance of a [BattDB](https://github.com/BattGenie/battdb) database to load the data to. Follow the instructions there for deploying the database.
+
+## Usage
+
+A video demonstrating how to use BattETL and BattDB can be found [here](https://www.youtube.com/watch?v=3wNd3fhqBwo)
+
+Using BattETL as an all-in-one ETL function is as easy as:
+
+```python
+from battetl import BattETL
+
+cell = BattETL(config_path).extract().transform().load()
+```
+
+Where `config_path` is the absolute or relative path to BattETL [config file](#config-file).
+
+It is also necessary to include an [.env file](#env-file) within the working directory that contains the associated database credentials.
+
+Finally, the data must be exported from the cycler in a [specific format](#data-export-requirements)
+
+For a practical implementation of `BattETL`, please refer to the example notebook `examples/battetl_demo.ipynb` located in the `examples` directory. This notebook demonstrates how to implement `BattETL` and can serve as a useful reference for your own project.
+
+> Note that repeated calls to load test data that already exists in the database (as determined by unix timestamp) will not overwrite any existing data. Only test data after the most recent existing unix timestamp will be loaded. In the case of loading cycle statistics, any duplicate cycles that already exist in the database will be overwritten.
+
+### Quick Mode
+
+BattETL provides a Quick Mode, which automatically detects whether the given file is test data or test stats from a Maccor or an Arbin cycler, and uploads it to the database accordingly. Here's an example command line:
+
+```bash
+python -m battetl.battetl_quick file="TEST_DATA.txt" db_url="postgres://postgres:password@localhost:5454/battdb_quick"
+```
+
+This command relies on [BattDB](https://github.com/BattGenie/BattDB). If BattDB does not exist, a database will be created using Docker Compose and the data will be uploaded to it. The command also returns a harmonized Pandas dataframe that can be used for analysis and visualization. 
+
+### Config File
+
+To use BattETL it is necessary to provide a path to JSON configuration file. This config file contains paths to the relevant test data files and test metadata used for analysis and establishing database relations. An example configuration file is given within `examples/battetl_config_example.json`
+
+```json
+{
+    "timezone": "America/Los_Angeles",
+    "data_file_path": [
+        "abs/path/to/your/arbin/or/maccor/test/data/file(s).txt"
+    ],
+    "stats_file_path": [
+        "abs/path/to/your/arbin/or/maccor/test/stats/file.txt"
+    ],
+    "schedule_file_path": [
+        "abs/path/to/your/schedule/or/procedure/file(s).000"
+    ],
+    "meta_data": {
+        "test_meta": {
+            "test_name": "the_name_of_your_test",
+            "channel": 10
+        },
+        "cell": {
+            "manufacturer_sn": "0001"
+        },
+        "cell_meta": {
+            "manufacturer": "FakeMN",
+            "manufacturer_pn": "1234"
+        },
+        "schedule_meta": {
+            "schedule_name": "fake_schedule.000",
+            "cycler_make": "BattGenie"
+        },
+        "cycler": {
+            "sn": "0001"
+        },
+        "cycler_meta": {
+            "manufacturer": "BattGenie",
+            "model": "Cycler9000"
+        },
+        "customers": {
+            "customer_name": "FakeCustomer"
+        },
+        "projects": {
+            "project_name": "FakeProject"
+        }
+    }
+}
+```
+
+#### Cell Thermocouple (optional)
+
+If the cell has a thermocouple, it is necessary to include the following in the header of the config file:
+
+```json
+"cell_thermocouple": 1
+```
+
+where `1` corresponds to the thermocouple index in the cycler test data export, i.e `Temp 1` for Maccor and `Aux_Temperature_1 (C)` for Arbin.
+
+If no cell thermocouple value is listed, `calculated_max_charge_temp_c` and `calculated_max_discharge_temp_c` will be set to `null` in the `test_data_cycle_stats` table.
+
+### Env File
+
+The .env contains the associated database credentials and is formatted as follows
+
+```text
+ENV=dev # dev, prod
+DB_TARGET=YOUR_DATABASE_NAME
+DB_USERNAME=YOUR_USERNAME
+DB_PASSWORD=YOUR_PASSWORD
+DB_HOSTNAME=localhost
+DB_PORT=5432
+```
+
+An example .env file is given within `examples/.env.example`
+
+### Data Export Requirements
+
+- [For Maccor Cycler](#maccor)
+- [For Arbin Cycler](#arbin)
+
+#### Maccor
+
+From the "Maccor Export" tool data should be exported as "Text Output" in a "Tab Delimited" format. The output sheets should include "Data Records" and "Cycle Statistics". The box for "Discharge Current Exported Negative" should be checked.
+
+The following columns are the minimum required for export:
+
+For Data Records:
+
+- Cycle : Header Label of Cyc#
+- Step : Header Label of Step
+- Test Time : Header Label of TestTime(s), Units of seconds
+- Step Time : Header Label of StepTime(s), Units of seconds
+- Capacity : Header Label of Capacity(Ah), Units of Amp-Hour
+- Energy : Header Label of Watt-hr, Units of Watt-hour
+- Current : Header Label of Current(A), Units of Amps
+- Voltage : Header Label of Voltage(V), Units of Volts
+- DPT Time : Header label of DPt Time
+
+<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/MaccorExport_DataRecords.png" width="85%" height="50%">
+
+For Cycle Statistics:
+
+- Cycle : Header Label of Cycle
+- Capacity Chg : Header label AH-IN, Units of Ahr
+- Capacity Dis : Header label AH-Out, Units of Ahr
+- DPT Time : Header Label of DPt Time
+
+<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/MaccorExport_CycleStats.png" width="85%" height="50%">
+
+#### Arbin
+
+Within the Arbin Export tool the "File Type" should be set to "To CSV". Within "Data Filter" the box "statistics by Cycle" should be checked along with any other data. For range filter "All" should be selected.
+
+<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/ArbinExport.jpg" width="45%" height="25%">
+
+An example notebook `battetl_demo.ipynb` that provides a tool to help generate config files is located in the `examples` directory.
+
+## BattETL Overview
+
+A video discussing the design of BattDB and BattETL can be found [here](https://www.youtube.com/watch?v=Y2tXInbkYF8)
+
+BattETL bundles together the three independent submodules:
+
+- [Extractor](#extractor) : Responsible for extractor the cycler data and schedule/procedure files.
+- [Transformer](#transformer) : Responsible for transforming cycler data
+- [Loader](#loader) : Responsible for loading data and associated data to the database.
+
+After running BattETL on a specific configuration file the following objects will be available as class variables from the instance:
+
+- `raw_test_data: pandas.DataFrame`: The raw test data exactly as it is in the generated cycler data file(s).
+- `raw_cycle_stats: pandas.DataFrame`: The raw cycle stats data exactly as it is in the generated cycler statistics file.
+- `test_data: pandas.DataFrame`: The transformed test data after normalizing units and datatype and adding a unixtime column.
+- `cycle_stats: pandas.DataFrame`: The transformed cycle stats after normalizing units, datatypes, and calculating supplemental cycle statistics.
+- `schedule: dict`: The procedure/schedule file and all associated files in a nested Dictionary.
+
+### System diagram
+
+<img src="https://raw.githubusercontent.com/BattGenie/battetl/main/images/BattETL_SystemDiagram.svg">
+
+### Extractor
+
+The Extractor is an interface that allows you to extract battery test data from raw data files. You can extract test data and cycle stats data from multiple files using `data_from_files`, and extract Arbin schedules or Maccor procedures and associated files using `schedule_from_files`.
+
+For an example of the Extractor as a standalone class, see `examples/submodule_demos/Extractor_demo.ipynb`
+
+#### Functions
+
+- `data_from_files(paths: list[str])`: Extracts multiple test data files into a single pandas DataFrame.  
+- `schedule_from_files(paths: list[str])`: Extracts Arbin schedules or Maccor procedures and associated files and stores them in a dictionary.  
+- `from_pickle(path: str)`: Reads data from the passed file path and returns it as a pandas DataFrame.  
+
+#### Variables
+
+- `cycler_make: str`: Cycler make  
+- `raw_test_data_meta_data: list[dict]`: Test data meta data  
+- `raw_cycle_stats_meta_data: list[dict]`: Cycler stats meta data  
+- `raw_test_data: pandas.DataFrame`: Test data  
+- `raw_cycle_stats: pandas.DataFrame`: Cycler stats  
+- `maccor_procedure: dict`: Maccor procedure  
+- `arbin_schedule: dict`: Arbin schedule  
+
+### Transformer
+
+The Transformer is an interface that allows you to transform battery test data to the BattETL schema. By default, the time zone is set to 'America/Los_Angeles', but you can modify it to your preferred time zone using the names found in the [IANA Time Zone Database](https://www.iana.org/time-zones). In addition to the default functions provided by the Transformer, you can add your own custom functions to perform specific transformations on your data.
+
+For an example of the Extractor as a standalone class, see `examples/submodule_demos/Transformer_demo.ipynb`
+
+#### Functions
+
+- `transform_test_data(self, data: pd.DataFrame)`: Transforms test data to conform to BattETL naming and data conventions  
+- `transform_cycle_stats`: Transforms cycle stats to conform to BattETL naming and data conventions  
+
+#### Variables
+
+- `timezone: str`: Time zone strings in the IANA Time Zone Database. Used to convert to unix timestamp in seconds. Default 'America/Los_Angeles'.  
+- `user_transform_test_data`: A user defined function to transform test data. The function should take a pandas.DataFrame as input and return a pandas.DataFrame as output.  
+- `user_transform_cycle_stats`: A user defined function to transform cycle stats. The function should take a pandas.DataFrame as input and return a pandas.DataFrame as output.  
+- `test_data: pandas.DataFrame`: Transformed test data  
+- `cycle_stats: pandas.DataFrame`: Transformed cycle stats  
+
+### Loader
+
+The `load` module provides an interface to load the extracted data into a database.
+
+Note that repeated calls to load test data that already exists in the database (as determined by unix timestamp) will not overwrite any existing data. Only test data after the latest existing unix timestamp will be loaded. In the case of loading cycle statistics, any duplicate cycles that already exist in the database will be overwritten.
+
+For an example of the Extractor as a standalone class, see `examples/submodule_demos/Loader_demo.ipynb`
+
+#### Functions
+
+- `load_test_data(test_data_df)`: Loads test_data_df to `test_data` table in the specified database.  
+- `load_cycle_stats(cycle_stats_df)`: Loads cycle_stats_df to `test_data_cycle_stats` table in the specified database.  
+
+## Testing
+
+To run the test suite, use the following commands:
+
+- Run all tests: `pytest`
+- Run Maccor tests: `pytest -m maccor`
+- Run Arbin tests: `pytest -m arbin`
+- Run database specific tests: `pytest -m database`
+- Run tests other than Arbin: `pytest -m "not arbin"`
+- Run Extractor tests: `pytest tests/test_extract_data.py`
+
+To show logs while testing, add the `-o log_cli=true` flag.
+
+## Troubleshooting
+
+### pip install psycopg2 error
+
+If there is an error `Error: pg_config executable not found.` Try installing `libpq-dev` before installing `psycopg2`
+
+```sh
+sudo apt install libpq-dev
+```
```

### Comparing `battetl-1.0.2/battetl.egg-info/SOURCES.txt` & `battetl-1.1.0/battetl.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 LICENSE
 README.md
 setup.py
 battetl/BattETL.py
 battetl/__init__.py
+battetl/battetl_quick.py
 battetl/constants.py
 battetl/logger.py
 battetl/utils.py
 battetl.egg-info/PKG-INFO
 battetl.egg-info/SOURCES.txt
 battetl.egg-info/dependency_links.txt
 battetl.egg-info/requires.txt
 battetl.egg-info/top_level.txt
 battetl/extract/Extractor.py
 battetl/extract/__init__.py
 battetl/load/Loader.py
 battetl/load/__init__.py
 battetl/load/batt_db_test_helper.py
+battetl/load/quick_loader.py
 battetl/transform/Transformer.py
-battetl/transform/__init__.py
-tests/test_BattETL.py
-tests/test_Extractor.py
-tests/test_Loader.py
-tests/test_Transformer.py
-tests/test_utils.py
+battetl/transform/__init__.py
```

### Comparing `battetl-1.0.2/setup.py` & `battetl-1.1.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import setuptools
-
-with open('requirements.txt') as f:
-    requirements = f.read().splitlines()
-
-with open("README.md", "r") as fh:
-    long_description = fh.read()
-
-setuptools.setup(
-    name="battetl",
-    version="1.0.2",
-    author="Zander Nevitt, Bing Syuan Wang and Chintan Pathak",
-    author_email="info@battgenie.life",
-    description="A Python module for extracting, transforming, and loading battery data to a database.",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/BattGenie/battetl",
-    packages=setuptools.find_packages(),
-    install_requires=requirements,
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    python_requires='>=3.9, <3.11',
-    license='MIT',
-)
+import setuptools
+
+with open('requirements.txt') as f:
+    requirements = f.read().splitlines()
+
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+
+setuptools.setup(
+    name="battetl",
+    version="1.1.0",
+    author="Zander Nevitt, Bing Syuan Wang, Eric Ravet, and Chintan Pathak",
+    author_email="info@battgenie.life",
+    description="A Python module for extracting, transforming, and loading battery data to a database.",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/BattGenie/battetl",
+    packages=setuptools.find_packages(),
+    install_requires=requirements,
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    python_requires='>=3.9, <3.11',
+    license='MIT',
+)
```

