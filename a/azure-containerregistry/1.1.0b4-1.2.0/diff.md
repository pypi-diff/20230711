# Comparing `tmp/azure-containerregistry-1.1.0b4.zip` & `tmp/azure-containerregistry-1.2.0.zip`

## zipinfo {}

```diff
@@ -1,96 +1,96 @@
-Zip file size: 153094 bytes, number of entries: 94
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-26 00:32 azure-containerregistry-1.1.0b4/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-26 00:32 azure-containerregistry-1.1.0b4/tests/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-26 00:32 azure-containerregistry-1.1.0b4/azure/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-26 00:32 azure-containerregistry-1.1.0b4/samples/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-26 00:32 azure-containerregistry-1.1.0b4/azure_containerregistry.egg-info/
--rw-rw-r--  2.0 unx     2312 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/setup.py
--rw-rw-r--  2.0 unx       38 b- defN 23-Apr-26 00:32 azure-containerregistry-1.1.0b4/setup.cfg
--rw-rw-r--  2.0 unx      161 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/MANIFEST.in
--rw-rw-r--  2.0 unx       86 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/pyproject.toml
--rw-rw-r--  2.0 unx     4713 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/CHANGELOG.md
--rw-rw-r--  2.0 unx    11022 b- defN 23-Apr-26 00:32 azure-containerregistry-1.1.0b4/PKG-INFO
--rw-rw-r--  2.0 unx     4279 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/TROUBLESHOOTING.md
--rw-rw-r--  2.0 unx     1073 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/LICENSE
--rw-rw-r--  2.0 unx     9999 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/README.md
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-26 00:32 azure-containerregistry-1.1.0b4/tests/perfstress_tests/
--rw-rw-r--  2.0 unx     7543 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/tests/testcase.py
--rw-rw-r--  2.0 unx     1743 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/tests/conftest.py
--rw-rw-r--  2.0 unx    39478 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/tests/test_container_registry_client.py
--rw-rw-r--  2.0 unx     9393 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/tests/test_anon_access_async.py
--rw-rw-r--  2.0 unx     3121 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/tests/asynctestcase.py
--rw-rw-r--  2.0 unx     9002 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/tests/test_anon_access.py
--rw-rw-r--  2.0 unx      290 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/tests/constants.py
--rw-rw-r--  2.0 unx      505 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/tests/preparer.py
--rw-rw-r--  2.0 unx    41494 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/tests/test_container_registry_client_async.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/tests/perfstress_tests/__init__.py
--rw-rw-r--  2.0 unx     1235 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/tests/perfstress_tests/list_artifacts.py
--rw-rw-r--  2.0 unx     1162 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/tests/perfstress_tests/list_repositories.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-26 00:32 azure-containerregistry-1.1.0b4/azure/containerregistry/
--rw-rw-r--  2.0 unx       81 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-26 00:32 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-26 00:32 azure-containerregistry-1.1.0b4/azure/containerregistry/aio/
--rw-rw-r--  2.0 unx     2504 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_download_stream.py
--rw-rw-r--  2.0 unx     1206 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/__init__.py
--rw-rw-r--  2.0 unx     4273 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_exchange_client.py
--rw-rw-r--  2.0 unx    11863 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_models.py
--rw-rw-r--  2.0 unx     2883 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_base_client.py
--rw-rw-r--  2.0 unx     3862 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_authentication_policy.py
--rw-rw-r--  2.0 unx      248 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_user_agent.py
--rw-rw-r--  2.0 unx    47682 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_container_registry_client.py
--rw-rw-r--  2.0 unx     2887 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_anonymous_exchange_client.py
--rw-rw-r--  2.0 unx      172 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_version.py
--rw-rw-r--  2.0 unx     4717 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_helpers.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/py.typed
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-26 00:32 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/models/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-26 00:32 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-26 00:32 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/operations/
--rw-rw-r--  2.0 unx     4629 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/_client.py
--rw-rw-r--  2.0 unx      722 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/__init__.py
--rw-rw-r--  2.0 unx     3326 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/_configuration.py
--rw-rw-r--  2.0 unx     1530 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/_patch.py
--rw-rw-r--  2.0 unx     1369 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/_vendor.py
--rw-rw-r--  2.0 unx    78836 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/_serialization.py
--rw-rw-r--  2.0 unx     3412 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/models/__init__.py
--rw-rw-r--  2.0 unx    64438 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/models/_models.py
--rw-rw-r--  2.0 unx      791 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/models/_patch.py
--rw-rw-r--  2.0 unx     2960 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/models/_enums.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-Apr-26 00:32 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/operations/
--rw-rw-r--  2.0 unx     4778 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/_client.py
--rw-rw-r--  2.0 unx      722 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/__init__.py
--rw-rw-r--  2.0 unx     3368 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/_configuration.py
--rw-rw-r--  2.0 unx     1530 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/_patch.py
--rw-rw-r--  2.0 unx      845 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/_vendor.py
--rw-rw-r--  2.0 unx      870 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/operations/__init__.py
--rw-rw-r--  2.0 unx     8679 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/operations/_patch.py
--rw-rw-r--  2.0 unx    80761 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/operations/_operations.py
--rw-rw-r--  2.0 unx      870 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/operations/__init__.py
--rw-rw-r--  2.0 unx    10863 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/operations/_patch.py
--rw-rw-r--  2.0 unx   103037 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/operations/_operations.py
--rw-rw-r--  2.0 unx    49024 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/aio/_async_container_registry_client.py
--rw-rw-r--  2.0 unx     3963 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/aio/_async_authentication_policy.py
--rw-rw-r--  2.0 unx     3207 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/aio/_async_anonymous_exchange_client.py
--rw-rw-r--  2.0 unx      675 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/aio/__init__.py
--rw-rw-r--  2.0 unx     2667 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/aio/_async_download_stream.py
--rw-rw-r--  2.0 unx     4382 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/aio/_async_exchange_client.py
--rw-rw-r--  2.0 unx     3244 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/azure/containerregistry/aio/_async_base_client.py
--rw-rw-r--  2.0 unx     6940 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/samples/sample_set_get_image_async.py
--rw-rw-r--  2.0 unx     3000 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/samples/sample_set_image_properties.py
--rw-rw-r--  2.0 unx     3314 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/samples/sample_delete_images_async.py
--rw-rw-r--  2.0 unx     2566 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/samples/sample_list_tags.py
--rw-rw-r--  2.0 unx     2694 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/samples/sample_list_tags_async.py
--rw-rw-r--  2.0 unx     3246 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/samples/sample_hello_world.py
--rw-rw-r--  2.0 unx     6689 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/samples/sample_set_get_image.py
--rw-rw-r--  2.0 unx     4356 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/samples/utilities.py
--rw-rw-r--  2.0 unx     2745 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/samples/sample_delete_tags.py
--rw-rw-r--  2.0 unx     3136 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/samples/sample_delete_images.py
--rw-rw-r--  2.0 unx     3388 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/samples/sample_hello_world_async.py
--rw-rw-r--  2.0 unx     2940 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/samples/sample_delete_tags_async.py
--rw-rw-r--  2.0 unx     4698 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/samples/README.md
--rw-rw-r--  2.0 unx     3120 b- defN 23-Apr-26 00:30 azure-containerregistry-1.1.0b4/samples/sample_set_image_properties_async.py
--rw-rw-r--  2.0 unx       41 b- defN 23-Apr-26 00:32 azure-containerregistry-1.1.0b4/azure_containerregistry.egg-info/requires.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Apr-26 00:32 azure-containerregistry-1.1.0b4/azure_containerregistry.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx        6 b- defN 23-Apr-26 00:32 azure-containerregistry-1.1.0b4/azure_containerregistry.egg-info/top_level.txt
--rw-rw-r--  2.0 unx    11022 b- defN 23-Apr-26 00:32 azure-containerregistry-1.1.0b4/azure_containerregistry.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx     3161 b- defN 23-Apr-26 00:32 azure-containerregistry-1.1.0b4/azure_containerregistry.egg-info/SOURCES.txt
-94 files, 743588 bytes uncompressed, 133032 bytes compressed:  82.1%
+Zip file size: 159643 bytes, number of entries: 94
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:43 azure-containerregistry-1.2.0/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:43 azure-containerregistry-1.2.0/samples/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:43 azure-containerregistry-1.2.0/tests/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:43 azure-containerregistry-1.2.0/azure/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:43 azure-containerregistry-1.2.0/azure_containerregistry.egg-info/
+-rw-rw-r--  2.0 unx     1073 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/LICENSE
+-rw-rw-r--  2.0 unx     5462 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/CHANGELOG.md
+-rw-rw-r--  2.0 unx     4279 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/TROUBLESHOOTING.md
+-rw-rw-r--  2.0 unx    16014 b- defN 23-Jul-11 16:43 azure-containerregistry-1.2.0/PKG-INFO
+-rw-rw-r--  2.0 unx     2325 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/setup.py
+-rw-rw-r--  2.0 unx       86 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/pyproject.toml
+-rw-rw-r--  2.0 unx       38 b- defN 23-Jul-11 16:43 azure-containerregistry-1.2.0/setup.cfg
+-rw-rw-r--  2.0 unx    14980 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/README.md
+-rw-rw-r--  2.0 unx      161 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/MANIFEST.in
+-rw-rw-r--  2.0 unx     8110 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/samples/sample_set_get_image.py
+-rw-rw-r--  2.0 unx     3078 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/samples/sample_delete_images_async.py
+-rw-rw-r--  2.0 unx     2811 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/samples/sample_delete_tags_async.py
+-rw-rw-r--  2.0 unx     2290 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/samples/sample_list_tags.py
+-rw-rw-r--  2.0 unx     2910 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/samples/sample_set_image_properties_async.py
+-rw-rw-r--  2.0 unx     4176 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/samples/utilities.py
+-rw-rw-r--  2.0 unx     3045 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/samples/sample_hello_world.py
+-rw-rw-r--  2.0 unx     2968 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/samples/sample_delete_images.py
+-rw-rw-r--  2.0 unx     2357 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/samples/sample_list_tags_async.py
+-rw-rw-r--  2.0 unx     2818 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/samples/sample_set_image_properties.py
+-rw-rw-r--  2.0 unx     7402 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/samples/sample_set_get_image_async.py
+-rw-rw-r--  2.0 unx     3187 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/samples/sample_hello_world_async.py
+-rw-rw-r--  2.0 unx     2616 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/samples/sample_delete_tags.py
+-rw-rw-r--  2.0 unx     4698 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/samples/README.md
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:43 azure-containerregistry-1.2.0/tests/perfstress_tests/
+-rw-rw-r--  2.0 unx     6413 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/tests/testcase.py
+-rw-rw-r--  2.0 unx    40789 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/tests/test_container_registry_client.py
+-rw-rw-r--  2.0 unx     2320 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/tests/conftest.py
+-rw-rw-r--  2.0 unx     8845 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/tests/test_anon_access.py
+-rw-rw-r--  2.0 unx      290 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/tests/constants.py
+-rw-rw-r--  2.0 unx      505 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/tests/preparer.py
+-rw-rw-r--  2.0 unx     3121 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/tests/asynctestcase.py
+-rw-rw-r--  2.0 unx    42755 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/tests/test_container_registry_client_async.py
+-rw-rw-r--  2.0 unx     9315 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/tests/test_anon_access_async.py
+-rw-rw-r--  2.0 unx     1162 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/tests/perfstress_tests/list_repositories.py
+-rw-rw-r--  2.0 unx     1235 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/tests/perfstress_tests/list_artifacts.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/tests/perfstress_tests/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:43 azure-containerregistry-1.2.0/azure/containerregistry/
+-rw-rw-r--  2.0 unx       81 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:43 azure-containerregistry-1.2.0/azure/containerregistry/aio/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:43 azure-containerregistry-1.2.0/azure/containerregistry/_generated/
+-rw-rw-r--  2.0 unx     2919 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/azure/containerregistry/_anonymous_exchange_client.py
+-rw-rw-r--  2.0 unx     4031 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/azure/containerregistry/_authentication_policy.py
+-rw-rw-r--  2.0 unx     4417 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/azure/containerregistry/_exchange_client.py
+-rw-rw-r--  2.0 unx     2625 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/azure/containerregistry/_download_stream.py
+-rw-rw-r--  2.0 unx     2799 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/azure/containerregistry/_base_client.py
+-rw-rw-r--  2.0 unx     1262 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/azure/containerregistry/__init__.py
+-rw-rw-r--  2.0 unx    12381 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/azure/containerregistry/_models.py
+-rw-rw-r--  2.0 unx     5886 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/azure/containerregistry/_helpers.py
+-rw-rw-r--  2.0 unx      248 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/azure/containerregistry/_user_agent.py
+-rw-rw-r--  2.0 unx    49249 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/azure/containerregistry/_container_registry_client.py
+-rw-rw-r--  2.0 unx      170 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/azure/containerregistry/_version.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/azure/containerregistry/py.typed
+-rw-rw-r--  2.0 unx    50611 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/azure/containerregistry/aio/_async_container_registry_client.py
+-rw-rw-r--  2.0 unx     4550 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/azure/containerregistry/aio/_async_exchange_client.py
+-rw-rw-r--  2.0 unx     4150 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/azure/containerregistry/aio/_async_authentication_policy.py
+-rw-rw-r--  2.0 unx      675 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/azure/containerregistry/aio/__init__.py
+-rw-rw-r--  2.0 unx     3129 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/azure/containerregistry/aio/_async_base_client.py
+-rw-rw-r--  2.0 unx     3251 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/azure/containerregistry/aio/_async_anonymous_exchange_client.py
+-rw-rw-r--  2.0 unx     2789 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/azure/containerregistry/aio/_async_download_stream.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:43 azure-containerregistry-1.2.0/azure/containerregistry/_generated/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:43 azure-containerregistry-1.2.0/azure/containerregistry/_generated/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:43 azure-containerregistry-1.2.0/azure/containerregistry/_generated/aio/
+-rw-rw-r--  2.0 unx     1530 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/azure/containerregistry/_generated/_patch.py
+-rw-rw-r--  2.0 unx      722 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/azure/containerregistry/_generated/__init__.py
+-rw-rw-r--  2.0 unx     3326 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/azure/containerregistry/_generated/_configuration.py
+-rw-rw-r--  2.0 unx    78836 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/azure/containerregistry/_generated/_serialization.py
+-rw-rw-r--  2.0 unx     4629 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/azure/containerregistry/_generated/_client.py
+-rw-rw-r--  2.0 unx     1369 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/azure/containerregistry/_generated/_vendor.py
+-rw-rw-r--  2.0 unx      791 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/azure/containerregistry/_generated/models/_patch.py
+-rw-rw-r--  2.0 unx     3412 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/azure/containerregistry/_generated/models/__init__.py
+-rw-rw-r--  2.0 unx     2960 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/azure/containerregistry/_generated/models/_enums.py
+-rw-rw-r--  2.0 unx    64438 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/azure/containerregistry/_generated/models/_models.py
+-rw-rw-r--  2.0 unx    10863 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/azure/containerregistry/_generated/operations/_patch.py
+-rw-rw-r--  2.0 unx      870 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/azure/containerregistry/_generated/operations/__init__.py
+-rw-rw-r--  2.0 unx   103037 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/azure/containerregistry/_generated/operations/_operations.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:43 azure-containerregistry-1.2.0/azure/containerregistry/_generated/aio/operations/
+-rw-rw-r--  2.0 unx     1530 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/azure/containerregistry/_generated/aio/_patch.py
+-rw-rw-r--  2.0 unx      722 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/azure/containerregistry/_generated/aio/__init__.py
+-rw-rw-r--  2.0 unx     3368 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/azure/containerregistry/_generated/aio/_configuration.py
+-rw-rw-r--  2.0 unx     4778 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/azure/containerregistry/_generated/aio/_client.py
+-rw-rw-r--  2.0 unx      845 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/azure/containerregistry/_generated/aio/_vendor.py
+-rw-rw-r--  2.0 unx     8679 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/azure/containerregistry/_generated/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx      870 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/azure/containerregistry/_generated/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx    80761 b- defN 23-Jul-11 16:42 azure-containerregistry-1.2.0/azure/containerregistry/_generated/aio/operations/_operations.py
+-rw-rw-r--  2.0 unx        6 b- defN 23-Jul-11 16:43 azure-containerregistry-1.2.0/azure_containerregistry.egg-info/top_level.txt
+-rw-rw-r--  2.0 unx       41 b- defN 23-Jul-11 16:43 azure-containerregistry-1.2.0/azure_containerregistry.egg-info/requires.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jul-11 16:43 azure-containerregistry-1.2.0/azure_containerregistry.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx    16014 b- defN 23-Jul-11 16:43 azure-containerregistry-1.2.0/azure_containerregistry.egg-info/PKG-INFO
+-rw-rw-r--  2.0 unx     3161 b- defN 23-Jul-11 16:43 azure-containerregistry-1.2.0/azure_containerregistry.egg-info/SOURCES.txt
+94 files, 766416 bytes uncompressed, 139957 bytes compressed:  81.7%
```

## zipnote {}

```diff
@@ -1,283 +1,283 @@
-Filename: azure-containerregistry-1.1.0b4/
+Filename: azure-containerregistry-1.2.0/
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/tests/
+Filename: azure-containerregistry-1.2.0/samples/
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/
+Filename: azure-containerregistry-1.2.0/tests/
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/samples/
+Filename: azure-containerregistry-1.2.0/azure/
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure_containerregistry.egg-info/
+Filename: azure-containerregistry-1.2.0/azure_containerregistry.egg-info/
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/setup.py
+Filename: azure-containerregistry-1.2.0/LICENSE
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/setup.cfg
+Filename: azure-containerregistry-1.2.0/CHANGELOG.md
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/MANIFEST.in
+Filename: azure-containerregistry-1.2.0/TROUBLESHOOTING.md
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/pyproject.toml
+Filename: azure-containerregistry-1.2.0/PKG-INFO
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/CHANGELOG.md
+Filename: azure-containerregistry-1.2.0/setup.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/PKG-INFO
+Filename: azure-containerregistry-1.2.0/pyproject.toml
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/TROUBLESHOOTING.md
+Filename: azure-containerregistry-1.2.0/setup.cfg
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/LICENSE
+Filename: azure-containerregistry-1.2.0/README.md
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/README.md
+Filename: azure-containerregistry-1.2.0/MANIFEST.in
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/tests/perfstress_tests/
+Filename: azure-containerregistry-1.2.0/samples/sample_set_get_image.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/tests/testcase.py
+Filename: azure-containerregistry-1.2.0/samples/sample_delete_images_async.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/tests/conftest.py
+Filename: azure-containerregistry-1.2.0/samples/sample_delete_tags_async.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/tests/test_container_registry_client.py
+Filename: azure-containerregistry-1.2.0/samples/sample_list_tags.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/tests/test_anon_access_async.py
+Filename: azure-containerregistry-1.2.0/samples/sample_set_image_properties_async.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/tests/asynctestcase.py
+Filename: azure-containerregistry-1.2.0/samples/utilities.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/tests/test_anon_access.py
+Filename: azure-containerregistry-1.2.0/samples/sample_hello_world.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/tests/constants.py
+Filename: azure-containerregistry-1.2.0/samples/sample_delete_images.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/tests/preparer.py
+Filename: azure-containerregistry-1.2.0/samples/sample_list_tags_async.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/tests/test_container_registry_client_async.py
+Filename: azure-containerregistry-1.2.0/samples/sample_set_image_properties.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/tests/perfstress_tests/__init__.py
+Filename: azure-containerregistry-1.2.0/samples/sample_set_get_image_async.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/tests/perfstress_tests/list_artifacts.py
+Filename: azure-containerregistry-1.2.0/samples/sample_hello_world_async.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/tests/perfstress_tests/list_repositories.py
+Filename: azure-containerregistry-1.2.0/samples/sample_delete_tags.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/
+Filename: azure-containerregistry-1.2.0/samples/README.md
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/__init__.py
+Filename: azure-containerregistry-1.2.0/tests/perfstress_tests/
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/
+Filename: azure-containerregistry-1.2.0/tests/testcase.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/aio/
+Filename: azure-containerregistry-1.2.0/tests/test_container_registry_client.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_download_stream.py
+Filename: azure-containerregistry-1.2.0/tests/conftest.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/__init__.py
+Filename: azure-containerregistry-1.2.0/tests/test_anon_access.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_exchange_client.py
+Filename: azure-containerregistry-1.2.0/tests/constants.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_models.py
+Filename: azure-containerregistry-1.2.0/tests/preparer.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_base_client.py
+Filename: azure-containerregistry-1.2.0/tests/asynctestcase.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_authentication_policy.py
+Filename: azure-containerregistry-1.2.0/tests/test_container_registry_client_async.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_user_agent.py
+Filename: azure-containerregistry-1.2.0/tests/test_anon_access_async.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_container_registry_client.py
+Filename: azure-containerregistry-1.2.0/tests/perfstress_tests/list_repositories.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_anonymous_exchange_client.py
+Filename: azure-containerregistry-1.2.0/tests/perfstress_tests/list_artifacts.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_version.py
+Filename: azure-containerregistry-1.2.0/tests/perfstress_tests/__init__.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_helpers.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/py.typed
+Filename: azure-containerregistry-1.2.0/azure/__init__.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/models/
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/aio/
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/_generated/
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/operations/
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/_anonymous_exchange_client.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/_client.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/_authentication_policy.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/__init__.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/_exchange_client.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/_configuration.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/_download_stream.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/_patch.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/_base_client.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/_vendor.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/__init__.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/_serialization.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/_models.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/models/__init__.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/_helpers.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/models/_models.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/_user_agent.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/models/_patch.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/_container_registry_client.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/models/_enums.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/_version.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/operations/
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/py.typed
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/_client.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/aio/_async_container_registry_client.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/__init__.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/aio/_async_exchange_client.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/_configuration.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/aio/_async_authentication_policy.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/_patch.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/aio/__init__.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/_vendor.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/aio/_async_base_client.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/operations/__init__.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/aio/_async_anonymous_exchange_client.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/operations/_patch.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/aio/_async_download_stream.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/operations/_operations.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/_generated/models/
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/operations/__init__.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/_generated/operations/
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/operations/_patch.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/_generated/aio/
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/operations/_operations.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/_generated/_patch.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/aio/_async_container_registry_client.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/_generated/__init__.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/aio/_async_authentication_policy.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/_generated/_configuration.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/aio/_async_anonymous_exchange_client.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/_generated/_serialization.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/aio/__init__.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/_generated/_client.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/aio/_async_download_stream.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/_generated/_vendor.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/aio/_async_exchange_client.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/_generated/models/_patch.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure/containerregistry/aio/_async_base_client.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/_generated/models/__init__.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/samples/sample_set_get_image_async.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/_generated/models/_enums.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/samples/sample_set_image_properties.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/_generated/models/_models.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/samples/sample_delete_images_async.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/_generated/operations/_patch.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/samples/sample_list_tags.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/_generated/operations/__init__.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/samples/sample_list_tags_async.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/_generated/operations/_operations.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/samples/sample_hello_world.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/_generated/aio/operations/
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/samples/sample_set_get_image.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/_generated/aio/_patch.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/samples/utilities.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/_generated/aio/__init__.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/samples/sample_delete_tags.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/_generated/aio/_configuration.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/samples/sample_delete_images.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/_generated/aio/_client.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/samples/sample_hello_world_async.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/_generated/aio/_vendor.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/samples/sample_delete_tags_async.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/_generated/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/samples/README.md
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/_generated/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/samples/sample_set_image_properties_async.py
+Filename: azure-containerregistry-1.2.0/azure/containerregistry/_generated/aio/operations/_operations.py
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure_containerregistry.egg-info/requires.txt
+Filename: azure-containerregistry-1.2.0/azure_containerregistry.egg-info/top_level.txt
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure_containerregistry.egg-info/dependency_links.txt
+Filename: azure-containerregistry-1.2.0/azure_containerregistry.egg-info/requires.txt
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure_containerregistry.egg-info/top_level.txt
+Filename: azure-containerregistry-1.2.0/azure_containerregistry.egg-info/dependency_links.txt
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure_containerregistry.egg-info/PKG-INFO
+Filename: azure-containerregistry-1.2.0/azure_containerregistry.egg-info/PKG-INFO
 Comment: 
 
-Filename: azure-containerregistry-1.1.0b4/azure_containerregistry.egg-info/SOURCES.txt
+Filename: azure-containerregistry-1.2.0/azure_containerregistry.egg-info/SOURCES.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-containerregistry-1.1.0b4/setup.py` & `azure-containerregistry-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     long_description_content_type="text/markdown",
     url="https://github.com/Azure/azure-sdk-for-python",
     author="Microsoft Corporation",
     author_email="azuresdkengsysadmins@microsoft.com",
     license="MIT License",
     # ensure that the development status reflects the status of your package
     classifiers=[
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
```

## Comparing `azure-containerregistry-1.1.0b4/CHANGELOG.md` & `azure-containerregistry-1.2.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,25 @@
 # Release History
 
+## 1.2.0 (2023-07-11)
+
+### Bugs Fixed
+- Fixed a bug when deserializing unknown architecture and os values in `ArtifactManifestProperties` object. ([#28469](https://github.com/Azure/azure-sdk-for-python/issues/28469) [#30077](https://github.com/Azure/azure-sdk-for-python/issues/30077))
+
+### Other Changes
+- Enum type properties in `ArtifactManifestProperties` class would be type `str` when its value is not in enum's known list.
+
+## 1.1.0 (2023-05-17)
+
+### Breaking Changes
+- Added sanity check for manifest size at download time - if manifest is bigger than 4MB, `ValueError` will be thrown.
+
+### Other Changes
+- Changed the digest validation exception type to `DigestValidationError` in `set/get manifest` and `upload/download blob` operations.
+
 ## 1.1.0b4 (2023-04-25)
 
 ### Features Added
 - Added an optional kwarg `media_type` in `set_manifest()` to enable uploading image manifests of any type.
 
 ### Breaking Changes
 - Renamed `upload_manifest()` to `set_manifest()`, and changed to consume manifest in `JSON` instead of `OCIManifest` type.
```

## Comparing `azure-containerregistry-1.1.0b4/TROUBLESHOOTING.md` & `azure-containerregistry-1.2.0/TROUBLESHOOTING.md`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b4/LICENSE` & `azure-containerregistry-1.2.0/LICENSE`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b4/tests/testcase.py` & `azure-containerregistry-1.2.0/tests/testcase.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,47 +1,37 @@
 # coding=utf-8
 # ------------------------------------
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 # ------------------------------------
 import logging
 import os
-import pytest
+import json
+from io import BytesIO
 
 from azure.containerregistry import ContainerRegistryClient
 from azure.containerregistry._helpers import _is_tag
+from azure.identity import AzureAuthorityHosts, ClientSecretCredential
 
-from azure.mgmt.containerregistry import ContainerRegistryManagementClient
-from azure.mgmt.containerregistry.models import ImportImageParameters, ImportSource, ImportMode
-from azure.identity import DefaultAzureCredential, AzureAuthorityHosts, ClientSecretCredential
-
-from devtools_testutils import AzureRecordedTestCase, is_live, FakeTokenCredential
+from devtools_testutils import AzureRecordedTestCase, FakeTokenCredential
 
 logger = logging.getLogger()
 
 
 class ContainerRegistryTestClass(AzureRecordedTestCase):
-    def import_image(self, endpoint, repository, tags, is_anonymous=False):
+    def import_image(self, endpoint, repository, tags):
         # repository must be a docker hub repository
         # tags is a List of repository/tag combos in the format <repository>:<tag>
         if not self.is_live:
             return
-        authority = get_authority(endpoint)
-        import_image(authority, repository, tags, is_anonymous=is_anonymous)
+        import_image(endpoint, repository, tags)
 
     def get_credential(self, authority=None, **kwargs):
         if self.is_live:
-            if authority != AzureAuthorityHosts.AZURE_PUBLIC_CLOUD:
-                return ClientSecretCredential(
-                    tenant_id=os.environ.get("CONTAINERREGISTRY_TENANT_ID"),
-                    client_id=os.environ.get("CONTAINERREGISTRY_CLIENT_ID"),
-                    client_secret=os.environ.get("CONTAINERREGISTRY_CLIENT_SECRET"),
-                    authority=authority
-                )
-            return DefaultAzureCredential(**kwargs)
+            return get_credential(authority)
         return FakeTokenCredential()
 
     def create_registry_client(self, endpoint, **kwargs):
         authority = get_authority(endpoint)
         audience = kwargs.pop("audience", None)
         if not audience:
             audience = get_audience(authority)
@@ -65,17 +55,14 @@
         assert properties.can_delete == value
         assert properties.can_read == value
         assert properties.can_write == value
         assert properties.can_list == value
 
     def create_fully_qualified_reference(self, registry, repository, digest):
         return f"{registry}/{repository}{':' if _is_tag(digest) else '@'}{digest.split(':')[-1]}"
-
-    def is_public_endpoint(self, endpoint):
-        return ".azurecr.io" in endpoint
     
     def upload_oci_manifest_prerequisites(self, repo, client):
         layer = "654b93f61054e4ce90ed203bb8d556a6200d5f906cf3eca0620738d6dc18cbed"
         config = "config.json"
         base_path = os.path.join(self.get_test_directory(), "data", "oci_artifact")
         # upload config
         client.upload_blob(repo, open(os.path.join(base_path, config), "rb"))
@@ -91,14 +78,17 @@
         # upload layers
         client.upload_blob(repo, open(os.path.join(base_path, layer), "rb"))
 
     def get_test_directory(self):
         return os.path.join(os.getcwd(), "tests")
 
 
+def is_public_endpoint(endpoint):
+    return ".azurecr.io" in endpoint
+
 def get_authority(endpoint: str) -> str:
     if ".azurecr.io" in endpoint:
         logger.warning("Public cloud Authority")
         return AzureAuthorityHosts.AZURE_PUBLIC_CLOUD
     if ".azurecr.cn" in endpoint:
         logger.warning("China Authority")
         return AzureAuthorityHosts.AZURE_CHINA
@@ -114,69 +104,51 @@
     if authority == AzureAuthorityHosts.AZURE_CHINA:
         logger.warning("China cloud auth audience")
         return "https://management.chinacloudapi.cn"
     if authority == AzureAuthorityHosts.AZURE_GOVERNMENT:
         logger.warning("US Gov cloud auth audience")
         return "https://management.usgovcloudapi.net"
 
-def import_image(authority, repository, tags, is_anonymous=False):
-    logger.warning(f"Import image authority: {authority}")
-    if is_anonymous:
-        registry_name = os.environ.get("CONTAINERREGISTRY_ANONREGISTRY_NAME")
-    else:
-        registry_name = os.environ.get("CONTAINERREGISTRY_REGISTRY_NAME")
-    sub_id = os.environ.get("CONTAINERREGISTRY_SUBSCRIPTION_ID")
-    tenant_id=os.environ.get("CONTAINERREGISTRY_TENANT_ID")
-    client_id=os.environ.get("CONTAINERREGISTRY_CLIENT_ID")
-    client_secret=os.environ.get("CONTAINERREGISTRY_CLIENT_SECRET")
-    credential = ClientSecretCredential(
-        tenant_id=tenant_id, client_id=client_id, client_secret=client_secret, authority=authority
-    )
-    audience = get_audience(authority)
-    scope = [audience + "/.default"]
-    mgmt_client = ContainerRegistryManagementClient(
-        credential, sub_id, api_version="2019-05-01", base_url=audience, credential_scopes=scope
-    )
-    logger.warning(f"LOGGING: {sub_id}{tenant_id}")
-    registry_uri = "registry.hub.docker.com"
-    rg_name = os.environ.get("CONTAINERREGISTRY_RESOURCE_GROUP")
-
-    import_source = ImportSource(source_image=repository, registry_uri=registry_uri)
-
-    import_params = ImportImageParameters(mode=ImportMode.Force, source=import_source, target_tags=tags)
-
-    result = mgmt_client.registries.begin_import_image(
-        rg_name,
-        registry_name,
-        parameters=import_params,
+def get_credential(authority: str, **kwargs):
+    return ClientSecretCredential(
+        tenant_id=os.environ.get("CONTAINERREGISTRY_TENANT_ID"),
+        client_id=os.environ.get("CONTAINERREGISTRY_CLIENT_ID"),
+        client_secret=os.environ.get("CONTAINERREGISTRY_CLIENT_SECRET"),
+        authority=authority
     )
 
-    result.wait()
+def import_image(endpoint, repository, tags):
+    authority = get_authority(endpoint)
+    logger.warning(f"Import image authority: {authority}")
+    credential = get_credential(authority)
 
-@pytest.fixture(scope="session")
-def load_registry():
-    if not is_live():
-        return
-    authority = get_authority(os.environ.get("CONTAINERREGISTRY_ENDPOINT"))
-    authority_anon = get_authority(os.environ.get("CONTAINERREGISTRY_ANONREGISTRY_ENDPOINT"))
-    repos = [
-        "library/hello-world",
-        "library/alpine",
-        "library/busybox",
-    ]
-    tags = [
-        [
-            "library/hello-world:latest",
-            "library/hello-world:v1",
-            "library/hello-world:v2",
-            "library/hello-world:v3",
-            "library/hello-world:v4",
-        ],
-        ["library/alpine"],
-        ["library/busybox"],
-    ]
-    for repo, tag in zip(repos, tags):
-        try:
-            import_image(authority, repo, tag)
-            import_image(authority_anon, repo, tag, is_anonymous=True)
-        except Exception as e:
-            print(e)
+    with ContainerRegistryClient(endpoint, credential) as client:
+        # Upload a layer
+        layer = BytesIO(b"Sample layer")
+        layer_digest, layer_size = client.upload_blob(repository, layer)
+        logger.info(f"Uploaded layer: digest - {layer_digest}, size - {layer_size}")
+        # Upload a config
+        config = BytesIO(json.dumps({"sample config": "content"}).encode())
+        config_digest, config_size = client.upload_blob(repository, config)
+        logger.info(f"Uploaded config: digest - {config_digest}, size - {config_size}")
+        # Upload images
+        oci_manifest = {
+            "config": {
+                "mediaType": "application/vnd.oci.image.config.v1+json",
+                "digest": config_digest,
+                "sizeInBytes": config_size,
+            },
+            "schemaVersion": 2,
+            "layers": [
+                {
+                    "mediaType": "application/vnd.oci.image.layer.v1.tar",
+                    "digest": layer_digest,
+                    "size": layer_size,
+                    "annotations": {
+                        "org.opencontainers.image.ref.name": "artifact.txt",
+                    },
+                },
+            ],
+        }
+        for tag in tags:
+            manifest_digest = client.set_manifest(repository, oci_manifest, tag=tag)
+            logger.info(f"Uploaded manifest: digest - {manifest_digest}")
```

## Comparing `azure-containerregistry-1.1.0b4/tests/conftest.py` & `azure-containerregistry-1.2.0/tests/conftest.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,44 @@
 # coding: utf-8
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
-
+import logging
 import os
-
 import pytest
-from devtools_testutils import add_general_regex_sanitizer, add_body_key_sanitizer, add_uri_regex_sanitizer, test_proxy
+from devtools_testutils import (
+    add_general_regex_sanitizer,
+    add_body_key_sanitizer,
+    add_uri_regex_sanitizer,
+    test_proxy,
+    is_live,
+)
+from testcase import import_image, is_public_endpoint
+from constants import HELLO_WORLD
 
-# Fixture
-from testcase import load_registry
+logger = logging.getLogger()
 
-
-def pytest_configure(config):
-    config.addinivalue_line("usefixtures", "load_registry")
+@pytest.fixture(scope="session", autouse=True)
+def load_registry():
+    if not is_live():
+        return
+    logger.info("loading registry")
+    endpoint = os.environ.get("CONTAINERREGISTRY_ENDPOINT")
+    endpoint_anon = os.environ.get("CONTAINERREGISTRY_ANONREGISTRY_ENDPOINT")
+    repo = HELLO_WORLD
+    tags = ["latest", "v1"]
+    try:
+        import_image(endpoint, repo, tags)
+        if is_public_endpoint(endpoint_anon):
+            import_image(endpoint_anon, repo, tags)
+    except Exception as e:
+        logger.exception(e)
+        raise
 
 @pytest.fixture(scope="session", autouse=True)
 def add_sanitizers(test_proxy):
     # sanitizes access and refresh tokens that are present in single-string request or response bodies
     # we expect tokens to either be at the end of this body string, or followed by "\u0026" and more content
     add_general_regex_sanitizer(value="access_token", regex="(?<=access_token=).*?(?=(?:\\u0026|$))")
     add_general_regex_sanitizer(value="refresh_token", regex="(?<=refresh_token=).*?(?=(?:\\u0026|$))")
```

## Comparing `azure-containerregistry-1.1.0b4/tests/test_container_registry_client.py` & `azure-containerregistry-1.2.0/tests/test_container_registry_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,44 @@
 # coding=utf-8
 # ------------------------------------
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 # ------------------------------------
 import os
 import pytest
-import six
 import hashlib
 import json
 from datetime import datetime
 from io import BytesIO
+from unittest.mock import MagicMock
+from typing import Optional, Iterator, Any, MutableMapping
 from azure.containerregistry import (
     RepositoryProperties,
     ArtifactManifestProperties,
     ArtifactManifestOrder,
     ArtifactTagProperties,
     ArtifactTagOrder,
+    ArtifactArchitecture,
+    ArtifactOperatingSystem,
     ContainerRegistryClient,
+    DigestValidationError,
 )
 from azure.containerregistry._helpers import DOCKER_MANIFEST, OCI_IMAGE_MANIFEST, DEFAULT_CHUNK_SIZE
-from azure.core.exceptions import ResourceNotFoundError, ClientAuthenticationError, HttpResponseError
+from azure.core.exceptions import (
+    ResourceNotFoundError,
+    ClientAuthenticationError,
+    HttpResponseError,
+    ServiceRequestError,
+    ServiceResponseError,
+)
 from azure.core.paging import ItemPaged
+from azure.core.pipeline import PipelineRequest
 from azure.identity import AzureAuthorityHosts
-from testcase import ContainerRegistryTestClass, get_authority, get_audience
-from constants import HELLO_WORLD, ALPINE, BUSYBOX, DOES_NOT_EXIST
+from testcase import ContainerRegistryTestClass, get_authority, get_audience, is_public_endpoint
+from constants import HELLO_WORLD, DOES_NOT_EXIST
 from preparer import acr_preparer
 from devtools_testutils import recorded_by_proxy
 
 
 class TestContainerRegistryClient(ContainerRegistryTestClass):
     @acr_preparer()
     @recorded_by_proxy
@@ -36,15 +47,15 @@
             repositories = client.list_repository_names()
             assert isinstance(repositories, ItemPaged)
 
             count = 0
             prev = None
             for repo in repositories:
                 count += 1
-                assert isinstance(repo, six.string_types)
+                assert isinstance(repo, str)
                 assert prev != repo
                 prev = repo
 
             assert count > 0
 
     @acr_preparer()
     @recorded_by_proxy
@@ -55,55 +66,56 @@
 
             repository_pages = client.list_repository_names(results_per_page=results_per_page)
 
             prev = None
             for page in repository_pages.by_page():
                 page_count = 0
                 for repo in page:
-                    assert isinstance(repo, six.string_types)
+                    assert isinstance(repo, str)
                     assert prev != repo
                     prev = repo
                     page_count += 1
                 assert page_count <= results_per_page
                 total_pages += 1
 
             assert total_pages >= 1
 
     @acr_preparer()
     @recorded_by_proxy
     def test_delete_repository(self, containerregistry_endpoint):
         repo = self.get_resource_name("repo")
-        self.import_image(containerregistry_endpoint, HELLO_WORLD, [repo])
+        self.import_image(containerregistry_endpoint, repo, ["test"])
+        self.sleep(5)
         with self.create_registry_client(containerregistry_endpoint) as client:
             client.delete_repository(repo)
 
-            self.sleep(10)
+            self.sleep(5)
             with pytest.raises(ResourceNotFoundError):
                 client.get_repository_properties(repo)
 
     @acr_preparer()
     @recorded_by_proxy
     def test_delete_repository_does_not_exist(self, containerregistry_endpoint):
         with self.create_registry_client(containerregistry_endpoint) as client:
             client.delete_repository(DOES_NOT_EXIST)
 
     @acr_preparer()
     @recorded_by_proxy
     def test_get_repository_properties(self, containerregistry_endpoint):
         with self.create_registry_client(containerregistry_endpoint) as client:
-            properties = client.get_repository_properties(ALPINE)
+            properties = client.get_repository_properties(HELLO_WORLD)
             assert isinstance(properties, RepositoryProperties)
-            assert properties.name == ALPINE
+            assert properties.name == HELLO_WORLD
 
     @acr_preparer()
     @recorded_by_proxy
     def test_update_repository_properties(self, containerregistry_endpoint):
         repo = self.get_resource_name("repo")
-        tag = self.get_resource_name("tag")
-        self.import_image(containerregistry_endpoint, HELLO_WORLD, [f"{repo}:{tag}"])
+        self.import_image(containerregistry_endpoint, repo, ["test"])
+        self.sleep(5)
         with self.create_registry_client(containerregistry_endpoint) as client:
             properties = self.set_all_properties(RepositoryProperties(), False)
             received = client.update_repository_properties(repo, properties)
             self.assert_all_properties(received, False)
 
             properties = self.set_all_properties(properties, True)
             received = client.update_repository_properties(repo, properties)
@@ -112,17 +124,16 @@
             # Cleanup
             client.delete_repository(repo)
 
     @acr_preparer()
     @recorded_by_proxy
     def test_update_repository_properties_kwargs(self, containerregistry_endpoint):
         repo = self.get_resource_name("repo")
-        tag = self.get_resource_name("tag")
-        self.import_image(containerregistry_endpoint, HELLO_WORLD, [f"{repo}:{tag}"])
-
+        self.import_image(containerregistry_endpoint, repo, ["test"])
+        self.sleep(5)
         with self.create_registry_client(containerregistry_endpoint) as client:
             received = client.update_repository_properties(
                 repo, can_delete=False, can_read=False, can_write=False, can_list=False
             )
             self.assert_all_properties(received, False)
 
             received = client.update_repository_properties(
@@ -134,31 +145,31 @@
             client.delete_repository(repo)
 
     @acr_preparer()
     @recorded_by_proxy
     def test_list_registry_artifacts(self, containerregistry_endpoint):
         with self.create_registry_client(containerregistry_endpoint) as client:
             count = 0
-            for artifact in client.list_manifest_properties(BUSYBOX):
+            for artifact in client.list_manifest_properties(HELLO_WORLD):
                 assert isinstance(artifact, ArtifactManifestProperties)
                 assert isinstance(artifact.created_on, datetime)
                 assert isinstance(artifact.last_updated_on, datetime)
-                assert artifact.repository_name == BUSYBOX
-                assert artifact.fully_qualified_reference in self.create_fully_qualified_reference(containerregistry_endpoint, BUSYBOX, artifact.digest)
+                assert artifact.repository_name == HELLO_WORLD
+                assert artifact.fully_qualified_reference in self.create_fully_qualified_reference(containerregistry_endpoint, HELLO_WORLD, artifact.digest)
                 count += 1
 
             assert count > 0
 
     @acr_preparer()
     @recorded_by_proxy
     def test_list_registry_artifacts_by_page(self, containerregistry_endpoint):
         with self.create_registry_client(containerregistry_endpoint) as client:
             results_per_page = 2
 
-            pages = client.list_manifest_properties(BUSYBOX, results_per_page=results_per_page)
+            pages = client.list_manifest_properties(HELLO_WORLD, results_per_page=results_per_page)
             page_count = 0
             for page in pages.by_page():
                 reg_count = 0
                 for tag in page:
                     reg_count += 1
                 assert reg_count <= results_per_page
                 page_count += 1
@@ -167,64 +178,64 @@
 
     @acr_preparer()
     @recorded_by_proxy
     def test_list_registry_artifacts_descending(self, containerregistry_endpoint):
         with self.create_registry_client(containerregistry_endpoint) as client:
             prev_last_updated_on = None
             count = 0
-            for artifact in client.list_manifest_properties(BUSYBOX, order_by=ArtifactManifestOrder.LAST_UPDATED_ON_DESCENDING):
+            for artifact in client.list_manifest_properties(HELLO_WORLD, order_by=ArtifactManifestOrder.LAST_UPDATED_ON_DESCENDING):
                 if prev_last_updated_on:
                     assert artifact.last_updated_on < prev_last_updated_on
                 prev_last_updated_on = artifact.last_updated_on
                 count += 1
 
             assert count > 0
 
     @acr_preparer()
     @recorded_by_proxy
     def test_list_registry_artifacts_ascending(self, containerregistry_endpoint):
         with self.create_registry_client(containerregistry_endpoint) as client:
             prev_last_updated_on = None
             count = 0
-            for artifact in client.list_manifest_properties(BUSYBOX, order_by=ArtifactManifestOrder.LAST_UPDATED_ON_ASCENDING):
+            for artifact in client.list_manifest_properties(HELLO_WORLD, order_by=ArtifactManifestOrder.LAST_UPDATED_ON_ASCENDING):
                 if prev_last_updated_on:
                     assert artifact.last_updated_on > prev_last_updated_on
                 prev_last_updated_on = artifact.last_updated_on
                 count += 1
 
             assert count > 0
 
     @acr_preparer()
     @recorded_by_proxy
     def test_get_manifest_properties(self, containerregistry_endpoint):
         with self.create_registry_client(containerregistry_endpoint) as client:
-            properties = client.get_manifest_properties(ALPINE, "latest")
+            properties = client.get_manifest_properties(HELLO_WORLD, "latest")
             assert isinstance(properties, ArtifactManifestProperties)
-            assert properties.repository_name == ALPINE
-            assert properties.fully_qualified_reference in self.create_fully_qualified_reference(containerregistry_endpoint, ALPINE, properties.digest)
+            assert properties.repository_name == HELLO_WORLD
+            assert properties.fully_qualified_reference in self.create_fully_qualified_reference(containerregistry_endpoint, HELLO_WORLD, properties.digest)
 
     @acr_preparer()
     @recorded_by_proxy
     def test_get_manifest_properties_does_not_exist(self, containerregistry_endpoint):
         with self.create_registry_client(containerregistry_endpoint) as client:
-            manifest = client.get_manifest_properties(ALPINE, "latest")
+            manifest = client.get_manifest_properties(HELLO_WORLD, "latest")
             invalid_digest = manifest.digest[:-10] + u"a" * 10
 
             with pytest.raises(ResourceNotFoundError):
-                client.get_manifest_properties(ALPINE, invalid_digest)
+                client.get_manifest_properties(HELLO_WORLD, invalid_digest)
             with pytest.raises(ResourceNotFoundError):
                 client.get_manifest_properties(DOES_NOT_EXIST, DOES_NOT_EXIST)
 
     @acr_preparer()
     @recorded_by_proxy
     def test_update_manifest_properties(self, containerregistry_endpoint):
         repo = self.get_resource_name("repo")
-        tag = self.get_resource_name("tag")
-        self.import_image(containerregistry_endpoint, HELLO_WORLD, [f"{repo}:{tag}"])
-
+        tag = "test"
+        self.import_image(containerregistry_endpoint, repo, [tag])
+        self.sleep(5)
         with self.create_registry_client(containerregistry_endpoint) as client:
             properties = self.set_all_properties(ArtifactManifestProperties(), False)
             received = client.update_manifest_properties(repo, tag, properties)
             self.assert_all_properties(received, False)
 
             properties = self.set_all_properties(properties, True)
             received = client.update_manifest_properties(repo, tag, properties)
@@ -233,17 +244,17 @@
             # Cleanup
             client.delete_repository(repo)
 
     @acr_preparer()
     @recorded_by_proxy
     def test_update_manifest_properties_kwargs(self, containerregistry_endpoint):
         repo = self.get_resource_name("repo")
-        tag = self.get_resource_name("tag")
-        self.import_image(containerregistry_endpoint, HELLO_WORLD, [f"{repo}:{tag}"])
-
+        tag = "test"
+        self.import_image(containerregistry_endpoint, repo, [tag])
+        self.sleep(5)
         with self.create_registry_client(containerregistry_endpoint) as client:
             received = client.update_manifest_properties(
                 repo, tag, can_delete=False, can_read=False, can_write=False, can_list=False
             )
             self.assert_all_properties(received, False)
 
             received = client.update_manifest_properties(
@@ -254,34 +265,34 @@
             # Cleanup
             client.delete_repository(repo)
 
     @acr_preparer()
     @recorded_by_proxy
     def test_get_tag_properties(self, containerregistry_endpoint):
         with self.create_registry_client(containerregistry_endpoint) as client:
-            properties = client.get_tag_properties(ALPINE, "latest")
+            properties = client.get_tag_properties(HELLO_WORLD, "latest")
             assert isinstance(properties, ArtifactTagProperties)
             assert properties.name == "latest"
 
     @acr_preparer()
     @recorded_by_proxy
     def test_get_tag_properties_does_not_exist(self, containerregistry_endpoint):
         with self.create_registry_client(containerregistry_endpoint) as client:
             with pytest.raises(ResourceNotFoundError):
                 client.get_tag_properties(DOES_NOT_EXIST, DOES_NOT_EXIST)
             with pytest.raises(ResourceNotFoundError):
-                client.get_tag_properties(ALPINE, DOES_NOT_EXIST)
+                client.get_tag_properties(HELLO_WORLD, DOES_NOT_EXIST)
 
     @acr_preparer()
     @recorded_by_proxy
     def test_update_tag_properties(self, containerregistry_endpoint):
         repo = self.get_resource_name("repo")
-        tag = self.get_resource_name("tag")
-        self.import_image(containerregistry_endpoint, HELLO_WORLD, [f"{repo}:{tag}"])
-
+        tag = "test"
+        self.import_image(containerregistry_endpoint, repo, [tag])
+        self.sleep(5)
         with self.create_registry_client(containerregistry_endpoint) as client:
             properties = self.set_all_properties(ArtifactTagProperties(), False)
             received = client.update_tag_properties(repo, tag, properties)
             self.assert_all_properties(received, False)
 
             properties = self.set_all_properties(properties, True)
             received = client.update_tag_properties(repo, tag, properties)
@@ -290,17 +301,17 @@
             # Cleanup
             client.delete_repository(repo)
 
     @acr_preparer()
     @recorded_by_proxy
     def test_update_tag_properties_kwargs(self, containerregistry_endpoint):
         repo = self.get_resource_name("repo")
-        tag = self.get_resource_name("tag")
-        self.import_image(containerregistry_endpoint, HELLO_WORLD, [f"{repo}:{tag}"])
-
+        tag = "test"
+        self.import_image(containerregistry_endpoint, repo, [tag])
+        self.sleep(5)
         with self.create_registry_client(containerregistry_endpoint) as client:
             received = client.update_tag_properties(
                 repo, tag, can_delete=False, can_read=False, can_write=False, can_list=False
             )
             self.assert_all_properties(received, False)
 
             received = client.update_tag_properties(
@@ -310,59 +321,55 @@
 
             # Cleanup
             client.delete_repository(repo)
 
     @acr_preparer()
     @recorded_by_proxy
     def test_list_tag_properties(self, containerregistry_endpoint):
-        tags = [f"{ALPINE}:latest"]
+        tags = ["latest", "v1"]
         with self.create_registry_client(containerregistry_endpoint) as client:
             count = 0
-            for tag in client.list_tag_properties(ALPINE):
-                assert f"{ALPINE}:{tag.name}" in tags
+            for tag in client.list_tag_properties(HELLO_WORLD):
+                assert tag.name in tags
                 count += 1
-            assert count == 1
+            assert count == len(tags)
 
     @acr_preparer()
     @recorded_by_proxy
     def test_list_tag_properties_order_descending(self, containerregistry_endpoint):
-        tags = [f"{ALPINE}:latest"]
         with self.create_registry_client(containerregistry_endpoint) as client:
             prev_last_updated_on = None
             count = 0
-            for tag in client.list_tag_properties(ALPINE, order_by=ArtifactTagOrder.LAST_UPDATED_ON_DESCENDING):
-                assert f"{ALPINE}:{tag.name}" in tags
+            for tag in client.list_tag_properties(HELLO_WORLD, order_by=ArtifactTagOrder.LAST_UPDATED_ON_DESCENDING):
                 if prev_last_updated_on:
                     assert tag.last_updated_on < prev_last_updated_on
                 prev_last_updated_on = tag.last_updated_on
                 count += 1
-            assert count == 1
+            assert count == 2
 
     @acr_preparer()
     @recorded_by_proxy
     def test_list_tag_properties_order_ascending(self, containerregistry_endpoint):
-        tags = [f"{ALPINE}:latest"]
         with self.create_registry_client(containerregistry_endpoint) as client:
             prev_last_updated_on = None
             count = 0
-            for tag in client.list_tag_properties(ALPINE, order_by=ArtifactTagOrder.LAST_UPDATED_ON_ASCENDING):
-                assert f"{ALPINE}:{tag.name}" in tags
+            for tag in client.list_tag_properties(HELLO_WORLD, order_by=ArtifactTagOrder.LAST_UPDATED_ON_ASCENDING):
                 if prev_last_updated_on:
                     assert tag.last_updated_on > prev_last_updated_on
                 prev_last_updated_on = tag.last_updated_on
                 count += 1
-            assert count == 1
+            assert count == 2
 
     @acr_preparer()
     @recorded_by_proxy
     def test_delete_tag(self, containerregistry_endpoint):
         repo = self.get_resource_name("repo")
-        tag = self.get_resource_name("tag")
-        self.import_image(containerregistry_endpoint, HELLO_WORLD, [f"{repo}:{tag}"])
-
+        tag = "test"
+        self.import_image(containerregistry_endpoint, repo, [tag])
+        self.sleep(5)
         with self.create_registry_client(containerregistry_endpoint) as client:
             client.delete_tag(repo, tag)
 
             self.sleep(10)
             with pytest.raises(ResourceNotFoundError):
                 client.get_tag_properties(repo, tag)
 
@@ -370,43 +377,43 @@
             client.delete_repository(repo)
 
     @acr_preparer()
     @recorded_by_proxy
     def test_delete_tag_does_not_exist(self, containerregistry_endpoint):
         with self.create_registry_client(containerregistry_endpoint) as client:
             client.delete_tag(DOES_NOT_EXIST, DOES_NOT_EXIST)
-            client.delete_tag(ALPINE, DOES_NOT_EXIST)
+            client.delete_tag(HELLO_WORLD, DOES_NOT_EXIST)
 
     @acr_preparer()
     @recorded_by_proxy
     def test_delete_manifest(self, containerregistry_endpoint):
         repo = self.get_resource_name("repo")
-        tag = self.get_resource_name("tag")
-        self.import_image(containerregistry_endpoint, HELLO_WORLD, [f"{repo}:{tag}"])
-
+        tag = "test"
+        self.import_image(containerregistry_endpoint, repo, [tag])
+        self.sleep(5)
         with self.create_registry_client(containerregistry_endpoint) as client:
             client.delete_manifest(repo, tag)
 
             self.sleep(10)
             with pytest.raises(ResourceNotFoundError):
                 client.get_manifest_properties(repo, tag)
 
             # Cleanup
             client.delete_repository(repo)
 
     @acr_preparer()
     @recorded_by_proxy
     def test_delete_manifest_does_not_exist(self, containerregistry_endpoint):
         with self.create_registry_client(containerregistry_endpoint) as client:
-            manifest = client.get_manifest_properties(ALPINE, "latest")
+            manifest = client.get_manifest_properties(HELLO_WORLD, "latest")
             invalid_digest = manifest.digest[:-10] + u"a" * 10
 
-            client.delete_manifest(ALPINE, invalid_digest)
+            client.delete_manifest(HELLO_WORLD, invalid_digest)
             with pytest.raises(ResourceNotFoundError):
-                client.delete_manifest(ALPINE, DOES_NOT_EXIST)
+                client.delete_manifest(HELLO_WORLD, DOES_NOT_EXIST)
             with pytest.raises(ResourceNotFoundError):
                 client.delete_manifest(DOES_NOT_EXIST, DOES_NOT_EXIST)
 
     @acr_preparer()
     @recorded_by_proxy
     def test_expiration_time_parsing(self, containerregistry_endpoint):
         from azure.containerregistry._authentication_policy import ContainerRegistryChallengePolicy
@@ -425,399 +432,261 @@
 
             assert count >= 1
 
     # Live only, the fake credential doesn't check auth scope the same way
     @pytest.mark.live_test_only
     @acr_preparer()
     @recorded_by_proxy
-    def test_construct_container_registry_client(self, **kwargs):
+    def construct_container_registry_client(self, **kwargs):
         containerregistry_endpoint = kwargs.pop("containerregistry_endpoint")
         authority = get_authority(containerregistry_endpoint)
         credential = self.get_credential(authority)
 
         with ContainerRegistryClient(
             endpoint=containerregistry_endpoint, credential=credential, audience="https://microsoft.com"
         ) as client:
             with pytest.raises(ClientAuthenticationError):
                 properties = client.get_repository_properties(HELLO_WORLD)
             
     @acr_preparer()
     @recorded_by_proxy
     def test_get_misspell_property(self, containerregistry_endpoint):
         with self.create_registry_client(containerregistry_endpoint) as client:
-            properties = client.get_repository_properties(ALPINE)
+            properties = client.get_repository_properties(HELLO_WORLD)
             
             with pytest.warns(DeprecationWarning):
                 last_udpated_on = properties.last_udpated_on
             last_updated_on = properties.last_updated_on
             assert last_udpated_on == last_updated_on
 
     # Live only, as test proxy now cannot handle spaces correctly
     # issue: https://github.com/Azure/azure-sdk-tools/issues/5968
     @pytest.mark.live_test_only
     @acr_preparer()
-    @recorded_by_proxy
-    def test_set_oci_manifest_json(self, containerregistry_endpoint):
-        repo = self.get_resource_name("repo")
-        path = os.path.join(self.get_test_directory(), "data", "oci_artifact", "manifest.json")
-        with self.create_registry_client(containerregistry_endpoint) as client:
-            self.upload_oci_manifest_prerequisites(repo, client)
-
-            with open(path, "rb") as manifest_stream:
-                manifest_json = json.loads(manifest_stream.read().decode())
-                with pytest.raises(HttpResponseError):
-                    client.set_manifest(repo, manifest_json, media_type=DOCKER_MANIFEST)
-                digest = client.set_manifest(repo, manifest_json)
-
-            response = client.get_manifest(repo, digest)
-            assert response.media_type == OCI_IMAGE_MANIFEST
-
-            client.delete_manifest(repo, digest)
-            client.delete_repository(repo)
-
-    # Live only, as test proxy now cannot handle spaces correctly
-    # issue: https://github.com/Azure/azure-sdk-tools/issues/5968
-    @pytest.mark.live_test_only
-    @acr_preparer()
-    @recorded_by_proxy
-    def test_set_oci_manifest_json_with_tag(self, containerregistry_endpoint):
+    def test_set_oci_manifest(self, **kwargs):
+        containerregistry_endpoint = kwargs.pop("containerregistry_endpoint")
         repo = self.get_resource_name("repo")
-        tag = "v1"
         path = os.path.join(self.get_test_directory(), "data", "oci_artifact", "manifest.json")
         with self.create_registry_client(containerregistry_endpoint) as client:
             self.upload_oci_manifest_prerequisites(repo, client)
             
             with open(path, "rb") as manifest_stream:
+                # test set oci manifest in stream format
+                with pytest.raises(HttpResponseError):
+                    client.set_manifest(repo, manifest_stream, tag="v1", media_type=DOCKER_MANIFEST)
+                manifest_stream.seek(0)
+                digest1 = client.set_manifest(repo, manifest_stream, tag="v1")
+                manifest_stream.seek(0)
+                
+                # test set oci manifest in JSON format
                 manifest_json = json.loads(manifest_stream.read().decode())
                 with pytest.raises(HttpResponseError):
-                    client.set_manifest(repo, manifest_json, tag=tag, media_type=DOCKER_MANIFEST)
-                digest = client.set_manifest(repo, manifest_json, tag=tag)
+                    client.set_manifest(repo, manifest_json, tag="v2", media_type=DOCKER_MANIFEST)
+                digest2 = client.set_manifest(repo, manifest_json, tag="v2")
+            
+            assert digest1 == digest2
             
-            response = client.get_manifest(repo, tag)
+            # test get oci manifest by digest
+            response = client.get_manifest(repo, digest1)
             assert response.media_type == OCI_IMAGE_MANIFEST
-
-            tags = client.get_manifest_properties(repo, digest).tags
-            assert len(tags) == 1
-            assert tags[0] == tag
-
-            client.delete_manifest(repo, digest)
-            client.delete_repository(repo)
-    
-    # Live only, as test proxy now cannot handle spaces correctly
-    # issue: https://github.com/Azure/azure-sdk-tools/issues/5968
-    @pytest.mark.live_test_only
-    @acr_preparer()
-    @recorded_by_proxy
-    def test_set_oci_manifest_stream(self, containerregistry_endpoint):
-        repo = self.get_resource_name("repo")
-        path = os.path.join(self.get_test_directory(), "data", "oci_artifact", "manifest.json")
-        with self.create_registry_client(containerregistry_endpoint) as client:
-            self.upload_oci_manifest_prerequisites(repo, client)
-
-            with open(path, "rb") as manifest_stream:
-                with pytest.raises(HttpResponseError):
-                    client.set_manifest(repo, manifest_stream, media_type=DOCKER_MANIFEST)
-                manifest_stream.seek(0)
-                digest = client.set_manifest(repo, manifest_stream)
-
-            response = client.get_manifest(repo, digest)
+            
+            # test get oci manifest by tag
+            response = client.get_manifest(repo, "v1")
+            assert response.media_type == OCI_IMAGE_MANIFEST
+            response = client.get_manifest(repo, "v2")
             assert response.media_type == OCI_IMAGE_MANIFEST
 
-            client.delete_manifest(repo, digest)
+            client.delete_manifest(repo, digest1)
             client.delete_repository(repo)
 
+    # Reading data from a no space file to make this test pass in playback as test proxy cannot handle spaces correctly.
+    # issue: https://github.com/Azure/azure-sdk-tools/issues/5968
     @acr_preparer()
     @recorded_by_proxy
-    def test_set_oci_manifest_stream_without_spaces(self, containerregistry_endpoint):
+    def test_set_oci_manifest_without_spaces(self, containerregistry_endpoint):
+        if not is_public_endpoint(containerregistry_endpoint):
+            pytest.skip("This test is for testing test_set_docker_manifest in playback.")
+        
         repo = self.get_resource_name("repo")
-        # Reading data from a no space file to make this test pass in playback as test proxy cannot handle spaces correctly
-        # issue: https://github.com/Azure/azure-sdk-tools/issues/5968
         path = os.path.join(self.get_test_directory(), "data", "oci_artifact", "manifest_without_spaces.json")
         with self.create_registry_client(containerregistry_endpoint) as client:
             self.upload_oci_manifest_prerequisites(repo, client)
 
             with open(path, "rb") as manifest_stream:
+                # test set oci manifest in stream format
                 with pytest.raises(HttpResponseError):
-                    client.set_manifest(repo, manifest_stream, media_type=DOCKER_MANIFEST)
+                    client.set_manifest(repo, manifest_stream, tag="v1", media_type=DOCKER_MANIFEST)
                 manifest_stream.seek(0)
-                digest = client.set_manifest(repo, manifest_stream)
-
+                digest = client.set_manifest(repo, manifest_stream, tag="v1")
+                        
+            # test get oci manifest by digest
             response = client.get_manifest(repo, digest)
             assert response.media_type == OCI_IMAGE_MANIFEST
-
-            client.delete_manifest(repo, digest)
-            client.delete_repository(repo)
-
-    # Live only, as test proxy now cannot handle spaces correctly
-    # issue: https://github.com/Azure/azure-sdk-tools/issues/5968
-    @pytest.mark.live_test_only
-    @acr_preparer()
-    @recorded_by_proxy
-    def test_set_oci_manifest_stream_with_tag(self, containerregistry_endpoint):
-        repo = self.get_resource_name("repo")
-        tag = "v1"
-        path = os.path.join(self.get_test_directory(), "data", "oci_artifact", "manifest.json")
-        with self.create_registry_client(containerregistry_endpoint) as client:
-            self.upload_oci_manifest_prerequisites(repo, client)
-            
-            with open(path, "rb") as manifest_stream:
-                with pytest.raises(HttpResponseError):
-                    client.set_manifest(repo, manifest_stream, tag=tag, media_type=DOCKER_MANIFEST)
-                manifest_stream.seek(0)
-                digest = client.set_manifest(repo, manifest_stream, tag=tag)
-            
-            response = client.get_manifest(repo, tag)
-            assert response.media_type == OCI_IMAGE_MANIFEST
-            
-            tags = client.get_manifest_properties(repo, digest).tags
-            assert len(tags) == 1
-            assert tags[0] == tag
-
-            client.delete_manifest(repo, digest)
-            client.delete_repository(repo)
-    
-    @acr_preparer()
-    @recorded_by_proxy
-    def test_set_oci_manifest_stream_without_spaces_with_tag(self, containerregistry_endpoint):
-        repo = self.get_resource_name("repo")
-        tag = "v1"
-        # Reading data from a no space file to make this test pass in playback as test proxy cannot handle spaces correctly
-        # issue: https://github.com/Azure/azure-sdk-tools/issues/5968
-        path = os.path.join(self.get_test_directory(), "data", "oci_artifact", "manifest_without_spaces.json")
-        with self.create_registry_client(containerregistry_endpoint) as client:
-            self.upload_oci_manifest_prerequisites(repo, client)
-            
-            with open(path, "rb") as manifest_stream:
-                with pytest.raises(HttpResponseError):
-                    client.set_manifest(repo, manifest_stream, tag=tag, media_type=DOCKER_MANIFEST)
-                manifest_stream.seek(0)
-                digest = client.set_manifest(repo, manifest_stream, tag=tag)
             
-            response = client.get_manifest(repo, tag)
+            # test get oci manifest by tag
+            response = client.get_manifest(repo, "v1")
             assert response.media_type == OCI_IMAGE_MANIFEST
-            
-            tags = client.get_manifest_properties(repo, digest).tags
-            assert len(tags) == 1
-            assert tags[0] == tag
 
             client.delete_manifest(repo, digest)
             client.delete_repository(repo)
     
     # Live only, as test proxy now cannot handle spaces correctly
     # issue: https://github.com/Azure/azure-sdk-tools/issues/5968
     @pytest.mark.live_test_only
     @acr_preparer()
-    @recorded_by_proxy
-    def test_set_docker_manifest_stream(self, containerregistry_endpoint):
-        repo = "library/hello-world"
+    def test_set_docker_manifest(self, **kwargs):
+        containerregistry_endpoint = kwargs.pop("containerregistry_endpoint")
+        repo = self.get_resource_name("repo")
         path = os.path.join(self.get_test_directory(), "data", "docker_artifact", "manifest.json")
         with self.create_registry_client(containerregistry_endpoint) as client:
             self.upload_docker_manifest_prerequisites(repo, client)
 
             with open(path, "rb") as manifest_stream:
+                # test set Docker manifest in stream format
                 with pytest.raises(HttpResponseError):
                     # It fails as the default media type is oci image manifest media type
-                    client.set_manifest(repo, manifest_stream)
+                    client.set_manifest(repo, manifest_stream, tag="v1")
                 manifest_stream.seek(0)
-                digest = client.set_manifest(repo, manifest_stream, media_type=DOCKER_MANIFEST)
-
-            response = client.get_manifest(repo, digest)
-            assert response.media_type == DOCKER_MANIFEST
-
-            client.delete_manifest(repo, digest)
-            client.delete_repository(repo)
-    
-    @acr_preparer()
-    @recorded_by_proxy
-    def test_set_docker_manifest_stream_without_spaces(self, containerregistry_endpoint):
-        repo = "library/hello-world"
-        # Reading data from a no space file to make this test pass in playback as test proxy cannot handle spaces correctly
-        # issue: https://github.com/Azure/azure-sdk-tools/issues/5968
-        path = os.path.join(self.get_test_directory(), "data", "docker_artifact", "manifest_without_spaces.json")
-        with self.create_registry_client(containerregistry_endpoint) as client:
-            self.upload_docker_manifest_prerequisites(repo, client)
-
-            with open(path, "rb") as manifest_stream:
-                with pytest.raises(HttpResponseError):
-                    # It fails as the default media type is oci image manifest media type
-                    client.set_manifest(repo, manifest_stream)
+                digest1 = client.set_manifest(repo, manifest_stream, tag="v1", media_type=DOCKER_MANIFEST)
                 manifest_stream.seek(0)
-                digest = client.set_manifest(repo, manifest_stream, media_type=DOCKER_MANIFEST)
-
-            response = client.get_manifest(repo, digest)
-            assert response.media_type == DOCKER_MANIFEST
-
-            client.delete_manifest(repo, digest)
-            client.delete_repository(repo)
-    
-    # Live only, as test proxy now cannot handle spaces correctly
-    # issue: https://github.com/Azure/azure-sdk-tools/issues/5968
-    @pytest.mark.live_test_only
-    @acr_preparer()
-    @recorded_by_proxy
-    def test_set_docker_manifest_stream_with_tag(self, containerregistry_endpoint):
-        repo = "library/hello-world"
-        tag = "v1"
-        path = os.path.join(self.get_test_directory(), "data", "docker_artifact", "manifest.json")
-        with self.create_registry_client(containerregistry_endpoint) as client:
-            self.upload_docker_manifest_prerequisites(repo, client)
-
-            with open(path, "rb") as manifest_stream:
+                
+                # test set Docker manifest in JSON format
+                manifest_json = json.loads(manifest_stream.read().decode())
                 with pytest.raises(HttpResponseError):
                     # It fails as the default media type is oci image manifest media type
-                    client.set_manifest(repo, manifest_stream, tag=tag)
-                digest = client.set_manifest(repo, manifest_stream, tag=tag, media_type=DOCKER_MANIFEST)
+                    client.set_manifest(repo, manifest_json, tag="v2")
+                digest2 = client.set_manifest(repo, manifest_json, tag="v2", media_type=DOCKER_MANIFEST)
             
-            response = client.get_manifest(repo, tag)
+            assert digest1 == digest2
+                
+            # test get Docker manifest by digest
+            response = client.get_manifest(repo, digest1)
             assert response.media_type == DOCKER_MANIFEST
-
-            tags = client.get_manifest_properties(repo, digest).tags
-            assert len(tags) == 1
-            assert tags[0] == tag
-            
-            client.delete_manifest(repo, digest)
-            client.delete_repository(repo)
-    
-    @acr_preparer()
-    @recorded_by_proxy
-    def test_set_docker_manifest_stream_without_spaces_with_tag(self, containerregistry_endpoint):
-        repo = "library/hello-world"
-        tag = "v1"
-        # Reading data from a no space file to make this test pass in playback as test proxy cannot handle spaces correctly
-        # issue: https://github.com/Azure/azure-sdk-tools/issues/5968
-        path = os.path.join(self.get_test_directory(), "data", "docker_artifact", "manifest_without_spaces.json")
-        with self.create_registry_client(containerregistry_endpoint) as client:
-            self.upload_docker_manifest_prerequisites(repo, client)
-
-            with open(path, "rb") as manifest_stream:
-                with pytest.raises(HttpResponseError):
-                    # It fails as the default media type is oci image manifest media type
-                    client.set_manifest(repo, manifest_stream, tag=tag)
-                digest = client.set_manifest(repo, manifest_stream, tag=tag, media_type=DOCKER_MANIFEST)
             
-            response = client.get_manifest(repo, tag)
+            # test get Docker manifest by tag
+            response = client.get_manifest(repo, "v1")
+            assert response.media_type == DOCKER_MANIFEST
+            response = client.get_manifest(repo, "v2")
             assert response.media_type == DOCKER_MANIFEST
 
-            tags = client.get_manifest_properties(repo, digest).tags
-            assert len(tags) == 1
-            assert tags[0] == tag
-            
-            client.delete_manifest(repo, digest)
+            client.delete_manifest(repo, digest1)
             client.delete_repository(repo)
     
-    # Live only, as test proxy now cannot handle spaces correctly
+    # Reading data from a no space file to make this test pass in playback as test proxy cannot handle spaces correctly.
     # issue: https://github.com/Azure/azure-sdk-tools/issues/5968
-    @pytest.mark.live_test_only
     @acr_preparer()
     @recorded_by_proxy
-    def test_set_docker_manifest_json(self, containerregistry_endpoint):
-        repo = "library/hello-world"
-        path = os.path.join(self.get_test_directory(), "data", "docker_artifact", "manifest.json")
+    def test_set_docker_manifest_without_spaces(self, containerregistry_endpoint):
+        if not is_public_endpoint(containerregistry_endpoint):
+            pytest.skip("This test is for testing test_set_docker_manifest in playback.")
+        
+        repo = self.get_resource_name("repo")
+        path = os.path.join(self.get_test_directory(), "data", "docker_artifact", "manifest_without_spaces.json")
         with self.create_registry_client(containerregistry_endpoint) as client:
             self.upload_docker_manifest_prerequisites(repo, client)
 
             with open(path, "rb") as manifest_stream:
-                manifest_json = json.loads(manifest_stream.read().decode())
+                # test set Docker manifest in stream format
                 with pytest.raises(HttpResponseError):
                     # It fails as the default media type is oci image manifest media type
-                    client.set_manifest(repo, manifest_json)
-                digest = client.set_manifest(repo, manifest_json, media_type=DOCKER_MANIFEST)
-            
+                    client.set_manifest(repo, manifest_stream, tag="v1")
+                manifest_stream.seek(0)
+                digest = client.set_manifest(repo, manifest_stream, tag="v1", media_type=DOCKER_MANIFEST)
+                
+            # test get Docker manifest by digest
             response = client.get_manifest(repo, digest)
             assert response.media_type == DOCKER_MANIFEST
-
-            client.delete_manifest(repo, digest)
-            client.delete_repository(repo)
-    
-    # Live only, as test proxy now cannot handle spaces correctly
-    # issue: https://github.com/Azure/azure-sdk-tools/issues/5968
-    @pytest.mark.live_test_only
-    @acr_preparer()
-    @recorded_by_proxy
-    def test_set_docker_manifest_json_with_tag(self, containerregistry_endpoint):
-        repo = "library/hello-world"
-        tag = "v1"
-        path = os.path.join(self.get_test_directory(), "data", "docker_artifact", "manifest.json")
-        with self.create_registry_client(containerregistry_endpoint) as client:
-            self.upload_docker_manifest_prerequisites(repo, client)
-
-            with open(path, "rb") as manifest_stream:
-                manifest_json = json.loads(manifest_stream.read().decode())
-                with pytest.raises(HttpResponseError):
-                    # It fails as the default media type is oci image manifest media type
-                    client.set_manifest(repo, manifest_json, tag=tag)
-                digest = client.set_manifest(repo, manifest_json, tag=tag, media_type=DOCKER_MANIFEST)
             
-            response = client.get_manifest(repo, tag)
+            # test get Docker manifest by tag
+            response = client.get_manifest(repo, "v1")
             assert response.media_type == DOCKER_MANIFEST
 
-            tags = client.get_manifest_properties(repo, digest).tags
-            assert len(tags) == 1
-            assert tags[0] == tag
-            
             client.delete_manifest(repo, digest)
             client.delete_repository(repo)
 
     @acr_preparer()
     @recorded_by_proxy
     def test_upload_blob(self, containerregistry_endpoint):
         repo = self.get_resource_name("repo")
-        blob = "654b93f61054e4ce90ed203bb8d556a6200d5f906cf3eca0620738d6dc18cbed"
-        path = os.path.join(self.get_test_directory(), "data", "oci_artifact", blob)
+        blob = BytesIO(b"hello world")
 
         with self.create_registry_client(containerregistry_endpoint) as client:
             # Act
-            with open(path, "rb") as data:
-                digest, blob_size = client.upload_blob(repo, data)
+            digest, blob_size = client.upload_blob(repo, blob)
 
             # Assert
             blob_content = b""
             stream = client.download_blob(repo, digest)
             for chunk in stream:
                 blob_content += chunk
             assert len(blob_content) == blob_size
 
             client.delete_blob(repo, digest)
             client.delete_repository(repo)
 
     @pytest.mark.live_test_only
     @acr_preparer()
-    @recorded_by_proxy
-    def test_upload_large_blob_in_chunk(self, containerregistry_endpoint):
+    def upload_large_blob_in_chunk(self, **kwargs):
+        containerregistry_endpoint = kwargs.pop("containerregistry_endpoint")
+        if not is_public_endpoint(containerregistry_endpoint):
+            pytest.skip("Running on non-public cloud may cause all tests finishing longer than the max time of 120 mins.")
+        
         repo = self.get_resource_name("repo")
         with self.create_registry_client(containerregistry_endpoint) as client:
             # Test blob upload and download in equal size chunks
-            blob_size = DEFAULT_CHUNK_SIZE * 1024 # 4GB
-            data = b'\x00' * int(blob_size)
-            digest, size = client.upload_blob(repo, BytesIO(data))
-            assert size == blob_size
-
-            stream = client.download_blob(repo, digest)
-            size = 0
-            with open("text1.txt", "wb") as file:
-                for chunk in stream:
-                    size += file.write(chunk)
-            assert size == blob_size
-
-            client.delete_blob(repo, digest)
+            try:
+                blob_size = DEFAULT_CHUNK_SIZE * 1024 # 4GB
+                data = b'\x00' * int(blob_size)
+                digest, size = client.upload_blob(repo, BytesIO(data))
+                assert size == blob_size
+
+                stream = client.download_blob(repo, digest)
+                size = 0
+                with open("text1.txt", "wb") as file:
+                    for chunk in stream:
+                        size += file.write(chunk)
+                assert size == blob_size
+
+                client.delete_blob(repo, digest)
+            except (ServiceRequestError, ServiceResponseError) as err:
+                # Service does not support resumable upload when get transient error while uploading
+                # issue: https://github.com/Azure/azure-sdk-for-python/issues/29738
+                print(f"Failed to upload blob: {err.message}")
+            except ResourceNotFoundError as err:
+                # Service does not support resumable upload when get transient error while uploading
+                # issue: https://github.com/Azure/azure-sdk-for-python/issues/29738
+                assert err.status_code == 404
+                assert err.response.request.method == "PATCH"
+                assert err.response.text() == '{"errors":[{"code":"BLOB_UPLOAD_INVALID","message":"blob upload invalid"}]}\n'
 
             # Test blob upload and download in unequal size chunks
-            blob_size = DEFAULT_CHUNK_SIZE * 1024 + 20
-            data = b'\x00' * int(blob_size)
-            digest, size = client.upload_blob(repo, BytesIO(data))
-            assert size == blob_size
-
-            stream = client.download_blob(repo, digest)
-            size = 0
-            with open("text2.txt", "wb") as file:
-                for chunk in stream:
-                    size += file.write(chunk)
-            assert size == blob_size
-
-            client.delete_blob(repo, digest)
+            try:
+                blob_size = DEFAULT_CHUNK_SIZE * 1024 + 20
+                data = b'\x00' * int(blob_size)
+                digest, size = client.upload_blob(repo, BytesIO(data))
+                assert size == blob_size
+
+                stream = client.download_blob(repo, digest)
+                size = 0
+                with open("text2.txt", "wb") as file:
+                    for chunk in stream:
+                        size += file.write(chunk)
+                assert size == blob_size
+
+                client.delete_blob(repo, digest)
+            except (ServiceRequestError, ServiceResponseError) as err:
+                # Service does not support resumable upload when get transient error while uploading
+                # issue: https://github.com/Azure/azure-sdk-for-python/issues/29738
+                print(f"Failed to upload blob: {err.message}")
+            except ResourceNotFoundError as err:
+                # Service does not support resumable upload when get transient error while uploading
+                # issue: https://github.com/Azure/azure-sdk-for-python/issues/29738
+                assert err.status_code == 404
+                assert err.response.request.method == "PATCH"
+                assert err.response.text() == '{"errors":[{"code":"BLOB_UPLOAD_INVALID","message":"blob upload invalid"}]}\n'
 
             # Cleanup
             client.delete_repository(repo)
     
     @acr_preparer()
     @recorded_by_proxy
     def test_delete_blob_does_not_exist(self, containerregistry_endpoint):
@@ -851,29 +720,179 @@
             ) as client:
                 with pytest.raises(ClientAuthenticationError):
                     for repo in client.list_repository_names():
                         pass
 
     @acr_preparer()
     @recorded_by_proxy
-    def test_list_tags_in_empty_repo(self, containerregistry_endpoint):
+    def test_list_in_empty_repo(self, containerregistry_endpoint):
+        repo = self.get_resource_name("repo")
+        self.import_image(containerregistry_endpoint, repo, ["test"])
+        self.sleep(5)
         with self.create_registry_client(containerregistry_endpoint) as client:
-            # cleanup tags in ALPINE repo
-            for tag in client.list_tag_properties(ALPINE):
-                client.delete_tag(ALPINE, tag.name)
-            
-            response = client.list_tag_properties(ALPINE)
-            if response is not None:
-                for tag in response:
-                    pass
+            # cleanup tags in repo
+            for tag in client.list_tag_properties(repo):
+                client.delete_tag(repo, tag.name)
+            
+            # test list tags in empty repo
+            response = client.list_tag_properties(repo)
+            for tag in response:
+                # cleanup manifests in repo
+                client.delete_manifest(repo, tag.name)
+
+            # test list manifests in empty repo
+            response = client.list_manifest_properties(repo)
+            for manifest in response:
+                pass
+            
+            client.delete_repository(repo)
+
+
+class TestContainerRegistryClientUnitTests:
+    containerregistry_endpoint="https://fake_url.azurecr.io"
     
-    @acr_preparer()
-    @recorded_by_proxy
-    def test_list_manifests_in_empty_repo(self, containerregistry_endpoint):
-        with self.create_registry_client(containerregistry_endpoint) as client:
-            # cleanup manifests in ALPINE repo
-            for tag in client.list_tag_properties(ALPINE):
-                client.delete_manifest(ALPINE, tag.name)
-            response = client.list_manifest_properties(ALPINE)
-            if response is not None:
-                for manifest in response:
+    def text(self, encoding: Optional[str] = None) -> str:
+            return '{"hello": "world"}'
+
+    def test_manifest_digest_validation(self):        
+        JSON = MutableMapping[str, Any]
+            
+        def send_in_set_manifest(request: PipelineRequest, **kwargs) -> MagicMock:
+            content_digest = hashlib.sha256(b"hello world").hexdigest()
+            return MagicMock(
+                status_code=201,
+                headers={"Docker-Content-Digest": content_digest},
+                content_type="application/json; charset=utf-8",
+                text=self.text
+        )
+            
+        def read() -> bytes:
+            return b'{"hello": "world"}'
+        
+        def json() -> JSON:
+            return {"hello": "world"}
+        
+        def send_in_get_manifest(request: PipelineRequest, **kwargs) -> MagicMock:
+            content_digest = hashlib.sha256(b"hello world").hexdigest()
+            content_type = "application/vnd.oci.image.manifest.v1+json"
+            return MagicMock(
+                status_code=200,
+                headers={"Docker-Content-Digest": content_digest, "Content-Type": content_type, "Content-Length": len(b"hello world")},
+                read=read,
+                json=json
+        )
+            
+        with ContainerRegistryClient(
+            endpoint=self.containerregistry_endpoint, transport = MagicMock(send=send_in_set_manifest)
+        ) as client:
+            with pytest.raises(DigestValidationError) as exp:
+                manifest = {"hello": "world"}
+                client.set_manifest("test-repo", manifest)
+            assert str(exp.value) == "The server-computed digest does not match the client-computed digest."
+            
+        with ContainerRegistryClient(
+            endpoint=self.containerregistry_endpoint,
+            transport = MagicMock(send=send_in_get_manifest)
+        ) as client:
+            with pytest.raises(DigestValidationError) as exp:
+                digest = hashlib.sha256(b"hello world").hexdigest()
+                client.get_manifest("test-repo", f"sha256:{digest}")
+            assert str(exp.value) == "The content of retrieved manifest digest does not match the requested digest."
+                
+            with pytest.raises(DigestValidationError) as exp:
+                client.get_manifest("test-repo", "test-tag")
+            assert str(exp.value) == "The server-computed digest does not match the client-computed digest."
+
+    def test_blob_digest_validation(self):       
+        def send_in_upload_blob(request: PipelineRequest, **kwargs) -> MagicMock:
+            if request.method == "PUT":
+                content_digest = hashlib.sha256(b"hello world").hexdigest()
+                return MagicMock(
+                    status_code=201,
+                    headers={"Docker-Content-Digest": content_digest},
+                    content_type="application/json; charset=utf-8",
+                    text=self.text
+                )
+            else:
+                return MagicMock(
+                    status_code=202,
+                    headers={"Location": "/v2/test-repo/blobs/uploads/fake_location"},
+                    content_type="application/json; charset=utf-8",
+                    text=self.text
+                )
+        
+        def iter_bytes() -> Iterator[bytes]:
+            yield b'{"hello": "world"}'
+        
+        def send_in_download_blob(request: PipelineRequest, **kwargs) -> MagicMock:
+            return MagicMock(
+                status_code=206,
+                headers={"Content-Range": "bytes 0-27/28", "Content-Length": "28"},
+                content_type="application/json; charset=utf-8",
+                text=self.text,
+                iter_bytes=iter_bytes
+            )
+            
+        with ContainerRegistryClient(
+            endpoint=self.containerregistry_endpoint, transport = MagicMock(send=send_in_upload_blob)
+        ) as client:
+            with pytest.raises(DigestValidationError) as exp:
+                client.upload_blob("test-repo", BytesIO(b'{"hello": "world"}'))
+            assert str(exp.value) == "The server-computed digest does not match the client-computed digest."
+            
+        with ContainerRegistryClient(
+            endpoint=self.containerregistry_endpoint, transport = MagicMock(send=send_in_download_blob)
+        ) as client:
+            digest = hashlib.sha256(b"hello world").hexdigest()
+            stream = client.download_blob("test-repo", f"sha256:{digest}")
+            with pytest.raises(DigestValidationError) as exp:
+                for chunk in stream:
                     pass
+            assert str(exp.value) == "The content of retrieved blob digest does not match the requested digest."
+    
+    def test_deserialize_manifest(self):
+        def get_manifest(encoding: Optional[str] = None) -> str:
+            manifest = {
+                "manifests": [
+                    {
+                        "mediaType": "application/vnd.docker.distribution.manifest.v2+json",
+                        "imageSize": 2199,
+                        "digest": "sha256:86fed9f0203a09f13cbbb9842132e9000eeff51b3de0d4ff66ee03ab0e860d1f",
+                        "architecture": "amd64",
+                        "os": "linux"
+                    },
+                    {
+                        "mediaType": "application/vnd.docker.distribution.manifest.v2+json",
+                        "imageSize": 566,
+                        "digest": "sha256:b808af65792ab617b9032c20fb12c455dc2bf5efe1af3f0ac81a129560772d35",
+                        "annotations": {
+                            "vnd.docker.reference.digest": "sha256:86fed9f0203a09f13cbbb9842132e9000eeff51b3de0d4ff66ee03ab0e860d1f",
+                            "vnd.docker.reference.type": "attestation-manifest"
+                        },
+                        "architecture": "unknown",
+                        "os": "unknown",
+                    }
+                ]
+            }
+            return json.dumps(manifest)
+        def send(request: PipelineRequest, **kwargs) -> MagicMock:
+            return MagicMock(
+                status_code=200,
+                content_type="application/json; charset=utf-8",
+                text=get_manifest,
+        )
+        
+        with ContainerRegistryClient(
+            endpoint=self.containerregistry_endpoint, transport = MagicMock(send=send)
+        ) as client:
+            manifests = client.list_manifest_properties(HELLO_WORLD)
+            for manifest in manifests:
+                if manifest.size_in_bytes == 2199:
+                    assert isinstance(manifest.architecture, ArtifactArchitecture)
+                    assert manifest.architecture == "amd64"
+                    assert isinstance(manifest.operating_system, ArtifactOperatingSystem)
+                    assert manifest.operating_system == "linux"
+                if manifest.size_in_bytes == 566:
+                    assert isinstance(manifest.architecture, str)
+                    assert manifest.architecture == "unknown"
+                    assert isinstance(manifest.operating_system, str)
+                    assert manifest.operating_system == "unknown"
```

## Comparing `azure-containerregistry-1.1.0b4/tests/test_anon_access_async.py` & `azure-containerregistry-1.2.0/tests/test_anon_access_async.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,221 +1,222 @@
 # coding=utf-8
 # ------------------------------------
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 # ------------------------------------
 import pytest
-import six
 from azure.containerregistry import (
     RepositoryProperties,
     ArtifactManifestProperties,
     ArtifactTagProperties,
 )
 from azure.containerregistry.aio import ContainerRegistryClient
 
 from azure.core.async_paging import AsyncItemPaged
 from azure.core.exceptions import ClientAuthenticationError
 
 from asynctestcase import AsyncContainerRegistryTestClass
+from testcase import is_public_endpoint
 from constants import HELLO_WORLD
 from preparer import acr_preparer
 from devtools_testutils.aio import recorded_by_proxy_async
 
 
 class TestContainerRegistryClientAsync(AsyncContainerRegistryTestClass):
     @acr_preparer()
     @recorded_by_proxy_async
     async def test_list_repository_names(self, containerregistry_anonregistry_endpoint):
-        if not self.is_public_endpoint(containerregistry_anonregistry_endpoint):
+        if not is_public_endpoint(containerregistry_anonregistry_endpoint):
             pytest.skip("Not a public endpoint")
 
         async with self.create_anon_client(containerregistry_anonregistry_endpoint) as client:
             assert client._credential is None
 
             repositories = client.list_repository_names()
             assert isinstance(repositories, AsyncItemPaged)
 
             count = 0
             prev = None
             async for repo in repositories:
                 count += 1
-                assert isinstance(repo, six.string_types)
+                assert isinstance(repo, str)
                 assert prev != repo
                 prev = repo
 
             assert count > 0
 
     @acr_preparer()
     @recorded_by_proxy_async
     async def test_list_repository_names_by_page(self, containerregistry_anonregistry_endpoint):
-        if not self.is_public_endpoint(containerregistry_anonregistry_endpoint):
+        if not is_public_endpoint(containerregistry_anonregistry_endpoint):
             pytest.skip("Not a public endpoint")
 
         async with self.create_anon_client(containerregistry_anonregistry_endpoint) as client:
             assert client._credential is None
 
             results_per_page = 2
             total_pages = 0
 
             repository_pages = client.list_repository_names(results_per_page=results_per_page)
 
             prev = None
             async for page in repository_pages.by_page():
                 page_count = 0
                 async for repo in page:
-                    assert isinstance(repo, six.string_types)
+                    assert isinstance(repo, str)
                     assert prev != repo
                     prev = repo
                     page_count += 1
                 assert page_count <= results_per_page
                 total_pages += 1
 
             assert total_pages >= 1
 
     @acr_preparer()
     @recorded_by_proxy_async
     async def test_get_repository_properties(self, containerregistry_anonregistry_endpoint):
-        if not self.is_public_endpoint(containerregistry_anonregistry_endpoint):
+        if not is_public_endpoint(containerregistry_anonregistry_endpoint):
             pytest.skip("Not a public endpoint")
 
         async with self.create_anon_client(containerregistry_anonregistry_endpoint) as client:
             assert client._credential is None
 
-            properties = await client.get_repository_properties("library/alpine")
+            properties = await client.get_repository_properties(HELLO_WORLD)
 
             assert isinstance(properties, RepositoryProperties)
-            assert properties.name == "library/alpine"
+            assert properties.name == HELLO_WORLD
 
     @acr_preparer()
     @recorded_by_proxy_async
     async def test_list_manifest_properties(self, containerregistry_anonregistry_endpoint):
-        if not self.is_public_endpoint(containerregistry_anonregistry_endpoint):
+        if not is_public_endpoint(containerregistry_anonregistry_endpoint):
             pytest.skip("Not a public endpoint")
 
         async with self.create_anon_client(containerregistry_anonregistry_endpoint) as client:
             assert client._credential is None
 
             count = 0
-            async for manifest in client.list_manifest_properties("library/alpine"):
+            async for manifest in client.list_manifest_properties(HELLO_WORLD):
                 assert isinstance(manifest, ArtifactManifestProperties)
                 count += 1
             assert count > 0
 
     @acr_preparer()
     @recorded_by_proxy_async
     async def test_get_manifest_properties(self, containerregistry_anonregistry_endpoint):
-        if not self.is_public_endpoint(containerregistry_anonregistry_endpoint):
+        if not is_public_endpoint(containerregistry_anonregistry_endpoint):
             pytest.skip("Not a public endpoint")
 
         async with self.create_anon_client(containerregistry_anonregistry_endpoint) as client:
             assert client._credential is None
 
-            registry_artifact = await client.get_manifest_properties("library/alpine", "latest")
+            registry_artifact = await client.get_manifest_properties(HELLO_WORLD, "latest")
 
             assert isinstance(registry_artifact, ArtifactManifestProperties)
             assert "latest" in registry_artifact.tags
-            assert registry_artifact.repository_name == "library/alpine"
+            assert registry_artifact.repository_name == HELLO_WORLD
 
     @acr_preparer()
     @recorded_by_proxy_async
     async def test_list_tag_properties(self, containerregistry_anonregistry_endpoint):
-        if not self.is_public_endpoint(containerregistry_anonregistry_endpoint):
+        if not is_public_endpoint(containerregistry_anonregistry_endpoint):
             pytest.skip("Not a public endpoint")
 
         async with self.create_anon_client(containerregistry_anonregistry_endpoint) as client:
             assert client._credential is None
 
             count = 0
-            async for tag in client.list_tag_properties("library/alpine"):
+            async for tag in client.list_tag_properties(HELLO_WORLD):
                 count += 1
                 assert isinstance(tag, ArtifactTagProperties)
             assert count > 0
 
     @acr_preparer()
     @recorded_by_proxy_async
     async def test_delete_repository(self, containerregistry_anonregistry_endpoint):
-        if not self.is_public_endpoint(containerregistry_anonregistry_endpoint):
+        if not is_public_endpoint(containerregistry_anonregistry_endpoint):
             pytest.skip("Not a public endpoint")
 
         async with self.create_anon_client(containerregistry_anonregistry_endpoint) as client:
             assert client._credential is None
 
             with pytest.raises(ClientAuthenticationError):
-                await client.delete_repository("library/hello-world")
+                await client.delete_repository(HELLO_WORLD)
 
     @acr_preparer()
     @recorded_by_proxy_async
     async def test_delete_tag(self, containerregistry_anonregistry_endpoint):
-        if not self.is_public_endpoint(containerregistry_anonregistry_endpoint):
+        if not is_public_endpoint(containerregistry_anonregistry_endpoint):
             pytest.skip("Not a public endpoint")
 
         async with self.create_anon_client(containerregistry_anonregistry_endpoint) as client:
             assert client._credential is None
 
             with pytest.raises(ClientAuthenticationError):
-                await client.delete_tag("library/hello-world", "latest")
+                await client.delete_tag(HELLO_WORLD, "latest")
 
     @acr_preparer()
     @recorded_by_proxy_async
     async def test_delete_manifest(self, containerregistry_anonregistry_endpoint):
-        if not self.is_public_endpoint(containerregistry_anonregistry_endpoint):
+        if not is_public_endpoint(containerregistry_anonregistry_endpoint):
             pytest.skip("Not a public endpoint")
 
         async with self.create_anon_client(containerregistry_anonregistry_endpoint) as client:
             assert client._credential is None
 
             with pytest.raises(ClientAuthenticationError):
-                await client.delete_manifest("library/hello-world", "latest")
+                await client.delete_manifest(HELLO_WORLD, "latest")
 
     @acr_preparer()
     @recorded_by_proxy_async
     async def test_update_repository_properties(self, containerregistry_anonregistry_endpoint):
-        if not self.is_public_endpoint(containerregistry_anonregistry_endpoint):
+        if not is_public_endpoint(containerregistry_anonregistry_endpoint):
             pytest.skip("Not a public endpoint")
 
         async with self.create_anon_client(containerregistry_anonregistry_endpoint) as client:
             properties = await client.get_repository_properties(HELLO_WORLD)
 
             with pytest.raises(ClientAuthenticationError):
                 await client.update_repository_properties(HELLO_WORLD, properties, can_delete=True)
 
     @acr_preparer()
     @recorded_by_proxy_async
     async def test_update_tag_properties(self, containerregistry_anonregistry_endpoint):
-        if not self.is_public_endpoint(containerregistry_anonregistry_endpoint):
+        if not is_public_endpoint(containerregistry_anonregistry_endpoint):
             pytest.skip("Not a public endpoint")
 
         async with self.create_anon_client(containerregistry_anonregistry_endpoint) as client:
             properties = await client.get_tag_properties(HELLO_WORLD, "latest")
 
             with pytest.raises(ClientAuthenticationError):
                 await client.update_tag_properties(HELLO_WORLD, "latest", properties, can_delete=True)
 
     @acr_preparer()
     @recorded_by_proxy_async
     async def test_update_manifest_properties(self, containerregistry_anonregistry_endpoint):
-        if not self.is_public_endpoint(containerregistry_anonregistry_endpoint):
+        if not is_public_endpoint(containerregistry_anonregistry_endpoint):
             pytest.skip("Not a public endpoint")
 
         async with self.create_anon_client(containerregistry_anonregistry_endpoint) as client:
             properties = await client.get_manifest_properties(HELLO_WORLD, "latest")
 
             with pytest.raises(ClientAuthenticationError):
                 await client.update_manifest_properties(HELLO_WORLD, "latest", properties, can_delete=True)
 
 
+@pytest.mark.asyncio
 async def test_set_api_version():
     containerregistry_endpoint="https://fake_url.azurecr.io"
     
-    with ContainerRegistryClient(endpoint=containerregistry_endpoint, audience="https://microsoft.com") as client:
+    async with ContainerRegistryClient(endpoint=containerregistry_endpoint, audience="https://microsoft.com") as client:
         assert client._client._config.api_version == "2021-07-01"
     
-    with ContainerRegistryClient(
+    async with ContainerRegistryClient(
         endpoint=containerregistry_endpoint, audience="https://microsoft.com", api_version = "2019-08-15-preview"
     ) as client:
         assert client._client._config.api_version == "2019-08-15-preview"
     
     with pytest.raises(ValueError):
-        with ContainerRegistryClient(
+        async with ContainerRegistryClient(
             endpoint=containerregistry_endpoint, audience="https://microsoft.com", api_version = "2019-08-15"
         ) as client:
             pass
```

## Comparing `azure-containerregistry-1.1.0b4/tests/asynctestcase.py` & `azure-containerregistry-1.2.0/tests/asynctestcase.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b4/tests/test_anon_access.py` & `azure-containerregistry-1.2.0/tests/test_anon_access.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,203 +1,202 @@
 # coding=utf-8
 # ------------------------------------
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 # ------------------------------------
 import pytest
-import six
 
 from azure.core.exceptions import ClientAuthenticationError
 from azure.core.paging import ItemPaged
 from azure.containerregistry import (
     ArtifactTagProperties,
     RepositoryProperties,
     ArtifactManifestProperties,
     ContainerRegistryClient,
 )
 
-from testcase import ContainerRegistryTestClass
+from testcase import ContainerRegistryTestClass, is_public_endpoint
 from constants import HELLO_WORLD
 from preparer import acr_preparer
 from devtools_testutils import recorded_by_proxy
 
 
 class TestContainerRegistryClient(ContainerRegistryTestClass):
     @acr_preparer()
     @recorded_by_proxy
     def test_list_repository_names(self, containerregistry_anonregistry_endpoint):
-        if not self.is_public_endpoint(containerregistry_anonregistry_endpoint):
+        if not is_public_endpoint(containerregistry_anonregistry_endpoint):
             pytest.skip("Not a public endpoint")
 
         with self.create_anon_client(containerregistry_anonregistry_endpoint) as client:
             assert client._credential is None
 
             repositories = client.list_repository_names()
             assert isinstance(repositories, ItemPaged)
 
             count = 0
             prev = None
             for repo in repositories:
                 count += 1
-                assert isinstance(repo, six.string_types)
+                assert isinstance(repo, str)
                 assert prev != repo
                 prev = repo
 
             assert count > 0
 
     @acr_preparer()
     @recorded_by_proxy
     def test_list_repository_names_by_page(self, containerregistry_anonregistry_endpoint):
-        if not self.is_public_endpoint(containerregistry_anonregistry_endpoint):
+        if not is_public_endpoint(containerregistry_anonregistry_endpoint):
             pytest.skip("Not a public endpoint")
 
         with self.create_anon_client(containerregistry_anonregistry_endpoint) as client:
             assert client._credential is None
 
             results_per_page = 2
             total_pages = 0
 
             repository_pages = client.list_repository_names(results_per_page=results_per_page)
 
             prev = None
             for page in repository_pages.by_page():
                 page_count = 0
                 for repo in page:
-                    assert isinstance(repo, six.string_types)
+                    assert isinstance(repo, str)
                     assert prev != repo
                     prev = repo
                     page_count += 1
                 assert page_count <= results_per_page
                 total_pages += 1
 
             assert total_pages >= 1
 
     @acr_preparer()
     @recorded_by_proxy
     def test_get_repository_properties(self, containerregistry_anonregistry_endpoint):
-        if not self.is_public_endpoint(containerregistry_anonregistry_endpoint):
+        if not is_public_endpoint(containerregistry_anonregistry_endpoint):
             pytest.skip("Not a public endpoint")
 
         with self.create_anon_client(containerregistry_anonregistry_endpoint) as client:
             assert client._credential is None
 
-            properties = client.get_repository_properties("library/hello-world")
+            properties = client.get_repository_properties(HELLO_WORLD)
 
             assert isinstance(properties, RepositoryProperties)
             assert properties.name == HELLO_WORLD
 
     @acr_preparer()
     @recorded_by_proxy
     def test_list_manifest_properties(self, containerregistry_anonregistry_endpoint):
-        if not self.is_public_endpoint(containerregistry_anonregistry_endpoint):
+        if not is_public_endpoint(containerregistry_anonregistry_endpoint):
             pytest.skip("Not a public endpoint")
 
         with self.create_anon_client(containerregistry_anonregistry_endpoint) as client:
             assert client._credential is None
 
             count = 0
-            for manifest in client.list_manifest_properties("library/hello-world"):
+            for manifest in client.list_manifest_properties(HELLO_WORLD):
                 assert isinstance(manifest, ArtifactManifestProperties)
                 count += 1
             assert count > 0
 
     @acr_preparer()
     @recorded_by_proxy
     def test_get_manifest_properties(self, containerregistry_anonregistry_endpoint):
-        if not self.is_public_endpoint(containerregistry_anonregistry_endpoint):
+        if not is_public_endpoint(containerregistry_anonregistry_endpoint):
             pytest.skip("Not a public endpoint")
 
         with self.create_anon_client(containerregistry_anonregistry_endpoint) as client:
             assert client._credential is None
 
-            registry_artifact = client.get_manifest_properties("library/hello-world", "latest")
+            registry_artifact = client.get_manifest_properties(HELLO_WORLD, "latest")
 
             assert isinstance(registry_artifact, ArtifactManifestProperties)
             assert "latest" in registry_artifact.tags
-            assert registry_artifact.repository_name == "library/hello-world"
+            assert registry_artifact.repository_name == HELLO_WORLD
 
     @acr_preparer()
     @recorded_by_proxy
     def test_list_tag_properties(self, containerregistry_anonregistry_endpoint):
-        if not self.is_public_endpoint(containerregistry_anonregistry_endpoint):
+        if not is_public_endpoint(containerregistry_anonregistry_endpoint):
             pytest.skip("Not a public endpoint")
 
         with self.create_anon_client(containerregistry_anonregistry_endpoint) as client:
             assert client._credential is None
 
             count = 0
-            for tag in client.list_tag_properties("library/hello-world"):
+            for tag in client.list_tag_properties(HELLO_WORLD):
                 count += 1
                 assert isinstance(tag, ArtifactTagProperties)
             assert count > 0
 
     @acr_preparer()
     @recorded_by_proxy
     def test_delete_repository(self, containerregistry_anonregistry_endpoint):
-        if not self.is_public_endpoint(containerregistry_anonregistry_endpoint):
+        if not is_public_endpoint(containerregistry_anonregistry_endpoint):
             pytest.skip("Not a public endpoint")
 
         with self.create_anon_client(containerregistry_anonregistry_endpoint) as client:
             assert client._credential is None
 
             with pytest.raises(ClientAuthenticationError):
-                client.delete_repository("library/hello-world")
+                client.delete_repository(HELLO_WORLD)
 
     @acr_preparer()
     @recorded_by_proxy
     def test_delete_tag(self, containerregistry_anonregistry_endpoint):
-        if not self.is_public_endpoint(containerregistry_anonregistry_endpoint):
+        if not is_public_endpoint(containerregistry_anonregistry_endpoint):
             pytest.skip("Not a public endpoint")
 
         with self.create_anon_client(containerregistry_anonregistry_endpoint) as client:
             assert client._credential is None
 
             with pytest.raises(ClientAuthenticationError):
-                client.delete_tag("library/hello-world", "latest")
+                client.delete_tag(HELLO_WORLD, "latest")
 
     @acr_preparer()
     @recorded_by_proxy
     def test_delete_manifest(self, containerregistry_anonregistry_endpoint):
-        if not self.is_public_endpoint(containerregistry_anonregistry_endpoint):
+        if not is_public_endpoint(containerregistry_anonregistry_endpoint):
             pytest.skip("Not a public endpoint")
 
         with self.create_anon_client(containerregistry_anonregistry_endpoint) as client:
             assert client._credential is None
 
             with pytest.raises(ClientAuthenticationError):
-                client.delete_manifest("library/hello-world", "latest")
+                client.delete_manifest(HELLO_WORLD, "latest")
 
     @acr_preparer()
     @recorded_by_proxy
     def test_update_repository_properties(self, containerregistry_anonregistry_endpoint):
-        if not self.is_public_endpoint(containerregistry_anonregistry_endpoint):
+        if not is_public_endpoint(containerregistry_anonregistry_endpoint):
             pytest.skip("Not a public endpoint")
 
         with self.create_anon_client(containerregistry_anonregistry_endpoint) as client:
             properties = client.get_repository_properties(HELLO_WORLD)
 
             with pytest.raises(ClientAuthenticationError):
                 client.update_repository_properties(HELLO_WORLD, properties, can_delete=True)
 
     @acr_preparer()
     @recorded_by_proxy
     def test_update_tag_properties(self, containerregistry_anonregistry_endpoint):
-        if not self.is_public_endpoint(containerregistry_anonregistry_endpoint):
+        if not is_public_endpoint(containerregistry_anonregistry_endpoint):
             pytest.skip("Not a public endpoint")
 
         with self.create_anon_client(containerregistry_anonregistry_endpoint) as client:
             properties = client.get_tag_properties(HELLO_WORLD, "latest")
 
             with pytest.raises(ClientAuthenticationError):
                 client.update_tag_properties(HELLO_WORLD, "latest", properties, can_delete=True)
 
     @acr_preparer()
     @recorded_by_proxy
     def test_update_manifest_properties(self, containerregistry_anonregistry_endpoint):
-        if not self.is_public_endpoint(containerregistry_anonregistry_endpoint):
+        if not is_public_endpoint(containerregistry_anonregistry_endpoint):
             pytest.skip("Not a public endpoint")
 
         with self.create_anon_client(containerregistry_anonregistry_endpoint) as client:
             properties = client.get_manifest_properties(HELLO_WORLD, "latest")
 
             with pytest.raises(ClientAuthenticationError):
                 client.update_manifest_properties(HELLO_WORLD, "latest", properties, can_delete=True)
```

## Comparing `azure-containerregistry-1.1.0b4/tests/test_container_registry_client_async.py` & `azure-containerregistry-1.2.0/tests/test_container_registry_client_async.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,45 @@
 # coding=utf-8
 # ------------------------------------
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 # ------------------------------------
 import os
 import pytest
-import six
 import hashlib
 import json
 from datetime import datetime
 from io import BytesIO
+from unittest.mock import MagicMock
+from typing import Optional, AsyncIterator, Any, MutableMapping
 from azure.containerregistry import (
     RepositoryProperties,
     ArtifactManifestProperties,
     ArtifactManifestOrder,
     ArtifactTagProperties,
     ArtifactTagOrder,
+    ArtifactArchitecture,
+    ArtifactOperatingSystem,
+    DigestValidationError,
 )
 from azure.containerregistry.aio import ContainerRegistryClient
 from azure.containerregistry._helpers import DOCKER_MANIFEST, OCI_IMAGE_MANIFEST, DEFAULT_CHUNK_SIZE
-from azure.core.exceptions import ResourceNotFoundError, ClientAuthenticationError, HttpResponseError
+from azure.core.exceptions import (
+    ResourceNotFoundError,
+    ClientAuthenticationError,
+    HttpResponseError,
+    ServiceRequestError,
+    ServiceResponseError,
+)
 from azure.core.async_paging import AsyncItemPaged
+from azure.core.pipeline import PipelineRequest
 from azure.identity import AzureAuthorityHosts
 from asynctestcase import AsyncContainerRegistryTestClass, get_authority, get_audience
-from constants import HELLO_WORLD, ALPINE, BUSYBOX, DOES_NOT_EXIST
+from testcase import is_public_endpoint
+from constants import HELLO_WORLD, DOES_NOT_EXIST
 from preparer import acr_preparer
 from devtools_testutils.aio import recorded_by_proxy_async
 
 
 class TestContainerRegistryClientAsync(AsyncContainerRegistryTestClass):
     @acr_preparer()
     @recorded_by_proxy_async
@@ -36,15 +48,15 @@
             repositories = client.list_repository_names()
             assert isinstance(repositories, AsyncItemPaged)
 
             count = 0
             prev = None
             async for repo in repositories:
                 count += 1
-                assert isinstance(repo, six.string_types)
+                assert isinstance(repo, str)
                 assert prev != repo
                 prev = repo
 
             assert count > 0
 
     @acr_preparer()
     @recorded_by_proxy_async
@@ -55,56 +67,56 @@
 
             repository_pages = client.list_repository_names(results_per_page=results_per_page)
 
             prev = None
             async for page in repository_pages.by_page():
                 page_count = 0
                 async for repo in page:
-                    assert isinstance(repo, six.string_types)
+                    assert isinstance(repo, str)
                     assert prev != repo
                     prev = repo
                     page_count += 1
                 assert page_count <= results_per_page
                 total_pages += 1
 
             assert total_pages >= 1
 
     @acr_preparer()
     @recorded_by_proxy_async
     async def test_delete_repository(self, containerregistry_endpoint):
         repo = self.get_resource_name("repo")
-        self.import_image(containerregistry_endpoint, HELLO_WORLD, [repo])
+        self.import_image(containerregistry_endpoint, repo, ["test"])
+        self.sleep(5)
         async with self.create_registry_client(containerregistry_endpoint) as client:
             await client.delete_repository(repo)
 
-            self.sleep(10)
+            self.sleep(5)
             with pytest.raises(ResourceNotFoundError):
                 await client.get_repository_properties(repo)
 
     @acr_preparer()
     @recorded_by_proxy_async
     async def test_delete_repository_does_not_exist(self, containerregistry_endpoint):
         async with self.create_registry_client(containerregistry_endpoint) as client:
             await client.delete_repository(DOES_NOT_EXIST)
 
     @acr_preparer()
     @recorded_by_proxy_async
     async def test_get_repository_properties(self, containerregistry_endpoint):
         async with self.create_registry_client(containerregistry_endpoint) as client:
-            properties = await client.get_repository_properties(ALPINE)
+            properties = await client.get_repository_properties(HELLO_WORLD)
             assert isinstance(properties, RepositoryProperties)
-            assert properties.name == ALPINE
+            assert properties.name == HELLO_WORLD
 
     @acr_preparer()
     @recorded_by_proxy_async
     async def test_update_repository_properties(self, containerregistry_endpoint):
         repo = self.get_resource_name("repo")
-        tag = self.get_resource_name("tag")
-        self.import_image(containerregistry_endpoint, HELLO_WORLD, [f"{repo}:{tag}"])
-
+        self.import_image(containerregistry_endpoint, repo, ["test"])
+        self.sleep(5)
         async with self.create_registry_client(containerregistry_endpoint) as client:
             properties = self.set_all_properties(RepositoryProperties(), False)
             received = await client.update_repository_properties(repo, properties)
             self.assert_all_properties(received, False)
 
             properties = self.set_all_properties(properties, True)
             received = await client.update_repository_properties(repo, properties)
@@ -113,17 +125,16 @@
             # Cleanup
             await client.delete_repository(repo)
 
     @acr_preparer()
     @recorded_by_proxy_async
     async def test_update_repository_properties_kwargs(self, containerregistry_endpoint):
         repo = self.get_resource_name("repo")
-        tag = self.get_resource_name("tag")
-        self.import_image(containerregistry_endpoint, HELLO_WORLD, [f"{repo}:{tag}"])
-
+        self.import_image(containerregistry_endpoint, repo, ["test"])
+        self.sleep(5)
         async with self.create_registry_client(containerregistry_endpoint) as client:
             received = await client.update_repository_properties(
                 repo, can_delete=False, can_read=False, can_write=False, can_list=False
             )
             self.assert_all_properties(received, False)
 
             received = await client.update_repository_properties(
@@ -135,31 +146,31 @@
             await client.delete_repository(repo)
 
     @acr_preparer()
     @recorded_by_proxy_async
     async def test_list_registry_artifacts(self, containerregistry_endpoint):
         async with self.create_registry_client(containerregistry_endpoint) as client:
             count = 0
-            async for artifact in client.list_manifest_properties(BUSYBOX):
+            async for artifact in client.list_manifest_properties(HELLO_WORLD):
                 assert isinstance(artifact, ArtifactManifestProperties)
                 assert isinstance(artifact.created_on, datetime)
                 assert isinstance(artifact.last_updated_on, datetime)
-                assert artifact.repository_name == BUSYBOX
-                assert artifact.fully_qualified_reference in self.create_fully_qualified_reference(containerregistry_endpoint, BUSYBOX, artifact.digest)
+                assert artifact.repository_name == HELLO_WORLD
+                assert artifact.fully_qualified_reference in self.create_fully_qualified_reference(containerregistry_endpoint, HELLO_WORLD, artifact.digest)
                 count += 1
 
             assert count > 0
 
     @acr_preparer()
     @recorded_by_proxy_async
     async def test_list_registry_artifacts_by_page(self, containerregistry_endpoint):
         async with self.create_registry_client(containerregistry_endpoint) as client:
             results_per_page = 2
 
-            pages = client.list_manifest_properties(BUSYBOX, results_per_page=results_per_page)
+            pages = client.list_manifest_properties(HELLO_WORLD, results_per_page=results_per_page)
             page_count = 0
             async for page in pages.by_page():
                 reg_count = 0
                 async for tag in page:
                     reg_count += 1
                 assert reg_count <= results_per_page
                 page_count += 1
@@ -169,15 +180,15 @@
     @acr_preparer()
     @recorded_by_proxy_async
     async def test_list_registry_artifacts_descending(self, containerregistry_endpoint):
         async with self.create_registry_client(containerregistry_endpoint) as client:
             prev_last_updated_on = None
             count = 0
             async for artifact in client.list_manifest_properties(
-                BUSYBOX, order_by=ArtifactManifestOrder.LAST_UPDATED_ON_DESCENDING
+                HELLO_WORLD, order_by=ArtifactManifestOrder.LAST_UPDATED_ON_DESCENDING
             ):
                 if prev_last_updated_on:
                     assert artifact.last_updated_on < prev_last_updated_on
                 prev_last_updated_on = artifact.last_updated_on
                 count += 1
 
             assert count > 0
@@ -185,51 +196,51 @@
     @acr_preparer()
     @recorded_by_proxy_async
     async def test_list_registry_artifacts_ascending(self, containerregistry_endpoint):
         async with self.create_registry_client(containerregistry_endpoint) as client:
             prev_last_updated_on = None
             count = 0
             async for artifact in client.list_manifest_properties(
-                BUSYBOX, order_by=ArtifactManifestOrder.LAST_UPDATED_ON_ASCENDING
+                HELLO_WORLD, order_by=ArtifactManifestOrder.LAST_UPDATED_ON_ASCENDING
             ):
                 if prev_last_updated_on:
                     assert artifact.last_updated_on > prev_last_updated_on
                 prev_last_updated_on = artifact.last_updated_on
                 count += 1
 
             assert count > 0
 
     @acr_preparer()
     @recorded_by_proxy_async
     async def test_get_manifest_properties(self, containerregistry_endpoint):
         async with self.create_registry_client(containerregistry_endpoint) as client:
-            properties = await client.get_manifest_properties(ALPINE, "latest")
+            properties = await client.get_manifest_properties(HELLO_WORLD, "latest")
             assert isinstance(properties, ArtifactManifestProperties)
-            assert properties.repository_name == ALPINE
-            assert properties.fully_qualified_reference in self.create_fully_qualified_reference(containerregistry_endpoint, ALPINE, properties.digest)
+            assert properties.repository_name == HELLO_WORLD
+            assert properties.fully_qualified_reference in self.create_fully_qualified_reference(containerregistry_endpoint, HELLO_WORLD, properties.digest)
 
     @acr_preparer()
     @recorded_by_proxy_async
     async def test_get_manifest_properties_does_not_exist(self, containerregistry_endpoint):
         async with self.create_registry_client(containerregistry_endpoint) as client:
-            manifest = await client.get_manifest_properties(ALPINE, "latest")
+            manifest = await client.get_manifest_properties(HELLO_WORLD, "latest")
             invalid_digest = manifest.digest[:-10] + u"a" * 10
 
             with pytest.raises(ResourceNotFoundError):
-                await client.get_manifest_properties(ALPINE, invalid_digest)
+                await client.get_manifest_properties(HELLO_WORLD, invalid_digest)
             with pytest.raises(ResourceNotFoundError):
                 await client.get_manifest_properties(DOES_NOT_EXIST, DOES_NOT_EXIST)
 
     @acr_preparer()
     @recorded_by_proxy_async
     async def test_update_manifest_properties(self, containerregistry_endpoint):
         repo = self.get_resource_name("repo")
-        tag = self.get_resource_name("tag")
-        self.import_image(containerregistry_endpoint, HELLO_WORLD, [f"{repo}:{tag}"])
-
+        tag = "test"
+        self.import_image(containerregistry_endpoint, repo, [tag])
+        self.sleep(5)
         async with self.create_registry_client(containerregistry_endpoint) as client: 
             properties = self.set_all_properties(ArtifactManifestProperties(), False)
             received = await client.update_manifest_properties(repo, tag, properties)
             self.assert_all_properties(received, False)
 
             properties = self.set_all_properties(properties, True)
             received = await client.update_manifest_properties(repo, tag, properties)
@@ -238,17 +249,17 @@
             # Cleanup
             await client.delete_repository(repo)
 
     @acr_preparer()
     @recorded_by_proxy_async
     async def test_update_manifest_properties_kwargs(self, containerregistry_endpoint):
         repo = self.get_resource_name("repo")
-        tag = self.get_resource_name("tag")
-        self.import_image(containerregistry_endpoint, HELLO_WORLD, [f"{repo}:{tag}"])
-
+        tag = "test"
+        self.import_image(containerregistry_endpoint, repo, [tag])
+        self.sleep(5)
         async with self.create_registry_client(containerregistry_endpoint) as client:
             received = await client.update_manifest_properties(
                 repo, tag, can_delete=False, can_read=False, can_write=False, can_list=False
             )
             self.assert_all_properties(received, False)
 
             received = await client.update_manifest_properties(
@@ -259,34 +270,34 @@
             # Cleanup
             await client.delete_repository(repo)
 
     @acr_preparer()
     @recorded_by_proxy_async
     async def test_get_tag_properties(self, containerregistry_endpoint):
         async with self.create_registry_client(containerregistry_endpoint) as client:
-            properties = await client.get_tag_properties(ALPINE, "latest")
+            properties = await client.get_tag_properties(HELLO_WORLD, "latest")
             assert isinstance(properties, ArtifactTagProperties)
             assert properties.name == "latest"
 
     @acr_preparer()
     @recorded_by_proxy_async
     async def test_get_tag_properties_does_not_exist(self, containerregistry_endpoint):
         async with self.create_registry_client(containerregistry_endpoint) as client:
             with pytest.raises(ResourceNotFoundError):
                 await client.get_tag_properties(DOES_NOT_EXIST, DOES_NOT_EXIST)
             with pytest.raises(ResourceNotFoundError):
-                await client.get_tag_properties(ALPINE, DOES_NOT_EXIST)
+                await client.get_tag_properties(HELLO_WORLD, DOES_NOT_EXIST)
 
     @acr_preparer()
     @recorded_by_proxy_async
     async def test_update_tag_properties(self, containerregistry_endpoint):
         repo = self.get_resource_name("repo")
-        tag = self.get_resource_name("tag")
-        self.import_image(containerregistry_endpoint, HELLO_WORLD, [f"{repo}:{tag}"])
-
+        tag = "test"
+        self.import_image(containerregistry_endpoint, repo, [tag])
+        self.sleep(5)
         async with self.create_registry_client(containerregistry_endpoint) as client:
             properties = self.set_all_properties(ArtifactTagProperties(), False)
             received = await client.update_tag_properties(repo, tag, properties)
             self.assert_all_properties(received, False)
 
             properties = self.set_all_properties(properties, True)
             received = await client.update_tag_properties(repo, tag, properties)
@@ -295,17 +306,17 @@
             # Cleanup
             await client.delete_repository(repo)
 
     @acr_preparer()
     @recorded_by_proxy_async
     async def test_update_tag_properties_kwargs(self, containerregistry_endpoint):
         repo = self.get_resource_name("repo")
-        tag = self.get_resource_name("tag")
-        self.import_image(containerregistry_endpoint, HELLO_WORLD, [f"{repo}:{tag}"])
-
+        tag = "test"
+        self.import_image(containerregistry_endpoint, repo, [tag])
+        self.sleep(5)
         async with self.create_registry_client(containerregistry_endpoint) as client:
             received = await client.update_tag_properties(
                 repo, tag, can_delete=False, can_read=False, can_write=False, can_list=False
             )
             self.assert_all_properties(received, False)
 
             received = await client.update_tag_properties(
@@ -315,59 +326,55 @@
 
             # Cleanup
             await client.delete_repository(repo)
 
     @acr_preparer()
     @recorded_by_proxy_async
     async def test_list_tag_properties(self, containerregistry_endpoint):
-        tags = [f"{ALPINE}:latest"]
+        tags = ["latest", "v1"]
         async with self.create_registry_client(containerregistry_endpoint) as client:
             count = 0
-            async for tag in client.list_tag_properties(ALPINE):
-                assert f"{ALPINE}:{tag.name}" in tags
+            async for tag in client.list_tag_properties(HELLO_WORLD):
+                assert tag.name in tags
                 count += 1
-            assert count == 1
+            assert count == 2
 
     @acr_preparer()
     @recorded_by_proxy_async
     async def test_list_tag_properties_order_descending(self, containerregistry_endpoint):
-        tags = [f"{ALPINE}:latest"]
         async with self.create_registry_client(containerregistry_endpoint) as client:
             prev_last_updated_on = None
             count = 0
-            async for tag in client.list_tag_properties(ALPINE, order_by=ArtifactTagOrder.LAST_UPDATED_ON_DESCENDING):
-                assert f"{ALPINE}:{tag.name}" in tags
+            async for tag in client.list_tag_properties(HELLO_WORLD, order_by=ArtifactTagOrder.LAST_UPDATED_ON_DESCENDING):
                 if prev_last_updated_on:
                     assert tag.last_updated_on < prev_last_updated_on
                 prev_last_updated_on = tag.last_updated_on
                 count += 1
-            assert count == 1
+            assert count == 2
 
     @acr_preparer()
     @recorded_by_proxy_async
     async def test_list_tag_properties_order_ascending(self, containerregistry_endpoint):
-        tags = [f"{ALPINE}:latest"]
         async with self.create_registry_client(containerregistry_endpoint) as client:
             prev_last_updated_on = None
             count = 0
-            async for tag in client.list_tag_properties(ALPINE, order_by=ArtifactTagOrder.LAST_UPDATED_ON_ASCENDING):
-                assert f"{ALPINE}:{tag.name}" in tags
+            async for tag in client.list_tag_properties(HELLO_WORLD, order_by=ArtifactTagOrder.LAST_UPDATED_ON_ASCENDING):
                 if prev_last_updated_on:
                     assert tag.last_updated_on > prev_last_updated_on
                 prev_last_updated_on = tag.last_updated_on
                 count += 1
-            assert count == 1
+            assert count == 2
 
     @acr_preparer()
     @recorded_by_proxy_async
     async def test_delete_tag(self, containerregistry_endpoint):
         repo = self.get_resource_name("repo")
-        tag = self.get_resource_name("tag")
-        self.import_image(containerregistry_endpoint, HELLO_WORLD, [f"{repo}:{tag}"])
-
+        tag = "test"
+        self.import_image(containerregistry_endpoint, repo, [tag])
+        self.sleep(5)
         async with self.create_registry_client(containerregistry_endpoint) as client:
             await client.delete_tag(repo, tag)
 
             self.sleep(10)
             with pytest.raises(ResourceNotFoundError):
                 await client.get_tag_properties(repo, tag)
 
@@ -375,43 +382,43 @@
             await client.delete_repository(repo)
 
     @acr_preparer()
     @recorded_by_proxy_async
     async def test_delete_tag_does_not_exist(self, containerregistry_endpoint):
         async with self.create_registry_client(containerregistry_endpoint) as client:
             await client.delete_tag(DOES_NOT_EXIST, DOES_NOT_EXIST)
-            await client.delete_tag(ALPINE, DOES_NOT_EXIST)
+            await client.delete_tag(HELLO_WORLD, DOES_NOT_EXIST)
 
     @acr_preparer()
     @recorded_by_proxy_async
     async def test_delete_manifest(self, containerregistry_endpoint):
         repo = self.get_resource_name("repo")
-        tag = self.get_resource_name("tag")
-        self.import_image(containerregistry_endpoint, HELLO_WORLD, [f"{repo}:{tag}"])
-
+        tag = "test"
+        self.import_image(containerregistry_endpoint, repo, [tag])
+        self.sleep(5)
         async with self.create_registry_client(containerregistry_endpoint) as client:
             await client.delete_manifest(repo, tag)
 
             self.sleep(10)
             with pytest.raises(ResourceNotFoundError):
                 await client.get_manifest_properties(repo, tag)
 
             # Cleanup
             await client.delete_repository(repo)
 
     @acr_preparer()
     @recorded_by_proxy_async
     async def test_delete_manifest_does_not_exist(self, containerregistry_endpoint):
         async with self.create_registry_client(containerregistry_endpoint) as client:
-            manifest = await client.get_manifest_properties(ALPINE, "latest")
+            manifest = await client.get_manifest_properties(HELLO_WORLD, "latest")
             invalid_digest = manifest.digest[:-10] + u"a" * 10
 
-            await client.delete_manifest(ALPINE, invalid_digest)
+            await client.delete_manifest(HELLO_WORLD, invalid_digest)
             with pytest.raises(ResourceNotFoundError):
-                await client.delete_manifest(ALPINE, DOES_NOT_EXIST)
+                await client.delete_manifest(HELLO_WORLD, DOES_NOT_EXIST)
             with pytest.raises(ResourceNotFoundError):
                 await client.delete_manifest(DOES_NOT_EXIST, DOES_NOT_EXIST)
 
     @acr_preparer()
     @recorded_by_proxy_async
     async def test_expiration_time_parsing(self, containerregistry_endpoint):
         from azure.containerregistry.aio._async_authentication_policy import ContainerRegistryChallengePolicy
@@ -444,387 +451,246 @@
             with pytest.raises(ClientAuthenticationError):
                 properties = await client.get_repository_properties(HELLO_WORLD)
 
     @acr_preparer()
     @recorded_by_proxy_async
     async def test_get_misspell_property(self, containerregistry_endpoint):
         async with self.create_registry_client(containerregistry_endpoint) as client:
-            properties = await client.get_repository_properties(ALPINE)
+            properties = await client.get_repository_properties(HELLO_WORLD)
             
             with pytest.warns(DeprecationWarning):
                 last_udpated_on = properties.last_udpated_on
             last_updated_on = properties.last_updated_on
             assert last_udpated_on == last_updated_on
     
     # Live only, as test proxy now cannot handle spaces correctly
     # issue: https://github.com/Azure/azure-sdk-tools/issues/5968
     @pytest.mark.live_test_only
     @acr_preparer()
-    @recorded_by_proxy_async
-    async def test_set_oci_manifest_json(self, containerregistry_endpoint):
+    async def test_set_oci_manifest(self, **kwargs):
+        containerregistry_endpoint = kwargs.pop("containerregistry_endpoint")
         repo = self.get_resource_name("repo")
         path = os.path.join(self.get_test_directory(), "data", "oci_artifact", "manifest.json")
         async with self.create_registry_client(containerregistry_endpoint) as client:
             await self.upload_oci_manifest_prerequisites(repo, client)
-
-            with open(path, "rb") as manifest_stream:
-                manifest_json = json.loads(manifest_stream.read().decode())
-                with pytest.raises(HttpResponseError):
-                    await client.set_manifest(repo, manifest_json, media_type=DOCKER_MANIFEST)
-            digest = await client.set_manifest(repo, manifest_json)
             
-            response = await client.get_manifest(repo, digest)
-            assert response.media_type == OCI_IMAGE_MANIFEST
-
-            await client.delete_manifest(repo, digest)
-            await client.delete_repository(repo)
-
-    # Live only, as test proxy now cannot handle spaces correctly
-    # issue: https://github.com/Azure/azure-sdk-tools/issues/5968
-    @pytest.mark.live_test_only
-    @acr_preparer()
-    @recorded_by_proxy_async
-    async def test_set_oci_manifest_json_with_tag(self, containerregistry_endpoint):
-        repo = self.get_resource_name("repo")
-        tag = "v1"
-        path = os.path.join(self.get_test_directory(), "data", "oci_artifact", "manifest.json")
-        async with self.create_registry_client(containerregistry_endpoint) as client:
-            await self.upload_oci_manifest_prerequisites(repo, client)
-
             with open(path, "rb") as manifest_stream:
+                # test set oci manifest in stream format
+                with pytest.raises(HttpResponseError):
+                    await client.set_manifest(repo, manifest_stream, tag="v1", media_type=DOCKER_MANIFEST)
+                manifest_stream.seek(0)
+                digest1 = await client.set_manifest(repo, manifest_stream, tag="v1")
+                manifest_stream.seek(0)
+                
+                # test set oci manifest in JSON format
                 manifest_json = json.loads(manifest_stream.read().decode())
                 with pytest.raises(HttpResponseError):
-                    await client.set_manifest(repo, manifest_json, tag=tag, media_type=DOCKER_MANIFEST)
-                digest = await client.set_manifest(repo, manifest_json, tag=tag)
+                    await client.set_manifest(repo, manifest_json, tag="v2", media_type=DOCKER_MANIFEST)
+                digest2 = await client.set_manifest(repo, manifest_json, tag="v2")
+                
+            assert digest1 == digest2
             
-            response = await client.get_manifest(repo, tag)
+            # test get oci manifest by digest
+            response = await client.get_manifest(repo, digest1)
             assert response.media_type == OCI_IMAGE_MANIFEST
-
-            tags = (await client.get_manifest_properties(repo, digest)).tags
-            assert len(tags) == 1
-            assert tags[0] == tag
-
-            await client.delete_manifest(repo, digest)
-            await client.delete_repository(repo)
-
-    # Live only, as test proxy now cannot handle spaces correctly
-    # issue: https://github.com/Azure/azure-sdk-tools/issues/5968
-    @pytest.mark.live_test_only
-    @acr_preparer()
-    @recorded_by_proxy_async
-    async def test_set_oci_manifest_stream(self, containerregistry_endpoint):
-        repo = self.get_resource_name("repo")
-        path = os.path.join(self.get_test_directory(), "data", "oci_artifact", "manifest.json")
-        async with self.create_registry_client(containerregistry_endpoint) as client:
-            await self.upload_oci_manifest_prerequisites(repo, client)
-
-            with open(path, "rb") as manifest_stream:
-                with pytest.raises(HttpResponseError):
-                    await client.set_manifest(repo, manifest_stream, media_type=DOCKER_MANIFEST)
-                manifest_stream.seek(0)
-                digest = await client.set_manifest(repo, manifest_stream)
             
-            response = await client.get_manifest(repo, digest)
+            # test get oci manifest by tag
+            response = await client.get_manifest(repo, "v1")
+            assert response.media_type == OCI_IMAGE_MANIFEST
+            response = await client.get_manifest(repo, "v2")
             assert response.media_type == OCI_IMAGE_MANIFEST
 
-            await client.delete_manifest(repo, digest)
+            await client.delete_manifest(repo, digest1)
             await client.delete_repository(repo)
     
+    # Reading data from a no space file to make this test pass in playback as test proxy cannot handle spaces correctly.
+    # issue: https://github.com/Azure/azure-sdk-tools/issues/5968
     @acr_preparer()
     @recorded_by_proxy_async
-    async def test_set_oci_manifest_stream_without_spaces(self, containerregistry_endpoint):
+    async def test_set_oci_manifest_without_spaces(self, containerregistry_endpoint):
+        if not is_public_endpoint(containerregistry_endpoint):
+            pytest.skip("This test is for testing test_set_docker_manifest in playback.")
+        
         repo = self.get_resource_name("repo")
-        # Reading data from a no space file to make this test pass in playback as test proxy cannot handle spaces correctly
-        # issue: https://github.com/Azure/azure-sdk-tools/issues/5968
         path = os.path.join(self.get_test_directory(), "data", "oci_artifact", "manifest_without_spaces.json")
         async with self.create_registry_client(containerregistry_endpoint) as client:
             await self.upload_oci_manifest_prerequisites(repo, client)
 
             with open(path, "rb") as manifest_stream:
+                # test set oci manifest in stream format
                 with pytest.raises(HttpResponseError):
-                    await client.set_manifest(repo, manifest_stream, media_type=DOCKER_MANIFEST)
+                    await client.set_manifest(repo, manifest_stream, tag="v1", media_type=DOCKER_MANIFEST)
                 manifest_stream.seek(0)
-                digest = await client.set_manifest(repo, manifest_stream)
-            
+                digest = await client.set_manifest(repo, manifest_stream, tag="v1")
+                
+            # test get oci manifest by digest
             response = await client.get_manifest(repo, digest)
             assert response.media_type == OCI_IMAGE_MANIFEST
-
-            await client.delete_manifest(repo, digest)
-            await client.delete_repository(repo)
-
-    # Live only, as test proxy now cannot handle spaces correctly
-    # issue: https://github.com/Azure/azure-sdk-tools/issues/5968
-    @pytest.mark.live_test_only
-    @acr_preparer()
-    @recorded_by_proxy_async
-    async def test_set_oci_manifest_stream_with_tag(self, containerregistry_endpoint):
-        repo = self.get_resource_name("repo")
-        tag = "v1"
-        path = os.path.join(self.get_test_directory(), "data", "oci_artifact", "manifest.json")
-        async with self.create_registry_client(containerregistry_endpoint) as client:
-            await self.upload_oci_manifest_prerequisites(repo, client)
             
-            with open(path, "rb") as manifest_stream:
-                with pytest.raises(HttpResponseError):
-                    await client.set_manifest(repo, manifest_stream, tag=tag, media_type=DOCKER_MANIFEST)
-                manifest_stream.seek(0)
-                digest = await client.set_manifest(repo, manifest_stream, tag=tag)
-            
-            response = await client.get_manifest(repo, tag)
+            # test get oci manifest by tag
+            response = await client.get_manifest(repo, "v1")
             assert response.media_type == OCI_IMAGE_MANIFEST
 
-            tags = (await client.get_manifest_properties(repo, digest)).tags
-            assert len(tags) == 1
-            assert tags[0] == tag
-
             await client.delete_manifest(repo, digest)
             await client.delete_repository(repo)
-    
-    @acr_preparer()
-    @recorded_by_proxy_async
-    async def test_set_oci_manifest_stream_without_spaces_with_tag(self, containerregistry_endpoint):
-        repo = self.get_resource_name("repo")
-        tag = "v1"
-        # Reading data from a no space file to make this test pass in playback as test proxy cannot handle spaces correctly
-        # issue: https://github.com/Azure/azure-sdk-tools/issues/5968
-        path = os.path.join(self.get_test_directory(), "data", "oci_artifact", "manifest_without_spaces.json")
-        async with self.create_registry_client(containerregistry_endpoint) as client:
-            await self.upload_oci_manifest_prerequisites(repo, client)
-            
-            with open(path, "rb") as manifest_stream:
-                with pytest.raises(HttpResponseError):
-                    await client.set_manifest(repo, manifest_stream, tag=tag, media_type=DOCKER_MANIFEST)
-                manifest_stream.seek(0)
-                digest = await client.set_manifest(repo, manifest_stream, tag=tag)
-            
-            response = await client.get_manifest(repo, tag)
-            assert response.media_type == OCI_IMAGE_MANIFEST
-
-            tags = (await client.get_manifest_properties(repo, digest)).tags
-            assert len(tags) == 1
-            assert tags[0] == tag
 
-            await client.delete_manifest(repo, digest)
-            await client.delete_repository(repo)
-    
     # Live only, as test proxy now cannot handle spaces correctly
     # issue: https://github.com/Azure/azure-sdk-tools/issues/5968
     @pytest.mark.live_test_only
     @acr_preparer()
-    @recorded_by_proxy_async
-    async def test_set_docker_manifest_stream(self, containerregistry_endpoint):
-        repo = "library/hello-world"
+    async def test_set_docker_manifest(self, **kwargs):
+        containerregistry_endpoint = kwargs.pop("containerregistry_endpoint")
+        repo = self.get_resource_name("repo")
         path = os.path.join(self.get_test_directory(), "data", "docker_artifact", "manifest.json")
         async with self.create_registry_client(containerregistry_endpoint) as client:
             await self.upload_docker_manifest_prerequisites(repo, client)
-
+            
             with open(path, "rb") as manifest_stream:
+                # test set Docker manifest in stream format
                 with pytest.raises(HttpResponseError):
                     # It fails as the default media type is oci image manifest media type
-                    await client.set_manifest(repo, manifest_stream)
+                    await client.set_manifest(repo, manifest_stream, tag="v1")
                 manifest_stream.seek(0)
-                digest = await client.set_manifest(repo, manifest_stream, media_type=DOCKER_MANIFEST)
-
-            response = await client.get_manifest(repo, digest)
-            assert response.media_type == DOCKER_MANIFEST
-
-            await client.delete_manifest(repo, digest)
-            await client.delete_repository(repo)
-    
-    @acr_preparer()
-    @recorded_by_proxy_async
-    async def test_set_docker_manifest_stream_without_spaces(self, containerregistry_endpoint):
-        repo = "library/hello-world"
-        # Reading data from a no space file to make this test pass in playback as test proxy cannot handle spaces correctly
-        # issue: https://github.com/Azure/azure-sdk-tools/issues/5968
-        path = os.path.join(self.get_test_directory(), "data", "docker_artifact", "manifest_without_spaces.json")
-        async with self.create_registry_client(containerregistry_endpoint) as client:
-            await self.upload_docker_manifest_prerequisites(repo, client)
-
-            with open(path, "rb") as manifest_stream:
-                with pytest.raises(HttpResponseError):
-                    # It fails as the default media type is oci image manifest media type
-                    await client.set_manifest(repo, manifest_stream)
+                digest1 = await client.set_manifest(repo, manifest_stream, tag="v1", media_type=DOCKER_MANIFEST)
                 manifest_stream.seek(0)
-                digest = await client.set_manifest(repo, manifest_stream, media_type=DOCKER_MANIFEST)
-
-            response = await client.get_manifest(repo, digest)
-            assert response.media_type == DOCKER_MANIFEST
-
-            await client.delete_manifest(repo, digest)
-            await client.delete_repository(repo)
-
-    # Live only, as test proxy now cannot handle spaces correctly
-    # issue: https://github.com/Azure/azure-sdk-tools/issues/5968
-    @pytest.mark.live_test_only
-    @acr_preparer()
-    @recorded_by_proxy_async
-    async def test_set_docker_manifest_stream_with_tag(self, containerregistry_endpoint):
-        repo = "library/hello-world"
-        tag = "v1"
-        path = os.path.join(self.get_test_directory(), "data", "docker_artifact", "manifest.json")
-        async with self.create_registry_client(containerregistry_endpoint) as client:
-            await self.upload_docker_manifest_prerequisites(repo, client)
-
-            with open(path, "rb") as manifest_stream:
+                
+                # test set Docker manifest in JSON format
+                manifest_json = json.loads(manifest_stream.read().decode())
                 with pytest.raises(HttpResponseError):
                     # It fails as the default media type is oci image manifest media type
-                    await client.set_manifest(repo, manifest_stream, tag=tag)
-                manifest_stream.seek(0)
-                digest = await client.set_manifest(repo, manifest_stream, tag=tag, media_type=DOCKER_MANIFEST)
+                    await client.set_manifest(repo, manifest_json, tag="v2")
+                digest2 = await client.set_manifest(repo, manifest_json, tag="v2", media_type=DOCKER_MANIFEST)
             
-            response = await client.get_manifest(repo, tag)
+            assert digest1 == digest2
+                
+            # test get Docker manifest by digest
+            response = await client.get_manifest(repo, digest1)
             assert response.media_type == DOCKER_MANIFEST
-
-            tags = (await client.get_manifest_properties(repo, digest)).tags
-            assert len(tags) == 1
-            assert tags[0] == tag
             
-            await client.delete_manifest(repo, digest)
+            # test get Docker manifest by tag
+            response = await client.get_manifest(repo, "v1")
+            assert response.media_type == DOCKER_MANIFEST
+            response = await client.get_manifest(repo, "v2")
+            assert response.media_type == DOCKER_MANIFEST
+
+            await client.delete_manifest(repo, digest1)
             await client.delete_repository(repo)
     
+    # Reading data from a no space file to make this test pass in playback as test proxy cannot handle spaces correctly.
+    # issue: https://github.com/Azure/azure-sdk-tools/issues/5968
     @acr_preparer()
     @recorded_by_proxy_async
-    async def test_set_docker_manifest_stream_without_spaces_with_tag(self, containerregistry_endpoint):
-        repo = "library/hello-world"
-        tag = "v1"
-        # Reading data from a no space file to make this test pass in playback as test proxy cannot handle spaces correctly
-        # issue: https://github.com/Azure/azure-sdk-tools/issues/5968
+    async def test_set_docker_manifest_without_spaces(self, containerregistry_endpoint):
+        if not is_public_endpoint(containerregistry_endpoint):
+            pytest.skip("This test is for testing test_set_docker_manifest in playback.")
+        
+        repo = self.get_resource_name("repo")
         path = os.path.join(self.get_test_directory(), "data", "docker_artifact", "manifest_without_spaces.json")
         async with self.create_registry_client(containerregistry_endpoint) as client:
             await self.upload_docker_manifest_prerequisites(repo, client)
-
+            
             with open(path, "rb") as manifest_stream:
+                # test set Docker manifest in stream format
                 with pytest.raises(HttpResponseError):
                     # It fails as the default media type is oci image manifest media type
-                    await client.set_manifest(repo, manifest_stream, tag=tag)
+                    await client.set_manifest(repo, manifest_stream, tag="v1")
                 manifest_stream.seek(0)
-                digest = await client.set_manifest(repo, manifest_stream, tag=tag, media_type=DOCKER_MANIFEST)
-            
-            response = await client.get_manifest(repo, tag)
-            assert response.media_type == DOCKER_MANIFEST
-
-            tags = (await client.get_manifest_properties(repo, digest)).tags
-            assert len(tags) == 1
-            assert tags[0] == tag
-            
-            await client.delete_manifest(repo, digest)
-            await client.delete_repository(repo)
-
-    # Live only, as test proxy now cannot handle spaces correctly
-    # issue: https://github.com/Azure/azure-sdk-tools/issues/5968
-    @pytest.mark.live_test_only
-    @acr_preparer()
-    @recorded_by_proxy_async
-    async def test_set_docker_manifest_json(self, containerregistry_endpoint):
-        repo = "library/hello-world"
-        path = os.path.join(self.get_test_directory(), "data", "docker_artifact", "manifest.json")
-        async with self.create_registry_client(containerregistry_endpoint) as client:
-            await self.upload_docker_manifest_prerequisites(repo, client)
-
-            with open(path, "rb") as manifest_stream:
-                manifest_json = json.loads(manifest_stream.read().decode())
+                digest = await client.set_manifest(repo, manifest_stream, tag="v1", media_type=DOCKER_MANIFEST)
                 
-                with pytest.raises(HttpResponseError):
-                    # It fails as the default media type is oci image manifest media type
-                    await client.set_manifest(repo, manifest_json)
-                digest = await client.set_manifest(repo, manifest_json, media_type=DOCKER_MANIFEST)
-            
+            # test get Docker manifest by digest
             response = await client.get_manifest(repo, digest)
             assert response.media_type == DOCKER_MANIFEST
-
-            await client.delete_manifest(repo, digest)
-            await client.delete_repository(repo)
-    
-    # Live only, as test proxy now cannot handle spaces correctly
-    # issue: https://github.com/Azure/azure-sdk-tools/issues/5968
-    @pytest.mark.live_test_only
-    @acr_preparer()
-    @recorded_by_proxy_async
-    async def test_set_docker_manifest_json_with_tag(self, containerregistry_endpoint):
-        repo = "library/hello-world"
-        tag = "v1"
-        path = os.path.join(self.get_test_directory(), "data", "docker_artifact", "manifest.json")
-        async with self.create_registry_client(containerregistry_endpoint) as client:
-            await self.upload_docker_manifest_prerequisites(repo, client)
-
-            with open(path, "rb") as manifest_stream:
-                manifest_json = json.loads(manifest_stream.read().decode())
-                with pytest.raises(HttpResponseError):
-                    # It fails as the default media type is oci image manifest media type
-                    await client.set_manifest(repo, manifest_json, tag=tag)
-                digest = await client.set_manifest(repo, manifest_json, tag=tag, media_type=DOCKER_MANIFEST)
             
-            response = await client.get_manifest(repo, tag)
+            # test get Docker manifest by tag
+            response = await client.get_manifest(repo, "v1")
             assert response.media_type == DOCKER_MANIFEST
 
-            tags = (await client.get_manifest_properties(repo, digest)).tags
-            assert len(tags) == 1
-            assert tags[0] == tag
-            
             await client.delete_manifest(repo, digest)
             await client.delete_repository(repo)
 
     @acr_preparer()
     @recorded_by_proxy_async
     async def test_upload_blob(self, containerregistry_endpoint):
         repo = self.get_resource_name("repo")
-        blob = "654b93f61054e4ce90ed203bb8d556a6200d5f906cf3eca0620738d6dc18cbed"
-        path = os.path.join(self.get_test_directory(), "data", "oci_artifact", blob)
+        blob = BytesIO(b"hello world")
 
         async with self.create_registry_client(containerregistry_endpoint) as client:
             # Act
-            with open(path, "rb") as data:
-                digest, blob_size = await client.upload_blob(repo, data)
+            digest, blob_size = await client.upload_blob(repo, blob)
 
             # Assert
             blob_content = b""
             stream = await client.download_blob(repo, digest)
             async for chunk in stream:
                 blob_content += chunk
             assert len(blob_content) == blob_size
 
             await client.delete_blob(repo, digest)
             await client.delete_repository(repo)
 
     @pytest.mark.live_test_only
     @acr_preparer()
-    @recorded_by_proxy_async
-    async def test_upload_large_blob_in_chunk(self, containerregistry_endpoint):
+    async def test_upload_large_blob_in_chunk(self, **kwargs):
+        containerregistry_endpoint = kwargs.pop("containerregistry_endpoint")
+        if not is_public_endpoint(containerregistry_endpoint):
+            pytest.skip("Running on non-public cloud may cause all tests finishing longer than the max time of 120 mins.")
+        
         repo = self.get_resource_name("repo")
         async with self.create_registry_client(containerregistry_endpoint) as client:
             # Test blob upload and download in equal size chunks
-            blob_size = DEFAULT_CHUNK_SIZE * 1024 # 4GB
-            data = b'\x00' * int(blob_size)
-            digest, size = await client.upload_blob(repo, BytesIO(data))
-            assert size == blob_size
-
-            stream = await client.download_blob(repo, digest)
-            size = 0
-            with open("text1.txt", "wb") as file:
-                async for chunk in stream:
-                    size += file.write(chunk)
-            assert size == blob_size
-
-            await client.delete_blob(repo, digest)
+            try:
+                blob_size = DEFAULT_CHUNK_SIZE * 1024 # 4GB
+                data = b'\x00' * int(blob_size)
+                digest, size = await client.upload_blob(repo, BytesIO(data))
+                assert size == blob_size
+
+                stream = await client.download_blob(repo, digest)
+                size = 0
+                with open("text1.txt", "wb") as file:
+                    async for chunk in stream:
+                        size += file.write(chunk)
+                assert size == blob_size
+
+                await client.delete_blob(repo, digest)
+            except (ServiceRequestError, ServiceResponseError) as err:
+                # Service does not support resumable upload when get transient error while uploading
+                # issue: https://github.com/Azure/azure-sdk-for-python/issues/29738
+                print(f"Failed to upload blob: {err.message}")
+            except ResourceNotFoundError as err:
+                # Service does not support resumable upload when get transient error while uploading
+                # issue: https://github.com/Azure/azure-sdk-for-python/issues/29738
+                assert err.status_code == 404
+                assert err.response.request.method == "PATCH"
+                assert err.response.text() == '{"errors":[{"code":"BLOB_UPLOAD_INVALID","message":"blob upload invalid"}]}\n'
 
             # Test blob upload and download in unequal size chunks
-            blob_size = DEFAULT_CHUNK_SIZE * 1024 + 20
-            data = b'\x00' * int(blob_size)
-            digest, size = await client.upload_blob(repo, BytesIO(data))
-            assert size == blob_size
-
-            stream = await client.download_blob(repo, digest)
-            size = 0
-            with open("text2.txt", "wb") as file:
-                async for chunk in stream:
-                    size += file.write(chunk)
-            assert size == blob_size
-
-            await client.delete_blob(repo, digest)
+            try:
+                blob_size = DEFAULT_CHUNK_SIZE * 1024 + 20
+                data = b'\x00' * int(blob_size)
+                digest, size = await client.upload_blob(repo, BytesIO(data))
+                assert size == blob_size
+
+                stream = await client.download_blob(repo, digest)
+                size = 0
+                with open("text2.txt", "wb") as file:
+                    async for chunk in stream:
+                        size += file.write(chunk)
+                assert size == blob_size
+
+                await client.delete_blob(repo, digest)
+            except (ServiceRequestError, ServiceResponseError) as err:
+                # Service does not support resumable upload when get transient error while uploading
+                # issue: https://github.com/Azure/azure-sdk-for-python/issues/29738
+                print(f"Failed to upload blob: {err.message}")
+            except ResourceNotFoundError as err:
+                # Service does not support resumable upload when get transient error while uploading
+                # issue: https://github.com/Azure/azure-sdk-for-python/issues/29738
+                assert err.status_code == 404
+                assert err.response.request.method == "PATCH"
+                assert err.response.text() == '{"errors":[{"code":"BLOB_UPLOAD_INVALID","message":"blob upload invalid"}]}\n'
 
             # Cleanup
             await client.delete_repository(repo)
 
     @acr_preparer()
     @recorded_by_proxy_async
     async def test_delete_blob_does_not_exist(self, containerregistry_endpoint):
@@ -858,30 +724,192 @@
             ) as client:
                 with pytest.raises(ClientAuthenticationError):
                     async for repo in client.list_repository_names():
                         pass
 
     @acr_preparer()
     @recorded_by_proxy_async
-    async def test_list_tags_in_empty_repo(self, containerregistry_endpoint):
+    async def test_list_in_empty_repo(self, containerregistry_endpoint):
+        repo = self.get_resource_name("repo")
+        self.import_image(containerregistry_endpoint, repo, ["test"])
+        self.sleep(5)
         async with self.create_registry_client(containerregistry_endpoint) as client:
-            # cleanup tags in ALPINE repo
-            async for tag in client.list_tag_properties(ALPINE):
-                await client.delete_tag(ALPINE, tag.name)
-            
-            response = client.list_tag_properties(ALPINE)
-            if response is not None:
-                async for tag in response:
-                    pass
+            # cleanup tags in repo
+            async for tag in client.list_tag_properties(repo):
+                await client.delete_tag(repo, tag.name)
+            
+            # test list tags in empty repo
+            response = client.list_tag_properties(repo)
+            async for tag in response:
+                # cleanup manifests in repo
+                await client.delete_manifest(repo, tag.name)
+
+            # test list manifests in empty repo
+            response = client.list_manifest_properties(repo)
+            async for manifest in response:
+                pass
+            
+            await client.delete_repository(repo)
+
+
+class MyMagicMock(MagicMock):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
     
-    @acr_preparer()
-    @recorded_by_proxy_async
-    async def test_list_manifests_in_empty_repo(self, containerregistry_endpoint):
-        async with self.create_registry_client(containerregistry_endpoint) as client:
-            # cleanup manifests in ALPINE repo
-            async for tag in client.list_tag_properties(ALPINE):
-                await client.delete_manifest(ALPINE, tag.name)
-
-            response = client.list_manifest_properties(ALPINE)
-            if response is not None:
-                async for manifest in response:
+    async def __aenter__(self):
+        return self
+    
+    async def __aexit__(self, *args):
+        return self
+
+
+class TestContainerRegistryClientAsyncUnitTests:
+    containerregistry_endpoint="https://fake_url.azurecr.io"
+    
+    def text(self, encoding: Optional[str] = None) -> str:
+            return '{"hello": "world"}'
+
+    @pytest.mark.asyncio
+    async def test_manifest_digest_validation(self):
+        JSON = MutableMapping[str, Any]
+            
+        async def send_in_set_manifest(request: PipelineRequest, **kwargs) -> MyMagicMock:
+            content_digest = hashlib.sha256(b"hello world").hexdigest()
+            return MyMagicMock(
+                status_code=201,
+                headers={"Docker-Content-Digest": content_digest},
+                content_type="application/json; charset=utf-8",
+                text=self.text
+        )
+        
+        async def read() -> bytes:
+            return b'{"hello": "world"}'
+        
+        def json() -> JSON:
+            return {"hello": "world"}
+        
+        async def send_in_get_manifest(request: PipelineRequest, **kwargs) -> MyMagicMock:
+            content_digest = hashlib.sha256(b"hello world").hexdigest()
+            content_type = "application/vnd.oci.image.manifest.v1+json"
+            return MyMagicMock(
+                status_code=200,
+                headers={"Docker-Content-Digest": content_digest, "Content-Type": content_type, "Content-Length": len(b"hello world")},
+                read=read,
+                json=json
+        )
+            
+        async with ContainerRegistryClient(
+            endpoint=self.containerregistry_endpoint, transport = MyMagicMock(send=send_in_set_manifest)
+        ) as client:
+            with pytest.raises(DigestValidationError) as exp:
+                manifest = {"hello": "world"}
+                await client.set_manifest("test-repo", manifest)
+            assert str(exp.value) == "The server-computed digest does not match the client-computed digest."
+            
+        async with ContainerRegistryClient(
+            endpoint=self.containerregistry_endpoint, transport = MyMagicMock(send=send_in_get_manifest)
+        ) as client:
+            with pytest.raises(DigestValidationError) as exp:
+                digest = hashlib.sha256(b"hello world").hexdigest()
+                await client.get_manifest("test-repo", f"sha256:{digest}")
+            assert str(exp.value) == "The content of retrieved manifest digest does not match the requested digest."
+                
+            with pytest.raises(DigestValidationError) as exp:
+                await client.get_manifest("test-repo", "test-tag")
+            assert str(exp.value) == "The server-computed digest does not match the client-computed digest."
+
+    @pytest.mark.asyncio
+    async def test_blob_digest_validation(self):
+        async def send_in_upload_blob(request: PipelineRequest, **kwargs) -> MyMagicMock:
+            if request.method == "PUT":
+                content_digest = hashlib.sha256(b"hello world").hexdigest()
+                return MyMagicMock(
+                    status_code=201,
+                    headers={"Docker-Content-Digest": content_digest},
+                    content_type="application/json; charset=utf-8",
+                    text=self.text
+                )
+            else:
+                return MyMagicMock(
+                    status_code=202,
+                    headers={"Location": "/v2/test-repo/blobs/uploads/fake_location"},
+                    content_type="application/json; charset=utf-8",
+                    text=self.text
+                )
+        
+        async def iter_bytes() -> AsyncIterator[bytes]:
+            yield b'{"hello": "world"}'
+        
+        async def send_in_download_blob(request: PipelineRequest, **kwargs) -> MyMagicMock:
+            return MyMagicMock(
+                status_code=206,
+                headers={"Content-Range": "bytes 0-27/28", "Content-Length": "28"},
+                content_type="application/octet-stream",
+                text=self.text,
+                iter_bytes=iter_bytes
+            )
+            
+        async with ContainerRegistryClient(
+            endpoint=self.containerregistry_endpoint, transport = MyMagicMock(send=send_in_upload_blob)
+        ) as client:
+            with pytest.raises(DigestValidationError) as exp:
+                await client.upload_blob("test-repo", BytesIO(b'{"hello": "world"}'))
+            assert str(exp.value) == "The server-computed digest does not match the client-computed digest."
+            
+        async with ContainerRegistryClient(
+            endpoint=self.containerregistry_endpoint, transport = MyMagicMock(send=send_in_download_blob)
+        ) as client:
+            digest = hashlib.sha256(b"hello world").hexdigest()
+            stream = await client.download_blob("test-repo", f"sha256:{digest}")
+            with pytest.raises(DigestValidationError) as exp:
+                async for chunk in stream:
                     pass
+            assert str(exp.value) == "The content of retrieved blob digest does not match the requested digest."
+    
+    @pytest.mark.asyncio
+    async def test_deserialize_manifest(self):
+        def get_manifest(encoding: Optional[str] = None) -> str:
+            manifest = {
+                "manifests": [
+                    {
+                        "mediaType": "application/vnd.docker.distribution.manifest.v2+json",
+                        "imageSize": 2199,
+                        "digest": "sha256:86fed9f0203a09f13cbbb9842132e9000eeff51b3de0d4ff66ee03ab0e860d1f",
+                        "architecture": "amd64",
+                        "os": "linux"
+                    },
+                    {
+                        "mediaType": "application/vnd.docker.distribution.manifest.v2+json",
+                        "imageSize": 566,
+                        "digest": "sha256:b808af65792ab617b9032c20fb12c455dc2bf5efe1af3f0ac81a129560772d35",
+                        "annotations": {
+                            "vnd.docker.reference.digest": "sha256:86fed9f0203a09f13cbbb9842132e9000eeff51b3de0d4ff66ee03ab0e860d1f",
+                            "vnd.docker.reference.type": "attestation-manifest"
+                        },
+                        "architecture": "unknown",
+                        "os": "unknown",
+                    }
+                ]
+            }
+            return json.dumps(manifest)
+        async def send(request: PipelineRequest, **kwargs) -> MyMagicMock:
+            return MyMagicMock(
+                status_code=200,
+                content_type="application/json; charset=utf-8",
+                text=get_manifest,
+        )
+        
+        async with ContainerRegistryClient(
+            endpoint=self.containerregistry_endpoint, transport = MyMagicMock(send=send)
+        ) as client:
+            manifests = client.list_manifest_properties(HELLO_WORLD)
+            async for manifest in manifests:
+                if manifest.size_in_bytes == 2199:
+                    assert isinstance(manifest.architecture, ArtifactArchitecture)
+                    assert manifest.architecture == "amd64"
+                    assert isinstance(manifest.operating_system, ArtifactOperatingSystem)
+                    assert manifest.operating_system == "linux"
+                if manifest.size_in_bytes == 566:
+                    assert isinstance(manifest.architecture, str)
+                    assert manifest.architecture == "unknown"
+                    assert isinstance(manifest.operating_system, str)
+                    assert manifest.operating_system == "unknown"
```

## Comparing `azure-containerregistry-1.1.0b4/tests/perfstress_tests/list_artifacts.py` & `azure-containerregistry-1.2.0/tests/perfstress_tests/list_artifacts.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b4/tests/perfstress_tests/list_repositories.py` & `azure-containerregistry-1.2.0/tests/perfstress_tests/list_repositories.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b4/azure/containerregistry/_download_stream.py` & `azure-containerregistry-1.2.0/azure/containerregistry/_download_stream.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 # ------------------------------------
 import hashlib
 from typing import Iterator, ContextManager, cast, Tuple, Dict, Any
 from typing_extensions import Protocol, Self
 from azure.core.pipeline import PipelineResponse
+from ._models import DigestValidationError
 
 
 class GetNext(Protocol):
     def __call__(self, *args: Any, range_header: str) -> Iterator[bytes]:
         pass
 
 
@@ -62,19 +63,21 @@
         )
         self._downloaded += int(headers["Content-Length"])
         return next_chunk
 
     def __next__(self) -> bytes:
         try:
             return self._yield_data()
-        except StopIteration:
+        except StopIteration as exc:
             if self._downloaded >= self._blob_size:
                 computed_digest = "sha256:" + self._hasher.hexdigest()
                 if computed_digest != self._digest:
-                    raise ValueError("The requested digest does not match the digest of the received blob.")
+                    raise DigestValidationError(
+                        "The content of retrieved blob digest does not match the requested digest."
+                    ) from exc
                 raise
             self._response = self._download_chunk()
             self._response_bytes = self._response.http_response.iter_bytes()
             return self.__next__()
 
     def close(self):
         self._response.http_response.close()
```

## Comparing `azure-containerregistry-1.1.0b4/azure/containerregistry/__init__.py` & `azure-containerregistry-1.2.0/azure/containerregistry/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from ._models import (
     ArtifactArchitecture,
     ArtifactOperatingSystem,
     ArtifactManifestProperties,
     RepositoryProperties,
     ArtifactTagProperties,
     GetManifestResult,
+    DigestValidationError,
 )
 from ._download_stream import DownloadBlobStream
 from ._version import VERSION
 
 __version__ = VERSION
 
 __all__ = [
@@ -31,8 +32,9 @@
     "ArtifactManifestOrder",
     "ArtifactManifestProperties",
     "RepositoryProperties",
     "ArtifactTagOrder",
     "ArtifactTagProperties",
     "GetManifestResult",
     "DownloadBlobStream",
+    "DigestValidationError",
 ]
```

## Comparing `azure-containerregistry-1.1.0b4/azure/containerregistry/_exchange_client.py` & `azure-containerregistry-1.2.0/azure/containerregistry/_exchange_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,19 +29,18 @@
 class ACRExchangeClient(object):
     """Class for handling oauth authentication requests
 
     :param endpoint: Azure Container Registry endpoint
     :type endpoint: str
     :param credential: Credential which provides tokens to authenticate requests
     :type credential: ~azure.core.credentials.TokenCredential
-    :keyword api_version: API Version. The default value is "2021-07-01". Note that overriding this default value
-        may result in unsupported behavior.
+    :keyword api_version: API Version. The default value is "2021-07-01".
     :paramtype api_version: str
     :keyword credential_scopes: The scopes that access token can request.
-    :paramtype credential_scopes: List[str]
+    :paramtype credential_scopes: list[str]
     """
 
     def __init__(self, endpoint: str, credential: TokenCredential, **kwargs) -> None:
         if not endpoint.startswith("https://") and not endpoint.startswith("http://"):
             endpoint = "https://" + endpoint
         self._endpoint = endpoint
         self.credential_scopes = kwargs.get("credential_scopes", ["https://management.core.windows.net/.default"])
@@ -52,37 +51,37 @@
             authentication_policy=ExchangeClientAuthenticationPolicy(),
             **kwargs
         )
         self._credential = credential
         self._refresh_token = None # type: Optional[str]
         self._expiration_time = 0 # type: float
 
-    def get_acr_access_token(self, challenge: str, **kwargs) -> Optional[str]:
+    def get_acr_access_token(self, challenge: str, **kwargs) -> Optional[str]: # pylint:disable=client-method-missing-tracing-decorator
         parsed_challenge = _parse_challenge(challenge)
         refresh_token = self.get_refresh_token(parsed_challenge["service"], **kwargs)
         return self.exchange_refresh_token_for_access_token(
             refresh_token, service=parsed_challenge["service"], scope=parsed_challenge["scope"], **kwargs
         )
 
-    def get_refresh_token(self, service: str, **kwargs) -> str:
+    def get_refresh_token(self, service: str, **kwargs) -> str: # pylint:disable=client-method-missing-tracing-decorator
         if not self._refresh_token or self._expiration_time - time.time() > 300:
             self._refresh_token = self.exchange_aad_token_for_refresh_token(service, **kwargs)
             self._expiration_time = _parse_exp_time(self._refresh_token)
         return self._refresh_token
 
-    def exchange_aad_token_for_refresh_token(self, service: str, **kwargs) -> str:
+    def exchange_aad_token_for_refresh_token(self, service: str, **kwargs) -> str: # pylint:disable=client-method-missing-tracing-decorator
         refresh_token = self._client.authentication.exchange_aad_access_token_for_acr_refresh_token( # type: ignore
             grant_type=PostContentSchemaGrantType.ACCESS_TOKEN,
             service=service,
             access_token=self._credential.get_token(*self.credential_scopes).token,
             **kwargs
         )
         return refresh_token.refresh_token if refresh_token.refresh_token is not None else ""
 
-    def exchange_refresh_token_for_access_token(
+    def exchange_refresh_token_for_access_token( # pylint:disable=client-method-missing-tracing-decorator
         self, refresh_token: str, service: str, scope: str, **kwargs
     ) -> Optional[str]:
         access_token = self._client.authentication.exchange_acr_refresh_token_for_acr_access_token( # type: ignore
             service=service, scope=scope, refresh_token=refresh_token, **kwargs
         )
         return access_token.access_token
```

## Comparing `azure-containerregistry-1.1.0b4/azure/containerregistry/_models.py` & `azure-containerregistry-1.2.0/azure/containerregistry/_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,45 +49,51 @@
     NETBSD = "netbsd"
     OPENBSD = "openbsd"
     PLAN9 = "plan9"
     SOLARIS = "solaris"
     WINDOWS = "windows"
 
 
-class ArtifactManifestProperties(object):  # pylint: disable=too-many-instance-attributes
+class ArtifactManifestProperties:  # pylint: disable=too-many-instance-attributes
     """Represents properties of a registry artifact.
 
     :ivar bool can_delete: Delete Permissions for an artifact.
     :ivar bool can_write: Write Permissions for an artifact.
     :ivar bool can_read: Read Permissions for an artifact.
     :ivar bool can_list: List Permissions for an artifact.
     :ivar architecture: CPU Architecture of an artifact.
-    :vartype architecture: Optional[~azure.containerregistry.ArtifactArchitecture]
+        Note: any value not listed in enum ArtifactArchitecture will be string type.
+    :vartype architecture: Optional[Union[str, ~azure.containerregistry.ArtifactArchitecture]]
     :ivar created_on: Time and date an artifact was created.
     :vartype created_on: Optional[~datetime.datetime]
     :ivar Optional[str] digest: Digest for the artifact.
     :ivar last_updated_on: Time and date an artifact was last updated.
     :vartype last_updated_on: Optional[~datetime.datetime]
     :ivar operating_system: Operating system for the artifact.
-    :vartype operating_system: Optional[~azure.containerregistry.ArtifactOperatingSystem]
+        Note: any value not listed in enum ArtifactOperatingSystem will be string type.
+    :vartype operating_system: Optional[Union[str, ~azure.containerregistry.ArtifactOperatingSystem]]
     :ivar Optional[str] repository_name: Repository name the artifact belongs to.
     :ivar Optional[int] size_in_bytes: Size of the artifact.
     :ivar Optional[List[str]] tags: Tags associated with a registry artifact.
     """
 
     def __init__(self, **kwargs):
         self._architecture = kwargs.get("cpu_architecture", None)
-        if self._architecture is not None:
+        try:
             self._architecture = ArtifactArchitecture(self._architecture)
+        except ValueError:
+            pass
         self._created_on = kwargs.get("created_on", None)
         self._digest = kwargs.get("digest", None)
         self._last_updated_on = kwargs.get("last_updated_on", None)
         self._operating_system = kwargs.get("operating_system", None)
-        if self._operating_system is not None:
+        try:
             self._operating_system = ArtifactOperatingSystem(self._operating_system)
+        except ValueError:
+            pass
         self._repository_name = kwargs.get("repository_name", None)
         self._registry = kwargs.get("registry", None)
         self._size_in_bytes = kwargs.get("size_in_bytes", None)
         self._tags = kwargs.get("tags", None)
         self.can_delete = kwargs.get("can_delete")
         self.can_read = kwargs.get("can_read")
         self.can_list = kwargs.get("can_list")
@@ -152,15 +158,15 @@
         return self._tags
 
     @property
     def fully_qualified_reference(self) -> str:
         return f"{_host_only(self._registry)}/{self._repository_name}{':' if _is_tag(self._digest) else '@'}{_strip_alg(self._digest)}" # pylint: disable=line-too-long
 
 
-class RepositoryProperties(object):
+class RepositoryProperties:
     """Represents properties of a single repository.
 
     :ivar bool can_delete: Delete Permissions for a repository.
     :ivar bool can_write: Write Permissions for a repository.
     :ivar bool can_read: Read Permissions for a repository.
     :ivar bool can_list: List Permissions for a repository.
     :ivar created_on: Time the repository was created
@@ -230,15 +236,15 @@
         return self._name
 
     @property
     def tag_count(self) -> int:
         return self._tag_count
 
 
-class ArtifactTagProperties(object):
+class ArtifactTagProperties:
     """Represents properties of a single tag
 
     :ivar bool can_delete: Delete Permissions for a tag.
     :ivar bool can_write: Write Permissions for a tag.
     :ivar bool can_read: Read Permissions for a tag.
     :ivar bool can_list: List Permissions for a tag.
     :ivar created_on: Time the tag was created.
@@ -300,19 +306,31 @@
         return self._name
 
     @property
     def repository_name(self) -> str:
         return self._repository_name
 
 
-class GetManifestResult(object):
+class GetManifestResult:
     """The get manifest result.
 
-    :ivar dict manifest: The manifest JSON.
+    :ivar manifest: The manifest JSON.
+    :vartype manifest: Mapping[str, Any]
     :ivar str media_type: The manifest's media type.
     :ivar str digest: The manifest's digest, calculated by the registry.
     """
 
     def __init__(self, **kwargs):
         self.manifest = kwargs.get("manifest")
         self.media_type = kwargs.get("media_type")
         self.digest = kwargs.get("digest")
+
+
+class DigestValidationError(ValueError):
+    """Thrown when a manifest digest validation fails.
+
+    :param str message: Message for caller describing the reason for the failure.
+    """
+
+    def __init__(self, message):
+        self.message = message
+        super().__init__(self.message)
```

## Comparing `azure-containerregistry-1.1.0b4/azure/containerregistry/_base_client.py` & `azure-containerregistry-1.2.0/azure/containerregistry/_base_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,17 +25,16 @@
 class ContainerRegistryBaseClient(object):
     """Base class for ContainerRegistryClient
 
     :param str endpoint: Azure Container Registry endpoint
     :param credential: Token credential for authenticating requests with Azure, or None in anonymous access
     :type credential: ~azure.core.credentials.TokenCredential or None
     :keyword credential_scopes: URL for credential authentication if different from the default
-    :paramtype credential_scopes: List[str]
-    :keyword api_version: API Version. The default value is "2021-07-01". Note that overriding this default value
-        may result in unsupported behavior.
+    :paramtype credential_scopes: list[str]
+    :keyword api_version: API Version. The default value is "2021-07-01".
     :paramtype api_version: str
     """
 
     def __init__(self, endpoint: str, credential: Optional[TokenCredential], **kwargs) -> None:
         self._auth_policy = ContainerRegistryChallengePolicy(credential, endpoint, **kwargs)
         self._client = ContainerRegistry(
             credential=credential or AnonymousAccessCredential(),
```

## Comparing `azure-containerregistry-1.1.0b4/azure/containerregistry/_authentication_policy.py` & `azure-containerregistry-1.2.0/azure/containerregistry/_authentication_policy.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,22 +28,26 @@
             self._exchange_client = ACRExchangeClient(endpoint, self._credential, **kwargs)
 
     def on_request(self, request: PipelineRequest) -> None:
         """Called before the policy sends a request.
         The base implementation authorizes the request with a bearer token.
 
         :param ~azure.core.pipeline.PipelineRequest request: the request
+        :return: None
+        :rtype: None
         """
         # Future caching implementation will be included here
         pass  # pylint: disable=unnecessary-pass
 
     def send(self, request: PipelineRequest) -> PipelineResponse:
         """Authorizes a request with a bearer token, possibly handling an authentication challenge
 
-        :param ~azure.core.pipeline.PipelineRequest request: the request
+        :param ~azure.core.pipeline.PipelineRequest request: The pipeline request object.
+        :return: The pipeline response object.
+        :rtype: ~azure.core.pipeline.PipelineResponse
         """
         _enforce_https(request)
 
         self.on_request(request)
 
         response = self.next.send(request)
 
@@ -66,16 +70,17 @@
         """Authorize request according to an authentication challenge
         This method is called when the resource provider responds 401 with a WWW-Authenticate header.
 
         :param ~azure.core.pipeline.PipelineRequest request: the request which elicited an authentication challenge
         :param ~azure.core.pipeline.PipelineResponse response: the resource provider's response
         :param str challenge: response's WWW-Authenticate header, unparsed. It may contain multiple challenges.
         :returns: a bool indicating whether the policy should send the request
+        :rtype: bool
         """
-        # pylint:disable=unused-argument, no-self-use
+        # pylint:disable=unused-argument
 
         access_token = self._exchange_client.get_acr_access_token(challenge)
         if access_token is not None:
             request.http_request.headers["Authorization"] = "Bearer " + access_token
         return access_token is not None
 
     def __enter__(self):
```

## Comparing `azure-containerregistry-1.1.0b4/azure/containerregistry/_container_registry_client.py` & `azure-containerregistry-1.2.0/azure/containerregistry/_container_registry_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,25 +26,29 @@
 from ._generated.models import AcrErrors
 from ._download_stream import DownloadBlobStream
 from ._helpers import (
     _compute_digest,
     _is_tag,
     _parse_next_link,
     _validate_digest,
+    _get_blob_size,
+    _get_manifest_size,
     SUPPORTED_API_VERSIONS,
     OCI_IMAGE_MANIFEST,
     SUPPORTED_MANIFEST_MEDIA_TYPES,
     DEFAULT_AUDIENCE,
     DEFAULT_CHUNK_SIZE,
+    MAX_MANIFEST_SIZE,
 )
 from ._models import (
     RepositoryProperties,
     ArtifactTagProperties,
     ArtifactManifestProperties,
     GetManifestResult,
+    DigestValidationError,
 )
 
 JSON = MutableMapping[str, Any]
 
 def _return_response(pipeline_response, _, __):
     return pipeline_response
 
@@ -66,16 +70,15 @@
         **kwargs
     ) -> None:
         """Create a ContainerRegistryClient from an ACR endpoint and a credential.
 
         :param str endpoint: An ACR endpoint.
         :param credential: The credential with which to authenticate. This should be None in anonymous access.
         :type credential: ~azure.core.credentials.TokenCredential or None
-        :keyword api_version: API Version. The default value is "2021-07-01". Note that overriding this default value
-         may result in unsupported behavior.
+        :keyword api_version: API Version. The default value is "2021-07-01".
         :paramtype api_version: str
         :keyword audience: URL to use for credential authentication with AAD. Its value could be
             "https://management.azure.com", "https://management.chinacloudapi.cn" or
             "https://management.usgovcloudapi.net". The default value is "https://containerregistry.azure.net".
         :paramtype audience: str
         :returns: None
         :rtype: None
@@ -239,14 +242,15 @@
 
     @distributed_trace
     def get_repository_properties(self, repository: str, **kwargs) -> RepositoryProperties:
         """Get the properties of a repository
 
         :param str repository: Name of the repository
         :rtype: ~azure.containerregistry.RepositoryProperties
+        :return: The properties of a repository
         :raises: ~azure.core.exceptions.ResourceNotFoundError
         """
         return RepositoryProperties._from_generated(  # pylint: disable=protected-access
             self._client.container_registry.get_properties(repository, **kwargs)
         )
 
     @distributed_trace
@@ -393,14 +397,15 @@
 
     @distributed_trace
     def get_manifest_properties(self, repository: str, tag_or_digest: str, **kwargs) -> ArtifactManifestProperties:
         """Get the properties of a registry artifact
 
         :param str repository: Name of the repository
         :param str tag_or_digest: Tag or digest of the manifest
+        :return: The properties of a registry artifact
         :rtype: ~azure.containerregistry.ArtifactManifestProperties
         :raises: ~azure.core.exceptions.ResourceNotFoundError
 
         Example
 
         .. code-block:: python
 
@@ -425,14 +430,15 @@
 
     @distributed_trace
     def get_tag_properties(self, repository: str, tag: str, **kwargs) -> ArtifactTagProperties:
         """Get the properties for a tag
 
         :param str repository: Name of the repository
         :param str tag: The tag to get tag properties for
+        :return: The properties for a tag
         :rtype: ~azure.containerregistry.ArtifactTagProperties
         :raises: ~azure.core.exceptions.ResourceNotFoundError
 
         Example
 
         .. code-block:: python
 
@@ -880,16 +886,17 @@
         :paramtype tag: str or None
         :keyword media_type: The media type of the manifest. If not specified, this value will be set to
             a default value of "application/vnd.oci.image.manifest.v1+json". Note: the current known media types are:
             "application/vnd.oci.image.manifest.v1+json", and "application/vnd.docker.distribution.manifest.v2+json".
         :paramtype media_type: str
         :returns: The digest of the set manifest, calculated by the registry.
         :rtype: str
-        :raises ValueError: If the parameter repository or manifest is None,
-            or the digest in the response does not match the digest of the set manifest.
+        :raises ValueError: If the parameter repository or manifest is None.
+        :raises ~azure.containerregistry.DigestValidationError:
+            If the server-computed digest does not match the client-computed digest.
         """
         try:
             data: IO[bytes]
             if isinstance(manifest, MutableMapping):
                 data = BytesIO(json.dumps(manifest).encode())
             else:
                 data = manifest
@@ -903,15 +910,17 @@
                 payload=data,
                 content_type=media_type,
                 cls=_return_response_headers,
                 **kwargs
             )
             digest = response_headers['Docker-Content-Digest']
             if not _validate_digest(data, digest):
-                raise ValueError("The server-computed digest does not match the client-computed digest.")
+                raise DigestValidationError(
+                    "The server-computed digest does not match the client-computed digest."
+                )
         except Exception as e:
             if repository is None or manifest is None:
                 raise ValueError("The parameter repository and manifest cannot be None.") from e
             raise
         return digest
 
     @distributed_trace
@@ -920,50 +929,64 @@
 
         :param str repository: Name of the repository.
         :param str tag_or_digest: The tag or digest of the manifest to get.
             When digest is provided, will use this digest to compare with the one calculated by the response payload.
             When tag is provided, will use the digest in response headers to compare.
         :returns: GetManifestResult
         :rtype: ~azure.containerregistry.GetManifestResult
-        :raises ValueError: If the requested digest does not match the digest of the received manifest.
+        :raises ~azure.containerregistry.DigestValidationError:
+            If the content of retrieved manifest digest does not match the requested digest, or
+            the server-computed digest does not match the client-computed digest when tag is passing.
+        :raises ValueError: If the content-length header is missing or invalid in response, or the manifest size is
+            bigger than 4MB.
         """
         response = cast(
             PipelineResponse,
             self._client.container_registry.get_manifest(
                 name=repository,
                 reference=tag_or_digest,
                 accept=SUPPORTED_MANIFEST_MEDIA_TYPES,
                 cls=_return_response,
                 **kwargs
             )
         )
+        manifest_size = _get_manifest_size(response.http_response.headers)
+        # This check is to address part of the service threat model. If a manifest does not have a proper
+        # content length or is too big, it indicates a malicious or faulty service and should not be trusted.
+        if manifest_size > MAX_MANIFEST_SIZE:
+            raise ValueError("Manifest size is bigger than max allowed size of 4MB.")
         media_type = response.http_response.headers['Content-Type']
         manifest_bytes = response.http_response.read()
         manifest_json = response.http_response.json()
+        manifest_digest = _compute_digest(manifest_bytes)
         if tag_or_digest.startswith("sha256:"):
-            digest = tag_or_digest
-            if not _validate_digest(manifest_bytes, digest):
-                raise ValueError("The requested digest does not match the digest of the received manifest.")
-        else:
-            digest = response.http_response.headers['Docker-Content-Digest']
-            if not _validate_digest(manifest_bytes, digest):
-                raise ValueError("The server-computed digest does not match the client-computed digest.")
+            if manifest_digest != tag_or_digest:
+                raise DigestValidationError(
+                    "The content of retrieved manifest digest does not match the requested digest."
+                )
+        digest = response.http_response.headers['Docker-Content-Digest']
+        if manifest_digest != digest:
+            raise DigestValidationError(
+                "The server-computed digest does not match the client-computed digest."
+            )
 
         return GetManifestResult(digest=digest, manifest=manifest_json, media_type=media_type)
 
     @distributed_trace
     def upload_blob(self, repository: str, data: IO[bytes], **kwargs) -> Tuple[str, int]:
         """Upload an artifact blob.
 
         :param str repository: Name of the repository.
         :param data: The blob to upload. Note: This must be a seekable stream.
         :type data: IO
         :returns: The digest and size in bytes of the uploaded blob.
         :rtype: Tuple[str, int]
         :raises ValueError: If the parameter repository or data is None.
+        :raises ~azure.containerregistry.DigestValidationError:
+            If the server-computed digest does not match the client-computed digest.
         """
         try:
             start_upload_response_headers = cast(Dict[str, str], self._client.container_registry_blob.start_upload(
                 repository, cls=_return_response_headers, **kwargs
             ))
             digest, location, blob_size = self._upload_blob_chunk(
                 start_upload_response_headers['Location'], data, **kwargs
@@ -973,14 +996,18 @@
                 self._client.container_registry_blob.complete_upload(
                     digest=digest,
                     next_link=location,
                     cls=_return_response_headers,
                     **kwargs
                 )
             )
+            if digest != complete_upload_response_headers["Docker-Content-Digest"]:
+                raise DigestValidationError(
+                    "The server-computed digest does not match the client-computed digest."
+                )
         except Exception as e:
             if repository is None or data is None:
                 raise ValueError("The parameter repository and data cannot be None.") from e
             raise
         return complete_upload_response_headers['Docker-Content-Digest'], blob_size
 
     def _upload_blob_chunk(self, location: str, data: IO[bytes], **kwargs) -> Tuple[str, str, int]:
@@ -1004,38 +1031,41 @@
     def download_blob(self, repository: str, digest: str, **kwargs) -> DownloadBlobStream:
         """Download a blob that is part of an artifact to a stream.
 
         :param str repository: Name of the repository.
         :param str digest: The digest of the blob to download.
         :returns: DownloadBlobStream
         :rtype: ~azure.containerregistry.DownloadBlobStream
-        :raises ValueError: If the requested digest does not match the digest of the received blob.
+        :raises DigestValidationError:
+            If the content of retrieved blob digest does not match the requested digest.
+        :raises ValueError: If the content-range header is missing or invalid in response.
         """
         end_range = DEFAULT_CHUNK_SIZE - 1
         first_chunk, headers = cast(
             Tuple[PipelineResponse, Dict[str, str]],
             self._client.container_registry_blob.get_chunk(
                 repository,
                 digest,
                 range_header=f"bytes=0-{end_range}",
                 cls=_return_response_and_headers,
                 **kwargs
             )
         )
+        blob_size = _get_blob_size(headers)
         return DownloadBlobStream(
             response=first_chunk,
             digest=digest,
             get_next=functools.partial(
                 self._client.container_registry_blob.get_chunk,
                 name=repository,
                 digest=digest,
                 cls=_return_response_and_headers,
                 **kwargs
             ),
-            blob_size=int(headers["Content-Range"].split("/")[1]),
+            blob_size=blob_size,
             downloaded=int(headers["Content-Length"]),
             chunk_size=DEFAULT_CHUNK_SIZE
         )
 
     @distributed_trace
     def delete_manifest(self, repository: str, tag_or_digest: str, **kwargs) -> None:
         """Delete a manifest. If the manifest cannot be found or a response status code of
```

## Comparing `azure-containerregistry-1.1.0b4/azure/containerregistry/_anonymous_exchange_client.py` & `azure-containerregistry-1.2.0/azure/containerregistry/aio/_async_anonymous_exchange_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,73 +1,84 @@
 # coding=utf-8
 # ------------------------------------
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 # ------------------------------------
 from typing import Optional, Union
-from azure.core.credentials import TokenCredential, AccessToken
-from ._exchange_client import ExchangeClientAuthenticationPolicy
-from ._generated import ContainerRegistry
-from ._generated.models import TokenGrantType
-from ._helpers import _parse_challenge
-from ._user_agent import USER_AGENT
 
+from azure.core.credentials import AccessToken
+from azure.core.credentials_async import AsyncTokenCredential
 
-class AnonymousAccessCredential(TokenCredential):
-    def get_token(
+from ._async_exchange_client import ExchangeClientAuthenticationPolicy
+from .._generated.aio import ContainerRegistry
+from .._generated.models import TokenGrantType
+from .._helpers import _parse_challenge
+from .._user_agent import USER_AGENT
+
+
+class AsyncAnonymousAccessCredential(AsyncTokenCredential):
+    async def get_token(
         self, *scopes: str, claims: Optional[str] = None, tenant_id: Optional[str] = None, **kwargs
     ) -> AccessToken:
         raise ValueError("This credential cannot be used to obtain access tokens.")
 
+    async def close(self) -> None:
+        pass
+
+    async def __aenter__(self):
+        pass
+
+    async def __aexit__(self, exc_type, exc_value, traceback) -> None:
+        pass
+
 
 class AnonymousACRExchangeClient(object):
     """Class for handling oauth authentication requests
 
     :param endpoint: Azure Container Registry endpoint
     :type endpoint: str
-    :keyword api_version: API Version. The default value is "2021-07-01". Note that overriding this default value
-        may result in unsupported behavior.
+    :keyword api_version: Api Version. Default value is "2021-07-01".
     :paramtype api_version: str
     """
 
     def __init__(self, endpoint: str, **kwargs) -> None: # pylint: disable=missing-client-constructor-parameter-credential
         if not endpoint.startswith("https://") and not endpoint.startswith("http://"):
             endpoint = "https://" + endpoint
         self._endpoint = endpoint
         self._client = ContainerRegistry(
-            credential=AnonymousAccessCredential(),
+            credential=AsyncAnonymousAccessCredential(),
             url=endpoint,
             sdk_moniker=USER_AGENT,
             authentication_policy=ExchangeClientAuthenticationPolicy(),
             **kwargs
         )
 
-    def get_acr_access_token(self, challenge: str, **kwargs) -> Optional[str]:
+    async def get_acr_access_token(self, challenge: str, **kwargs) -> Optional[str]: # pylint:disable=client-method-missing-tracing-decorator-async
         parsed_challenge = _parse_challenge(challenge)
-        return self.exchange_refresh_token_for_access_token(
+        return await self.exchange_refresh_token_for_access_token(
             "",
             service=parsed_challenge["service"],
             scope=parsed_challenge["scope"],
             grant_type=TokenGrantType.PASSWORD,
             **kwargs
         )
 
-    def exchange_refresh_token_for_access_token(
+    async def exchange_refresh_token_for_access_token( # pylint:disable=client-method-missing-tracing-decorator-async
         self, refresh_token: str, service: str, scope: str, grant_type: Union[str, TokenGrantType], **kwargs
     ) -> Optional[str]:
-        access_token = self._client.authentication.exchange_acr_refresh_token_for_acr_access_token( # type: ignore
+        access_token = await self._client.authentication.exchange_acr_refresh_token_for_acr_access_token( # type: ignore
             service=service, scope=scope, refresh_token=refresh_token, grant_type=grant_type, **kwargs
         )
         return access_token.access_token
 
-    def __enter__(self):
-        self._client.__enter__()
+    async def __aenter__(self):
+        await self._client.__aenter__()
         return self
 
-    def __exit__(self, *args):
-        self._client.__exit__(*args)
+    async def __aexit__(self, *args):
+        await self._client.__aexit__(*args)
 
-    def close(self) -> None:
+    async def close(self) -> None:
         """Close sockets opened by the client.
         Calling this method is unnecessary when using the client as a context manager.
         """
-        self._client.close()
+        await self._client.close()
```

## Comparing `azure-containerregistry-1.1.0b4/azure/containerregistry/_helpers.py` & `azure-containerregistry-1.2.0/azure/containerregistry/_helpers.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 BEARER = "Bearer"
 AUTHENTICATION_CHALLENGE_PARAMS_PATTERN = re.compile('(?:(\\w+)="([^""]*)")+')
 SUPPORTED_API_VERSIONS = [
     "2019-08-15-preview",
     "2021-07-01"
 ]
 DEFAULT_CHUNK_SIZE = 4 * 1024 * 1024 # 4MB
+MAX_MANIFEST_SIZE = 4 * 1024 * 1024
 
 # The default audience used for all clouds when audience is not set
 DEFAULT_AUDIENCE = "https://containerregistry.azure.net"
 
 # Known manifest media types
 OCI_IMAGE_MANIFEST = "application/vnd.oci.image.manifest.v1+json"
 DOCKER_MANIFEST = "application/vnd.docker.distribution.manifest.v2+json"
@@ -42,58 +43,75 @@
 )
 
 def _is_tag(tag_or_digest: str) -> bool:
     tag = tag_or_digest.split(":")
     return not (len(tag) == 2 and tag[0].startswith("sha"))
 
 def _clean(matches: List[str]) -> None:
-    """This method removes empty strings and commas from the regex matching of the Challenge header"""
+    """This method removes empty strings and commas from the regex matching of the Challenge header.
+
+    :param list[str] matches: The regex list to clean.
+    :return: None
+    """
     while True:
         try:
             matches.remove("")
         except ValueError:
             break
 
     while True:
         try:
             matches.remove(",")
         except ValueError:
             return
 
 def _parse_challenge(header: str) -> Dict[str, str]:
-    """Parse challenge header into service and scope"""
+    """Parse challenge header into service and scope
+
+    :param str header: The challenge header to parse.
+    :return: A service and scope dict parsed from challenge header.
+    :rtype: dict[str, str]
+    """
     ret: Dict[str, str] = {}
     if header.startswith(BEARER):
         challenge_params = header[len(BEARER) + 1 :]
 
         matches = re.split(AUTHENTICATION_CHALLENGE_PARAMS_PATTERN, challenge_params)
         _clean(matches)
         for i in range(0, len(matches), 2):
             ret[matches[i]] = matches[i + 1]
 
     return ret
 
 def _parse_next_link(link_string: str) -> Optional[str]:
-    """Parses the next link in the list operations response URL
+    """Parse the next link in the list operations response URL
 
     Per the Docker v2 HTTP API spec, the Link header is an RFC5988
     compliant rel='next' with URL to next result set, if available.
     See: https://docs.docker.com/registry/spec/api/
 
     The URI reference can be obtained from link-value as follows:
     Link       = "Link" ":" #link-value
     link-value = "<" URI-Reference ">" * (";" link-param )
     See: https://tools.ietf.org/html/rfc5988#section-5
+
+    :param str link_string: The Link header in HTTP response.
+    :return: The URI reference of next link.
+    :rtype: str or None
     """
     if not link_string:
         return None
     return link_string[1 : link_string.find(">")]
 
 def _enforce_https(request: PipelineRequest) -> None:
-    """Raise ServiceRequestError if the request URL is non-HTTPS and the sender did not specify enforce_https=False"""
+    """Raise ServiceRequestError if the request URL is non-HTTPS and the sender did not specify enforce_https=False
+
+    :param ~azure.core.pipeline.PipelineRequest request: The pipeline request object.
+    :return: None
+    """
 
     # move 'enforce_https' from options to context so it persists
     # across retries but isn't passed to a transport implementation
     option = request.context.options.pop("enforce_https", None)
 
     # True is the default setting; we needn't preserve an explicit opt in to the default behavior
     if option is False:
@@ -109,16 +127,15 @@
     return urlparse(url).netloc
 
 def _strip_alg(digest):
     if len(digest.split(":")) == 2:
         return digest.split(":")[1]
     return digest
 
-def _parse_exp_time(raw_token):
-    # type: (str) -> float
+def _parse_exp_time(raw_token: str) -> float:
     raw_token_list = raw_token.split(".")
     if len(raw_token_list) > 2:
         value = raw_token_list[1]
         padding = len(value) % 4
         if padding > 0:
             value += "=" * padding
         byte_value = base64.b64decode(value).decode("utf-8")
@@ -132,10 +149,25 @@
         value = data
     else:
         data.seek(0)
         value = data.read()
         data.seek(0)
     return "sha256:" + hashlib.sha256(value).hexdigest()
 
-def _validate_digest(data: Union[IO[bytes], bytes], expected_digest: str) -> bool:
-    digest = _compute_digest(data)
-    return digest == expected_digest
+def _validate_digest(data: IO[bytes], expected_digest: str) -> bool:
+    return _compute_digest(data) == expected_digest
+
+def _get_blob_size(headers: Dict[str, str]) -> int:
+    if not headers["Content-Range"]:
+        raise ValueError("Missing content-range header in response.")
+    blob_size = int(headers["Content-Range"].split("/")[1])
+    if blob_size <= 0:
+        raise ValueError(f"Invalid content-range header in response: {blob_size}")
+    return blob_size
+
+def _get_manifest_size(headers: Dict[str, str]) -> int:
+    if not headers["Content-Length"]:
+        raise ValueError("Missing content-length header in response.")
+    manifest_size = int(headers["Content-Length"])
+    if manifest_size <= 0:
+        raise ValueError(f"Invalid content-length header in response: {manifest_size}")
+    return manifest_size
```

## Comparing `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/_client.py` & `azure-containerregistry-1.2.0/azure/containerregistry/_generated/_client.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/__init__.py` & `azure-containerregistry-1.2.0/azure/containerregistry/_generated/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/_configuration.py` & `azure-containerregistry-1.2.0/azure/containerregistry/_generated/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/_patch.py` & `azure-containerregistry-1.2.0/azure/containerregistry/_generated/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/_vendor.py` & `azure-containerregistry-1.2.0/azure/containerregistry/_generated/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/_serialization.py` & `azure-containerregistry-1.2.0/azure/containerregistry/_generated/_serialization.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/models/__init__.py` & `azure-containerregistry-1.2.0/azure/containerregistry/_generated/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/models/_models.py` & `azure-containerregistry-1.2.0/azure/containerregistry/_generated/models/_models.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/models/_patch.py` & `azure-containerregistry-1.2.0/azure/containerregistry/_generated/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/models/_enums.py` & `azure-containerregistry-1.2.0/azure/containerregistry/_generated/models/_enums.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/_client.py` & `azure-containerregistry-1.2.0/azure/containerregistry/_generated/aio/_client.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/__init__.py` & `azure-containerregistry-1.2.0/azure/containerregistry/_generated/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/_configuration.py` & `azure-containerregistry-1.2.0/azure/containerregistry/_generated/aio/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/_patch.py` & `azure-containerregistry-1.2.0/azure/containerregistry/_generated/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/_vendor.py` & `azure-containerregistry-1.2.0/azure/containerregistry/_generated/aio/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/operations/__init__.py` & `azure-containerregistry-1.2.0/azure/containerregistry/_generated/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/operations/_patch.py` & `azure-containerregistry-1.2.0/azure/containerregistry/_generated/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/aio/operations/_operations.py` & `azure-containerregistry-1.2.0/azure/containerregistry/_generated/aio/operations/_operations.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/operations/__init__.py` & `azure-containerregistry-1.2.0/azure/containerregistry/_generated/aio/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/operations/_patch.py` & `azure-containerregistry-1.2.0/azure/containerregistry/_generated/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b4/azure/containerregistry/_generated/operations/_operations.py` & `azure-containerregistry-1.2.0/azure/containerregistry/_generated/operations/_operations.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b4/azure/containerregistry/aio/_async_container_registry_client.py` & `azure-containerregistry-1.2.0/azure/containerregistry/aio/_async_container_registry_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,21 +32,30 @@
 )
 from .._generated.models import AcrErrors
 from .._helpers import (
     _compute_digest,
     _is_tag,
     _parse_next_link,
     _validate_digest,
+    _get_blob_size,
+    _get_manifest_size,
     SUPPORTED_API_VERSIONS,
     OCI_IMAGE_MANIFEST,
     SUPPORTED_MANIFEST_MEDIA_TYPES,
     DEFAULT_AUDIENCE,
     DEFAULT_CHUNK_SIZE,
+    MAX_MANIFEST_SIZE,
+)
+from .._models import (
+    RepositoryProperties,
+    ArtifactManifestProperties,
+    ArtifactTagProperties,
+    GetManifestResult,
+    DigestValidationError,
 )
-from .._models import RepositoryProperties, ArtifactManifestProperties, ArtifactTagProperties, GetManifestResult
 
 JSON = MutableMapping[str, Any]
 
 
 class _UnclosableBytesIO(BytesIO):
     def close(self):
         pass
@@ -66,16 +75,15 @@
         **kwargs
     ) -> None:
         """Create a ContainerRegistryClient from an ACR endpoint and a credential.
 
         :param str endpoint: An ACR endpoint.
         :param credential: The credential with which to authenticate. This should be None in anonymous access.
         :type credential: ~azure.core.credentials_async.AsyncTokenCredential or None
-        :keyword api_version: API Version. The default value is "2021-07-01". Note that overriding this default value
-            may result in unsupported behavior.
+        :keyword api_version: API Version. The default value is "2021-07-01".
         :paramtype api_version: str
         :keyword audience: URL to use for credential authentication with AAD. Its value could be
             "https://management.azure.com", "https://management.chinacloudapi.cn" or
             "https://management.usgovcloudapi.net". The default value is "https://containerregistry.azure.net".
         :paramtype audience: str
         :returns: None
         :rtype: None
@@ -238,14 +246,15 @@
         return AsyncItemPaged(get_next, extract_data)
 
     @distributed_trace_async
     async def get_repository_properties(self, repository: str, **kwargs) -> RepositoryProperties:
         """Get the properties of a repository
 
         :param str repository: Name of the repository
+        :return: The properties of a repository.
         :rtype: ~azure.containerregistry.RepositoryProperties
         :raises: ~azure.core.exceptions.ResourceNotFoundError
         """
         return RepositoryProperties._from_generated(  # pylint: disable=protected-access
             await self._client.container_registry.get_properties(repository, **kwargs)
         )
 
@@ -395,14 +404,15 @@
     async def get_manifest_properties(
         self, repository: str, tag_or_digest: str, **kwargs
     ) -> ArtifactManifestProperties:
         """Get the properties of a registry artifact
 
         :param str repository: Name of the repository
         :param str tag_or_digest: The tag or digest of the manifest
+        :return: The properties of a registry artifact
         :rtype: ~azure.containerregistry.ArtifactManifestProperties
         :raises: ~azure.core.exceptions.ResourceNotFoundError
 
         Example
 
         .. code-block:: python
 
@@ -428,14 +438,15 @@
     @distributed_trace_async
     async def get_tag_properties(self, repository: str, tag: str, **kwargs) -> ArtifactTagProperties:
         """Get the properties for a tag
 
         :param str repository: Repository the tag belongs to
         :param tag: The tag to get properties for
         :type tag: str
+        :return: The properties for a tag.
         :rtype: ~azure.containerregistry.ArtifactTagProperties
         :raises: ~azure.core.exceptions.ResourceNotFoundError
 
         Example
 
         .. code-block:: python
 
@@ -890,16 +901,17 @@
         :paramtype tag: str or None
         :keyword media_type: The media type of the manifest. If not specified, this value will be set to
             a default value of "application/vnd.oci.image.manifest.v1+json". Note: the current known media types are:
             "application/vnd.oci.image.manifest.v1+json", and "application/vnd.docker.distribution.manifest.v2+json".
         :paramtype media_type: str
         :returns: The digest of the set manifest, calculated by the registry.
         :rtype: str
-        :raises ValueError: If the parameter repository or manifest is None,
-            or the digest in the response does not match the digest of the set manifest.
+        :raises ValueError: If the parameter repository or manifest is None.
+        :raises ~azure.containerregistry.DigestValidationError:
+            If the server-computed digest does not match the client-computed digest.
         """
         try:
             if isinstance(manifest, MutableMapping):
                 data = _UnclosableBytesIO(json.dumps(manifest).encode())
             else:
                 data = _UnclosableBytesIO(manifest.read())
             tag_or_digest = tag
@@ -912,15 +924,17 @@
                 payload=data,
                 content_type=media_type,
                 cls=_return_response_headers,
                 **kwargs
             )
             digest = response_headers['Docker-Content-Digest']
             if not _validate_digest(data, digest):
-                raise ValueError("The server-computed digest does not match the client-computed digest.")
+                raise DigestValidationError(
+                    "The server-computed digest does not match the client-computed digest."
+                )
         except Exception as e:
             if repository is None or manifest is None:
                 raise ValueError("The parameter repository and manifest cannot be None.") from e
             raise
         return digest
 
     @distributed_trace_async
@@ -929,50 +943,64 @@
 
         :param str repository: Name of the repository.
         :param str tag_or_digest: The tag or digest of the manifest to get.
             When digest is provided, will use this digest to compare with the one calculated by the response payload.
             When tag is provided, will use the digest in response headers to compare.
         :returns: GetManifestResult
         :rtype: ~azure.containerregistry.GetManifestResult
-        :raises ValueError: If the requested digest does not match the digest of the received manifest.
+        :raises ~azure.containerregistry.DigestValidationError:
+            If the content of retrieved manifest digest does not match the requested digest, or
+            the server-computed digest does not match the client-computed digest when tag is passing.
+        :raises ValueError: If the content-length header is missing or invalid in response, or the manifest size is
+            bigger than 4MB.
         """
         response = cast(
             PipelineResponse,
             await self._client.container_registry.get_manifest(
                 name=repository,
                 reference=tag_or_digest,
                 accept=SUPPORTED_MANIFEST_MEDIA_TYPES,
                 cls=_return_response,
                 **kwargs
             )
         )
+        manifest_size = _get_manifest_size(response.http_response.headers)
+        # This check is to address part of the service threat model. If a manifest does not have a proper
+        # content length or is too big, it indicates a malicious or faulty service and should not be trusted.
+        if manifest_size > MAX_MANIFEST_SIZE:
+            raise ValueError("Manifest size is bigger than max allowed size of 4MB.")
         media_type = response.http_response.headers['Content-Type']
         manifest_bytes = await response.http_response.read()
         manifest_json = response.http_response.json()
+        manifest_digest = _compute_digest(manifest_bytes)
         if tag_or_digest.startswith("sha256:"):
-            digest = tag_or_digest
-            if not _validate_digest(manifest_bytes, digest):
-                raise ValueError("The requested digest does not match the digest of the received manifest.")
-        else:
-            digest = response.http_response.headers['Docker-Content-Digest']
-            if not _validate_digest(manifest_bytes, digest):
-                raise ValueError("The server-computed digest does not match the client-computed digest.")
+            if manifest_digest != tag_or_digest:
+                raise DigestValidationError(
+                    "The content of retrieved manifest digest does not match the requested digest."
+                )
+        digest = response.http_response.headers['Docker-Content-Digest']
+        if manifest_digest != digest:
+            raise DigestValidationError(
+                "The server-computed digest does not match the client-computed digest."
+            )
 
         return GetManifestResult(digest=digest, manifest=manifest_json, media_type=media_type)
 
     @distributed_trace_async
     async def upload_blob(self, repository: str, data: IO[bytes], **kwargs) -> Tuple[str, int]:
         """Upload an artifact blob.
 
         :param str repository: Name of the repository.
         :param data: The blob to upload. Note: This must be a seekable stream.
         :type data: IO
         :returns: The digest and size in bytes of the uploaded blob.
         :rtype: Tuple[str, int]
         :raises ValueError: If the parameter repository or data is None.
+        :raises ~azure.containerregistry.DigestValidationError:
+            If the server-computed digest does not match the client-computed digest.
         """
         try:
             start_upload_response_headers = cast(
                 Dict[str, str],
                 await self._client.container_registry_blob.start_upload(
                     repository, cls=_return_response_headers, **kwargs
                 )
@@ -985,14 +1013,18 @@
                 await self._client.container_registry_blob.complete_upload(
                     digest=digest,
                     next_link=location,
                     cls=_return_response_headers,
                     **kwargs
                 )
             )
+            if digest != complete_upload_response_headers["Docker-Content-Digest"]:
+                raise DigestValidationError(
+                    "The server-computed digest does not match the client-computed digest."
+                )
         except Exception as e:
             if repository is None or data is None:
                 raise ValueError("The parameter repository and data cannot be None.") from e
             raise
         return complete_upload_response_headers['Docker-Content-Digest'], blob_size
 
     async def _upload_blob_chunk(self, location: str, data: IO[bytes], **kwargs) -> Tuple[str, str, int]:
@@ -1024,38 +1056,41 @@
     async def download_blob(self, repository: str, digest: str, **kwargs) -> AsyncDownloadBlobStream:
         """Download a blob that is part of an artifact to a stream.
 
         :param str repository: Name of the repository.
         :param str digest: The digest of the blob to download.
         :returns: AsyncDownloadBlobStream
         :rtype: ~azure.containerregistry.aio.AsyncDownloadBlobStream
-        :raises ValueError: If the requested digest does not match the digest of the received blob.
+        :raises DigestValidationError:
+            If the content of retrieved blob digest does not match the requested digest.
+        :raises ValueError: If the content-range header is missing or invalid in response.
         """
         end_range = DEFAULT_CHUNK_SIZE - 1
         first_chunk, headers = cast(
             Tuple[PipelineResponse, Dict[str, str]],
             await self._client.container_registry_blob.get_chunk(
                 repository,
                 digest,
                 range_header=f"bytes=0-{end_range}",
                 cls=_return_response_and_headers,
                 **kwargs
             )
         )
+        blob_size = _get_blob_size(headers)
         return AsyncDownloadBlobStream(
             response=first_chunk,
             digest=digest,
             get_next=functools.partial(
                 self._client.container_registry_blob.get_chunk,
                 name=repository,
                 digest=digest,
                 cls=_return_response_and_headers,
                 **kwargs
             ),
-            blob_size=int(headers["Content-Range"].split("/")[1]),
+            blob_size=blob_size,
             downloaded=int(headers["Content-Length"]),
             chunk_size=DEFAULT_CHUNK_SIZE
         )
 
     @distributed_trace_async
     async def delete_manifest(self, repository: str, tag_or_digest: str, **kwargs) -> None:
         """Delete a manifest. If the manifest cannot be found or a response status code of
```

## Comparing `azure-containerregistry-1.1.0b4/azure/containerregistry/aio/_async_authentication_policy.py` & `azure-containerregistry-1.2.0/azure/containerregistry/aio/_async_authentication_policy.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,23 +27,27 @@
         else:
             self._exchange_client = ACRExchangeClient(endpoint, self._credential, **kwargs)
 
     async def on_request(self, request: PipelineRequest) -> None:
         """Called before the policy sends a request.
         The base implementation authorizes the request with a bearer token.
 
-        :param ~azure.core.pipeline.PipelineRequest request: the request
+        :param ~azure.core.pipeline.PipelineRequest request: The pipeline request object.
+        :return: None
+        :rtype: None
         """
         # Future caching implementation will be included here
         pass  # pylint: disable=unnecessary-pass
 
     async def send(self, request: PipelineRequest) -> PipelineResponse:
         """Authorizes a request with a bearer token, possibly handling an authentication challenge
 
-        :param ~azure.core.pipeline.PipelineRequest request: the request
+        :param ~azure.core.pipeline.PipelineRequest request: The pipeline request object.
+        :return: The pipeline response object.
+        :rtype: ~azure.core.pipeline.PipelineResponse
         """
         _enforce_https(request)
 
         await self.on_request(request)
 
         response = await self.next.send(request)
 
@@ -66,16 +70,17 @@
         """Authorize request according to an authentication challenge
         This method is called when the resource provider responds 401 with a WWW-Authenticate header.
 
         :param ~azure.core.pipeline.PipelineRequest request: the request which elicited an authentication challenge
         :param ~azure.core.pipeline.PipelineResponse response: the resource provider's response
         :param str challenge: response's WWW-Authenticate header, unparsed. It may contain multiple challenges.
         :returns: a bool indicating whether the policy should send the request
+        :rtype: bool
         """
-        # pylint:disable=unused-argument,no-self-use
+        # pylint:disable=unused-argument
 
         access_token = await self._exchange_client.get_acr_access_token(challenge)
         if access_token is not None:
             request.http_request.headers["Authorization"] = "Bearer " + access_token
         return access_token is not None
 
     async def __aenter__(self):
```

## Comparing `azure-containerregistry-1.1.0b4/azure/containerregistry/aio/_async_anonymous_exchange_client.py` & `azure-containerregistry-1.2.0/azure/containerregistry/aio/_async_exchange_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,89 @@
 # coding=utf-8
 # ------------------------------------
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 # ------------------------------------
-from typing import Optional, Union
-from azure.core.credentials import AccessToken
+import time
+from typing import Optional
+
 from azure.core.credentials_async import AsyncTokenCredential
-from ._async_exchange_client import ExchangeClientAuthenticationPolicy
+from azure.core.pipeline import PipelineRequest, PipelineResponse
+from azure.core.pipeline.policies import SansIOHTTPPolicy
+
 from .._generated.aio import ContainerRegistry
-from .._generated.models import TokenGrantType
-from .._helpers import _parse_challenge
+from .._generated.models import PostContentSchemaGrantType
+from .._helpers import _parse_challenge, _parse_exp_time
 from .._user_agent import USER_AGENT
 
 
-class AsyncAnonymousAccessCredential(AsyncTokenCredential):
-    async def get_token(
-        self, *scopes: str, claims: Optional[str] = None, tenant_id: Optional[str] = None, **kwargs
-    ) -> AccessToken:
-        raise ValueError("This credential cannot be used to obtain access tokens.")
-
-    async def close(self) -> None:
-        pass
+class ExchangeClientAuthenticationPolicy(SansIOHTTPPolicy):
+    """Authentication policy for exchange client that does not modify the request"""
 
-    async def __aenter__(self):
+    def on_request(self, request: PipelineRequest) -> None:
         pass
 
-    async def __aexit__(self, exc_type, exc_value, traceback) -> None:
+    def on_response(self, request: PipelineRequest, response: PipelineResponse) -> None:
         pass
 
 
-class AnonymousACRExchangeClient(object):
+class ACRExchangeClient(object):
     """Class for handling oauth authentication requests
 
     :param endpoint: Azure Container Registry endpoint
     :type endpoint: str
-    :keyword api_version: Api Version. Default value is "2021-07-01". Note that overriding this
-        default value may result in unsupported behavior.
+    :param credential: Credential which provides tokens to authenticate requests
+    :type credential: ~azure.core.credentials.TokenCredential
+    :keyword api_version: Api Version. Default value is "2021-07-01".
     :paramtype api_version: str
+    :keyword credential_scopes: The scopes that access token can request.
+    :paramtype credential_scopes: list[str]
     """
 
-    def __init__(self, endpoint: str, **kwargs) -> None: # pylint: disable=missing-client-constructor-parameter-credential
+    def __init__(self, endpoint: str, credential: AsyncTokenCredential, **kwargs) -> None:
         if not endpoint.startswith("https://") and not endpoint.startswith("http://"):
             endpoint = "https://" + endpoint
         self._endpoint = endpoint
+        self.credential_scopes = kwargs.get("credential_scopes", ["https://management.core.windows.net/.default"])
         self._client = ContainerRegistry(
-            credential=AsyncAnonymousAccessCredential(),
+            credential=credential,
             url=endpoint,
             sdk_moniker=USER_AGENT,
             authentication_policy=ExchangeClientAuthenticationPolicy(),
             **kwargs
         )
+        self._credential = credential
+        self._refresh_token = None # type: Optional[str]
+        self._expiration_time = 0 # type: float
 
-    async def get_acr_access_token(self, challenge: str, **kwargs) -> Optional[str]:
+    async def get_acr_access_token(self, challenge: str, **kwargs) -> Optional[str]: # pylint:disable=client-method-missing-tracing-decorator-async
         parsed_challenge = _parse_challenge(challenge)
+        refresh_token = await self.get_refresh_token(parsed_challenge["service"], **kwargs)
         return await self.exchange_refresh_token_for_access_token(
-            "",
-            service=parsed_challenge["service"],
-            scope=parsed_challenge["scope"],
-            grant_type=TokenGrantType.PASSWORD,
-            **kwargs
+            refresh_token, service=parsed_challenge["service"], scope=parsed_challenge["scope"], **kwargs
+        )
+
+    async def get_refresh_token(self, service: str, **kwargs) -> str: # pylint:disable=client-method-missing-tracing-decorator-async
+        if not self._refresh_token or self._expiration_time - time.time() > 300:
+            self._refresh_token = await self.exchange_aad_token_for_refresh_token(service, **kwargs)
+            self._expiration_time = _parse_exp_time(self._refresh_token)
+        return self._refresh_token
+
+    async def exchange_aad_token_for_refresh_token(self, service: str, **kwargs) -> str: # pylint:disable=client-method-missing-tracing-decorator-async
+        token = await self._credential.get_token(*self.credential_scopes)
+        refresh_token = await self._client.authentication.exchange_aad_access_token_for_acr_refresh_token( # type: ignore # pylint: disable=line-too-long
+            grant_type=PostContentSchemaGrantType.ACCESS_TOKEN, service=service, access_token=token.token, **kwargs
         )
+        return refresh_token.refresh_token if refresh_token.refresh_token is not None else ""
 
-    async def exchange_refresh_token_for_access_token(
-        self, refresh_token: str, service: str, scope: str, grant_type: Union[str, TokenGrantType], **kwargs
+    async def exchange_refresh_token_for_access_token( # pylint:disable=client-method-missing-tracing-decorator-async
+        self, refresh_token: str, service: str, scope: str, **kwargs
     ) -> Optional[str]:
-        access_token = await self._client.authentication.exchange_acr_refresh_token_for_acr_access_token( # type: ignore
-            service=service, scope=scope, refresh_token=refresh_token, grant_type=grant_type, **kwargs
+        access_token = await self._client.authentication.exchange_acr_refresh_token_for_acr_access_token(# type: ignore
+            service, scope, refresh_token, **kwargs
         )
         return access_token.access_token
 
     async def __aenter__(self):
         await self._client.__aenter__()
         return self
```

## Comparing `azure-containerregistry-1.1.0b4/azure/containerregistry/aio/__init__.py` & `azure-containerregistry-1.2.0/azure/containerregistry/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b4/azure/containerregistry/aio/_async_download_stream.py` & `azure-containerregistry-1.2.0/azure/containerregistry/aio/_async_download_stream.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 # ------------------------------------
 import hashlib
 from typing import AsyncIterator, AsyncContextManager, Awaitable, cast, Tuple, Dict, Any
 from typing_extensions import Protocol, Self
 from azure.core.pipeline import PipelineResponse
+from .._models import DigestValidationError
 
 
 class AsyncGetNext(Protocol):
     def __call__(self, *args: Any, range_header: str) -> Awaitable[AsyncIterator[bytes]]:
         pass
 
 
@@ -62,19 +63,21 @@
         )
         self._downloaded += int(headers["Content-Length"])
         return next_chunk
 
     async def __anext__(self) -> bytes:
         try:
             return await self._yield_data()
-        except StopAsyncIteration:
+        except StopAsyncIteration as exc:
             if self._downloaded >= self._blob_size:
                 computed_digest = "sha256:" + self._hasher.hexdigest()
                 if computed_digest != self._digest:
-                    raise ValueError("The requested digest does not match the digest of the received blob.")
+                    raise DigestValidationError(
+                        "The content of retrieved blob digest does not match the requested digest."
+                    ) from exc
                 raise
             self._response = await self._download_chunk()
             self._response_bytes = self._response.http_response.iter_bytes()
             return await self._yield_data()
 
     async def close(self):
         await self._response.http_response.close()
```

## Comparing `azure-containerregistry-1.1.0b4/azure/containerregistry/aio/_async_base_client.py` & `azure-containerregistry-1.2.0/azure/containerregistry/aio/_async_base_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,17 +25,16 @@
     """Base class for ContainerRegistryClient
 
     :param endpoint: Azure Container Registry endpoint
     :type endpoint: str
     :param credential: Token credential for authenticating requests with Azure, or None in anonymous access
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential or None
     :keyword credential_scopes: URL for credential authentication if different from the default
-    :paramtype credential_scopes: List[str]
-    :keyword api_version: Api Version. Default value is "2021-07-01". Note that overriding this
-        default value may result in unsupported behavior.
+    :paramtype credential_scopes: list[str]
+    :keyword api_version: Api Version. Default value is "2021-07-01".
     :paramtype api_version: str
     """
 
     def __init__(self, endpoint: str, credential: Optional[AsyncTokenCredential], **kwargs) -> None:
         self._auth_policy = ContainerRegistryChallengePolicy(credential, endpoint, **kwargs)
         self._client = ContainerRegistry(
             credential=credential or AsyncAnonymousAccessCredential(),
@@ -56,15 +55,15 @@
 
     async def close(self) -> None:
         """Close sockets opened by the client.
         Calling this method is unnecessary when using the client as a context manager.
         """
         await self._client.close()
 
-    def _is_tag(self, tag_or_digest: str) -> bool:  # pylint: disable=no-self-use
+    def _is_tag(self, tag_or_digest: str) -> bool:
         tag = tag_or_digest.split(":")
         return not (len(tag) == 2 and tag[0].startswith("sha"))
 
 
 class AsyncTransportWrapper(AsyncHttpTransport):
     """Wrapper class that ensures that an inner client created
     by a `get_client` method does not close the outer transport for the parent
```

## Comparing `azure-containerregistry-1.1.0b4/samples/sample_set_image_properties.py` & `azure-containerregistry-1.2.0/samples/sample_set_image_properties.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,54 +13,53 @@
     This sample demonstrates setting an image's properties on the tag so it can't be overwritten during a lengthy
     deployment.
 
 USAGE:
     python sample_set_image_properties.py
 
     Set the environment variables with your own values before running the sample:
-    1) CONTAINERREGISTRY_ENDPOINT - The URL of you Container Registry account
+    1) CONTAINERREGISTRY_ENDPOINT - The URL of your Container Registry account
     
     This sample assumes your registry has a repository "library/hello-world" with image tagged "v1",
     run load_registry() if you don't have.
     Set the environment variables with your own values before running load_registry():
-    1) CONTAINERREGISTRY_ENDPOINT - The URL of you Container Registry account
+    1) CONTAINERREGISTRY_ENDPOINT - The URL of your Container Registry account
     2) CONTAINERREGISTRY_TENANT_ID - The service principal's tenant ID
     3) CONTAINERREGISTRY_CLIENT_ID - The service principal's client ID
     4) CONTAINERREGISTRY_CLIENT_SECRET - The service principal's client secret
-    5) CONTAINERREGISTRY_RESOURCE_GROUP - The resource group name
-    6) CONTAINERREGISTRY_REGISTRY_NAME - The registry name
 """
 import os
 from dotenv import find_dotenv, load_dotenv
 from azure.containerregistry import ContainerRegistryClient
-from utilities import load_registry, get_authority, get_audience, get_credential
+from utilities import load_registry, get_authority, get_credential
 
 
 class SetImageProperties(object):
     def __init__(self):
         load_dotenv(find_dotenv())
         self.endpoint = os.environ.get("CONTAINERREGISTRY_ENDPOINT")
         self.authority = get_authority(self.endpoint)
-        self.audience = get_audience(self.authority)
         self.credential = get_credential(self.authority)
 
     def set_image_properties(self):
-        load_registry()
-        # Instantiate an instance of ContainerRegistryClient
-        with ContainerRegistryClient(self.endpoint, self.credential, audience=self.audience) as client:
-            # Set permissions on the v1 image's "latest" tag
+        load_registry(self.endpoint)
+        # [START update_manifest_properties]
+        with ContainerRegistryClient(self.endpoint, self.credential) as client:
+            # Set permissions on image "library/hello-world:v1"
             client.update_manifest_properties(
                 "library/hello-world",
                 "v1",
                 can_write=False,
                 can_delete=False
             )
-            # After this update, if someone were to push an update to `<registry endpoint>\library\hello-world:v1`,
-            # it would fail. It's worth noting that if this image also had another tag, such as `latest`,
-            # and that tag did not have permissions set to prevent reads or deletes, the image could still be
-            # overwritten. For example, if someone were to push an update to `<registry endpoint>\hello-world:latest`
-            # (which references the same image), it would succeed.
+        # [END update_manifest_properties]
+        
+        # After this update, if someone were to push an update to `<registry endpoint>\library\hello-world:v1`,
+        # it would fail. It's worth noting that if this image also had another tag, such as `latest`,
+        # and that tag did not have permissions set to prevent reads or deletes, the image could still be
+        # overwritten. For example, if someone were to push an update to `<registry endpoint>\hello-world:latest`
+        # (which references the same image), it would succeed.
 
 
 if __name__ == "__main__":
     sample = SetImageProperties()
     sample.set_image_properties()
```

## Comparing `azure-containerregistry-1.1.0b4/samples/sample_delete_images_async.py` & `azure-containerregistry-1.2.0/samples/sample_delete_images_async.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,49 +12,44 @@
 DESCRIPTION:
     This sample demonstrates deleting all but the most recent three images for each repository.
 
 USAGE:
     python sample_delete_images_async.py
 
     Set the environment variables with your own values before running the sample:
-    1) CONTAINERREGISTRY_ENDPOINT - The URL of you Container Registry account
+    1) CONTAINERREGISTRY_ENDPOINT - The URL of your Container Registry account
 
     This sample assumes your registry has at least one repository with more than three images,
     run load_registry() if you don't have.
     Set the environment variables with your own values before running load_registry():
-    1) CONTAINERREGISTRY_ENDPOINT - The URL of you Container Registry account
+    1) CONTAINERREGISTRY_ENDPOINT - The URL of your Container Registry account
     2) CONTAINERREGISTRY_TENANT_ID - The service principal's tenant ID
     3) CONTAINERREGISTRY_CLIENT_ID - The service principal's client ID
     4) CONTAINERREGISTRY_CLIENT_SECRET - The service principal's client secret
-    5) CONTAINERREGISTRY_RESOURCE_GROUP - The resource group name
-    6) CONTAINERREGISTRY_REGISTRY_NAME - The registry name
 """
 import asyncio
 import os
 from dotenv import find_dotenv, load_dotenv
 from azure.containerregistry import ArtifactManifestOrder
 from azure.containerregistry.aio import ContainerRegistryClient
-from utilities import load_registry, get_authority, get_audience, get_credential
+from utilities import load_registry, get_authority, get_credential
 
 
 class DeleteImagesAsync(object):
     def __init__(self):
         load_dotenv(find_dotenv())
         self.endpoint = os.environ.get("CONTAINERREGISTRY_ENDPOINT")
         self.authority = get_authority(self.endpoint)
-        self.audience = get_audience(self.authority)
         self.credential = get_credential(self.authority, is_async=True)
 
     async def delete_images(self):
-        load_registry()
+        load_registry(self.endpoint)
         # Instantiate an instance of ContainerRegistryClient
-        async with ContainerRegistryClient(self.endpoint, self.credential, audience=self.audience) as client:
+        async with ContainerRegistryClient(self.endpoint, self.credential) as client:
             async for repository in client.list_repository_names():
-                print(repository)
-
                 # Keep the three most recent images, delete everything else
                 manifest_count = 0
                 async for manifest in client.list_manifest_properties(
                     repository, order_by=ArtifactManifestOrder.LAST_UPDATED_ON_DESCENDING
                 ):
                     manifest_count += 1
                     if manifest_count > 3:
```

## Comparing `azure-containerregistry-1.1.0b4/samples/sample_list_tags.py` & `azure-containerregistry-1.2.0/samples/sample_list_tags.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,47 +14,43 @@
     Anonymous access allows a user to list all the collections there, but they wouldn't have permissions to
     modify or delete any of the images in the registry.
 
 USAGE:
     python sample_list_tags.py
 
     Set the environment variables with your own values before running the sample:
-    1) CONTAINERREGISTRY_ENDPOINT - The URL of you Container Registry account
+    1) CONTAINERREGISTRY_ANONREGISTRY_ENDPOINT - The URL of your Container Registry account for anonymous access
 
     This sample assumes your registry has a repository "library/hello-world" with image tagged "latest",
     run load_registry() if you don't have.
     Set the environment variables with your own values before running load_registry():
-    1) CONTAINERREGISTRY_ENDPOINT - The URL of you Container Registry account
+    1) CONTAINERREGISTRY_ANONREGISTRY_ENDPOINT - The URL of your Container Registry account for anonymous access
     2) CONTAINERREGISTRY_TENANT_ID - The service principal's tenant ID
     3) CONTAINERREGISTRY_CLIENT_ID - The service principal's client ID
     4) CONTAINERREGISTRY_CLIENT_SECRET - The service principal's client secret
-    5) CONTAINERREGISTRY_RESOURCE_GROUP - The resource group name
-    6) CONTAINERREGISTRY_REGISTRY_NAME - The registry name
 """
 import os
 from dotenv import find_dotenv, load_dotenv
 from azure.containerregistry import ContainerRegistryClient
-from utilities import load_registry, get_authority, get_audience, get_credential
+from utilities import load_registry
 
 
 class ListTags(object):
     def __init__(self):
         load_dotenv(find_dotenv())
-        self.endpoint = os.environ.get("CONTAINERREGISTRY_ENDPOINT")
-        self.authority = get_authority(self.endpoint)
-        self.audience = get_audience(self.authority)
-        self.credential = get_credential(self.authority)
 
     def list_tags(self):
-        load_registry()
-        # Instantiate an instance of ContainerRegistryClient
-        with ContainerRegistryClient(self.endpoint, self.credential, audience=self.audience) as client:
-            manifest = client.get_manifest_properties("library/hello-world", "latest")
-            print("Tags of " + manifest.repository_name + ": ")
+        endpoint = os.environ.get("CONTAINERREGISTRY_ANONREGISTRY_ENDPOINT")
+        load_registry(endpoint)
+        # [START list_tags_anonymous]
+        with ContainerRegistryClient(endpoint) as anon_client:
+            manifest = anon_client.get_manifest_properties("library/hello-world", "latest")
+            print(f"Tags of {manifest.repository_name}: ")
             # Iterate through all the tags
             for tag in manifest.tags:
                 print(tag)
+        # [END list_tags_anonymous]
 
 
 if __name__ == "__main__":
     sample = ListTags()
     sample.list_tags()
```

## Comparing `azure-containerregistry-1.1.0b4/samples/sample_list_tags_async.py` & `azure-containerregistry-1.2.0/samples/sample_set_image_properties_async.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,63 +3,66 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 
 """
-FILE: sample_list_tags_async.py
+FILE: sample_set_image_properties_async.py
 
 DESCRIPTION:
-    This sample demonstrates listing the tags for an image in a repository with anonymous pull access.
-    Anonymous access allows a user to list all the collections there, but they wouldn't have permissions to
-    modify or delete any of the images in the registry.
+    This sample demonstrates setting an image's properties on the tag so it can't be overwritten during a lengthy
+    deployment.
 
 USAGE:
-    python sample_list_tags_async.py
+    python sample_set_image_properties_async.py
 
     Set the environment variables with your own values before running the sample:
-    1) CONTAINERREGISTRY_ENDPOINT - The URL of you Container Registry account
+    1) CONTAINERREGISTRY_ENDPOINT - The URL of your Container Registry account
 
-    This sample assumes your registry has a repository "library/hello-world" with image tagged "latest",
+    This sample assumes your registry has a repository "library/hello-world" with image tagged "v1",
     run load_registry() if you don't have.
     Set the environment variables with your own values before running load_registry():
-    1) CONTAINERREGISTRY_ENDPOINT - The URL of you Container Registry account
+    1) CONTAINERREGISTRY_ENDPOINT - The URL of your Container Registry account
     2) CONTAINERREGISTRY_TENANT_ID - The service principal's tenant ID
     3) CONTAINERREGISTRY_CLIENT_ID - The service principal's client ID
     4) CONTAINERREGISTRY_CLIENT_SECRET - The service principal's client secret
-    5) CONTAINERREGISTRY_RESOURCE_GROUP - The resource group name
-    6) CONTAINERREGISTRY_REGISTRY_NAME - The registry name
 """
 import asyncio
 import os
 from dotenv import find_dotenv, load_dotenv
 from azure.containerregistry.aio import ContainerRegistryClient
-from utilities import load_registry, get_authority, get_audience, get_credential
+from utilities import load_registry, get_authority, get_credential
 
 
-class ListTagsAsync(object):
+class SetImagePropertiesAsync(object):
     def __init__(self):
         load_dotenv(find_dotenv())
         self.endpoint = os.environ.get("CONTAINERREGISTRY_ENDPOINT")
         self.authority = get_authority(self.endpoint)
-        self.audience = get_audience(self.authority)
         self.credential = get_credential(self.authority, is_async=True)
 
-    async def list_tags(self):
-        load_registry()
-        # Instantiate an instance of ContainerRegistryClient    
-        async with ContainerRegistryClient(self.endpoint, self.credential, audience=self.audience) as client:
-            manifest = await client.get_manifest_properties("library/hello-world", "latest")
-            print("Tags of " + manifest.repository_name + ": ")
-            # Iterate through all the tags
-            for tag in manifest.tags:
-                print(tag)
+    async def set_image_properties(self):
+        load_registry(self.endpoint)
+        # Instantiate an instance of ContainerRegistryClient
+        async with ContainerRegistryClient(self.endpoint, self.credential) as client:
+            # Set permissions on image "library/hello-world:v1"
+            await client.update_manifest_properties(
+                "library/hello-world",
+                "v1",
+                can_write=False,
+                can_delete=False
+            )        
+        # After this update, if someone were to push an update to `<registry endpoint>\library\hello-world:v1`,
+        # it would fail. It's worth noting that if this image also had another tag, such as `latest`,
+        # and that tag did not have permissions set to prevent reads or deletes, the image could still be
+        # overwritten. For example, if someone were to push an update to `<registry endpoint>\hello-world:latest`
+        # (which references the same image), it would succeed.
 
 
 async def main():
-    sample = ListTagsAsync()
-    await sample.list_tags()
+    sample = SetImagePropertiesAsync()
+    await sample.set_image_properties()
 
 
 if __name__ == "__main__":
     asyncio.run(main())
```

## Comparing `azure-containerregistry-1.1.0b4/samples/sample_hello_world.py` & `azure-containerregistry-1.2.0/samples/sample_hello_world.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,44 +13,41 @@
     This sample demonstrate creating a ContainerRegistryClient and iterating
     through the collection of tags in the repository with anonymous access.
 
 USAGE:
     python sample_hello_world.py
 
     Set the environment variables with your own values before running the sample:
-    1) CONTAINERREGISTRY_ENDPOINT - The URL of you Container Registry account
+    1) CONTAINERREGISTRY_ENDPOINT - The URL of your Container Registry account
 
     This sample assumes your registry has a repository "library/hello-world", run load_registry() if you don't have.
     Set the environment variables with your own values before running load_registry():
-    1) CONTAINERREGISTRY_ENDPOINT - The URL of you Container Registry account
+    1) CONTAINERREGISTRY_ENDPOINT - The URL of your Container Registry account
     2) CONTAINERREGISTRY_TENANT_ID - The service principal's tenant ID
     3) CONTAINERREGISTRY_CLIENT_ID - The service principal's client ID
     4) CONTAINERREGISTRY_CLIENT_SECRET - The service principal's client secret
-    5) CONTAINERREGISTRY_RESOURCE_GROUP - The resource group name
-    6) CONTAINERREGISTRY_REGISTRY_NAME - The registry name
 """
 import os
 from dotenv import find_dotenv, load_dotenv
 from azure.containerregistry import ContainerRegistryClient
-from utilities import load_registry, get_authority, get_audience, get_credential
+from utilities import load_registry, get_authority, get_credential
 
 
 class HelloWorld(object):
     def __init__(self):
         load_dotenv(find_dotenv())
         self.endpoint = os.environ.get("CONTAINERREGISTRY_ENDPOINT")
         self.authority = get_authority(self.endpoint)
-        self.audience = get_audience(self.authority)
         self.credential = get_credential(self.authority)
 
     def basic_sample(self):
-        load_registry()
+        load_registry(self.endpoint)
         # Instantiate an instance of ContainerRegistryClient
         # [START create_registry_client]
-        with ContainerRegistryClient(self.endpoint, self.credential, audience=self.audience) as client:
+        with ContainerRegistryClient(self.endpoint, self.credential) as client:
         # [END create_registry_client]
             # Iterate through all the repositories
             for repository_name in client.list_repository_names():
                 print(repository_name)
                 if repository_name == "library/hello-world":
                     print("Tags of repository library/hello-world:")
                     for tag in client.list_tag_properties(repository_name):
```

## Comparing `azure-containerregistry-1.1.0b4/samples/sample_set_get_image.py` & `azure-containerregistry-1.2.0/samples/sample_set_get_image_async.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,62 +3,56 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 
 """
-FILE: sample_set_get_image.py
+FILE: sample_set_get_image_async.py
 
 DESCRIPTION:
     This sample demonstrates setting and getting OCI and non-OCI images to a repository.
 
 USAGE:
-    python sample_set_get_image.py
+    python sample_set_get_image_async.py
 
     Set the environment variables with your own values before running the sample:
-    1) CONTAINERREGISTRY_ENDPOINT - The URL of you Container Registry account
-
-    This sample assumes your registry has a repository "library/hello-world", run load_registry() if you don't have.
-    Set the environment variables with your own values before running load_registry():
-    1) CONTAINERREGISTRY_ENDPOINT - The URL of you Container Registry account
-    2) CONTAINERREGISTRY_TENANT_ID - The service principal's tenant ID
-    3) CONTAINERREGISTRY_CLIENT_ID - The service principal's client ID
-    4) CONTAINERREGISTRY_CLIENT_SECRET - The service principal's client secret
-    5) CONTAINERREGISTRY_RESOURCE_GROUP - The resource group name
-    6) CONTAINERREGISTRY_REGISTRY_NAME - The registry name
+    1) CONTAINERREGISTRY_ANONREGISTRY_ENDPOINT - The URL of your Container Registry account for anonymous access
 """
+import asyncio
 import os
 import json
 from io import BytesIO
 from dotenv import find_dotenv, load_dotenv
-from azure.containerregistry import ContainerRegistryClient, ArtifactArchitecture, ArtifactOperatingSystem
-from utilities import load_registry, get_authority, get_audience, get_credential
+from azure.containerregistry import DigestValidationError
+from azure.containerregistry.aio import ContainerRegistryClient
+from utilities import get_authority, get_credential
 
 
-class SetGetImage(object):
+class SetGetImageAsync(object):
     def __init__(self):
         load_dotenv(find_dotenv())
-        self.endpoint = os.environ.get("CONTAINERREGISTRY_ENDPOINT")
+        self.endpoint = os.environ.get("CONTAINERREGISTRY_ANONREGISTRY_ENDPOINT")
         self.authority = get_authority(self.endpoint)
-        self.audience = get_audience(self.authority)
-        self.credential = get_credential(self.authority)
+        self.credential = get_credential(self.authority, is_async=True)
 
-    def set_get_oci_image(self):
-        repository_name = "sample-oci-image"
+    async def set_get_oci_image(self):
+        repository_name = "sample-oci-image-async"
         layer = BytesIO(b"Sample layer")
         config = BytesIO(json.dumps(
             {
                 "sample config": "content",
             }).encode())
-        with ContainerRegistryClient(self.endpoint, self.credential, audience=self.audience) as client:
+        async with ContainerRegistryClient(self.endpoint, self.credential) as client:
             # Upload a layer
-            layer_digest, layer_size = client.upload_blob(repository_name, layer)
+            layer_digest, layer_size = await client.upload_blob(repository_name, layer)
+            print(f"Uploaded layer: digest - {layer_digest}, size - {layer_size}")
             # Upload a config
-            config_digest, config_size = client.upload_blob(repository_name, config)
+            config_digest, config_size = await client.upload_blob(repository_name, config)
+            print(f"Uploaded config: digest - {config_digest}, size - {config_size}")
             # Create an oci image with config and layer info
             oci_manifest = {
                 "config": {
                     "mediaType": "application/vnd.oci.image.config.v1+json",
                     "digest": config_digest,
                     "sizeInBytes": config_size,
                 },
@@ -70,79 +64,103 @@
                         "size": layer_size,
                         "annotations": {
                             "org.opencontainers.image.ref.name": "artifact.txt",
                         },
                     },
                 ],
             }
+
             # Set the image
-            manifest_digest = client.set_manifest(repository_name, oci_manifest)
+            manifest_digest = await client.set_manifest(repository_name, oci_manifest, tag="latest")
+            print(f"Uploaded manifest: digest - {manifest_digest}")
+            # [END upload_blob_and_manifest]
 
+            # [START download_blob_and_manifest]
             # Get the image
-            get_manifest_result = client.get_manifest(repository_name, manifest_digest)
+            get_manifest_result = await client.get_manifest(repository_name, "latest")
             received_manifest = get_manifest_result.manifest
-            print(received_manifest)
+            print(f"Got manifest:\n{received_manifest}")
+
             # Download and write out the layers
             for layer in received_manifest["layers"]:
                 # Remove the "sha256:" prefix from digest
                 layer_file_name = layer["digest"].split(":")[1]
                 try:
-                    stream = client.download_blob(repository_name, layer["digest"])
+                    stream = await client.download_blob(repository_name, layer["digest"])
                     with open(layer_file_name, "wb") as layer_file:
-                        for chunk in stream:
+                        async for chunk in stream:
                             layer_file.write(chunk)
-                except ValueError:
+                except DigestValidationError:
                     print(f"Downloaded layer digest value did not match. Deleting file {layer_file_name}.")
                     os.remove(layer_file_name)
+                print(f"Got layer: {layer_file_name}")
             # Download and write out the config
             config_file_name = "config.json"
             try:
-                stream = client.download_blob(repository_name, received_manifest["config"]["digest"])
+                stream = await client.download_blob(repository_name, received_manifest["config"]["digest"])
                 with open(config_file_name, "wb") as config_file:
-                    for chunk in stream:
+                    async for chunk in stream:
                         config_file.write(chunk)
-            except ValueError:
+            except DigestValidationError:
                 print(f"Downloaded config digest value did not match. Deleting file {config_file_name}.")
                 os.remove(config_file_name)
+            print(f"Got config: {config_file_name}")
 
             # Delete the layers
             for layer in received_manifest["layers"]:
-                client.delete_blob(repository_name, layer["digest"])
+                await client.delete_blob(repository_name, layer["digest"])
             # Delete the config
-            client.delete_blob(repository_name, received_manifest["config"]["digest"])
+            await client.delete_blob(repository_name, received_manifest["config"]["digest"])
+            
             # Delete the image
-            client.delete_manifest(repository_name, manifest_digest)
+            await client.delete_manifest(repository_name, get_manifest_result.digest)
 
-    def set_get_docker_image(self):
-        load_registry()
-        repository_name = "library/hello-world"
-        # create a Docker image object in Docker v2 Manifest List format
-        manifest_list = {
-            "schemaVersion": 2,
-            "mediaType": "application/vnd.docker.distribution.manifest.list.v2+json",
-            "manifests": [
-                {
-                    "digest": "sha256:f54a58bc1aac5ea1a25d796ae155dc228b3f0e11d046ae276b39c4bf2f13d8c4",
-                    "mediaType": "application/vnd.docker.distribution.manifest.v2+json",
-                    "platform": {
-                        "architecture": ArtifactArchitecture.AMD64,
-                        "os": ArtifactOperatingSystem.LINUX
+    async def set_get_docker_image(self):
+        repository_name = "sample-docker-image"
+        async with ContainerRegistryClient(self.endpoint, self.credential) as client:
+            # Upload a layer
+            layer = BytesIO(b"Sample layer")
+            layer_digest, layer_size = await client.upload_blob(repository_name, layer)
+            print(f"Uploaded layer: digest - {layer_digest}, size - {layer_size}")
+            # Upload a config
+            config = BytesIO(json.dumps({"sample config": "content"}).encode())
+            config_digest, config_size = await client.upload_blob(repository_name, config)
+            print(f"Uploaded config: digest - {config_digest}, size - {config_size}")
+            # create a Docker image object in Docker v2 Manifest format
+            docker_manifest = {
+                "config": {
+                    "digest": config_digest,
+                    "mediaType": "application/vnd.docker.container.image.v1+json",
+                    "size": config_size
+                },
+                "layers": [
+                    {
+                        "digest": layer_digest,
+                        "mediaType": "application/vnd.docker.image.rootfs.diff.tar.gzip",
+                        "size": layer_size
                     }
-                }
-            ]
-        }
-        with ContainerRegistryClient(self.endpoint, self.credential, audience=self.audience) as client:
+                ],
+                "mediaType": "application/vnd.docker.distribution.manifest.v2+json",
+                "schemaVersion": 2
+            }
             # Set the image with one custom media type
-            client.set_manifest(repository_name, manifest_list, tag="sample", media_type=manifest_list["mediaType"])
+            await client.set_manifest(repository_name, docker_manifest, tag="sample", media_type=docker_manifest["mediaType"])
 
             # Get the image
-            get_manifest_result = client.get_manifest(repository_name, "sample")
+            get_manifest_result = await client.get_manifest(repository_name, "sample")
             received_manifest = get_manifest_result.manifest
             print(received_manifest)
             received_manifest_media_type = get_manifest_result.media_type
             print(received_manifest_media_type)
+            
+            # Delete the image
+            client.delete_manifest(repository_name, get_manifest_result.digest)
+
+
+async def main():
+    sample = SetGetImageAsync()
+    await sample.set_get_oci_image()
+    await sample.set_get_docker_image()
 
 
 if __name__ == "__main__":
-    sample = SetGetImage()
-    sample.set_get_oci_image()
-    sample.set_get_docker_image()
+    asyncio.run(main())
```

## Comparing `azure-containerregistry-1.1.0b4/samples/sample_delete_tags.py` & `azure-containerregistry-1.2.0/samples/sample_delete_tags.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,55 +12,53 @@
 DESCRIPTION:
     This sample demonstrates deleting all but the most recent three tags for each repository.
 
 USAGE:
     python sample_delete_tags.py
 
     Set the environment variables with your own values before running the sample:
-    1) CONTAINERREGISTRY_ENDPOINT - The URL of you Container Registry account
+    1) CONTAINERREGISTRY_ENDPOINT - The URL of your Container Registry account
 
     This sample assumes your registry has at least one repository with more than three tags,
     run load_registry() if you don't have.
     Set the environment variables with your own values before running load_registry():
-    1) CONTAINERREGISTRY_ENDPOINT - The URL of you Container Registry account
+    1) CONTAINERREGISTRY_ENDPOINT - The URL of your Container Registry account
     2) CONTAINERREGISTRY_TENANT_ID - The service principal's tenant ID
     3) CONTAINERREGISTRY_CLIENT_ID - The service principal's client ID
     4) CONTAINERREGISTRY_CLIENT_SECRET - The service principal's client secret
-    5) CONTAINERREGISTRY_RESOURCE_GROUP - The resource group name
-    6) CONTAINERREGISTRY_REGISTRY_NAME - The registry name
 """
 import os
 from dotenv import find_dotenv, load_dotenv
 from azure.containerregistry import ContainerRegistryClient, ArtifactTagOrder
-from utilities import load_registry, get_authority, get_audience, get_credential
+from utilities import load_registry, get_authority, get_credential
 
 
 class DeleteTags(object):
     def __init__(self):
         load_dotenv(find_dotenv())
         self.endpoint = os.environ.get("CONTAINERREGISTRY_ENDPOINT")
         self.authority = get_authority(self.endpoint)
-        self.audience = get_audience(self.authority)
         self.credential = get_credential(self.authority)
 
     def delete_tags(self):
-        load_registry()
-        with ContainerRegistryClient(self.endpoint, self.credential, audience=self.audience) as client:
-            # [START list_repository_names]
-            for repository in client.list_repository_names():
-                print(repository)
+        load_registry(self.endpoint)
+        # [START list_repository_names]
+        with ContainerRegistryClient(self.endpoint, self.credential) as client:
+            # Iterate through all the repositories
+            for repository_name in client.list_repository_names():
+                print(repository_name)
                 # [END list_repository_names]
 
                 # Keep the three most recent tags, delete everything else
                 tag_count = 0
                 for tag in client.list_tag_properties(
-                    repository, order_by=ArtifactTagOrder.LAST_UPDATED_ON_DESCENDING
+                    repository_name, order_by=ArtifactTagOrder.LAST_UPDATED_ON_DESCENDING
                 ):
                     tag_count += 1
                     if tag_count > 3:
-                        print(f"Deleting {repository}:{tag.name}")
-                        client.delete_tag(repository, tag.name)
+                        print(f"Deleting {repository_name}:{tag.name}")
+                        client.delete_tag(repository_name, tag.name)
 
 
 if __name__ == "__main__":
     sample = DeleteTags()
     sample.delete_tags()
```

## Comparing `azure-containerregistry-1.1.0b4/samples/sample_delete_images.py` & `azure-containerregistry-1.2.0/samples/sample_delete_images.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,47 +12,43 @@
 DESCRIPTION:
     This sample demonstrates deleting all but the most recent three images for each repository.
 
 USAGE:
     python sample_delete_images.py
 
     Set the environment variables with your own values before running the sample:
-    1) CONTAINERREGISTRY_ENDPOINT - The URL of you Container Registry account
+    1) CONTAINERREGISTRY_ENDPOINT - The URL of your Container Registry account
 
     This sample assumes your registry has at least one repository with more than three images,
     run load_registry() if you don't have.
     Set the environment variables with your own values before running load_registry():
-    1) CONTAINERREGISTRY_ENDPOINT - The URL of you Container Registry account
+    1) CONTAINERREGISTRY_ENDPOINT - The URL of your Container Registry account
     2) CONTAINERREGISTRY_TENANT_ID - The service principal's tenant ID
     3) CONTAINERREGISTRY_CLIENT_ID - The service principal's client ID
     4) CONTAINERREGISTRY_CLIENT_SECRET - The service principal's client secret
-    5) CONTAINERREGISTRY_RESOURCE_GROUP - The resource group name
-    6) CONTAINERREGISTRY_REGISTRY_NAME - The registry name
 """
 import os
 from dotenv import find_dotenv, load_dotenv
 from azure.containerregistry import ContainerRegistryClient, ArtifactManifestOrder
-from utilities import load_registry, get_authority, get_audience, get_credential
+from utilities import load_registry, get_authority, get_credential
 
 
 class DeleteImages(object):
     def __init__(self):
         load_dotenv(find_dotenv())
         self.endpoint = os.environ.get("CONTAINERREGISTRY_ENDPOINT")
         self.authority = get_authority(self.endpoint)
-        self.audience = get_audience(self.authority)
         self.credential = get_credential(self.authority)
 
     def delete_images(self):
-        load_registry()
+        load_registry(self.endpoint)
         # Instantiate an instance of ContainerRegistryClient
-        with ContainerRegistryClient(self.endpoint, self.credential, audience=self.audience) as client:
+        # [START delete_manifests]
+        with ContainerRegistryClient(self.endpoint, self.credential) as client:
             for repository in client.list_repository_names():
-                print(repository)
-
                 # Keep the three most recent images, delete everything else
                 manifest_count = 0
                 for manifest in client.list_manifest_properties(
                     repository, order_by=ArtifactManifestOrder.LAST_UPDATED_ON_DESCENDING
                 ):
                     manifest_count += 1
                     if manifest_count > 3:
@@ -61,12 +57,13 @@
                             repository,
                             manifest.digest,
                             can_write=True,
                             can_delete=True
                         )
                         print(f"Deleting {repository}:{manifest.digest}")
                         client.delete_manifest(repository, manifest.digest)
+        # [END delete_manifests]
 
 
 if __name__ == "__main__":
     sample = DeleteImages()
     sample.delete_images()
```

## Comparing `azure-containerregistry-1.1.0b4/samples/sample_hello_world_async.py` & `azure-containerregistry-1.2.0/samples/sample_hello_world_async.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,45 +13,42 @@
     This sample demonstrate creating a ContainerRegistryClient and iterating
     through the collection of tags in the repository with anonymous access.
 
 USAGE:
     python sample_hello_world_async.py
 
     Set the environment variables with your own values before running the sample:
-    1) CONTAINERREGISTRY_ENDPOINT - The URL of you Container Registry account
+    1) CONTAINERREGISTRY_ENDPOINT - The URL of your Container Registry account
 
     This sample assumes your registry has a repository "library/hello-world", run load_registry() if you don't have.
     Set the environment variables with your own values before running load_registry():
-    1) CONTAINERREGISTRY_ENDPOINT - The URL of you Container Registry account
+    1) CONTAINERREGISTRY_ENDPOINT - The URL of your Container Registry account
     2) CONTAINERREGISTRY_TENANT_ID - The service principal's tenant ID
     3) CONTAINERREGISTRY_CLIENT_ID - The service principal's client ID
     4) CONTAINERREGISTRY_CLIENT_SECRET - The service principal's client secret
-    5) CONTAINERREGISTRY_RESOURCE_GROUP - The resource group name
-    6) CONTAINERREGISTRY_REGISTRY_NAME - The registry name
 """
 import asyncio
 import os
 from dotenv import find_dotenv, load_dotenv
 from azure.containerregistry.aio import ContainerRegistryClient
-from utilities import load_registry, get_authority, get_audience, get_credential
+from utilities import load_registry, get_authority, get_credential
 
 
 class HelloWorldAsync(object):
     def __init__(self):
         load_dotenv(find_dotenv())
         self.endpoint = os.environ.get("CONTAINERREGISTRY_ENDPOINT")
         self.authority = get_authority(self.endpoint)
-        self.audience = get_audience(self.authority)
         self.credential = get_credential(self.authority, is_async=True)
 
     async def basic_sample(self):
-        load_registry()
+        load_registry(self.endpoint)
         # Instantiate an instance of ContainerRegistryClient
         # [START create_registry_client]
-        async with ContainerRegistryClient(self.endpoint, self.credential, audience=self.audience) as client:
+        async with ContainerRegistryClient(self.endpoint, self.credential) as client:
         # [END create_registry_client]
             # Iterate through all the repositories
             async for repository_name in client.list_repository_names():
                 print(repository_name)
                 if repository_name == "library/hello-world":
                     print("Tags of repository library/hello-world:")
                     async for tag in client.list_tag_properties(repository_name):
```

## Comparing `azure-containerregistry-1.1.0b4/samples/sample_delete_tags_async.py` & `azure-containerregistry-1.2.0/samples/sample_delete_tags_async.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,59 +12,57 @@
 DESCRIPTION:
     This sample demonstrates deleting all but the most recent three tags for each repository.
 
 USAGE:
     python sample_delete_tags_async.py
 
     Set the environment variables with your own values before running the sample:
-    1) CONTAINERREGISTRY_ENDPOINT - The URL of you Container Registry account
+    1) CONTAINERREGISTRY_ENDPOINT - The URL of your Container Registry account
 
     This sample assumes your registry has at least one repository with more than three tags,
     run load_registry() if you don't have.
     Set the environment variables with your own values before running load_registry():
-    1) CONTAINERREGISTRY_ENDPOINT - The URL of you Container Registry account
+    1) CONTAINERREGISTRY_ENDPOINT - The URL of your Container Registry account
     2) CONTAINERREGISTRY_TENANT_ID - The service principal's tenant ID
     3) CONTAINERREGISTRY_CLIENT_ID - The service principal's client ID
     4) CONTAINERREGISTRY_CLIENT_SECRET - The service principal's client secret
-    5) CONTAINERREGISTRY_RESOURCE_GROUP - The resource group name
-    6) CONTAINERREGISTRY_REGISTRY_NAME - The registry name
 """
 import asyncio
 import os
 from dotenv import find_dotenv, load_dotenv
 from azure.containerregistry import ArtifactTagOrder
 from azure.containerregistry.aio import ContainerRegistryClient
-from utilities import load_registry, get_authority, get_audience, get_credential
+from utilities import load_registry, get_authority, get_credential
 
 
 class DeleteTagsAsync(object):
     def __init__(self):
         load_dotenv(find_dotenv())
         self.endpoint = os.environ.get("CONTAINERREGISTRY_ENDPOINT")
         self.authority = get_authority(self.endpoint)
-        self.audience = get_audience(self.authority)
         self.credential = get_credential(self.authority, is_async=True)
 
     async def delete_tags(self):
-        load_registry()
-        async with ContainerRegistryClient(self.endpoint, self.credential, audience=self.audience) as client:
-            # [START list_repository_names]
-            async for repository in client.list_repository_names():
-                print(repository)
+        load_registry(self.endpoint)
+        # [START list_repository_names]
+        async with ContainerRegistryClient(self.endpoint, self.credential) as client:
+            # Iterate through all the repositories
+            async for repository_name in client.list_repository_names():
+                print(repository_name)
                 # [END list_repository_names]
 
                 # Keep the three most recent tags, delete everything else
                 tag_count = 0
                 async for tag in client.list_tag_properties(
-                    repository, order_by=ArtifactTagOrder.LAST_UPDATED_ON_DESCENDING
+                    repository_name, order_by=ArtifactTagOrder.LAST_UPDATED_ON_DESCENDING
                 ):
                     tag_count += 1
                     if tag_count > 3:                        
-                        print(f"Deleting {repository}:{tag.name}")
-                        await client.delete_tag(repository, tag.name)
+                        print(f"Deleting {repository_name}:{tag.name}")
+                        await client.delete_tag(repository_name, tag.name)
 
 
 async def main():
     sample = DeleteTagsAsync()
     await sample.delete_tags()
```

## Comparing `azure-containerregistry-1.1.0b4/samples/README.md` & `azure-containerregistry-1.2.0/samples/README.md`

 * *Files identical despite different names*

## Comparing `azure-containerregistry-1.1.0b4/samples/sample_set_image_properties_async.py` & `azure-containerregistry-1.2.0/samples/sample_list_tags_async.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,69 +3,59 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 
 """
-FILE: sample_set_image_properties_async.py
+FILE: sample_list_tags_async.py
 
 DESCRIPTION:
-    This sample demonstrates setting an image's properties on the tag so it can't be overwritten during a lengthy
-    deployment.
+    This sample demonstrates listing the tags for an image in a repository with anonymous pull access.
+    Anonymous access allows a user to list all the collections there, but they wouldn't have permissions to
+    modify or delete any of the images in the registry.
 
 USAGE:
-    python sample_set_image_properties_async.py
+    python sample_list_tags_async.py
 
     Set the environment variables with your own values before running the sample:
-    1) CONTAINERREGISTRY_ENDPOINT - The URL of you Container Registry account
+    1) CONTAINERREGISTRY_ANONREGISTRY_ENDPOINT - The URL of your Container Registry account
 
-    This sample assumes your registry has a repository "library/hello-world" with image tagged "v1",
+    This sample assumes your registry has a repository "library/hello-world" with image tagged "latest",
     run load_registry() if you don't have.
     Set the environment variables with your own values before running load_registry():
-    1) CONTAINERREGISTRY_ENDPOINT - The URL of you Container Registry account
+    1) CONTAINERREGISTRY_ANONREGISTRY_ENDPOINT - The URL of your Container Registry account
     2) CONTAINERREGISTRY_TENANT_ID - The service principal's tenant ID
     3) CONTAINERREGISTRY_CLIENT_ID - The service principal's client ID
     4) CONTAINERREGISTRY_CLIENT_SECRET - The service principal's client secret
-    5) CONTAINERREGISTRY_RESOURCE_GROUP - The resource group name
-    6) CONTAINERREGISTRY_REGISTRY_NAME - The registry name
 """
 import asyncio
 import os
 from dotenv import find_dotenv, load_dotenv
 from azure.containerregistry.aio import ContainerRegistryClient
-from utilities import load_registry, get_authority, get_audience, get_credential
+from utilities import load_registry
 
 
-class SetImagePropertiesAsync(object):
+class ListTagsAsync(object):
     def __init__(self):
         load_dotenv(find_dotenv())
-        self.endpoint = os.environ.get("CONTAINERREGISTRY_ENDPOINT")
-        self.authority = get_authority(self.endpoint)
-        self.audience = get_audience(self.authority)
-        self.credential = get_credential(self.authority, is_async=True)
-
-    async def set_image_properties(self):
-        load_registry()
-        # Instantiate an instance of ContainerRegistryClient
-        async with ContainerRegistryClient(self.endpoint, self.credential, audience=self.audience) as client:
-            # Set permissions on the v1 image's "latest" tag
-            await client.update_manifest_properties(
-                "library/hello-world",
-                "v1",
-                can_write=False,
-                can_delete=False
-            )
-            # After this update, if someone were to push an update to `<registry endpoint>\library\hello-world:v1`,
-            # it would fail. It's worth noting that if this image also had another tag, such as `latest`,
-            # and that tag did not have permissions set to prevent reads or deletes, the image could still be
-            # overwritten. For example, if someone were to push an update to `<registry endpoint>\hello-world:latest`
-            # (which references the same image), it would succeed.
+
+    async def list_tags(self):
+        endpoint = os.environ.get("CONTAINERREGISTRY_ANONREGISTRY_ENDPOINT")
+        load_registry(endpoint)
+        # [START list_tags_anonymous]
+        async with ContainerRegistryClient(endpoint) as anon_client:
+            manifest = await anon_client.get_manifest_properties("library/hello-world", "latest")
+            print(f"Tags of {manifest.repository_name}: ")
+            # Iterate through all the tags
+            for tag in manifest.tags:
+                print(tag)
+        # [END list_tags_anonymous]
 
 
 async def main():
-    sample = SetImagePropertiesAsync()
-    await sample.set_image_properties()
+    sample = ListTagsAsync()
+    await sample.list_tags()
 
 
 if __name__ == "__main__":
     asyncio.run(main())
```

## Comparing `azure-containerregistry-1.1.0b4/azure_containerregistry.egg-info/SOURCES.txt` & `azure-containerregistry-1.2.0/azure_containerregistry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

