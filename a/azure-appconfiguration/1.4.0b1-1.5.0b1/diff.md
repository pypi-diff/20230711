# Comparing `tmp/azure-appconfiguration-1.4.0b1.zip` & `tmp/azure-appconfiguration-1.5.0b1.zip`

## zipinfo {}

```diff
@@ -1,94 +1,98 @@
-Zip file size: 126561 bytes, number of entries: 92
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-07 19:28 azure-appconfiguration-1.4.0b1/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-07 19:28 azure-appconfiguration-1.4.0b1/azure/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-07 19:28 azure-appconfiguration-1.4.0b1/tests/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-07 19:28 azure-appconfiguration-1.4.0b1/samples/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-07 19:28 azure-appconfiguration-1.4.0b1/azure_appconfiguration.egg-info/
--rw-rw-r--  2.0 unx     2540 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/setup.py
--rw-rw-r--  2.0 unx     3416 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/CHANGELOG.md
--rw-rw-r--  2.0 unx       38 b- defN 23-Feb-07 19:28 azure-appconfiguration-1.4.0b1/setup.cfg
--rw-rw-r--  2.0 unx    17683 b- defN 23-Feb-07 19:28 azure-appconfiguration-1.4.0b1/PKG-INFO
--rw-rw-r--  2.0 unx    13406 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/README.md
--rw-rw-r--  2.0 unx      188 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/MANIFEST.in
--rw-rw-r--  2.0 unx     1073 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/LICENSE
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-07 19:28 azure-appconfiguration-1.4.0b1/azure/appconfiguration/
--rw-rw-r--  2.0 unx       81 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-07 19:28 azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-07 19:28 azure-appconfiguration-1.4.0b1/azure/appconfiguration/aio/
--rw-rw-r--  2.0 unx     3150 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/azure/appconfiguration/_azure_appconfiguration_requests.py
--rw-rw-r--  2.0 unx     2472 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/azure/appconfiguration/_utils.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/azure/appconfiguration/py.typed
--rw-rw-r--  2.0 unx      331 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/azure/appconfiguration/_user_agent.py
--rw-rw-r--  2.0 unx      530 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/azure/appconfiguration/_azure_appconfiguration_error.py
--rw-rw-r--  2.0 unx    25698 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/azure/appconfiguration/_azure_appconfiguration_client.py
--rw-rw-r--  2.0 unx     4922 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/azure/appconfiguration/_sync_token.py
--rw-rw-r--  2.0 unx     1136 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/azure/appconfiguration/__init__.py
--rw-rw-r--  2.0 unx    12745 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/azure/appconfiguration/_models.py
--rw-rw-r--  2.0 unx      172 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/azure/appconfiguration/_version.py
--rw-rw-r--  2.0 unx      444 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/azure/appconfiguration/_constants.py
--rw-rw-r--  2.0 unx      881 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/azure/appconfiguration/_azure_appconfiguration_credential.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-07 19:28 azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-07 19:28 azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/models/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-07 19:28 azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/aio/
--rw-rw-r--  2.0 unx      674 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/_patch.py
--rw-rw-r--  2.0 unx    77450 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/_serialization.py
--rw-rw-r--  2.0 unx     1693 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/_vendor.py
--rw-rw-r--  2.0 unx      858 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/__init__.py
--rw-rw-r--  2.0 unx     2838 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/_configuration.py
--rw-rw-r--  2.0 unx     3661 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/_azure_app_configuration.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/operations/_patch.py
--rw-rw-r--  2.0 unx    82692 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/operations/_azure_app_configuration_operations.py
--rw-rw-r--  2.0 unx      852 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/operations/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/models/_patch.py
--rw-rw-r--  2.0 unx     2411 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/models/_azure_app_configuration_enums.py
--rw-rw-r--  2.0 unx     1700 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/models/__init__.py
--rw-rw-r--  2.0 unx     8111 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/models/_models_py3.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-07 19:28 azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/aio/operations/
--rw-rw-r--  2.0 unx      674 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/aio/_patch.py
--rw-rw-r--  2.0 unx     1042 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/aio/_vendor.py
--rw-rw-r--  2.0 unx      858 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/aio/__init__.py
--rw-rw-r--  2.0 unx     2804 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/aio/_configuration.py
--rw-rw-r--  2.0 unx     3703 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/aio/_azure_app_configuration.py
--rw-rw-r--  2.0 unx      674 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/aio/operations/_patch.py
--rw-rw-r--  2.0 unx    61626 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/aio/operations/_azure_app_configuration_operations.py
--rw-rw-r--  2.0 unx      852 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/aio/operations/__init__.py
--rw-rw-r--  2.0 unx     4275 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/azure/appconfiguration/aio/_sync_token_async.py
--rw-rw-r--  2.0 unx      592 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/azure/appconfiguration/aio/__init__.py
--rw-rw-r--  2.0 unx    25164 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/azure/appconfiguration/aio/_azure_configuration_client_async.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Feb-07 19:28 azure-appconfiguration-1.4.0b1/tests/perfstress_tests/
--rw-rw-r--  2.0 unx    37828 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/tests/test_azure_appconfiguration_client_aad_async.py
--rw-rw-r--  2.0 unx     2279 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/tests/preparers.py
--rw-rw-r--  2.0 unx     5653 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/tests/test_consistency.py
--rw-rw-r--  2.0 unx     3667 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/tests/testcase.py
--rw-rw-r--  2.0 unx    40549 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/tests/test_azure_appconfiguration_client.py
--rw-rw-r--  2.0 unx    34134 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/tests/test_azure_appconfiguration_client_aad.py
--rw-rw-r--  2.0 unx     2032 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/tests/conftest.py
--rw-rw-r--  2.0 unx     1369 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/tests/async_preparers.py
--rw-rw-r--  2.0 unx     4658 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/tests/test_sync_token_policy.py
--rw-rw-r--  2.0 unx    44783 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/tests/test_azure_appconfiguration_client_async.py
--rw-rw-r--  2.0 unx      862 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/tests/consts.py
--rw-rw-r--  2.0 unx     2439 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/tests/asynctestcase.py
--rw-rw-r--  2.0 unx     1609 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/tests/perfstress_tests/get.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/tests/perfstress_tests/__init__.py
--rw-rw-r--  2.0 unx     1681 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/tests/perfstress_tests/set.py
--rw-rw-r--  2.0 unx     2263 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/samples/conditional_operation_sample.py
--rw-rw-r--  2.0 unx     1717 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/samples/hello_world_sample_async.py
--rw-rw-r--  2.0 unx     1482 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/samples/list_revision_sample.py
--rw-rw-r--  2.0 unx     2076 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/samples/hello_world_advanced_sample_async.py
--rw-rw-r--  2.0 unx     1911 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/samples/read_only_sample_async.py
--rw-rw-r--  2.0 unx     1968 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/samples/hello_world_advanced_sample.py
--rw-rw-r--  2.0 unx     1700 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/samples/README.md
--rw-rw-r--  2.0 unx     1590 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/samples/list_revision_sample_async.py
--rw-rw-r--  2.0 unx     1470 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/samples/sync_token_samples_async.py
--rw-rw-r--  2.0 unx     2383 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/samples/conditional_operation_sample_async.py
--rw-rw-r--  2.0 unx     1408 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/samples/sync_token_samples.py
--rw-rw-r--  2.0 unx     1075 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/samples/util.py
--rw-rw-r--  2.0 unx     1615 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/samples/hello_world_sample.py
--rw-rw-r--  2.0 unx     1803 b- defN 23-Feb-07 19:26 azure-appconfiguration-1.4.0b1/samples/read_only_sample.py
--rw-rw-r--  2.0 unx        1 b- defN 23-Feb-07 19:28 azure-appconfiguration-1.4.0b1/azure_appconfiguration.egg-info/not-zip-safe
--rw-rw-r--  2.0 unx        1 b- defN 23-Feb-07 19:28 azure-appconfiguration-1.4.0b1/azure_appconfiguration.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx    17683 b- defN 23-Feb-07 19:28 azure-appconfiguration-1.4.0b1/azure_appconfiguration.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx        6 b- defN 23-Feb-07 19:28 azure-appconfiguration-1.4.0b1/azure_appconfiguration.egg-info/top_level.txt
--rw-rw-r--  2.0 unx     3154 b- defN 23-Feb-07 19:28 azure-appconfiguration-1.4.0b1/azure_appconfiguration.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx       41 b- defN 23-Feb-07 19:28 azure-appconfiguration-1.4.0b1/azure_appconfiguration.egg-info/requires.txt
-92 files, 606348 bytes uncompressed, 106989 bytes compressed:  82.4%
+Zip file size: 147926 bytes, number of entries: 96
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/tests/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/azure/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/azure_appconfiguration.egg-info/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/samples/
+-rw-rw-r--  2.0 unx     2482 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/setup.py
+-rw-rw-r--  2.0 unx      188 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/MANIFEST.in
+-rw-rw-r--  2.0 unx     1073 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/LICENSE
+-rw-rw-r--  2.0 unx    18279 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/README.md
+-rw-rw-r--  2.0 unx       38 b- defN 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/setup.cfg
+-rw-rw-r--  2.0 unx     4294 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/TROUBLESHOOTING.md
+-rw-rw-r--  2.0 unx       59 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/pyproject.toml
+-rw-rw-r--  2.0 unx    22915 b- defN 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/PKG-INFO
+-rw-rw-r--  2.0 unx     3724 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/CHANGELOG.md
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/tests/perfstress_tests/
+-rw-rw-r--  2.0 unx    33084 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/tests/test_azure_appconfiguration_client_aad.py
+-rw-rw-r--  2.0 unx     4383 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/tests/testcase.py
+-rw-rw-r--  2.0 unx     2029 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/tests/conftest.py
+-rw-rw-r--  2.0 unx     4662 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/tests/test_sync_token_policy.py
+-rw-rw-r--  2.0 unx     2207 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/tests/asynctestcase.py
+-rw-rw-r--  2.0 unx    42558 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/tests/test_azure_appconfiguration_client.py
+-rw-rw-r--  2.0 unx     2283 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/tests/preparers.py
+-rw-rw-r--  2.0 unx    37229 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/tests/test_azure_appconfiguration_client_aad_async.py
+-rw-rw-r--  2.0 unx     4923 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/tests/test_consistency.py
+-rw-rw-r--  2.0 unx      863 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/tests/consts.py
+-rw-rw-r--  2.0 unx    47189 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/tests/test_azure_appconfiguration_client_async.py
+-rw-rw-r--  2.0 unx     1364 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/tests/async_preparers.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/tests/perfstress_tests/__init__.py
+-rw-rw-r--  2.0 unx     1609 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/tests/perfstress_tests/get.py
+-rw-rw-r--  2.0 unx     1681 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/tests/perfstress_tests/set.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/azure/appconfiguration/
+-rw-rw-r--  2.0 unx       81 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/azure/appconfiguration/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/
+-rw-rw-r--  2.0 unx    35741 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_azure_appconfiguration_client.py
+-rw-rw-r--  2.0 unx     1232 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/__init__.py
+-rw-rw-r--  2.0 unx     2472 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_utils.py
+-rw-rw-r--  2.0 unx    19911 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_models.py
+-rw-rw-r--  2.0 unx      859 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_azure_appconfiguration_credential.py
+-rw-rw-r--  2.0 unx      530 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_azure_appconfiguration_error.py
+-rw-rw-r--  2.0 unx      313 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_user_agent.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/py.typed
+-rw-rw-r--  2.0 unx      172 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_version.py
+-rw-rw-r--  2.0 unx      441 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_constants.py
+-rw-rw-r--  2.0 unx     3145 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_azure_appconfiguration_requests.py
+-rw-rw-r--  2.0 unx     5026 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_sync_token.py
+-rw-rw-r--  2.0 unx      595 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/aio/__init__.py
+-rw-rw-r--  2.0 unx    35061 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/aio/_azure_appconfiguration_client_async.py
+-rw-rw-r--  2.0 unx     4231 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/aio/_sync_token_async.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/models/
+-rw-rw-r--  2.0 unx    78836 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/_serialization.py
+-rw-rw-r--  2.0 unx      850 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/_patch.py
+-rw-rw-r--  2.0 unx     1828 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/_vendor.py
+-rw-rw-r--  2.0 unx     3786 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/_azure_app_configuration.py
+-rw-rw-r--  2.0 unx     2816 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/_configuration.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/operations/
+-rw-rw-r--  2.0 unx      850 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/_patch.py
+-rw-rw-r--  2.0 unx     1063 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/_vendor.py
+-rw-rw-r--  2.0 unx     3891 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/_azure_app_configuration.py
+-rw-rw-r--  2.0 unx     2826 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/_configuration.py
+-rw-rw-r--  2.0 unx      837 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx    99054 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/operations/_azure_app_configuration_operations.py
+-rw-rw-r--  2.0 unx      837 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/operations/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/operations/_patch.py
+-rw-rw-r--  2.0 unx   128662 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/operations/_azure_app_configuration_operations.py
+-rw-rw-r--  2.0 unx     1983 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/models/__init__.py
+-rw-rw-r--  2.0 unx     2180 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/models/_azure_app_configuration_enums.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/models/_patch.py
+-rw-rw-r--  2.0 unx    21674 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/models/_models_py3.py
+-rw-rw-r--  2.0 unx        6 b- defN 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/azure_appconfiguration.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/azure_appconfiguration.egg-info/not-zip-safe
+-rw-rw-r--  2.0 unx    22915 b- defN 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/azure_appconfiguration.egg-info/PKG-INFO
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/azure_appconfiguration.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx       41 b- defN 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/azure_appconfiguration.egg-info/requires.txt
+-rw-rw-r--  2.0 unx     3253 b- defN 23-Jul-11 20:36 azure-appconfiguration-1.5.0b1/azure_appconfiguration.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx     2409 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/samples/hello_world_advanced_sample.py
+-rw-rw-r--  2.0 unx     2912 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/samples/snapshot_samples.py
+-rw-rw-r--  2.0 unx     1530 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/samples/sync_token_samples.py
+-rw-rw-r--  2.0 unx     1949 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/samples/hello_world_sample.py
+-rw-rw-r--  2.0 unx     2512 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/samples/conditional_operation_sample_async.py
+-rw-rw-r--  2.0 unx     2017 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/samples/hello_world_sample_async.py
+-rw-rw-r--  2.0 unx     4498 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/samples/README.md
+-rw-rw-r--  2.0 unx     2062 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/samples/read_only_sample_async.py
+-rw-rw-r--  2.0 unx     1954 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/samples/read_only_sample.py
+-rw-rw-r--  2.0 unx     2313 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/samples/hello_world_advanced_sample_async.py
+-rw-rw-r--  2.0 unx     1769 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/samples/list_revision_sample_async.py
+-rw-rw-r--  2.0 unx     1309 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/samples/util.py
+-rw-rw-r--  2.0 unx     2356 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/samples/conditional_operation_sample.py
+-rw-rw-r--  2.0 unx     3086 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/samples/snapshot_samples_async.py
+-rw-rw-r--  2.0 unx     1661 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/samples/list_revision_sample.py
+-rw-rw-r--  2.0 unx     1591 b- defN 23-Jul-11 20:35 azure-appconfiguration-1.5.0b1/samples/sync_token_samples_async.py
+96 files, 766414 bytes uncompressed, 127612 bytes compressed:  83.3%
```

## zipnote {}

```diff
@@ -1,277 +1,289 @@
-Filename: azure-appconfiguration-1.4.0b1/
+Filename: azure-appconfiguration-1.5.0b1/
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/
+Filename: azure-appconfiguration-1.5.0b1/tests/
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/tests/
+Filename: azure-appconfiguration-1.5.0b1/azure/
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/samples/
+Filename: azure-appconfiguration-1.5.0b1/azure_appconfiguration.egg-info/
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure_appconfiguration.egg-info/
+Filename: azure-appconfiguration-1.5.0b1/samples/
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/setup.py
+Filename: azure-appconfiguration-1.5.0b1/setup.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/CHANGELOG.md
+Filename: azure-appconfiguration-1.5.0b1/MANIFEST.in
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/setup.cfg
+Filename: azure-appconfiguration-1.5.0b1/LICENSE
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/PKG-INFO
+Filename: azure-appconfiguration-1.5.0b1/README.md
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/README.md
+Filename: azure-appconfiguration-1.5.0b1/setup.cfg
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/MANIFEST.in
+Filename: azure-appconfiguration-1.5.0b1/TROUBLESHOOTING.md
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/LICENSE
+Filename: azure-appconfiguration-1.5.0b1/pyproject.toml
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/
+Filename: azure-appconfiguration-1.5.0b1/PKG-INFO
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/__init__.py
+Filename: azure-appconfiguration-1.5.0b1/CHANGELOG.md
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/
+Filename: azure-appconfiguration-1.5.0b1/tests/perfstress_tests/
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/aio/
+Filename: azure-appconfiguration-1.5.0b1/tests/test_azure_appconfiguration_client_aad.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/_azure_appconfiguration_requests.py
+Filename: azure-appconfiguration-1.5.0b1/tests/testcase.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/_utils.py
+Filename: azure-appconfiguration-1.5.0b1/tests/conftest.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/py.typed
+Filename: azure-appconfiguration-1.5.0b1/tests/test_sync_token_policy.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/_user_agent.py
+Filename: azure-appconfiguration-1.5.0b1/tests/asynctestcase.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/_azure_appconfiguration_error.py
+Filename: azure-appconfiguration-1.5.0b1/tests/test_azure_appconfiguration_client.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/_azure_appconfiguration_client.py
+Filename: azure-appconfiguration-1.5.0b1/tests/preparers.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/_sync_token.py
+Filename: azure-appconfiguration-1.5.0b1/tests/test_azure_appconfiguration_client_aad_async.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/__init__.py
+Filename: azure-appconfiguration-1.5.0b1/tests/test_consistency.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/_models.py
+Filename: azure-appconfiguration-1.5.0b1/tests/consts.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/_version.py
+Filename: azure-appconfiguration-1.5.0b1/tests/test_azure_appconfiguration_client_async.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/_constants.py
+Filename: azure-appconfiguration-1.5.0b1/tests/async_preparers.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/_azure_appconfiguration_credential.py
+Filename: azure-appconfiguration-1.5.0b1/tests/perfstress_tests/__init__.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/operations/
+Filename: azure-appconfiguration-1.5.0b1/tests/perfstress_tests/get.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/models/
+Filename: azure-appconfiguration-1.5.0b1/tests/perfstress_tests/set.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/aio/
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/_patch.py
+Filename: azure-appconfiguration-1.5.0b1/azure/__init__.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/_serialization.py
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/aio/
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/_vendor.py
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/__init__.py
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_azure_appconfiguration_client.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/_configuration.py
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/__init__.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/_azure_app_configuration.py
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_utils.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/operations/_patch.py
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_models.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/operations/_azure_app_configuration_operations.py
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_azure_appconfiguration_credential.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/operations/__init__.py
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_azure_appconfiguration_error.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/models/_patch.py
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_user_agent.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/models/_azure_app_configuration_enums.py
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/py.typed
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/models/__init__.py
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_version.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/models/_models_py3.py
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_constants.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/aio/operations/
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_azure_appconfiguration_requests.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/aio/_patch.py
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_sync_token.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/aio/_vendor.py
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/aio/__init__.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/aio/__init__.py
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/aio/_azure_appconfiguration_client_async.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/aio/_configuration.py
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/aio/_sync_token_async.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/aio/_azure_app_configuration.py
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/aio/operations/_patch.py
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/operations/
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/aio/operations/_azure_app_configuration_operations.py
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/models/
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/aio/operations/__init__.py
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/_serialization.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/aio/_sync_token_async.py
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/__init__.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/aio/__init__.py
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/_patch.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure/appconfiguration/aio/_azure_configuration_client_async.py
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/_vendor.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/tests/perfstress_tests/
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/_azure_app_configuration.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/tests/test_azure_appconfiguration_client_aad_async.py
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/_configuration.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/tests/preparers.py
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/operations/
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/tests/test_consistency.py
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/__init__.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/tests/testcase.py
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/_patch.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/tests/test_azure_appconfiguration_client.py
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/_vendor.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/tests/test_azure_appconfiguration_client_aad.py
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/_azure_app_configuration.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/tests/conftest.py
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/_configuration.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/tests/async_preparers.py
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/tests/test_sync_token_policy.py
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/tests/test_azure_appconfiguration_client_async.py
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/operations/_azure_app_configuration_operations.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/tests/consts.py
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/operations/__init__.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/tests/asynctestcase.py
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/operations/_patch.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/tests/perfstress_tests/get.py
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/operations/_azure_app_configuration_operations.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/tests/perfstress_tests/__init__.py
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/models/__init__.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/tests/perfstress_tests/set.py
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/models/_azure_app_configuration_enums.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/samples/conditional_operation_sample.py
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/models/_patch.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/samples/hello_world_sample_async.py
+Filename: azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/models/_models_py3.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/samples/list_revision_sample.py
+Filename: azure-appconfiguration-1.5.0b1/azure_appconfiguration.egg-info/top_level.txt
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/samples/hello_world_advanced_sample_async.py
+Filename: azure-appconfiguration-1.5.0b1/azure_appconfiguration.egg-info/not-zip-safe
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/samples/read_only_sample_async.py
+Filename: azure-appconfiguration-1.5.0b1/azure_appconfiguration.egg-info/PKG-INFO
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/samples/hello_world_advanced_sample.py
+Filename: azure-appconfiguration-1.5.0b1/azure_appconfiguration.egg-info/dependency_links.txt
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/samples/README.md
+Filename: azure-appconfiguration-1.5.0b1/azure_appconfiguration.egg-info/requires.txt
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/samples/list_revision_sample_async.py
+Filename: azure-appconfiguration-1.5.0b1/azure_appconfiguration.egg-info/SOURCES.txt
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/samples/sync_token_samples_async.py
+Filename: azure-appconfiguration-1.5.0b1/samples/hello_world_advanced_sample.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/samples/conditional_operation_sample_async.py
+Filename: azure-appconfiguration-1.5.0b1/samples/snapshot_samples.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/samples/sync_token_samples.py
+Filename: azure-appconfiguration-1.5.0b1/samples/sync_token_samples.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/samples/util.py
+Filename: azure-appconfiguration-1.5.0b1/samples/hello_world_sample.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/samples/hello_world_sample.py
+Filename: azure-appconfiguration-1.5.0b1/samples/conditional_operation_sample_async.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/samples/read_only_sample.py
+Filename: azure-appconfiguration-1.5.0b1/samples/hello_world_sample_async.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure_appconfiguration.egg-info/not-zip-safe
+Filename: azure-appconfiguration-1.5.0b1/samples/README.md
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure_appconfiguration.egg-info/dependency_links.txt
+Filename: azure-appconfiguration-1.5.0b1/samples/read_only_sample_async.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure_appconfiguration.egg-info/PKG-INFO
+Filename: azure-appconfiguration-1.5.0b1/samples/read_only_sample.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure_appconfiguration.egg-info/top_level.txt
+Filename: azure-appconfiguration-1.5.0b1/samples/hello_world_advanced_sample_async.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure_appconfiguration.egg-info/SOURCES.txt
+Filename: azure-appconfiguration-1.5.0b1/samples/list_revision_sample_async.py
 Comment: 
 
-Filename: azure-appconfiguration-1.4.0b1/azure_appconfiguration.egg-info/requires.txt
+Filename: azure-appconfiguration-1.5.0b1/samples/util.py
+Comment: 
+
+Filename: azure-appconfiguration-1.5.0b1/samples/conditional_operation_sample.py
+Comment: 
+
+Filename: azure-appconfiguration-1.5.0b1/samples/snapshot_samples_async.py
+Comment: 
+
+Filename: azure-appconfiguration-1.5.0b1/samples/list_revision_sample.py
+Comment: 
+
+Filename: azure-appconfiguration-1.5.0b1/samples/sync_token_samples_async.py
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-appconfiguration-1.4.0b1/setup.py` & `azure-appconfiguration-1.5.0b1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 
-import sys
 import re
 import os.path
 from io import open
 from setuptools import find_packages, setup
 
 # Change the PACKAGE_NAME only to change folder and different name
 PACKAGE_NAME = "azure-appconfiguration"
@@ -19,17 +18,15 @@
 # a-b-c => a/b/c
 package_folder_path = PACKAGE_NAME.replace("-", "/")
 # a-b-c => a.b.c
 namespace_name = PACKAGE_NAME.replace("-", ".")
 
 # Version extraction inspired from 'requests'
 with open(os.path.join(package_folder_path, "_version.py"), "r") as fd:
-    version = re.search(
-        r'^VERSION\s*=\s*[\'"]([^\'"]*)[\'"]', fd.read(), re.MULTILINE
-    ).group(1)
+    version = re.search(r'^VERSION\s*=\s*[\'"]([^\'"]*)[\'"]', fd.read(), re.MULTILINE).group(1)
 
 if not version:
     raise RuntimeError("Cannot find version information")
 
 with open("README.md", encoding="utf-8") as f:
     readme = f.read()
 with open("CHANGELOG.md", encoding="utf-8") as f:
@@ -38,16 +35,14 @@
 exclude_packages = [
     "tests",
     "tests.*",
     "samples",
     # Exclude packages that will be covered by PEP420 or nspkg
     "azure",
 ]
-if sys.version_info < (3, 5, 3):
-    exclude_packages.extend(["*.aio", "*.aio.*"])
 
 setup(
     name=PACKAGE_NAME,
     version=version,
     include_package_data=True,
     description="Microsoft {} Library for Python".format(PACKAGE_PPRINT_NAME),
     long_description=readme + "\n\n" + changelog,
@@ -61,17 +56,18 @@
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
     ],
     zip_safe=False,
     packages=find_packages(exclude=exclude_packages),
     python_requires=">=3.7",
     install_requires=[
-        "azure-core<2.0.0,>=1.24.0",
+        "azure-core<2.0.0,>=1.25.0",
         "isodate>=0.6.0",
     ],
 )
```

## Comparing `azure-appconfiguration-1.4.0b1/CHANGELOG.md` & `azure-appconfiguration-1.5.0b1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,22 @@
 # Release History
 
-## 1.4.0b1 (2022-02-07)
+## 1.5.0b1 (2023-07-11)
+
+### Features Added
+- Added support for `Snapshot` CRUD operations.
+
+### Bugs Fixed
+- Fixed async `update_sync_token` to use async/await keywords
+
+### Other Changes
+- Bumped minimum dependency on `azure-core` to `>=1.25.0`.
+- Updated the default `api_version` to "2022-11-01-preview".
+
+## 1.4.0 (2022-02-13)
 
 ### Other Changes
 - Python 2.7 is no longer supported. Please use Python version 3.7 or later.
 - Bumped minimum dependency on `azure-core` to `>=1.24.0`.
 - Changed the default async transport from `AsyncioRequestsTransport` to the one used in current `azure-core` (`AioHttpTransport`). ([#26427](https://github.com/Azure/azure-sdk-for-python/issues/26427))
 - Dropped `msrest` requirement.
 - Added dependency `isodate` with version range `>=0.6.0`.
```

## Comparing `azure-appconfiguration-1.4.0b1/LICENSE` & `azure-appconfiguration-1.5.0b1/LICENSE`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.4.0b1/azure/appconfiguration/_azure_appconfiguration_requests.py` & `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_azure_appconfiguration_requests.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,48 +23,41 @@
 
         # Get the path and query from url, which looks like https://host/path/query
         query_url = str(request.http_request.url[len(self._credentials.host) + 8 :])
         # Need URL() to get a correct encoded key value, from "%2A" to "*", when transport is in type AioHttpTransport.
         # There's a similar scenario in azure-storage-blob, the check logic is from there.
         try:
             from yarl import URL
-            from azure.core.pipeline.transport import AioHttpTransport
-            if isinstance(request.context.transport, AioHttpTransport) or \
-                isinstance(getattr(request.context.transport, "_transport", None), AioHttpTransport) or \
-                isinstance(getattr(getattr(request.context.transport, "_transport", None), "_transport", None),
-                            AioHttpTransport):
+            from azure.core.pipeline.transport import (
+                AioHttpTransport,
+            )  # pylint:disable=non-abstract-transport-import,no-name-in-module
+
+            if (
+                isinstance(request.context.transport, AioHttpTransport)
+                or isinstance(getattr(request.context.transport, "_transport", None), AioHttpTransport)
+                or isinstance(
+                    getattr(getattr(request.context.transport, "_transport", None), "_transport", None),
+                    AioHttpTransport,
+                )
+            ):
                 query_url = str(URL(query_url))
         except (ImportError, TypeError):
             pass
         signed_headers = "x-ms-date;host;x-ms-content-sha256"
 
         utc_now = get_current_utc_time()
         if request.http_request.body is None:
             request.http_request.body = ""
-        content_digest = hashlib.sha256(
-            (request.http_request.body.encode("utf-8"))
-        ).digest()
+        content_digest = hashlib.sha256((request.http_request.body.encode("utf-8"))).digest()
         content_hash = base64.b64encode(content_digest).decode("utf-8")
 
-        string_to_sign = (
-            verb
-            + "\n"
-            + query_url
-            + "\n"
-            + utc_now
-            + ";"
-            + self._credentials.host
-            + ";"
-            + content_hash
-        )
+        string_to_sign = verb + "\n" + query_url + "\n" + utc_now + ";" + self._credentials.host + ";" + content_hash
 
         decoded_secret = base64.b64decode(self._credentials.secret)
-        digest = hmac.new(
-            decoded_secret, string_to_sign.encode("utf-8"), hashlib.sha256
-        ).digest()
+        digest = hmac.new(decoded_secret, string_to_sign.encode("utf-8"), hashlib.sha256).digest()
         signature = base64.b64encode(digest).decode("utf-8")
 
         signature_header = {
             "x-ms-date": utc_now,
             "x-ms-content-sha256": content_hash,
             "Authorization": "HMAC-SHA256 Credential="
             + self._credentials.credential
```

## Comparing `azure-appconfiguration-1.4.0b1/azure/appconfiguration/_utils.py` & `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_utils.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.4.0b1/azure/appconfiguration/_azure_appconfiguration_error.py` & `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_azure_appconfiguration_error.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.4.0b1/azure/appconfiguration/_azure_appconfiguration_client.py` & `azure-appconfiguration-1.5.0b1/azure/appconfiguration/aio/_azure_appconfiguration_client_async.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,412 +1,412 @@
 # ------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # -------------------------------------------------------------------------
 import binascii
-from typing import Optional, Any, Union, Mapping
-from requests.structures import CaseInsensitiveDict
+import sys
+from typing import Any, Dict, List, Mapping, Optional, Union, cast
 from azure.core import MatchConditions
-from azure.core.paging import ItemPaged
-from azure.core.credentials import TokenCredential
-from azure.core.pipeline import Pipeline
+from azure.core.async_paging import AsyncItemPaged
+from azure.core.credentials_async import AsyncTokenCredential
 from azure.core.pipeline.policies import (
     UserAgentPolicy,
-    DistributedTracingPolicy,
-    HttpLoggingPolicy,
-    BearerTokenCredentialPolicy,
-    ContentDecodePolicy,
+    AsyncBearerTokenCredentialPolicy,
 )
+from azure.core.polling import AsyncLROPoller
 from azure.core.tracing.decorator import distributed_trace
-from azure.core.pipeline.transport import RequestsTransport
+from azure.core.tracing.decorator_async import distributed_trace_async
 from azure.core.exceptions import (
     HttpResponseError,
     ClientAuthenticationError,
     ResourceExistsError,
-    ResourceNotFoundError,
     ResourceModifiedError,
+    ResourceNotFoundError,
     ResourceNotModifiedError,
 )
-from ._azure_appconfiguration_error import ResourceReadOnlyError
-from ._generated import AzureAppConfiguration
-from ._generated._configuration import AzureAppConfigurationConfiguration
-from ._models import ConfigurationSetting
-from ._azure_appconfiguration_requests import AppConfigRequestsCredentialsPolicy
-from ._azure_appconfiguration_credential import AppConfigConnectionStringCredential
-from ._utils import (
+from azure.core.utils import CaseInsensitiveDict
+from ._sync_token_async import AsyncSyncTokenPolicy
+from .._azure_appconfiguration_error import ResourceReadOnlyError
+from .._azure_appconfiguration_requests import AppConfigRequestsCredentialsPolicy
+from .._azure_appconfiguration_credential import AppConfigConnectionStringCredential
+from .._generated.aio import AzureAppConfiguration
+from .._generated.models import SnapshotStatus, SnapshotUpdateParameters
+from .._models import ConfigurationSetting, ConfigurationSettingFilter, Snapshot
+from .._user_agent import USER_AGENT
+from .._utils import (
     get_endpoint_from_connection_string,
     prep_if_match,
     prep_if_none_match,
 )
-from ._sync_token import SyncTokenPolicy
-from ._user_agent import USER_AGENT
+
+if sys.version_info >= (3, 8):
+    from typing import Literal  # pylint: disable=no-name-in-module, ungrouped-imports
+else:
+    from typing_extensions import Literal  # type: ignore  # pylint: disable=ungrouped-imports
 
 
 class AzureAppConfigurationClient:
     """Represents a client that calls restful API of Azure App Configuration service.
 
-    :param str base_url: Base url of the service.
-    :param credential: An object which can provide secrets for the app configuration service
-    :type credential: :class:`~azure.appconfiguration.AppConfigConnectionStringCredential`
-        or :class:`~azure.core.credentials.TokenCredential`
-    :keyword api_version: Api Version. Default value is "1.0". Note that overriding this default
-        value may result in unsupported behavior.
-    :paramtype api_version: str
+        :param str base_url: Base url of the service.
+        :param credential: An object which can provide secrets for the app configuration service
+        :type credential: ~azure.appconfiguration.AppConfigConnectionStringCredential
+            or ~azure.core.credentials_async.AsyncTokenCredential
+        :keyword api_version: Api Version. Default value is "2022-11-01-preview". Note that overriding this default
+            value may result in unsupported behavior.
+        :paramtype api_version: str
+
+    This is the async version of :class:`~azure.appconfiguration.AzureAppConfigurationClient`
 
     """
 
     # pylint:disable=protected-access
-    def __init__(
-        self, base_url: str, credential: Union[AppConfigConnectionStringCredential, TokenCredential], **kwargs: Any
-    ) -> None:
+
+    def __init__(self, base_url: str, credential: AsyncTokenCredential, **kwargs) -> None:
         try:
             if not base_url.lower().startswith("http"):
                 base_url = "https://" + base_url
-        except AttributeError:
-            raise ValueError("Base URL must be a string.")
+        except AttributeError as exc:
+            raise ValueError("Base URL must be a string.") from exc
 
         if not credential:
             raise ValueError("Missing credential")
 
-        self._credential_scopes = base_url.strip("/") + "/.default"
+        credential_scopes = base_url.strip("/") + "/.default"
 
-        self._config = AzureAppConfigurationConfiguration(
-            base_url, credential_scopes=self._credential_scopes, **kwargs
-        )
-        self._config.user_agent_policy = UserAgentPolicy(
-            base_user_agent=USER_AGENT, **kwargs
-        )
-        self._sync_token_policy = SyncTokenPolicy()
+        user_agent_policy = UserAgentPolicy(base_user_agent=USER_AGENT, **kwargs)
 
-        pipeline = kwargs.get("pipeline")
+        self._sync_token_policy = AsyncSyncTokenPolicy()
 
-        if pipeline is None:
-            aad_mode = not isinstance(credential, AppConfigConnectionStringCredential)
-            pipeline = self._create_appconfig_pipeline(
-                credential=credential, aad_mode=aad_mode, base_url=base_url, **kwargs
-            )
+        aad_mode = not isinstance(credential, AppConfigConnectionStringCredential)
+        if aad_mode:
+            if hasattr(credential, "get_token"):
+                credential_policy = AsyncBearerTokenCredentialPolicy(
+                    credential,  # type: ignore
+                    credential_scopes,
+                )
+            else:
+                raise TypeError(
+                    "Please provide an instance from azure-identity or a class that implements the 'get_token' protocol"
+                )
+        else:
+            credential_policy = AppConfigRequestsCredentialsPolicy(credential)  # type: ignore
 
         self._impl = AzureAppConfiguration(
-            base_url, pipeline=pipeline, credential_scopes=self._credential_scopes
+            base_url,
+            credential_scopes=credential_scopes,
+            authentication_policy=credential_policy,
+            user_agent_policy=user_agent_policy,
+            per_call_policies=self._sync_token_policy,
+            **kwargs
         )
 
     @classmethod
-    def from_connection_string(cls, connection_string: str, **kwargs: Any) -> "AzureAppConfigurationClient":
+    def from_connection_string(cls, connection_string: str, **kwargs) -> "AzureAppConfigurationClient":
         """Create AzureAppConfigurationClient from a Connection String.
+        This is the async version of :class:`~azure.appconfiguration.AzureAppConfigurationClient`
 
         :param str connection_string: Connection String
             (one of the access keys of the Azure App Configuration resource)
             used to access the Azure App Configuration.
         :return: An AzureAppConfigurationClient authenticated with the connection string
-        :rtype: :class:`~azure.appconfiguration.AzureAppConfigurationClient`
+        :rtype: ~azure.appconfiguration.AzureAppConfigurationClient
 
         Example
 
         .. code-block:: python
 
-            from azure.appconfiguration import AzureAppConfigurationClient
+            from azure.appconfiguration.aio import AzureAppConfigurationClient
             connection_str = "<my connection string>"
-            client = AzureAppConfigurationClient.from_connection_string(connection_str)
+            async_client = AzureAppConfigurationClient.from_connection_string(connection_str)
         """
         base_url = "https://" + get_endpoint_from_connection_string(connection_string)
         return cls(
-            credential=AppConfigConnectionStringCredential(connection_string),
+            credential=AppConfigConnectionStringCredential(connection_string),  # type: ignore
             base_url=base_url,
             **kwargs
         )
 
-    def _create_appconfig_pipeline(self, credential, base_url=None, aad_mode=False, **kwargs):
-        transport = kwargs.get("transport")
-        policies = kwargs.get("policies")
-
-        if policies is None:  # [] is a valid policy list
-            if aad_mode:
-                scope = base_url.strip("/") + "/.default"
-                if hasattr(credential, "get_token"):
-                    credential_policy = BearerTokenCredentialPolicy(credential, scope)
-                else:
-                    raise TypeError(
-                        "Please provide an instance from azure-identity "
-                        "or a class that implement the 'get_token protocol"
-                    )
-            else:
-                credential_policy = AppConfigRequestsCredentialsPolicy(credential)
-            policies = [
-                self._config.headers_policy,
-                self._config.user_agent_policy,
-                self._config.retry_policy,
-                self._sync_token_policy,
-                credential_policy,
-                self._config.logging_policy,  # HTTP request/response log
-                DistributedTracingPolicy(**kwargs),
-                HttpLoggingPolicy(**kwargs),
-                ContentDecodePolicy(**kwargs),
-            ]
-
-        if not transport:
-            transport = RequestsTransport(**kwargs)
-
-        return Pipeline(transport, policies)
-
     @distributed_trace
     def list_configuration_settings(
-        self, key_filter: Optional[str] = None, label_filter: Optional[str] = None, **kwargs: Any
-    ) -> ItemPaged[ConfigurationSetting]:
+        self, key_filter: Optional[str] = None, label_filter: Optional[str] = None, **kwargs
+    ) -> AsyncItemPaged[ConfigurationSetting]:
+
         """List the configuration settings stored in the configuration service, optionally filtered by
-        label and accept_datetime
+        key, label and accept_datetime.
 
         :param key_filter: filter results based on their keys. '*' can be
-         used as wildcard in the beginning or end of the filter
+            used as wildcard in the beginning or end of the filter
         :type key_filter: str
         :param label_filter: filter results based on their label. '*' can be
-         used as wildcard in the beginning or end of the filter
+            used as wildcard in the beginning or end of the filter
         :type label_filter: str
-        :keyword datetime accept_datetime: filter out ConfigurationSetting created after this datetime
-        :keyword List[str] fields: specify which fields to include in the results. Leave None to include all fields
-        :return: An iterator of :class:`ConfigurationSetting`
-        :rtype: ~azure.core.paging.ItemPaged[ConfigurationSetting]
-        :raises: :class:`HttpResponseError`, :class:`ClientAuthenticationError`
+        :keyword str accept_datetime: retrieve ConfigurationSetting existed at this datetime
+        :keyword list[str] fields: specify which fields to include in the results. Leave None to include all fields
+        :return: An iterator of :class:`~azure.appconfiguration.ConfigurationSetting`
+        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.appconfiguration.ConfigurationSetting]
+        :raises: :class:`~azure.core.exceptions.HttpResponseError`, \
+            :class:`~azure.core.exceptions.ClientAuthenticationError`
 
         Example
 
         .. code-block:: python
 
             from datetime import datetime, timedelta
 
-            accept_datetime = datetime.today() + timedelta(days=-1)
+            accept_datetime = datetime.utcnow() + timedelta(days=-1)
 
-            all_listed = client.list_configuration_settings()
-            for item in all_listed:
+            all_listed = async_client.list_configuration_settings()
+            async for item in all_listed:
                 pass  # do something
 
-            filtered_listed = client.list_configuration_settings(
-                label_filter="Labe*", key_filter="Ke*", accept_datetime=accept_datetime
+            filtered_listed = async_client.list_configuration_settings(
+                label_filter="Labe*", key_filter="Ke*", accept_datetime=str(accept_datetime)
             )
-            for item in filtered_listed:
+            async for item in filtered_listed:
                 pass  # do something
         """
         select = kwargs.pop("fields", None)
         if select:
             select = ["locked" if x == "read_only" else x for x in select]
         error_map = {401: ClientAuthenticationError}
 
         try:
             return self._impl.get_key_values(  # type: ignore
                 label=label_filter,
                 key=key_filter,
                 select=select,
-                cls=lambda objs: [
-                    ConfigurationSetting._from_generated(x) for x in objs
-                ],
+                cls=lambda objs: [ConfigurationSetting._from_generated(x) for x in objs],
                 error_map=error_map,
                 **kwargs
             )
         except HttpResponseError as error:
             e = error_map[error.status_code]
-            raise e(message=error.message, response=error.response)
-        except binascii.Error:
-            raise binascii.Error("Connection string secret has incorrect padding")
+            raise e(message=error.message, response=error.response) from error
+        except binascii.Error as exc:
+            raise binascii.Error("Connection string secret has incorrect padding") from exc
 
-    @distributed_trace
-    def get_configuration_setting(
+    @distributed_trace_async
+    async def get_configuration_setting(
         self,
         key: str,
         label: Optional[str] = None,
         etag: Optional[str] = "*",
-        match_condition: Optional[MatchConditions] = MatchConditions.Unconditionally,
-        **kwargs: Any
+        match_condition: MatchConditions = MatchConditions.Unconditionally,
+        **kwargs
     ) -> Union[None, ConfigurationSetting]:
+
         """Get the matched ConfigurationSetting from Azure App Configuration service
 
         :param key: key of the ConfigurationSetting
         :type key: str
         :param label: label used to identify the ConfigurationSetting. Default is `None`.
         :type label: str
         :param etag: check if the ConfigurationSetting is changed. Set None to skip checking etag
         :type etag: str or None
         :param match_condition: The match condition to use upon the etag
-        :type match_condition: :class:`~azure.core.MatchConditions`
-        :keyword datetime accept_datetime: the retrieved ConfigurationSetting that created no later than this datetime
+        :type match_condition: ~azure.core.MatchConditions
+        :keyword str accept_datetime: retrieve ConfigurationSetting existed at this datetime
         :return: The matched ConfigurationSetting object
-        :rtype: :class:`~azure.appconfiguration.ConfigurationSetting`
-        :raises: :class:`HttpResponseError`, :class:`ClientAuthenticationError`, \
-        :class:`ResourceNotFoundError`, :class:`ResourceModifiedError`, :class:`ResourceExistsError`
+        :rtype: ~azure.appconfiguration.ConfigurationSetting
+        :raises: :class:`~azure.core.exceptions.HttpResponseError`, \
+            :class:`~azure.core.exceptions.ClientAuthenticationError`, \
+            :class:`~azure.core.exceptions.ResourceNotFoundError`, \
+            :class:`~azure.core.exceptions.ResourceModifiedError`, \
+            :class:`~azure.core.exceptions.ResourceExistsError`
 
         Example
 
         .. code-block:: python
 
-            fetched_config_setting = client.get_configuration_setting(
+            # in async function
+            fetched_config_setting = await async_client.get_configuration_setting(
                 key="MyKey", label="MyLabel"
             )
         """
         error_map = {401: ClientAuthenticationError, 404: ResourceNotFoundError}
         if match_condition == MatchConditions.IfNotModified:
             error_map[412] = ResourceModifiedError
         if match_condition == MatchConditions.IfModified:
             error_map[304] = ResourceNotModifiedError
         if match_condition == MatchConditions.IfPresent:
             error_map[412] = ResourceNotFoundError
         if match_condition == MatchConditions.IfMissing:
             error_map[412] = ResourceExistsError
 
         try:
-            key_value = self._impl.get_key_value(
+            key_value = await self._impl.get_key_value(
                 key=key,
                 label=label,
                 if_match=prep_if_match(etag, match_condition),
                 if_none_match=prep_if_none_match(etag, match_condition),
                 error_map=error_map,
                 **kwargs
             )
             return ConfigurationSetting._from_generated(key_value)
         except ResourceNotModifiedError:
             return None
         except HttpResponseError as error:
             e = error_map[error.status_code]
-            raise e(message=error.message, response=error.response)
-        except binascii.Error:
-            raise binascii.Error("Connection string secret has incorrect padding")
-
-    @distributed_trace
-    def add_configuration_setting(
-        self, configuration_setting: ConfigurationSetting, **kwargs: Any
+            raise e(message=error.message, response=error.response) from error
+        except binascii.Error as exc:
+            raise binascii.Error("Connection string secret has incorrect padding") from exc
+
+    @distributed_trace_async
+    async def add_configuration_setting(
+        self, configuration_setting: ConfigurationSetting, **kwargs
     ) -> ConfigurationSetting:
+
         """Add a ConfigurationSetting instance into the Azure App Configuration service.
 
         :param configuration_setting: the ConfigurationSetting object to be added
-        :type configuration_setting: :class:`~azure.appconfiguration.ConfigurationSetting`
+        :type configuration_setting: ~azure.appconfiguration.ConfigurationSetting
         :return: The ConfigurationSetting object returned from the App Configuration service
-        :rtype: :class:`~azure.appconfiguration.ConfigurationSetting`
-        :raises: :class:`HttpResponseError`, :class:`ClientAuthenticationError`, :class:`ResourceExistsError`
+        :rtype: ~azure.appconfiguration.ConfigurationSetting
+        :raises: :class:`~azure.core.exceptions.HttpResponseError`, \
+            :class:`~azure.core.exceptions.ClientAuthenticationError`, \
+            :class:`~azure.core.exceptions.ResourceExistsError`
 
         Example
 
         .. code-block:: python
 
+            # in async function
             config_setting = ConfigurationSetting(
                 key="MyKey",
                 label="MyLabel",
                 value="my value",
                 content_type="my content type",
                 tags={"my tag": "my tag value"}
             )
-            added_config_setting = client.add_configuration_setting(config_setting)
+            added_config_setting = await async_client.add_configuration_setting(config_setting)
         """
         key_value = configuration_setting._to_generated()
         custom_headers = CaseInsensitiveDict(kwargs.get("headers"))  # type: Mapping[str, Any]
         error_map = {401: ClientAuthenticationError, 412: ResourceExistsError}
+
         try:
-            key_value_added = self._impl.put_key_value(
+            key_value_added = await self._impl.put_key_value(
                 entity=key_value,
                 key=key_value.key,  # type: ignore
                 label=key_value.label,
                 if_none_match="*",
                 headers=custom_headers,
                 error_map=error_map,
             )
             return ConfigurationSetting._from_generated(key_value_added)
         except HttpResponseError as error:
             e = error_map[error.status_code]
-            raise e(message=error.message, response=error.response)
-        except binascii.Error:
-            raise binascii.Error("Connection string secret has incorrect padding")
+            raise e(message=error.message, response=error.response) from error
+        except binascii.Error as exc:
+            raise binascii.Error("Connection string secret has incorrect padding") from exc
 
-    @distributed_trace
-    def set_configuration_setting(
+    @distributed_trace_async
+    async def set_configuration_setting(
         self,
         configuration_setting: ConfigurationSetting,
-        match_condition: Optional[MatchConditions] = MatchConditions.Unconditionally,
-        **kwargs: Any
+        match_condition: MatchConditions = MatchConditions.Unconditionally,
+        **kwargs
     ) -> ConfigurationSetting:
+
         """Add or update a ConfigurationSetting.
         If the configuration setting identified by key and label does not exist, this is a create.
         Otherwise this is an update.
 
         :param configuration_setting: the ConfigurationSetting to be added (if not exists) \
-        or updated (if exists) to the service
-        :type configuration_setting: :class:`ConfigurationSetting`
+            or updated (if exists) to the service
+        :type configuration_setting: ~azure.appconfiguration.ConfigurationSetting
         :param match_condition: The match condition to use upon the etag
-        :type match_condition: :class:`~azure.core.MatchConditions`
+        :type match_condition: ~azure.core.MatchConditions
         :keyword str etag: check if the ConfigurationSetting is changed. Set None to skip checking etag
         :return: The ConfigurationSetting returned from the service
-        :rtype: :class:`~azure.appconfiguration.ConfigurationSetting`
-        :raises: :class:`HttpResponseError`, :class:`ClientAuthenticationError`, \
-        :class:`ResourceReadOnlyError`, :class:`ResourceModifiedError`, :class:`ResourceNotModifiedError`, \
-        :class:`ResourceNotFoundError`, :class:`ResourceExistsError`
+        :rtype: ~azure.appconfiguration.ConfigurationSetting
+        :raises: :class:`~azure.core.exceptions.HttpResponseError`, \
+            :class:`~azure.core.exceptions.ClientAuthenticationError`, \
+            :class:`~azure.core.exceptions.ResourceReadOnlyError`, \
+            :class:`~azure.core.exceptions.ResourceModifiedError`, \
+            :class:`~azure.core.exceptions.ResourceNotModifiedError`, \
+            :class:`~azure.core.exceptions.ResourceNotFoundError`, \
+            :class:`~azure.core.exceptions.ResourceExistsError`
 
         Example
 
         .. code-block:: python
 
+            # in async function
             config_setting = ConfigurationSetting(
                 key="MyKey",
                 label="MyLabel",
                 value="my set value",
                 content_type="my set content type",
                 tags={"my set tag": "my set tag value"}
             )
-            returned_config_setting = client.set_configuration_setting(config_setting)
+            returned_config_setting = await async_client.set_configuration_setting(config_setting)
         """
+        etag = kwargs.get("etag", configuration_setting.etag)
+
         key_value = configuration_setting._to_generated()
         custom_headers = CaseInsensitiveDict(kwargs.get("headers"))  # type: Mapping[str, Any]
         error_map = {401: ClientAuthenticationError, 409: ResourceReadOnlyError}
         if match_condition == MatchConditions.IfNotModified:
             error_map[412] = ResourceModifiedError
         if match_condition == MatchConditions.IfModified:
             error_map[412] = ResourceNotModifiedError
         if match_condition == MatchConditions.IfPresent:
             error_map[412] = ResourceNotFoundError
         if match_condition == MatchConditions.IfMissing:
             error_map[412] = ResourceExistsError
 
         try:
-            key_value_set = self._impl.put_key_value(
+            key_value_set = await self._impl.put_key_value(
                 entity=key_value,
                 key=key_value.key,  # type: ignore
                 label=key_value.label,
                 if_match=prep_if_match(configuration_setting.etag, match_condition),
-                if_none_match=prep_if_none_match(
-                    configuration_setting.etag, match_condition
-                ),
+                if_none_match=prep_if_none_match(etag, match_condition),
                 headers=custom_headers,
                 error_map=error_map,
             )
             return ConfigurationSetting._from_generated(key_value_set)
         except HttpResponseError as error:
             e = error_map[error.status_code]
-            raise e(message=error.message, response=error.response)
-        except binascii.Error:
-            raise binascii.Error("Connection string secret has incorrect padding")
-
-    @distributed_trace
-    def delete_configuration_setting(
-        self, key: str, label: Optional[str] = None, **kwargs: Any
+            raise e(message=error.message, response=error.response) from error
+        except binascii.Error as exc:
+            raise binascii.Error("Connection string secret has incorrect padding") from exc
+
+    @distributed_trace_async
+    async def delete_configuration_setting(
+        self, key: str, label: Optional[str] = None, **kwargs
     ) -> ConfigurationSetting:
         """Delete a ConfigurationSetting if it exists
 
         :param key: key used to identify the ConfigurationSetting
         :type key: str
         :param label: label used to identify the ConfigurationSetting. Default is `None`.
         :type label: str
         :keyword str etag: check if the ConfigurationSetting is changed. Set None to skip checking etag
         :keyword match_condition: The match condition to use upon the etag
-        :paramtype match_condition: :class:`~azure.core.MatchConditions`
+        :paramtype match_condition: ~azure.core.MatchConditions
         :return: The deleted ConfigurationSetting returned from the service, or None if it doesn't exist.
-        :rtype: :class:`~azure.appconfiguration.ConfigurationSetting`
-        :raises: :class:`HttpResponseError`, :class:`ClientAuthenticationError`, \
-        :class:`ResourceReadOnlyError`, :class:`ResourceModifiedError`, :class:`ResourceNotModifiedError`, \
-        :class:`ResourceNotFoundError`, :class:`ResourceExistsError`
+        :rtype: ~azure.appconfiguration.ConfigurationSetting
+        :raises: :class:`~azure.core.exceptions.HttpResponseError`, \
+            :class:`~azure.core.exceptions.ClientAuthenticationError`, \
+            :class:`~azure.core.exceptions.ResourceReadOnlyError`, \
+            :class:`~azure.core.exceptions.ResourceModifiedError`, \
+            :class:`~azure.core.exceptions.ResourceNotModifiedError`, \
+            :class:`~azure.core.exceptions.ResourceNotFoundError`, \
+            :class:`~azure.core.exceptions.ResourceExistsError`
 
         Example
 
         .. code-block:: python
 
-            deleted_config_setting = client.delete_configuration_setting(
+            # in async function
+            deleted_config_setting = await async_client.delete_configuration_setting(
                 key="MyKey", label="MyLabel"
             )
         """
         etag = kwargs.pop("etag", None)
         match_condition = kwargs.pop("match_condition", MatchConditions.Unconditionally)
         custom_headers = CaseInsensitiveDict(kwargs.get("headers"))  # type: Mapping[str, Any]
         error_map = {401: ClientAuthenticationError, 409: ResourceReadOnlyError}
@@ -416,114 +416,118 @@
             error_map[412] = ResourceNotModifiedError
         if match_condition == MatchConditions.IfPresent:
             error_map[412] = ResourceNotFoundError
         if match_condition == MatchConditions.IfMissing:
             error_map[412] = ResourceExistsError
 
         try:
-            key_value_deleted = self._impl.delete_key_value(
+            key_value_deleted = await self._impl.delete_key_value(
                 key=key,
                 label=label,
                 if_match=prep_if_match(etag, match_condition),
                 headers=custom_headers,
                 error_map=error_map,
             )
             return ConfigurationSetting._from_generated(key_value_deleted)  # type: ignore
         except HttpResponseError as error:
             e = error_map[error.status_code]
-            raise e(message=error.message, response=error.response)
-        except binascii.Error:
-            raise binascii.Error("Connection string secret has incorrect padding")
+            raise e(message=error.message, response=error.response) from error
+        except binascii.Error as exc:
+            raise binascii.Error("Connection string secret has incorrect padding") from exc
 
     @distributed_trace
     def list_revisions(
-        self, key_filter: Optional[str] = None, label_filter: Optional[str] = None, **kwargs: Any
-    ) -> ItemPaged[ConfigurationSetting]:
+        self, key_filter: Optional[str] = None, label_filter: Optional[str] = None, **kwargs
+    ) -> AsyncItemPaged[ConfigurationSetting]:
+
         """
-        Find the ConfigurationSetting revision history.
+        Find the ConfigurationSetting revision history, optionally filtered by key, label and accept_datetime.
 
         :param key_filter: filter results based on their keys. '*' can be
-         used as wildcard in the beginning or end of the filter
+            used as wildcard in the beginning or end of the filter
         :type key_filter: str
         :param label_filter: filter results based on their label. '*' can be
-         used as wildcard in the beginning or end of the filter
+            used as wildcard in the beginning or end of the filter
         :type label_filter: str
-        :keyword datetime accept_datetime: filter out ConfigurationSetting created after this datetime
-        :keyword List[str] fields: specify which fields to include in the results. Leave None to include all fields
-        :return: An iterator of :class:`ConfigurationSetting`
-        :rtype: ~azure.core.paging.ItemPaged[ConfigurationSetting]
-        :raises: :class:`HttpResponseError`, :class:`ClientAuthenticationError`
+        :keyword str accept_datetime: retrieve ConfigurationSetting existed at this datetime
+        :keyword list[str] fields: specify which fields to include in the results. Leave None to include all fields
+        :return: An iterator of :class:`~azure.appconfiguration.ConfigurationSetting`
+        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.appconfiguration.ConfigurationSetting]
+        :raises: :class:`~azure.core.exceptions.HttpResponseError`, \
+            :class:`~azure.core.exceptions.ClientAuthenticationError`
 
         Example
 
         .. code-block:: python
 
+            # in async function
             from datetime import datetime, timedelta
 
-            accept_datetime = datetime.today() + timedelta(days=-1)
+            accept_datetime = datetime.utcnow() + timedelta(days=-1)
 
-            all_revisions = client.list_revisions()
-            for item in all_revisions:
+            all_revisions = async_client.list_revisions()
+            async for item in all_revisions:
                 pass  # do something
 
-            filtered_revisions = client.list_revisions(
-                label_filter="Labe*", key_filter="Ke*", accept_datetime=accept_datetime
+            filtered_revisions = async_client.list_revisions(
+                label_filter="Labe*", key_filter="Ke*", accept_datetime=str(accept_datetime)
             )
-            for item in filtered_revisions:
+            async for item in filtered_revisions:
                 pass  # do something
         """
         select = kwargs.pop("fields", None)
         if select:
             select = ["locked" if x == "read_only" else x for x in select]
         error_map = {401: ClientAuthenticationError}
 
         try:
             return self._impl.get_revisions(  # type: ignore
                 label=label_filter,
                 key=key_filter,
                 select=select,
-                cls=lambda objs: [
-                    ConfigurationSetting._from_generated(x) for x in objs
-                ],
+                cls=lambda objs: [ConfigurationSetting._from_generated(x) for x in objs],
                 error_map=error_map,
                 **kwargs
             )
         except HttpResponseError as error:
             e = error_map[error.status_code]
-            raise e(message=error.message, response=error.response)
-        except binascii.Error:
-            raise binascii.Error("Connection string secret has incorrect padding")
-
-    @distributed_trace
-    def set_read_only(
-        self, configuration_setting: ConfigurationSetting, read_only: Optional[bool] = True, **kwargs: Any
+            raise e(message=error.message, response=error.response) from error
+        except binascii.Error as exc:
+            raise binascii.Error("Connection string secret has incorrect padding") from exc
+
+    @distributed_trace_async
+    async def set_read_only(
+        self, configuration_setting: ConfigurationSetting, read_only: bool = True, **kwargs
     ) -> ConfigurationSetting:
+
         """Set a configuration setting read only
 
         :param configuration_setting: the ConfigurationSetting to be set read only
-        :type configuration_setting: :class:`ConfigurationSetting`
+        :type configuration_setting: ~azure.appconfiguration.ConfigurationSetting
         :param read_only: set the read only setting if true, else clear the read only setting
         :type read_only: bool
         :keyword match_condition: The match condition to use upon the etag
-        :paramtype match_condition: :class:`~azure.core.MatchConditions`
+        :paramtype match_condition: ~azure.core.MatchConditions
         :keyword str etag: check if the ConfigurationSetting is changed. Set None to skip checking etag
         :return: The ConfigurationSetting returned from the service
-        :rtype: :class:`~azure.appconfiguration.ConfigurationSetting`
-        :raises: :class:`HttpResponseError`, :class:`ClientAuthenticationError`, :class:`ResourceNotFoundError`
+        :rtype: ~azure.appconfiguration.ConfigurationSetting
+        :raises: :class:`~azure.core.exceptions.HttpResponseError`, \
+            :class:`~azure.core.exceptions.ClientAuthenticationError`, \
+            :class:`~azure.core.exceptions.ResourceNotFoundError`
 
         Example
 
         .. code-block:: python
 
-            config_setting = client.get_configuration_setting(
+            config_setting = await async_client.get_configuration_setting(
                 key="MyKey", label="MyLabel"
             )
 
-            read_only_config_setting = client.set_read_only(config_setting)
-            read_only_config_setting = client.set_read_only(config_setting, read_only=False)
+            read_only_config_setting = await async_client.set_read_only(config_setting)
+            read_only_config_setting = await client.set_read_only(config_setting, read_only=False)
         """
         error_map = {401: ClientAuthenticationError, 404: ResourceNotFoundError}
 
         match_condition = kwargs.pop("match_condition", MatchConditions.Unconditionally)
         if match_condition == MatchConditions.IfNotModified:
             error_map[412] = ResourceModifiedError
         if match_condition == MatchConditions.IfModified:
@@ -531,56 +535,232 @@
         if match_condition == MatchConditions.IfPresent:
             error_map[412] = ResourceNotFoundError
         if match_condition == MatchConditions.IfMissing:
             error_map[412] = ResourceExistsError
 
         try:
             if read_only:
-                key_value = self._impl.put_lock(
+                key_value = await self._impl.put_lock(
                     key=configuration_setting.key,
                     label=configuration_setting.label,
                     if_match=prep_if_match(configuration_setting.etag, match_condition),
-                    if_none_match=prep_if_none_match(
-                        configuration_setting.etag, match_condition
-                    ),
+                    if_none_match=prep_if_none_match(configuration_setting.etag, match_condition),
                     error_map=error_map,
                     **kwargs
                 )
             else:
-                key_value = self._impl.delete_lock(
+                key_value = await self._impl.delete_lock(
                     key=configuration_setting.key,
                     label=configuration_setting.label,
                     if_match=prep_if_match(configuration_setting.etag, match_condition),
-                    if_none_match=prep_if_none_match(
-                        configuration_setting.etag, match_condition
-                    ),
+                    if_none_match=prep_if_none_match(configuration_setting.etag, match_condition),
                     error_map=error_map,
                     **kwargs
                 )
             return ConfigurationSetting._from_generated(key_value)
         except HttpResponseError as error:
             e = error_map[error.status_code]
-            raise e(message=error.message, response=error.response)
+            raise e(message=error.message, response=error.response) from error
+        except binascii.Error as exc:
+            raise binascii.Error("Connection string secret has incorrect padding") from exc
+
+    @distributed_trace_async
+    async def begin_create_snapshot(
+        self,
+        name: str,
+        filters: List[ConfigurationSettingFilter],
+        *,
+        composition_type: Optional[Literal["key", "key_label"]] = None,
+        retention_period: Optional[int] = None,
+        tags: Optional[Dict[str, str]] = None,
+        **kwargs
+    ) -> AsyncLROPoller[Snapshot]:
+        """Create a snapshot of the configuration settings.
+
+        :param name: The name of the snapshot to create.
+        :type name: str
+        :param filters: A list of filters used to filter the configuration settings by key field and label field
+            included in the snapshot.
+        :type filters: list[~azure.appconfiguration.ConfigurationSettingFilter]
+        :keyword str composition_type: The composition type describes how the key-values
+            within the snapshot are composed. Known values are: "key" and "key_label". The "key" composition type
+            ensures there are no two key-values containing the same key. The 'key_label' composition type ensures
+            there are no two key-values containing the same key and label.
+        :keyword int retention_period: The amount of time, in seconds, that a snapshot will remain in the
+            archived state before expiring. This property is only writable during the creation of a
+            snapshot. If not specified, will set to 2592000(30 days). If specified, should be
+            in range 3600(1 hour) to 7776000(90 days).
+        :keyword dict[str, str] tags: The tags of the snapshot.
+        :return: A poller for create snapshot operation. Call `result()` on this object to wait for the
+            operation to complete and get the created snapshot.
+        :rtype: ~azure.core.polling.AsyncLROPoller[~azure.appconfiguration.Snapshot]
+        """
+        snapshot = Snapshot(
+            filters=filters, composition_type=composition_type, retention_period=retention_period, tags=tags
+        )
+        try:
+            return cast(
+                AsyncLROPoller[Snapshot],
+                await self._impl.begin_create_snapshot(
+                    name=name, entity=snapshot._to_generated(), cls=Snapshot._from_deserialized, **kwargs
+                ),
+            )
+        except binascii.Error:
+            raise binascii.Error("Connection string secret has incorrect padding")
+
+    @distributed_trace_async
+    async def archive_snapshot(
+        self,
+        name: str,
+        *,
+        match_condition: MatchConditions = MatchConditions.Unconditionally,
+        etag: Optional[str] = None,
+        **kwargs
+    ) -> Snapshot:
+        """Archive a configuration setting snapshot. It will update the status of a snapshot from "ready" to "archived".
+        The retention period will start to count, the snapshot will expire when the entire retention period elapses.
+
+        :param name: The name of the configuration setting snapshot to archive.
+        :type name: str
+        :keyword match_condition: The match condition to use upon the etag.
+        :type match_condition: ~azure.core.MatchConditions
+        :keyword str etag: Check if the Snapshot is changed. Set None to skip checking etag.
+        :return: The Snapshot returned from the service.
+        :rtype: ~azure.appconfiguration.Snapshot
+        """
+        try:
+            generated_snapshot = await self._impl.update_snapshot(
+                name=name,
+                entity=SnapshotUpdateParameters(status=SnapshotStatus.ARCHIVED),
+                if_match=prep_if_match(etag, match_condition),
+                if_none_match=prep_if_none_match(etag, match_condition),
+                **kwargs
+            )
+            return Snapshot._from_generated(generated_snapshot)
+        except binascii.Error:
+            raise binascii.Error("Connection string secret has incorrect padding")
+
+    @distributed_trace_async
+    async def recover_snapshot(
+        self,
+        name: str,
+        *,
+        match_condition: MatchConditions = MatchConditions.Unconditionally,
+        etag: Optional[str] = None,
+        **kwargs
+    ) -> Snapshot:
+        """Recover a configuration setting snapshot. It will update the status of a snapshot from "archived" to "ready".
+
+        :param name: The name of the configuration setting snapshot to recover.
+        :type name: str
+        :keyword match_condition: The match condition to use upon the etag.
+        :type match_condition: ~azure.core.MatchConditions
+        :keyword str etag: Check if the Snapshot is changed. Set None to skip checking etag.
+        :return: The Snapshot returned from the service.
+        :rtype: ~azure.appconfiguration.Snapshot
+        """
+        try:
+            generated_snapshot = await self._impl.update_snapshot(
+                name=name,
+                entity=SnapshotUpdateParameters(status=SnapshotStatus.READY),
+                if_match=prep_if_match(etag, match_condition),
+                if_none_match=prep_if_none_match(etag, match_condition),
+                **kwargs
+            )
+            return Snapshot._from_generated(generated_snapshot)
         except binascii.Error:
             raise binascii.Error("Connection string secret has incorrect padding")
 
-    def update_sync_token(self, token: str) -> None:
+    @distributed_trace_async
+    async def get_snapshot(self, name: str, *, fields: Optional[List[str]] = None, **kwargs) -> Snapshot:
+        """Get a configuration setting snapshot.
+
+        :param name: The name of the configuration setting snapshot to retrieve.
+        :type name: str
+        :keyword list[str] fields: Specify which fields to include in the results. Leave None to include all fields.
+        :return: The Snapshot returned from the service.
+        :rtype: ~azure.appconfiguration.Snapshot
+        """
+        try:
+            generated_snapshot = await self._impl.get_snapshot(
+                name=name, if_match=None, if_none_match=None, select=fields, **kwargs
+            )
+            return Snapshot._from_generated(generated_snapshot)
+        except binascii.Error:
+            raise binascii.Error("Connection string secret has incorrect padding")
+
+    @distributed_trace
+    def list_snapshots(
+        self,
+        *,
+        name: Optional[str] = None,
+        fields: Optional[List[str]] = None,
+        status: Optional[List[str]] = None,
+        **kwargs
+    ) -> AsyncItemPaged[Snapshot]:
+        """List the configuration setting snapshots stored in the configuration service, optionally filtered by
+        snapshot name, snapshot status and fields to present in return.
+
+        :keyword str name: Filter results based on snapshot name.
+        :keyword list[str] fields: Specify which fields to include in the results. Leave None to include all fields.
+        :keyword list[str] status: Filter results based on snapshot keys.
+        :return: An iterator of :class:`~azure.appconfiguration.Snapshot`
+        :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.appconfiguration.Snapshot]
+        """
+        try:
+            return self._impl.get_snapshots(  # type: ignore
+                name=name,
+                select=fields,
+                status=status,
+                cls=lambda objs: [Snapshot._from_generated(x) for x in objs],
+                **kwargs
+            )
+        except binascii.Error:
+            raise binascii.Error("Connection string secret has incorrect padding")
+
+    @distributed_trace
+    def list_snapshot_configuration_settings(
+        self, name: str, *, accept_datetime: Optional[str] = None, fields: Optional[List[str]] = None, **kwargs
+    ) -> AsyncItemPaged[ConfigurationSetting]:
+        """List the configuration settings stored under a snapshot in the configuration service, optionally filtered by
+        accept_datetime and fields to present in return.
+
+        :param str name: The snapshot name.
+        :keyword str accept_datetime: Filter out ConfigurationSetting created after this datetime.
+        :keyword list[str] fields: Specify which fields to include in the results. Leave None to include all fields.
+        :return: An iterator of :class:`~azure.appconfiguration.ConfigurationSetting`
+        :rtype: ~azure.core.paging.AsyncItemPaged[~azure.appconfiguration.ConfigurationSetting]
+        """
+        if fields:
+            fields = ["locked" if x == "read_only" else x for x in fields]
+
+        try:
+            return self._impl.get_key_values(  # type: ignore
+                select=fields,
+                snapshot=name,
+                accept_datetime=accept_datetime,
+                cls=lambda objs: [ConfigurationSetting._from_generated(x) for x in objs],
+                **kwargs
+            )
+        except binascii.Error:
+            raise binascii.Error("Connection string secret has incorrect padding")
+
+    async def update_sync_token(self, token: str) -> None:
+
         """Add a sync token to the internal list of tokens.
 
         :param str token: The sync token to be added to the internal list of tokens
         """
-        if not self._sync_token_policy:
-            raise AttributeError(
-                "Client has no sync token policy, possibly because it was not provided during instantiation."
-            )
-        self._sync_token_policy.add_token(token)
 
-    def close(self) -> None:
+        await self._sync_token_policy.add_token(token)
+
+    async def close(self) -> None:
+
         """Close all connections made by the client"""
-        self._impl._client.close()
+        await self._impl._client.close()
 
-    def __enter__(self):
-        self._impl.__enter__()
+    async def __aenter__(self):
+        await self._impl.__aenter__()
         return self
 
-    def __exit__(self, *args):
-        self._impl.__exit__(*args)
+    async def __aexit__(self, *args):
+        await self._impl.__aexit__(*args)
```

## Comparing `azure-appconfiguration-1.4.0b1/azure/appconfiguration/_sync_token.py` & `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_sync_token.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,24 +25,29 @@
 # --------------------------------------------------------------------------
 from typing import Any, Dict
 from threading import Lock
 from azure.core.pipeline import PipelineRequest, PipelineResponse
 from azure.core.pipeline.policies import SansIOHTTPPolicy
 
 
-class SyncToken(object):
-    """The sync token structure"""
+class SyncToken:
+    """The sync token structure
+
+    :param str token_id: The id of sync token.
+    :param str value: The value of sync token.
+    :param int sequence_number: The sequence number of sync token.
+    """
 
     def __init__(self, token_id, value, sequence_number):
         self.token_id = token_id
         self.value = value
         self.sequence_number = sequence_number
 
     def __str__(self):
-        return "{}={}".format(self.token_id, self.value)
+        return f"{self.token_id}={self.value}"
 
     @classmethod
     def from_sync_token_string(cls, sync_token):
         try:
             position = sync_token.index(";sn=")
             sequence_number = int(sync_token[position + 4 :])
             id_value = sync_token[:position]
@@ -51,38 +56,37 @@
             value = id_value[position + 1 :]
             return SyncToken(token_id, value, sequence_number)
         except ValueError:
             return None
 
 
 class SyncTokenPolicy(SansIOHTTPPolicy):
-    """A simple policy that enable the given callback
-    with the response.
+    """A simple policy that enable the given callback with the response.
+
     :keyword callback raw_response_hook: Callback function. Will be invoked on response.
     """
 
-    def __init__(self, **kwargs: Any) -> None:  # pylint: disable=unused-argument
+    def __init__(self, **kwargs) -> None:  # pylint: disable=unused-argument
         self._sync_token_header = "Sync-Token"
         self._sync_tokens = {}  # type: Dict[str, Any]
         self._lock = Lock()
 
     def on_request(self, request: PipelineRequest) -> None:  # type: ignore # pylint: disable=arguments-differ
         """This is executed before sending the request to the next policy.
         :param request: The PipelineRequest object.
         :type request: ~azure.core.pipeline.PipelineRequest
         """
         with self._lock:
             sync_token_header = ",".join(str(x) for x in self._sync_tokens.values())
             if sync_token_header:
-                request.http_request.headers.update(
-                    {self._sync_token_header: sync_token_header}
-                )
+                request.http_request.headers.update({self._sync_token_header: sync_token_header})
 
     def on_response(self, request: PipelineRequest, response: PipelineResponse) -> None:  # type: ignore # pylint: disable=arguments-differ
         """This is executed after the request comes back from the policy.
+
         :param request: The PipelineRequest object.
         :type request: ~azure.core.pipeline.PipelineRequest
         :param response: The PipelineResponse object.
         :type response: ~azure.core.pipeline.PipelineResponse
         """
         sync_token_header = response.http_response.headers.get(self._sync_token_header)
         if not sync_token_header:
```

## Comparing `azure-appconfiguration-1.4.0b1/azure/appconfiguration/__init__.py` & `azure-appconfiguration-1.5.0b1/azure/appconfiguration/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,22 +11,26 @@
 
 from ._azure_appconfiguration_client import AzureAppConfigurationClient
 from ._constants import FILTER_PERCENTAGE, FILTER_TARGETING, FILTER_TIME_WINDOW
 from ._models import (
     ConfigurationSetting,
     FeatureFlagConfigurationSetting,
     SecretReferenceConfigurationSetting,
+    Snapshot,
+    ConfigurationSettingFilter,
 )
 from ._version import VERSION
 from ._azure_appconfiguration_error import ResourceReadOnlyError
 
 __version__ = VERSION
 __all__ = [
     "AzureAppConfigurationClient",
     "ConfigurationSetting",
     "ResourceReadOnlyError",
     "FeatureFlagConfigurationSetting",
     "SecretReferenceConfigurationSetting",
+    "Snapshot",
+    "ConfigurationSettingFilter",
     "FILTER_PERCENTAGE",
     "FILTER_TARGETING",
     "FILTER_TIME_WINDOW",
 ]
```

## Comparing `azure-appconfiguration-1.4.0b1/azure/appconfiguration/_azure_appconfiguration_credential.py` & `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_azure_appconfiguration_credential.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,10 +13,8 @@
 
     :param connection_string: Connection String(one of the access keys of the Azure App Configuration resource)
         used to access the Azure App Configuration.
     :type connection_string: str
     """
 
     def __init__(self, connection_string):
-        self.host, self.credential, self.secret = parse_connection_string(
-            connection_string
-        )
+        self.host, self.credential, self.secret = parse_connection_string(connection_string)
```

## Comparing `azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/_patch.py` & `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/_serialization.py` & `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/_serialization.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,56 +21,71 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
 # IN THE SOFTWARE.
 #
 # --------------------------------------------------------------------------
 
 # pylint: skip-file
+# pyright: reportUnnecessaryTypeIgnoreComment=false
 
 from base64 import b64decode, b64encode
 import calendar
 import datetime
 import decimal
 import email
 from enum import Enum
 import json
 import logging
 import re
 import sys
 import codecs
+from typing import (
+    Dict,
+    Any,
+    cast,
+    Optional,
+    Union,
+    AnyStr,
+    IO,
+    Mapping,
+    Callable,
+    TypeVar,
+    MutableMapping,
+    Type,
+    List,
+    Mapping,
+)
 
 try:
     from urllib import quote  # type: ignore
 except ImportError:
-    from urllib.parse import quote  # type: ignore
+    from urllib.parse import quote
 import xml.etree.ElementTree as ET
 
-import isodate
-
-from typing import Dict, Any, cast, TYPE_CHECKING
+import isodate  # type: ignore
 
 from azure.core.exceptions import DeserializationError, SerializationError, raise_with_traceback
+from azure.core.serialization import NULL as AzureCoreNull
 
 _BOM = codecs.BOM_UTF8.decode(encoding="utf-8")
 
-if TYPE_CHECKING:
-    from typing import Optional, Union, AnyStr, IO, Mapping
+ModelType = TypeVar("ModelType", bound="Model")
+JSON = MutableMapping[str, Any]
 
 
 class RawDeserializer:
 
     # Accept "text" because we're open minded people...
     JSON_REGEXP = re.compile(r"^(application|text)/([a-z+.]+\+)?json$")
 
     # Name used in context
     CONTEXT_NAME = "deserialized_data"
 
     @classmethod
-    def deserialize_from_text(cls, data, content_type=None):
-        # type: (Optional[Union[AnyStr, IO]], Optional[str]) -> Any
+    def deserialize_from_text(cls, data: Optional[Union[AnyStr, IO]], content_type: Optional[str] = None) -> Any:
         """Decode data according to content-type.
 
         Accept a stream of data as well, but will be load at once in memory for now.
 
         If no content-type, will return the string version (not bytes, not stream)
 
         :param data: Input, could be bytes or stream (will be decoded with UTF8) or text
@@ -128,16 +143,15 @@
                 # The function hack is because Py2.7 messes up with exception
                 # context otherwise.
                 _LOGGER.critical("Wasn't XML not JSON, failing")
                 raise_with_traceback(DeserializationError, "XML is invalid")
         raise DeserializationError("Cannot deserialize content-type: {}".format(content_type))
 
     @classmethod
-    def deserialize_from_http_generics(cls, body_bytes, headers):
-        # type: (Optional[Union[AnyStr, IO]], Mapping) -> Any
+    def deserialize_from_http_generics(cls, body_bytes: Optional[Union[AnyStr, IO]], headers: Mapping) -> Any:
         """Deserialize from HTTP response.
 
         Use bytes and headers to NOT use any requests/aiohttp or whatever
         specific implementation.
         Headers will tested for "content-type"
         """
         # Try to use content-type from headers if available
@@ -156,16 +170,16 @@
         return None
 
 
 try:
     basestring  # type: ignore
     unicode_str = unicode  # type: ignore
 except NameError:
-    basestring = str  # type: ignore
-    unicode_str = str  # type: ignore
+    basestring = str
+    unicode_str = str
 
 _LOGGER = logging.getLogger(__name__)
 
 try:
     _long_type = long  # type: ignore
 except NameError:
     _long_type = int
@@ -184,15 +198,15 @@
 
     def dst(self, dt):
         """No daylight saving for UTC."""
         return datetime.timedelta(hours=1)
 
 
 try:
-    from datetime import timezone as _FixedOffset
+    from datetime import timezone as _FixedOffset  # type: ignore
 except ImportError:  # Python 2.7
 
     class _FixedOffset(datetime.tzinfo):  # type: ignore
         """Fixed offset in minutes east from UTC.
         Copy/pasted from Python doc
         :param datetime.timedelta offset: offset in timedelta format
         """
@@ -215,15 +229,15 @@
         def __getinitargs__(self):
             return (self.__offset,)
 
 
 try:
     from datetime import timezone
 
-    TZ_UTC = timezone.utc  # type: ignore
+    TZ_UTC = timezone.utc
 except ImportError:
     TZ_UTC = UTC()  # type: ignore
 
 _FLATTEN = re.compile(r"(?<!\\)\.")
 
 
 def attribute_transformer(key, attr_desc, value):
@@ -272,79 +286,84 @@
 
 
 class Model(object):
     """Mixin for all client request body/response body models to support
     serialization and deserialization.
     """
 
-    _subtype_map = {}  # type: Dict[str, Dict[str, Any]]
-    _attribute_map = {}  # type: Dict[str, Dict[str, Any]]
-    _validation = {}  # type: Dict[str, Dict[str, Any]]
+    _subtype_map: Dict[str, Dict[str, Any]] = {}
+    _attribute_map: Dict[str, Dict[str, Any]] = {}
+    _validation: Dict[str, Dict[str, Any]] = {}
 
-    def __init__(self, **kwargs):
-        self.additional_properties = {}
+    def __init__(self, **kwargs: Any) -> None:
+        self.additional_properties: Dict[str, Any] = {}
         for k in kwargs:
             if k not in self._attribute_map:
                 _LOGGER.warning("%s is not a known attribute of class %s and will be ignored", k, self.__class__)
             elif k in self._validation and self._validation[k].get("readonly", False):
                 _LOGGER.warning("Readonly attribute %s will be ignored in class %s", k, self.__class__)
             else:
                 setattr(self, k, kwargs[k])
 
-    def __eq__(self, other):
+    def __eq__(self, other: Any) -> bool:
         """Compare objects by comparing all attributes."""
         if isinstance(other, self.__class__):
             return self.__dict__ == other.__dict__
         return False
 
-    def __ne__(self, other):
+    def __ne__(self, other: Any) -> bool:
         """Compare objects by comparing all attributes."""
         return not self.__eq__(other)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return str(self.__dict__)
 
     @classmethod
-    def enable_additional_properties_sending(cls):
+    def enable_additional_properties_sending(cls) -> None:
         cls._attribute_map["additional_properties"] = {"key": "", "type": "{object}"}
 
     @classmethod
-    def is_xml_model(cls):
+    def is_xml_model(cls) -> bool:
         try:
-            cls._xml_map
+            cls._xml_map  # type: ignore
         except AttributeError:
             return False
         return True
 
     @classmethod
     def _create_xml_node(cls):
         """Create XML node."""
         try:
-            xml_map = cls._xml_map
+            xml_map = cls._xml_map  # type: ignore
         except AttributeError:
             xml_map = {}
 
         return _create_xml_node(xml_map.get("name", cls.__name__), xml_map.get("prefix", None), xml_map.get("ns", None))
 
-    def serialize(self, keep_readonly=False, **kwargs):
+    def serialize(self, keep_readonly: bool = False, **kwargs: Any) -> JSON:
         """Return the JSON that would be sent to azure from this model.
 
         This is an alias to `as_dict(full_restapi_key_transformer, keep_readonly=False)`.
 
         If you want XML serialization, you can pass the kwargs is_xml=True.
 
         :param bool keep_readonly: If you want to serialize the readonly attributes
         :returns: A dict JSON compatible object
         :rtype: dict
         """
         serializer = Serializer(self._infer_class_models())
         return serializer._serialize(self, keep_readonly=keep_readonly, **kwargs)
 
-    def as_dict(self, keep_readonly=True, key_transformer=attribute_transformer, **kwargs):
-        """Return a dict that can be JSONify using json.dump.
+    def as_dict(
+        self,
+        keep_readonly: bool = True,
+        key_transformer: Callable[[str, Dict[str, Any], Any], Any] = attribute_transformer,
+        **kwargs: Any
+    ) -> JSON:
+        """Return a dict that can be serialized using json.dump.
 
         Advanced usage might optionally use a callback as parameter:
 
         .. code::python
 
             def my_key_transformer(key, attr_desc, value):
                 return key
@@ -383,41 +402,46 @@
                 raise ValueError("Not Autorest generated code")
         except Exception:
             # Assume it's not Autorest generated (tests?). Add ourselves as dependencies.
             client_models = {cls.__name__: cls}
         return client_models
 
     @classmethod
-    def deserialize(cls, data, content_type=None):
+    def deserialize(cls: Type[ModelType], data: Any, content_type: Optional[str] = None) -> ModelType:
         """Parse a str using the RestAPI syntax and return a model.
 
         :param str data: A str using RestAPI structure. JSON by default.
         :param str content_type: JSON by default, set application/xml if XML.
         :returns: An instance of this model
         :raises: DeserializationError if something went wrong
         """
         deserializer = Deserializer(cls._infer_class_models())
         return deserializer(cls.__name__, data, content_type=content_type)
 
     @classmethod
-    def from_dict(cls, data, key_extractors=None, content_type=None):
+    def from_dict(
+        cls: Type[ModelType],
+        data: Any,
+        key_extractors: Optional[Callable[[str, Dict[str, Any], Any], Any]] = None,
+        content_type: Optional[str] = None,
+    ) -> ModelType:
         """Parse a dict using given key extractor return a model.
 
         By default consider key
         extractors (rest_key_case_insensitive_extractor, attribute_key_case_insensitive_extractor
         and last_rest_key_case_insensitive_extractor)
 
         :param dict data: A dict using RestAPI structure
         :param str content_type: JSON by default, set application/xml if XML.
         :returns: An instance of this model
         :raises: DeserializationError if something went wrong
         """
         deserializer = Deserializer(cls._infer_class_models())
-        deserializer.key_extractors = (
-            [
+        deserializer.key_extractors = (  # type: ignore
+            [  # type: ignore
                 attribute_key_case_insensitive_extractor,
                 rest_key_case_insensitive_extractor,
                 last_rest_key_case_insensitive_extractor,
             ]
             if key_extractors is None
             else key_extractors
         )
@@ -449,15 +473,15 @@
             if subtype_value:
                 # Try to match base class. Can be class name only
                 # (bug to fix in Autorest to support x-ms-discriminator-name)
                 if cls.__name__ == subtype_value:
                     return cls
                 flatten_mapping_type = cls._flatten_subtype(subtype_key, objects)
                 try:
-                    return objects[flatten_mapping_type[subtype_value]]
+                    return objects[flatten_mapping_type[subtype_value]]  # type: ignore
                 except KeyError:
                     _LOGGER.warning(
                         "Subtype value %s has no mapping, use base class %s.",
                         subtype_value,
                         cls.__name__,
                     )
                     break
@@ -517,15 +541,15 @@
         "min_items": lambda x, y: len(x) < y,
         "max_items": lambda x, y: len(x) > y,
         "pattern": lambda x, y: not re.match(y, x, re.UNICODE),
         "unique": lambda x, y: len(x) != len(set(x)),
         "multiple": lambda x, y: x % y != 0,
     }
 
-    def __init__(self, classes=None):
+    def __init__(self, classes: Optional[Mapping[str, Type[ModelType]]] = None):
         self.serialize_type = {
             "iso-8601": Serializer.serialize_iso,
             "rfc-1123": Serializer.serialize_rfc,
             "unix-time": Serializer.serialize_unix,
             "duration": Serializer.serialize_duration,
             "date": Serializer.serialize_date,
             "time": Serializer.serialize_time,
@@ -533,15 +557,15 @@
             "long": Serializer.serialize_long,
             "bytearray": Serializer.serialize_bytearray,
             "base64": Serializer.serialize_base64,
             "object": self.serialize_object,
             "[]": self.serialize_iter,
             "{}": self.serialize_dict,
         }
-        self.dependencies = dict(classes) if classes else {}
+        self.dependencies: Dict[str, Type[ModelType]] = dict(classes) if classes else {}
         self.key_transformer = full_restapi_key_transformer
         self.client_side_validation = True
 
     def _serialize(self, target_obj, data_type=None, **kwargs):
         """Serialize data into a string according to type.
 
         :param target_obj: The data to be serialized.
@@ -601,47 +625,46 @@
                         xml_desc = attr_desc.get("xml", {})
                         xml_name = xml_desc.get("name", attr_desc["key"])
                         xml_prefix = xml_desc.get("prefix", None)
                         xml_ns = xml_desc.get("ns", None)
                         if xml_desc.get("attr", False):
                             if xml_ns:
                                 ET.register_namespace(xml_prefix, xml_ns)
-                                xml_name = "{}{}".format(xml_ns, xml_name)
-                            serialized.set(xml_name, new_attr)
+                                xml_name = "{{{}}}{}".format(xml_ns, xml_name)
+                            serialized.set(xml_name, new_attr)  # type: ignore
                             continue
                         if xml_desc.get("text", False):
-                            serialized.text = new_attr
+                            serialized.text = new_attr  # type: ignore
                             continue
                         if isinstance(new_attr, list):
-                            serialized.extend(new_attr)
+                            serialized.extend(new_attr)  # type: ignore
                         elif isinstance(new_attr, ET.Element):
                             # If the down XML has no XML/Name, we MUST replace the tag with the local tag. But keeping the namespaces.
                             if "name" not in getattr(orig_attr, "_xml_map", {}):
                                 splitted_tag = new_attr.tag.split("}")
                                 if len(splitted_tag) == 2:  # Namespace
                                     new_attr.tag = "}".join([splitted_tag[0], xml_name])
                                 else:
                                     new_attr.tag = xml_name
-                            serialized.append(new_attr)
+                            serialized.append(new_attr)  # type: ignore
                         else:  # That's a basic type
                             # Integrate namespace if necessary
                             local_node = _create_xml_node(xml_name, xml_prefix, xml_ns)
                             local_node.text = unicode_str(new_attr)
-                            serialized.append(local_node)
+                            serialized.append(local_node)  # type: ignore
                     else:  # JSON
-                        for k in reversed(keys):
-                            unflattened = {k: new_attr}
-                            new_attr = unflattened
+                        for k in reversed(keys):  # type: ignore
+                            new_attr = {k: new_attr}
 
                         _new_attr = new_attr
                         _serialized = serialized
-                        for k in keys:
+                        for k in keys:  # type: ignore
                             if k not in _serialized:
-                                _serialized.update(_new_attr)
-                            _new_attr = _new_attr[k]
+                                _serialized.update(_new_attr)  # type: ignore
+                            _new_attr = _new_attr[k]  # type: ignore
                             _serialized = _serialized[k]
                 except ValueError:
                     continue
 
         except (AttributeError, KeyError, TypeError) as err:
             msg = "Attribute {} in object {} cannot be serialized.\n{}".format(attr_name, class_name, str(target_obj))
             raise_with_traceback(SerializationError, msg, err)
@@ -655,31 +678,31 @@
         :param str data_type: The type to be serialized from.
         :rtype: dict
         :raises: SerializationError if serialization fails.
         :raises: ValueError if data is None
         """
 
         # Just in case this is a dict
-        internal_data_type = data_type.strip("[]{}")
-        internal_data_type = self.dependencies.get(internal_data_type, None)
+        internal_data_type_str = data_type.strip("[]{}")
+        internal_data_type = self.dependencies.get(internal_data_type_str, None)
         try:
             is_xml_model_serialization = kwargs["is_xml"]
         except KeyError:
             if internal_data_type and issubclass(internal_data_type, Model):
                 is_xml_model_serialization = kwargs.setdefault("is_xml", internal_data_type.is_xml_model())
             else:
                 is_xml_model_serialization = False
         if internal_data_type and not isinstance(internal_data_type, Enum):
             try:
                 deserializer = Deserializer(self.dependencies)
                 # Since it's on serialization, it's almost sure that format is not JSON REST
                 # We're not able to deal with additional properties for now.
                 deserializer.additional_properties_detection = False
                 if is_xml_model_serialization:
-                    deserializer.key_extractors = [
+                    deserializer.key_extractors = [  # type: ignore
                         attribute_key_case_insensitive_extractor,
                     ]
                 else:
                     deserializer.key_extractors = [
                         rest_key_case_insensitive_extractor,
                         attribute_key_case_insensitive_extractor,
                         last_rest_key_case_insensitive_extractor,
@@ -776,14 +799,16 @@
         :raises: ValueError if data is None
         :raises: SerializationError if serialization fails.
         """
         if data is None:
             raise ValueError("No value for given attribute")
 
         try:
+            if data is AzureCoreNull:
+                return None
             if data_type in self.basic_types.values():
                 return self.serialize_basic(data, data_type, **kwargs)
 
             elif data_type in self.serialize_type:
                 return self.serialize_type[data_type](data, **kwargs)
 
             # If dependencies is empty, try with current data class
@@ -839,15 +864,15 @@
         """
         try:  # If I received an enum, return its value
             return data.value
         except AttributeError:
             pass
 
         try:
-            if isinstance(data, unicode):
+            if isinstance(data, unicode):  # type: ignore
                 # Don't change it, JSON and XML ElementTree are totally able
                 # to serialize correctly u'' strings
                 return data
         except NameError:
             return str(data)
         else:
             return str(data)
@@ -997,18 +1022,18 @@
     @staticmethod
     def serialize_enum(attr, enum_obj=None):
         try:
             result = attr.value
         except AttributeError:
             result = attr
         try:
-            enum_obj(result)
+            enum_obj(result)  # type: ignore
             return result
         except ValueError:
-            for enum_value in enum_obj:
+            for enum_value in enum_obj:  # type: ignore
                 if enum_value.value.lower() == str(attr).lower():
                     return enum_value.value
             error = "{!r} is not valid value for enum {!r}"
             raise SerializationError(error.format(attr, enum_obj))
 
     @staticmethod
     def serialize_bytearray(attr, **kwargs):
@@ -1160,15 +1185,16 @@
 
 
 def rest_key_extractor(attr, attr_desc, data):
     key = attr_desc["key"]
     working_data = data
 
     while "." in key:
-        dict_keys = _FLATTEN.split(key)
+        # Need the cast, as for some reasons "split" is typed as list[str | Any]
+        dict_keys = cast(List[str], _FLATTEN.split(key))
         if len(dict_keys) == 1:
             key = _decode_attribute_map_key(dict_keys[0])
             break
         working_key = _decode_attribute_map_key(dict_keys[0])
         working_data = working_data.get(working_key, data)
         if working_data is None:
             # If at any point while following flatten JSON path see None, it means
@@ -1241,15 +1267,15 @@
     :rtype: tuple
     :returns: A tuple XML name + namespace dict
     """
     internal_type_xml_map = getattr(internal_type, "_xml_map", {})
     xml_name = internal_type_xml_map.get("name", internal_type.__name__)
     xml_ns = internal_type_xml_map.get("ns", None)
     if xml_ns:
-        xml_name = "{}{}".format(xml_ns, xml_name)
+        xml_name = "{{{}}}{}".format(xml_ns, xml_name)
     return xml_name
 
 
 def xml_key_extractor(attr, attr_desc, data):
     if isinstance(data, dict):
         return None
 
@@ -1265,15 +1291,15 @@
     is_wrapped = xml_desc.get("wrapped", False)
     internal_type = attr_desc.get("internalType", None)
     internal_type_xml_map = getattr(internal_type, "_xml_map", {})
 
     # Integrate namespace if necessary
     xml_ns = xml_desc.get("ns", internal_type_xml_map.get("ns", None))
     if xml_ns:
-        xml_name = "{}{}".format(xml_ns, xml_name)
+        xml_name = "{{{}}}{}".format(xml_ns, xml_name)
 
     # If it's an attribute, that's simple
     if xml_desc.get("attr", False):
         return data.get(xml_name)
 
     # If it's x-ms-text, that's simple too
     if xml_desc.get("text", False):
@@ -1331,15 +1357,15 @@
     :ivar list key_extractors: Ordered list of extractors to be used by this deserializer.
     """
 
     basic_types = {str: "str", int: "int", bool: "bool", float: "float"}
 
     valid_date = re.compile(r"\d{4}[-]\d{2}[-]\d{2}T\d{2}:\d{2}:\d{2}" r"\.?\d*Z?[-+]?[\d{2}]?:?[\d{2}]?")
 
-    def __init__(self, classes=None):
+    def __init__(self, classes: Optional[Mapping[str, Type[ModelType]]] = None):
         self.deserialize_type = {
             "iso-8601": Deserializer.deserialize_iso,
             "rfc-1123": Deserializer.deserialize_rfc,
             "unix-time": Deserializer.deserialize_unix,
             "duration": Deserializer.deserialize_duration,
             "date": Deserializer.deserialize_date,
             "time": Deserializer.deserialize_time,
@@ -1351,15 +1377,15 @@
             "[]": self.deserialize_iter,
             "{}": self.deserialize_dict,
         }
         self.deserialize_expected_types = {
             "duration": (isodate.Duration, datetime.timedelta),
             "iso-8601": (datetime.datetime),
         }
-        self.dependencies = dict(classes) if classes else {}
+        self.dependencies: Dict[str, Type[ModelType]] = dict(classes) if classes else {}
         self.key_extractors = [rest_key_extractor, xml_key_extractor]
         # Additional properties only works if the "rest_key_extractor" is used to
         # extract the keys. Making it to work whatever the key extractor is too much
         # complicated, with no real scenario for now.
         # So adding a flag to disable additional properties detection. This flag should be
         # used if your expect the deserialization to NOT come from a JSON REST syntax.
         # Otherwise, result are unexpected
@@ -1412,15 +1438,15 @@
             return self.deserialize_data(data, response)
         elif isinstance(response, type) and issubclass(response, Enum):
             return self.deserialize_enum(data, response)
 
         if data is None:
             return data
         try:
-            attributes = response._attribute_map
+            attributes = response._attribute_map  # type: ignore
             d_attrs = {}
             for attr, attr_desc in attributes.items():
                 # Check empty string. If it's not empty, someone has a real "additionalProperties"...
                 if attr == "additional_properties" and attr_desc["key"] == "":
                     continue
                 raw_value = None
                 # Enhance attr_desc with some dynamic data
@@ -1440,15 +1466,15 @@
                             _LOGGER.warning(msg, found_value, key_extractor, attr)
                             continue
                         raw_value = found_value
 
                 value = self.deserialize_data(raw_value, attr_desc["type"])
                 d_attrs[attr] = value
         except (AttributeError, TypeError, KeyError) as err:
-            msg = "Unable to deserialize to object: " + class_name
+            msg = "Unable to deserialize to object: " + class_name  # type: ignore
             raise_with_traceback(DeserializationError, msg, err)
         else:
             additional_properties = self._build_additional_properties(attributes, data)
             return self._instantiate_model(response, d_attrs, additional_properties)
 
     def _build_additional_properties(self, attribute_map, data):
         if not self.additional_properties_detection:
@@ -1470,40 +1496,40 @@
 
     def _classify_target(self, target, data):
         """Check to see whether the deserialization target object can
         be classified into a subclass.
         Once classification has been determined, initialize object.
 
         :param str target: The target object type to deserialize to.
-        :param str/dict data: The response data to deseralize.
+        :param str/dict data: The response data to deserialize.
         """
         if target is None:
             return None, None
 
         if isinstance(target, basestring):
             try:
                 target = self.dependencies[target]
             except KeyError:
                 return target, target
 
         try:
             target = target._classify(data, self.dependencies)
         except AttributeError:
             pass  # Target is not a Model, no classify
-        return target, target.__class__.__name__
+        return target, target.__class__.__name__  # type: ignore
 
     def failsafe_deserialize(self, target_obj, data, content_type=None):
         """Ignores any errors encountered in deserialization,
         and falls back to not deserializing the object. Recommended
         for use in error deserialization, as we want to return the
         HttpResponseError to users, and not have them deal with
         a deserialization error.
 
         :param str target_obj: The target object type to deserialize to.
-        :param str/dict data: The response data to deseralize.
+        :param str/dict data: The response data to deserialize.
         :param str content_type: Swagger "produces" if available.
         """
         try:
             return self(target_obj, data, content_type=content_type)
         except:
             _LOGGER.debug(
                 "Ran into a deserialization error. Ignoring since this is failsafe deserialization", exc_info=True
@@ -1539,15 +1565,15 @@
             return RawDeserializer.deserialize_from_http_generics(raw_data.text(), raw_data.headers)
 
         # Assume this enough to recognize requests.Response without importing it.
         if hasattr(raw_data, "_content_consumed"):
             return RawDeserializer.deserialize_from_http_generics(raw_data.text, raw_data.headers)
 
         if isinstance(raw_data, (basestring, bytes)) or hasattr(raw_data, "read"):
-            return RawDeserializer.deserialize_from_text(raw_data, content_type)
+            return RawDeserializer.deserialize_from_text(raw_data, content_type)  # type: ignore
         return raw_data
 
     def _instantiate_model(self, response, attrs, additional_properties=None):
         """Instantiate a response model passing in deserialized args.
 
         :param response: The response model class.
         :param d_attrs: The deserialized response attributes.
@@ -1561,15 +1587,15 @@
                 response_obj = response(**kwargs)
                 for attr in readonly:
                     setattr(response_obj, attr, attrs.get(attr))
                 if additional_properties:
                     response_obj.additional_properties = additional_properties
                 return response_obj
             except TypeError as err:
-                msg = "Unable to deserialize {} into model {}. ".format(kwargs, response)
+                msg = "Unable to deserialize {} into model {}. ".format(kwargs, response)  # type: ignore
                 raise DeserializationError(msg + str(err))
         else:
             try:
                 for attr, value in attrs.items():
                     setattr(response, attr, value)
                 return response
             except Exception as exp:
@@ -1743,15 +1769,15 @@
         # We might be here because we have an enum modeled as string,
         # and we try to deserialize a partial dict with enum inside
         if isinstance(data, Enum):
             return data
 
         # Consider this is real string
         try:
-            if isinstance(data, unicode):
+            if isinstance(data, unicode):  # type: ignore
                 return data
         except NameError:
             return str(data)
         else:
             return str(data)
 
     @staticmethod
@@ -1794,58 +1820,58 @@
 
         :param str attr: response string to be deserialized.
         :rtype: bytearray
         :raises: TypeError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
-        return bytearray(b64decode(attr))
+        return bytearray(b64decode(attr))  # type: ignore
 
     @staticmethod
     def deserialize_base64(attr):
         """Deserialize base64 encoded string into string.
 
         :param str attr: response string to be deserialized.
         :rtype: bytearray
         :raises: TypeError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
-        padding = "=" * (3 - (len(attr) + 3) % 4)
-        attr = attr + padding
+        padding = "=" * (3 - (len(attr) + 3) % 4)  # type: ignore
+        attr = attr + padding  # type: ignore
         encoded = attr.replace("-", "+").replace("_", "/")
         return b64decode(encoded)
 
     @staticmethod
     def deserialize_decimal(attr):
         """Deserialize string into Decimal object.
 
         :param str attr: response string to be deserialized.
         :rtype: Decimal
         :raises: DeserializationError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
         try:
-            return decimal.Decimal(attr)
+            return decimal.Decimal(attr)  # type: ignore
         except decimal.DecimalException as err:
             msg = "Invalid decimal {}".format(attr)
             raise_with_traceback(DeserializationError, msg, err)
 
     @staticmethod
     def deserialize_long(attr):
         """Deserialize string into long (Py2) or int (Py3).
 
         :param str attr: response string to be deserialized.
         :rtype: long or int
         :raises: ValueError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
-        return _long_type(attr)
+        return _long_type(attr)  # type: ignore
 
     @staticmethod
     def deserialize_duration(attr):
         """Deserialize ISO-8601 formatted string into TimeDelta object.
 
         :param str attr: response string to be deserialized.
         :rtype: TimeDelta
@@ -1867,45 +1893,45 @@
 
         :param str attr: response string to be deserialized.
         :rtype: Date
         :raises: DeserializationError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
-        if re.search(r"[^\W\d_]", attr, re.I + re.U):
+        if re.search(r"[^\W\d_]", attr, re.I + re.U):  # type: ignore
             raise DeserializationError("Date must have only digits and -. Received: %s" % attr)
         # This must NOT use defaultmonth/defaultday. Using None ensure this raises an exception.
         return isodate.parse_date(attr, defaultmonth=None, defaultday=None)
 
     @staticmethod
     def deserialize_time(attr):
         """Deserialize ISO-8601 formatted string into time object.
 
         :param str attr: response string to be deserialized.
         :rtype: datetime.time
         :raises: DeserializationError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
-        if re.search(r"[^\W\d_]", attr, re.I + re.U):
+        if re.search(r"[^\W\d_]", attr, re.I + re.U):  # type: ignore
             raise DeserializationError("Date must have only digits and -. Received: %s" % attr)
         return isodate.parse_time(attr)
 
     @staticmethod
     def deserialize_rfc(attr):
         """Deserialize RFC-1123 formatted string into Datetime object.
 
         :param str attr: response string to be deserialized.
         :rtype: Datetime
         :raises: DeserializationError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
         try:
-            parsed_date = email.utils.parsedate_tz(attr)
+            parsed_date = email.utils.parsedate_tz(attr)  # type: ignore
             date_obj = datetime.datetime(
                 *parsed_date[:6], tzinfo=_FixedOffset(datetime.timedelta(minutes=(parsed_date[9] or 0) / 60))
             )
             if not date_obj.tzinfo:
                 date_obj = date_obj.astimezone(tz=TZ_UTC)
         except ValueError as err:
             msg = "Cannot deserialize to rfc datetime object."
@@ -1920,15 +1946,15 @@
         :param str attr: response string to be deserialized.
         :rtype: Datetime
         :raises: DeserializationError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
         try:
-            attr = attr.upper()
+            attr = attr.upper()  # type: ignore
             match = Deserializer.valid_date.match(attr)
             if not match:
                 raise ValueError("Invalid datetime string: " + attr)
 
             check_decimal = attr.split(".")
             if len(check_decimal) > 1:
                 decimal_str = ""
@@ -1956,15 +1982,15 @@
         This is represented as seconds.
 
         :param int attr: Object to be serialized.
         :rtype: Datetime
         :raises: DeserializationError if format invalid
         """
         if isinstance(attr, ET.Element):
-            attr = int(attr.text)
+            attr = int(attr.text)  # type: ignore
         try:
             date_obj = datetime.datetime.fromtimestamp(attr, TZ_UTC)
         except ValueError as err:
             msg = "Cannot deserialize to unix datetime object."
             raise_with_traceback(DeserializationError, msg, err)
         else:
             return date_obj
```

## Comparing `azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/_vendor.py` & `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/_vendor.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from abc import ABC
-from typing import TYPE_CHECKING
+from typing import List, TYPE_CHECKING, cast
 
 from azure.core.pipeline.transport import HttpRequest
 
 from ._configuration import AzureAppConfigurationConfiguration
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
@@ -29,19 +29,20 @@
 
 def _format_url_section(template, **kwargs):
     components = template.split("/")
     while components:
         try:
             return template.format(**kwargs)
         except KeyError as key:
-            formatted_components = template.split("/")
+            # Need the cast, as for some reasons "split" is typed as list[str | Any]
+            formatted_components = cast(List[str], template.split("/"))
             components = [c for c in formatted_components if "{}".format(key.args[0]) not in c]
             template = "/".join(components)
 
 
-class MixinABC(ABC):
+class AzureAppConfigurationMixinABC(ABC):
     """DO NOT use this class. It is for internal typing use only."""
 
     _client: "PipelineClient"
     _config: AzureAppConfigurationConfiguration
     _serialize: "Serializer"
     _deserialize: "Deserializer"
```

## Comparing `azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/__init__.py` & `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/operations/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,20 +2,18 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
-from ._azure_app_configuration import AzureAppConfiguration
+from ._azure_app_configuration_operations import AzureAppConfigurationOperationsMixin
 
-try:
-    from ._patch import __all__ as _patch_all
-    from ._patch import *  # type: ignore # pylint: disable=unused-wildcard-import
-except ImportError:
-    _patch_all = []
+from ._patch import __all__ as _patch_all
+from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
-__all__ = ["AzureAppConfiguration"]
+__all__ = [
+    "AzureAppConfigurationOperationsMixin",
+]
 __all__.extend([p for p in _patch_all if p not in __all__])
-
 _patch_sdk()
```

## Comparing `azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/_configuration.py` & `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/_configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,36 +21,33 @@
     attributes.
 
     :param endpoint: The endpoint of the App Configuration instance to send requests to. Required.
     :type endpoint: str
     :param sync_token: Used to guarantee real-time consistency between requests. Default value is
      None.
     :type sync_token: str
-    :keyword api_version: Api Version. Default value is "1.0". Note that overriding this default
-     value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2022-11-01-preview". Note that overriding
+     this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, endpoint: str, sync_token: Optional[str] = None, **kwargs: Any) -> None:
         super(AzureAppConfigurationConfiguration, self).__init__(**kwargs)
-        api_version = kwargs.pop("api_version", "1.0")  # type: str
+        api_version: str = kwargs.pop("api_version", "2022-11-01-preview")
 
         if endpoint is None:
             raise ValueError("Parameter 'endpoint' must not be None.")
 
         self.endpoint = endpoint
         self.sync_token = sync_token
         self.api_version = api_version
         kwargs.setdefault("sdk_moniker", "appconfiguration/{}".format(VERSION))
         self._configure(**kwargs)
 
-    def _configure(
-        self, **kwargs  # type: Any
-    ):
-        # type: (...) -> None
+    def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get("http_logging_policy") or policies.HttpLoggingPolicy(**kwargs)
         self.retry_policy = kwargs.get("retry_policy") or policies.RetryPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
```

## Comparing `azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/_azure_app_configuration.py` & `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/_azure_app_configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,41 +8,43 @@
 
 from copy import deepcopy
 from typing import Any, Optional
 
 from azure.core import PipelineClient
 from azure.core.rest import HttpRequest, HttpResponse
 
-from . import models
+from . import models as _models
 from ._configuration import AzureAppConfigurationConfiguration
 from ._serialization import Deserializer, Serializer
 from .operations import AzureAppConfigurationOperationsMixin
 
 
 class AzureAppConfiguration(AzureAppConfigurationOperationsMixin):  # pylint: disable=client-accepts-api-version-keyword
     """AzureAppConfiguration.
 
     :param endpoint: The endpoint of the App Configuration instance to send requests to. Required.
     :type endpoint: str
     :param sync_token: Used to guarantee real-time consistency between requests. Default value is
      None.
     :type sync_token: str
-    :keyword api_version: Api Version. Default value is "1.0". Note that overriding this default
-     value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2022-11-01-preview". Note that overriding
+     this default value may result in unsupported behavior.
     :paramtype api_version: str
+    :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+     Retry-After header is present.
     """
 
     def __init__(  # pylint: disable=missing-client-constructor-parameter-credential
         self, endpoint: str, sync_token: Optional[str] = None, **kwargs: Any
     ) -> None:
         _endpoint = "{endpoint}"
         self._config = AzureAppConfigurationConfiguration(endpoint=endpoint, sync_token=sync_token, **kwargs)
-        self._client = PipelineClient(base_url=_endpoint, config=self._config, **kwargs)
+        self._client: PipelineClient = PipelineClient(base_url=_endpoint, config=self._config, **kwargs)
 
-        client_models = {k: v for k, v in models.__dict__.items() if isinstance(v, type)}
+        client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
 
     def _send_request(self, request: HttpRequest, **kwargs: Any) -> HttpResponse:
         """Runs the network request through the client's chained policies.
 
@@ -65,19 +67,16 @@
         path_format_arguments = {
             "endpoint": self._serialize.url("self._config.endpoint", self._config.endpoint, "str", skip_quote=True),
         }
 
         request_copy.url = self._client.format_url(request_copy.url, **path_format_arguments)
         return self._client.send_request(request_copy, **kwargs)
 
-    def close(self):
-        # type: () -> None
+    def close(self) -> None:
         self._client.close()
 
-    def __enter__(self):
-        # type: () -> AzureAppConfiguration
+    def __enter__(self) -> "AzureAppConfiguration":
         self._client.__enter__()
         return self
 
-    def __exit__(self, *exc_details):
-        # type: (Any) -> None
+    def __exit__(self, *exc_details: Any) -> None:
         self._client.__exit__(*exc_details)
```

## Comparing `azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/operations/_patch.py` & `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/operations/__init__.py` & `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/operations/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._azure_app_configuration_operations import AzureAppConfigurationOperationsMixin
 
 from ._patch import __all__ as _patch_all
-from ._patch import *  # type: ignore # pylint: disable=unused-wildcard-import
+from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "AzureAppConfigurationOperationsMixin",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

## Comparing `azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/models/_patch.py` & `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/models/__init__.py` & `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/models/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,45 +3,55 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._models_py3 import Error
+from ._models_py3 import ErrorDetail
+from ._models_py3 import InnerError
 from ._models_py3 import Key
 from ._models_py3 import KeyListResult
 from ._models_py3 import KeyValue
+from ._models_py3 import KeyValueFilter
 from ._models_py3 import KeyValueListResult
 from ._models_py3 import Label
 from ._models_py3 import LabelListResult
+from ._models_py3 import OperationDetails
+from ._models_py3 import Snapshot
+from ._models_py3 import SnapshotListResult
+from ._models_py3 import SnapshotUpdateParameters
 
-from ._azure_app_configuration_enums import Enum6
-from ._azure_app_configuration_enums import Enum7
-from ._azure_app_configuration_enums import Get5ItemsItem
-from ._azure_app_configuration_enums import Get6ItemsItem
-from ._azure_app_configuration_enums import Get7ItemsItem
-from ._azure_app_configuration_enums import Head5ItemsItem
-from ._azure_app_configuration_enums import Head6ItemsItem
-from ._azure_app_configuration_enums import Head7ItemsItem
+from ._azure_app_configuration_enums import CompositionType
+from ._azure_app_configuration_enums import KeyValueFields
+from ._azure_app_configuration_enums import LabelFields
+from ._azure_app_configuration_enums import SnapshotFields
+from ._azure_app_configuration_enums import SnapshotStatus
+from ._azure_app_configuration_enums import State
 from ._patch import __all__ as _patch_all
-from ._patch import *  # type: ignore # pylint: disable=unused-wildcard-import
+from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
     "Error",
+    "ErrorDetail",
+    "InnerError",
     "Key",
     "KeyListResult",
     "KeyValue",
+    "KeyValueFilter",
     "KeyValueListResult",
     "Label",
     "LabelListResult",
-    "Enum6",
-    "Enum7",
-    "Get5ItemsItem",
-    "Get6ItemsItem",
-    "Get7ItemsItem",
-    "Head5ItemsItem",
-    "Head6ItemsItem",
-    "Head7ItemsItem",
+    "OperationDetails",
+    "Snapshot",
+    "SnapshotListResult",
+    "SnapshotUpdateParameters",
+    "CompositionType",
+    "KeyValueFields",
+    "LabelFields",
+    "SnapshotFields",
+    "SnapshotStatus",
+    "State",
 ]
 __all__.extend([p for p in _patch_all if p not in __all__])
 _patch_sdk()
```

## Comparing `azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/aio/_patch.py` & `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/aio/_vendor.py` & `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/_vendor.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,14 @@
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core import AsyncPipelineClient
 
     from .._serialization import Deserializer, Serializer
 
 
-class MixinABC(ABC):
+class AzureAppConfigurationMixinABC(ABC):
     """DO NOT use this class. It is for internal typing use only."""
 
     _client: "AsyncPipelineClient"
     _config: AzureAppConfigurationConfiguration
     _serialize: "Serializer"
     _deserialize: "Deserializer"
```

## Comparing `azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/aio/__init__.py` & `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,16 +6,18 @@
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._azure_app_configuration import AzureAppConfiguration
 
 try:
     from ._patch import __all__ as _patch_all
-    from ._patch import *  # type: ignore # pylint: disable=unused-wildcard-import
+    from ._patch import *  # pylint: disable=unused-wildcard-import
 except ImportError:
     _patch_all = []
 from ._patch import patch_sdk as _patch_sdk
 
-__all__ = ["AzureAppConfiguration"]
+__all__ = [
+    "AzureAppConfiguration",
+]
 __all__.extend([p for p in _patch_all if p not in __all__])
 
 _patch_sdk()
```

## Comparing `azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/aio/_configuration.py` & `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/_configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,22 +21,22 @@
     attributes.
 
     :param endpoint: The endpoint of the App Configuration instance to send requests to. Required.
     :type endpoint: str
     :param sync_token: Used to guarantee real-time consistency between requests. Default value is
      None.
     :type sync_token: str
-    :keyword api_version: Api Version. Default value is "1.0". Note that overriding this default
-     value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2022-11-01-preview". Note that overriding
+     this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, endpoint: str, sync_token: Optional[str] = None, **kwargs: Any) -> None:
         super(AzureAppConfigurationConfiguration, self).__init__(**kwargs)
-        api_version = kwargs.pop("api_version", "1.0")  # type: str
+        api_version: str = kwargs.pop("api_version", "2022-11-01-preview")
 
         if endpoint is None:
             raise ValueError("Parameter 'endpoint' must not be None.")
 
         self.endpoint = endpoint
         self.sync_token = sync_token
         self.api_version = api_version
```

## Comparing `azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/aio/_azure_app_configuration.py` & `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/aio/_azure_app_configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,41 +8,43 @@
 
 from copy import deepcopy
 from typing import Any, Awaitable, Optional
 
 from azure.core import AsyncPipelineClient
 from azure.core.rest import AsyncHttpResponse, HttpRequest
 
-from .. import models
+from .. import models as _models
 from .._serialization import Deserializer, Serializer
 from ._configuration import AzureAppConfigurationConfiguration
 from .operations import AzureAppConfigurationOperationsMixin
 
 
 class AzureAppConfiguration(AzureAppConfigurationOperationsMixin):  # pylint: disable=client-accepts-api-version-keyword
     """AzureAppConfiguration.
 
     :param endpoint: The endpoint of the App Configuration instance to send requests to. Required.
     :type endpoint: str
     :param sync_token: Used to guarantee real-time consistency between requests. Default value is
      None.
     :type sync_token: str
-    :keyword api_version: Api Version. Default value is "1.0". Note that overriding this default
-     value may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2022-11-01-preview". Note that overriding
+     this default value may result in unsupported behavior.
     :paramtype api_version: str
+    :keyword int polling_interval: Default waiting time between two polls for LRO operations if no
+     Retry-After header is present.
     """
 
     def __init__(  # pylint: disable=missing-client-constructor-parameter-credential
         self, endpoint: str, sync_token: Optional[str] = None, **kwargs: Any
     ) -> None:
         _endpoint = "{endpoint}"
         self._config = AzureAppConfigurationConfiguration(endpoint=endpoint, sync_token=sync_token, **kwargs)
-        self._client = AsyncPipelineClient(base_url=_endpoint, config=self._config, **kwargs)
+        self._client: AsyncPipelineClient = AsyncPipelineClient(base_url=_endpoint, config=self._config, **kwargs)
 
-        client_models = {k: v for k, v in models.__dict__.items() if isinstance(v, type)}
+        client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
 
     def _send_request(self, request: HttpRequest, **kwargs: Any) -> Awaitable[AsyncHttpResponse]:
         """Runs the network request through the client's chained policies.
 
@@ -72,9 +74,9 @@
     async def close(self) -> None:
         await self._client.close()
 
     async def __aenter__(self) -> "AzureAppConfiguration":
         await self._client.__aenter__()
         return self
 
-    async def __aexit__(self, *exc_details) -> None:
+    async def __aexit__(self, *exc_details: Any) -> None:
         await self._client.__aexit__(*exc_details)
```

## Comparing `azure-appconfiguration-1.4.0b1/azure/appconfiguration/_generated/aio/operations/_patch.py` & `azure-appconfiguration-1.5.0b1/azure/appconfiguration/_generated/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.4.0b1/azure/appconfiguration/aio/_sync_token_async.py` & `azure-appconfiguration-1.5.0b1/azure/appconfiguration/aio/_sync_token_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,38 +28,38 @@
 from azure.core.pipeline import PipelineRequest, PipelineResponse
 from azure.core.pipeline.policies import SansIOHTTPPolicy
 
 from .._sync_token import SyncToken
 
 
 class AsyncSyncTokenPolicy(SansIOHTTPPolicy):
-    """A simple policy that enable the given callback
-    with the response.
+    """A simple policy that enable the given callback with the response.
+
     :keyword callback raw_response_hook: Callback function. Will be invoked on response.
     """
 
-    def __init__(self, **kwargs: Any) -> None:  # pylint: disable=unused-argument
+    def __init__(self, **kwargs) -> None:  # pylint: disable=unused-argument
         self._sync_token_header = "Sync-Token"
         self._sync_tokens = {}  # type: Dict[str, Any]
         self._lock = Lock()
 
     async def on_request(self, request: PipelineRequest) -> None:  # type: ignore # pylint: disable=arguments-differ, invalid-overridden-method
         """This is executed before sending the request to the next policy.
+
         :param request: The PipelineRequest object.
         :type request: ~azure.core.pipeline.PipelineRequest
         """
         async with self._lock:
             sync_token_header = ",".join(str(x) for x in self._sync_tokens.values())
             if sync_token_header:
-                request.http_request.headers.update(
-                    {self._sync_token_header: sync_token_header}
-                )
+                request.http_request.headers.update({self._sync_token_header: sync_token_header})
 
     async def on_response(self, request: PipelineRequest, response: PipelineResponse) -> None:  # type: ignore # pylint: disable=arguments-differ, invalid-overridden-method
         """This is executed after the request comes back from the policy.
+
         :param request: The PipelineRequest object.
         :type request: ~azure.core.pipeline.PipelineRequest
         :param response: The PipelineResponse object.
         :type response: ~azure.core.pipeline.PipelineResponse
         """
         sync_token_header = response.http_response.headers.get(self._sync_token_header)
         if not sync_token_header:
```

## Comparing `azure-appconfiguration-1.4.0b1/azure/appconfiguration/aio/__init__.py` & `azure-appconfiguration-1.5.0b1/azure/appconfiguration/aio/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,10 +5,10 @@
 # license information.
 #
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is
 # regenerated.
 # --------------------------------------------------------------------------
 
-from ._azure_configuration_client_async import AzureAppConfigurationClient
+from ._azure_appconfiguration_client_async import AzureAppConfigurationClient
 
 __all__ = ["AzureAppConfigurationClient"]
```

## Comparing `azure-appconfiguration-1.4.0b1/tests/test_azure_appconfiguration_client_aad_async.py` & `azure-appconfiguration-1.5.0b1/tests/test_azure_appconfiguration_client_aad_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,17 +56,15 @@
             assert (
                 created_kv.label == kv.label
                 and kv.value == kv.value
                 and created_kv.content_type == kv.content_type
                 and created_kv.tags == kv.tags
             )
             assert (
-                created_kv.etag is not None
-                and created_kv.last_modified is not None
-                and created_kv.read_only is False
+                created_kv.etag is not None and created_kv.last_modified is not None and created_kv.read_only is False
             )
             await client.delete_configuration_setting(key=created_kv.key, label=created_kv.label)
 
     @app_config_aad_decorator_async
     @recorded_by_proxy_async
     async def test_add_existing_configuration_setting(self, appconfiguration_endpoint_string):
         async with self.create_aad_client(appconfiguration_endpoint_string) as client:
@@ -167,17 +165,15 @@
 
     @app_config_aad_decorator_async
     @recorded_by_proxy_async
     async def test_get_configuration_setting_label(self, appconfiguration_endpoint_string):
         async with self.create_aad_client(appconfiguration_endpoint_string) as client:
             compare_kv = self.create_config_setting()
             await self.add_for_test(client, compare_kv)
-            fetched_kv = await client.get_configuration_setting(
-                compare_kv.key, compare_kv.label
-            )
+            fetched_kv = await client.get_configuration_setting(compare_kv.key, compare_kv.label)
             assert (
                 fetched_kv.key == compare_kv.key
                 and fetched_kv.value == compare_kv.value
                 and fetched_kv.content_type == compare_kv.content_type
                 and fetched_kv.tags == compare_kv.tags
             )
             assert fetched_kv.label is not None
@@ -185,17 +181,15 @@
 
     @app_config_aad_decorator_async
     @recorded_by_proxy_async
     async def test_get_non_existing_configuration_setting(self, appconfiguration_endpoint_string):
         async with self.create_aad_client(appconfiguration_endpoint_string) as client:
             compare_kv = self.create_config_setting()
             with pytest.raises(ResourceNotFoundError):
-                await client.get_configuration_setting(
-                    compare_kv.key, compare_kv.label + "a"
-                )
+                await client.get_configuration_setting(compare_kv.key, compare_kv.label + "a")
 
     # method: delete_configuration_setting
     @app_config_aad_decorator_async
     @recorded_by_proxy_async
     async def test_delete_with_key_no_label(self, appconfiguration_endpoint_string):
         async with self.create_aad_client(appconfiguration_endpoint_string) as client:
             to_delete_kv = self.create_config_setting_no_label()
@@ -273,17 +267,17 @@
         assert all(x.key == KEY for x in items)
         await self.tear_down()
 
     @app_config_aad_decorator_async
     @recorded_by_proxy_async
     async def test_list_configuration_settings_fields(self, appconfiguration_endpoint_string):
         await self.set_up(appconfiguration_endpoint_string, is_aad=True)
-        items = await self.convert_to_list(self.client.list_configuration_settings(
-            key_filter="*", label_filter=LABEL, fields=["key", "content_type"]
-        ))
+        items = await self.convert_to_list(
+            self.client.list_configuration_settings(key_filter="*", label_filter=LABEL, fields=["key", "content_type"])
+        )
         assert len(items) == 1
         assert all(x.key and not x.label and x.content_type for x in items)
         await self.tear_down()
 
     @app_config_aad_decorator_async
     @recorded_by_proxy_async
     async def test_list_configuration_settings_reserved_chars(self, appconfiguration_endpoint_string):
@@ -309,17 +303,19 @@
     @app_config_aad_decorator_async
     @recorded_by_proxy_async
     async def test_list_configuration_settings_correct_etag(self, appconfiguration_endpoint_string):
         async with self.create_aad_client(appconfiguration_endpoint_string) as client:
             to_list_kv = self.create_config_setting()
             await self.add_for_test(client, to_list_kv)
             custom_headers = {"If-Match": to_list_kv.etag or ""}
-            items = await self.convert_to_list(client.list_configuration_settings(
-                key_filter=to_list_kv.key, label_filter=to_list_kv.label, headers=custom_headers
-            ))
+            items = await self.convert_to_list(
+                client.list_configuration_settings(
+                    key_filter=to_list_kv.key, label_filter=to_list_kv.label, headers=custom_headers
+                )
+            )
             assert len(items) == 1
             assert all(x.key == to_list_kv.key and x.label == to_list_kv.label for x in items)
             await client.delete_configuration_setting(to_list_kv.key)
 
     @app_config_aad_decorator_async
     @recorded_by_proxy_async
     async def test_list_configuration_settings_multi_pages(self, appconfiguration_endpoint_string):
@@ -361,33 +357,35 @@
         await self.tear_down()
 
     @app_config_aad_decorator_async
     @recorded_by_proxy_async
     async def test_list_configuration_settings_only_accepttime(self, appconfiguration_endpoint_string, **kwargs):
         recorded_variables = kwargs.pop("variables", {})
         await self.set_up(appconfiguration_endpoint_string, is_aad=True)
-        exclude_today = await self.convert_to_list(self.client.list_configuration_settings(
-            accept_datetime=recorded_variables.setdefault(
-                "datetime", str(datetime.datetime.today() + datetime.timedelta(days=-1))
+        exclude_today = await self.convert_to_list(
+            self.client.list_configuration_settings(
+                accept_datetime=recorded_variables.setdefault(
+                    "datetime", str(datetime.datetime.today() + datetime.timedelta(days=-1))
+                )
             )
-        ))
+        )
         all_inclusive = await self.convert_to_list(self.client.list_configuration_settings())
         assert len(all_inclusive) > len(exclude_today)
         await self.tear_down()
         return recorded_variables
 
     # method: list_revisions
     @app_config_aad_decorator_async
     @recorded_by_proxy_async
     async def test_list_revisions_key_label(self, appconfiguration_endpoint_string):
         await self.set_up(appconfiguration_endpoint_string, is_aad=True)
         to_list = self.create_config_setting()
-        items = await self.convert_to_list(self.client.list_revisions(
-            label_filter=to_list.label, key_filter=to_list.key
-        ))
+        items = await self.convert_to_list(
+            self.client.list_revisions(label_filter=to_list.label, key_filter=to_list.key)
+        )
         assert len(items) >= 2
         assert all(x.key == to_list.key and x.label == to_list.label for x in items)
         await self.tear_down()
 
     @app_config_aad_decorator_async
     @recorded_by_proxy_async
     async def test_list_revisions_only_label(self, appconfiguration_endpoint_string):
@@ -406,29 +404,29 @@
         assert all(x.key == KEY for x in items)
         await self.tear_down()
 
     @app_config_aad_decorator_async
     @recorded_by_proxy_async
     async def test_list_revisions_fields(self, appconfiguration_endpoint_string):
         await self.set_up(appconfiguration_endpoint_string, is_aad=True)
-        items = await self.convert_to_list(self.client.list_revisions(
-            key_filter="*", label_filter=LABEL, fields=["key", "content_type"]
-        ))
+        items = await self.convert_to_list(
+            self.client.list_revisions(key_filter="*", label_filter=LABEL, fields=["key", "content_type"])
+        )
         assert all(x.key and not x.label and x.content_type and not x.tags and not x.etag for x in items)
         await self.tear_down()
 
     @app_config_aad_decorator_async
     @recorded_by_proxy_async
     async def test_list_revisions_correct_etag(self, appconfiguration_endpoint_string):
         await self.set_up(appconfiguration_endpoint_string, is_aad=True)
         to_list_kv = self.create_config_setting()
         custom_headers = {"If-Match": to_list_kv.etag or ""}
-        items = await self.convert_to_list(self.client.list_revisions(
-            key_filter=to_list_kv.key, label_filter=to_list_kv.label, headers=custom_headers
-        ))
+        items = await self.convert_to_list(
+            self.client.list_revisions(key_filter=to_list_kv.key, label_filter=to_list_kv.label, headers=custom_headers)
+        )
         assert len(items) >= 1
         assert all(x.key == to_list_kv.key and x.label == to_list_kv.label for x in items)
         await self.tear_down()
 
     @app_config_aad_decorator_async
     @recorded_by_proxy_async
     async def test_read_only(self, appconfiguration_endpoint_string):
@@ -467,20 +465,20 @@
             with pytest.raises(ResourceReadOnlyError):
                 await client.set_configuration_setting(read_only_kv)
             readable_kv = await client.set_read_only(read_only_kv, False)
             readable_kv.value = to_set_kv.value
             readable_kv.tags = to_set_kv.tags
             set_kv = await client.set_configuration_setting(readable_kv)
             assert (
-                    to_set_kv.key == set_kv.key
-                    and to_set_kv.label == to_set_kv.label
-                    and to_set_kv.value == set_kv.value
-                    and to_set_kv.content_type == set_kv.content_type
-                    and to_set_kv.tags == set_kv.tags
-                    and to_set_kv.etag != set_kv.etag
+                to_set_kv.key == set_kv.key
+                and to_set_kv.label == to_set_kv.label
+                and to_set_kv.value == set_kv.value
+                and to_set_kv.content_type == set_kv.content_type
+                and to_set_kv.tags == set_kv.tags
+                and to_set_kv.etag != set_kv.etag
             )
             set_kv.etag = "bad"
             with pytest.raises(ResourceModifiedError):
                 await client.set_read_only(set_kv, True, match_condition=MatchConditions.IfNotModified)
             await client.delete_configuration_setting(to_set_kv.key)
 
     @app_config_aad_decorator_async
@@ -488,100 +486,93 @@
     async def test_sync_tokens_with_configuration_setting(self, appconfiguration_endpoint_string):
         async with self.create_aad_client(appconfiguration_endpoint_string) as client:
             sync_tokens = copy.deepcopy(client._sync_token_policy._sync_tokens)
             sync_token_header = self._order_dict(sync_tokens)
             sync_token_header = ",".join(str(x) for x in sync_token_header.values())
 
             new = ConfigurationSetting(
-                    key="KEY1",
-                    label=None,
-                    value="TEST_VALUE1",
-                    content_type=TEST_CONTENT_TYPE,
-                    tags={"tag1": "tag1", "tag2": "tag2"},
+                key="KEY1",
+                label=None,
+                value="TEST_VALUE1",
+                content_type=TEST_CONTENT_TYPE,
+                tags={"tag1": "tag1", "tag2": "tag2"},
             )
 
             await client.set_configuration_setting(new)
             sync_tokens2 = copy.deepcopy(client._sync_token_policy._sync_tokens)
             sync_token_header2 = self._order_dict(sync_tokens2)
             sync_token_header2 = ",".join(str(x) for x in sync_token_header2.values())
             assert sync_token_header != sync_token_header2
 
             new = ConfigurationSetting(
-                    key="KEY2",
-                    label=None,
-                    value="TEST_VALUE2",
-                    content_type=TEST_CONTENT_TYPE,
-                    tags={"tag1": "tag1", "tag2": "tag2"},
+                key="KEY2",
+                label=None,
+                value="TEST_VALUE2",
+                content_type=TEST_CONTENT_TYPE,
+                tags={"tag1": "tag1", "tag2": "tag2"},
             )
 
             await client.set_configuration_setting(new)
             sync_tokens3 = copy.deepcopy(client._sync_token_policy._sync_tokens)
             sync_token_header3 = self._order_dict(sync_tokens3)
             sync_token_header3 = ",".join(str(x) for x in sync_token_header3.values())
             assert sync_token_header2 != sync_token_header3
-            
+
             await client.delete_configuration_setting(new.key)
 
     @app_config_aad_decorator_async
     @recorded_by_proxy_async
     async def test_sync_tokens_with_feature_flag_configuration_setting(self, appconfiguration_endpoint_string):
         await self.set_up(appconfiguration_endpoint_string, is_aad=True)
         new = FeatureFlagConfigurationSetting(
-            'custom',
+            "custom",
             enabled=True,
-            filters = [
+            filters=[
                 {
                     "name": "Microsoft.Percentage",
                     "parameters": {
                         "Value": 10,
                         "User": "user1",
-                    }
+                    },
                 }
-            ]
+            ],
         )
 
         sync_tokens = copy.deepcopy(self.client._sync_token_policy._sync_tokens)
         keys = list(sync_tokens.keys())
         seq_num = sync_tokens[keys[0]].sequence_number
         await self.client.set_configuration_setting(new)
 
         new = FeatureFlagConfigurationSetting(
-            'time_window',
+            "time_window",
             enabled=True,
-            filters = [
+            filters=[
                 {
-                    u"name": FILTER_TIME_WINDOW,
-                    u"parameters": {
-                        "Start": "Wed, 10 Mar 2021 05:00:00 GMT",
-                        "End": "Fri, 02 Apr 2021 04:00:00 GMT"
-                    }
+                    "name": FILTER_TIME_WINDOW,
+                    "parameters": {"Start": "Wed, 10 Mar 2021 05:00:00 GMT", "End": "Fri, 02 Apr 2021 04:00:00 GMT"},
                 },
-            ]
+            ],
         )
 
         await self.client.set_configuration_setting(new)
         sync_tokens2 = copy.deepcopy(self.client._sync_token_policy._sync_tokens)
         keys = list(sync_tokens2.keys())
         seq_num2 = sync_tokens2[keys[0]].sequence_number
 
         new = FeatureFlagConfigurationSetting(
             "newflag",
             enabled=True,
             filters=[
                 {
                     "name": FILTER_TARGETING,
                     "parameters": {
-                        u"Audience": {
-                            u"Users": [u"abc", u"def"],
-                            u"Groups": [u"ghi", u"jkl"],
-                            u"DefaultRolloutPercentage": 75
-                        }
-                    }
+                        "Audience": {"Users": ["abc", "def"], "Groups": ["ghi", "jkl"], "DefaultRolloutPercentage": 75}
+                    },
                 },
-            ]
+            ],
         )
 
         await self.client.set_configuration_setting(new)
         sync_tokens3 = copy.deepcopy(self.client._sync_token_policy._sync_tokens)
         keys = list(sync_tokens3.keys())
         seq_num3 = sync_tokens3[keys[0]].sequence_number
 
@@ -601,52 +592,53 @@
             self._assert_same_keys(feature_flag, set_flag)
 
             set_flag.enabled = not set_flag.enabled
             changed_flag = await client.set_configuration_setting(set_flag)
 
             changed_flag.enabled = False
             temp = json.loads(changed_flag.value)
-            assert temp['enabled'] == False
+            assert temp["enabled"] == False
 
             c = json.loads(copy.deepcopy(changed_flag.value))
-            c['enabled'] = True
+            c["enabled"] = True
             changed_flag.value = json.dumps(c)
             assert changed_flag.enabled == True
 
             changed_flag.value = json.dumps({})
             assert changed_flag.enabled == None
-            assert changed_flag.value == json.dumps({'enabled': None, "conditions": {"client_filters": None}})
+            assert changed_flag.value == json.dumps({"enabled": None, "conditions": {"client_filters": None}})
 
             set_flag.value = "bad_value"
             assert set_flag.enabled == None
             assert set_flag.filters == None
 
             await client.delete_configuration_setting(changed_flag.key)
 
     @app_config_aad_decorator_async
     @recorded_by_proxy_async
     async def test_config_setting_secret_reference(self, appconfiguration_endpoint_string):
-        async with  self.create_aad_client(appconfiguration_endpoint_string) as client:
+        async with self.create_aad_client(appconfiguration_endpoint_string) as client:
             secret_reference = SecretReferenceConfigurationSetting(
-                "ConnectionString", "https://test-test.vault.azure.net/secrets/connectionString")
+                "ConnectionString", "https://test-test.vault.azure.net/secrets/connectionString"
+            )
             set_flag = await client.set_configuration_setting(secret_reference)
             self._assert_same_keys(secret_reference, set_flag)
 
             set_flag.secret_id = "https://test-test.vault.azure.net/new_secrets/connectionString"
             updated_flag = await client.set_configuration_setting(set_flag)
             self._assert_same_keys(set_flag, updated_flag)
 
             assert isinstance(updated_flag, SecretReferenceConfigurationSetting)
             new_uri = "https://aka.ms/azsdk"
             new_uri2 = "https://aka.ms/azsdk/python"
             updated_flag.secret_id = new_uri
             temp = json.loads(updated_flag.value)
-            assert temp['uri'] == new_uri
+            assert temp["uri"] == new_uri
 
-            updated_flag.value = json.dumps({'uri': new_uri2})
+            updated_flag.value = json.dumps({"uri": new_uri2})
             assert updated_flag.secret_id == new_uri2
 
             set_flag.value = "bad_value"
             assert set_flag.secret_id == None
 
             await client.delete_configuration_setting(secret_reference.key)
 
@@ -657,22 +649,22 @@
             new = FeatureFlagConfigurationSetting(
                 "newflag",
                 enabled=True,
                 filters=[
                     {
                         "name": FILTER_TARGETING,
                         "parameters": {
-                            u"Audience": {
-                                u"Users": [u"abc", u"def"],
-                                u"Groups": [u"ghi", u"jkl"],
-                                u"DefaultRolloutPercentage": 75
+                            "Audience": {
+                                "Users": ["abc", "def"],
+                                "Groups": ["ghi", "jkl"],
+                                "DefaultRolloutPercentage": 75,
                             }
-                        }
+                        },
                     }
-                ]
+                ],
             )
 
             sent_config = await client.set_configuration_setting(new)
             self._assert_same_keys(sent_config, new)
 
             assert isinstance(sent_config.filters[0], dict)
             assert len(sent_config.filters) == 1
@@ -681,56 +673,56 @@
             updated_sent_config = await client.set_configuration_setting(sent_config)
             self._assert_same_keys(sent_config, updated_sent_config)
 
             updated_sent_config.filters.append(
                 {
                     "name": FILTER_TARGETING,
                     "parameters": {
-                        u"Audience": {
-                            u"Users": [u"abcd", u"defg"], # cspell:disable-line
-                            u"Groups": [u"ghij", u"jklm"], # cspell:disable-line
-                            u"DefaultRolloutPercentage": 50
+                        "Audience": {
+                            "Users": ["abcd", "defg"],  # cspell:disable-line
+                            "Groups": ["ghij", "jklm"],  # cspell:disable-line
+                            "DefaultRolloutPercentage": 50,
                         }
-                    }
+                    },
                 }
             )
             updated_sent_config.filters.append(
                 {
                     "name": FILTER_TARGETING,
                     "parameters": {
-                        u"Audience": {
-                            u"Users": [u"abcde", u"defgh"], # cspell:disable-line
-                            u"Groups": [u"ghijk", u"jklmn"], # cspell:disable-line
-                            u"DefaultRolloutPercentage": 100
+                        "Audience": {
+                            "Users": ["abcde", "defgh"],  # cspell:disable-line
+                            "Groups": ["ghijk", "jklmn"],  # cspell:disable-line
+                            "DefaultRolloutPercentage": 100,
                         }
-                    }
+                    },
                 }
             )
             sent_config = await client.set_configuration_setting(updated_sent_config)
             self._assert_same_keys(sent_config, updated_sent_config)
             assert len(sent_config.filters) == 3
 
             await client.delete_configuration_setting(updated_sent_config.key)
 
     @app_config_aad_decorator_async
     @recorded_by_proxy_async
     async def test_feature_filter_time_window(self, appconfiguration_endpoint_string):
         async with self.create_aad_client(appconfiguration_endpoint_string) as client:
             new = FeatureFlagConfigurationSetting(
-                'time_window',
+                "time_window",
                 enabled=True,
                 filters=[
                     {
                         "name": FILTER_TIME_WINDOW,
                         "parameters": {
                             "Start": "Wed, 10 Mar 2021 05:00:00 GMT",
-                            "End": "Fri, 02 Apr 2021 04:00:00 GMT"
-                        }
+                            "End": "Fri, 02 Apr 2021 04:00:00 GMT",
+                        },
                     }
-                ]
+                ],
             )
 
             sent = await client.set_configuration_setting(new)
             self._assert_same_keys(sent, new)
 
             sent.filters[0]["parameters"]["Start"] = "Thurs, 11 Mar 2021 05:00:00 GMT"
             new_sent = await client.set_configuration_setting(sent)
@@ -739,25 +731,17 @@
             await client.delete_configuration_setting(new_sent.key)
 
     @app_config_aad_decorator_async
     @recorded_by_proxy_async
     async def test_feature_filter_custom(self, appconfiguration_endpoint_string):
         async with self.create_aad_client(appconfiguration_endpoint_string) as client:
             new = FeatureFlagConfigurationSetting(
-                'custom',
+                "custom",
                 enabled=True,
-                filters=[
-                    {
-                        "name": FILTER_PERCENTAGE,
-                        "parameters": {
-                            "Value": 10,
-                            "User": "user1"
-                        }
-                    }
-                ]
+                filters=[{"name": FILTER_PERCENTAGE, "parameters": {"Value": 10, "User": "user1"}}],
             )
 
             sent = await client.set_configuration_setting(new)
             self._assert_same_keys(sent, new)
 
             sent.filters[0]["parameters"]["Value"] = 100
             new_sent = await client.set_configuration_setting(sent)
@@ -766,41 +750,36 @@
             await client.delete_configuration_setting(new_sent.key)
 
     @app_config_aad_decorator_async
     @recorded_by_proxy_async
     async def test_feature_filter_multiple(self, appconfiguration_endpoint_string):
         async with self.create_aad_client(appconfiguration_endpoint_string) as client:
             new = FeatureFlagConfigurationSetting(
-                'custom',
+                "custom",
                 enabled=True,
                 filters=[
-                    {
-                        "name": FILTER_PERCENTAGE,
-                        "parameters": {
-                            "Value": 10
-                        }
-                    },
+                    {"name": FILTER_PERCENTAGE, "parameters": {"Value": 10}},
                     {
                         "name": FILTER_TIME_WINDOW,
                         "parameters": {
                             "Start": "Wed, 10 Mar 2021 05:00:00 GMT",
-                            "End": "Fri, 02 Apr 2021 04:00:00 GMT"
-                        }
+                            "End": "Fri, 02 Apr 2021 04:00:00 GMT",
+                        },
                     },
                     {
                         "name": FILTER_TARGETING,
                         "parameters": {
-                            u"Audience": {
-                                u"Users": [u"abcde", u"defgh"], # cspell:disable-line
-                                u"Groups": [u"ghijk", u"jklmn"], # cspell:disable-line
-                                u"DefaultRolloutPercentage": 100
+                            "Audience": {
+                                "Users": ["abcde", "defgh"],  # cspell:disable-line
+                                "Groups": ["ghijk", "jklmn"],  # cspell:disable-line
+                                "DefaultRolloutPercentage": 100,
                             }
-                        }
-                    }
-                ]
+                        },
+                    },
+                ],
             )
 
             sent = await client.set_configuration_setting(new)
             self._assert_same_keys(sent, new)
 
             sent.filters[0]["parameters"]["Value"] = 100
             sent.filters[1]["parameters"]["Start"] = "Wed, 10 Mar 2021 08:00:00 GMT"
```

## Comparing `azure-appconfiguration-1.4.0b1/tests/preparers.py` & `azure-appconfiguration-1.5.0b1/tests/preparers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,57 +1,58 @@
-
 # coding: utf-8
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 from devtools_testutils import PowerShellPreparer
 import functools
 import inspect
 
 AppConfigPreparer = functools.partial(
     PowerShellPreparer,
-    'appconfiguration',
+    "appconfiguration",
     appconfiguration_connection_string="Endpoint=https://fake_app_config.azconfig-test.io;Id=0-l4-s0:h5htBaY5Z1LwFz50bIQv;Secret=lamefakesecretlamefakesecretlamefakesecrett=",
     appconfiguration_endpoint_string="https://fake_app_config.azconfig-test.io",
 )
 
 
 def trim_kwargs_from_test_function(fn, kwargs):
     # the next function is the actual test function. the kwargs need to be trimmed so
     # that parameters which are not required will not be passed to it.
-    if not getattr(fn, '__is_preparer', False):
+    if not getattr(fn, "__is_preparer", False):
         try:
             args, _, kw, _, _, _, _ = inspect.getfullargspec(fn)
         except AttributeError:
-            args, _, kw, _ = inspect.getargspec(fn) # pylint: disable=deprecated-method
+            args, _, kw, _ = inspect.getargspec(fn)  # pylint: disable=deprecated-method
         if kw is None:
             args = set(args)
             for key in [k for k in kwargs if k not in args]:
                 del kwargs[key]
 
+
 def app_config_decorator(func, **kwargs):
     @AppConfigPreparer()
     def wrapper(*args, **kwargs):
         appconfiguration_connection_string = kwargs.pop("appconfiguration_connection_string")
-        kwargs['appconfiguration_connection_string'] = appconfiguration_connection_string
+        kwargs["appconfiguration_connection_string"] = appconfiguration_connection_string
 
-        trimmed_kwargs = {k:v for k, v in kwargs.items()}
+        trimmed_kwargs = {k: v for k, v in kwargs.items()}
         trim_kwargs_from_test_function(func, trimmed_kwargs)
 
         func(*args, **trimmed_kwargs)
 
     return wrapper
 
+
 def app_config_aad_decorator(func, **kwargs):
     @AppConfigPreparer()
     def wrapper(*args, **kwargs):
         appconfiguration_endpoint_string = kwargs.pop("appconfiguration_endpoint_string")
-        kwargs['appconfiguration_endpoint_string'] = appconfiguration_endpoint_string
+        kwargs["appconfiguration_endpoint_string"] = appconfiguration_endpoint_string
 
-        trimmed_kwargs = {k:v for k, v in kwargs.items()}
+        trimmed_kwargs = {k: v for k, v in kwargs.items()}
         trim_kwargs_from_test_function(func, trimmed_kwargs)
 
         func(*args, **trimmed_kwargs)
 
     return wrapper
```

## Comparing `azure-appconfiguration-1.4.0b1/tests/test_consistency.py` & `azure-appconfiguration-1.5.0b1/tests/test_consistency.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,50 +17,36 @@
 class TestAppConfigurationConsistency(AppConfigTestCase):
     @app_config_decorator
     @recorded_by_proxy
     def test_update_json_by_value(self, appconfiguration_connection_string):
         client = self.create_client(appconfiguration_connection_string)
         key = self.get_resource_name("key")
         feature_flag = FeatureFlagConfigurationSetting(
-            key,
-            enabled=True,
-            filters=[
-                {
-                    "name": FILTER_PERCENTAGE,
-                    "parameters": {
-                        "Value": 10,
-                        "User": "user1"
-                    }
-                }
-            ]
+            key, enabled=True, filters=[{"name": FILTER_PERCENTAGE, "parameters": {"Value": 10, "User": "user1"}}]
         )
         set_flag = client.set_configuration_setting(feature_flag)
 
-        set_flag.value = json.dumps({
-            'conditions': {
-                'client_filters': [
-                    {
-                        'name': 'Microsoft.Targeting',
-                        'parameters': {
-                            'name': 'Microsoft.Targeting',
-                            'parameters': {
-                                'Audience': {
-                                    'DefaultRolloutPercentage': 50,
-                                    'Groups': [],
-                                    'Users': []
-                                }
-                            }
+        set_flag.value = json.dumps(
+            {
+                "conditions": {
+                    "client_filters": [
+                        {
+                            "name": "Microsoft.Targeting",
+                            "parameters": {
+                                "name": "Microsoft.Targeting",
+                                "parameters": {"Audience": {"DefaultRolloutPercentage": 50, "Groups": [], "Users": []}},
+                            },
                         }
-                    }
-                ]
-            },
-            'description': '',
-            'enabled': False,
-            'id': key,
-        })
+                    ]
+                },
+                "description": "",
+                "enabled": False,
+                "id": key,
+            }
+        )
 
         set_flag = client.set_configuration_setting(set_flag)
         assert isinstance(set_flag, FeatureFlagConfigurationSetting)
         assert set_flag.enabled == False
         assert set_flag.key.endswith(key)
 
         client.delete_configuration_setting(set_flag)
@@ -107,49 +93,24 @@
         client.delete_configuration_setting(feature_flag)
 
 
 class TestAppConfigurationConsistencyUnitTest(AppConfigTestCase):
     def test_feature_flag_set_value(self):
         key = self.get_resource_name("key")
         feature_flag = FeatureFlagConfigurationSetting(
-            key,
-            enabled=True,
-            filters=[
-                {
-                    "name": FILTER_PERCENTAGE,
-                    "parameters": {
-                        "Value": 10,
-                        "User": "user1"
-                    }
-                }
-            ]
+            key, enabled=True, filters=[{"name": FILTER_PERCENTAGE, "parameters": {"Value": 10, "User": "user1"}}]
         )
-        feature_flag.value = json.dumps({
-            "conditions": {
-                "client_filters": []
-            },
-            "enabled": False
-        })
+        feature_flag.value = json.dumps({"conditions": {"client_filters": []}, "enabled": False})
 
         assert feature_flag.enabled == False
 
     def test_feature_flag_set_enabled(self):
         key = self.get_resource_name("key")
         feature_flag = FeatureFlagConfigurationSetting(
-            key,
-            enabled=True,
-            filters=[
-                {
-                    "name": FILTER_PERCENTAGE,
-                    "parameters": {
-                        "Value": 10,
-                        "User": "user1"
-                    }
-                }
-            ]
+            key, enabled=True, filters=[{"name": FILTER_PERCENTAGE, "parameters": {"Value": 10, "User": "user1"}}]
         )
         feature_flag.enabled = False
 
         temp = json.loads(feature_flag.value)
         assert temp["enabled"] == False
 
     def test_feature_flag_prefix(self):
```

## Comparing `azure-appconfiguration-1.4.0b1/tests/test_azure_appconfiguration_client.py` & `azure-appconfiguration-1.5.0b1/tests/test_azure_appconfiguration_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     ResourceNotFoundError,
     ResourceExistsError,
 )
 from azure.appconfiguration import (
     ResourceReadOnlyError,
     AzureAppConfigurationClient,
     ConfigurationSetting,
+    ConfigurationSettingFilter,
     FeatureFlagConfigurationSetting,
     SecretReferenceConfigurationSetting,
     FILTER_PERCENTAGE,
     FILTER_TARGETING,
     FILTER_TIME_WINDOW,
 )
 from testcase import AppConfigTestCase
@@ -31,15 +32,14 @@
     LABEL,
     TEST_VALUE,
     TEST_CONTENT_TYPE,
     LABEL_RESERVED_CHARS,
     PAGE_SIZE,
     KEY_UUID,
 )
-from typing import Any
 from uuid import uuid4
 from preparers import app_config_decorator
 from devtools_testutils import recorded_by_proxy
 
 
 class TestAppConfigurationClient(AppConfigTestCase):
     # method: add_configuration_setting
@@ -57,19 +57,15 @@
         created_kv = client.add_configuration_setting(kv)
         assert (
             created_kv.label == kv.label
             and kv.value == kv.value
             and created_kv.content_type == kv.content_type
             and created_kv.tags == kv.tags
         )
-        assert (
-            created_kv.etag is not None
-            and created_kv.last_modified is not None
-            and created_kv.read_only is False
-        )
+        assert created_kv.etag is not None and created_kv.last_modified is not None and created_kv.read_only is False
         client.delete_configuration_setting(key=created_kv.key, label=created_kv.label)
 
     @app_config_decorator
     @recorded_by_proxy
     def test_add_existing_configuration_setting(self, appconfiguration_connection_string):
         client = self.create_client(appconfiguration_connection_string)
         test_config_setting = self.create_config_setting()
@@ -82,15 +78,15 @@
                 )
             )
         client.delete_configuration_setting(key=test_config_setting.key, label=test_config_setting.label)
 
     # method: set_configuration_setting
     @app_config_decorator
     @recorded_by_proxy
-    def test_set_existing_configuration_setting_label_etag(self,  appconfiguration_connection_string):
+    def test_set_existing_configuration_setting_label_etag(self, appconfiguration_connection_string):
         client = self.create_client(appconfiguration_connection_string)
         to_set_kv = self.create_config_setting()
         to_set_kv.value = to_set_kv.value + "a"
         to_set_kv.tags = {"a": "b", "c": "d"}
         set_kv = client.set_configuration_setting(to_set_kv)
         assert (
             to_set_kv.key == set_kv.key
@@ -169,17 +165,15 @@
 
     @app_config_decorator
     @recorded_by_proxy
     def test_get_configuration_setting_label(self, appconfiguration_connection_string):
         client = self.create_client(appconfiguration_connection_string)
         compare_kv = self.create_config_setting()
         self.add_for_test(client, compare_kv)
-        fetched_kv = client.get_configuration_setting(
-            compare_kv.key, compare_kv.label
-        )
+        fetched_kv = client.get_configuration_setting(compare_kv.key, compare_kv.label)
         assert (
             fetched_kv.key == compare_kv.key
             and fetched_kv.value == compare_kv.value
             and fetched_kv.content_type == compare_kv.content_type
             and fetched_kv.tags == compare_kv.tags
             and fetched_kv.label == compare_kv.label
         )
@@ -277,17 +271,17 @@
         assert all(x.key == KEY for x in items)
         self.tear_down()
 
     @app_config_decorator
     @recorded_by_proxy
     def test_list_configuration_settings_fields(self, appconfiguration_connection_string):
         self.set_up(appconfiguration_connection_string)
-        items = list(self.client.list_configuration_settings(
-            key_filter="*", label_filter=LABEL, fields=["key", "content_type"]
-        ))
+        items = list(
+            self.client.list_configuration_settings(key_filter="*", label_filter=LABEL, fields=["key", "content_type"])
+        )
         assert len(items) == 1
         assert all(x.key and not x.label and x.content_type for x in items)
         self.tear_down()
 
     @app_config_decorator
     @recorded_by_proxy
     def test_list_configuration_settings_reserved_chars(self, appconfiguration_connection_string):
@@ -310,19 +304,21 @@
         self.tear_down()
 
     @app_config_decorator
     @recorded_by_proxy
     def test_list_configuration_settings_correct_etag(self, appconfiguration_connection_string):
         client = self.create_client(appconfiguration_connection_string)
         to_list_kv = self.create_config_setting()
-        to_list_kv = self.add_for_test(client, to_list_kv)
+        self.add_for_test(client, to_list_kv)
         custom_headers = {"If-Match": to_list_kv.etag}
-        items = list(client.list_configuration_settings(
-            key_filter=to_list_kv.key, label_filter=to_list_kv.label, headers=custom_headers
-        ))
+        items = list(
+            client.list_configuration_settings(
+                key_filter=to_list_kv.key, label_filter=to_list_kv.label, headers=custom_headers
+            )
+        )
         assert len(items) == 1
         assert all(x.key == to_list_kv.key and x.label == to_list_kv.label for x in items)
         client.delete_configuration_setting(to_list_kv.key)
 
     @app_config_decorator
     @recorded_by_proxy
     def test_list_configuration_settings_multi_pages(self, appconfiguration_connection_string):
@@ -339,21 +335,19 @@
                 )
                 for i in range(PAGE_SIZE + 1)
             ]
         except ResourceExistsError:
             pass
         items = client.list_configuration_settings(key_filter="multi_*")
         assert len(list(items)) > PAGE_SIZE
-        
+
         # Remove the configuration settings
         try:
             [
-                client.delete_configuration_setting(
-                    key="multi_" + str(i) + KEY_UUID, label="multi_label_" + str(i)
-                )
+                client.delete_configuration_setting(key="multi_" + str(i) + KEY_UUID, label="multi_label_" + str(i))
                 for i in range(PAGE_SIZE + 1)
             ]
         except AzureError:
             pass
 
     @app_config_decorator
     @recorded_by_proxy
@@ -363,23 +357,26 @@
         assert len(list(items)) > 0
         self.tear_down()
 
     @app_config_decorator
     @recorded_by_proxy
     def test_list_configuration_settings_only_accepttime(self, appconfiguration_connection_string, **kwargs):
         recorded_variables = kwargs.pop("variables", {})
-        self.set_up(appconfiguration_connection_string)
-        exclude_today = self.client.list_configuration_settings(
-            accept_datetime=recorded_variables.setdefault(
-                "datetime", str(datetime.datetime.today() + datetime.timedelta(days=-1))
-            )
-        )
-        all_inclusive = self.client.list_configuration_settings()
-        assert len(list(all_inclusive)) > len(list(exclude_today))
-        self.tear_down()
+        recorded_variables.setdefault("timestamp", str(datetime.datetime.utcnow()))
+
+        with self.create_client(appconfiguration_connection_string) as client:
+            # Confirm all configuration settings are cleaned up
+            current_config_settings = client.list_configuration_settings()
+            if len(list(current_config_settings)) != 0:
+                for config_setting in current_config_settings:
+                    client.delete_configuration_setting(config_setting)
+
+            revision = client.list_configuration_settings(accept_datetime=recorded_variables.get("timestamp"))
+            assert len(list(revision)) >= 0
+
         return recorded_variables
 
     # method: list_revisions
     @app_config_decorator
     @recorded_by_proxy
     def test_list_revisions_key_label(self, appconfiguration_connection_string):
         self.set_up(appconfiguration_connection_string)
@@ -416,19 +413,19 @@
         self.tear_down()
 
     @app_config_decorator
     @recorded_by_proxy
     def test_list_revisions_correct_etag(self, appconfiguration_connection_string):
         client = self.create_client(appconfiguration_connection_string)
         to_list_kv = self.create_config_setting()
-        to_list_kv = self.add_for_test(client, to_list_kv)
+        self.add_for_test(client, to_list_kv)
         custom_headers = {"If-Match": to_list_kv.etag}
-        items = list(client.list_revisions(
-            key_filter=to_list_kv.key, label_filter=to_list_kv.label, headers=custom_headers
-        ))
+        items = list(
+            client.list_revisions(key_filter=to_list_kv.key, label_filter=to_list_kv.label, headers=custom_headers)
+        )
         assert len(items) >= 1
         assert all(x.key == to_list_kv.key and x.label == to_list_kv.label for x in items)
         client.delete_configuration_setting(to_list_kv.key)
 
     @app_config_decorator
     @recorded_by_proxy
     def test_read_only(self, appconfiguration_connection_string):
@@ -467,20 +464,20 @@
         with pytest.raises(ResourceReadOnlyError):
             client.set_configuration_setting(read_only_kv)
         readable_kv = client.set_read_only(read_only_kv, False)
         readable_kv.value = to_set_kv.value
         readable_kv.tags = to_set_kv.tags
         set_kv = client.set_configuration_setting(readable_kv)
         assert (
-                to_set_kv.key == set_kv.key
-                and to_set_kv.label == to_set_kv.label
-                and to_set_kv.value == set_kv.value
-                and to_set_kv.content_type == set_kv.content_type
-                and to_set_kv.tags == set_kv.tags
-                and to_set_kv.etag != set_kv.etag
+            to_set_kv.key == set_kv.key
+            and to_set_kv.label == to_set_kv.label
+            and to_set_kv.value == set_kv.value
+            and to_set_kv.content_type == set_kv.content_type
+            and to_set_kv.tags == set_kv.tags
+            and to_set_kv.etag != set_kv.etag
         )
         set_kv.etag = "bad"
         with pytest.raises(ResourceModifiedError):
             client.set_read_only(set_kv, True, match_condition=MatchConditions.IfNotModified)
         client.delete_configuration_setting(to_set_kv.key)
 
     @app_config_decorator
@@ -488,100 +485,93 @@
     def test_sync_tokens_with_configuration_setting(self, appconfiguration_connection_string):
         client = self.create_client(appconfiguration_connection_string)
         sync_tokens = copy.deepcopy(client._sync_token_policy._sync_tokens)
         sync_token_header = self._order_dict(sync_tokens)
         sync_token_header = ",".join(str(x) for x in sync_token_header.values())
 
         new = ConfigurationSetting(
-                key="KEY1",
-                label=None,
-                value="TEST_VALUE1",
-                content_type=TEST_CONTENT_TYPE,
-                tags={"tag1": "tag1", "tag2": "tag2"},
+            key="KEY1",
+            label=None,
+            value="TEST_VALUE1",
+            content_type=TEST_CONTENT_TYPE,
+            tags={"tag1": "tag1", "tag2": "tag2"},
         )
 
         client.set_configuration_setting(new)
         sync_tokens2 = copy.deepcopy(client._sync_token_policy._sync_tokens)
         sync_token_header2 = self._order_dict(sync_tokens2)
         sync_token_header2 = ",".join(str(x) for x in sync_token_header2.values())
         assert sync_token_header != sync_token_header2
 
         new = ConfigurationSetting(
-                key="KEY2",
-                label=None,
-                value="TEST_VALUE2",
-                content_type=TEST_CONTENT_TYPE,
-                tags={"tag1": "tag1", "tag2": "tag2"},
+            key="KEY2",
+            label=None,
+            value="TEST_VALUE2",
+            content_type=TEST_CONTENT_TYPE,
+            tags={"tag1": "tag1", "tag2": "tag2"},
         )
 
         client.set_configuration_setting(new)
         sync_tokens3 = copy.deepcopy(client._sync_token_policy._sync_tokens)
         sync_token_header3 = self._order_dict(sync_tokens3)
         sync_token_header3 = ",".join(str(x) for x in sync_token_header3.values())
         assert sync_token_header2 != sync_token_header3
-        
+
         client.delete_configuration_setting(new.key)
 
     @app_config_decorator
     @recorded_by_proxy
     def test_sync_tokens_with_feature_flag_configuration_setting(self, appconfiguration_connection_string):
         self.set_up(appconfiguration_connection_string)
         new = FeatureFlagConfigurationSetting(
-            'custom',
+            "custom",
             enabled=True,
-            filters = [
+            filters=[
                 {
                     "name": "Microsoft.Percentage",
                     "parameters": {
                         "Value": 10,
                         "User": "user1",
-                    }
+                    },
                 }
-            ]
+            ],
         )
 
         sync_tokens = copy.deepcopy(self.client._sync_token_policy._sync_tokens)
         keys = list(sync_tokens.keys())
         seq_num = sync_tokens[keys[0]].sequence_number
         self.client.set_configuration_setting(new)
 
         new = FeatureFlagConfigurationSetting(
-            'time_window',
+            "time_window",
             enabled=True,
-            filters = [
+            filters=[
                 {
-                    u"name": FILTER_TIME_WINDOW,
-                    u"parameters": {
-                        "Start": "Wed, 10 Mar 2021 05:00:00 GMT",
-                        "End": "Fri, 02 Apr 2021 04:00:00 GMT"
-                    }
+                    "name": FILTER_TIME_WINDOW,
+                    "parameters": {"Start": "Wed, 10 Mar 2021 05:00:00 GMT", "End": "Fri, 02 Apr 2021 04:00:00 GMT"},
                 },
-            ]
+            ],
         )
 
         self.client.set_configuration_setting(new)
         sync_tokens2 = copy.deepcopy(self.client._sync_token_policy._sync_tokens)
         keys = list(sync_tokens2.keys())
         seq_num2 = sync_tokens2[keys[0]].sequence_number
 
         new = FeatureFlagConfigurationSetting(
             "newflag",
             enabled=True,
             filters=[
                 {
                     "name": FILTER_TARGETING,
                     "parameters": {
-                        u"Audience": {
-                            u"Users": [u"abc", u"def"],
-                            u"Groups": [u"ghi", u"jkl"],
-                            u"DefaultRolloutPercentage": 75
-                        }
-                    }
+                        "Audience": {"Users": ["abc", "def"], "Groups": ["ghi", "jkl"], "DefaultRolloutPercentage": 75}
+                    },
                 },
-            ]
+            ],
         )
 
         self.client.set_configuration_setting(new)
         sync_tokens3 = copy.deepcopy(self.client._sync_token_policy._sync_tokens)
         keys = list(sync_tokens3.keys())
         seq_num3 = sync_tokens3[keys[0]].sequence_number
 
@@ -600,51 +590,52 @@
         self._assert_same_keys(feature_flag, set_flag)
 
         set_flag.enabled = not set_flag.enabled
         changed_flag = client.set_configuration_setting(set_flag)
 
         changed_flag.enabled = False
         temp = json.loads(changed_flag.value)
-        assert temp['enabled'] == False
+        assert temp["enabled"] == False
 
         c = json.loads(changed_flag.value)
-        c['enabled'] = True
+        c["enabled"] = True
         changed_flag.value = json.dumps(c)
         assert changed_flag.enabled == True
 
         changed_flag.value = json.dumps({})
         assert changed_flag.enabled == None
-        assert changed_flag.value == json.dumps({'enabled': None, "conditions": {"client_filters": None}})
+        assert changed_flag.value == json.dumps({"enabled": None, "conditions": {"client_filters": None}})
 
         set_flag.value = "bad_value"
         assert set_flag.enabled == None
         assert set_flag.filters == None
 
         client.delete_configuration_setting(changed_flag.key)
 
     @app_config_decorator
     @recorded_by_proxy
     def test_config_setting_secret_reference(self, appconfiguration_connection_string):
         client = self.create_client(appconfiguration_connection_string)
         secret_reference = SecretReferenceConfigurationSetting(
-            "ConnectionString", "https://test-test.vault.azure.net/secrets/connectionString")
+            "ConnectionString", "https://test-test.vault.azure.net/secrets/connectionString"
+        )
         set_flag = client.set_configuration_setting(secret_reference)
         self._assert_same_keys(secret_reference, set_flag)
 
         updated_flag = client.set_configuration_setting(set_flag)
         self._assert_same_keys(set_flag, updated_flag)
 
         assert isinstance(updated_flag, SecretReferenceConfigurationSetting)
         new_uri = "https://aka.ms/azsdk"
         new_uri2 = "https://aka.ms/azsdk/python"
         updated_flag.secret_id = new_uri
         temp = json.loads(updated_flag.value)
-        assert temp['uri'] == new_uri
+        assert temp["uri"] == new_uri
 
-        updated_flag.value = json.dumps({'uri': new_uri2})
+        updated_flag.value = json.dumps({"uri": new_uri2})
         assert updated_flag.secret_id == new_uri2
 
         set_flag.value = "bad_value"
         assert set_flag.secret_id == None
 
         client.delete_configuration_setting(secret_reference.key)
 
@@ -655,22 +646,18 @@
         new = FeatureFlagConfigurationSetting(
             "newflag",
             enabled=True,
             filters=[
                 {
                     "name": FILTER_TARGETING,
                     "parameters": {
-                        u"Audience": {
-                            u"Users": [u"abc", u"def"],
-                            u"Groups": [u"ghi", u"jkl"],
-                            u"DefaultRolloutPercentage": 75
-                        }
-                    }
+                        "Audience": {"Users": ["abc", "def"], "Groups": ["ghi", "jkl"], "DefaultRolloutPercentage": 75}
+                    },
                 }
-            ]
+            ],
         )
 
         sent_config = client.set_configuration_setting(new)
         self._assert_same_keys(sent_config, new)
 
         assert isinstance(sent_config.filters[0], dict)
         assert len(sent_config.filters) == 1
@@ -679,56 +666,53 @@
         updated_sent_config = client.set_configuration_setting(sent_config)
         self._assert_same_keys(sent_config, updated_sent_config)
 
         updated_sent_config.filters.append(
             {
                 "name": FILTER_TARGETING,
                 "parameters": {
-                    u"Audience": {
-                        u"Users": [u"abcd", u"defg"], # cspell:disable-line
-                        u"Groups": [u"ghij", u"jklm"], # cspell:disable-line
-                        u"DefaultRolloutPercentage": 50
+                    "Audience": {
+                        "Users": ["abcd", "defg"],  # cspell:disable-line
+                        "Groups": ["ghij", "jklm"],  # cspell:disable-line
+                        "DefaultRolloutPercentage": 50,
                     }
-                }
+                },
             }
         )
         updated_sent_config.filters.append(
             {
                 "name": FILTER_TARGETING,
                 "parameters": {
-                    u"Audience": {
-                        u"Users": [u"abcde", u"defgh"], # cspell:disable-line
-                        u"Groups": [u"ghijk", u"jklmn"], # cspell:disable-line
-                        u"DefaultRolloutPercentage": 100
+                    "Audience": {
+                        "Users": ["abcde", "defgh"],  # cspell:disable-line
+                        "Groups": ["ghijk", "jklmn"],  # cspell:disable-line
+                        "DefaultRolloutPercentage": 100,
                     }
-                }
+                },
             }
         )
         sent_config = client.set_configuration_setting(updated_sent_config)
         self._assert_same_keys(sent_config, updated_sent_config)
         assert len(sent_config.filters) == 3
 
         client.delete_configuration_setting(updated_sent_config.key)
 
     @app_config_decorator
     @recorded_by_proxy
     def test_feature_filter_time_window(self, appconfiguration_connection_string):
         client = self.create_client(appconfiguration_connection_string)
         new = FeatureFlagConfigurationSetting(
-            'time_window',
+            "time_window",
             enabled=True,
             filters=[
                 {
                     "name": FILTER_TIME_WINDOW,
-                    "parameters": {
-                        "Start": "Wed, 10 Mar 2021 05:00:00 GMT",
-                        "End": "Fri, 02 Apr 2021 04:00:00 GMT"
-                    }
+                    "parameters": {"Start": "Wed, 10 Mar 2021 05:00:00 GMT", "End": "Fri, 02 Apr 2021 04:00:00 GMT"},
                 }
-            ]
+            ],
         )
 
         sent = client.set_configuration_setting(new)
         self._assert_same_keys(sent, new)
 
         sent.filters[0]["parameters"]["Start"] = "Thurs, 11 Mar 2021 05:00:00 GMT"
         new_sent = client.set_configuration_setting(sent)
@@ -737,25 +721,15 @@
         client.delete_configuration_setting(new_sent.key)
 
     @app_config_decorator
     @recorded_by_proxy
     def test_feature_filter_custom(self, appconfiguration_connection_string):
         client = self.create_client(appconfiguration_connection_string)
         new = FeatureFlagConfigurationSetting(
-            'custom',
-            enabled=True,
-            filters=[
-                {
-                    "name": FILTER_PERCENTAGE,
-                    "parameters": {
-                        "Value": 10,
-                        "User": "user1"
-                    }
-                }
-            ]
+            "custom", enabled=True, filters=[{"name": FILTER_PERCENTAGE, "parameters": {"Value": 10, "User": "user1"}}]
         )
 
         sent = client.set_configuration_setting(new)
         self._assert_same_keys(sent, new)
 
         sent.filters[0]["parameters"]["Value"] = 100
         new_sent = client.set_configuration_setting(sent)
@@ -764,41 +738,33 @@
         client.delete_configuration_setting(new_sent.key)
 
     @app_config_decorator
     @recorded_by_proxy
     def test_feature_filter_multiple(self, appconfiguration_connection_string):
         client = self.create_client(appconfiguration_connection_string)
         new = FeatureFlagConfigurationSetting(
-            'custom',
+            "custom",
             enabled=True,
             filters=[
-                {
-                    "name": FILTER_PERCENTAGE,
-                    "parameters": {
-                        "Value": 10
-                    }
-                },
+                {"name": FILTER_PERCENTAGE, "parameters": {"Value": 10}},
                 {
                     "name": FILTER_TIME_WINDOW,
-                    "parameters": {
-                        "Start": "Wed, 10 Mar 2021 05:00:00 GMT",
-                        "End": "Fri, 02 Apr 2021 04:00:00 GMT"
-                    }
+                    "parameters": {"Start": "Wed, 10 Mar 2021 05:00:00 GMT", "End": "Fri, 02 Apr 2021 04:00:00 GMT"},
                 },
                 {
                     "name": FILTER_TARGETING,
                     "parameters": {
-                        u"Audience": {
-                            u"Users": [u"abcde", u"defgh"], # cspell:disable-line
-                            u"Groups": [u"ghijk", u"jklmn"], # cspell:disable-line
-                            u"DefaultRolloutPercentage": 100
+                        "Audience": {
+                            "Users": ["abcde", "defgh"],  # cspell:disable-line
+                            "Groups": ["ghijk", "jklmn"],  # cspell:disable-line
+                            "DefaultRolloutPercentage": 100,
                         }
-                    }
-                }
-            ]
+                    },
+                },
+            ],
         )
 
         sent = client.set_configuration_setting(new)
         self._assert_same_keys(sent, new)
 
         sent.filters[0]["parameters"]["Value"] = 100
         sent.filters[1]["parameters"]["Start"] = "Wed, 10 Mar 2021 08:00:00 GMT"
@@ -814,188 +780,228 @@
         client.delete_configuration_setting(new_sent.key)
 
     @app_config_decorator
     @recorded_by_proxy
     def test_breaking_with_feature_flag_configuration_setting(self, appconfiguration_connection_string):
         client = self.create_client(appconfiguration_connection_string)
         new = FeatureFlagConfigurationSetting(
-            'breaking1',
+            "breaking1",
             enabled=True,
             filters=[
                 {
                     "name": FILTER_TIME_WINDOW,
                     "parameters": {
-                        "Start": "bababooey, 31 Mar 2021 25:00:00 GMT", # cspell:disable-line
-                        "End": "Fri, 02 Apr 2021 04:00:00 GMT"
-                    }
+                        "Start": "bababooey, 31 Mar 2021 25:00:00 GMT",  # cspell:disable-line
+                        "End": "Fri, 02 Apr 2021 04:00:00 GMT",
+                    },
                 },
-            ]
+            ],
         )
         client.set_configuration_setting(new)
         client.get_configuration_setting(new.key)
 
         new = FeatureFlagConfigurationSetting(
-            'breaking2',
+            "breaking2",
             enabled=True,
             filters=[
                 {
                     "name": FILTER_TIME_WINDOW,
                     "parameters": {
-                        "Start": "bababooey, 31 Mar 2021 25:00:00 GMT", # cspell:disable-line
-                        "End": "not even trying to be a date"
-                    }
+                        "Start": "bababooey, 31 Mar 2021 25:00:00 GMT",  # cspell:disable-line
+                        "End": "not even trying to be a date",
+                    },
                 },
-            ]
+            ],
         )
         client.set_configuration_setting(new)
         client.get_configuration_setting(new.key)
 
         # This will show up as a Custom filter
         new = FeatureFlagConfigurationSetting(
-            'breaking3',
+            "breaking3",
             enabled=True,
             filters=[
                 {
                     "name": FILTER_TIME_WINDOW,
                     "parameters": {
-                        "Start": "bababooey, 31 Mar 2021 25:00:00 GMT", # cspell:disable-line
-                        "End": "not even trying to be a date"
-                    }
+                        "Start": "bababooey, 31 Mar 2021 25:00:00 GMT",  # cspell:disable-line
+                        "End": "not even trying to be a date",
+                    },
                 },
-            ]
+            ],
         )
         client.set_configuration_setting(new)
         client.get_configuration_setting(new.key)
 
         new = FeatureFlagConfigurationSetting(
-            'breaking4',
+            "breaking4",
             enabled=True,
             filters=[
-                {
-                    "name": FILTER_TIME_WINDOW,
-                    "parameters": "stringystring"
-                },
-            ]
+                {"name": FILTER_TIME_WINDOW, "parameters": "stringystring"},
+            ],
         )
         client.set_configuration_setting(new)
         client.get_configuration_setting(new.key)
 
         new = FeatureFlagConfigurationSetting(
-            'breaking5',
+            "breaking5",
             enabled=True,
-            filters=[
-                {
-                    "name": FILTER_TARGETING,
-                    "parameters": {
-                        u"Audience": {
-                            u"Users": '123'
-                        }
-                    }
-                }
-            ]
+            filters=[{"name": FILTER_TARGETING, "parameters": {"Audience": {"Users": "123"}}}],
         )
         client.set_configuration_setting(new)
         client.get_configuration_setting(new.key)
 
         new = FeatureFlagConfigurationSetting(
-            'breaking6',
-            enabled=True,
-            filters=[
-                {
-                    "name": FILTER_TARGETING,
-                    "parameters": "invalidformat"
-                }
-            ]
+            "breaking6", enabled=True, filters=[{"name": FILTER_TARGETING, "parameters": "invalidformat"}]
         )
         client.set_configuration_setting(new)
         client.get_configuration_setting(new.key)
 
-        new = FeatureFlagConfigurationSetting(
-            'breaking7',
-            enabled=True,
-            filters=[
-                {
-                    'abc': 'def'
-                }
-            ]
-        )
+        new = FeatureFlagConfigurationSetting("breaking7", enabled=True, filters=[{"abc": "def"}])
         client.set_configuration_setting(new)
         client.get_configuration_setting(new.key)
 
-        new = FeatureFlagConfigurationSetting(
-            'breaking8',
-            enabled=True,
-            filters=[
-                {
-                    'abc': 'def'
-                }
-            ]
-        )
-        new.feature_flag_content_type = "fakeyfakey" # cspell:disable-line
+        new = FeatureFlagConfigurationSetting("breaking8", enabled=True, filters=[{"abc": "def"}])
+        new.feature_flag_content_type = "fakeyfakey"  # cspell:disable-line
         client.set_configuration_setting(new)
         client.get_configuration_setting(new.key)
 
         client.delete_configuration_setting(new.key)
 
     @app_config_decorator
     @recorded_by_proxy
     def test_breaking_with_secret_reference_configuration_setting(self, appconfiguration_connection_string):
         client = self.create_client(appconfiguration_connection_string)
-        new = SecretReferenceConfigurationSetting(
-            "aref", # cspell:disable-line
-            "notaurl"
-        )
+        new = SecretReferenceConfigurationSetting("aref", "notaurl")  # cspell:disable-line
         client.set_configuration_setting(new)
         client.get_configuration_setting(new.key)
 
-        new = SecretReferenceConfigurationSetting(
-            "aref1", # cspell:disable-line
-            "notaurl"
-        )
-        new.content_type = "fkaeyjfdkal;" # cspell:disable-line
+        new = SecretReferenceConfigurationSetting("aref1", "notaurl")  # cspell:disable-line
+        new.content_type = "fkaeyjfdkal;"  # cspell:disable-line
         client.set_configuration_setting(new)
         client.get_configuration_setting(new.key)
 
         client.delete_configuration_setting(new.key)
 
+    @app_config_decorator
+    @recorded_by_proxy
+    def test_create_snapshot(self, appconfiguration_connection_string):
+        self.set_up(appconfiguration_connection_string)
+        snapshot_name = self.get_resource_name("snapshot")
+        filters = [ConfigurationSettingFilter(key=KEY, label=LABEL)]
+        response = self.client.begin_create_snapshot(name=snapshot_name, filters=filters)
+        created_snapshot = response.result()
+        assert created_snapshot.name == snapshot_name
+        assert created_snapshot.status == "ready"
+        assert len(created_snapshot.filters) == 1
+        assert created_snapshot.filters[0].key == KEY
+        assert created_snapshot.filters[0].label == LABEL
+
+        received_snapshot = self.client.get_snapshot(name=snapshot_name)
+        self._assert_snapshots(received_snapshot, created_snapshot)
+
+        self.tear_down()
+
+    @app_config_decorator
+    @recorded_by_proxy
+    def test_update_snapshot_status(self, appconfiguration_connection_string):
+        self.set_up(appconfiguration_connection_string)
+        snapshot_name = self.get_resource_name("snapshot")
+        filters = [ConfigurationSettingFilter(key=KEY, label=LABEL)]
+        response = self.client.begin_create_snapshot(name=snapshot_name, filters=filters)
+        created_snapshot = response.result()
+        assert created_snapshot.status == "ready"
+
+        archived_snapshot = self.client.archive_snapshot(name=snapshot_name)
+        assert archived_snapshot.status == "archived"
+
+        recovered_snapshot = self.client.recover_snapshot(name=snapshot_name)
+        assert recovered_snapshot.status == "ready"
+
+        self.tear_down()
+
+    @app_config_decorator
+    @recorded_by_proxy
+    def test_list_snapshots(self, appconfiguration_connection_string):
+        self.set_up(appconfiguration_connection_string)
+
+        result = self.client.list_snapshots()
+        initial_snapshots = len(list(result))
+
+        snapshot_name1 = self.get_resource_name("snapshot1")
+        snapshot_name2 = self.get_resource_name("snapshot2")
+        filters1 = [ConfigurationSettingFilter(key=KEY)]
+        response1 = self.client.begin_create_snapshot(name=snapshot_name1, filters=filters1)
+        created_snapshot1 = response1.result()
+        assert created_snapshot1.status == "ready"
+        filters2 = [ConfigurationSettingFilter(key=KEY, label=LABEL)]
+        response2 = self.client.begin_create_snapshot(name=snapshot_name2, filters=filters2)
+        created_snapshot2 = response2.result()
+        assert created_snapshot2.status == "ready"
+
+        result = self.client.list_snapshots()
+        assert len(list(result)) == initial_snapshots + 2
+
+        self.tear_down()
+
+    @app_config_decorator
+    @recorded_by_proxy
+    def test_list_snapshot_configuration_settings(self, appconfiguration_connection_string):
+        self.set_up(appconfiguration_connection_string)
+        snapshot_name = self.get_resource_name("snapshot")
+        filters = [ConfigurationSettingFilter(key=KEY, label=LABEL)]
+        response = self.client.begin_create_snapshot(name=snapshot_name, filters=filters)
+        created_snapshot = response.result()
+        assert created_snapshot.status == "ready"
+
+        items = self.client.list_snapshot_configuration_settings(snapshot_name)
+        assert len(list(items)) == 1
+
+        self.tear_down()
+
 
 class TestAppConfigurationClientUnitTest:
     def test_type_error(self):
         with pytest.raises(TypeError):
             _ = FeatureFlagConfigurationSetting("blah", key="blah")
         with pytest.raises(TypeError):
             _ = FeatureFlagConfigurationSetting("blah", value="blah")
         with pytest.raises(TypeError):
             _ = SecretReferenceConfigurationSetting("blah", value="blah")
 
     def test_mock_policies(self):
         from azure.core.pipeline.transport import HttpResponse, HttpTransport
         from azure.core.pipeline import PipelineRequest, PipelineResponse
         from consts import APPCONFIGURATION_CONNECTION_STRING
+
         class MockTransport(HttpTransport):
             def __init__(self):
                 self.auth_headers = []
+
             def __exit__(self, exc_type, exc_val, exc_tb):
                 pass
+
             def close(self):
                 pass
+
             def open(self):
                 pass
 
-            def send(self, request: PipelineRequest, **kwargs: Any) -> PipelineResponse:
-                assert request.headers['Authorization'] != self.auth_headers
-                self.auth_headers.append(request.headers['Authorization'])
+            def send(self, request: PipelineRequest, **kwargs) -> PipelineResponse:
+                assert request.headers["Authorization"] != self.auth_headers
+                self.auth_headers.append(request.headers["Authorization"])
                 response = HttpResponse(request, None)
                 response.status_code = 429
                 return response
 
         def new_method(self, request):
             request.http_request.headers["Authorization"] = str(uuid4())
 
         from azure.appconfiguration._azure_appconfiguration_requests import AppConfigRequestsCredentialsPolicy
+
         # Store the method to restore later
         temp = AppConfigRequestsCredentialsPolicy._signed_request
         AppConfigRequestsCredentialsPolicy._signed_request = new_method
 
         client = AzureAppConfigurationClient.from_connection_string(
             APPCONFIGURATION_CONNECTION_STRING, transport=MockTransport()
         )
```

## Comparing `azure-appconfiguration-1.4.0b1/tests/test_azure_appconfiguration_client_aad.py` & `azure-appconfiguration-1.5.0b1/tests/test_azure_appconfiguration_client_aad.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,19 +54,15 @@
         created_kv = client.add_configuration_setting(kv)
         assert (
             created_kv.label == kv.label
             and kv.value == kv.value
             and created_kv.content_type == kv.content_type
             and created_kv.tags == kv.tags
         )
-        assert (
-            created_kv.etag is not None
-            and created_kv.last_modified is not None
-            and created_kv.read_only is False
-        )
+        assert created_kv.etag is not None and created_kv.last_modified is not None and created_kv.read_only is False
         client.delete_configuration_setting(key=created_kv.key, label=created_kv.label)
 
     @app_config_aad_decorator
     @recorded_by_proxy
     def test_add_existing_configuration_setting(self, appconfiguration_endpoint_string):
         client = self.create_aad_client(appconfiguration_endpoint_string)
         test_config_setting = self.create_config_setting()
@@ -166,17 +162,15 @@
 
     @app_config_aad_decorator
     @recorded_by_proxy
     def test_get_configuration_setting_label(self, appconfiguration_endpoint_string):
         client = self.create_aad_client(appconfiguration_endpoint_string)
         compare_kv = self.create_config_setting()
         self.add_for_test(client, compare_kv)
-        fetched_kv = client.get_configuration_setting(
-            compare_kv.key, compare_kv.label
-        )
+        fetched_kv = client.get_configuration_setting(compare_kv.key, compare_kv.label)
         assert (
             fetched_kv.key == compare_kv.key
             and fetched_kv.value == compare_kv.value
             and fetched_kv.content_type == compare_kv.content_type
             and fetched_kv.tags == compare_kv.tags
         )
         assert fetched_kv.label is not None
@@ -246,17 +240,15 @@
         client.delete_configuration_setting(key=to_delete_kv.key, label=to_delete_kv.label)
 
     # method: list_configuration_settings
     @app_config_aad_decorator
     @recorded_by_proxy
     def test_list_configuration_settings_key_label(self, appconfiguration_endpoint_string):
         self.set_up(appconfiguration_endpoint_string, is_aad=True)
-        items = list(self.client.list_configuration_settings(
-            label_filter=LABEL, key_filter=KEY
-        ))
+        items = list(self.client.list_configuration_settings(label_filter=LABEL, key_filter=KEY))
         assert len(items) == 1
         assert all(x.key == KEY and x.label == LABEL for x in items)
         self.tear_down()
 
     @app_config_aad_decorator
     @recorded_by_proxy
     def test_list_configuration_settings_only_label(self, appconfiguration_endpoint_string):
@@ -275,60 +267,54 @@
         assert all(x.key == KEY for x in items)
         self.tear_down()
 
     @app_config_aad_decorator
     @recorded_by_proxy
     def test_list_configuration_settings_fields(self, appconfiguration_endpoint_string):
         self.set_up(appconfiguration_endpoint_string, is_aad=True)
-        items = list(self.client.list_configuration_settings(
-            key_filter="*", label_filter=LABEL, fields=["key", "content_type"]
-        ))
+        items = list(
+            self.client.list_configuration_settings(key_filter="*", label_filter=LABEL, fields=["key", "content_type"])
+        )
         assert len(items) == 1
         assert all(x.key and not x.label and x.content_type for x in items)
         self.tear_down()
 
     @app_config_aad_decorator
     @recorded_by_proxy
     def test_list_configuration_settings_reserved_chars(self, appconfiguration_endpoint_string):
         client = self.create_aad_client(appconfiguration_endpoint_string)
-        reserved_char_kv = ConfigurationSetting(
-            key=KEY, label=LABEL_RESERVED_CHARS, value=TEST_VALUE
-        )
-        reserved_char_kv = client.add_configuration_setting(
-            reserved_char_kv
-        )
+        reserved_char_kv = ConfigurationSetting(key=KEY, label=LABEL_RESERVED_CHARS, value=TEST_VALUE)
+        reserved_char_kv = client.add_configuration_setting(reserved_char_kv)
         escaped_label = re.sub(r"((?!^)\*(?!$)|\\|,)", r"\\\1", LABEL_RESERVED_CHARS)
-        items = list(client.list_configuration_settings(
-            label_filter=escaped_label
-        ))
+        items = list(client.list_configuration_settings(label_filter=escaped_label))
         assert len(items) == 1
         assert all(x.label == LABEL_RESERVED_CHARS for x in items)
         client.delete_configuration_setting(reserved_char_kv.key)
 
     @app_config_aad_decorator
     @recorded_by_proxy
     def test_list_configuration_settings_contains(self, appconfiguration_endpoint_string):
         self.set_up(appconfiguration_endpoint_string, is_aad=True)
-        items = list(self.client.list_configuration_settings(
-            label_filter=LABEL + "*"
-        ))
+        items = list(self.client.list_configuration_settings(label_filter=LABEL + "*"))
         assert len(items) == 1
         assert all(x.label == LABEL for x in items)
         self.tear_down()
 
     @app_config_aad_decorator
     @recorded_by_proxy
     def test_list_configuration_settings_correct_etag(self, appconfiguration_endpoint_string):
         client = self.create_aad_client(appconfiguration_endpoint_string)
         to_list_kv = self.create_config_setting()
-        to_list_kv = self.add_for_test(client, to_list_kv)
+        self.add_for_test(client, to_list_kv)
         custom_headers = {"If-Match": to_list_kv.etag}
-        items = list(client.list_configuration_settings(
-            key_filter=to_list_kv.key, label_filter=to_list_kv.label, headers=custom_headers
-        ))
+        items = list(
+            client.list_configuration_settings(
+                key_filter=to_list_kv.key, label_filter=to_list_kv.label, headers=custom_headers
+            )
+        )
         assert len(items) == 1
         assert all(x.key == to_list_kv.key and x.label == to_list_kv.label for x in items)
         client.delete_configuration_setting(to_list_kv.key)
 
     @app_config_aad_decorator
     @recorded_by_proxy
     def test_list_configuration_settings_multi_pages(self, appconfiguration_endpoint_string):
@@ -349,17 +335,15 @@
             pass
         items = client.list_configuration_settings(key_filter="multi_*")
         assert len(list(items)) > PAGE_SIZE
 
         # Remove the configuration settings
         try:
             [
-                client.delete_configuration_setting(
-                    key="multi_" + str(i) + KEY_UUID, label="multi_label_" + str(i)
-                )
+                client.delete_configuration_setting(key="multi_" + str(i) + KEY_UUID, label="multi_label_" + str(i))
                 for i in range(PAGE_SIZE + 1)
             ]
         except AzureError:
             pass
 
     @app_config_aad_decorator
     @recorded_by_proxy
@@ -386,17 +370,15 @@
 
     # method: list_revisions
     @app_config_aad_decorator
     @recorded_by_proxy
     def test_list_revisions_key_label(self, appconfiguration_endpoint_string):
         self.set_up(appconfiguration_endpoint_string, is_aad=True)
         to_list = self.create_config_setting()
-        items = list(self.client.list_revisions(
-            label_filter=to_list.label, key_filter=to_list.key
-        ))
+        items = list(self.client.list_revisions(label_filter=to_list.label, key_filter=to_list.key))
         assert len(items) >= 2
         assert all(x.key == to_list.key and x.label == to_list.label for x in items)
         self.tear_down()
 
     @app_config_aad_decorator
     @recorded_by_proxy
     def test_list_revisions_only_label(self, appconfiguration_endpoint_string):
@@ -415,30 +397,28 @@
         assert all(x.key == KEY for x in items)
         self.tear_down()
 
     @app_config_aad_decorator
     @recorded_by_proxy
     def test_list_revisions_fields(self, appconfiguration_endpoint_string):
         self.set_up(appconfiguration_endpoint_string, is_aad=True)
-        items = list(self.client.list_revisions(
-            key_filter="*", label_filter=LABEL, fields=["key", "content_type"]
-        ))
+        items = list(self.client.list_revisions(key_filter="*", label_filter=LABEL, fields=["key", "content_type"]))
         assert all(x.key and not x.label and x.content_type and not x.tags and not x.etag for x in items)
         self.tear_down()
 
     @app_config_aad_decorator
     @recorded_by_proxy
     def test_list_revisions_correct_etag(self, appconfiguration_endpoint_string):
         client = self.create_aad_client(appconfiguration_endpoint_string)
         to_list_kv = self.create_config_setting()
-        to_list_kv = self.add_for_test(client, to_list_kv)
+        self.add_for_test(client, to_list_kv)
         custom_headers = {"If-Match": to_list_kv.etag}
-        items = list(client.list_revisions(
-            key_filter=to_list_kv.key, label_filter=to_list_kv.label, headers=custom_headers
-        ))
+        items = list(
+            client.list_revisions(key_filter=to_list_kv.key, label_filter=to_list_kv.label, headers=custom_headers)
+        )
         assert len(items) >= 1
         assert all(x.key == to_list_kv.key and x.label == to_list_kv.label for x in items)
         client.delete_configuration_setting(to_list_kv.key)
 
     @app_config_aad_decorator
     @recorded_by_proxy
     def test_read_only(self, appconfiguration_endpoint_string):
@@ -477,20 +457,20 @@
         with pytest.raises(ResourceReadOnlyError):
             client.set_configuration_setting(read_only_kv)
         readable_kv = client.set_read_only(read_only_kv, False)
         readable_kv.value = to_set_kv.value
         readable_kv.tags = to_set_kv.tags
         set_kv = client.set_configuration_setting(readable_kv)
         assert (
-                to_set_kv.key == set_kv.key
-                and to_set_kv.label == to_set_kv.label
-                and to_set_kv.value == set_kv.value
-                and to_set_kv.content_type == set_kv.content_type
-                and to_set_kv.tags == set_kv.tags
-                and to_set_kv.etag != set_kv.etag
+            to_set_kv.key == set_kv.key
+            and to_set_kv.label == to_set_kv.label
+            and to_set_kv.value == set_kv.value
+            and to_set_kv.content_type == set_kv.content_type
+            and to_set_kv.tags == set_kv.tags
+            and to_set_kv.etag != set_kv.etag
         )
         set_kv.etag = "bad"
         with pytest.raises(ResourceModifiedError):
             client.set_read_only(set_kv, True, match_condition=MatchConditions.IfNotModified)
         client.delete_configuration_setting(to_set_kv.key)
 
     @app_config_aad_decorator
@@ -498,33 +478,33 @@
     def test_sync_tokens_with_configuration_setting(self, appconfiguration_endpoint_string):
         client = self.create_aad_client(appconfiguration_endpoint_string)
         sync_tokens = copy.deepcopy(client._sync_token_policy._sync_tokens)
         sync_token_header = self._order_dict(sync_tokens)
         sync_token_header = ",".join(str(x) for x in sync_token_header.values())
 
         new = ConfigurationSetting(
-                key="KEY1",
-                label=None,
-                value="TEST_VALUE1",
-                content_type=TEST_CONTENT_TYPE,
-                tags={"tag1": "tag1", "tag2": "tag2"},
+            key="KEY1",
+            label=None,
+            value="TEST_VALUE1",
+            content_type=TEST_CONTENT_TYPE,
+            tags={"tag1": "tag1", "tag2": "tag2"},
         )
 
         client.set_configuration_setting(new)
         sync_tokens2 = copy.deepcopy(client._sync_token_policy._sync_tokens)
         sync_token_header2 = self._order_dict(sync_tokens2)
         sync_token_header2 = ",".join(str(x) for x in sync_token_header2.values())
         assert sync_token_header != sync_token_header2
 
         new = ConfigurationSetting(
-                key="KEY2",
-                label=None,
-                value="TEST_VALUE2",
-                content_type=TEST_CONTENT_TYPE,
-                tags={"tag1": "tag1", "tag2": "tag2"},
+            key="KEY2",
+            label=None,
+            value="TEST_VALUE2",
+            content_type=TEST_CONTENT_TYPE,
+            tags={"tag1": "tag1", "tag2": "tag2"},
         )
 
         client.set_configuration_setting(new)
         sync_tokens3 = copy.deepcopy(client._sync_token_policy._sync_tokens)
         sync_token_header3 = self._order_dict(sync_tokens3)
         sync_token_header3 = ",".join(str(x) for x in sync_token_header3.values())
         assert sync_token_header2 != sync_token_header3
@@ -532,66 +512,59 @@
         client.delete_configuration_setting(new.key)
 
     @app_config_aad_decorator
     @recorded_by_proxy
     def test_sync_tokens_with_feature_flag_configuration_setting(self, appconfiguration_endpoint_string):
         self.set_up(appconfiguration_endpoint_string, is_aad=True)
         new = FeatureFlagConfigurationSetting(
-            'custom',
+            "custom",
             enabled=True,
-            filters = [
+            filters=[
                 {
                     "name": "Microsoft.Percentage",
                     "parameters": {
                         "Value": 10,
                         "User": "user1",
-                    }
+                    },
                 }
-            ]
+            ],
         )
 
         sync_tokens = copy.deepcopy(self.client._sync_token_policy._sync_tokens)
         keys = list(sync_tokens.keys())
         seq_num = sync_tokens[keys[0]].sequence_number
         self.client.set_configuration_setting(new)
 
         new = FeatureFlagConfigurationSetting(
-            'time_window',
+            "time_window",
             enabled=True,
-            filters = [
+            filters=[
                 {
-                    u"name": FILTER_TIME_WINDOW,
-                    u"parameters": {
-                        "Start": "Wed, 10 Mar 2021 05:00:00 GMT",
-                        "End": "Fri, 02 Apr 2021 04:00:00 GMT"
-                    }
+                    "name": FILTER_TIME_WINDOW,
+                    "parameters": {"Start": "Wed, 10 Mar 2021 05:00:00 GMT", "End": "Fri, 02 Apr 2021 04:00:00 GMT"},
                 },
-            ]
+            ],
         )
 
         self.client.set_configuration_setting(new)
         sync_tokens2 = copy.deepcopy(self.client._sync_token_policy._sync_tokens)
         keys = list(sync_tokens2.keys())
         seq_num2 = sync_tokens2[keys[0]].sequence_number
 
         new = FeatureFlagConfigurationSetting(
             "newflag",
             enabled=True,
             filters=[
                 {
                     "name": FILTER_TARGETING,
                     "parameters": {
-                        u"Audience": {
-                            u"Users": [u"abc", u"def"],
-                            u"Groups": [u"ghi", u"jkl"],
-                            u"DefaultRolloutPercentage": 75
-                        }
-                    }
+                        "Audience": {"Users": ["abc", "def"], "Groups": ["ghi", "jkl"], "DefaultRolloutPercentage": 75}
+                    },
                 },
-            ]
+            ],
         )
 
         self.client.set_configuration_setting(new)
         sync_tokens3 = copy.deepcopy(self.client._sync_token_policy._sync_tokens)
         keys = list(sync_tokens3.keys())
         seq_num3 = sync_tokens3[keys[0]].sequence_number
 
@@ -610,51 +583,52 @@
         self._assert_same_keys(feature_flag, set_flag)
 
         set_flag.enabled = not set_flag.enabled
         changed_flag = client.set_configuration_setting(set_flag)
 
         changed_flag.enabled = False
         temp = json.loads(changed_flag.value)
-        assert temp['enabled'] == False
+        assert temp["enabled"] == False
 
         c = json.loads(copy.deepcopy(changed_flag.value))
-        c['enabled'] = True
+        c["enabled"] = True
         changed_flag.value = json.dumps(c)
         assert changed_flag.enabled == True
 
         changed_flag.value = json.dumps({})
         assert changed_flag.enabled == None
-        assert changed_flag.value == json.dumps({'enabled': None, "conditions": {"client_filters": None}})
+        assert changed_flag.value == json.dumps({"enabled": None, "conditions": {"client_filters": None}})
 
         set_flag.value = "bad_value"
         assert set_flag.enabled == None
         assert set_flag.filters == None
 
         client.delete_configuration_setting(changed_flag.key)
 
     @app_config_aad_decorator
     @recorded_by_proxy
     def test_config_setting_secret_reference(self, appconfiguration_endpoint_string):
         client = self.create_aad_client(appconfiguration_endpoint_string)
         secret_reference = SecretReferenceConfigurationSetting(
-            "ConnectionString", "https://test-test.vault.azure.net/secrets/connectionString")
+            "ConnectionString", "https://test-test.vault.azure.net/secrets/connectionString"
+        )
         set_flag = client.set_configuration_setting(secret_reference)
         self._assert_same_keys(secret_reference, set_flag)
 
         updated_flag = client.set_configuration_setting(set_flag)
         self._assert_same_keys(set_flag, updated_flag)
 
         assert isinstance(updated_flag, SecretReferenceConfigurationSetting)
         new_uri = "https://aka.ms/azsdk"
         new_uri2 = "https://aka.ms/azsdk/python"
         updated_flag.secret_id = new_uri
         temp = json.loads(updated_flag.value)
-        assert temp['uri'] == new_uri
+        assert temp["uri"] == new_uri
 
-        updated_flag.value = json.dumps({'uri': new_uri2})
+        updated_flag.value = json.dumps({"uri": new_uri2})
         assert updated_flag.secret_id == new_uri2
 
         set_flag.value = "bad_value"
         assert set_flag.secret_id == None
 
         client.delete_configuration_setting(secret_reference.key)
 
@@ -665,22 +639,18 @@
         new = FeatureFlagConfigurationSetting(
             "newflag",
             enabled=True,
             filters=[
                 {
                     "name": FILTER_TARGETING,
                     "parameters": {
-                        u"Audience": {
-                            u"Users": [u"abc", u"def"],
-                            u"Groups": [u"ghi", u"jkl"],
-                            u"DefaultRolloutPercentage": 75
-                        }
-                    }
+                        "Audience": {"Users": ["abc", "def"], "Groups": ["ghi", "jkl"], "DefaultRolloutPercentage": 75}
+                    },
                 }
-            ]
+            ],
         )
 
         sent_config = client.set_configuration_setting(new)
         self._assert_same_keys(sent_config, new)
 
         assert isinstance(sent_config.filters[0], dict)
         assert len(sent_config.filters) == 1
@@ -689,56 +659,53 @@
         updated_sent_config = client.set_configuration_setting(sent_config)
         self._assert_same_keys(sent_config, updated_sent_config)
 
         updated_sent_config.filters.append(
             {
                 "name": FILTER_TARGETING,
                 "parameters": {
-                    u"Audience": {
-                        u"Users": [u"abcd", u"defg"], # cspell:disable-line
-                        u"Groups": [u"ghij", u"jklm"], # cspell:disable-line
-                        u"DefaultRolloutPercentage": 50
+                    "Audience": {
+                        "Users": ["abcd", "defg"],  # cspell:disable-line
+                        "Groups": ["ghij", "jklm"],  # cspell:disable-line
+                        "DefaultRolloutPercentage": 50,
                     }
-                }
+                },
             }
         )
         updated_sent_config.filters.append(
             {
                 "name": FILTER_TARGETING,
                 "parameters": {
-                    u"Audience": {
-                        u"Users": [u"abcde", u"defgh"], # cspell:disable-line
-                        u"Groups": [u"ghijk", u"jklmn"], # cspell:disable-line
-                        u"DefaultRolloutPercentage": 100
+                    "Audience": {
+                        "Users": ["abcde", "defgh"],  # cspell:disable-line
+                        "Groups": ["ghijk", "jklmn"],  # cspell:disable-line
+                        "DefaultRolloutPercentage": 100,
                     }
-                }
+                },
             }
         )
         sent_config = client.set_configuration_setting(updated_sent_config)
         self._assert_same_keys(sent_config, updated_sent_config)
         assert len(sent_config.filters) == 3
 
         client.delete_configuration_setting(updated_sent_config.key)
 
     @app_config_aad_decorator
     @recorded_by_proxy
     def test_feature_filter_time_window(self, appconfiguration_endpoint_string):
         client = self.create_aad_client(appconfiguration_endpoint_string)
         new = FeatureFlagConfigurationSetting(
-            'time_window',
+            "time_window",
             enabled=True,
             filters=[
                 {
                     "name": FILTER_TIME_WINDOW,
-                    "parameters": {
-                        "Start": "Wed, 10 Mar 2021 05:00:00 GMT",
-                        "End": "Fri, 02 Apr 2021 04:00:00 GMT"
-                    }
+                    "parameters": {"Start": "Wed, 10 Mar 2021 05:00:00 GMT", "End": "Fri, 02 Apr 2021 04:00:00 GMT"},
                 }
-            ]
+            ],
         )
 
         sent = client.set_configuration_setting(new)
         self._assert_same_keys(sent, new)
 
         sent.filters[0]["parameters"]["Start"] = "Thurs, 11 Mar 2021 05:00:00 GMT"
         new_sent = client.set_configuration_setting(sent)
@@ -747,25 +714,15 @@
         client.delete_configuration_setting(new_sent.key)
 
     @app_config_aad_decorator
     @recorded_by_proxy
     def test_feature_filter_custom(self, appconfiguration_endpoint_string):
         client = self.create_aad_client(appconfiguration_endpoint_string)
         new = FeatureFlagConfigurationSetting(
-            'custom',
-            enabled=True,
-            filters=[
-                {
-                    "name": FILTER_PERCENTAGE,
-                    "parameters": {
-                        "Value": 10,
-                        "User": "user1"
-                    }
-                }
-            ]
+            "custom", enabled=True, filters=[{"name": FILTER_PERCENTAGE, "parameters": {"Value": 10, "User": "user1"}}]
         )
 
         sent = client.set_configuration_setting(new)
         self._assert_same_keys(sent, new)
 
         sent.filters[0]["parameters"]["Value"] = 100
         new_sent = client.set_configuration_setting(sent)
@@ -774,41 +731,33 @@
         client.delete_configuration_setting(new_sent.key)
 
     @app_config_aad_decorator
     @recorded_by_proxy
     def test_feature_filter_multiple(self, appconfiguration_endpoint_string):
         client = self.create_aad_client(appconfiguration_endpoint_string)
         new = FeatureFlagConfigurationSetting(
-            'custom',
+            "custom",
             enabled=True,
             filters=[
-                {
-                    "name": FILTER_PERCENTAGE,
-                    "parameters": {
-                        "Value": 10
-                    }
-                },
+                {"name": FILTER_PERCENTAGE, "parameters": {"Value": 10}},
                 {
                     "name": FILTER_TIME_WINDOW,
-                    "parameters": {
-                        "Start": "Wed, 10 Mar 2021 05:00:00 GMT",
-                        "End": "Fri, 02 Apr 2021 04:00:00 GMT"
-                    }
+                    "parameters": {"Start": "Wed, 10 Mar 2021 05:00:00 GMT", "End": "Fri, 02 Apr 2021 04:00:00 GMT"},
                 },
                 {
                     "name": FILTER_TARGETING,
                     "parameters": {
-                        u"Audience": {
-                            u"Users": [u"abcde", u"defgh"], # cspell:disable-line
-                            u"Groups": [u"ghijk", u"jklmn"], # cspell:disable-line
-                            u"DefaultRolloutPercentage": 100
+                        "Audience": {
+                            "Users": ["abcde", "defgh"],  # cspell:disable-line
+                            "Groups": ["ghijk", "jklmn"],  # cspell:disable-line
+                            "DefaultRolloutPercentage": 100,
                         }
-                    }
-                }
-            ]
+                    },
+                },
+            ],
         )
 
         sent = client.set_configuration_setting(new)
         self._assert_same_keys(sent, new)
 
         sent.filters[0]["parameters"]["Value"] = 100
         sent.filters[1]["parameters"]["Start"] = "Wed, 10 Mar 2021 08:00:00 GMT"
```

## Comparing `azure-appconfiguration-1.4.0b1/tests/conftest.py` & `azure-appconfiguration-1.5.0b1/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,18 @@
 # IN THE SOFTWARE.
 #
 # --------------------------------------------------------------------------
 import pytest
 import os
 from devtools_testutils import add_general_regex_sanitizer, test_proxy, set_bodiless_matcher
 
+
 @pytest.fixture(scope="session", autouse=True)
 def add_sanitizers(test_proxy):
     set_bodiless_matcher()
-    
+
     client_id = os.environ.get("APPCONFIGURATION_CLIENT_ID", "client-id")
     add_general_regex_sanitizer(regex=client_id, value="client-id")
     client_secret = os.environ.get("APPCONFIGURATION_CLIENT_SECRET", "client-secret")
     add_general_regex_sanitizer(regex=client_secret, value="client-secret")
     tenant_id = os.environ.get("APPCONFIGURATION_TENANT_ID", "00000000-0000-0000-0000-000000000000")
     add_general_regex_sanitizer(value="00000000-0000-0000-0000-000000000000", regex=tenant_id)
```

## Comparing `azure-appconfiguration-1.4.0b1/tests/async_preparers.py` & `azure-appconfiguration-1.5.0b1/tests/async_preparers.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,28 +7,29 @@
 from preparers import AppConfigPreparer, trim_kwargs_from_test_function
 
 
 def app_config_decorator_async(func, **kwargs):
     @AppConfigPreparer()
     async def wrapper(*args, **kwargs):
         appconfiguration_connection_string = kwargs.pop("appconfiguration_connection_string")
-        kwargs['appconfiguration_connection_string'] = appconfiguration_connection_string
-        
-        trimmed_kwargs = {k:v for k, v in kwargs.items()}
+        kwargs["appconfiguration_connection_string"] = appconfiguration_connection_string
+
+        trimmed_kwargs = {k: v for k, v in kwargs.items()}
         trim_kwargs_from_test_function(func, trimmed_kwargs)
 
         await func(*args, **trimmed_kwargs)
 
     return wrapper
 
+
 def app_config_aad_decorator_async(func, **kwargs):
     @AppConfigPreparer()
     async def wrapper(*args, **kwargs):
         appconfiguration_endpoint_string = kwargs.pop("appconfiguration_endpoint_string")
-        kwargs['appconfiguration_endpoint_string'] = appconfiguration_endpoint_string
+        kwargs["appconfiguration_endpoint_string"] = appconfiguration_endpoint_string
 
-        trimmed_kwargs = {k:v for k, v in kwargs.items()}
+        trimmed_kwargs = {k: v for k, v in kwargs.items()}
         trim_kwargs_from_test_function(func, trimmed_kwargs)
 
         await func(*args, **trimmed_kwargs)
 
     return wrapper
```

## Comparing `azure-appconfiguration-1.4.0b1/tests/test_sync_token_policy.py` & `azure-appconfiguration-1.5.0b1/tests/test_sync_token_policy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,100 +1,106 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 
 from azure.core.pipeline.transport import HttpRequest, HttpResponse
-from azure.core.pipeline import PipelineRequest,PipelineResponse
+from azure.core.pipeline import PipelineRequest, PipelineResponse
 from azure.appconfiguration._sync_token import SyncToken, SyncTokenPolicy
 
+
 def test_parse_sync_token():
     test_sync_token = "jtqGc1I4=MDoyOA==;sn=28"
     sync_token = SyncToken.from_sync_token_string(test_sync_token)
-    assert  sync_token.token_id == 'jtqGc1I4'
-    assert  sync_token.value == 'MDoyOA=='
-    assert  sync_token.sequence_number == 28
+    assert sync_token.token_id == "jtqGc1I4"
+    assert sync_token.value == "MDoyOA=="
+    assert sync_token.sequence_number == 28
+
 
 def test_save_sync_token():
     test_sync_token = "jtqGc1I4=MDoyOA==;sn=28"
     header = {"Sync-Token": test_sync_token}
     request = HttpRequest("GET", "https://bing.com/")
     response = HttpResponse(request, None)
     response.headers = header
     pipeline_response = PipelineResponse(request, response, None)
     sync_token_policy = SyncTokenPolicy()
     sync_token_policy.on_response(None, pipeline_response)
-    sync_token = sync_token_policy._sync_tokens['jtqGc1I4']
-    assert sync_token.token_id == 'jtqGc1I4'
-    assert sync_token.value == 'MDoyOA=='
+    sync_token = sync_token_policy._sync_tokens["jtqGc1I4"]
+    assert sync_token.token_id == "jtqGc1I4"
+    assert sync_token.value == "MDoyOA=="
     assert sync_token.sequence_number == 28
 
+
 def test_set_sync_token():
     test_sync_token = "jtqGc1I4=MDoyOA==;sn=28"
     header = {"Sync-Token": test_sync_token}
     request = HttpRequest("GET", "https://bing.com/")
     response = HttpResponse(request, None)
     response.headers = header
     pipeline_response = PipelineResponse(request, response, None)
     pipeline_request = PipelineRequest(request, None)
     sync_token_policy = SyncTokenPolicy()
     sync_token_policy.on_response(None, pipeline_response)
     sync_token_policy.on_request(pipeline_request)
     sync_token_header = pipeline_request.http_request.headers.get("Sync-Token")
-    assert sync_token_header == 'jtqGc1I4=MDoyOA=='
+    assert sync_token_header == "jtqGc1I4=MDoyOA=="
+
 
 def test_save_multi_sync_token():
     test_sync_token = "syncToken1=val1;sn=6,syncToken2=val2;sn=10"
     header = {"Sync-Token": test_sync_token}
     request = HttpRequest("GET", "https://bing.com/")
     response = HttpResponse(request, None)
     response.headers = header
     pipeline_response = PipelineResponse(request, response, None)
     sync_token_policy = SyncTokenPolicy()
     sync_token_policy.on_response(None, pipeline_response)
-    sync_token = sync_token_policy._sync_tokens['syncToken1']
-    assert sync_token.token_id == 'syncToken1'
-    assert sync_token.value == 'val1'
+    sync_token = sync_token_policy._sync_tokens["syncToken1"]
+    assert sync_token.token_id == "syncToken1"
+    assert sync_token.value == "val1"
     assert sync_token.sequence_number == 6
-    sync_token = sync_token_policy._sync_tokens['syncToken2']
-    assert sync_token.token_id == 'syncToken2'
-    assert sync_token.value == 'val2'
+    sync_token = sync_token_policy._sync_tokens["syncToken2"]
+    assert sync_token.token_id == "syncToken2"
+    assert sync_token.value == "val2"
     assert sync_token.sequence_number == 10
 
+
 def test_set_multi_sync_token():
     test_sync_token = "syncToken1=val1;sn=6,syncToken2=val2;sn=10"
     header = {"Sync-Token": test_sync_token}
     request = HttpRequest("GET", "https://bing.com/")
     response = HttpResponse(request, None)
     response.headers = header
     pipeline_response = PipelineResponse(request, response, None)
     pipeline_request = PipelineRequest(request, None)
     sync_token_policy = SyncTokenPolicy()
     sync_token_policy.on_response(None, pipeline_response)
     sync_token_policy.on_request(pipeline_request)
     sync_token_header = pipeline_request.http_request.headers.get("Sync-Token")
-    assert 'syncToken1=val1' in sync_token_header
-    assert 'syncToken2=val2' in sync_token_header
+    assert "syncToken1=val1" in sync_token_header
+    assert "syncToken2=val2" in sync_token_header
+
 
 def test_update_cached_sync_token():
     test_sync_token = "syncToken1=val1;sn=6"
     header = {"Sync-Token": test_sync_token}
     request = HttpRequest("GET", "https://bing.com/")
     response = HttpResponse(request, None)
     response.headers = header
     pipeline_response = PipelineResponse(request, response, None)
     sync_token_policy = SyncTokenPolicy()
     sync_token_policy.on_response(None, pipeline_response)
-    sync_token = sync_token_policy._sync_tokens['syncToken1']
-    assert sync_token.token_id == 'syncToken1'
-    assert sync_token.value == 'val1'
+    sync_token = sync_token_policy._sync_tokens["syncToken1"]
+    assert sync_token.token_id == "syncToken1"
+    assert sync_token.value == "val1"
     assert sync_token.sequence_number == 6
     test_new_sync_token = "syncToken1=val2;sn=10"
     header["Sync-Token"] = test_new_sync_token
     response.headers = header
     pipeline_response = PipelineResponse(request, response, None)
     sync_token_policy.on_response(None, pipeline_response)
-    sync_token = sync_token_policy._sync_tokens['syncToken1']
-    assert sync_token.token_id == 'syncToken1'
-    assert sync_token.value == 'val2'
+    sync_token = sync_token_policy._sync_tokens["syncToken1"]
+    assert sync_token.token_id == "syncToken1"
+    assert sync_token.value == "val2"
     assert sync_token.sequence_number == 10
```

## Comparing `azure-appconfiguration-1.4.0b1/tests/test_azure_appconfiguration_client_async.py` & `azure-appconfiguration-1.5.0b1/tests/test_azure_appconfiguration_client_async.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # license information.
 # --------------------------------------------------------------------------
 import pytest
 import copy
 import datetime
 import json
 import re
-import copy
 from azure.core import MatchConditions
 from azure.core.exceptions import (
     ResourceModifiedError,
     ResourceNotFoundError,
     ResourceExistsError,
     AzureError,
 )
 from azure.appconfiguration import (
     ResourceReadOnlyError,
     ConfigurationSetting,
+    ConfigurationSettingFilter,
     SecretReferenceConfigurationSetting,
     FeatureFlagConfigurationSetting,
     FILTER_PERCENTAGE,
     FILTER_TARGETING,
     FILTER_TIME_WINDOW,
 )
 from azure.appconfiguration.aio import AzureAppConfigurationClient
@@ -34,15 +34,14 @@
     TEST_CONTENT_TYPE,
     LABEL_RESERVED_CHARS,
     PAGE_SIZE,
     KEY_UUID,
 )
 from devtools_testutils.aio import recorded_by_proxy_async
 from async_preparers import app_config_decorator_async
-from typing import Any
 from uuid import uuid4
 
 
 class TestAppConfigurationClientAsync(AsyncAppConfigTestCase):
     # method: add_configuration_setting
     @app_config_decorator_async
     @recorded_by_proxy_async
@@ -59,17 +58,15 @@
             assert (
                 created_kv.label == kv.label
                 and kv.value == kv.value
                 and created_kv.content_type == kv.content_type
                 and created_kv.tags == kv.tags
             )
             assert (
-                created_kv.etag is not None
-                and created_kv.last_modified is not None
-                and created_kv.read_only is False
+                created_kv.etag is not None and created_kv.last_modified is not None and created_kv.read_only is False
             )
             await client.delete_configuration_setting(key=created_kv.key, label=created_kv.label)
 
     @app_config_decorator_async
     @recorded_by_proxy_async
     async def test_add_existing_configuration_setting(self, appconfiguration_connection_string):
         async with self.create_client(appconfiguration_connection_string) as client:
@@ -170,17 +167,15 @@
 
     @app_config_decorator_async
     @recorded_by_proxy_async
     async def test_get_configuration_setting_label(self, appconfiguration_connection_string):
         async with self.create_client(appconfiguration_connection_string) as client:
             compare_kv = self.create_config_setting()
             await self.add_for_test(client, compare_kv)
-            fetched_kv = await client.get_configuration_setting(
-                compare_kv.key, compare_kv.label
-            )
+            fetched_kv = await client.get_configuration_setting(compare_kv.key, compare_kv.label)
             assert (
                 fetched_kv.key == compare_kv.key
                 and fetched_kv.value == compare_kv.value
                 and fetched_kv.content_type == compare_kv.content_type
                 and fetched_kv.tags == compare_kv.tags
             )
             assert fetched_kv.label is not None
@@ -189,17 +184,15 @@
     @app_config_decorator_async
     @recorded_by_proxy_async
     async def test_get_non_existing_configuration_setting(self, appconfiguration_connection_string):
         async with self.create_client(appconfiguration_connection_string) as client:
             compare_kv = self.create_config_setting()
             await self.add_for_test(client, compare_kv)
             with pytest.raises(ResourceNotFoundError):
-                await client.get_configuration_setting(
-                    compare_kv.key, compare_kv.label + "a"
-                )
+                await client.get_configuration_setting(compare_kv.key, compare_kv.label + "a")
             await client.delete_configuration_setting(key=compare_kv.key, label=compare_kv.label)
 
     # method: delete_configuration_setting
     @app_config_decorator_async
     @recorded_by_proxy_async
     async def test_delete_with_key_no_label(self, appconfiguration_connection_string):
         async with self.create_client(appconfiguration_connection_string) as client:
@@ -279,17 +272,17 @@
         assert all(x.key == KEY for x in items)
         await self.tear_down()
 
     @app_config_decorator_async
     @recorded_by_proxy_async
     async def test_list_configuration_settings_fields(self, appconfiguration_connection_string):
         await self.set_up(appconfiguration_connection_string)
-        items = await self.convert_to_list(self.client.list_configuration_settings(
-            key_filter="*", label_filter=LABEL, fields=["key", "content_type"]
-        ))
+        items = await self.convert_to_list(
+            self.client.list_configuration_settings(key_filter="*", label_filter=LABEL, fields=["key", "content_type"])
+        )
         assert len(items) == 1
         assert all(x.key and not x.label and x.content_type for x in items)
         await self.tear_down()
 
     @app_config_decorator_async
     @recorded_by_proxy_async
     async def test_list_configuration_settings_reserved_chars(self, appconfiguration_connection_string):
@@ -314,17 +307,19 @@
     @app_config_decorator_async
     @recorded_by_proxy_async
     async def test_list_configuration_settings_correct_etag(self, appconfiguration_connection_string):
         async with self.create_client(appconfiguration_connection_string) as client:
             to_list_kv = self.create_config_setting()
             await self.add_for_test(client, to_list_kv)
             custom_headers = {"If-Match": to_list_kv.etag or ""}
-            items = await self.convert_to_list(client.list_configuration_settings(
-                key_filter=to_list_kv.key, label_filter=to_list_kv.label, headers=custom_headers
-            ))
+            items = await self.convert_to_list(
+                client.list_configuration_settings(
+                    key_filter=to_list_kv.key, label_filter=to_list_kv.label, headers=custom_headers
+                )
+            )
             assert len(items) == 1
             assert all(x.key == to_list_kv.key and x.label == to_list_kv.label for x in items)
             await client.delete_configuration_setting(to_list_kv.key)
 
     @app_config_decorator_async
     @recorded_by_proxy_async
     async def test_list_configuration_settings_multi_pages(self, appconfiguration_connection_string):
@@ -365,34 +360,39 @@
         assert len(items) > 0
         await self.tear_down()
 
     @app_config_decorator_async
     @recorded_by_proxy_async
     async def test_list_configuration_settings_only_accepttime(self, appconfiguration_connection_string, **kwargs):
         recorded_variables = kwargs.pop("variables", {})
-        await self.set_up(appconfiguration_connection_string)
-        exclude_today = await self.convert_to_list(self.client.list_configuration_settings(
-            accept_datetime=recorded_variables.setdefault(
-                "datetime", str(datetime.datetime.today() + datetime.timedelta(days=-1))
-            )
-        ))
-        all_inclusive = await self.convert_to_list(self.client.list_configuration_settings())
-        assert len(all_inclusive) > len(exclude_today)
-        await self.tear_down()
+        recorded_variables.setdefault("timestamp", str(datetime.datetime.utcnow()))
+
+        async with self.create_client(appconfiguration_connection_string) as client:
+            # Confirm all configuration settings are cleaned up
+            current_config_settings = await self.convert_to_list(client.list_configuration_settings())
+            if len(current_config_settings) != 0:
+                for config_setting in current_config_settings:
+                    client.delete_configuration_setting(config_setting)
+
+            revision = await self.convert_to_list(
+                client.list_configuration_settings(accept_datetime=recorded_variables.get("timestamp"))
+            )
+            assert len(revision) >= 0
+
         return recorded_variables
 
     # method: list_revisions
     @app_config_decorator_async
     @recorded_by_proxy_async
     async def test_list_revisions_key_label(self, appconfiguration_connection_string):
         await self.set_up(appconfiguration_connection_string)
         to_list1 = self.create_config_setting()
-        items = await self.convert_to_list(self.client.list_revisions(
-            label_filter=to_list1.label, key_filter=to_list1.key
-        ))
+        items = await self.convert_to_list(
+            self.client.list_revisions(label_filter=to_list1.label, key_filter=to_list1.key)
+        )
         assert len(items) >= 2
         assert all(x.key == to_list1.key and x.label == to_list1.label for x in items)
         await self.tear_down()
 
     @app_config_decorator_async
     @recorded_by_proxy_async
     async def test_list_revisions_only_label(self, appconfiguration_connection_string):
@@ -411,29 +411,29 @@
         assert all(x.key == KEY for x in items)
         await self.tear_down()
 
     @app_config_decorator_async
     @recorded_by_proxy_async
     async def test_list_revisions_fields(self, appconfiguration_connection_string):
         await self.set_up(appconfiguration_connection_string)
-        items = await self.convert_to_list(self.client.list_revisions(
-            key_filter="*", label_filter=LABEL, fields=["key", "content_type"]
-        ))
+        items = await self.convert_to_list(
+            self.client.list_revisions(key_filter="*", label_filter=LABEL, fields=["key", "content_type"])
+        )
         assert all(x.key and not x.label and x.content_type and not x.tags and not x.etag for x in items)
         await self.tear_down()
 
     @app_config_decorator_async
     @recorded_by_proxy_async
     async def test_list_revisions_correct_etag(self, appconfiguration_connection_string):
         await self.set_up(appconfiguration_connection_string)
         to_list_kv = self.create_config_setting()
         custom_headers = {"If-Match": to_list_kv.etag or ""}
-        items = await self.convert_to_list(self.client.list_revisions(
-            key_filter=to_list_kv.key, label_filter=to_list_kv.label, headers=custom_headers
-        ))
+        items = await self.convert_to_list(
+            self.client.list_revisions(key_filter=to_list_kv.key, label_filter=to_list_kv.label, headers=custom_headers)
+        )
         assert len(items) >= 1
         assert all(x.key == to_list_kv.key and x.label == to_list_kv.label for x in items)
         await self.tear_down()
 
     @app_config_decorator_async
     @recorded_by_proxy_async
     async def test_read_only(self, appconfiguration_connection_string):
@@ -472,20 +472,20 @@
             with pytest.raises(ResourceReadOnlyError):
                 await client.set_configuration_setting(read_only_kv)
             readable_kv = await client.set_read_only(read_only_kv, False)
             readable_kv.value = to_set_kv.value
             readable_kv.tags = to_set_kv.tags
             set_kv = await client.set_configuration_setting(readable_kv)
             assert (
-                    to_set_kv.key == set_kv.key
-                    and to_set_kv.label == to_set_kv.label
-                    and to_set_kv.value == set_kv.value
-                    and to_set_kv.content_type == set_kv.content_type
-                    and to_set_kv.tags == set_kv.tags
-                    and to_set_kv.etag != set_kv.etag
+                to_set_kv.key == set_kv.key
+                and to_set_kv.label == to_set_kv.label
+                and to_set_kv.value == set_kv.value
+                and to_set_kv.content_type == set_kv.content_type
+                and to_set_kv.tags == set_kv.tags
+                and to_set_kv.etag != set_kv.etag
             )
             set_kv.etag = "bad"
             with pytest.raises(ResourceModifiedError):
                 await client.set_read_only(set_kv, True, match_condition=MatchConditions.IfNotModified)
             await client.delete_configuration_setting(to_set_kv.key)
 
     @app_config_decorator_async
@@ -493,33 +493,33 @@
     async def test_sync_tokens_with_configuration_setting(self, appconfiguration_connection_string):
         async with self.create_client(appconfiguration_connection_string) as client:
             sync_tokens = copy.deepcopy(client._sync_token_policy._sync_tokens)
             sync_token_header = self._order_dict(sync_tokens)
             sync_token_header = ",".join(str(x) for x in sync_token_header.values())
 
             new = ConfigurationSetting(
-                    key="KEY1",
-                    label=None,
-                    value="TEST_VALUE1",
-                    content_type=TEST_CONTENT_TYPE,
-                    tags={"tag1": "tag1", "tag2": "tag2"},
+                key="KEY1",
+                label=None,
+                value="TEST_VALUE1",
+                content_type=TEST_CONTENT_TYPE,
+                tags={"tag1": "tag1", "tag2": "tag2"},
             )
 
             await client.set_configuration_setting(new)
             sync_tokens2 = copy.deepcopy(client._sync_token_policy._sync_tokens)
             sync_token_header2 = self._order_dict(sync_tokens2)
             sync_token_header2 = ",".join(str(x) for x in sync_token_header2.values())
             assert sync_token_header != sync_token_header2
 
             new = ConfigurationSetting(
-                    key="KEY2",
-                    label=None,
-                    value="TEST_VALUE2",
-                    content_type=TEST_CONTENT_TYPE,
-                    tags={"tag1": "tag1", "tag2": "tag2"},
+                key="KEY2",
+                label=None,
+                value="TEST_VALUE2",
+                content_type=TEST_CONTENT_TYPE,
+                tags={"tag1": "tag1", "tag2": "tag2"},
             )
 
             await client.set_configuration_setting(new)
             sync_tokens3 = copy.deepcopy(client._sync_token_policy._sync_tokens)
             sync_token_header3 = self._order_dict(sync_tokens3)
             sync_token_header3 = ",".join(str(x) for x in sync_token_header3.values())
             assert sync_token_header2 != sync_token_header3
@@ -527,66 +527,59 @@
             await client.delete_configuration_setting(new.key)
 
     @app_config_decorator_async
     @recorded_by_proxy_async
     async def test_sync_tokens_with_feature_flag_configuration_setting(self, appconfiguration_connection_string):
         await self.set_up(appconfiguration_connection_string)
         new = FeatureFlagConfigurationSetting(
-            'custom',
+            "custom",
             enabled=True,
-            filters = [
+            filters=[
                 {
                     "name": "Microsoft.Percentage",
                     "parameters": {
                         "Value": 10,
                         "User": "user1",
-                    }
+                    },
                 }
-            ]
+            ],
         )
 
         sync_tokens = copy.deepcopy(self.client._sync_token_policy._sync_tokens)
         keys = list(sync_tokens.keys())
         seq_num = sync_tokens[keys[0]].sequence_number
         await self.client.set_configuration_setting(new)
 
         new = FeatureFlagConfigurationSetting(
-            'time_window',
+            "time_window",
             enabled=True,
-            filters = [
+            filters=[
                 {
-                    u"name": FILTER_TIME_WINDOW,
-                    u"parameters": {
-                        "Start": "Wed, 10 Mar 2021 05:00:00 GMT",
-                        "End": "Fri, 02 Apr 2021 04:00:00 GMT"
-                    }
+                    "name": FILTER_TIME_WINDOW,
+                    "parameters": {"Start": "Wed, 10 Mar 2021 05:00:00 GMT", "End": "Fri, 02 Apr 2021 04:00:00 GMT"},
                 },
-            ]
+            ],
         )
 
         await self.client.set_configuration_setting(new)
         sync_tokens2 = copy.deepcopy(self.client._sync_token_policy._sync_tokens)
         keys = list(sync_tokens2.keys())
         seq_num2 = sync_tokens2[keys[0]].sequence_number
 
         new = FeatureFlagConfigurationSetting(
             "newflag",
             enabled=True,
             filters=[
                 {
                     "name": FILTER_TARGETING,
                     "parameters": {
-                        u"Audience": {
-                            u"Users": [u"abc", u"def"],
-                            u"Groups": [u"ghi", u"jkl"],
-                            u"DefaultRolloutPercentage": 75
-                        }
-                    }
+                        "Audience": {"Users": ["abc", "def"], "Groups": ["ghi", "jkl"], "DefaultRolloutPercentage": 75}
+                    },
                 },
-            ]
+            ],
         )
 
         await self.client.set_configuration_setting(new)
         sync_tokens3 = copy.deepcopy(self.client._sync_token_policy._sync_tokens)
         keys = list(sync_tokens3.keys())
         seq_num3 = sync_tokens3[keys[0]].sequence_number
 
@@ -606,52 +599,53 @@
             self._assert_same_keys(feature_flag, set_flag)
 
             set_flag.enabled = not set_flag.enabled
             changed_flag = await client.set_configuration_setting(set_flag)
 
             changed_flag.enabled = False
             temp = json.loads(changed_flag.value)
-            assert temp['enabled'] == False
+            assert temp["enabled"] == False
 
             c = json.loads(copy.deepcopy(changed_flag.value))
-            c['enabled'] = True
+            c["enabled"] = True
             changed_flag.value = json.dumps(c)
             assert changed_flag.enabled == True
 
             changed_flag.value = json.dumps({})
             assert changed_flag.enabled == None
-            assert changed_flag.value == json.dumps({'enabled': None, "conditions": {"client_filters": None}})
+            assert changed_flag.value == json.dumps({"enabled": None, "conditions": {"client_filters": None}})
 
             set_flag.value = "bad_value"
             assert set_flag.enabled == None
             assert set_flag.filters == None
 
             await client.delete_configuration_setting(changed_flag.key)
 
     @app_config_decorator_async
     @recorded_by_proxy_async
     async def test_config_setting_secret_reference(self, appconfiguration_connection_string):
         async with self.create_client(appconfiguration_connection_string) as client:
             secret_reference = SecretReferenceConfigurationSetting(
-                "ConnectionString", "https://test-test.vault.azure.net/secrets/connectionString")
+                "ConnectionString", "https://test-test.vault.azure.net/secrets/connectionString"
+            )
             set_flag = await client.set_configuration_setting(secret_reference)
             self._assert_same_keys(secret_reference, set_flag)
 
             set_flag.secret_id = "https://test-test.vault.azure.net/new_secrets/connectionString"
             updated_flag = await client.set_configuration_setting(set_flag)
             self._assert_same_keys(set_flag, updated_flag)
 
             assert isinstance(updated_flag, SecretReferenceConfigurationSetting)
             new_uri = "https://aka.ms/azsdk"
             new_uri2 = "https://aka.ms/azsdk/python"
             updated_flag.secret_id = new_uri
             temp = json.loads(updated_flag.value)
-            assert temp['uri'] == new_uri
+            assert temp["uri"] == new_uri
 
-            updated_flag.value = json.dumps({'uri': new_uri2})
+            updated_flag.value = json.dumps({"uri": new_uri2})
             assert updated_flag.secret_id == new_uri2
 
             set_flag.value = "bad_value"
             assert set_flag.secret_id == None
 
             await client.delete_configuration_setting(secret_reference.key)
 
@@ -662,22 +656,22 @@
             new = FeatureFlagConfigurationSetting(
                 "newflag",
                 enabled=True,
                 filters=[
                     {
                         "name": FILTER_TARGETING,
                         "parameters": {
-                            u"Audience": {
-                                u"Users": [u"abc", u"def"],
-                                u"Groups": [u"ghi", u"jkl"],
-                                u"DefaultRolloutPercentage": 75
+                            "Audience": {
+                                "Users": ["abc", "def"],
+                                "Groups": ["ghi", "jkl"],
+                                "DefaultRolloutPercentage": 75,
                             }
-                        }
+                        },
                     }
-                ]
+                ],
             )
 
             sent_config = await client.set_configuration_setting(new)
             self._assert_same_keys(sent_config, new)
 
             assert isinstance(sent_config.filters[0], dict)
             assert len(sent_config.filters) == 1
@@ -686,56 +680,56 @@
             updated_sent_config = await client.set_configuration_setting(sent_config)
             self._assert_same_keys(sent_config, updated_sent_config)
 
             updated_sent_config.filters.append(
                 {
                     "name": FILTER_TARGETING,
                     "parameters": {
-                        u"Audience": {
-                            u"Users": [u"abcd", u"defg"], # cspell:disable-line
-                            u"Groups": [u"ghij", u"jklm"], # cspell:disable-line
-                            u"DefaultRolloutPercentage": 50
+                        "Audience": {
+                            "Users": ["abcd", "defg"],  # cspell:disable-line
+                            "Groups": ["ghij", "jklm"],  # cspell:disable-line
+                            "DefaultRolloutPercentage": 50,
                         }
-                    }
+                    },
                 }
             )
             updated_sent_config.filters.append(
                 {
                     "name": FILTER_TARGETING,
                     "parameters": {
-                        u"Audience": {
-                            u"Users": [u"abcde", u"defgh"], # cspell:disable-line
-                            u"Groups": [u"ghijk", u"jklmn"], # cspell:disable-line
-                            u"DefaultRolloutPercentage": 100
+                        "Audience": {
+                            "Users": ["abcde", "defgh"],  # cspell:disable-line
+                            "Groups": ["ghijk", "jklmn"],  # cspell:disable-line
+                            "DefaultRolloutPercentage": 100,
                         }
-                    }
+                    },
                 }
             )
             sent_config = await client.set_configuration_setting(updated_sent_config)
             self._assert_same_keys(sent_config, updated_sent_config)
             assert len(sent_config.filters) == 3
 
             await client.delete_configuration_setting(updated_sent_config.key)
 
     @app_config_decorator_async
     @recorded_by_proxy_async
     async def test_feature_filter_time_window(self, appconfiguration_connection_string):
         async with self.create_client(appconfiguration_connection_string) as client:
             new = FeatureFlagConfigurationSetting(
-                'time_window',
+                "time_window",
                 enabled=True,
                 filters=[
                     {
                         "name": FILTER_TIME_WINDOW,
                         "parameters": {
                             "Start": "Wed, 10 Mar 2021 05:00:00 GMT",
-                            "End": "Fri, 02 Apr 2021 04:00:00 GMT"
-                        }
+                            "End": "Fri, 02 Apr 2021 04:00:00 GMT",
+                        },
                     }
-                ]
+                ],
             )
 
             sent = await client.set_configuration_setting(new)
             self._assert_same_keys(sent, new)
 
             sent.filters[0]["parameters"]["Start"] = "Thurs, 11 Mar 2021 05:00:00 GMT"
             new_sent = await client.set_configuration_setting(sent)
@@ -744,25 +738,17 @@
             await client.delete_configuration_setting(new_sent.key)
 
     @app_config_decorator_async
     @recorded_by_proxy_async
     async def test_feature_filter_custom(self, appconfiguration_connection_string):
         async with self.create_client(appconfiguration_connection_string) as client:
             new = FeatureFlagConfigurationSetting(
-                'custom',
+                "custom",
                 enabled=True,
-                filters=[
-                    {
-                        "name": FILTER_PERCENTAGE,
-                        "parameters": {
-                            "Value": 10,
-                            "User": "user1"
-                        }
-                    }
-                ]
+                filters=[{"name": FILTER_PERCENTAGE, "parameters": {"Value": 10, "User": "user1"}}],
             )
 
             sent = await client.set_configuration_setting(new)
             self._assert_same_keys(sent, new)
 
             sent.filters[0]["parameters"]["Value"] = 100
             new_sent = await client.set_configuration_setting(sent)
@@ -771,41 +757,36 @@
             await client.delete_configuration_setting(new_sent.key)
 
     @app_config_decorator_async
     @recorded_by_proxy_async
     async def test_feature_filter_multiple(self, appconfiguration_connection_string):
         async with self.create_client(appconfiguration_connection_string) as client:
             new = FeatureFlagConfigurationSetting(
-                'custom',
+                "custom",
                 enabled=True,
                 filters=[
-                    {
-                        "name": FILTER_PERCENTAGE,
-                        "parameters": {
-                            "Value": 10
-                        }
-                    },
+                    {"name": FILTER_PERCENTAGE, "parameters": {"Value": 10}},
                     {
                         "name": FILTER_TIME_WINDOW,
                         "parameters": {
                             "Start": "Wed, 10 Mar 2021 05:00:00 GMT",
-                            "End": "Fri, 02 Apr 2021 04:00:00 GMT"
-                        }
+                            "End": "Fri, 02 Apr 2021 04:00:00 GMT",
+                        },
                     },
                     {
                         "name": FILTER_TARGETING,
                         "parameters": {
-                            u"Audience": {
-                                u"Users": [u"abcde", u"defgh"], # cspell:disable-line
-                                u"Groups": [u"ghijk", u"jklmn"], # cspell:disable-line
-                                u"DefaultRolloutPercentage": 100
+                            "Audience": {
+                                "Users": ["abcde", "defgh"],  # cspell:disable-line
+                                "Groups": ["ghijk", "jklmn"],  # cspell:disable-line
+                                "DefaultRolloutPercentage": 100,
                             }
-                        }
-                    }
-                ]
+                        },
+                    },
+                ],
             )
 
             sent = await client.set_configuration_setting(new)
             self._assert_same_keys(sent, new)
 
             sent.filters[0]["parameters"]["Value"] = 100
             sent.filters[1]["parameters"]["Start"] = "Wed, 10 Mar 2021 08:00:00 GMT"
@@ -815,187 +796,227 @@
             self._assert_same_keys(sent, new_sent)
 
             assert new_sent.filters[0]["parameters"]["Value"] == 100
             assert new_sent.filters[1]["parameters"]["Start"] == "Wed, 10 Mar 2021 08:00:00 GMT"
             assert new_sent.filters[2]["parameters"]["Audience"]["DefaultRolloutPercentage"] == 100
 
             await client.delete_configuration_setting(new_sent.key)
-    
+
     @app_config_decorator_async
     @recorded_by_proxy_async
     async def test_breaking_with_feature_flag_configuration_setting(self, appconfiguration_connection_string):
         async with self.create_client(appconfiguration_connection_string) as client:
             new = FeatureFlagConfigurationSetting(
-                'breaking1',
+                "breaking1",
                 enabled=True,
                 filters=[
                     {
                         "name": FILTER_TIME_WINDOW,
                         "parameters": {
-                            "Start": "bababooey, 31 Mar 2021 25:00:00 GMT", # cspell:disable-line
-                            "End": "Fri, 02 Apr 2021 04:00:00 GMT"
-                        }
+                            "Start": "bababooey, 31 Mar 2021 25:00:00 GMT",  # cspell:disable-line
+                            "End": "Fri, 02 Apr 2021 04:00:00 GMT",
+                        },
                     },
-                ]
+                ],
             )
             await client.set_configuration_setting(new)
             await client.get_configuration_setting(new.key)
 
             new = FeatureFlagConfigurationSetting(
-                'breaking2',
+                "breaking2",
                 enabled=True,
                 filters=[
                     {
                         "name": FILTER_TIME_WINDOW,
                         "parameters": {
-                            "Start": "bababooey, 31 Mar 2021 25:00:00 GMT", # cspell:disable-line
-                            "End": "not even trying to be a date"
-                        }
+                            "Start": "bababooey, 31 Mar 2021 25:00:00 GMT",  # cspell:disable-line
+                            "End": "not even trying to be a date",
+                        },
                     },
-                ]
+                ],
             )
             await client.set_configuration_setting(new)
             await client.get_configuration_setting(new.key)
 
             # This will show up as a Custom filter
             new = FeatureFlagConfigurationSetting(
-                'breaking3',
+                "breaking3",
                 enabled=True,
                 filters=[
                     {
                         "name": FILTER_TIME_WINDOW,
                         "parameters": {
-                            "Start": "bababooey, 31 Mar 2021 25:00:00 GMT", # cspell:disable-line
-                            "End": "not even trying to be a date"
-                        }
+                            "Start": "bababooey, 31 Mar 2021 25:00:00 GMT",  # cspell:disable-line
+                            "End": "not even trying to be a date",
+                        },
                     },
-                ]
+                ],
             )
             await client.set_configuration_setting(new)
             await client.get_configuration_setting(new.key)
 
             new = FeatureFlagConfigurationSetting(
-                'breaking4',
+                "breaking4",
                 enabled=True,
                 filters=[
-                    {
-                        "name": FILTER_TIME_WINDOW,
-                        "parameters": "stringystring"
-                    },
-                ]
+                    {"name": FILTER_TIME_WINDOW, "parameters": "stringystring"},
+                ],
             )
             await client.set_configuration_setting(new)
             await client.get_configuration_setting(new.key)
 
             new = FeatureFlagConfigurationSetting(
-                'breaking5',
+                "breaking5",
                 enabled=True,
-                filters=[
-                    {
-                        "name": FILTER_TARGETING,
-                        "parameters": {
-                            u"Audience": {
-                                u"Users": '123'
-                            }
-                        }
-                    }
-                ]
+                filters=[{"name": FILTER_TARGETING, "parameters": {"Audience": {"Users": "123"}}}],
             )
             await client.set_configuration_setting(new)
             await client.get_configuration_setting(new.key)
 
             new = FeatureFlagConfigurationSetting(
-                'breaking6',
-                enabled=True,
-                filters=[
-                    {
-                        "name": FILTER_TARGETING,
-                        "parameters": "invalidformat"
-                    }
-                ]
+                "breaking6", enabled=True, filters=[{"name": FILTER_TARGETING, "parameters": "invalidformat"}]
             )
             await client.set_configuration_setting(new)
             await client.get_configuration_setting(new.key)
 
-            new = FeatureFlagConfigurationSetting(
-                'breaking7',
-                enabled=True,
-                filters=[
-                    {
-                        'abc': 'def'
-                    }
-                ]
-            )
+            new = FeatureFlagConfigurationSetting("breaking7", enabled=True, filters=[{"abc": "def"}])
             await client.set_configuration_setting(new)
             await client.get_configuration_setting(new.key)
 
-            new = FeatureFlagConfigurationSetting(
-                'breaking8',
-                enabled=True,
-                filters=[
-                    {
-                        'abc': 'def'
-                    }
-                ]
-            )
-            new.feature_flag_content_type = "fakeyfakey" # cspell:disable-line
+            new = FeatureFlagConfigurationSetting("breaking8", enabled=True, filters=[{"abc": "def"}])
+            new.feature_flag_content_type = "fakeyfakey"  # cspell:disable-line
             await client.set_configuration_setting(new)
             await client.get_configuration_setting(new.key)
 
             await client.delete_configuration_setting(new.key)
 
     @app_config_decorator_async
     @recorded_by_proxy_async
     async def test_breaking_with_secret_reference_configuration_setting(self, appconfiguration_connection_string):
         async with self.create_client(appconfiguration_connection_string) as client:
-            new = SecretReferenceConfigurationSetting(
-                "aref", # cspell:disable-line
-                "notaurl"
-            )
+            new = SecretReferenceConfigurationSetting("aref", "notaurl")  # cspell:disable-line
             await client.set_configuration_setting(new)
             await client.get_configuration_setting(new.key)
 
-            new = SecretReferenceConfigurationSetting(
-                "aref1", # cspell:disable-line
-                "notaurl"
-            )
-            new.content_type = "fkaeyjfdkal;" # cspell:disable-line
+            new = SecretReferenceConfigurationSetting("aref1", "notaurl")  # cspell:disable-line
+            new.content_type = "fkaeyjfdkal;"  # cspell:disable-line
             await client.set_configuration_setting(new)
             await client.get_configuration_setting(new.key)
 
             await client.delete_configuration_setting(new.key)
 
+    @app_config_decorator_async
+    @recorded_by_proxy_async
+    async def test_create_snapshot(self, appconfiguration_connection_string):
+        await self.set_up(appconfiguration_connection_string)
+        snapshot_name = self.get_resource_name("snapshot")
+        filters = [ConfigurationSettingFilter(key=KEY, label=LABEL)]
+        response = await self.client.begin_create_snapshot(name=snapshot_name, filters=filters)
+        created_snapshot = await response.result()
+        assert created_snapshot.name == snapshot_name
+        assert created_snapshot.status == "ready"
+        assert len(created_snapshot.filters) == 1
+        assert created_snapshot.filters[0].key == KEY
+        assert created_snapshot.filters[0].label == LABEL
+
+        received_snapshot = await self.client.get_snapshot(name=snapshot_name)
+        self._assert_snapshots(received_snapshot, created_snapshot)
+
+        await self.tear_down()
+
+    @app_config_decorator_async
+    @recorded_by_proxy_async
+    async def test_update_snapshot_status(self, appconfiguration_connection_string):
+        await self.set_up(appconfiguration_connection_string)
+        snapshot_name = self.get_resource_name("snapshot")
+        filters = [ConfigurationSettingFilter(key=KEY, label=LABEL)]
+        response = await self.client.begin_create_snapshot(name=snapshot_name, filters=filters)
+        created_snapshot = await response.result()
+        assert created_snapshot.status == "ready"
+
+        archived_snapshot = await self.client.archive_snapshot(name=snapshot_name)
+        assert archived_snapshot.status == "archived"
+
+        recovered_snapshot = await self.client.recover_snapshot(name=snapshot_name)
+        assert recovered_snapshot.status == "ready"
+
+        await self.tear_down()
+
+    @app_config_decorator_async
+    @recorded_by_proxy_async
+    async def test_list_snapshots(self, appconfiguration_connection_string):
+        await self.set_up(appconfiguration_connection_string)
+
+        result = await self.convert_to_list(self.client.list_snapshots())
+        initial_snapshots = len(result)
+
+        snapshot_name1 = self.get_resource_name("snapshot1")
+        snapshot_name2 = self.get_resource_name("snapshot2")
+        filters1 = [ConfigurationSettingFilter(key=KEY)]
+        response1 = await self.client.begin_create_snapshot(name=snapshot_name1, filters=filters1)
+        created_snapshot1 = await response1.result()
+        assert created_snapshot1.status == "ready"
+        filters2 = [ConfigurationSettingFilter(key=KEY, label=LABEL)]
+        response2 = await self.client.begin_create_snapshot(name=snapshot_name2, filters=filters2)
+        created_snapshot2 = await response2.result()
+        assert created_snapshot2.status == "ready"
+
+        result = await self.convert_to_list(self.client.list_snapshots())
+        assert len(result) == initial_snapshots + 2
+
+        await self.tear_down()
+
+    @app_config_decorator_async
+    @recorded_by_proxy_async
+    async def test_list_snapshot_configuration_settings(self, appconfiguration_connection_string):
+        await self.set_up(appconfiguration_connection_string)
+        snapshot_name = self.get_resource_name("snapshot")
+        filters = [ConfigurationSettingFilter(key=KEY, label=LABEL)]
+        response = await self.client.begin_create_snapshot(name=snapshot_name, filters=filters)
+        created_snapshot = await response.result()
+        assert created_snapshot.status == "ready"
+
+        items = await self.convert_to_list(self.client.list_snapshot_configuration_settings(snapshot_name))
+        assert len(items) == 1
+
+        await self.tear_down()
+
 
 class TestAppConfigurationClientUnitTest:
     @pytest.mark.asyncio
     async def test_mock_policies(self):
         from azure.core.pipeline.transport import HttpResponse, AsyncHttpTransport
         from azure.core.pipeline import PipelineRequest, PipelineResponse
         from consts import APPCONFIGURATION_CONNECTION_STRING
+
         class MockTransport(AsyncHttpTransport):
             def __init__(self):
                 self.auth_headers = []
+
             async def __aexit__(self, exc_type, exc_val, exc_tb):
                 pass
+
             async def close(self):
                 pass
+
             async def open(self):
                 pass
 
-            async def send(self, request: PipelineRequest, **kwargs: Any) -> PipelineResponse:
-                assert request.headers['Authorization'] != self.auth_headers
-                self.auth_headers.append(request.headers['Authorization'])
+            async def send(self, request: PipelineRequest, **kwargs) -> PipelineResponse:
+                assert request.headers["Authorization"] != self.auth_headers
+                self.auth_headers.append(request.headers["Authorization"])
                 response = HttpResponse(request, None)
                 response.status_code = 429
                 return response
 
         def new_method(self, request):
             request.http_request.headers["Authorization"] = str(uuid4())
 
         from azure.appconfiguration._azure_appconfiguration_requests import AppConfigRequestsCredentialsPolicy
+
         # Store the method to restore later
         temp = AppConfigRequestsCredentialsPolicy._signed_request
         AppConfigRequestsCredentialsPolicy._signed_request = new_method
 
         client = AzureAppConfigurationClient.from_connection_string(
             APPCONFIGURATION_CONNECTION_STRING, transport=MockTransport()
         )
```

## Comparing `azure-appconfiguration-1.4.0b1/tests/consts.py` & `azure-appconfiguration-1.5.0b1/tests/consts.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 KEY_UUID = "test_key_a6af8952-54a6-11e9-b600-2816a84d0309"
 LABEL_UUID = "1d7b2b28-549e-11e9-b51c-2816a84d0309"
 KEY = "PYTHON_UNIT_" + KEY_UUID
 LABEL = "test_label1_" + LABEL_UUID
 LABEL_RESERVED_CHARS = "test_label2_*, \\" + LABEL_UUID  # contains reserved chars *,\
 TEST_CONTENT_TYPE = "test content type"
 TEST_VALUE = "test value"
-APPCONFIGURATION_CONNECTION_STRING = "Endpoint=https://fake_app_config.azconfig-test.io;Id=0-l4-s0:h5htBaY5Z1LwFz50bIQv;Secret=lamefakesecretlamefakesecretlamefakesecrett=" # pylint:disable=line-too-long
+APPCONFIGURATION_CONNECTION_STRING = "Endpoint=https://fake_app_config.azconfig-test.io;Id=0-l4-s0:h5htBaY5Z1LwFz50bIQv;Secret=lamefakesecretlamefakesecretlamefakesecrett="  # pylint:disable=line-too-long
```

## Comparing `azure-appconfiguration-1.4.0b1/tests/asynctestcase.py` & `azure-appconfiguration-1.5.0b1/tests/asynctestcase.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,49 +2,47 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 from azure.appconfiguration.aio import AzureAppConfigurationClient
 from azure.core.async_paging import AsyncItemPaged
+from azure.core.exceptions import ResourceExistsError
 from testcase import AppConfigTestCase
 from typing import List
 
 
 class AsyncAppConfigTestCase(AppConfigTestCase):
     def create_aad_client(self, appconfiguration_endpoint_string):
         cred = self.get_credential(AzureAppConfigurationClient, is_async=True)
         return AzureAppConfigurationClient(appconfiguration_endpoint_string, cred)
-    
+
     def create_client(self, appconfiguration_connection_string):
         return AzureAppConfigurationClient.from_connection_string(appconfiguration_connection_string)
 
     async def add_for_test(self, client, config_setting):
-        exist_list = await self.convert_to_list(client.list_configuration_settings(
-            key_filter=config_setting.key, label_filter=config_setting.label
-        ))
-        exist = bool(exist_list)
-        if exist:
-            await client.delete_configuration_setting(key=config_setting.key, label=config_setting.label)
-        return await client.add_configuration_setting(config_setting)
-        
+        try:
+            await client.add_configuration_setting(config_setting)
+        except ResourceExistsError:
+            pass
+
     async def convert_to_list(self, config_settings: AsyncItemPaged) -> List:
         list = []
         async for item in config_settings:
             list.append(item)
         return list
-    
+
     async def set_up(self, appconfiguration_string, is_aad=False):
         if is_aad:
             self.client = self.create_aad_client(appconfiguration_string)
         else:
             self.client = self.create_client(appconfiguration_string)
         await self.add_for_test(self.client, self.create_config_setting())
         await self.add_for_test(self.client, self.create_config_setting_no_label())
-    
+
     async def tear_down(self):
         if self.client is not None:
             config_settings = self.client.list_configuration_settings()
             async for config_setting in config_settings:
                 await self.client.delete_configuration_setting(key=config_setting.key, label=config_setting.label)
             await self.client.close()
         else:
```

## Comparing `azure-appconfiguration-1.4.0b1/tests/perfstress_tests/get.py` & `azure-appconfiguration-1.5.0b1/tests/perfstress_tests/get.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.4.0b1/tests/perfstress_tests/set.py` & `azure-appconfiguration-1.5.0b1/tests/perfstress_tests/set.py`

 * *Files identical despite different names*

## Comparing `azure-appconfiguration-1.4.0b1/samples/conditional_operation_sample.py` & `azure-appconfiguration-1.5.0b1/samples/conditional_operation_sample.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,68 +4,62 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 
 """
 FILE: conditional_operation_sample.py
+
 DESCRIPTION:
     This sample demos conditional set/get/delete operations for app configuration
+
 USAGE: python conditional_operation_sample.py
-"""
 
+    Set the environment variables with your own values before running the sample:
+    1) APPCONFIGURATION_CONNECTION_STRING: Connection String used to access the Azure App Configuration.
+"""
+import os
 from azure.core import MatchConditions
 from azure.core.exceptions import ResourceModifiedError
 from azure.appconfiguration import AzureAppConfigurationClient, ConfigurationSetting
-from util import print_configuration_setting, get_connection_string
+from util import print_configuration_setting
+
 
 def main():
-    CONNECTION_STRING = get_connection_string()
+    CONNECTION_STRING = os.environ["APPCONFIGURATION_CONNECTION_STRING"]
 
     # Create app config client
     client = AzureAppConfigurationClient.from_connection_string(CONNECTION_STRING)
 
     # Unconditional set
     config_setting = ConfigurationSetting(
-        key="MyKey",
-        value="my value",
-        content_type="my content type",
-        tags={"my tag": "my tag value"}
+        key="MyKey", value="my value", content_type="my content type", tags={"my tag": "my tag value"}
     )
     client.set_configuration_setting(config_setting)
 
     # Unconditional get
     first_get = client.get_configuration_setting(key="MyKey")
     if first_get is None:
         return print("Error, unconditional set failed.")
     print_configuration_setting(first_get)
 
     # Conditional get, expect to return None because it is not modified
     second_get = client.get_configuration_setting(
-        key="MyKey",
-        etag=first_get.etag,
-        match_condition=MatchConditions.IfModified
+        key="MyKey", etag=first_get.etag, match_condition=MatchConditions.IfModified
     )
     print_configuration_setting(second_get)
 
     # Conditional set
     first_get.value = "new value"
-    client.set_configuration_setting(
-        configuration_setting=first_get,
-        match_condition=MatchConditions.IfNotModified
-    )
+    client.set_configuration_setting(configuration_setting=first_get, match_condition=MatchConditions.IfNotModified)
 
     # Conditional set, expect to see error because it is modified
     try:
-        client.set_configuration_setting(
-            configuration_setting=first_get,
-            match_condition=MatchConditions.IfNotModified
-        )
+        client.set_configuration_setting(configuration_setting=first_get, match_condition=MatchConditions.IfNotModified)
     except ResourceModifiedError:
         pass
 
-    client.delete_configuration_setting(
-        key="MyKey"
-    )
+    client.delete_configuration_setting(key="MyKey")
+
 
 if __name__ == "__main__":
     main()
```

## Comparing `azure-appconfiguration-1.4.0b1/samples/hello_world_sample_async.py` & `azure-appconfiguration-1.5.0b1/samples/hello_world_sample_async.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,50 +4,55 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 
 """
 FILE: hello_world_async_sample.py
+
 DESCRIPTION:
     This sample demos set/get/delete operations for app configuration
+
 USAGE: python hello_world_async_sample.py
-"""
 
+    Set the environment variables with your own values before running the sample:
+    1) APPCONFIGURATION_CONNECTION_STRING: Connection String used to access the Azure App Configuration.
+"""
 import asyncio
 from azure.appconfiguration import ConfigurationSetting
-from azure.appconfiguration.aio import AzureAppConfigurationClient
-from util import print_configuration_setting, get_connection_string
+from util import print_configuration_setting
+
 
 async def main():
-    CONNECTION_STRING = get_connection_string()
+    # [START create_app_config_client]
+    import os
+    from azure.appconfiguration.aio import AzureAppConfigurationClient
+
+    CONNECTION_STRING = os.environ["APPCONFIGURATION_CONNECTION_STRING"]
 
     # Create app config client
     client = AzureAppConfigurationClient.from_connection_string(CONNECTION_STRING)
+    # [END create_app_config_client]
 
     print("Set new configuration setting")
     config_setting = ConfigurationSetting(
-        key="MyKey",
-        value="my value",
-        content_type="my content type",
-        tags={"my tag": "my tag value"}
+        key="MyKey", value="my value", content_type="my content type", tags={"my tag": "my tag value"}
     )
     returned_config_setting = await client.set_configuration_setting(config_setting)
     print("New configuration setting:")
     print_configuration_setting(returned_config_setting)
     print("")
 
     print("Get configuration setting")
-    fetched_config_setting = await client.get_configuration_setting(
-        key="MyKey"
-    )
+    # [START get_config_setting]
+    fetched_config_setting = await client.get_configuration_setting(key="MyKey")
+    # [END get_config_setting]
     print("Fetched configuration setting:")
     print_configuration_setting(fetched_config_setting)
     print("")
 
     print("Delete configuration setting")
-    await client.delete_configuration_setting(
-        key="MyKey"
-    )
+    await client.delete_configuration_setting(key="MyKey")
+
 
 if __name__ == "__main__":
     asyncio.run(main())
```

## Comparing `azure-appconfiguration-1.4.0b1/samples/list_revision_sample.py` & `azure-appconfiguration-1.5.0b1/samples/read_only_sample_async.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,45 +3,57 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 
 """
-FILE: list_revision_sample.py
+FILE: read_only_async_sample.py
+
 DESCRIPTION:
-    This sample demos list revision operations for app configuration
-USAGE: python list_revision_sample.py
+    This sample demos set_read_only operations for app configuration
+
+USAGE: python read_only_async_sample.py
+
+    Set the environment variables with your own values before running the sample:
+    1) APPCONFIGURATION_CONNECTION_STRING: Connection String used to access the Azure App Configuration.
 """
+import asyncio
+import os
+from azure.appconfiguration import ConfigurationSetting
+from azure.appconfiguration.aio import AzureAppConfigurationClient
+from util import print_configuration_setting
 
-from azure.appconfiguration import AzureAppConfigurationClient, ConfigurationSetting
-from util import print_configuration_setting, get_connection_string
 
-def main():
-    CONNECTION_STRING = get_connection_string()
+async def main():
+    CONNECTION_STRING = os.environ["APPCONFIGURATION_CONNECTION_STRING"]
 
     # Create app config client
     client = AzureAppConfigurationClient.from_connection_string(CONNECTION_STRING)
 
+    print("Set new configuration setting")
     config_setting = ConfigurationSetting(
-        key="MyKey",
-        value="my value",
-        content_type="my content type",
-        tags={"my tag": "my tag value"}
+        key="MyKey", value="my value", content_type="my content type", tags={"my tag": "my tag value"}
     )
-    returned_config_setting = client.set_configuration_setting(config_setting)
-
-    returned_config_setting.value = "new value"
-    returned_config_setting.content_type = "new content type"
-    client.set_configuration_setting(config_setting)
-
-    items = client.list_revisions(key_filter="MyKey")
-    for item in items:
-        print_configuration_setting(item)
-        print("")
+    returned_config_setting = await client.set_configuration_setting(config_setting)
+    print("New configuration setting:")
+    print_configuration_setting(returned_config_setting)
+    print("")
+
+    print("Read only configuration setting:")
+    read_only_config_setting = await client.set_read_only(returned_config_setting)
+    print_configuration_setting(read_only_config_setting)
+    print("")
+
+    print("Clear read only configuration setting:")
+    read_write_config_setting = await client.set_read_only(returned_config_setting, False)
+    print_configuration_setting(read_write_config_setting)
+    print("")
 
-    client.delete_configuration_setting(
+    print("Delete configuration setting")
+    await client.delete_configuration_setting(
         key="MyKey",
     )
 
+
 if __name__ == "__main__":
-    main()
+    asyncio.run(main())
```

## Comparing `azure-appconfiguration-1.4.0b1/samples/hello_world_advanced_sample_async.py` & `azure-appconfiguration-1.5.0b1/samples/hello_world_advanced_sample_async.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,56 +4,61 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 
 """
 FILE: hello_world_advanced_async_sample.py
+
 DESCRIPTION:
     This sample demos more advanced scenarios including add/set with label/list operations for app configuration
+
 USAGE: python hello_world_advanced_async_sample.py
-"""
 
+    Set the environment variables with your own values before running the sample:
+    1) APPCONFIGURATION_CONNECTION_STRING: Connection String used to access the Azure App Configuration.
+"""
 import asyncio
+import os
 from azure.appconfiguration import ConfigurationSetting
 from azure.appconfiguration.aio import AzureAppConfigurationClient
-from util import print_configuration_setting, get_connection_string
+from util import print_configuration_setting
+
 
 async def main():
-    CONNECTION_STRING = get_connection_string()
+    CONNECTION_STRING = os.environ["APPCONFIGURATION_CONNECTION_STRING"]
 
     # Create app config client
     client = AzureAppConfigurationClient.from_connection_string(CONNECTION_STRING)
 
     print("Add new configuration setting")
     config_setting = ConfigurationSetting(
-        key="MyKey",
-        label="MyLabel",
-        value="my value",
-        content_type="my content type",
-        tags={"my tag": "my tag value"}
+        key="MyKey", label="MyLabel", value="my value", content_type="my content type", tags={"my tag": "my tag value"}
     )
     added_config_setting = await client.add_configuration_setting(config_setting)
     print("New configuration setting:")
     print_configuration_setting(added_config_setting)
     print("")
 
     print("Set configuration setting")
     added_config_setting.value = "new value"
     added_config_setting.content_type = "new content type"
     updated_config_setting = await client.set_configuration_setting(config_setting)
     print_configuration_setting(updated_config_setting)
     print("")
 
     print("List configuration settings")
+    # [START list_config_setting]
     config_settings = client.list_configuration_settings(label_filter="MyLabel")
     async for item in config_settings:
         print_configuration_setting(item)
+    # [END list_config_setting]
 
     print("Delete configuration setting")
     await client.delete_configuration_setting(
         key="MyKey",
         label="MyLabel",
     )
 
+
 if __name__ == "__main__":
     asyncio.run(main())
```

## Comparing `azure-appconfiguration-1.4.0b1/samples/read_only_sample_async.py` & `azure-appconfiguration-1.5.0b1/samples/read_only_sample.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,57 +3,55 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 
 """
-FILE: read_only_async_sample.py
+FILE: read_only_sample.py
+
 DESCRIPTION:
     This sample demos set_read_only operations for app configuration
-USAGE: python read_only_async_sample.py
+
+USAGE: python read_only_sample.py
+
+    Set the environment variables with your own values before running the sample:
+    1) APPCONFIGURATION_CONNECTION_STRING: Connection String used to access the Azure App Configuration.
 """
+import os
+from azure.appconfiguration import AzureAppConfigurationClient, ConfigurationSetting
+from util import print_configuration_setting
 
-import asyncio
-from azure.appconfiguration import ConfigurationSetting
-from azure.appconfiguration.aio import AzureAppConfigurationClient
-from util import print_configuration_setting, get_connection_string
 
-async def main():
-    CONNECTION_STRING = get_connection_string()
+def main():
+    CONNECTION_STRING = os.environ["APPCONFIGURATION_CONNECTION_STRING"]
 
     # Create app config client
     client = AzureAppConfigurationClient.from_connection_string(CONNECTION_STRING)
 
     print("Set new configuration setting")
     config_setting = ConfigurationSetting(
-        key="MyKey",
-        value="my value",
-        content_type="my content type",
-        tags={"my tag": "my tag value"}
+        key="MyKey", value="my value", content_type="my content type", tags={"my tag": "my tag value"}
     )
-    returned_config_setting = await client.set_configuration_setting(config_setting)
+    returned_config_setting = client.set_configuration_setting(config_setting)
     print("New configuration setting:")
     print_configuration_setting(returned_config_setting)
     print("")
 
     print("Read only configuration setting:")
-    read_only_config_setting = await client.set_read_only(
-        returned_config_setting
-    )
+    read_only_config_setting = client.set_read_only(returned_config_setting)
     print_configuration_setting(read_only_config_setting)
     print("")
 
     print("Clear read only configuration setting:")
-    read_write_config_setting = await client.set_read_only(
-        returned_config_setting, False
-    )
+    read_write_config_setting = client.set_read_only(returned_config_setting, False)
     print_configuration_setting(read_write_config_setting)
     print("")
 
     print("Delete configuration setting")
-    await client.delete_configuration_setting(
+    client.delete_configuration_setting(
         key="MyKey",
     )
 
+
 if __name__ == "__main__":
-    asyncio.run(main())
+    main()
```

## Comparing `azure-appconfiguration-1.4.0b1/samples/hello_world_advanced_sample.py` & `azure-appconfiguration-1.5.0b1/samples/hello_world_advanced_sample.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,54 +4,65 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 
 """
 FILE: hello_world_advanced_sample.py
+
 DESCRIPTION:
     This sample demos more advanced scenarios including add/set with label/list operations for app configuration
+
 USAGE: python hello_world_advanced_sample.py
-"""
 
+    Set the environment variables with your own values before running the sample:
+    1) APPCONFIGURATION_CONNECTION_STRING: Connection String used to access the Azure App Configuration.
+"""
+import os
 from azure.appconfiguration import AzureAppConfigurationClient, ConfigurationSetting
-from util import print_configuration_setting, get_connection_string
+from util import print_configuration_setting
+
 
 def main():
-    CONNECTION_STRING = get_connection_string()
+    CONNECTION_STRING = os.environ["APPCONFIGURATION_CONNECTION_STRING"]
 
     # Create app config client
     client = AzureAppConfigurationClient.from_connection_string(CONNECTION_STRING)
 
     print("Add new configuration setting")
+    # [START create_config_setting]
     config_setting = ConfigurationSetting(
-        key="MyKey",
-        label="MyLabel",
-        value="my value",
-        content_type="my content type",
-        tags={"my tag": "my tag value"}
+        key="MyKey", label="MyLabel", value="my value", content_type="my content type", tags={"my tag": "my tag value"}
     )
     added_config_setting = client.add_configuration_setting(config_setting)
+    # [END create_config_setting]
     print("New configuration setting:")
     print_configuration_setting(added_config_setting)
     print("")
 
     print("Set configuration setting")
+    # [START set_config_setting]
     added_config_setting.value = "new value"
     added_config_setting.content_type = "new content type"
     updated_config_setting = client.set_configuration_setting(config_setting)
+    # [END set_config_setting]
     print_configuration_setting(updated_config_setting)
     print("")
 
     print("List configuration settings")
+    # [START list_config_setting]
     config_settings = client.list_configuration_settings(label_filter="MyLabel")
     for item in config_settings:
         print_configuration_setting(item)
+    # [END list_config_setting]
 
     print("Delete configuration setting")
+    # [START delete_config_setting]
     client.delete_configuration_setting(
         key="MyKey",
         label="MyLabel",
     )
+    # [END delete_config_setting]
+
 
 if __name__ == "__main__":
     main()
```

## Comparing `azure-appconfiguration-1.4.0b1/samples/list_revision_sample_async.py` & `azure-appconfiguration-1.5.0b1/samples/list_revision_sample.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,47 +3,49 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 
 """
-FILE: list_revision_async_sample.py
+FILE: list_revision_sample.py
+
 DESCRIPTION:
     This sample demos list revision operations for app configuration
-USAGE: python list_revision_async_sample.py
+
+USAGE: python list_revision_sample.py
+
+    Set the environment variables with your own values before running the sample:
+    1) APPCONFIGURATION_CONNECTION_STRING: Connection String used to access the Azure App Configuration.
 """
+import os
+from azure.appconfiguration import AzureAppConfigurationClient, ConfigurationSetting
+from util import print_configuration_setting
 
-import asyncio
-from azure.appconfiguration import ConfigurationSetting
-from azure.appconfiguration.aio import AzureAppConfigurationClient
-from util import print_configuration_setting, get_connection_string
 
-async def main():
-    CONNECTION_STRING = get_connection_string()
+def main():
+    CONNECTION_STRING = os.environ["APPCONFIGURATION_CONNECTION_STRING"]
 
     # Create app config client
     client = AzureAppConfigurationClient.from_connection_string(CONNECTION_STRING)
 
     config_setting = ConfigurationSetting(
-        key="MyKey",
-        value="my value",
-        content_type="my content type",
-        tags={"my tag": "my tag value"}
+        key="MyKey", value="my value", content_type="my content type", tags={"my tag": "my tag value"}
     )
-    returned_config_setting = await client.set_configuration_setting(config_setting)
+    returned_config_setting = client.set_configuration_setting(config_setting)
 
     returned_config_setting.value = "new value"
     returned_config_setting.content_type = "new content type"
-    await client.set_configuration_setting(config_setting)
+    client.set_configuration_setting(config_setting)
 
     items = client.list_revisions(key_filter="MyKey")
-    async for item in items:
+    for item in items:
         print_configuration_setting(item)
         print("")
 
-    await client.delete_configuration_setting(
+    client.delete_configuration_setting(
         key="MyKey",
     )
 
+
 if __name__ == "__main__":
-    asyncio.run(main())
+    main()
```

## Comparing `azure-appconfiguration-1.4.0b1/samples/sync_token_samples_async.py` & `azure-appconfiguration-1.5.0b1/samples/sync_token_samples.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,38 +3,42 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 
 """
-FILE: sync_token_async_samples.py
+FILE: sync_token_samples.py
+
 DESCRIPTION:
     This sample demos update_sync_token for the AzureAppConfigurationClient
-USAGE: python sync_token_async_samples.py
+
+
+USAGE: python sync_token_samples.py
+
+    Set the environment variables with your own values before running the sample:
+    1) APPCONFIGURATION_CONNECTION_STRING: Connection String used to access the Azure App Configuration.
 """
-import asyncio
-from typing import Any, Dict, List
-from azure.appconfiguration.aio import AzureAppConfigurationClient
-from util import get_connection_string
+import os
+from azure.appconfiguration import AzureAppConfigurationClient
 
 
-async def handle_event_grid_notifications(event_grid_events: List[Dict[str, Any]]) -> None:
-    CONNECTION_STRING = get_connection_string()
+def handle_event_grid_notifications(event_grid_events):
+    CONNECTION_STRING = os.environ["APPCONFIGURATION_CONNECTION_STRING"]
 
     all_keys = []
 
-    async with AzureAppConfigurationClient.from_connection_string(CONNECTION_STRING) as client:
+    with AzureAppConfigurationClient.from_connection_string(CONNECTION_STRING) as client:
         for event_grid_event in event_grid_events:
-            if event_grid_event["eventType"] == 'Microsoft.KeyValueModified':
-                sync_token = event_grid_event['data']['syncToken']
+            if event_grid_event["eventType"] == "Microsoft.KeyValueModified":
+                sync_token = event_grid_event["data"]["syncToken"]
                 client.update_sync_token(sync_token)
 
-                new_key = await client.get_configuration_setting(
-                    key=event_grid_event['data']['key'], label=event_grid_event['data']['label']
+                new_key = client.get_configuration_setting(
+                    key=event_grid_event["data"]["key"], label=event_grid_event["data"]["label"]
                 )
 
                 all_keys.append(new_key)
 
 
 if __name__ == "__main__":
-    asyncio.run(handle_event_grid_notifications([]))
+    handle_event_grid_notifications([])
```

## Comparing `azure-appconfiguration-1.4.0b1/samples/conditional_operation_sample_async.py` & `azure-appconfiguration-1.5.0b1/samples/conditional_operation_sample_async.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,70 +4,68 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 
 """
 FILE: conditional_operation_async_sample.py
+
 DESCRIPTION:
     This sample demos conditional set/get/delete operations for app configuration
+
 USAGE: python conditional_operation_async_sample.py
-"""
 
+    Set the environment variables with your own values before running the sample:
+    1) APPCONFIGURATION_CONNECTION_STRING: Connection String used to access the Azure App Configuration.
+"""
+import asyncio
+import os
 from azure.core import MatchConditions
 from azure.core.exceptions import ResourceModifiedError
-import asyncio
 from azure.appconfiguration import ConfigurationSetting
 from azure.appconfiguration.aio import AzureAppConfigurationClient
-from util import print_configuration_setting, get_connection_string
+from util import print_configuration_setting
+
 
 async def main():
-    CONNECTION_STRING = get_connection_string()
+    CONNECTION_STRING = os.environ["APPCONFIGURATION_CONNECTION_STRING"]
 
     # Create app config client
     client = AzureAppConfigurationClient.from_connection_string(CONNECTION_STRING)
 
     # Unconditional set
     config_setting = ConfigurationSetting(
-        key="MyKey",
-        value="my value",
-        content_type="my content type",
-        tags={"my tag": "my tag value"}
+        key="MyKey", value="my value", content_type="my content type", tags={"my tag": "my tag value"}
     )
     await client.set_configuration_setting(config_setting)
 
     # Unconditional get
     first_get = await client.get_configuration_setting(key="MyKey")
     if first_get is None:
         return print("Error, unconditional set failed.")
     print_configuration_setting(first_get)
 
     # Conditional get, expect to return None because it is not modified
     second_get = await client.get_configuration_setting(
-        key="MyKey",
-        etag=first_get.etag,
-        match_condition=MatchConditions.IfModified
+        key="MyKey", etag=first_get.etag, match_condition=MatchConditions.IfModified
     )
     print_configuration_setting(second_get)
 
     # Conditional set
     first_get.value = "new value"
     await client.set_configuration_setting(
-        configuration_setting=first_get,
-        match_condition=MatchConditions.IfNotModified
+        configuration_setting=first_get, match_condition=MatchConditions.IfNotModified
     )
 
     # Conditional set, expect to see error because it is modified
     try:
         await client.set_configuration_setting(
-            configuration_setting=first_get,
-            match_condition=MatchConditions.IfNotModified
+            configuration_setting=first_get, match_condition=MatchConditions.IfNotModified
         )
     except ResourceModifiedError:
         pass
 
-    await client.delete_configuration_setting(
-        key="MyKey"
-    )
+    await client.delete_configuration_setting(key="MyKey")
+
 
 if __name__ == "__main__":
     asyncio.run(main())
```

## Comparing `azure-appconfiguration-1.4.0b1/samples/hello_world_sample.py` & `azure-appconfiguration-1.5.0b1/samples/list_revision_sample_async.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,49 +3,51 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 
 """
-FILE: hello_world_sample.py
+FILE: list_revision_async_sample.py
+
 DESCRIPTION:
-    This sample demos set/get/delete operations for app configuration
-USAGE: python hello_world_sample.py
+    This sample demos list revision operations for app configuration
+
+USAGE: python list_revision_async_sample.py
+
+    Set the environment variables with your own values before running the sample:
+    1) APPCONFIGURATION_CONNECTION_STRING: Connection String used to access the Azure App Configuration.
 """
+import asyncio
+import os
+from azure.appconfiguration import ConfigurationSetting
+from azure.appconfiguration.aio import AzureAppConfigurationClient
+from util import print_configuration_setting
 
-from azure.appconfiguration import AzureAppConfigurationClient, ConfigurationSetting
-from util import print_configuration_setting, get_connection_string
 
-def main():
-    CONNECTION_STRING = get_connection_string()
+async def main():
+    CONNECTION_STRING = os.environ["APPCONFIGURATION_CONNECTION_STRING"]
 
     # Create app config client
     client = AzureAppConfigurationClient.from_connection_string(CONNECTION_STRING)
 
-    print("Set new configuration setting")
     config_setting = ConfigurationSetting(
-        key="MyKey",
-        value="my value",
-        content_type="my content type",
-        tags={"my tag": "my tag value"}
-    )
-    returned_config_setting = client.set_configuration_setting(config_setting)
-    print("New configuration setting:")
-    print_configuration_setting(returned_config_setting)
-    print("")
-
-    print("Get configuration setting")
-    fetched_config_setting = client.get_configuration_setting(
-        key="MyKey"
+        key="MyKey", value="my value", content_type="my content type", tags={"my tag": "my tag value"}
     )
-    print("Fetched configuration setting:")
-    print_configuration_setting(fetched_config_setting)
-    print("")
-
-    print("Delete configuration setting")
-    client.delete_configuration_setting(
-        key="MyKey"
+    returned_config_setting = await client.set_configuration_setting(config_setting)
+
+    returned_config_setting.value = "new value"
+    returned_config_setting.content_type = "new content type"
+    await client.set_configuration_setting(config_setting)
+
+    items = client.list_revisions(key_filter="MyKey")
+    async for item in items:
+        print_configuration_setting(item)
+        print("")
+
+    await client.delete_configuration_setting(
+        key="MyKey",
     )
 
+
 if __name__ == "__main__":
-    main()
+    asyncio.run(main())
```

## Comparing `azure-appconfiguration-1.4.0b1/azure_appconfiguration.egg-info/SOURCES.txt` & `azure-appconfiguration-1.5.0b1/azure_appconfiguration.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
+TROUBLESHOOTING.md
+pyproject.toml
 setup.py
 azure/__init__.py
 azure/appconfiguration/__init__.py
 azure/appconfiguration/_azure_appconfiguration_client.py
 azure/appconfiguration/_azure_appconfiguration_credential.py
 azure/appconfiguration/_azure_appconfiguration_error.py
 azure/appconfiguration/_azure_appconfiguration_requests.py
@@ -34,15 +36,15 @@
 azure/appconfiguration/_generated/models/_azure_app_configuration_enums.py
 azure/appconfiguration/_generated/models/_models_py3.py
 azure/appconfiguration/_generated/models/_patch.py
 azure/appconfiguration/_generated/operations/__init__.py
 azure/appconfiguration/_generated/operations/_azure_app_configuration_operations.py
 azure/appconfiguration/_generated/operations/_patch.py
 azure/appconfiguration/aio/__init__.py
-azure/appconfiguration/aio/_azure_configuration_client_async.py
+azure/appconfiguration/aio/_azure_appconfiguration_client_async.py
 azure/appconfiguration/aio/_sync_token_async.py
 azure_appconfiguration.egg-info/PKG-INFO
 azure_appconfiguration.egg-info/SOURCES.txt
 azure_appconfiguration.egg-info/dependency_links.txt
 azure_appconfiguration.egg-info/not-zip-safe
 azure_appconfiguration.egg-info/requires.txt
 azure_appconfiguration.egg-info/top_level.txt
@@ -53,14 +55,16 @@
 samples/hello_world_advanced_sample_async.py
 samples/hello_world_sample.py
 samples/hello_world_sample_async.py
 samples/list_revision_sample.py
 samples/list_revision_sample_async.py
 samples/read_only_sample.py
 samples/read_only_sample_async.py
+samples/snapshot_samples.py
+samples/snapshot_samples_async.py
 samples/sync_token_samples.py
 samples/sync_token_samples_async.py
 samples/util.py
 tests/async_preparers.py
 tests/asynctestcase.py
 tests/conftest.py
 tests/consts.py
```

