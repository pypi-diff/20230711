# Comparing `tmp/nginx-static-analysis-0.2.8.tar.gz` & `tmp/nginx-static-analysis-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nginx-static-analysis-0.2.8.tar", last modified: Sat Jul  8 08:29:55 2023, max compression
+gzip compressed data, was "nginx-static-analysis-0.2.9.tar", last modified: Mon Jul 10 22:18:35 2023, max compression
```

## Comparing `nginx-static-analysis-0.2.8.tar` & `nginx-static-analysis-0.2.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:29:55.073852 nginx-static-analysis-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-08 08:29:47.000000 nginx-static-analysis-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-07-08 08:29:55.073852 nginx-static-analysis-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-07-08 08:29:47.000000 nginx-static-analysis-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:29:55.073852 nginx-static-analysis-0.2.8/nginx_analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 08:29:47.000000 nginx-static-analysis-0.2.8/nginx_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8284 2023-07-08 08:29:47.000000 nginx-static-analysis-0.2.8/nginx_analysis/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-07-08 08:29:47.000000 nginx-static-analysis-0.2.8/nginx_analysis/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-08 08:29:47.000000 nginx-static-analysis-0.2.8/nginx_analysis/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-08 08:29:47.000000 nginx-static-analysis-0.2.8/nginx_analysis/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-07-08 08:29:47.000000 nginx-static-analysis-0.2.8/nginx_analysis/log.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1739 2023-07-08 08:29:47.000000 nginx-static-analysis-0.2.8/nginx_analysis/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-08 08:29:47.000000 nginx-static-analysis-0.2.8/nginx_analysis/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 08:29:55.073852 nginx-static-analysis-0.2.8/nginx_static_analysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8243 2023-07-08 08:29:55.000000 nginx-static-analysis-0.2.8/nginx_static_analysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-08 08:29:55.000000 nginx-static-analysis-0.2.8/nginx_static_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 08:29:55.000000 nginx-static-analysis-0.2.8/nginx_static_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-08 08:29:55.000000 nginx-static-analysis-0.2.8/nginx_static_analysis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-08 08:29:55.000000 nginx-static-analysis-0.2.8/nginx_static_analysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-08 08:29:55.000000 nginx-static-analysis-0.2.8/nginx_static_analysis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-08 08:29:47.000000 nginx-static-analysis-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-08 08:29:55.073852 nginx-static-analysis-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-08 08:29:47.000000 nginx-static-analysis-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:18:35.609096 nginx-static-analysis-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-10 22:18:31.000000 nginx-static-analysis-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-07-10 22:18:35.609096 nginx-static-analysis-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-07-10 22:18:31.000000 nginx-static-analysis-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:18:35.609096 nginx-static-analysis-0.2.9/nginx_analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 22:18:31.000000 nginx-static-analysis-0.2.9/nginx_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-07-10 22:18:31.000000 nginx-static-analysis-0.2.9/nginx_analysis/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-07-10 22:18:31.000000 nginx-static-analysis-0.2.9/nginx_analysis/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-10 22:18:31.000000 nginx-static-analysis-0.2.9/nginx_analysis/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-10 22:18:31.000000 nginx-static-analysis-0.2.9/nginx_analysis/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-07-10 22:18:31.000000 nginx-static-analysis-0.2.9/nginx_analysis/log.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1739 2023-07-10 22:18:31.000000 nginx-static-analysis-0.2.9/nginx_analysis/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-10 22:18:31.000000 nginx-static-analysis-0.2.9/nginx_analysis/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 22:18:35.609096 nginx-static-analysis-0.2.9/nginx_static_analysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-07-10 22:18:35.000000 nginx-static-analysis-0.2.9/nginx_static_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-10 22:18:35.000000 nginx-static-analysis-0.2.9/nginx_static_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 22:18:35.000000 nginx-static-analysis-0.2.9/nginx_static_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-10 22:18:35.000000 nginx-static-analysis-0.2.9/nginx_static_analysis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-10 22:18:35.000000 nginx-static-analysis-0.2.9/nginx_static_analysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-10 22:18:35.000000 nginx-static-analysis-0.2.9/nginx_static_analysis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-10 22:18:31.000000 nginx-static-analysis-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-10 22:18:35.613096 nginx-static-analysis-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-10 22:18:31.000000 nginx-static-analysis-0.2.9/setup.py
```

### Comparing `nginx-static-analysis-0.2.8/LICENSE` & `nginx-static-analysis-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nginx-static-analysis-0.2.8/PKG-INFO` & `nginx-static-analysis-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nginx-static-analysis
-Version: 0.2.8
+Version: 0.2.9
 Summary: Parse Nginx configurations in a clear manner for debugging purposes
 Home-page: https://github.com/AlexanderGrooff/nginx-static-analysis
 Author: Alexander Grooff
 Author-email: Alexander Grooff <alexandergrooff@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Alexander Grooff
@@ -36,14 +36,27 @@
 
 [![nginx-static-analysis](https://img.shields.io/pypi/v/nginx-static-analysis)](https://pypi.org/project/nginx-static-analysis/)
 
 Parse Nginx configurations on your host and filter for directives/values.
 
 Largely powered by [Crossplane](https://github.com/nginxinc/crossplane).
 
+## Installation
+
+You're able to find the `nginx-static-analysis` binary in the following places:
+
+```bash
+
+# Pip
+pip install nginx-static-analysis
+
+# Arch
+yay -S nginx-static-analysis
+```
+
 ## Analysing your Nginx configuration
 
 You can list any directive within your Nginx configuration. For example, show all `listen` directives:
 ```
 app@wifbtb-testalex-magweb-cmbl:~$ nginx-static-analysis -d listen
 +-------------------------------------------------+--------------------+-------------------------------------+
 |                       File                      |       Values       |              Directives             |
```

### Comparing `nginx-static-analysis-0.2.8/README.md` & `nginx-static-analysis-0.2.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,27 @@
 
 [![nginx-static-analysis](https://img.shields.io/pypi/v/nginx-static-analysis)](https://pypi.org/project/nginx-static-analysis/)
 
 Parse Nginx configurations on your host and filter for directives/values.
 
 Largely powered by [Crossplane](https://github.com/nginxinc/crossplane).
 
+## Installation
+
+You're able to find the `nginx-static-analysis` binary in the following places:
+
+```bash
+
+# Pip
+pip install nginx-static-analysis
+
+# Arch
+yay -S nginx-static-analysis
+```
+
 ## Analysing your Nginx configuration
 
 You can list any directive within your Nginx configuration. For example, show all `listen` directives:
 ```
 app@wifbtb-testalex-magweb-cmbl:~$ nginx-static-analysis -d listen
 +-------------------------------------------------+--------------------+-------------------------------------+
 |                       File                      |       Values       |              Directives             |
```

### Comparing `nginx-static-analysis-0.2.8/nginx_analysis/analysis.py` & `nginx-static-analysis-0.2.9/nginx_analysis/analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,17 +88,14 @@
 def get_unique_directives(root_config: RootNginxConfig) -> List[str]:
     """
     Find all unique directives in the given root config
     """
     unique_directives: Set[str] = set()
     for line_config in root_config.lines:
         directives = get_unique_directives_in_line(line_config)
-        logger.debug(
-            f"Found directives on line {line_config.line} in file {line_config.file}: {directives}"
-        )
         unique_directives = unique_directives.union(directives)
     return list(unique_directives)
 
 
 def get_line_at_linenr(
     root_config: RootNginxConfig, linenr: int
 ) -> Optional[NginxLineConfig]:
@@ -132,27 +129,23 @@
     If there are no matches, return an empty list for both the matching
     lines and the matched filters.
     """
     if not filters:
         # No filters, meaning that the line matches directly
         return [line], []
 
-    logger.debug(f"Checking if line {line} matches filters: {filters}")
     matched_filter = is_partial_direct_match(line, filters)
     if matched_filter:
         logger.debug(f"Found match in children: {line}")
         all_matched_filters = set([matched_filter])
         # Search for remaining filters in children, as the parent
         # might still be looking for other filters
         for child in line.children:
             remaining_filters = [f for f in filters if f not in all_matched_filters]
             if remaining_filters:
-                logger.debug(
-                    f"Looking for remaining filters in child {child}: {remaining_filters}"
-                )
                 _, child_matched_filters = get_matching_lines_in_children(
                     child, remaining_filters
                 )
                 all_matched_filters.update(child_matched_filters)
             else:
                 logger.debug(
                     f"Found all filters in children of line {line}. We should stop!"
```

### Comparing `nginx-static-analysis-0.2.8/nginx_analysis/dataclasses.py` & `nginx-static-analysis-0.2.9/nginx_analysis/dataclasses.py`

 * *Files identical despite different names*

### Comparing `nginx-static-analysis-0.2.8/nginx_analysis/filter.py` & `nginx-static-analysis-0.2.9/nginx_analysis/filter.py`

 * *Files identical despite different names*

### Comparing `nginx-static-analysis-0.2.8/nginx_analysis/input.py` & `nginx-static-analysis-0.2.9/nginx_analysis/input.py`

 * *Files identical despite different names*

### Comparing `nginx-static-analysis-0.2.8/nginx_analysis/log.py` & `nginx-static-analysis-0.2.9/nginx_analysis/log.py`

 * *Files identical despite different names*

### Comparing `nginx-static-analysis-0.2.8/nginx_analysis/main.py` & `nginx-static-analysis-0.2.9/nginx_analysis/main.py`

 * *Files identical despite different names*

### Comparing `nginx-static-analysis-0.2.8/nginx_analysis/output.py` & `nginx-static-analysis-0.2.9/nginx_analysis/output.py`

 * *Files identical despite different names*

### Comparing `nginx-static-analysis-0.2.8/nginx_static_analysis.egg-info/PKG-INFO` & `nginx-static-analysis-0.2.9/nginx_static_analysis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nginx-static-analysis
-Version: 0.2.8
+Version: 0.2.9
 Summary: Parse Nginx configurations in a clear manner for debugging purposes
 Home-page: https://github.com/AlexanderGrooff/nginx-static-analysis
 Author: Alexander Grooff
 Author-email: Alexander Grooff <alexandergrooff@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Alexander Grooff
@@ -36,14 +36,27 @@
 
 [![nginx-static-analysis](https://img.shields.io/pypi/v/nginx-static-analysis)](https://pypi.org/project/nginx-static-analysis/)
 
 Parse Nginx configurations on your host and filter for directives/values.
 
 Largely powered by [Crossplane](https://github.com/nginxinc/crossplane).
 
+## Installation
+
+You're able to find the `nginx-static-analysis` binary in the following places:
+
+```bash
+
+# Pip
+pip install nginx-static-analysis
+
+# Arch
+yay -S nginx-static-analysis
+```
+
 ## Analysing your Nginx configuration
 
 You can list any directive within your Nginx configuration. For example, show all `listen` directives:
 ```
 app@wifbtb-testalex-magweb-cmbl:~$ nginx-static-analysis -d listen
 +-------------------------------------------------+--------------------+-------------------------------------+
 |                       File                      |       Values       |              Directives             |
```

### Comparing `nginx-static-analysis-0.2.8/nginx_static_analysis.egg-info/SOURCES.txt` & `nginx-static-analysis-0.2.9/nginx_static_analysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nginx-static-analysis-0.2.8/pyproject.toml` & `nginx-static-analysis-0.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nginx-static-analysis"
-version = "0.2.8"
+version = "0.2.9"
 description = "Parse Nginx configurations in a clear manner for debugging purposes"
 authors = [
     {name = "Alexander Grooff", email = "alexandergrooff@gmail.com"},
 ]
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.7"
 license = {name = "MIT", file = "LICENSE"}
```

### Comparing `nginx-static-analysis-0.2.8/setup.py` & `nginx-static-analysis-0.2.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 loguru==0.5.3
 prettytable==2.5.0
 """
 
 
 setup(
     name="nginx-static-analysis",
-    version="0.2.8",
+    version="0.2.9",
     description="Parse Nginx configurations in a clear manner for debugging purposes",
     url="https://github.com/AlexanderGrooff/nginx-static-analysis",
     packages=find_packages(
         include=["nginx_analysis", "requirements/base.txt"], exclude=["tests"]
     ),
     author="Alexander Grooff",
     author_email="alexandergrooff@gmail.com",
```

