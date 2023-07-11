# Comparing `tmp/huhk-1.5.7.tar.gz` & `tmp/huhk-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\huhk-1.5.7.tar", last modified: Tue Jul 11 14:32:54 2023, max compression
+gzip compressed data, was "dist\huhk-1.5.8.tar", last modified: Tue Jul 11 14:34:47 2023, max compression
```

## Comparing `huhk-1.5.7.tar` & `huhk-1.5.8.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 14:32:54.000000 huhk-1.5.7/
--rw-rw-rw-   0        0        0      153 2023-07-11 14:32:54.000000 huhk-1.5.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-11 14:32:54.000000 huhk-1.5.7/huhk/
--rw-rw-rw-   0        0        0      931 2023-07-11 13:40:55.000000 huhk-1.5.7/huhk/__init__.py
--rw-rw-rw-   0        0        0      532 2023-07-11 13:40:55.000000 huhk-1.5.7/huhk/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 14:32:54.000000 huhk-1.5.7/huhk/case_project/
--rw-rw-rw-   0        0        0        0 2023-07-11 13:40:55.000000 huhk-1.5.7/huhk/case_project/__init__.py
--rw-rw-rw-   0        0        0     3072 2023-07-11 13:40:55.000000 huhk-1.5.7/huhk/case_project/base_project.py
--rw-rw-rw-   0        0        0      639 2023-07-11 13:40:55.000000 huhk-1.5.7/huhk/case_project/json_coder.py
--rw-rw-rw-   0        0        0      770 2023-07-11 14:32:45.000000 huhk-1.5.7/huhk/case_project/main.py
--rw-rw-rw-   0        0        0      908 2023-07-11 13:40:55.000000 huhk-1.5.7/huhk/case_project/setup_set.py
--rw-rw-rw-   0        0        0       17 2023-07-11 14:32:54.000000 huhk-1.5.7/huhk/case_project/version.py
--rw-rw-rw-   0        0        0    29291 2023-07-11 13:40:55.000000 huhk-1.5.7/huhk/init_project.py
--rw-rw-rw-   0        0        0      274 2023-07-11 13:40:55.000000 huhk-1.5.7/huhk/setup_run.py
-drwxrwxrwx   0        0        0        0 2023-07-11 14:32:54.000000 huhk-1.5.7/huhk/testcase/
--rw-rw-rw-   0        0        0        0 2023-07-11 13:40:55.000000 huhk-1.5.7/huhk/testcase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 14:32:54.000000 huhk-1.5.7/huhk/testcase/apache/
--rw-rw-rw-   0        0        0        0 2023-07-11 13:40:55.000000 huhk-1.5.7/huhk/testcase/apache/__init__.py
--rw-rw-rw-   0        0        0     3355 2023-07-11 13:40:55.000000 huhk-1.5.7/huhk/testcase/apache/beam_class.py
--rw-rw-rw-   0        0        0     5523 2023-07-11 14:08:30.000000 huhk-1.5.7/huhk/testcase/apache/data.py
--rw-rw-rw-   0        0        0     1764 2023-07-11 13:40:55.000000 huhk-1.5.7/huhk/testcase/apache/par_do.py
--rw-rw-rw-   0        0        0     7303 2023-07-11 14:11:21.000000 huhk-1.5.7/huhk/testcase/apache/test_cogroupbykey.py
--rw-rw-rw-   0        0        0      517 2023-07-11 13:40:55.000000 huhk-1.5.7/huhk/testcase/apache/test_file.py
--rw-rw-rw-   0        0        0     1544 2023-07-11 13:40:55.000000 huhk-1.5.7/huhk/testcase/apache/test_fiter.py
--rw-rw-rw-   0        0        0     2144 2023-07-11 13:40:55.000000 huhk-1.5.7/huhk/testcase/apache/test_flatmap.py
--rw-rw-rw-   0        0        0      564 2023-07-11 13:40:55.000000 huhk-1.5.7/huhk/testcase/apache/test_map.py
--rw-rw-rw-   0        0        0     2615 2023-07-11 13:40:55.000000 huhk-1.5.7/huhk/testcase/apache/test_par_do.py
--rw-rw-rw-   0        0        0     1692 2023-07-11 13:40:55.000000 huhk-1.5.7/huhk/testcase/apache/test_regex.py
--rw-rw-rw-   0        0        0      515 2023-07-11 13:40:55.000000 huhk-1.5.7/huhk/testcase/apache/test_time.py
--rw-rw-rw-   0        0        0      549 2023-07-11 13:40:55.000000 huhk-1.5.7/huhk/testcase/apache/test_to_string.py
--rw-rw-rw-   0        0        0    21927 2023-07-11 14:22:19.000000 huhk-1.5.7/huhk/unit_apache_beam.py
--rw-rw-rw-   0        0        0     4508 2023-07-11 13:40:55.000000 huhk-1.5.7/huhk/unit_dict.py
--rw-rw-rw-   0        0        0     3843 2023-07-11 13:40:55.000000 huhk-1.5.7/huhk/unit_encryption.py
--rw-rw-rw-   0        0        0    24874 2023-07-11 13:40:55.000000 huhk-1.5.7/huhk/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2023-07-11 13:40:55.000000 huhk-1.5.7/huhk/unit_logger.py
--rw-rw-rw-   0        0        0     9212 2023-07-11 13:40:55.000000 huhk-1.5.7/huhk/unit_request.py
--rw-rw-rw-   0        0        0     2473 2023-07-11 13:40:55.000000 huhk-1.5.7/huhk/unit_tasks.py
--rw-rw-rw-   0        0        0      733 2023-07-11 13:40:55.000000 huhk-1.5.7/huhk/常用命令.py
-drwxrwxrwx   0        0        0        0 2023-07-11 14:32:54.000000 huhk-1.5.7/huhk.egg-info/
--rw-rw-rw-   0        0        0      153 2023-07-11 14:32:54.000000 huhk-1.5.7/huhk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1068 2023-07-11 14:32:54.000000 huhk-1.5.7/huhk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 14:32:54.000000 huhk-1.5.7/huhk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-07-11 14:32:54.000000 huhk-1.5.7/huhk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      134 2023-07-11 14:32:54.000000 huhk-1.5.7/huhk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-11 14:32:54.000000 huhk-1.5.7/huhk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 14:32:54.000000 huhk-1.5.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-11 14:34:47.000000 huhk-1.5.8/
+-rw-rw-rw-   0        0        0      153 2023-07-11 14:34:47.000000 huhk-1.5.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-11 14:34:47.000000 huhk-1.5.8/huhk/
+-rw-rw-rw-   0        0        0      931 2023-07-11 13:40:55.000000 huhk-1.5.8/huhk/__init__.py
+-rw-rw-rw-   0        0        0      532 2023-07-11 13:40:55.000000 huhk-1.5.8/huhk/__main__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 14:34:47.000000 huhk-1.5.8/huhk/case_project/
+-rw-rw-rw-   0        0        0        0 2023-07-11 13:40:55.000000 huhk-1.5.8/huhk/case_project/__init__.py
+-rw-rw-rw-   0        0        0     3072 2023-07-11 13:40:55.000000 huhk-1.5.8/huhk/case_project/base_project.py
+-rw-rw-rw-   0        0        0      639 2023-07-11 13:40:55.000000 huhk-1.5.8/huhk/case_project/json_coder.py
+-rw-rw-rw-   0        0        0      727 2023-07-11 14:34:34.000000 huhk-1.5.8/huhk/case_project/main.py
+-rw-rw-rw-   0        0        0      908 2023-07-11 13:40:55.000000 huhk-1.5.8/huhk/case_project/setup_set.py
+-rw-rw-rw-   0        0        0       17 2023-07-11 14:34:47.000000 huhk-1.5.8/huhk/case_project/version.py
+-rw-rw-rw-   0        0        0    29291 2023-07-11 13:40:55.000000 huhk-1.5.8/huhk/init_project.py
+-rw-rw-rw-   0        0        0      274 2023-07-11 13:40:55.000000 huhk-1.5.8/huhk/setup_run.py
+drwxrwxrwx   0        0        0        0 2023-07-11 14:34:47.000000 huhk-1.5.8/huhk/testcase/
+-rw-rw-rw-   0        0        0        0 2023-07-11 13:40:55.000000 huhk-1.5.8/huhk/testcase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 14:34:47.000000 huhk-1.5.8/huhk/testcase/apache/
+-rw-rw-rw-   0        0        0        0 2023-07-11 13:40:55.000000 huhk-1.5.8/huhk/testcase/apache/__init__.py
+-rw-rw-rw-   0        0        0     3355 2023-07-11 13:40:55.000000 huhk-1.5.8/huhk/testcase/apache/beam_class.py
+-rw-rw-rw-   0        0        0     5523 2023-07-11 14:08:30.000000 huhk-1.5.8/huhk/testcase/apache/data.py
+-rw-rw-rw-   0        0        0     1764 2023-07-11 13:40:55.000000 huhk-1.5.8/huhk/testcase/apache/par_do.py
+-rw-rw-rw-   0        0        0     7303 2023-07-11 14:11:21.000000 huhk-1.5.8/huhk/testcase/apache/test_cogroupbykey.py
+-rw-rw-rw-   0        0        0      517 2023-07-11 13:40:55.000000 huhk-1.5.8/huhk/testcase/apache/test_file.py
+-rw-rw-rw-   0        0        0     1544 2023-07-11 13:40:55.000000 huhk-1.5.8/huhk/testcase/apache/test_fiter.py
+-rw-rw-rw-   0        0        0     2144 2023-07-11 13:40:55.000000 huhk-1.5.8/huhk/testcase/apache/test_flatmap.py
+-rw-rw-rw-   0        0        0      564 2023-07-11 13:40:55.000000 huhk-1.5.8/huhk/testcase/apache/test_map.py
+-rw-rw-rw-   0        0        0     2615 2023-07-11 13:40:55.000000 huhk-1.5.8/huhk/testcase/apache/test_par_do.py
+-rw-rw-rw-   0        0        0     1692 2023-07-11 13:40:55.000000 huhk-1.5.8/huhk/testcase/apache/test_regex.py
+-rw-rw-rw-   0        0        0      515 2023-07-11 13:40:55.000000 huhk-1.5.8/huhk/testcase/apache/test_time.py
+-rw-rw-rw-   0        0        0      549 2023-07-11 13:40:55.000000 huhk-1.5.8/huhk/testcase/apache/test_to_string.py
+-rw-rw-rw-   0        0        0    21927 2023-07-11 14:22:19.000000 huhk-1.5.8/huhk/unit_apache_beam.py
+-rw-rw-rw-   0        0        0     4508 2023-07-11 13:40:55.000000 huhk-1.5.8/huhk/unit_dict.py
+-rw-rw-rw-   0        0        0     3843 2023-07-11 13:40:55.000000 huhk-1.5.8/huhk/unit_encryption.py
+-rw-rw-rw-   0        0        0    24874 2023-07-11 13:40:55.000000 huhk-1.5.8/huhk/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2023-07-11 13:40:55.000000 huhk-1.5.8/huhk/unit_logger.py
+-rw-rw-rw-   0        0        0     9212 2023-07-11 13:40:55.000000 huhk-1.5.8/huhk/unit_request.py
+-rw-rw-rw-   0        0        0     2473 2023-07-11 13:40:55.000000 huhk-1.5.8/huhk/unit_tasks.py
+-rw-rw-rw-   0        0        0      733 2023-07-11 13:40:55.000000 huhk-1.5.8/huhk/常用命令.py
+drwxrwxrwx   0        0        0        0 2023-07-11 14:34:47.000000 huhk-1.5.8/huhk.egg-info/
+-rw-rw-rw-   0        0        0      153 2023-07-11 14:34:47.000000 huhk-1.5.8/huhk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1068 2023-07-11 14:34:47.000000 huhk-1.5.8/huhk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 14:34:47.000000 huhk-1.5.8/huhk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-07-11 14:34:47.000000 huhk-1.5.8/huhk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      134 2023-07-11 14:34:47.000000 huhk-1.5.8/huhk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-11 14:34:47.000000 huhk-1.5.8/huhk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 14:34:47.000000 huhk-1.5.8/setup.cfg
```

### Comparing `huhk-1.5.7/huhk/__init__.py` & `huhk-1.5.8/huhk/__init__.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.7/huhk/__main__.py` & `huhk-1.5.8/huhk/__main__.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.7/huhk/case_project/base_project.py` & `huhk-1.5.8/huhk/case_project/base_project.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.7/huhk/case_project/json_coder.py` & `huhk-1.5.8/huhk/case_project/json_coder.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.7/huhk/case_project/main.py` & `huhk-1.5.8/huhk/case_project/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,11 @@
 import click
 from huhk.case_project.version import version as _version
 
 
-@click.group()
-def main():
-    pass
-
-
 @click.command()
 @click.option('-v', '--version', help='线索版本', required=False)
 @click.option('-i', '--init', help='项目key', required=False)
 @click.option('-u', '--update', help='项目key', required=False)
 def main(version, init, update):
     """Simple program that greets NAME for a total of COUNT times."""
     if version:
```

### Comparing `huhk-1.5.7/huhk/case_project/setup_set.py` & `huhk-1.5.8/huhk/case_project/setup_set.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.7/huhk/init_project.py` & `huhk-1.5.8/huhk/init_project.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.7/huhk/testcase/apache/beam_class.py` & `huhk-1.5.8/huhk/testcase/apache/beam_class.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.7/huhk/testcase/apache/data.py` & `huhk-1.5.8/huhk/testcase/apache/data.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.7/huhk/testcase/apache/par_do.py` & `huhk-1.5.8/huhk/testcase/apache/par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.7/huhk/testcase/apache/test_cogroupbykey.py` & `huhk-1.5.8/huhk/testcase/apache/test_cogroupbykey.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.7/huhk/testcase/apache/test_file.py` & `huhk-1.5.8/huhk/testcase/apache/test_file.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.7/huhk/testcase/apache/test_fiter.py` & `huhk-1.5.8/huhk/testcase/apache/test_fiter.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.7/huhk/testcase/apache/test_flatmap.py` & `huhk-1.5.8/huhk/testcase/apache/test_flatmap.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.7/huhk/testcase/apache/test_map.py` & `huhk-1.5.8/huhk/testcase/apache/test_map.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.7/huhk/testcase/apache/test_par_do.py` & `huhk-1.5.8/huhk/testcase/apache/test_par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.7/huhk/testcase/apache/test_regex.py` & `huhk-1.5.8/huhk/testcase/apache/test_regex.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.7/huhk/testcase/apache/test_time.py` & `huhk-1.5.8/huhk/testcase/apache/test_time.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.7/huhk/testcase/apache/test_to_string.py` & `huhk-1.5.8/huhk/testcase/apache/test_to_string.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.7/huhk/unit_apache_beam.py` & `huhk-1.5.8/huhk/unit_apache_beam.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.7/huhk/unit_dict.py` & `huhk-1.5.8/huhk/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.7/huhk/unit_encryption.py` & `huhk-1.5.8/huhk/unit_encryption.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.7/huhk/unit_fun.py` & `huhk-1.5.8/huhk/unit_fun.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.7/huhk/unit_logger.py` & `huhk-1.5.8/huhk/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.7/huhk/unit_request.py` & `huhk-1.5.8/huhk/unit_request.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.7/huhk/unit_tasks.py` & `huhk-1.5.8/huhk/unit_tasks.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.7/huhk/常用命令.py` & `huhk-1.5.8/huhk/常用命令.py`

 * *Files identical despite different names*

### Comparing `huhk-1.5.7/huhk.egg-info/SOURCES.txt` & `huhk-1.5.8/huhk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

