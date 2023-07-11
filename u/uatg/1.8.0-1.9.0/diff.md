# Comparing `tmp/uatg-1.8.0.tar.gz` & `tmp/uatg-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/uatg-1.8.0.tar", last modified: Fri Mar 31 05:23:07 2023, max compression
+gzip compressed data, was "dist/uatg-1.9.0.tar", last modified: Tue Jul 11 12:29:09 2023, max compression
```

## Comparing `uatg-1.8.0.tar` & `uatg-1.9.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 05:23:07.000000 uatg-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-03-31 05:22:56.000000 uatg-1.8.0/LICENSE.incore
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-03-31 05:22:56.000000 uatg-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-31 05:23:07.000000 uatg-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-31 05:22:56.000000 uatg-1.8.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-03-31 05:23:07.000000 uatg-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-03-31 05:22:56.000000 uatg-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 05:23:07.000000 uatg-1.8.0/uatg/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-31 05:22:56.000000 uatg-1.8.0/uatg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    66406 2023-03-31 05:22:56.000000 uatg-1.8.0/uatg/instruction_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    34654 2023-03-31 05:22:56.000000 uatg-1.8.0/uatg/instruction_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    31817 2023-03-31 05:22:56.000000 uatg-1.8.0/uatg/isem.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-03-31 05:22:56.000000 uatg-1.8.0/uatg/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    19681 2023-03-31 05:22:56.000000 uatg-1.8.0/uatg/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-03-31 05:22:56.000000 uatg-1.8.0/uatg/regex_formats.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-31 05:22:56.000000 uatg-1.8.0/uatg/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    27888 2023-03-31 05:22:56.000000 uatg-1.8.0/uatg/test_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    55526 2023-03-31 05:22:56.000000 uatg-1.8.0/uatg/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 05:23:07.000000 uatg-1.8.0/uatg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-03-31 05:23:07.000000 uatg-1.8.0/uatg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-03-31 05:23:07.000000 uatg-1.8.0/uatg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 05:23:07.000000 uatg-1.8.0/uatg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-31 05:23:07.000000 uatg-1.8.0/uatg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 05:23:07.000000 uatg-1.8.0/uatg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-31 05:23:07.000000 uatg-1.8.0/uatg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-31 05:23:07.000000 uatg-1.8.0/uatg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:29:09.000000 uatg-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-11 12:28:52.000000 uatg-1.9.0/LICENSE.incore
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-11 12:28:52.000000 uatg-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-11 12:29:09.000000 uatg-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-11 12:28:52.000000 uatg-1.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-11 12:29:09.000000 uatg-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-11 12:28:52.000000 uatg-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:29:09.000000 uatg-1.9.0/uatg/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-11 12:28:52.000000 uatg-1.9.0/uatg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66406 2023-07-11 12:28:52.000000 uatg-1.9.0/uatg/instruction_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34654 2023-07-11 12:28:52.000000 uatg-1.9.0/uatg/instruction_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31817 2023-07-11 12:28:52.000000 uatg-1.9.0/uatg/isem.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-07-11 12:28:52.000000 uatg-1.9.0/uatg/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19681 2023-07-11 12:28:52.000000 uatg-1.9.0/uatg/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-07-11 12:28:52.000000 uatg-1.9.0/uatg/regex_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-11 12:28:52.000000 uatg-1.9.0/uatg/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    28449 2023-07-11 12:28:52.000000 uatg-1.9.0/uatg/test_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55622 2023-07-11 12:28:52.000000 uatg-1.9.0/uatg/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:29:09.000000 uatg-1.9.0/uatg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-11 12:29:09.000000 uatg-1.9.0/uatg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-11 12:29:09.000000 uatg-1.9.0/uatg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 12:29:09.000000 uatg-1.9.0/uatg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-11 12:29:09.000000 uatg-1.9.0/uatg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 12:29:09.000000 uatg-1.9.0/uatg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-11 12:29:09.000000 uatg-1.9.0/uatg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-11 12:29:09.000000 uatg-1.9.0/uatg.egg-info/top_level.txt
```

### Comparing `uatg-1.8.0/LICENSE.incore` & `uatg-1.9.0/LICENSE.incore`

 * *Files identical despite different names*

### Comparing `uatg-1.8.0/PKG-INFO` & `uatg-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: uatg
-Version: 1.8.0
+Version: 1.9.0
 Summary: UATG - Micro-Architecture (µArch) Tests Generator
 Home-page: https://github.com/incoresemi/uatg
 Author: InCore Semiconductors Pvt. Ltd.
 Author-email: neelgala@incoresemi.com
 License: BSD-3-Clause
 Description: #########################################
         **UATG - μArchitectural Tests Generator**
```

### Comparing `uatg-1.8.0/setup.py` & `uatg-1.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 setup_requirements = []
 
 test_requirements = []
 
 setup(
     name='uatg',
-    version='1.8.0',
+    version='1.9.0',
     description="UATG - Micro-Architecture (µArch) Tests Generator",
     long_description=readme + '\n\n',
     classifiers=[
         "Programming Language :: Python :: 3.7",
         "License :: OSI Approved :: BSD License",
         "Development Status :: 3 - Alpha"
     ],
```

### Comparing `uatg-1.8.0/uatg/instruction_constants.py` & `uatg-1.9.0/uatg/instruction_constants.py`

 * *Files identical despite different names*

### Comparing `uatg-1.8.0/uatg/instruction_generator.py` & `uatg-1.9.0/uatg/instruction_generator.py`

 * *Files identical despite different names*

### Comparing `uatg-1.8.0/uatg/isem.yaml` & `uatg-1.9.0/uatg/isem.yaml`

 * *Files identical despite different names*

### Comparing `uatg-1.8.0/uatg/log.py` & `uatg-1.9.0/uatg/log.py`

 * *Files identical despite different names*

### Comparing `uatg-1.8.0/uatg/main.py` & `uatg-1.9.0/uatg/main.py`

 * *Files identical despite different names*

### Comparing `uatg-1.8.0/uatg/regex_formats.py` & `uatg-1.9.0/uatg/regex_formats.py`

 * *Files identical despite different names*

### Comparing `uatg-1.8.0/uatg/test_generator.py` & `uatg-1.9.0/uatg/test_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     """
         for every plugin, a process shall be spawned.
         The new process shall create an Assembly test file.
     """
     # unpacking the args tuple
     plugin, core_yaml, isa_yaml, isa, test_format_string, work_tests_dir, \
     make_file, module, linker_dir, uarch_dir, work_dir, \
-    compile_macros_dict, module_test_count_dict, page_modes = args
+    compile_macros_dict, self_checking_dict, module_test_count_dict, page_modes = args
 
     # actual generation process
     check = plugin.plugin_object.execute(core_yaml, isa_yaml)
 
     name = (str(plugin.plugin_object).split(".", 1))
     t_name = ((name[1].split(" ", 1))[0])
 
@@ -77,14 +77,21 @@
                 asm_sig = '\n'
 
             # create an entry in the compile_macros dict
             if 'rv64' in isa.lower():
                 compile_macros_dict[test_name] = ['XLEN=64']
             else:
                 compile_macros_dict[test_name] = ['XLEN=32']
+            
+            # if self_checking is included in returned dictionary, set the value accordingly
+            # else, default it to False
+            try:
+                self_checking_dict[test_name] = ret_list_of_dicts['self_checking']
+            except KeyError:
+                self_checking_dict[test_name] = False
 
             list_of_env_paths = [join(dirname(__file__), 'env/arch_test_unpriv.h'),
                                  join(dirname(__file__), 'env/arch_test_priv.h')]
             
             try:
                 available_macros = macros_parser(list_of_env_paths)
                 for i in ret_list_of_dicts['compile_macros']:
@@ -353,14 +360,18 @@
     # test_list_dict = process_manager.dict()
     test_list_dict = {}
 
     # creating a shared compile_macros dict
     # this dictionary will contain all the compile macros for each test
     compile_macros_dict = process_manager.dict()
 
+    # Create a shared self_checking flag dict
+    # this dictionary will store the status of self_check flag for each test
+    self_checking_dict = process_manager.dict()
+
     if exists(join(work_dir, 'makefile')):
         remove(join(work_dir, 'makefile'))
 
     logger.info('****** Generating Tests ******')
 
     total_test_count_dict = {}
 
@@ -431,15 +442,15 @@
         # Loop around and find the plugins and writes the contents from the
         # plugins into an asm file
         arg_list = []
         for plugin in manager.getAllPlugins():
             arg_list.append(
                 (plugin, core_yaml, isa_yaml, isa, test_format_string,
                  work_tests_dir, make_file, module, linker_dir, uarch_dir,
-                 work_dir, compile_macros_dict, module_test_count_dict,
+                 work_dir, compile_macros_dict, self_checking_dict, module_test_count_dict,
                  paging_modes))
 
         # multi processing process pool
         logger.info(f"Spawning {jobs} processes")
         process_pool = Pool(jobs)
         # creating a map of processes
         process_pool.map(asm_generation_process, arg_list)
@@ -461,15 +472,15 @@
 
         logger.info(f'Finished Generating Assembly Tests for {module}')
 
         if test_list:
             logger.info(f'Creating test_list for the {module}')
             test_list_dict.update(
                 generate_test_list(work_tests_dir, uarch_dir, isa,
-                                   test_list_dict, compile_macros_dict))
+                                   test_list_dict, compile_macros_dict, self_checking_dict))
 
     logger.info('Assembly generation for all modules completed')
 
     with open(join(work_dir, 'makefile'), 'w') as f:
         logger.info('Dumping makefile')
         f.write('all' + ': ')
         f.write(' \\\n\t'.join(make_file['all']))
```

### Comparing `uatg-1.8.0/uatg/utils.py` & `uatg-1.9.0/uatg/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -761,15 +761,15 @@
                 extension_list.append(e)
         if z != '':
             extension_list.append(z)
 
     return extension_list
 
 
-def generate_test_list(asm_dir, uarch_dir, isa, test_list, compile_macros_dict):
+def generate_test_list(asm_dir, uarch_dir, isa, test_list, compile_macros_dict, self_checking_dict):
     """
       updates the test_list.yaml file with the location of the
       tests generated by test_generator as well the directory to dump the logs.
       Check the test_list format documentation present.
       The test list generation is an optional feature which the user may choose
       to use.
     """
@@ -801,14 +801,15 @@
             target_dir, 'link.ld'))
         test_list[base_key]['asm_file'] = abspath(
             join(asm_dir, base_key, base_key + '.S'))
         test_list[base_key]['include'] = [env_dir, target_dir]
         test_list[base_key]['compile_macros'] = compile_macros_dict[base_key]
         test_list[base_key]['extra_compile'] = []
         test_list[base_key]['result'] = 'Unavailable'
+        test_list[base_key]['self_checking'] = self_checking_dict[base_key]
     return test_list
 
 
 def generate_sv_components(sv_dir, alias_file):
     """
     invokes the methods within the sv_components class and creates the sv files.
     tb_top.sv, interface.sv and Defines.sv are created.
```

### Comparing `uatg-1.8.0/uatg.egg-info/PKG-INFO` & `uatg-1.9.0/uatg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: uatg
-Version: 1.8.0
+Version: 1.9.0
 Summary: UATG - Micro-Architecture (µArch) Tests Generator
 Home-page: https://github.com/incoresemi/uatg
 Author: InCore Semiconductors Pvt. Ltd.
 Author-email: neelgala@incoresemi.com
 License: BSD-3-Clause
 Description: #########################################
         **UATG - μArchitectural Tests Generator**
```

