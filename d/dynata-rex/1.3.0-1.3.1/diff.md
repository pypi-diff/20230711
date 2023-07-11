# Comparing `tmp/dynata_rex-1.3.0.tar.gz` & `tmp/dynata_rex-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynata_rex-1.3.0.tar", last modified: Wed May 31 23:09:17 2023, max compression
+gzip compressed data, was "dynata_rex-1.3.1.tar", last modified: Tue Jul 11 17:47:08 2023, max compression
```

## Comparing `dynata_rex-1.3.0.tar` & `dynata_rex-1.3.1.tar`

### file list

```diff
@@ -1,50 +1,57 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 23:09:17.701019 dynata_rex-1.3.0/
--rw-r--r--   0 root         (0) root         (0)     1063 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     9699 2023-05-31 23:09:17.702019 dynata_rex-1.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8929 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 23:09:17.694019 dynata_rex-1.3.0/dynata_rex/
--rw-r--r--   0 root         (0) root         (0)      661 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/dynata_rex/__init__.py
--rw-r--r--   0 root         (0) root         (0)      732 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/dynata_rex/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2029 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/dynata_rex/helpers.py
--rw-r--r--   0 root         (0) root         (0)      378 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/dynata_rex/logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 23:09:17.696019 dynata_rex-1.3.0/dynata_rex/models/
--rw-r--r--   0 root         (0) root         (0)      989 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/dynata_rex/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1126 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/dynata_rex/models/base.py
--rw-r--r--   0 root         (0) root         (0)     3526 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/dynata_rex/models/opportunity_registry.py
--rw-r--r--   0 root         (0) root         (0)     3561 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/dynata_rex/models/respondent_gateway.py
--rw-r--r--   0 root         (0) root         (0)     7668 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/dynata_rex/opportunity_registry.py
--rw-r--r--   0 root         (0) root         (0)    11434 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/dynata_rex/respondent_gateway.py
--rw-r--r--   0 root         (0) root         (0)     8715 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/dynata_rex/signer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 23:09:17.695019 dynata_rex-1.3.0/dynata_rex.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9699 2023-05-31 23:09:17.000000 dynata_rex-1.3.0/dynata_rex.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1767 2023-05-31 23:09:17.000000 dynata_rex-1.3.0/dynata_rex.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 23:09:17.000000 dynata_rex-1.3.0/dynata_rex.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      174 2023-05-31 23:09:17.000000 dynata_rex-1.3.0/dynata_rex.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-05-31 23:09:17.000000 dynata_rex-1.3.0/dynata_rex.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 23:09:17.697019 dynata_rex-1.3.0/examples/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 23:09:17.698019 dynata_rex-1.3.0/examples/opportunity_registry/
--rw-r--r--   0 root         (0) root         (0)      111 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/opportunity_registry/01_instantiate_client.py
--rw-r--r--   0 root         (0) root         (0)      280 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/opportunity_registry/02_receive_notifications.py
--rw-r--r--   0 root         (0) root         (0)      267 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/opportunity_registry/03_convert_opportunity_json.py
--rw-r--r--   0 root         (0) root         (0)      275 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/opportunity_registry/04_acknowledge_multiple_notifications.py
--rw-r--r--   0 root         (0) root         (0)      236 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/opportunity_registry/05_acknowledge_single_notification.py
--rw-r--r--   0 root         (0) root         (0)      329 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/opportunity_registry/06_list_corresponding_opportunities_by_project.py
--rw-r--r--   0 root         (0) root         (0)      190 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/opportunity_registry/07_download_collection_type_cell.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/opportunity_registry/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 23:09:17.701019 dynata_rex-1.3.0/examples/respondent_gateway/
--rw-r--r--   0 root         (0) root         (0)      106 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/respondent_gateway/01_instantiate_client.py
--rw-r--r--   0 root         (0) root         (0)      392 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/respondent_gateway/02_create_signed_link.py
--rw-r--r--   0 root         (0) root         (0)      447 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/respondent_gateway/03_create_quoted_signed_link.py
--rw-r--r--   0 root         (0) root         (0)      948 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/respondent_gateway/04_create_survey_link_for_panelist.py
--rw-r--r--   0 root         (0) root         (0)     1219 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/respondent_gateway/05_create_survey_link_for_panelist_with_custom_parameters.py
--rw-r--r--   0 root         (0) root         (0)     1316 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/respondent_gateway/06_verify_signed_url.py
--rw-r--r--   0 root         (0) root         (0)     1360 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/respondent_gateway/07_get_end_link_disposition.py
--rw-r--r--   0 root         (0) root         (0)      353 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/respondent_gateway/08_create_context.py
--rw-r--r--   0 root         (0) root         (0)      384 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/respondent_gateway/09_retrieve_context.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/respondent_gateway/10_expire_context.py
--rw-r--r--   0 root         (0) root         (0)      424 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/respondent_gateway/11_list_attributes.py
--rw-r--r--   0 root         (0) root         (0)     1437 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/respondent_gateway/12_get_attribute_info.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/examples/respondent_gateway/__init__.py
--rw-r--r--   0 root         (0) root         (0)       79 2023-05-31 23:09:17.703019 dynata_rex-1.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1473 2023-05-31 23:08:33.000000 dynata_rex-1.3.0/setup.py
+drwxr-xr-x   0 colton.nielsen   (503) staff       (20)        0 2023-07-11 17:47:08.096058 dynata_rex-1.3.1/
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)     1063 2023-05-09 18:27:19.000000 dynata_rex-1.3.1/LICENSE
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)     9681 2023-07-11 17:47:08.097215 dynata_rex-1.3.1/PKG-INFO
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)     8929 2023-07-10 22:15:40.000000 dynata_rex-1.3.1/README.md
+drwxr-xr-x   0 colton.nielsen   (503) staff       (20)        0 2023-07-11 17:47:08.065047 dynata_rex-1.3.1/dynata_rex/
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)      661 2023-05-09 18:27:19.000000 dynata_rex-1.3.1/dynata_rex/__init__.py
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)      732 2023-05-09 18:27:19.000000 dynata_rex-1.3.1/dynata_rex/exceptions.py
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)     2029 2023-05-09 18:27:19.000000 dynata_rex-1.3.1/dynata_rex/helpers.py
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)      378 2023-05-09 18:27:19.000000 dynata_rex-1.3.1/dynata_rex/logs.py
+drwxr-xr-x   0 colton.nielsen   (503) staff       (20)        0 2023-07-11 17:47:08.073491 dynata_rex-1.3.1/dynata_rex/models/
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)      989 2023-07-10 22:15:40.000000 dynata_rex-1.3.1/dynata_rex/models/__init__.py
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)     1126 2023-03-20 17:15:41.000000 dynata_rex-1.3.1/dynata_rex/models/base.py
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)     3526 2023-07-11 17:26:13.000000 dynata_rex-1.3.1/dynata_rex/models/opportunity_registry.py
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)     3561 2023-07-10 22:15:40.000000 dynata_rex-1.3.1/dynata_rex/models/respondent_gateway.py
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)     7668 2023-07-11 17:26:13.000000 dynata_rex-1.3.1/dynata_rex/opportunity_registry.py
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)    11434 2023-07-10 22:15:40.000000 dynata_rex-1.3.1/dynata_rex/respondent_gateway.py
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)     8715 2023-05-09 18:27:19.000000 dynata_rex-1.3.1/dynata_rex/signer.py
+drwxr-xr-x   0 colton.nielsen   (503) staff       (20)        0 2023-07-11 17:47:08.070474 dynata_rex-1.3.1/dynata_rex.egg-info/
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)     9681 2023-07-11 17:47:07.000000 dynata_rex-1.3.1/dynata_rex.egg-info/PKG-INFO
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)     1928 2023-07-11 17:47:07.000000 dynata_rex-1.3.1/dynata_rex.egg-info/SOURCES.txt
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)        1 2023-07-11 17:47:07.000000 dynata_rex-1.3.1/dynata_rex.egg-info/dependency_links.txt
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)      174 2023-07-11 17:47:07.000000 dynata_rex-1.3.1/dynata_rex.egg-info/requires.txt
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)       20 2023-07-11 17:47:07.000000 dynata_rex-1.3.1/dynata_rex.egg-info/top_level.txt
+drwxr-xr-x   0 colton.nielsen   (503) staff       (20)        0 2023-07-11 17:47:08.074160 dynata_rex-1.3.1/examples/
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)        0 2023-05-09 18:27:19.000000 dynata_rex-1.3.1/examples/__init__.py
+drwxr-xr-x   0 colton.nielsen   (503) staff       (20)        0 2023-07-11 17:47:08.080531 dynata_rex-1.3.1/examples/opportunity_registry/
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)      111 2023-03-20 17:15:41.000000 dynata_rex-1.3.1/examples/opportunity_registry/01_instantiate_client.py
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)      280 2023-03-20 17:15:41.000000 dynata_rex-1.3.1/examples/opportunity_registry/02_receive_notifications.py
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)      267 2023-03-20 17:15:41.000000 dynata_rex-1.3.1/examples/opportunity_registry/03_convert_opportunity_json.py
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)      275 2023-03-20 17:15:41.000000 dynata_rex-1.3.1/examples/opportunity_registry/04_acknowledge_multiple_notifications.py
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)      236 2023-03-20 17:15:41.000000 dynata_rex-1.3.1/examples/opportunity_registry/05_acknowledge_single_notification.py
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)      329 2023-03-20 17:15:41.000000 dynata_rex-1.3.1/examples/opportunity_registry/06_list_corresponding_opportunities_by_project.py
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)      190 2023-03-20 17:15:41.000000 dynata_rex-1.3.1/examples/opportunity_registry/07_download_collection_type_cell.py
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)        0 2023-03-20 17:15:41.000000 dynata_rex-1.3.1/examples/opportunity_registry/__init__.py
+drwxr-xr-x   0 colton.nielsen   (503) staff       (20)        0 2023-07-11 17:47:08.090959 dynata_rex-1.3.1/examples/respondent_gateway/
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)      106 2023-03-20 17:15:41.000000 dynata_rex-1.3.1/examples/respondent_gateway/01_instantiate_client.py
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)      392 2023-03-20 17:15:41.000000 dynata_rex-1.3.1/examples/respondent_gateway/02_create_signed_link.py
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)      447 2023-03-20 17:15:41.000000 dynata_rex-1.3.1/examples/respondent_gateway/03_create_quoted_signed_link.py
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)      948 2023-03-20 17:15:41.000000 dynata_rex-1.3.1/examples/respondent_gateway/04_create_survey_link_for_panelist.py
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)     1219 2023-03-20 17:15:41.000000 dynata_rex-1.3.1/examples/respondent_gateway/05_create_survey_link_for_panelist_with_custom_parameters.py
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)     1316 2023-03-20 17:15:41.000000 dynata_rex-1.3.1/examples/respondent_gateway/06_verify_signed_url.py
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)     1360 2023-03-20 17:15:41.000000 dynata_rex-1.3.1/examples/respondent_gateway/07_get_end_link_disposition.py
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)      353 2023-03-20 17:15:41.000000 dynata_rex-1.3.1/examples/respondent_gateway/08_create_context.py
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)      384 2023-03-20 17:15:41.000000 dynata_rex-1.3.1/examples/respondent_gateway/09_retrieve_context.py
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)      432 2023-03-20 17:15:41.000000 dynata_rex-1.3.1/examples/respondent_gateway/10_expire_context.py
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)      424 2023-03-20 17:15:41.000000 dynata_rex-1.3.1/examples/respondent_gateway/11_list_attributes.py
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)     1437 2023-03-20 17:15:41.000000 dynata_rex-1.3.1/examples/respondent_gateway/12_get_attribute_info.py
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)        0 2023-03-20 17:15:41.000000 dynata_rex-1.3.1/examples/respondent_gateway/__init__.py
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)       79 2023-07-11 17:47:08.098231 dynata_rex-1.3.1/setup.cfg
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)     1473 2023-07-11 17:38:34.000000 dynata_rex-1.3.1/setup.py
+drwxr-xr-x   0 colton.nielsen   (503) staff       (20)        0 2023-07-11 17:47:08.095362 dynata_rex-1.3.1/tests/
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)     2631 2023-05-09 18:27:19.000000 dynata_rex-1.3.1/tests/test_helpers.py
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)     2230 2023-05-09 18:27:19.000000 dynata_rex-1.3.1/tests/test_models_base.py
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)     7186 2023-05-09 18:27:19.000000 dynata_rex-1.3.1/tests/test_opportunity_registry.py
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)     4938 2023-05-09 18:27:19.000000 dynata_rex-1.3.1/tests/test_requester.py
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)    19294 2023-07-10 22:15:40.000000 dynata_rex-1.3.1/tests/test_respondent_gateway.py
+-rw-r--r--   0 colton.nielsen   (503) staff       (20)     5459 2023-05-09 18:27:19.000000 dynata_rex-1.3.1/tests/test_signer.py
```

### Comparing `dynata_rex-1.3.0/LICENSE` & `dynata_rex-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dynata_rex-1.3.0/PKG-INFO` & `dynata_rex-1.3.1/dynata_rex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
-Name: dynata_rex
-Version: 1.3.0
+Name: dynata-rex
+Version: 1.3.1
 Summary: Package for building and interacting with the Dynata Respondent Exchange (REX)
 Home-page: https://github.com/dynata/rex-sdk-python
 Author: REX Maintainers
 Author-email: tech.supply@Dynata.com
-License: UNKNOWN
 Keywords: respondent exchange rex smor dynata python
 Platform: Any
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -357,8 +356,7 @@
 respondent_answers = PutRespondentAnswersRequest(
     respondent_id="respondent_id",
     attributes= [Attribute(attribute_id=111, answers=[111, 222, 333])]
 )
 
 gateway.put_respondent_answers(respondent_answers)
 ```
-
```

### Comparing `dynata_rex-1.3.0/README.md` & `dynata_rex-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `dynata_rex-1.3.0/dynata_rex/__init__.py` & `dynata_rex-1.3.1/dynata_rex/__init__.py`

 * *Files identical despite different names*

### Comparing `dynata_rex-1.3.0/dynata_rex/exceptions.py` & `dynata_rex-1.3.1/dynata_rex/exceptions.py`

 * *Files identical despite different names*

### Comparing `dynata_rex-1.3.0/dynata_rex/helpers.py` & `dynata_rex-1.3.1/dynata_rex/helpers.py`

 * *Files identical despite different names*

### Comparing `dynata_rex-1.3.0/dynata_rex/models/__init__.py` & `dynata_rex-1.3.1/dynata_rex/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dynata_rex-1.3.0/dynata_rex/models/base.py` & `dynata_rex-1.3.1/dynata_rex/models/base.py`

 * *Files identical despite different names*

### Comparing `dynata_rex-1.3.0/dynata_rex/models/opportunity_registry.py` & `dynata_rex-1.3.1/dynata_rex/models/opportunity_registry.py`

 * *Files identical despite different names*

### Comparing `dynata_rex-1.3.0/dynata_rex/models/respondent_gateway.py` & `dynata_rex-1.3.1/dynata_rex/models/respondent_gateway.py`

 * *Files identical despite different names*

### Comparing `dynata_rex-1.3.0/dynata_rex/opportunity_registry.py` & `dynata_rex-1.3.1/dynata_rex/opportunity_registry.py`

 * *Files identical despite different names*

### Comparing `dynata_rex-1.3.0/dynata_rex/respondent_gateway.py` & `dynata_rex-1.3.1/dynata_rex/respondent_gateway.py`

 * *Files identical despite different names*

### Comparing `dynata_rex-1.3.0/dynata_rex/signer.py` & `dynata_rex-1.3.1/dynata_rex/signer.py`

 * *Files identical despite different names*

### Comparing `dynata_rex-1.3.0/dynata_rex.egg-info/PKG-INFO` & `dynata_rex-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
-Name: dynata-rex
-Version: 1.3.0
+Name: dynata_rex
+Version: 1.3.1
 Summary: Package for building and interacting with the Dynata Respondent Exchange (REX)
 Home-page: https://github.com/dynata/rex-sdk-python
 Author: REX Maintainers
 Author-email: tech.supply@Dynata.com
-License: UNKNOWN
 Keywords: respondent exchange rex smor dynata python
 Platform: Any
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -357,8 +356,7 @@
 respondent_answers = PutRespondentAnswersRequest(
     respondent_id="respondent_id",
     attributes= [Attribute(attribute_id=111, answers=[111, 222, 333])]
 )
 
 gateway.put_respondent_answers(respondent_answers)
 ```
-
```

### Comparing `dynata_rex-1.3.0/dynata_rex.egg-info/SOURCES.txt` & `dynata_rex-1.3.1/dynata_rex.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -35,8 +35,14 @@
 examples/respondent_gateway/06_verify_signed_url.py
 examples/respondent_gateway/07_get_end_link_disposition.py
 examples/respondent_gateway/08_create_context.py
 examples/respondent_gateway/09_retrieve_context.py
 examples/respondent_gateway/10_expire_context.py
 examples/respondent_gateway/11_list_attributes.py
 examples/respondent_gateway/12_get_attribute_info.py
-examples/respondent_gateway/__init__.py
+examples/respondent_gateway/__init__.py
+tests/test_helpers.py
+tests/test_models_base.py
+tests/test_opportunity_registry.py
+tests/test_requester.py
+tests/test_respondent_gateway.py
+tests/test_signer.py
```

### Comparing `dynata_rex-1.3.0/examples/respondent_gateway/04_create_survey_link_for_panelist.py` & `dynata_rex-1.3.1/examples/respondent_gateway/04_create_survey_link_for_panelist.py`

 * *Files identical despite different names*

### Comparing `dynata_rex-1.3.0/examples/respondent_gateway/05_create_survey_link_for_panelist_with_custom_parameters.py` & `dynata_rex-1.3.1/examples/respondent_gateway/05_create_survey_link_for_panelist_with_custom_parameters.py`

 * *Files identical despite different names*

### Comparing `dynata_rex-1.3.0/examples/respondent_gateway/06_verify_signed_url.py` & `dynata_rex-1.3.1/examples/respondent_gateway/06_verify_signed_url.py`

 * *Files identical despite different names*

### Comparing `dynata_rex-1.3.0/examples/respondent_gateway/07_get_end_link_disposition.py` & `dynata_rex-1.3.1/examples/respondent_gateway/07_get_end_link_disposition.py`

 * *Files identical despite different names*

### Comparing `dynata_rex-1.3.0/examples/respondent_gateway/12_get_attribute_info.py` & `dynata_rex-1.3.1/examples/respondent_gateway/12_get_attribute_info.py`

 * *Files identical despite different names*

### Comparing `dynata_rex-1.3.0/setup.py` & `dynata_rex-1.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 
 setuptools.setup(
     name="dynata_rex",
-    version="1.3.0",
+    version="1.3.1",
     author="REX Maintainers",
     author_email="tech.supply@Dynata.com",
     description=("Package for building and interacting with the "
                  "Dynata Respondent Exchange (REX)"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dynata/rex-sdk-python",
@@ -21,19 +21,19 @@
     platforms=['Any'],
     install_requires=requirements,
     setup_requires=['pytest-runner'],
     extras_require={
         # pip install -e ".[testing]"
         "testing": ['pytest'],
         ':python_version == "3.6"': [
-            "typing-extensions==4.6.2",
+            "typing-extensions==4.7.1",
             'dataclasses==0.8'
         ],
         ':python_version == "3.7"': [
-            "typing-extensions==4.6.2"
+            "typing-extensions==4.7.1"
         ]
     },
     tests_require=['pytest'],
     keywords='respondent exchange rex smor dynata python',
     classifiers=[
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
```

