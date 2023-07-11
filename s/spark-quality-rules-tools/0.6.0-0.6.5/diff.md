# Comparing `tmp/spark_quality_rules_tools-0.6.0.tar.gz` & `tmp/spark_quality_rules_tools-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_quality_rules_tools-0.6.0.tar", last modified: Thu Jul  6 08:07:32 2023, max compression
+gzip compressed data, was "spark_quality_rules_tools-0.6.5.tar", last modified: Tue Jul 11 02:06:54 2023, max compression
```

## Comparing `spark_quality_rules_tools-0.6.0.tar` & `spark_quality_rules_tools-0.6.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 08:07:32.135801 spark_quality_rules_tools-0.6.0/
--rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.6.0/LICENSE
--rw-rw-rw-   0        0        0       50 2023-06-14 13:33:57.000000 spark_quality_rules_tools-0.6.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4041 2023-07-06 08:07:32.135801 spark_quality_rules_tools-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     3242 2023-06-14 13:39:58.000000 spark_quality_rules_tools-0.6.0/README.md
--rw-rw-rw-   0        0        0      685 2023-07-06 02:24:33.000000 spark_quality_rules_tools-0.6.0/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-07-06 08:07:32.136802 spark_quality_rules_tools-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0     1210 2023-07-06 08:07:00.000000 spark_quality_rules_tools-0.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 08:07:32.087791 spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/
--rw-rw-rw-   0        0        0     2790 2023-07-06 07:26:52.000000 spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-06 08:07:32.109798 spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/functions/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/functions/__init__.py
--rw-rw-rw-   0        0        0    56427 2023-07-06 07:47:24.000000 spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2023-07-06 08:07:32.125799 spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/utils/
--rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/utils/__init__.py
--rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/utils/color.py
--rw-rw-rw-   0        0        0     2138 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/utils/resolve.py
-drwxrwxrwx   0        0        0        0 2023-07-06 08:07:32.134803 spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/utils/resource/
--rw-rw-rw-   0        0        0      532 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/utils/resource/resolve_edge.conf
--rw-rw-rw-   0        0        0      742 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf
--rw-rw-rw-   0        0        0    25809 2023-07-06 02:34:48.000000 spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/utils/resource/rules.json
--rw-rw-rw-   0        0        0     3920 2023-07-06 05:59:35.000000 spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/utils/rules.py
-drwxrwxrwx   0        0        0        0 2023-07-06 08:07:32.108797 spark_quality_rules_tools-0.6.0/spark_quality_rules_tools.egg-info/
--rw-rw-rw-   0        0        0     4041 2023-07-06 08:07:32.000000 spark_quality_rules_tools-0.6.0/spark_quality_rules_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      784 2023-07-06 08:07:32.000000 spark_quality_rules_tools-0.6.0/spark_quality_rules_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 08:07:32.000000 spark_quality_rules_tools-0.6.0/spark_quality_rules_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      205 2023-07-06 08:07:32.000000 spark_quality_rules_tools-0.6.0/spark_quality_rules_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-07-06 08:07:32.000000 spark_quality_rules_tools-0.6.0/spark_quality_rules_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 02:06:54.139676 spark_quality_rules_tools-0.6.5/
+-rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.6.5/LICENSE
+-rw-rw-rw-   0        0        0       50 2023-06-14 13:33:57.000000 spark_quality_rules_tools-0.6.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     4041 2023-07-11 02:06:54.139676 spark_quality_rules_tools-0.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3242 2023-06-14 13:39:58.000000 spark_quality_rules_tools-0.6.5/README.md
+-rw-rw-rw-   0        0        0      685 2023-07-06 02:24:33.000000 spark_quality_rules_tools-0.6.5/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-07-11 02:06:54.139676 spark_quality_rules_tools-0.6.5/setup.cfg
+-rw-rw-rw-   0        0        0     1210 2023-07-11 02:06:38.000000 spark_quality_rules_tools-0.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 02:06:54.077172 spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/
+-rw-rw-rw-   0        0        0     2790 2023-07-06 07:26:52.000000 spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 02:06:54.108423 spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/functions/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0    56738 2023-07-11 02:06:38.000000 spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2023-07-11 02:06:54.124050 spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/utils/
+-rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/utils/__init__.py
+-rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/utils/color.py
+-rw-rw-rw-   0        0        0     2138 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/utils/resolve.py
+drwxrwxrwx   0        0        0        0 2023-07-11 02:06:54.139676 spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/utils/resource/
+-rw-rw-rw-   0        0        0      532 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/utils/resource/resolve_edge.conf
+-rw-rw-rw-   0        0        0      742 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf
+-rw-rw-rw-   0        0        0    25809 2023-07-06 02:34:48.000000 spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/utils/resource/rules.json
+-rw-rw-rw-   0        0        0     3920 2023-07-06 05:59:35.000000 spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/utils/rules.py
+drwxrwxrwx   0        0        0        0 2023-07-11 02:06:54.108423 spark_quality_rules_tools-0.6.5/spark_quality_rules_tools.egg-info/
+-rw-rw-rw-   0        0        0     4041 2023-07-11 02:06:53.000000 spark_quality_rules_tools-0.6.5/spark_quality_rules_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      784 2023-07-11 02:06:54.000000 spark_quality_rules_tools-0.6.5/spark_quality_rules_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 02:06:53.000000 spark_quality_rules_tools-0.6.5/spark_quality_rules_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      205 2023-07-11 02:06:53.000000 spark_quality_rules_tools-0.6.5/spark_quality_rules_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-07-11 02:06:53.000000 spark_quality_rules_tools-0.6.5/spark_quality_rules_tools.egg-info/top_level.txt
```

### Comparing `spark_quality_rules_tools-0.6.0/LICENSE` & `spark_quality_rules_tools-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.6.0/PKG-INFO` & `spark_quality_rules_tools-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark_quality_rules_tools
-Version: 0.6.0
+Version: 0.6.5
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_quality_rules_tools-0.6.0/README.md` & `spark_quality_rules_tools-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.6.0/pyproject.toml` & `spark_quality_rules_tools-0.6.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.6.0/setup.py` & `spark_quality_rules_tools-0.6.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_quality_rules_tools',
     packages=find_packages(),
-    version='0.6.0',
+    version='0.6.5',
     description='spark_quality_rules_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_quality_rules_tools/',
     download_url='https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip',
```

### Comparing `spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/__init__.py` & `spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/functions/generator.py` & `spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/functions/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -296,15 +296,15 @@
         hammurabi_conf = f.read()
 
     variables_1 = sorted(list(set(re.findall(r'{([a-zA-Z_.-]+)}', hammurabi_conf))))
     variables_2 = sorted(list(set(re.findall(r'{?([a-zA-Z_.-]+)}', hammurabi_conf))))
     variables_list = list(set(variables_1 + variables_2))
 
     variables_dict = {variables: "" for variables in variables_list if
-                      variables not in ("ARTIFACTORY_UNIQUE_CACHE", "SCHEMAS_REPOSITORY")}
+                      variables not in ("ARTIFACTORY_UNIQUE_CACHE", "SCHEMAS_REPOSITORY", "TEST_PATH")}
 
     parameter_dict = dict()
     parameter_dict[uuaa_name] = list()
     parameter_dict[uuaa_name].append({"table": url_conf_name,
                                       "conf_name": url_conf_extension,
                                       "parameters": variables_dict})
 
@@ -359,15 +359,15 @@
         hammurabi_conf = f.read()
 
     variables_1 = sorted(list(set(re.findall(r'{([a-zA-Z_.-]+)}', hammurabi_conf))))
     variables_2 = sorted(list(set(re.findall(r'{?([a-zA-Z_.-]+)}', hammurabi_conf))))
     variables_list = list(set(variables_1 + variables_2))
 
     variables_dict = {variables: "" for variables in variables_list if
-                      variables not in ("ARTIFACTORY_UNIQUE_CACHE", "SCHEMAS_REPOSITORY")}
+                      variables not in ("ARTIFACTORY_UNIQUE_CACHE", "SCHEMAS_REPOSITORY", "TEST_PATH")}
 
     parameter_dict = dict()
     parameter_dict[uuaa_name] = list()
     parameter_dict[uuaa_name].append({"table": table_name,
                                       "conf_name": url_conf_name,
                                       "parameters": variables_dict})
 
@@ -465,17 +465,18 @@
     if not validate_compare_parameters:
         raise Exception(f'Need more variables the parameters: parameter_conf_list')
 
     cutoff_date = ""
     with open(dir_confs_filename) as f:
         txt_conf = f.read()
 
+    txt_conf = txt_conf.replace(f'${{TEST_PATH}}', "")
+    txt_conf = txt_conf.replace(f'${{COUNTRY}}', "pe")
     txt_conf = txt_conf.replace(f'"/artifactory/"', "/artifactory/")
-    txt_conf = txt_conf.replace(f'${{ARTIFACTORY_UNIQUE_CACHE}}',
-                                "http://artifactory-gdt.central-02.nextgen.igrupobbva")
+    txt_conf = txt_conf.replace(f'${{ARTIFACTORY_UNIQUE_CACHE}}',"http://artifactory-gdt.central-02.nextgen.igrupobbva")
     if is_prod:
         txt_conf = txt_conf.replace(f'${{SCHEMAS_REPOSITORY}}', "gl-datio-da-generic-local")
     else:
         txt_conf = txt_conf.replace(f'${{SCHEMAS_REPOSITORY}}', "gl-datio-da-generic-dev-local")
 
     for params_parameter_conf in tqdm(parameter_conf_list):
         for k, v in params_parameter_conf.items():
@@ -622,17 +623,18 @@
     if not validate_compare_parameters:
         raise Exception(f'Need more variables the parameters: parameter_conf_list')
 
     cutoff_date = ""
     with open(dir_confs_filename) as f:
         txt_conf = f.read()
 
+    txt_conf = txt_conf.replace(f'${{TEST_PATH}}', "")
+    txt_conf = txt_conf.replace(f'${{COUNTRY}}', "pe")
     txt_conf = txt_conf.replace(f'"/artifactory/"', "/artifactory/")
-    txt_conf = txt_conf.replace(f'${{ARTIFACTORY_UNIQUE_CACHE}}',
-                                "http://artifactory-gdt.central-02.nextgen.igrupobbva")
+    txt_conf = txt_conf.replace(f'${{ARTIFACTORY_UNIQUE_CACHE}}', "http://artifactory-gdt.central-02.nextgen.igrupobbva")
     if is_prod:
         txt_conf = txt_conf.replace(f'${{SCHEMAS_REPOSITORY}}', "gl-datio-da-generic-local")
     else:
         txt_conf = txt_conf.replace(f'${{SCHEMAS_REPOSITORY}}', "gl-datio-da-generic-dev-local")
 
     for params_parameter_conf in tqdm(parameter_conf_list):
         for k, v in params_parameter_conf.items():
@@ -783,14 +785,16 @@
     if not validate_compare_parameters:
         raise Exception(f'Need more variables the parameters: parameter_conf_list')
 
     cutoff_date = ""
     with open(dir_confs_filename) as f:
         txt_conf = f.read()
 
+    txt_conf = txt_conf.replace(f'${{TEST_PATH}}', "")
+    txt_conf = txt_conf.replace(f'${{COUNTRY}}', "pe")
     txt_conf = txt_conf.replace(f'"/artifactory/"', "/artifactory/")
     txt_conf = txt_conf.replace(f'${{ARTIFACTORY_UNIQUE_CACHE}}', "http://artifactory-gdt.central-02.nextgen.igrupobbva")
     if is_prod:
         txt_conf = txt_conf.replace(f'${{SCHEMAS_REPOSITORY}}', "gl-datio-da-generic-local")
     else:
         txt_conf = txt_conf.replace(f'${{SCHEMAS_REPOSITORY}}', "gl-datio-da-generic-dev-local")
 
@@ -819,15 +823,15 @@
             dataframeinfo = info["dataFrameInfo"]
         if 'input' in info.keys():
             input = info["input"]
         if 'rules' in info.keys():
             rules = info["rules"]
             for rule in rules:
                 key_id_rule = rule.get("config").get("id", None)
-                if str(key_id_rule) == str(rules_id):
+                if str(key_id_rule).strip() == str(rules_id).strip():
                     rule_list.append(rule)
         hamu_dict = dict(hammurabi=dict(dataFrameInfo=dataframeinfo, input=input, rules=rule_list))
     json_file2 = json.dumps(hamu_dict, indent=4)
     conf2 = ConfigFactory.parse_string(json_file2)
     hocons_file2 = HOCONConverter.convert(conf2, "hocon")
     with open(dir_hocons_filename, "w") as f:
         f.write(hocons_file2)
```

### Comparing `spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/utils/resolve.py` & `spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/utils/resolve.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/utils/resource/resolve_edge.conf` & `spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/utils/resource/resolve_edge.conf`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf` & `spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/utils/resource/rules.json` & `spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/utils/resource/rules.json`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.6.0/spark_quality_rules_tools/utils/rules.py` & `spark_quality_rules_tools-0.6.5/spark_quality_rules_tools/utils/rules.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.6.0/spark_quality_rules_tools.egg-info/PKG-INFO` & `spark_quality_rules_tools-0.6.5/spark_quality_rules_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-quality-rules-tools
-Version: 0.6.0
+Version: 0.6.5
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_quality_rules_tools-0.6.0/spark_quality_rules_tools.egg-info/SOURCES.txt` & `spark_quality_rules_tools-0.6.5/spark_quality_rules_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

