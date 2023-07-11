# Comparing `tmp/jVMC-1.2.3.tar.gz` & `tmp/jVMC-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jVMC-1.2.3.tar", last modified: Mon Jul  3 11:50:25 2023, max compression
+gzip compressed data, was "jVMC-1.2.4.tar", last modified: Tue Jul 11 17:02:53 2023, max compression
```

## Comparing `jVMC-1.2.3.tar` & `jVMC-1.2.4.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:50:25.298665 jVMC-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-03 11:50:15.000000 jVMC-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-03 11:50:25.298665 jVMC-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-03 11:50:15.000000 jVMC-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:50:25.294665 jVMC-1.2.3/jVMC/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/global_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/mpi_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:50:25.294665 jVMC-1.2.3/jVMC/nets/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/nets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/nets/activation_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/nets/cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/nets/ffn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/nets/initializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/nets/rbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/nets/rnn1d_general.py
--rw-r--r--   0 runner    (1001) docker     (123)    13674 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/nets/rnn2d_general.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/nets/sym_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/nets/two_nets_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:50:25.294665 jVMC-1.2.3/jVMC/operator/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12194 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/operator/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/operator/branch_free.py
--rw-r--r--   0 runner    (1001) docker     (123)    19685 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/operator/povm.py
--rw-r--r--   0 runner    (1001) docker     (123)    21051 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8537 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:50:25.294665 jVMC-1.2.3/jVMC/util/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/util/minsr.py
--rw-r--r--   0 runner    (1001) docker     (123)     7730 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/util/output_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/util/stepper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/util/symmetries.py
--rw-r--r--   0 runner    (1001) docker     (123)    12322 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/util/tdvp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/util/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    18494 2023-07-03 11:50:15.000000 jVMC-1.2.3/jVMC/vqs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:50:25.294665 jVMC-1.2.3/jVMC.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-03 11:50:25.000000 jVMC-1.2.3/jVMC.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-03 11:50:25.000000 jVMC-1.2.3/jVMC.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 11:50:25.000000 jVMC-1.2.3/jVMC.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-03 11:50:25.000000 jVMC-1.2.3/jVMC.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-03 11:50:25.000000 jVMC-1.2.3/jVMC.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 11:50:25.298665 jVMC-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-03 11:50:15.000000 jVMC-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 11:50:25.298665 jVMC-1.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 11:50:15.000000 jVMC-1.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-03 11:50:15.000000 jVMC-1.2.3/tests/minsr_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-03 11:50:15.000000 jVMC-1.2.3/tests/mpi_wrapper_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-07-03 11:50:15.000000 jVMC-1.2.3/tests/nets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-07-03 11:50:15.000000 jVMC-1.2.3/tests/operator_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-07-03 11:50:15.000000 jVMC-1.2.3/tests/povm_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17909 2023-07-03 11:50:15.000000 jVMC-1.2.3/tests/sampler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-03 11:50:15.000000 jVMC-1.2.3/tests/stats_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-03 11:50:15.000000 jVMC-1.2.3/tests/stepper_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-07-03 11:50:15.000000 jVMC-1.2.3/tests/symmetries_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-07-03 11:50:15.000000 jVMC-1.2.3/tests/tdvp_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9497 2023-07-03 11:50:15.000000 jVMC-1.2.3/tests/vqs_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:02:53.643095 jVMC-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-11 17:02:43.000000 jVMC-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-11 17:02:53.643095 jVMC-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-11 17:02:43.000000 jVMC-1.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:02:53.631095 jVMC-1.2.4/jVMC/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-11 17:02:43.000000 jVMC-1.2.4/jVMC/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-11 17:02:43.000000 jVMC-1.2.4/jVMC/global_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-07-11 17:02:43.000000 jVMC-1.2.4/jVMC/mpi_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:02:53.635095 jVMC-1.2.4/jVMC/nets/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-11 17:02:43.000000 jVMC-1.2.4/jVMC/nets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-11 17:02:43.000000 jVMC-1.2.4/jVMC/nets/activation_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-07-11 17:02:43.000000 jVMC-1.2.4/jVMC/nets/cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-07-11 17:02:43.000000 jVMC-1.2.4/jVMC/nets/ffn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-11 17:02:43.000000 jVMC-1.2.4/jVMC/nets/initializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-07-11 17:02:43.000000 jVMC-1.2.4/jVMC/nets/rbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-07-11 17:02:43.000000 jVMC-1.2.4/jVMC/nets/rnn1d_general.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13674 2023-07-11 17:02:43.000000 jVMC-1.2.4/jVMC/nets/rnn2d_general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-11 17:02:43.000000 jVMC-1.2.4/jVMC/nets/sym_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-11 17:02:43.000000 jVMC-1.2.4/jVMC/nets/two_nets_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:02:53.635095 jVMC-1.2.4/jVMC/operator/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-11 17:02:43.000000 jVMC-1.2.4/jVMC/operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12194 2023-07-11 17:02:43.000000 jVMC-1.2.4/jVMC/operator/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-07-11 17:02:43.000000 jVMC-1.2.4/jVMC/operator/branch_free.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19685 2023-07-11 17:02:43.000000 jVMC-1.2.4/jVMC/operator/povm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21782 2023-07-11 17:02:43.000000 jVMC-1.2.4/jVMC/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8537 2023-07-11 17:02:43.000000 jVMC-1.2.4/jVMC/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:02:53.639095 jVMC-1.2.4/jVMC/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-11 17:02:43.000000 jVMC-1.2.4/jVMC/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-07-11 17:02:43.000000 jVMC-1.2.4/jVMC/util/minsr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7730 2023-07-11 17:02:43.000000 jVMC-1.2.4/jVMC/util/output_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-07-11 17:02:43.000000 jVMC-1.2.4/jVMC/util/stepper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8869 2023-07-11 17:02:43.000000 jVMC-1.2.4/jVMC/util/symmetries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12322 2023-07-11 17:02:43.000000 jVMC-1.2.4/jVMC/util/tdvp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-07-11 17:02:43.000000 jVMC-1.2.4/jVMC/util/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-11 17:02:43.000000 jVMC-1.2.4/jVMC/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18600 2023-07-11 17:02:43.000000 jVMC-1.2.4/jVMC/vqs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:02:53.631095 jVMC-1.2.4/jVMC.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-11 17:02:53.000000 jVMC-1.2.4/jVMC.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-07-11 17:02:53.000000 jVMC-1.2.4/jVMC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 17:02:53.000000 jVMC-1.2.4/jVMC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-11 17:02:53.000000 jVMC-1.2.4/jVMC.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-11 17:02:53.000000 jVMC-1.2.4/jVMC.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 17:02:53.643095 jVMC-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-11 17:02:43.000000 jVMC-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:02:53.643095 jVMC-1.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:02:43.000000 jVMC-1.2.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-07-11 17:02:43.000000 jVMC-1.2.4/tests/minsr_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-11 17:02:43.000000 jVMC-1.2.4/tests/mpi_wrapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-07-11 17:02:43.000000 jVMC-1.2.4/tests/nets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-07-11 17:02:43.000000 jVMC-1.2.4/tests/operator_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-07-11 17:02:43.000000 jVMC-1.2.4/tests/povm_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19642 2023-07-11 17:02:43.000000 jVMC-1.2.4/tests/sampler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-11 17:02:43.000000 jVMC-1.2.4/tests/stats_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-11 17:02:43.000000 jVMC-1.2.4/tests/stepper_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-07-11 17:02:43.000000 jVMC-1.2.4/tests/symmetries_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-07-11 17:02:43.000000 jVMC-1.2.4/tests/tdvp_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9497 2023-07-11 17:02:43.000000 jVMC-1.2.4/tests/vqs_test.py
```

### Comparing `jVMC-1.2.3/LICENSE` & `jVMC-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.3/PKG-INFO` & `jVMC-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jVMC
-Version: 1.2.3
+Version: 1.2.4
 Summary: jVMC: Versatile and performant variational Monte Carlo
 Home-page: https://jvmc.readthedocs.io/en/latest/#
 Author: Markus Schmitt, Moritz Reh
 Author-email: markus.schmitt@uni-koeln.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jVMC-1.2.3/README.md` & `jVMC-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.3/jVMC/global_defs.py` & `jVMC-1.2.4/jVMC/global_defs.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.3/jVMC/mpi_wrapper.py` & `jVMC-1.2.4/jVMC/mpi_wrapper.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.3/jVMC/nets/activation_functions.py` & `jVMC-1.2.4/jVMC/nets/activation_functions.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.3/jVMC/nets/cnn.py` & `jVMC-1.2.4/jVMC/nets/cnn.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.3/jVMC/nets/ffn.py` & `jVMC-1.2.4/jVMC/nets/ffn.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.3/jVMC/nets/initializers.py` & `jVMC-1.2.4/jVMC/nets/initializers.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.3/jVMC/nets/rbm.py` & `jVMC-1.2.4/jVMC/nets/rbm.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.3/jVMC/nets/rnn1d_general.py` & `jVMC-1.2.4/jVMC/nets/rnn1d_general.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.3/jVMC/nets/rnn2d_general.py` & `jVMC-1.2.4/jVMC/nets/rnn2d_general.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.3/jVMC/nets/sym_wrapper.py` & `jVMC-1.2.4/jVMC/nets/sym_wrapper.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.3/jVMC/nets/two_nets_wrapper.py` & `jVMC-1.2.4/jVMC/nets/two_nets_wrapper.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.3/jVMC/operator/base.py` & `jVMC-1.2.4/jVMC/operator/base.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.3/jVMC/operator/branch_free.py` & `jVMC-1.2.4/jVMC/operator/branch_free.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.3/jVMC/operator/povm.py` & `jVMC-1.2.4/jVMC/operator/povm.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.3/jVMC/sampler.py` & `jVMC-1.2.4/jVMC/sampler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import jax
 import jax.numpy as jnp
 import jax.random as random
 import numpy as np
 from jax import vmap, jit
+import flax
 
 import jVMC.mpi_wrapper as mpi
 from jVMC.nets.sym_wrapper import SymNet
 
 from functools import partial
 
 import time
@@ -208,16 +209,22 @@
             A sample of computational basis configurations drawn from :math:`p_{\\mu}(s)`.
         """
 
         if numSamples is None:
             numSamples = self.numSamples
 
         if self.net.is_generator:
-            configs = self._get_samples_gen(parameters, numSamples, multipleOf)
-            return configs, self.net(configs), jnp.ones(configs.shape[:2]) / jnp.prod(jnp.asarray(configs.shape[:2]))
+            if parameters is not None:
+                tmpP = self.net.params
+                self.net.set_parameters(parameters)
+            configs = self._get_samples_gen(self.net.parameters, numSamples, multipleOf)
+            coeffs = self.net(configs)
+            if parameters is not None:
+                self.net.params = tmpP
+            return configs, coeffs, jnp.ones(configs.shape[:2]) / jnp.prod(jnp.asarray(configs.shape[:2]))
 
         configs, logPsi = self._get_samples_mcmc(parameters, numSamples, multipleOf)
         p = jnp.exp((1.0 / self.logProbFactor - self.mu) * jnp.real(logPsi))
         return configs, logPsi, p / mpi.global_sum(p)
 
     def _randomize_samples(self, samples, key, orbit):
         """ For a given set of samples apply a random symmetry transformation to each sample
@@ -243,21 +250,26 @@
         if not self.orbit is None:
             return self._randomize_samples_jitd[str(numSamples)](samples, tmpKey2, self.orbit)
         
         return samples
 
     def _get_samples_mcmc(self, params, numSamples, multipleOf=1):
 
-        net, netParams = self.net.get_sampler_net()
+        tmpP = None
+        if params is not None:
+            tmpP = self.net.params
+            self.net.set_parameters(params)
 
-        if params is None:
-            params = netParams
+        net, params = self.net.get_sampler_net()
+
+        if tmpP is not None:
+            self.net.params = tmpP        
 
         # Initialize sampling stuff
-        self._mc_init(netParams)
+        self._mc_init(params)
 
         numSamples = mpi.distribute_sampling(numSamples, localDevices=global_defs.device_count(), numChainsPerDevice=np.lcm(self.numChains, multipleOf))
         numSamplesStr = str(numSamples)
 
         # check whether _get_samples is already compiled for given number of samples
         if not numSamplesStr in self._get_samples_jitd:
             self._get_samples_jitd[numSamplesStr] = global_defs.pmap_for_my_devices(partial(self._get_samples, sweepFunction=partial(self._sweep, net=net)),
@@ -265,16 +277,21 @@
                                                                                     in_axes=(None, None, None, None, 0, 0, 0, 0, 0, None, None, None))
 
         (self.states, self.logAccProb, self.key, self.numProposed, self.numAccepted), configs =\
             self._get_samples_jitd[numSamplesStr](params, numSamples, self.thermalizationSweeps, self.sweepSteps,
                                                   self.states, self.logAccProb, self.key, self.numProposed, self.numAccepted,
                                                   self.updateProposer, self.updateProposerArg, self.sampleShape)
 
+        tmpP = self.net.params
+        self.net.params = params["params"]
+        coeffs = self.net(configs)
+        self.net.params = tmpP
+
         # return configs, None
-        return configs, self.net(configs)
+        return configs, coeffs
 
     def _get_samples(self, params, numSamples,
                      thermSweeps, sweepSteps,
                      states, logAccProb, key,
                      numProposed, numAccepted,
                      updateProposer, updateProposerArg,
                      sampleShape, sweepFunction=None):
@@ -483,15 +500,20 @@
 
         Returns:
             ``configs, logPsi, p``: All computational basis configurations, \
             corresponding wave function coefficients, and probabilities \
             :math:`|\psi(s)|^2` (normalized).
         """
 
+        if parameters is not None:
+            tmpP = self.psi.get_parameters()
+            self.psi.set_parameters(parameters)
         logPsi = self.psi(self.basis)
+        if parameters is not None:
+            self.psi.set_parameters(tmpP)
 
         p = self._compute_probabilities_pmapd(logPsi, self.lastNorm, self.numStatesPerDevice)
 
         nrm = mpi.global_sum(p)
         p = self._normalize_pmapd(p, nrm)
 
         self.lastNorm += self.logProbFactor * jnp.log(nrm)
```

### Comparing `jVMC-1.2.3/jVMC/stats.py` & `jVMC-1.2.4/jVMC/stats.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.3/jVMC/util/minsr.py` & `jVMC-1.2.4/jVMC/util/minsr.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.3/jVMC/util/output_manager.py` & `jVMC-1.2.4/jVMC/util/output_manager.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.3/jVMC/util/stepper.py` & `jVMC-1.2.4/jVMC/util/stepper.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.3/jVMC/util/symmetries.py` & `jVMC-1.2.4/jVMC/util/symmetries.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.3/jVMC/util/tdvp.py` & `jVMC-1.2.4/jVMC/util/tdvp.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.3/jVMC/util/util.py` & `jVMC-1.2.4/jVMC/util/util.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.3/jVMC/vqs.py` & `jVMC-1.2.4/jVMC/vqs.py`

 * *Files 1% similar despite different names*

```diff
@@ -413,15 +413,18 @@
             * ``P``: New values of variational parameters.
         """
 
         if not self.initialized:
             raise RuntimeError("Error in NQS.set_parameters(): Network not initialized. Evaluate net on example input for initialization.")
 
         # Update model parameters
-        self.params = self._param_unflatten(P)
+        if isinstance(P, flax.core.frozen_dict.FrozenDict):
+            self.params = P
+        else:
+            self.params = self._param_unflatten(P)
 
     # **  end def set_parameters
 
 
     def _param_unflatten(self, P):
 
         # Reshape parameter update according to net tree structure
```

### Comparing `jVMC-1.2.3/jVMC.egg-info/PKG-INFO` & `jVMC-1.2.4/jVMC.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jVMC
-Version: 1.2.3
+Version: 1.2.4
 Summary: jVMC: Versatile and performant variational Monte Carlo
 Home-page: https://jvmc.readthedocs.io/en/latest/#
 Author: Markus Schmitt, Moritz Reh
 Author-email: markus.schmitt@uni-koeln.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jVMC-1.2.3/jVMC.egg-info/SOURCES.txt` & `jVMC-1.2.4/jVMC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.3/setup.py` & `jVMC-1.2.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open("./jVMC/version.py") as fp:
     exec(fp.read(), version)
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
-DEFAULT_DEPENDENCIES = ["setuptools", "wheel", "numpy", "jax>=0.4.1,<=0.4.11", "jaxlib>=0.4.1,<=0.4.11", "flax>=0.6.4", "mpi4py", "h5py", "PyYAML", "matplotlib"]
+DEFAULT_DEPENDENCIES = ["setuptools", "wheel", "numpy", "jax>=0.4.1,<=0.4.11", "jaxlib>=0.4.1,<=0.4.11", "flax>=0.6.4,<=0.6.11", "mpi4py", "h5py", "PyYAML", "matplotlib"]
 #CUDA_DEPENDENCIES = ["setuptools", "wheel", "numpy", "jax[cuda]>=0.2.11,<=0.2.25", "flax>=0.3.6,<=0.3.6", "mpi4py", "h5py"]
 DEV_DEPENDENCIES = DEFAULT_DEPENDENCIES + ["sphinx", "mock", "sphinx_rtd_theme", "pytest", "pytest-mpi"]
 
 setuptools.setup(
     name='jVMC',
     version=version['__version__'],
     author="Markus Schmitt, Moritz Reh",
```

### Comparing `jVMC-1.2.3/tests/minsr_test.py` & `jVMC-1.2.4/tests/minsr_test.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.3/tests/mpi_wrapper_test.py` & `jVMC-1.2.4/tests/mpi_wrapper_test.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.3/tests/nets_test.py` & `jVMC-1.2.4/tests/nets_test.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.3/tests/operator_test.py` & `jVMC-1.2.4/tests/operator_test.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.3/tests/povm_test.py` & `jVMC-1.2.4/tests/povm_test.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.3/tests/sampler_test.py` & `jVMC-1.2.4/tests/sampler_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 
         # Set up exact sampler
         exactSampler = sampler.ExactSampler(psi, L)
 
         # Set up MCMC sampler
         mcSampler = sampler.MCSampler(psi, (L,), random.PRNGKey(0), updateProposer=jVMC.sampler.propose_spin_flip, numChains=777)
 
+        p0 = psi.get_parameters()
         psi.set_parameters(weights)
 
         # Compute exact probabilities
         _, _, pex = exactSampler.sample()
 
         # Get samples from MCMC sampler
         numSamples = 500000
@@ -71,14 +72,22 @@
         # Compute histogram of sampled configurations
         smcInt = jax.vmap(state_to_int)(smc)
         pmc, _ = np.histogram(smcInt, bins=np.arange(0, 17), weights=p[0])
 
         # Compare histogram to exact probabilities
         self.assertTrue(jnp.max(jnp.abs(pmc - pex.reshape((-1,))[:16])) < 2e-3)
 
+        
+        s, psi_s, _ = mcSampler.sample(parameters=p0, numSamples=100)
+        psi.set_parameters(p0)
+        psi_s1 = psi(s)
+        
+        self.assertTrue(jnp.max(jnp.abs((psi_s - psi_s1) / psi_s)) < 1e-14)
+
+
     def test_MCMC_sampling_with_mu(self):
         mu = 1
 
         L = 4
 
         weights = jnp.array(
             [0.23898957, 0.12614753, 0.19479055, 0.17325271, 0.14619853, 0.21392751,
@@ -287,14 +296,23 @@
         self.assertTrue(smc.shape[0] >= numSamples)
 
         # Compute histogram of sampled configurations
         smcInt = jax.vmap(state_to_int)(smc)
         pmc, _ = np.histogram(smcInt, bins=np.arange(0, 17), weights=p[0])
 
         self.assertTrue(jnp.max(jnp.abs(pmc - pex.reshape((-1,))[:16])) < 1.1e-3)
+        
+        
+        psi1 = NQS(net, seed=98475)
+        # Set up another MCMC sampler
+        mcSampler = sampler.MCSampler(psi1, (L,), random.PRNGKey(0), updateProposer=jVMC.sampler.propose_spin_flip, numChains=777)
+        s, psi_s, _ = mcSampler.sample(parameters=psi.get_parameters(), numSamples=100)
+        psi_s1 = psi(s)
+        
+        self.assertTrue(jnp.max(jnp.abs((psi_s - psi_s1) / psi_s)) < 1e-14)
 
     def test_autoregressive_sampling_with_symmetries(self):
 
         L = 4
 
         # Set up variational wave function
         rnn = nets.RNN1DGeneral(L=L, hiddenSize=5, realValuedOutput=True)
@@ -507,9 +525,43 @@
         # Compute histogram of sampled configurations
         smcInt = jax.vmap(state_to_int)(smc)
         pmc, _ = np.histogram(smcInt, bins=np.arange(0, 17), weights=p[0])
 
         self.assertTrue(jnp.max(jnp.abs(pmc - pex.reshape((-1,))[:16])) < 1e-3)
 
 
+class TestExactSampler(unittest.TestCase):
+
+    def test_exact_sampler(self):
+        L = 4
+
+        weights = jnp.array(
+            [0.23898957, 0.12614753, 0.19479055, 0.17325271, 0.14619853, 0.21392751,
+             0.19648707, 0.17103704, -0.15457255, 0.10954413, 0.13228065, -0.14935214,
+             -0.09963073, 0.17610707, 0.13386381, -0.14836467]
+        )
+
+        # Set up variational wave function
+        rbm = nets.CpxRBM(numHidden=2, bias=False)
+        psi = NQS(rbm)
+
+        # Set up exact sampler
+        exactSampler = sampler.ExactSampler(psi, L)
+
+        p0 = psi.get_parameters()
+        psi.set_parameters(weights)
+
+        # Compute exact probabilities
+        s, psi_s, pex = exactSampler.sample()
+
+        import flax
+        print(isinstance(psi.parameters, flax.core.frozen_dict.FrozenDict))
+        self.assertTrue(jnp.max((psi(s) - psi_s) / psi_s) < 1e-14)
+        
+        s, psi_s, pex = exactSampler.sample(parameters=p0)
+
+        psi.set_parameters(p0)
+        self.assertTrue(jnp.max((psi(s) - psi_s) / psi_s) < 1e-14)
+
+
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `jVMC-1.2.3/tests/stats_test.py` & `jVMC-1.2.4/tests/stats_test.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.3/tests/stepper_test.py` & `jVMC-1.2.4/tests/stepper_test.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.3/tests/symmetries_test.py` & `jVMC-1.2.4/tests/symmetries_test.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.3/tests/tdvp_test.py` & `jVMC-1.2.4/tests/tdvp_test.py`

 * *Files identical despite different names*

### Comparing `jVMC-1.2.3/tests/vqs_test.py` & `jVMC-1.2.4/tests/vqs_test.py`

 * *Files identical despite different names*

