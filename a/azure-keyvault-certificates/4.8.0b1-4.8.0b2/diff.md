# Comparing `tmp/azure-keyvault-certificates-4.8.0b1.zip` & `tmp/azure-keyvault-certificates-4.8.0b2.zip`

## zipinfo {}

```diff
@@ -1,256 +1,255 @@
-Zip file size: 534642 bytes, number of entries: 254
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/samples/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure_keyvault_certificates.egg-info/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/tests/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/
--rw-rw-r--  2.0 unx       38 b- defN 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/setup.cfg
--rw-rw-r--  2.0 unx    35007 b- defN 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/PKG-INFO
--rw-rw-r--  2.0 unx       86 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/pyproject.toml
--rw-rw-r--  2.0 unx      195 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/MANIFEST.in
--rw-rw-r--  2.0 unx    21358 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/README.md
--rw-rw-r--  2.0 unx    12720 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/CHANGELOG.md
--rw-rw-r--  2.0 unx     2464 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/setup.py
--rw-rw-r--  2.0 unx      285 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/TROUBLESHOOTING.md
--rw-rw-r--  2.0 unx     1073 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/LICENSE
--rw-rw-r--  2.0 unx    11900 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/migration_guide.md
--rw-rw-r--  2.0 unx     3235 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/samples/import_certificate.py
--rw-rw-r--  2.0 unx     2461 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/samples/contacts_async.py
--rw-rw-r--  2.0 unx     3549 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/samples/import_certificate_async.py
--rw-rw-r--  2.0 unx     4103 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/samples/recover_purge_operations_async.py
--rw-rw-r--  2.0 unx     4810 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/samples/parse_certificate.py
--rw-rw-r--  2.0 unx     4946 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/samples/parse_certificate_async.py
--rw-rw-r--  2.0 unx     3452 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/samples/issuers.py
--rw-rw-r--  2.0 unx     3790 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/samples/backup_restore_operations_async.py
--rw-rw-r--  2.0 unx     5000 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/samples/list_operations_async.py
--rw-rw-r--  2.0 unx     4491 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/samples/hello_world_async.py
--rw-rw-r--  2.0 unx     2272 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/samples/contacts.py
--rw-rw-r--  2.0 unx     4089 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/samples/recover_purge_operations.py
--rw-rw-r--  2.0 unx     3766 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/samples/issuers_async.py
--rw-rw-r--  2.0 unx     5032 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/samples/list_operations.py
--rw-rw-r--  2.0 unx     3826 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/samples/backup_restore_operations.py
--rw-rw-r--  2.0 unx     4453 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/samples/hello_world.py
--rw-rw-r--  2.0 unx        1 b- defN 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure_keyvault_certificates.egg-info/dependency_links.txt
--rw-rw-r--  2.0 unx    35007 b- defN 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure_keyvault_certificates.egg-info/PKG-INFO
--rw-rw-r--  2.0 unx        6 b- defN 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure_keyvault_certificates.egg-info/top_level.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure_keyvault_certificates.egg-info/not-zip-safe
--rw-rw-r--  2.0 unx    11428 b- defN 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure_keyvault_certificates.egg-info/SOURCES.txt
--rw-rw-r--  2.0 unx       84 b- defN 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure_keyvault_certificates.egg-info/requires.txt
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/tests/_shared/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/tests/perfstress_tests/
--rw-rw-r--  2.0 unx     2258 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/_async_test_case.py
--rw-rw-r--  2.0 unx    33352 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/test_certificates_client_async.py
--rw-rw-r--  2.0 unx     2778 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/test_merge_certificate_async.py
--rw-rw-r--  2.0 unx     2191 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/_test_case.py
--rw-rw-r--  2.0 unx      869 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/test_multi_api.py
--rw-rw-r--  2.0 unx     2544 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/test_merge_certificate.py
--rw-rw-r--  2.0 unx     3411 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/test_parse_id.py
--rw-rw-r--  2.0 unx     2847 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/conftest.py
--rw-rw-r--  2.0 unx    14239 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/test_examples_certificates.py
--rw-rw-r--  2.0 unx      959 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/test_context_manager_async.py
--rw-rw-r--  2.0 unx    14130 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/test_examples_certificates_async.py
--rw-rw-r--  2.0 unx    14389 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/certs.py
--rw-rw-r--  2.0 unx    32695 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/test_certificates_client.py
--rw-rw-r--  2.0 unx      841 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/test_context_manager.py
--rw-rw-r--  2.0 unx     3935 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/_shared/helpers.py
--rw-rw-r--  2.0 unx      578 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/_shared/json_attribute_matcher.py
--rw-rw-r--  2.0 unx     1407 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/_shared/helpers_async.py
--rw-rw-r--  2.0 unx     1094 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/_shared/preparer.py
--rw-rw-r--  2.0 unx     1909 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/_shared/test_case_async.py
--rw-rw-r--  2.0 unx     1639 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/_shared/test_case.py
--rw-rw-r--  2.0 unx      656 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/_shared/preparer_async.py
--rw-rw-r--  2.0 unx      151 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/_shared/__init__.py
--rw-rw-r--  2.0 unx     2077 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/perfstress_tests/get_certificate.py
--rw-rw-r--  2.0 unx        0 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/tests/perfstress_tests/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/
--rw-rw-r--  2.0 unx      267 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/
--rw-rw-r--  2.0 unx      267 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/aio/
--rw-rw-r--  2.0 unx    47947 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_client.py
--rw-rw-r--  2.0 unx     2437 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_polling.py
--rw-rw-r--  2.0 unx      172 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_version.py
--rw-rw-r--  2.0 unx    50258 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_models.py
--rw-rw-r--  2.0 unx     2861 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_enums.py
--rw-rw-r--  2.0 unx        0 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/py.typed
--rw-rw-r--  2.0 unx      231 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_sdk_moniker.py
--rw-rw-r--  2.0 unx    71756 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated_models.py
--rw-rw-r--  2.0 unx     1350 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/__init__.py
--rw-rw-r--  2.0 unx     4939 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/http_challenge.py
--rw-rw-r--  2.0 unx     4775 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/_polling.py
--rw-rw-r--  2.0 unx     2702 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/_polling_async.py
--rw-rw-r--  2.0 unx     2113 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/exceptions.py
--rw-rw-r--  2.0 unx     6078 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/challenge_auth_policy.py
--rw-rw-r--  2.0 unx     4968 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/async_client_base.py
--rw-rw-r--  2.0 unx     2579 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/http_challenge_cache.py
--rw-rw-r--  2.0 unx     5307 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/async_challenge_auth_policy.py
--rw-rw-r--  2.0 unx     2390 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/__init__.py
--rw-rw-r--  2.0 unx     6247 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/client_base.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/aio/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/
--rw-rw-r--  2.0 unx   191906 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/_operations_mixin.py
--rw-rw-r--  2.0 unx     1993 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/_configuration.py
--rw-rw-r--  2.0 unx      344 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/_version.py
--rw-rw-r--  2.0 unx     4616 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/_key_vault_client.py
--rw-rw-r--  2.0 unx      353 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/models.py
--rw-rw-r--  2.0 unx    78842 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/_serialization.py
--rw-rw-r--  2.0 unx      698 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/models/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/
--rw-rw-r--  2.0 unx     2511 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/_configuration.py
--rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/_patch.py
--rw-rw-r--  2.0 unx     3131 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/_key_vault_client.py
--rw-rw-r--  2.0 unx      829 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/__init__.py
--rw-rw-r--  2.0 unx     1808 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/_vendor.py
--rw-rw-r--  2.0 unx   461426 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/operations/_key_vault_client_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/operations/_patch.py
--rw-rw-r--  2.0 unx      816 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/operations/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/models/_patch.py
--rw-rw-r--  2.0 unx     7788 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/models/_key_vault_client_enums.py
--rw-rw-r--  2.0 unx   156906 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/models/_models_py3.py
--rw-rw-r--  2.0 unx     7985 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/models/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/operations/
--rw-rw-r--  2.0 unx     2521 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/_configuration.py
--rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/_patch.py
--rw-rw-r--  2.0 unx     3236 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/_key_vault_client.py
--rw-rw-r--  2.0 unx      829 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/__init__.py
--rw-rw-r--  2.0 unx     1043 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/_vendor.py
--rw-rw-r--  2.0 unx   382727 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/operations/_key_vault_client_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/operations/_patch.py
--rw-rw-r--  2.0 unx      816 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/operations/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/models/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/
--rw-rw-r--  2.0 unx     2511 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/_configuration.py
--rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/_patch.py
--rw-rw-r--  2.0 unx     3131 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/_key_vault_client.py
--rw-rw-r--  2.0 unx      829 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/__init__.py
--rw-rw-r--  2.0 unx     1808 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/_vendor.py
--rw-rw-r--  2.0 unx   155108 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/operations/_key_vault_client_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/operations/_patch.py
--rw-rw-r--  2.0 unx      816 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/operations/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/models/_patch.py
--rw-rw-r--  2.0 unx     5011 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/models/_key_vault_client_enums.py
--rw-rw-r--  2.0 unx    65498 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/models/_models_py3.py
--rw-rw-r--  2.0 unx     3963 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/models/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/operations/
--rw-rw-r--  2.0 unx     2521 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/_configuration.py
--rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/_patch.py
--rw-rw-r--  2.0 unx     3236 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/_key_vault_client.py
--rw-rw-r--  2.0 unx      829 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/__init__.py
--rw-rw-r--  2.0 unx     1043 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/_vendor.py
--rw-rw-r--  2.0 unx   128804 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/operations/_key_vault_client_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/operations/_patch.py
--rw-rw-r--  2.0 unx      816 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/operations/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/models/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/
--rw-rw-r--  2.0 unx     2511 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/_configuration.py
--rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/_patch.py
--rw-rw-r--  2.0 unx     3131 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/_key_vault_client.py
--rw-rw-r--  2.0 unx      829 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/__init__.py
--rw-rw-r--  2.0 unx     1808 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/_vendor.py
--rw-rw-r--  2.0 unx   155108 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/operations/_key_vault_client_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/operations/_patch.py
--rw-rw-r--  2.0 unx      816 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/operations/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/models/_patch.py
--rw-rw-r--  2.0 unx     5035 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/models/_key_vault_client_enums.py
--rw-rw-r--  2.0 unx    65586 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/models/_models_py3.py
--rw-rw-r--  2.0 unx     3963 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/models/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/operations/
--rw-rw-r--  2.0 unx     2521 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/_configuration.py
--rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/_patch.py
--rw-rw-r--  2.0 unx     3236 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/_key_vault_client.py
--rw-rw-r--  2.0 unx      829 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/__init__.py
--rw-rw-r--  2.0 unx     1043 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/_vendor.py
--rw-rw-r--  2.0 unx   128804 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/operations/_key_vault_client_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/operations/_patch.py
--rw-rw-r--  2.0 unx      816 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/operations/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/models/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/
--rw-rw-r--  2.0 unx     2511 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/_configuration.py
--rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/_patch.py
--rw-rw-r--  2.0 unx     3131 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/_key_vault_client.py
--rw-rw-r--  2.0 unx      829 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/__init__.py
--rw-rw-r--  2.0 unx     1808 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/_vendor.py
--rw-rw-r--  2.0 unx   156980 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/operations/_key_vault_client_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/operations/_patch.py
--rw-rw-r--  2.0 unx      816 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/operations/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/models/_patch.py
--rw-rw-r--  2.0 unx     5068 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/models/_key_vault_client_enums.py
--rw-rw-r--  2.0 unx    65953 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/models/_models_py3.py
--rw-rw-r--  2.0 unx     3963 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/models/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/operations/
--rw-rw-r--  2.0 unx     2521 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/_configuration.py
--rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/_patch.py
--rw-rw-r--  2.0 unx     3236 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/_key_vault_client.py
--rw-rw-r--  2.0 unx      829 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/__init__.py
--rw-rw-r--  2.0 unx     1043 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/_vendor.py
--rw-rw-r--  2.0 unx   130676 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/operations/_key_vault_client_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/operations/_patch.py
--rw-rw-r--  2.0 unx      816 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/operations/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/models/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/
--rw-rw-r--  2.0 unx     2532 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/_configuration.py
--rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/_patch.py
--rw-rw-r--  2.0 unx     3138 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/_key_vault_client.py
--rw-rw-r--  2.0 unx      829 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/__init__.py
--rw-rw-r--  2.0 unx     1808 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/_vendor.py
--rw-rw-r--  2.0 unx   408005 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/operations/_key_vault_client_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/operations/_patch.py
--rw-rw-r--  2.0 unx      816 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/operations/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/models/_patch.py
--rw-rw-r--  2.0 unx     3896 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/models/_key_vault_client_enums.py
--rw-rw-r--  2.0 unx   135465 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/models/_models_py3.py
--rw-rw-r--  2.0 unx     7089 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/models/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/
--rw-rw-r--  2.0 unx     2542 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/_configuration.py
--rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/_patch.py
--rw-rw-r--  2.0 unx     3243 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/_key_vault_client.py
--rw-rw-r--  2.0 unx      829 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/__init__.py
--rw-rw-r--  2.0 unx     1043 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/_vendor.py
--rw-rw-r--  2.0 unx   339680 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/_key_vault_client_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/_patch.py
--rw-rw-r--  2.0 unx      816 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/__init__.py
--rw-rw-r--  2.0 unx   194271 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/aio/_operations_mixin.py
--rw-rw-r--  2.0 unx     2020 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/aio/_configuration.py
--rw-rw-r--  2.0 unx     4685 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/aio/_key_vault_client.py
--rw-rw-r--  2.0 unx      543 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/aio/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/operations/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/models/
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/
--rw-rw-r--  2.0 unx     2511 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/_configuration.py
--rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/_patch.py
--rw-rw-r--  2.0 unx     3131 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/_key_vault_client.py
--rw-rw-r--  2.0 unx      829 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/__init__.py
--rw-rw-r--  2.0 unx     1808 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/_vendor.py
--rw-rw-r--  2.0 unx   154948 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/operations/_key_vault_client_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/operations/_patch.py
--rw-rw-r--  2.0 unx      816 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/operations/__init__.py
--rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/models/_patch.py
--rw-rw-r--  2.0 unx     5035 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/models/_key_vault_client_enums.py
--rw-rw-r--  2.0 unx    66011 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/models/_models_py3.py
--rw-rw-r--  2.0 unx     3963 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/models/__init__.py
-drwxrwxr-x  2.0 unx        0 b- stor 23-May-16 23:25 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/operations/
--rw-rw-r--  2.0 unx     2521 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/_configuration.py
--rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/_patch.py
--rw-rw-r--  2.0 unx     3236 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/_key_vault_client.py
--rw-rw-r--  2.0 unx      829 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/__init__.py
--rw-rw-r--  2.0 unx     1043 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/_vendor.py
--rw-rw-r--  2.0 unx   128644 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/operations/_key_vault_client_operations.py
--rw-rw-r--  2.0 unx      674 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/operations/_patch.py
--rw-rw-r--  2.0 unx      816 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/operations/__init__.py
--rw-rw-r--  2.0 unx    46900 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/aio/_client.py
--rw-rw-r--  2.0 unx     2311 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/aio/_polling_async.py
--rw-rw-r--  2.0 unx      224 b- defN 23-May-16 23:24 azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/aio/__init__.py
-254 files, 4559831 bytes uncompressed, 470826 bytes compressed:  89.7%
+Zip file size: 536158 bytes, number of entries: 253
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure_keyvault_certificates.egg-info/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/tests/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/samples/
+-rw-rw-r--  2.0 unx    21358 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/README.md
+-rw-rw-r--  2.0 unx      195 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/MANIFEST.in
+-rw-rw-r--  2.0 unx       86 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/pyproject.toml
+-rw-rw-r--  2.0 unx    12978 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/CHANGELOG.md
+-rw-rw-r--  2.0 unx    12685 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/migration_guide.md
+-rw-rw-r--  2.0 unx     2464 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/setup.py
+-rw-rw-r--  2.0 unx    35265 b- defN 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/PKG-INFO
+-rw-rw-r--  2.0 unx       38 b- defN 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/setup.cfg
+-rw-rw-r--  2.0 unx     1073 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/LICENSE
+-rw-rw-r--  2.0 unx      285 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/TROUBLESHOOTING.md
+-rw-rw-r--  2.0 unx    11378 b- defN 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure_keyvault_certificates.egg-info/SOURCES.txt
+-rw-rw-r--  2.0 unx       84 b- defN 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure_keyvault_certificates.egg-info/requires.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure_keyvault_certificates.egg-info/dependency_links.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure_keyvault_certificates.egg-info/not-zip-safe
+-rw-rw-r--  2.0 unx    35265 b- defN 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure_keyvault_certificates.egg-info/PKG-INFO
+-rw-rw-r--  2.0 unx        6 b- defN 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure_keyvault_certificates.egg-info/top_level.txt
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure/keyvault/
+-rw-rw-r--  2.0 unx      267 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/
+-rw-rw-r--  2.0 unx      267 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/__init__.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_shared/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/aio/
+-rw-rw-r--  2.0 unx     2250 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_polling.py
+-rw-rw-r--  2.0 unx     1350 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/__init__.py
+-rw-rw-r--  2.0 unx     2861 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_enums.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/py.typed
+-rw-rw-r--  2.0 unx    55208 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_models.py
+-rw-rw-r--  2.0 unx    71756 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated_models.py
+-rw-rw-r--  2.0 unx      231 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_sdk_moniker.py
+-rw-rw-r--  2.0 unx      172 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_version.py
+-rw-rw-r--  2.0 unx    47100 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_client.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/aio/
+-rw-rw-r--  2.0 unx    78842 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/_serialization.py
+-rw-rw-r--  2.0 unx     1993 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/_configuration.py
+-rw-rw-r--  2.0 unx      698 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/__init__.py
+-rw-rw-r--  2.0 unx   191906 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/_operations_mixin.py
+-rw-rw-r--  2.0 unx      353 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/models.py
+-rw-rw-r--  2.0 unx      344 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/_version.py
+-rw-rw-r--  2.0 unx     4616 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/_key_vault_client.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/aio/
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/_patch.py
+-rw-rw-r--  2.0 unx     2511 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/_configuration.py
+-rw-rw-r--  2.0 unx      829 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/__init__.py
+-rw-rw-r--  2.0 unx     1808 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/_vendor.py
+-rw-rw-r--  2.0 unx     3131 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/_key_vault_client.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/models/_patch.py
+-rw-rw-r--  2.0 unx    65498 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/models/_models_py3.py
+-rw-rw-r--  2.0 unx     5011 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/models/_key_vault_client_enums.py
+-rw-rw-r--  2.0 unx     3963 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/models/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/operations/_patch.py
+-rw-rw-r--  2.0 unx      816 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/operations/__init__.py
+-rw-rw-r--  2.0 unx   155108 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/operations/_key_vault_client_operations.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/aio/operations/
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/aio/_patch.py
+-rw-rw-r--  2.0 unx     2521 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/aio/_configuration.py
+-rw-rw-r--  2.0 unx      829 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/aio/__init__.py
+-rw-rw-r--  2.0 unx     1043 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/aio/_vendor.py
+-rw-rw-r--  2.0 unx     3236 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/aio/_key_vault_client.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx      816 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx   128804 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/aio/operations/_key_vault_client_operations.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/aio/
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/_patch.py
+-rw-rw-r--  2.0 unx     2511 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/_configuration.py
+-rw-rw-r--  2.0 unx      829 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/__init__.py
+-rw-rw-r--  2.0 unx     1808 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/_vendor.py
+-rw-rw-r--  2.0 unx     3131 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/_key_vault_client.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/models/_patch.py
+-rw-rw-r--  2.0 unx    65586 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/models/_models_py3.py
+-rw-rw-r--  2.0 unx     5035 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/models/_key_vault_client_enums.py
+-rw-rw-r--  2.0 unx     3963 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/models/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/operations/_patch.py
+-rw-rw-r--  2.0 unx      816 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/operations/__init__.py
+-rw-rw-r--  2.0 unx   155108 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/operations/_key_vault_client_operations.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/aio/operations/
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/aio/_patch.py
+-rw-rw-r--  2.0 unx     2521 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/aio/_configuration.py
+-rw-rw-r--  2.0 unx      829 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/aio/__init__.py
+-rw-rw-r--  2.0 unx     1043 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/aio/_vendor.py
+-rw-rw-r--  2.0 unx     3236 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/aio/_key_vault_client.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx      816 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx   128804 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/aio/operations/_key_vault_client_operations.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/aio/
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/_patch.py
+-rw-rw-r--  2.0 unx     2511 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/_configuration.py
+-rw-rw-r--  2.0 unx      829 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/__init__.py
+-rw-rw-r--  2.0 unx     1808 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/_vendor.py
+-rw-rw-r--  2.0 unx     3131 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/_key_vault_client.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/models/_patch.py
+-rw-rw-r--  2.0 unx    65953 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/models/_models_py3.py
+-rw-rw-r--  2.0 unx     5068 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/models/_key_vault_client_enums.py
+-rw-rw-r--  2.0 unx     3963 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/models/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/operations/_patch.py
+-rw-rw-r--  2.0 unx      816 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/operations/__init__.py
+-rw-rw-r--  2.0 unx   156980 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/operations/_key_vault_client_operations.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/aio/operations/
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/aio/_patch.py
+-rw-rw-r--  2.0 unx     2521 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/aio/_configuration.py
+-rw-rw-r--  2.0 unx      829 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/aio/__init__.py
+-rw-rw-r--  2.0 unx     1043 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/aio/_vendor.py
+-rw-rw-r--  2.0 unx     3236 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/aio/_key_vault_client.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx      816 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx   130676 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/aio/operations/_key_vault_client_operations.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/aio/
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/_patch.py
+-rw-rw-r--  2.0 unx     2532 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/_configuration.py
+-rw-rw-r--  2.0 unx      829 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/__init__.py
+-rw-rw-r--  2.0 unx     1808 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/_vendor.py
+-rw-rw-r--  2.0 unx     3138 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/_key_vault_client.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/models/_patch.py
+-rw-rw-r--  2.0 unx   135465 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/models/_models_py3.py
+-rw-rw-r--  2.0 unx     3896 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/models/_key_vault_client_enums.py
+-rw-rw-r--  2.0 unx     7089 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/models/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/operations/_patch.py
+-rw-rw-r--  2.0 unx      816 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/operations/__init__.py
+-rw-rw-r--  2.0 unx   408005 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/operations/_key_vault_client_operations.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/aio/_patch.py
+-rw-rw-r--  2.0 unx     2542 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/aio/_configuration.py
+-rw-rw-r--  2.0 unx      829 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/aio/__init__.py
+-rw-rw-r--  2.0 unx     1043 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/aio/_vendor.py
+-rw-rw-r--  2.0 unx     3243 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/aio/_key_vault_client.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx      816 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx   339680 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/_key_vault_client_operations.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/aio/
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/_patch.py
+-rw-rw-r--  2.0 unx     2511 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/_configuration.py
+-rw-rw-r--  2.0 unx      829 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/__init__.py
+-rw-rw-r--  2.0 unx     1808 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/_vendor.py
+-rw-rw-r--  2.0 unx     3131 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/_key_vault_client.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/models/_patch.py
+-rw-rw-r--  2.0 unx   156906 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/models/_models_py3.py
+-rw-rw-r--  2.0 unx     7788 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/models/_key_vault_client_enums.py
+-rw-rw-r--  2.0 unx     7985 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/models/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/operations/_patch.py
+-rw-rw-r--  2.0 unx      816 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/operations/__init__.py
+-rw-rw-r--  2.0 unx   461426 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/operations/_key_vault_client_operations.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/aio/operations/
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/aio/_patch.py
+-rw-rw-r--  2.0 unx     2521 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/aio/_configuration.py
+-rw-rw-r--  2.0 unx      829 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/aio/__init__.py
+-rw-rw-r--  2.0 unx     1043 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/aio/_vendor.py
+-rw-rw-r--  2.0 unx     3236 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/aio/_key_vault_client.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx      816 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx   382727 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/aio/operations/_key_vault_client_operations.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/models/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/operations/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/aio/
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/_patch.py
+-rw-rw-r--  2.0 unx     2511 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/_configuration.py
+-rw-rw-r--  2.0 unx      829 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/__init__.py
+-rw-rw-r--  2.0 unx     1808 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/_vendor.py
+-rw-rw-r--  2.0 unx     3131 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/_key_vault_client.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/models/_patch.py
+-rw-rw-r--  2.0 unx    66011 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/models/_models_py3.py
+-rw-rw-r--  2.0 unx     5035 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/models/_key_vault_client_enums.py
+-rw-rw-r--  2.0 unx     3963 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/models/__init__.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/operations/_patch.py
+-rw-rw-r--  2.0 unx      816 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/operations/__init__.py
+-rw-rw-r--  2.0 unx   154948 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/operations/_key_vault_client_operations.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/aio/operations/
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/aio/_patch.py
+-rw-rw-r--  2.0 unx     2521 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/aio/_configuration.py
+-rw-rw-r--  2.0 unx      829 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/aio/__init__.py
+-rw-rw-r--  2.0 unx     1043 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/aio/_vendor.py
+-rw-rw-r--  2.0 unx     3236 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/aio/_key_vault_client.py
+-rw-rw-r--  2.0 unx      674 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/aio/operations/_patch.py
+-rw-rw-r--  2.0 unx      816 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/aio/operations/__init__.py
+-rw-rw-r--  2.0 unx   128644 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/aio/operations/_key_vault_client_operations.py
+-rw-rw-r--  2.0 unx     2020 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/aio/_configuration.py
+-rw-rw-r--  2.0 unx      543 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/aio/__init__.py
+-rw-rw-r--  2.0 unx   194271 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/aio/_operations_mixin.py
+-rw-rw-r--  2.0 unx     4685 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/aio/_key_vault_client.py
+-rw-rw-r--  2.0 unx     5243 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_shared/_polling.py
+-rw-rw-r--  2.0 unx     5527 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_shared/async_challenge_auth_policy.py
+-rw-rw-r--  2.0 unx     2784 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_shared/http_challenge_cache.py
+-rw-rw-r--  2.0 unx     2989 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_shared/_polling_async.py
+-rw-rw-r--  2.0 unx     6661 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_shared/http_challenge.py
+-rw-rw-r--  2.0 unx     2406 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_shared/__init__.py
+-rw-rw-r--  2.0 unx     6655 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_shared/challenge_auth_policy.py
+-rw-rw-r--  2.0 unx     4984 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_shared/async_client_base.py
+-rw-rw-r--  2.0 unx     6593 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_shared/client_base.py
+-rw-rw-r--  2.0 unx     2311 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/aio/_polling_async.py
+-rw-rw-r--  2.0 unx      224 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/aio/__init__.py
+-rw-rw-r--  2.0 unx    46308 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/aio/_client.py
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/tests/perfstress_tests/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Jul-11 16:56 azure-keyvault-certificates-4.8.0b2/tests/_shared/
+-rw-rw-r--  2.0 unx      959 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/tests/test_context_manager_async.py
+-rw-rw-r--  2.0 unx      841 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/tests/test_context_manager.py
+-rw-rw-r--  2.0 unx    14389 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/tests/certs.py
+-rw-rw-r--  2.0 unx     2191 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/tests/_test_case.py
+-rw-rw-r--  2.0 unx    14130 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/tests/test_examples_certificates_async.py
+-rw-rw-r--  2.0 unx    34260 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/tests/test_certificates_client.py
+-rw-rw-r--  2.0 unx     2258 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/tests/_async_test_case.py
+-rw-rw-r--  2.0 unx    34443 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/tests/test_certificates_client_async.py
+-rw-rw-r--  2.0 unx     2847 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/tests/conftest.py
+-rw-rw-r--  2.0 unx     3411 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/tests/test_parse_id.py
+-rw-rw-r--  2.0 unx     2544 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/tests/test_merge_certificate.py
+-rw-rw-r--  2.0 unx      869 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/tests/test_multi_api.py
+-rw-rw-r--  2.0 unx    14239 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/tests/test_examples_certificates.py
+-rw-rw-r--  2.0 unx     2778 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/tests/test_merge_certificate_async.py
+-rw-rw-r--  2.0 unx     2077 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/tests/perfstress_tests/get_certificate.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/tests/perfstress_tests/__init__.py
+-rw-rw-r--  2.0 unx     1909 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/tests/_shared/test_case_async.py
+-rw-rw-r--  2.0 unx     1094 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/tests/_shared/preparer.py
+-rw-rw-r--  2.0 unx      151 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/tests/_shared/__init__.py
+-rw-rw-r--  2.0 unx      656 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/tests/_shared/preparer_async.py
+-rw-rw-r--  2.0 unx     3935 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/tests/_shared/helpers.py
+-rw-rw-r--  2.0 unx     1407 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/tests/_shared/helpers_async.py
+-rw-rw-r--  2.0 unx     1639 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/tests/_shared/test_case.py
+-rw-rw-r--  2.0 unx      578 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/tests/_shared/json_attribute_matcher.py
+-rw-rw-r--  2.0 unx     4453 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/samples/hello_world.py
+-rw-rw-r--  2.0 unx     4491 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/samples/hello_world_async.py
+-rw-rw-r--  2.0 unx     3766 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/samples/issuers_async.py
+-rw-rw-r--  2.0 unx     4103 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/samples/recover_purge_operations_async.py
+-rw-rw-r--  2.0 unx     3549 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/samples/import_certificate_async.py
+-rw-rw-r--  2.0 unx     4946 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/samples/parse_certificate_async.py
+-rw-rw-r--  2.0 unx     4810 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/samples/parse_certificate.py
+-rw-rw-r--  2.0 unx     3790 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/samples/backup_restore_operations_async.py
+-rw-rw-r--  2.0 unx     2272 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/samples/contacts.py
+-rw-rw-r--  2.0 unx     2461 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/samples/contacts_async.py
+-rw-rw-r--  2.0 unx     5032 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/samples/list_operations.py
+-rw-rw-r--  2.0 unx     5000 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/samples/list_operations_async.py
+-rw-rw-r--  2.0 unx     3452 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/samples/issuers.py
+-rw-rw-r--  2.0 unx     3826 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/samples/backup_restore_operations.py
+-rw-rw-r--  2.0 unx     3235 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/samples/import_certificate.py
+-rw-rw-r--  2.0 unx     4089 b- defN 23-Jul-11 16:55 azure-keyvault-certificates-4.8.0b2/samples/recover_purge_operations.py
+253 files, 4569064 bytes uncompressed, 472588 bytes compressed:  89.7%
```

## zipnote {}

```diff
@@ -1,763 +1,760 @@
-Filename: azure-keyvault-certificates-4.8.0b1/
+Filename: azure-keyvault-certificates-4.8.0b2/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/samples/
+Filename: azure-keyvault-certificates-4.8.0b2/azure_keyvault_certificates.egg-info/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure_keyvault_certificates.egg-info/
+Filename: azure-keyvault-certificates-4.8.0b2/azure/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/tests/
+Filename: azure-keyvault-certificates-4.8.0b2/tests/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/
+Filename: azure-keyvault-certificates-4.8.0b2/samples/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/setup.cfg
+Filename: azure-keyvault-certificates-4.8.0b2/README.md
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/PKG-INFO
+Filename: azure-keyvault-certificates-4.8.0b2/MANIFEST.in
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/pyproject.toml
+Filename: azure-keyvault-certificates-4.8.0b2/pyproject.toml
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/MANIFEST.in
+Filename: azure-keyvault-certificates-4.8.0b2/CHANGELOG.md
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/README.md
+Filename: azure-keyvault-certificates-4.8.0b2/migration_guide.md
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/CHANGELOG.md
+Filename: azure-keyvault-certificates-4.8.0b2/setup.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/setup.py
+Filename: azure-keyvault-certificates-4.8.0b2/PKG-INFO
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/TROUBLESHOOTING.md
+Filename: azure-keyvault-certificates-4.8.0b2/setup.cfg
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/LICENSE
+Filename: azure-keyvault-certificates-4.8.0b2/LICENSE
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/migration_guide.md
+Filename: azure-keyvault-certificates-4.8.0b2/TROUBLESHOOTING.md
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/samples/import_certificate.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure_keyvault_certificates.egg-info/SOURCES.txt
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/samples/contacts_async.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure_keyvault_certificates.egg-info/requires.txt
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/samples/import_certificate_async.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure_keyvault_certificates.egg-info/dependency_links.txt
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/samples/recover_purge_operations_async.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure_keyvault_certificates.egg-info/not-zip-safe
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/samples/parse_certificate.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure_keyvault_certificates.egg-info/PKG-INFO
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/samples/parse_certificate_async.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure_keyvault_certificates.egg-info/top_level.txt
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/samples/issuers.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/samples/backup_restore_operations_async.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/samples/list_operations_async.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/samples/hello_world_async.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/samples/contacts.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/samples/recover_purge_operations.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_shared/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/samples/issuers_async.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/aio/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/samples/list_operations.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_polling.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/samples/backup_restore_operations.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/samples/hello_world.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_enums.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure_keyvault_certificates.egg-info/dependency_links.txt
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/py.typed
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure_keyvault_certificates.egg-info/PKG-INFO
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_models.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure_keyvault_certificates.egg-info/top_level.txt
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated_models.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure_keyvault_certificates.egg-info/not-zip-safe
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_sdk_moniker.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure_keyvault_certificates.egg-info/SOURCES.txt
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_version.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure_keyvault_certificates.egg-info/requires.txt
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_client.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/tests/_shared/
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/tests/perfstress_tests/
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/tests/_async_test_case.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/tests/test_certificates_client_async.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/tests/test_merge_certificate_async.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/tests/_test_case.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/tests/test_multi_api.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/aio/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/tests/test_merge_certificate.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/_serialization.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/tests/test_parse_id.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/tests/conftest.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/tests/test_examples_certificates.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/_operations_mixin.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/tests/test_context_manager_async.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/models.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/tests/test_examples_certificates_async.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/_version.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/tests/certs.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/tests/test_certificates_client.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/models/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/tests/test_context_manager.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/operations/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/tests/_shared/helpers.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/aio/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/tests/_shared/json_attribute_matcher.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/tests/_shared/helpers_async.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/tests/_shared/preparer.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/tests/_shared/test_case_async.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/_vendor.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/tests/_shared/test_case.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/tests/_shared/preparer_async.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/models/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/tests/_shared/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/models/_models_py3.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/tests/perfstress_tests/get_certificate.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/models/_key_vault_client_enums.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/tests/perfstress_tests/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/models/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/operations/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/operations/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/operations/_key_vault_client_operations.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/aio/operations/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/aio/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/aio/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/aio/
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/aio/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_client.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/aio/_vendor.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_polling.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/aio/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_version.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_models.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_enums.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/aio/operations/_key_vault_client_operations.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/py.typed
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/models/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_sdk_moniker.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/operations/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated_models.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/aio/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/http_challenge.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/_polling.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/_polling_async.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/_vendor.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/exceptions.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/challenge_auth_policy.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/models/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/async_client_base.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/models/_models_py3.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/http_challenge_cache.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/models/_key_vault_client_enums.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/async_challenge_auth_policy.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/models/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/operations/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/client_base.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/operations/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/operations/_key_vault_client_operations.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/aio/operations/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/aio/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/aio/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/aio/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/aio/
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/aio/_vendor.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/aio/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/_operations_mixin.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/_configuration.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/_version.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/aio/operations/_key_vault_client_operations.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/_key_vault_client.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/models/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/models.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/operations/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/_serialization.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/aio/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/operations/
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/models/
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/_vendor.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/_configuration.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/models/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/_key_vault_client.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/models/_models_py3.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/models/_key_vault_client_enums.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/_vendor.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/models/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/operations/_key_vault_client_operations.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/operations/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/operations/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/operations/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/operations/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/operations/_key_vault_client_operations.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/models/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/aio/operations/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/models/_key_vault_client_enums.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/aio/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/models/_models_py3.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/aio/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/models/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/aio/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/operations/
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/aio/_vendor.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/_configuration.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/aio/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/_key_vault_client.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/aio/operations/_key_vault_client_operations.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/_vendor.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/models/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/operations/_key_vault_client_operations.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/operations/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/operations/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/aio/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/operations/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/operations/
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/models/
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/_vendor.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/_configuration.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/models/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/_key_vault_client.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/models/_models_py3.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/models/_key_vault_client_enums.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/_vendor.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/models/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/operations/_key_vault_client_operations.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/operations/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/operations/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/operations/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/operations/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/operations/_key_vault_client_operations.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/models/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/models/_key_vault_client_enums.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/aio/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/models/_models_py3.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/aio/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/models/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/aio/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/operations/
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/aio/_vendor.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/_configuration.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/aio/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/_key_vault_client.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/_key_vault_client_operations.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/_vendor.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/models/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/operations/_key_vault_client_operations.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/operations/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/operations/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/aio/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/operations/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/operations/
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/models/
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/_vendor.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/_configuration.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/models/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/_key_vault_client.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/models/_models_py3.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/models/_key_vault_client_enums.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/_vendor.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/models/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/operations/_key_vault_client_operations.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/operations/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/operations/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/operations/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/operations/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/operations/_key_vault_client_operations.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/models/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/aio/operations/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/models/_key_vault_client_enums.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/aio/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/models/_models_py3.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/aio/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/models/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/aio/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/operations/
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/aio/_vendor.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/_configuration.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/aio/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/_key_vault_client.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/aio/operations/_key_vault_client_operations.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/_vendor.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/models/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/operations/_key_vault_client_operations.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/operations/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/operations/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/aio/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/operations/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/operations/
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/models/
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/_vendor.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/_configuration.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/models/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/_key_vault_client.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/models/_models_py3.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/models/_key_vault_client_enums.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/_vendor.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/models/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/operations/_key_vault_client_operations.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/operations/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/operations/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/operations/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/operations/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/operations/_key_vault_client_operations.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/models/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/aio/operations/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/models/_key_vault_client_enums.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/aio/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/models/_models_py3.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/aio/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/models/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/aio/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/operations/
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/aio/_vendor.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/_configuration.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/aio/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/aio/operations/_patch.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/_key_vault_client.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/aio/operations/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/aio/operations/_key_vault_client_operations.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/_vendor.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/aio/_configuration.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/operations/_key_vault_client_operations.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/aio/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/operations/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/aio/_operations_mixin.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/operations/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/aio/_key_vault_client.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/operations/
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_shared/_polling.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/models/
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_shared/async_challenge_auth_policy.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_shared/http_challenge_cache.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/_configuration.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_shared/_polling_async.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_shared/http_challenge.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/_key_vault_client.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_shared/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_shared/challenge_auth_policy.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/_vendor.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_shared/async_client_base.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/operations/_key_vault_client_operations.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_shared/client_base.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/operations/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/aio/_polling_async.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/operations/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/aio/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/models/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/aio/_client.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/models/_key_vault_client_enums.py
+Filename: azure-keyvault-certificates-4.8.0b2/tests/perfstress_tests/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/models/_models_py3.py
+Filename: azure-keyvault-certificates-4.8.0b2/tests/_shared/
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/models/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b2/tests/test_context_manager_async.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/
+Filename: azure-keyvault-certificates-4.8.0b2/tests/test_context_manager.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/_configuration.py
+Filename: azure-keyvault-certificates-4.8.0b2/tests/certs.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b2/tests/_test_case.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/_key_vault_client.py
+Filename: azure-keyvault-certificates-4.8.0b2/tests/test_examples_certificates_async.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b2/tests/test_certificates_client.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/_vendor.py
+Filename: azure-keyvault-certificates-4.8.0b2/tests/_async_test_case.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/_key_vault_client_operations.py
+Filename: azure-keyvault-certificates-4.8.0b2/tests/test_certificates_client_async.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b2/tests/conftest.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b2/tests/test_parse_id.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/aio/_operations_mixin.py
+Filename: azure-keyvault-certificates-4.8.0b2/tests/test_merge_certificate.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/aio/_configuration.py
+Filename: azure-keyvault-certificates-4.8.0b2/tests/test_multi_api.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/aio/_key_vault_client.py
+Filename: azure-keyvault-certificates-4.8.0b2/tests/test_examples_certificates.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/aio/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b2/tests/test_merge_certificate_async.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/operations/
+Filename: azure-keyvault-certificates-4.8.0b2/tests/perfstress_tests/get_certificate.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/models/
+Filename: azure-keyvault-certificates-4.8.0b2/tests/perfstress_tests/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/
+Filename: azure-keyvault-certificates-4.8.0b2/tests/_shared/test_case_async.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/_configuration.py
+Filename: azure-keyvault-certificates-4.8.0b2/tests/_shared/preparer.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b2/tests/_shared/__init__.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/_key_vault_client.py
+Filename: azure-keyvault-certificates-4.8.0b2/tests/_shared/preparer_async.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b2/tests/_shared/helpers.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/_vendor.py
+Filename: azure-keyvault-certificates-4.8.0b2/tests/_shared/helpers_async.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/operations/_key_vault_client_operations.py
+Filename: azure-keyvault-certificates-4.8.0b2/tests/_shared/test_case.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/operations/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b2/tests/_shared/json_attribute_matcher.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/operations/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b2/samples/hello_world.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/models/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b2/samples/hello_world_async.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/models/_key_vault_client_enums.py
+Filename: azure-keyvault-certificates-4.8.0b2/samples/issuers_async.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/models/_models_py3.py
+Filename: azure-keyvault-certificates-4.8.0b2/samples/recover_purge_operations_async.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/models/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b2/samples/import_certificate_async.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/operations/
+Filename: azure-keyvault-certificates-4.8.0b2/samples/parse_certificate_async.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/_configuration.py
+Filename: azure-keyvault-certificates-4.8.0b2/samples/parse_certificate.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b2/samples/backup_restore_operations_async.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/_key_vault_client.py
+Filename: azure-keyvault-certificates-4.8.0b2/samples/contacts.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b2/samples/contacts_async.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/_vendor.py
+Filename: azure-keyvault-certificates-4.8.0b2/samples/list_operations.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/operations/_key_vault_client_operations.py
+Filename: azure-keyvault-certificates-4.8.0b2/samples/list_operations_async.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/operations/_patch.py
+Filename: azure-keyvault-certificates-4.8.0b2/samples/issuers.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/operations/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b2/samples/backup_restore_operations.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/aio/_client.py
+Filename: azure-keyvault-certificates-4.8.0b2/samples/import_certificate.py
 Comment: 
 
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/aio/_polling_async.py
-Comment: 
-
-Filename: azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/aio/__init__.py
+Filename: azure-keyvault-certificates-4.8.0b2/samples/recover_purge_operations.py
 Comment: 
 
 Zip file comment:
```

## Comparing `azure-keyvault-certificates-4.8.0b1/PKG-INFO` & `azure-keyvault-certificates-4.8.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-keyvault-certificates
-Version: 4.8.0b1
+Version: 4.8.0b2
 Summary: Microsoft Azure Key Vault Certificates Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/keyvault/azure-keyvault-certificates
 Author: Microsoft Corporation
 Author-email: azurekeyvault@microsoft.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -414,14 +414,20 @@
 [soft_delete]: https://docs.microsoft.com/azure/key-vault/general/soft-delete-overview
 
 ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fsdk%2Fkeyvault%2Fazure-keyvault-certificates%2FREADME.png)
 
 
 # Release History
 
+## 4.8.0b2 (2023-07-11)
+
+### Features Added
+- Added `CertificateProperties.x509_thumbprint_string` to return the hexadecimal string representation of the SHA-1 hash
+  of the certificate ([#30166](https://github.com/Azure/azure-sdk-for-python/issues/30166))
+
 ## 4.8.0b1 (2023-05-16)
 
 ### Bugs Fixed
 - Token requests made during AD FS authentication no longer specify an erroneous "adfs" tenant ID
   ([#29888](https://github.com/Azure/azure-sdk-for-python/issues/29888))
 
 ## 4.7.0 (2023-03-16)
```

## Comparing `azure-keyvault-certificates-4.8.0b1/README.md` & `azure-keyvault-certificates-4.8.0b2/README.md`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/CHANGELOG.md` & `azure-keyvault-certificates-4.8.0b2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Release History
 
+## 4.8.0b2 (2023-07-11)
+
+### Features Added
+- Added `CertificateProperties.x509_thumbprint_string` to return the hexadecimal string representation of the SHA-1 hash
+  of the certificate ([#30166](https://github.com/Azure/azure-sdk-for-python/issues/30166))
+
 ## 4.8.0b1 (2023-05-16)
 
 ### Bugs Fixed
 - Token requests made during AD FS authentication no longer specify an erroneous "adfs" tenant ID
   ([#29888](https://github.com/Azure/azure-sdk-for-python/issues/29888))
 
 ## 4.7.0 (2023-03-16)
```

## Comparing `azure-keyvault-certificates-4.8.0b1/setup.py` & `azure-keyvault-certificates-4.8.0b2/setup.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/LICENSE` & `azure-keyvault-certificates-4.8.0b2/LICENSE`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/migration_guide.md` & `azure-keyvault-certificates-4.8.0b2/migration_guide.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 # Guide for migrating to azure-keyvault-certificates from azure-keyvault
 
-This guide is intended to assist in the migration to `azure-keyvault-certificates` from `azure-keyvault`. It will focus on side-by-side comparisons for similar operations between the two packages.
+This guide is intended to assist in the migration to `azure-keyvault-certificates` from the [deprecated] `azure-keyvault` library. It will focus on side-by-side comparisons for similar operations between the two packages.
 
 Familiarity with the `azure-keyvault` package is assumed. For those new to the Key Vault client library for Python, please refer to the [README for `azure-keyvault-certificates`](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/keyvault/azure-keyvault-certificates/README.md) rather than this guide.
 
 ## Table of contents
 
-* [Migration benefits](#migration-benefits)
-* [Important changes](#important-changes)
+- [Migration benefits](#migration-benefits)
+- [Important changes](#important-changes)
     - [Separate packages and clients](#separate-packages-and-clients)
     - [Client constructors](#client-constructors)
     - [Async operations](#async-operations)
     - [Create a certificate](#create-a-certificate)
     - [Retrieve a certificate](#retrieve-a-certificate)
     - [List properties of certificates](#list-properties-of-certificates)
     - [Delete a certificate](#delete-a-certificate)
-* [Additional samples](#additional-samples)
+- [Additional samples](#additional-samples)
+- [Support](#support)
 
 ## Migration benefits
 
+> Note: `azure-keyvault` has been [deprecated]. Please upgrade to `azure-keyvault-certificates` for continued support.
+
 A natural question to ask when considering whether or not to adopt a new version or library is what the benefits of doing so would be. As Azure has matured and been embraced by a more diverse group of developers, we have been focused on learning the patterns and practices to best support developer productivity and to understand the gaps that the Python client libraries have.
 
 There were several areas of consistent feedback expressed across the Azure client library ecosystem. One of the most important is that the client libraries for different Azure services have not had a consistent approach to organization, naming, and API structure. Additionally, many developers have felt that the learning curve was difficult, and the APIs did not offer a good, approachable, and consistent onboarding story for those learning Azure or exploring a specific Azure service.
 
-To try and improve the development experience across Azure services, a set of uniform [design guidelines](https://azure.github.io/azure-sdk/python/guidelines/index.html) was created for all languages to drive a consistent experience with established API patterns for all services. A set of [Python-specific guidelines](https://azure.github.io/azure-sdk/python_design.html) was also introduced to ensure that Python clients have a natural and idiomatic feel with respect to the Python ecosystem. Further details are available in the guidelines for those interested.
+To try and improve the development experience across Azure services, a set of uniform [design guidelines](https://azure.github.io/azure-sdk/general_introduction.html) was created for all languages to drive a consistent experience with established API patterns for all services. A set of [Python-specific guidelines](https://azure.github.io/azure-sdk/python_design.html) was also introduced to ensure that Python clients have a natural and idiomatic feel with respect to the Python ecosystem. Further details are available in the guidelines for those interested.
 
 ### Cross Service SDK improvements
 
 The modern Key Vault client library also provides the ability to share in some of the cross-service improvements made to the Azure development experience, such as
 - using the new [`azure-identity`](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/identity/azure-identity/README.md) library to share a single authentication approach between clients
 - a unified logging and diagnostics pipeline offering a common view of the activities across each of the client libraries
 
@@ -209,7 +212,16 @@
 certificate_client.purge_deleted_certificate(certificate_name="cert-name")
 ```
 
 ## Additional samples
 
 * [Key Vault certificates samples for Python](https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/keyvault/azure-keyvault-certificates/samples)
 * [General Key Vault samples for Python](https://docs.microsoft.com/samples/browse/?products=azure-key-vault&languages=python)
+
+## Support
+
+If you have migrated your code base and are experiencing errors, see our [troubleshooting guide](https://github.com/Azure/azure-sdk-for-python/blob/main/sdk/keyvault/azure-keyvault-certificates/TROUBLESHOOTING.md).
+For additional support, please search our [existing issues](https://github.com/Azure/azure-sdk-for-python/issues) or [open a new issue](https://github.com/Azure/azure-sdk-for-python/issues/new/choose).
+You may also find existing answers on community sites like [Stack Overflow](https://stackoverflow.com/questions/tagged/azure-keyvault+python).
+
+
+[deprecated]: https://aka.ms/azsdk/deprecated
```

## Comparing `azure-keyvault-certificates-4.8.0b1/samples/import_certificate.py` & `azure-keyvault-certificates-4.8.0b2/samples/import_certificate.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/samples/contacts_async.py` & `azure-keyvault-certificates-4.8.0b2/samples/contacts_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/samples/import_certificate_async.py` & `azure-keyvault-certificates-4.8.0b2/samples/import_certificate_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/samples/recover_purge_operations_async.py` & `azure-keyvault-certificates-4.8.0b2/samples/recover_purge_operations_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/samples/parse_certificate.py` & `azure-keyvault-certificates-4.8.0b2/samples/parse_certificate.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/samples/parse_certificate_async.py` & `azure-keyvault-certificates-4.8.0b2/samples/parse_certificate_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/samples/issuers.py` & `azure-keyvault-certificates-4.8.0b2/samples/issuers.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/samples/backup_restore_operations_async.py` & `azure-keyvault-certificates-4.8.0b2/samples/backup_restore_operations_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/samples/list_operations_async.py` & `azure-keyvault-certificates-4.8.0b2/samples/list_operations_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/samples/hello_world_async.py` & `azure-keyvault-certificates-4.8.0b2/samples/hello_world_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/samples/contacts.py` & `azure-keyvault-certificates-4.8.0b2/samples/contacts.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/samples/recover_purge_operations.py` & `azure-keyvault-certificates-4.8.0b2/samples/recover_purge_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/samples/issuers_async.py` & `azure-keyvault-certificates-4.8.0b2/samples/issuers_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/samples/list_operations.py` & `azure-keyvault-certificates-4.8.0b2/samples/list_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/samples/backup_restore_operations.py` & `azure-keyvault-certificates-4.8.0b2/samples/backup_restore_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/samples/hello_world.py` & `azure-keyvault-certificates-4.8.0b2/samples/hello_world.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure_keyvault_certificates.egg-info/PKG-INFO` & `azure-keyvault-certificates-4.8.0b2/azure_keyvault_certificates.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-keyvault-certificates
-Version: 4.8.0b1
+Version: 4.8.0b2
 Summary: Microsoft Azure Key Vault Certificates Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/keyvault/azure-keyvault-certificates
 Author: Microsoft Corporation
 Author-email: azurekeyvault@microsoft.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -414,14 +414,20 @@
 [soft_delete]: https://docs.microsoft.com/azure/key-vault/general/soft-delete-overview
 
 ![Impressions](https://azure-sdk-impressions.azurewebsites.net/api/impressions/azure-sdk-for-python%2Fsdk%2Fkeyvault%2Fazure-keyvault-certificates%2FREADME.png)
 
 
 # Release History
 
+## 4.8.0b2 (2023-07-11)
+
+### Features Added
+- Added `CertificateProperties.x509_thumbprint_string` to return the hexadecimal string representation of the SHA-1 hash
+  of the certificate ([#30166](https://github.com/Azure/azure-sdk-for-python/issues/30166))
+
 ## 4.8.0b1 (2023-05-16)
 
 ### Bugs Fixed
 - Token requests made during AD FS authentication no longer specify an erroneous "adfs" tenant ID
   ([#29888](https://github.com/Azure/azure-sdk-for-python/issues/29888))
 
 ## 4.7.0 (2023-03-16)
```

## Comparing `azure-keyvault-certificates-4.8.0b1/azure_keyvault_certificates.egg-info/SOURCES.txt` & `azure-keyvault-certificates-4.8.0b2/azure_keyvault_certificates.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,14 @@
 azure/keyvault/certificates/_shared/__init__.py
 azure/keyvault/certificates/_shared/_polling.py
 azure/keyvault/certificates/_shared/_polling_async.py
 azure/keyvault/certificates/_shared/async_challenge_auth_policy.py
 azure/keyvault/certificates/_shared/async_client_base.py
 azure/keyvault/certificates/_shared/challenge_auth_policy.py
 azure/keyvault/certificates/_shared/client_base.py
-azure/keyvault/certificates/_shared/exceptions.py
 azure/keyvault/certificates/_shared/http_challenge.py
 azure/keyvault/certificates/_shared/http_challenge_cache.py
 azure/keyvault/certificates/aio/__init__.py
 azure/keyvault/certificates/aio/_client.py
 azure/keyvault/certificates/aio/_polling_async.py
 azure_keyvault_certificates.egg-info/PKG-INFO
 azure_keyvault_certificates.egg-info/SOURCES.txt
```

## Comparing `azure-keyvault-certificates-4.8.0b1/tests/_async_test_case.py` & `azure-keyvault-certificates-4.8.0b2/tests/_async_test_case.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/tests/test_certificates_client_async.py` & `azure-keyvault-certificates-4.8.0b2/tests/test_certificates_client_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 # ------------------------------------
 import asyncio
 import functools
 import logging
 import json
+from unittest.mock import Mock, patch
 
-from azure.core.exceptions import ResourceExistsError
+from azure.core.exceptions import ResourceExistsError, ResourceNotFoundError
 from azure.core.pipeline.policies import SansIOHTTPPolicy
 from azure_devtools.scenario_tests import RecordingProcessor
 from devtools_testutils import set_bodiless_matcher
 from devtools_testutils.aio import recorded_by_proxy_async
 from azure.keyvault.certificates import (
     AdministratorContact,
     ApiVersion,
@@ -26,26 +27,28 @@
     LifetimeAction,
     CertificateIssuer,
     IssuerProperties,
     WellKnownIssuerNames
 )
 from azure.keyvault.certificates.aio import CertificateClient
 from azure.keyvault.certificates._client import NO_SAN_OR_SUBJECT
+from azure.keyvault.certificates._shared.client_base import DEFAULT_VERSION
 import pytest
 
 from _shared.test_case_async import KeyVaultTestCase
 from _async_test_case import get_decorator, AsyncCertificatesClientPreparer
 from certs import CERT_CONTENT_PASSWORD_ENCODED, CERT_CONTENT_NOT_PASSWORD_ENCODED
 
 
-all_api_versions = get_decorator(is_async=True)
-logging_enabled = get_decorator(is_async=True, logging_enable=True)
-logging_disabled = get_decorator(is_async=True, logging_enable=False)
-exclude_2016_10_01 = get_decorator(is_async=True, api_versions=[v for v in ApiVersion if v != ApiVersion.V2016_10_01])
-only_2016_10_01 = get_decorator(is_async=True, api_versions=[ApiVersion.V2016_10_01])
+all_api_versions = get_decorator()
+only_latest = get_decorator(api_versions=[DEFAULT_VERSION])
+logging_enabled = get_decorator(logging_enable=True)
+logging_disabled = get_decorator(logging_enable=False)
+exclude_2016_10_01 = get_decorator(api_versions=[v for v in ApiVersion if v != ApiVersion.V2016_10_01])
+only_2016_10_01 = get_decorator(api_versions=[ApiVersion.V2016_10_01])
 LIST_TEST_SIZE = 7
 
 
 class RetryAfterReplacer(RecordingProcessor):
     """Replace the retry after wait time in the replay process to 0."""
 
     def process_response(self, response):
@@ -746,14 +749,33 @@
         with pytest.raises(NotImplementedError) as excinfo:
             certs = client.list_deleted_certificates(include_pending=True)
             async for cert in certs:
                 pass
 
         assert "The 'include_pending' parameter to `list_deleted_certificates` is only available for API versions v7.0 and up" in str(excinfo.value)
 
+    @pytest.mark.asyncio
+    @pytest.mark.parametrize("api_version", only_latest)
+    @AsyncCertificatesClientPreparer()
+    @recorded_by_proxy_async
+    async def test_40x_handling(self, client, **kwargs):
+        """Ensure 404 and 409 responses are raised with azure-core exceptions instead of generated KV ones"""
+
+        # Test that 404 is raised correctly by fetching a nonexistent cert
+        with pytest.raises(ResourceNotFoundError):
+            await client.get_certificate("cert-that-does-not-exist")
+
+        # 409 is raised correctly (`create_certificate` shouldn't actually trigger this, but for raising behavior)
+        async def run(*_, **__):
+            return Mock(http_response=Mock(status_code=409))
+        with patch.object(client._client._client._pipeline, "run", run):
+            with pytest.raises(ResourceExistsError):
+                await client.create_certificate("...", CertificatePolicy.get_default())
+        await client.close()
+
 
 @pytest.mark.asyncio
 async def test_policy_expected_errors_for_create_cert():
     """Either a subject or subject alternative name property are required for creating a certificate"""
     client = CertificateClient("...", object())
 
     with pytest.raises(ValueError, match=NO_SAN_OR_SUBJECT):
```

## Comparing `azure-keyvault-certificates-4.8.0b1/tests/test_merge_certificate_async.py` & `azure-keyvault-certificates-4.8.0b2/tests/test_merge_certificate_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/tests/_test_case.py` & `azure-keyvault-certificates-4.8.0b2/tests/_test_case.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/tests/test_multi_api.py` & `azure-keyvault-certificates-4.8.0b2/tests/test_multi_api.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/tests/test_merge_certificate.py` & `azure-keyvault-certificates-4.8.0b2/tests/test_merge_certificate.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/tests/test_parse_id.py` & `azure-keyvault-certificates-4.8.0b2/tests/test_parse_id.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/tests/conftest.py` & `azure-keyvault-certificates-4.8.0b2/tests/conftest.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/tests/test_examples_certificates.py` & `azure-keyvault-certificates-4.8.0b2/tests/test_examples_certificates.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/tests/test_context_manager_async.py` & `azure-keyvault-certificates-4.8.0b2/tests/test_context_manager_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/tests/test_examples_certificates_async.py` & `azure-keyvault-certificates-4.8.0b2/tests/test_examples_certificates_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/tests/certs.py` & `azure-keyvault-certificates-4.8.0b2/tests/certs.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/tests/test_certificates_client.py` & `azure-keyvault-certificates-4.8.0b2/tests/test_certificates_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,45 +2,49 @@
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 # ------------------------------------
 import functools
 import json
 import logging
 import time
+from unittest.mock import Mock, patch
 
-from azure.core.exceptions import ResourceExistsError
+from azure.core.exceptions import ResourceExistsError, ResourceNotFoundError
 from azure.core.pipeline.policies import SansIOHTTPPolicy
 from azure_devtools.scenario_tests import RecordingProcessor
 from devtools_testutils import recorded_by_proxy
 from azure.keyvault.certificates import (
     AdministratorContact,
     ApiVersion,
     CertificateClient,
     CertificateContact,
     CertificatePolicyAction,
     CertificatePolicy,
+    CertificateProperties,
     KeyType,
     KeyCurveName,
     KeyUsageType,
     KeyVaultCertificateIdentifier,
     CertificateContentType,
     LifetimeAction,
     CertificateIssuer,
     IssuerProperties,
     WellKnownIssuerNames
 )
 from azure.keyvault.certificates._client import NO_SAN_OR_SUBJECT
+from azure.keyvault.certificates._shared.client_base import DEFAULT_VERSION
 import pytest
 
 from _shared.test_case import KeyVaultTestCase
 from _test_case import get_decorator, CertificatesClientPreparer
 from certs import CERT_CONTENT_PASSWORD_ENCODED, CERT_CONTENT_NOT_PASSWORD_ENCODED
 
 
 all_api_versions = get_decorator()
+only_latest = get_decorator(api_versions=[DEFAULT_VERSION])
 logging_enabled = get_decorator(logging_enable=True)
 logging_disabled = get_decorator(logging_enable=False)
 exclude_2016_10_01 = get_decorator(api_versions=[v for v in ApiVersion if v != ApiVersion.V2016_10_01])
 only_2016_10_01 = get_decorator(api_versions=[ApiVersion.V2016_10_01])
 LIST_TEST_SIZE = 7
 
 
@@ -718,14 +722,31 @@
         [_ for _ in client.list_deleted_certificates()]
 
         with pytest.raises(NotImplementedError) as excinfo:
             [_ for _ in client.list_deleted_certificates(include_pending=True)]
 
         assert "The 'include_pending' parameter to `list_deleted_certificates` is only available for API versions v7.0 and up" in str(excinfo.value)
 
+    @pytest.mark.parametrize("api_version", only_latest)
+    @CertificatesClientPreparer()
+    @recorded_by_proxy
+    def test_40x_handling(self, client, **kwargs):
+        """Ensure 404 and 409 responses are raised with azure-core exceptions instead of generated KV ones"""
+
+        # Test that 404 is raised correctly by fetching a nonexistent cert
+        with pytest.raises(ResourceNotFoundError):
+            client.get_certificate("cert-that-does-not-exist")
+
+        # 409 is raised correctly (`begin_create_certificate` shouldn't actually trigger this, but for raising behavior)
+        def run(*_, **__):
+            return Mock(http_response=Mock(status_code=409))
+        with patch.object(client._client._client._pipeline, "run", run):
+            with pytest.raises(ResourceExistsError):
+                client.begin_create_certificate("...", CertificatePolicy.get_default())
+
 
 def test_policy_expected_errors_for_create_cert():
     """Either a subject or subject alternative name property are required for creating a certificate"""
     client = CertificateClient("...", object())
 
     with pytest.raises(ValueError, match=NO_SAN_OR_SUBJECT):
         policy = CertificatePolicy()
@@ -756,7 +777,16 @@
     """
     # KeyType with all upper-case value
     assert KeyType("rsa") == KeyType.rsa
     # KeyType with all lower-case value
     assert KeyType("OCT") == KeyType.oct
     # KeyType with mixed-case value
     assert KeyType("oct-hsm") == KeyType.oct_hsm
+
+
+def test_thumbprint_hex():
+    """Ensure the `CertificateProperties.x509_thumbprint_string` property correctly converts a thumbprint to hex."""
+    properties = CertificateProperties(
+        cert_id="https://vaultname.vault.azure.net/certificates/certname/version",
+        x509_thumbprint=b"v\xe1\x81\x9f\xad\xf0jU\xefK\x12j.\xf7C\xc2\xba\xe8\xa1Q",
+    )
+    assert properties.x509_thumbprint_string == "76E1819FADF06A55EF4B126A2EF743C2BAE8A151"
```

## Comparing `azure-keyvault-certificates-4.8.0b1/tests/test_context_manager.py` & `azure-keyvault-certificates-4.8.0b2/tests/test_context_manager.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/tests/_shared/helpers.py` & `azure-keyvault-certificates-4.8.0b2/tests/_shared/helpers.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/tests/_shared/json_attribute_matcher.py` & `azure-keyvault-certificates-4.8.0b2/tests/_shared/json_attribute_matcher.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/tests/_shared/helpers_async.py` & `azure-keyvault-certificates-4.8.0b2/tests/_shared/helpers_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/tests/_shared/preparer.py` & `azure-keyvault-certificates-4.8.0b2/tests/_shared/preparer.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/tests/_shared/test_case_async.py` & `azure-keyvault-certificates-4.8.0b2/tests/_shared/test_case_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/tests/_shared/test_case.py` & `azure-keyvault-certificates-4.8.0b2/tests/_shared/test_case.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/tests/_shared/preparer_async.py` & `azure-keyvault-certificates-4.8.0b2/tests/_shared/preparer_async.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/tests/perfstress_tests/get_certificate.py` & `azure-keyvault-certificates-4.8.0b2/tests/perfstress_tests/get_certificate.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_client.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,34 @@
 # ------------------------------------
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 # ------------------------------------
-# pylint:disable=too-many-lines,too-many-public-methods
+# pylint:disable=too-many-lines,too-many-public-methods,bad-option-value,delete-operation-wrong-return-type
 import base64
 from functools import partial
+from typing import Any, List, Optional, Union
 
 from azure.core.polling import LROPoller
+from azure.core.paging import ItemPaged
 from azure.core.tracing.decorator import distributed_trace
 
 from ._shared import KeyVaultClientBase
-from ._shared.exceptions import error_map as _error_map
 from ._shared._polling import DeleteRecoverPollingMethod, KeyVaultOperationPoller
 from ._models import (
     KeyVaultCertificate,
     CertificateProperties,
     CertificatePolicy,
     DeletedCertificate,
     CertificateIssuer,
     IssuerProperties,
     CertificateContact,
     CertificateOperation,
 )
 from ._polling import CreateCertificatePoller
 
-try:
-    from typing import TYPE_CHECKING
-except ImportError:
-    TYPE_CHECKING = False
-
-if TYPE_CHECKING:
-    # pylint:disable=unused-import
-    from typing import Any, List, Optional, Union
-    from azure.core.paging import ItemPaged
-
 
 NO_SAN_OR_SUBJECT = "You need to set either subject or one of the subject alternative names parameters in the policy"
 
 
 class CertificateClient(KeyVaultClientBase):
     """A high-level interface for managing a vault's certificates.
 
@@ -63,15 +54,15 @@
     """
 
     # pylint:disable=protected-access
 
     @distributed_trace
     def begin_create_certificate(
         self, certificate_name: str, policy: CertificatePolicy, **kwargs
-    ) -> "LROPoller[Union[KeyVaultCertificate, CertificateOperation]]":
+    ) -> LROPoller[Union[KeyVaultCertificate, CertificateOperation]]:
         """Creates a new certificate.
 
         If this is the first version, the certificate resource is created. This operation requires the
         certificates/create permission. Waiting on the returned poller requires the certificates/get permission and
         gives you the certificate if creation is successful, or the CertificateOperation if not -- otherwise, it raises
         an :class:`~azure.core.exceptions.HttpResponseError`.
 
@@ -120,28 +111,29 @@
             tags=kwargs.pop("tags", None),
         )
 
         cert_bundle = self._client.create_certificate(
             vault_base_url=self.vault_url,
             certificate_name=certificate_name,
             parameters=parameters,
-            error_map=_error_map,
             **kwargs
         )
 
         create_certificate_operation = CertificateOperation._from_certificate_operation_bundle(cert_bundle)
 
         command = partial(self.get_certificate_operation, certificate_name=certificate_name, **kwargs)
 
         get_certificate_command = partial(self.get_certificate, certificate_name=certificate_name, **kwargs)
 
         create_certificate_polling = CreateCertificatePoller(
             get_certificate_command=get_certificate_command, interval=polling_interval
         )
-        return LROPoller(command, create_certificate_operation, lambda *_: None, create_certificate_polling)
+        def no_op(*_, **__) -> Any:  # The deserialization callback is ignored based on polling implementation
+            pass
+        return LROPoller(command, create_certificate_operation, no_op, create_certificate_polling)
 
     @distributed_trace
     def get_certificate(self, certificate_name: str, **kwargs) -> KeyVaultCertificate:
         """Gets a certificate with its management policy attached. Requires certificates/get permission.
 
         Does not accept the version of the certificate as a parameter. To get a specific version of the
         certificate, call :func:`get_certificate_version`.
@@ -163,15 +155,14 @@
                 :caption: Get a certificate
                 :dedent: 8
         """
         bundle = self._client.get_certificate(
             vault_base_url=self.vault_url,
             certificate_name=certificate_name,
             certificate_version="",
-            error_map=_error_map,
             **kwargs
         )
         return KeyVaultCertificate._from_certificate_bundle(certificate_bundle=bundle)
 
     @distributed_trace
     def get_certificate_version(
         self, certificate_name: str, version: str, **kwargs
@@ -199,15 +190,14 @@
                 :caption: Get a certificate with a specific version
                 :dedent: 8
         """
         bundle = self._client.get_certificate(
             vault_base_url=self.vault_url,
             certificate_name=certificate_name,
             certificate_version=version,
-            error_map=_error_map,
             **kwargs
         )
         return KeyVaultCertificate._from_certificate_bundle(certificate_bundle=bundle)
 
     @distributed_trace
     def begin_delete_certificate(self, certificate_name: str, **kwargs) -> LROPoller[DeletedCertificate]:
         """Delete all versions of a certificate. Requires certificates/delete permission.
@@ -237,15 +227,15 @@
                 :caption: Delete a certificate
                 :dedent: 8
         """
         polling_interval = kwargs.pop("_polling_interval", None)
         if polling_interval is None:
             polling_interval = 2
         deleted_cert_bundle = self._client.delete_certificate(
-            vault_base_url=self.vault_url, certificate_name=certificate_name, error_map=_error_map, **kwargs
+            vault_base_url=self.vault_url, certificate_name=certificate_name, **kwargs
         )
         deleted_cert = DeletedCertificate._from_deleted_certificate_bundle(deleted_cert_bundle)
 
         polling_method = DeleteRecoverPollingMethod(
             # no recovery ID means soft-delete is disabled, in which case we initialize the poller as finished
             finished=deleted_cert.recovery_id is None,
             command=partial(self.get_deleted_certificate, certificate_name=certificate_name, **kwargs),
@@ -276,15 +266,15 @@
                 :start-after: [START get_deleted_certificate]
                 :end-before: [END get_deleted_certificate]
                 :language: python
                 :caption: Get a deleted certificate
                 :dedent: 8
         """
         bundle = self._client.get_deleted_certificate(
-            vault_base_url=self.vault_url, certificate_name=certificate_name, error_map=_error_map, **kwargs
+            vault_base_url=self.vault_url, certificate_name=certificate_name, **kwargs
         )
         return DeletedCertificate._from_deleted_certificate_bundle(deleted_certificate_bundle=bundle)
 
     @distributed_trace
     def purge_deleted_certificate(self, certificate_name: str, **kwargs) -> None:
         """Permanently deletes a deleted certificate. Possible only in vaults with soft-delete enabled.
 
@@ -298,15 +288,15 @@
 
         :return: None
         :rtype: None
 
         :raises: :class:`~azure.core.exceptions.HttpResponseError`
         """
         self._client.purge_deleted_certificate(
-            vault_base_url=self.vault_url, certificate_name=certificate_name, error_map=_error_map, **kwargs
+            vault_base_url=self.vault_url, certificate_name=certificate_name, **kwargs
         )
 
     @distributed_trace
     def begin_recover_deleted_certificate(
         self, certificate_name: str, **kwargs
     ) -> LROPoller[KeyVaultCertificate]:
         """Recover a deleted certificate to its latest version. Possible only in a vault with soft-delete enabled.
@@ -335,15 +325,15 @@
                 :dedent: 8
         """
         polling_interval = kwargs.pop("_polling_interval", None)
         if polling_interval is None:
             polling_interval = 2
 
         recovered_cert_bundle = self._client.recover_deleted_certificate(
-            vault_base_url=self.vault_url, certificate_name=certificate_name, error_map=_error_map, **kwargs
+            vault_base_url=self.vault_url, certificate_name=certificate_name, **kwargs
         )
         recovered_certificate = KeyVaultCertificate._from_certificate_bundle(recovered_cert_bundle)
         command = partial(self.get_certificate, certificate_name=certificate_name, **kwargs)
         polling_method = DeleteRecoverPollingMethod(
             finished=False, command=command, final_resource=recovered_certificate, interval=polling_interval
         )
 
@@ -398,15 +388,14 @@
             tags=kwargs.pop("tags", None),
         )
 
         bundle = self._client.import_certificate(
             vault_base_url=self.vault_url,
             certificate_name=certificate_name,
             parameters=parameters,
-            error_map=_error_map,
             **kwargs
         )
         return KeyVaultCertificate._from_certificate_bundle(certificate_bundle=bundle)
 
     @distributed_trace
     def get_certificate_policy(self, certificate_name: str, **kwargs) -> CertificatePolicy:
         """Gets the policy for a certificate. Requires certificates/get permission.
@@ -417,15 +406,15 @@
 
         :return: The certificate policy
         :rtype: ~azure.keyvault.certificates.CertificatePolicy
 
         :raises: :class:`~azure.core.exceptions.HttpResponseError`
         """
         bundle = self._client.get_certificate_policy(
-            vault_base_url=self.vault_url, certificate_name=certificate_name, error_map=_error_map, **kwargs
+            vault_base_url=self.vault_url, certificate_name=certificate_name, **kwargs
         )
         return CertificatePolicy._from_certificate_policy_bundle(certificate_policy_bundle=bundle)
 
     @distributed_trace
     def update_certificate_policy(
         self, certificate_name: str, policy: CertificatePolicy, **kwargs
     ) -> CertificatePolicy:
@@ -442,15 +431,14 @@
 
         :raises: :class:`~azure.core.exceptions.HttpResponseError`
         """
         bundle = self._client.update_certificate_policy(
             vault_base_url=self.vault_url,
             certificate_name=certificate_name,
             certificate_policy=policy._to_certificate_policy_bundle(),
-            error_map=_error_map,
             **kwargs
         )
         return CertificatePolicy._from_certificate_policy_bundle(certificate_policy_bundle=bundle)
 
     @distributed_trace
     def update_certificate_properties(
         self, certificate_name: str, version: "Optional[str]" = None, **kwargs
@@ -490,15 +478,14 @@
         )
 
         bundle = self._client.update_certificate(
             vault_base_url=self.vault_url,
             certificate_name=certificate_name,
             certificate_version=version or "",
             parameters=parameters,
-            error_map=_error_map,
             **kwargs
         )
         return KeyVaultCertificate._from_certificate_bundle(certificate_bundle=bundle)
 
     @distributed_trace
     def backup_certificate(self, certificate_name: str, **kwargs) -> bytes:
         """Back up a certificate in a protected form useable only by Azure Key Vault.
@@ -522,15 +509,15 @@
                 :start-after: [START backup_certificate]
                 :end-before: [END backup_certificate]
                 :language: python
                 :caption: Get a certificate backup
                 :dedent: 8
         """
         backup_result = self._client.backup_certificate(
-            vault_base_url=self.vault_url, certificate_name=certificate_name, error_map=_error_map, **kwargs
+            vault_base_url=self.vault_url, certificate_name=certificate_name, **kwargs
         )
         return backup_result.value
 
     @distributed_trace
     def restore_certificate_backup(self, backup: bytes, **kwargs) -> KeyVaultCertificate:
         """Restore a certificate backup to the vault. Requires certificates/restore permission.
 
@@ -552,21 +539,20 @@
                 :language: python
                 :caption: Restore a certificate backup
                 :dedent: 8
         """
         bundle = self._client.restore_certificate(
             vault_base_url=self.vault_url,
             parameters=self._models.CertificateRestoreParameters(certificate_bundle_backup=backup),
-            error_map=_error_map,
             **kwargs
         )
         return KeyVaultCertificate._from_certificate_bundle(certificate_bundle=bundle)
 
     @distributed_trace
-    def list_deleted_certificates(self, **kwargs) -> "ItemPaged[DeletedCertificate]":
+    def list_deleted_certificates(self, **kwargs) -> ItemPaged[DeletedCertificate]:
         """Lists the currently-recoverable deleted certificates. Possible only if vault is soft-delete enabled.
 
         Requires certificates/get/list permission. Retrieves the certificates in the current vault which are in a
         deleted state and ready for recovery or purging. This operation includes deletion-specific information.
 
         :keyword bool include_pending: Specifies whether to include certificates which are not completely deleted.
             Only available for API versions v7.0 and up.
@@ -593,20 +579,19 @@
             )
         return self._client.get_deleted_certificates(
             vault_base_url=self._vault_url,
             maxresults=max_page_size,
             cls=lambda objs: [
                 DeletedCertificate._from_deleted_certificate_item(deleted_certificate_item=x) for x in objs
             ],
-            error_map=_error_map,
             **kwargs
         )
 
     @distributed_trace
-    def list_properties_of_certificates(self, **kwargs) -> "ItemPaged[CertificateProperties]":
+    def list_properties_of_certificates(self, **kwargs) -> ItemPaged[CertificateProperties]:
         """List identifiers and properties of all certificates in the vault.
 
         Requires certificates/list permission.
 
         :keyword bool include_pending: Specifies whether to include certificates which are not completely provisioned.
             Only available for API versions v7.0 and up.
 
@@ -631,22 +616,21 @@
                 "is only available for API versions v7.0 and up"
             )
 
         return self._client.get_certificates(
             vault_base_url=self._vault_url,
             maxresults=max_page_size,
             cls=lambda objs: [CertificateProperties._from_certificate_item(certificate_item=x) for x in objs],
-            error_map=_error_map,
             **kwargs
         )
 
     @distributed_trace
     def list_properties_of_certificate_versions(
         self, certificate_name: str, **kwargs
-    ) -> "ItemPaged[CertificateProperties]":
+    ) -> ItemPaged[CertificateProperties]:
         """List the identifiers and properties of a certificate's versions.
 
         Requires certificates/list permission.
 
         :param str certificate_name: The name of the certificate.
 
         :returns: An iterator-like instance of CertificateProperties
@@ -664,15 +648,14 @@
         """
         max_page_size = kwargs.pop("max_page_size", None)
         return self._client.get_certificate_versions(
             vault_base_url=self._vault_url,
             certificate_name=certificate_name,
             maxresults=max_page_size,
             cls=lambda objs: [CertificateProperties._from_certificate_item(certificate_item=x) for x in objs],
-            error_map=_error_map,
             **kwargs
         )
 
     @distributed_trace
     def set_contacts(self, contacts: "List[CertificateContact]", **kwargs) -> "List[CertificateContact]":
         """Sets the certificate contacts for the key vault. Requires certificates/managecontacts permission.
 
@@ -691,15 +674,14 @@
                 :language: python
                 :caption: Create contacts
                 :dedent: 8
         """
         new_contacts = self._client.set_certificate_contacts(
             vault_base_url=self.vault_url,
             contacts=self._models.Contacts(contact_list=[c._to_certificate_contacts_item() for c in contacts]),
-            error_map=_error_map,
             **kwargs
         )
         return [
             CertificateContact._from_certificate_contacts_item(contact_item=item) for item in new_contacts.contact_list
         ]
 
     @distributed_trace
@@ -715,15 +697,15 @@
             .. literalinclude:: ../tests/test_examples_certificates.py
                 :start-after: [START get_contacts]
                 :end-before: [END get_contacts]
                 :language: python
                 :caption: Get contacts
                 :dedent: 8
         """
-        contacts = self._client.get_certificate_contacts(vault_base_url=self._vault_url, error_map=_error_map, **kwargs)
+        contacts = self._client.get_certificate_contacts(vault_base_url=self._vault_url, **kwargs)
         return [CertificateContact._from_certificate_contacts_item(contact_item=item) for item in contacts.contact_list]
 
     @distributed_trace
     def delete_contacts(self, **kwargs) -> "List[CertificateContact]":
         """Deletes the certificate contacts for the key vault. Requires the certificates/managecontacts permission.
 
         :return: The deleted contacts for the key vault.
@@ -736,15 +718,15 @@
                 :start-after: [START delete_contacts]
                 :end-before: [END delete_contacts]
                 :language: python
                 :caption: Delete contacts
                 :dedent: 8
         """
         contacts = self._client.delete_certificate_contacts(
-            vault_base_url=self.vault_url, error_map=_error_map, **kwargs
+            vault_base_url=self.vault_url, **kwargs
         )
         return [CertificateContact._from_certificate_contacts_item(contact_item=item) for item in contacts.contact_list]
 
     @distributed_trace
     def get_certificate_operation(self, certificate_name: str, **kwargs) -> CertificateOperation:
         """Gets the creation operation of a certificate. Requires the certificates/get permission.
 
@@ -755,15 +737,15 @@
 
         :raises:
             :class:`~azure.core.exceptions.ResourceNotFoundError` if the certificate doesn't exist,
             :class:`~azure.core.exceptions.HttpResponseError` for other errors
         """
 
         bundle = self._client.get_certificate_operation(
-            vault_base_url=self.vault_url, certificate_name=certificate_name, error_map=_error_map, **kwargs
+            vault_base_url=self.vault_url, certificate_name=certificate_name, **kwargs
         )
         return CertificateOperation._from_certificate_operation_bundle(certificate_operation_bundle=bundle)
 
     @distributed_trace
     def delete_certificate_operation(self, certificate_name: str, **kwargs) -> CertificateOperation:
         """Deletes and stops the creation operation for a specific certificate.
 
@@ -773,15 +755,15 @@
 
         :return: The deleted CertificateOperation
         :rtype: ~azure.keyvault.certificates.CertificateOperation
 
         :raises: :class:`~azure.core.exceptions.HttpResponseError`
         """
         bundle = self._client.delete_certificate_operation(
-            vault_base_url=self.vault_url, certificate_name=certificate_name, error_map=_error_map, **kwargs
+            vault_base_url=self.vault_url, certificate_name=certificate_name, **kwargs
         )
         return CertificateOperation._from_certificate_operation_bundle(certificate_operation_bundle=bundle)
 
     @distributed_trace
     def cancel_certificate_operation(self, certificate_name: str, **kwargs) -> CertificateOperation:
         """Cancels an in-progress certificate operation. Requires the certificates/update permission.
 
@@ -792,15 +774,14 @@
 
         :raises: :class:`~azure.core.exceptions.HttpResponseError`
         """
         bundle = self._client.update_certificate_operation(
             vault_base_url=self.vault_url,
             certificate_name=certificate_name,
             certificate_operation=self._models.CertificateOperationUpdateParameter(cancellation_requested=True),
-            error_map=_error_map,
             **kwargs
         )
         return CertificateOperation._from_certificate_operation_bundle(certificate_operation_bundle=bundle)
 
     @distributed_trace
     def merge_certificate(
         self, certificate_name: str, x509_certificates: "List[bytes]", **kwargs
@@ -838,15 +819,14 @@
             x509_certificates=x509_certificates, certificate_attributes=attributes, tags=kwargs.pop("tags", None)
         )
 
         bundle = self._client.merge_certificate(
             vault_base_url=self.vault_url,
             certificate_name=certificate_name,
             parameters=parameters,
-            error_map=_error_map,
             **kwargs
         )
         return KeyVaultCertificate._from_certificate_bundle(certificate_bundle=bundle)
 
     @distributed_trace
     def get_issuer(self, issuer_name: str, **kwargs) -> CertificateIssuer:
         """Gets the specified certificate issuer. Requires certificates/manageissuers/getissuers permission.
@@ -865,15 +845,15 @@
                 :start-after: [START get_issuer]
                 :end-before: [END get_issuer]
                 :language: python
                 :caption: Get an issuer
                 :dedent: 8
         """
         issuer_bundle = self._client.get_certificate_issuer(
-            vault_base_url=self.vault_url, issuer_name=issuer_name, error_map=_error_map, **kwargs
+            vault_base_url=self.vault_url, issuer_name=issuer_name, **kwargs
         )
         return CertificateIssuer._from_issuer_bundle(issuer_bundle=issuer_bundle)
 
     @distributed_trace
     def create_issuer(self, issuer_name: str, provider: str, **kwargs) -> CertificateIssuer:
         """Sets the specified certificate issuer. Requires certificates/setissuers permission.
 
@@ -909,23 +889,23 @@
         admin_contacts = kwargs.pop("admin_contacts", None)
 
         if account_id or password:
             issuer_credentials = self._models.IssuerCredentials(account_id=account_id, password=password)
         else:
             issuer_credentials = None
         if admin_contacts:
-            admin_details = [
+            admin_details: Optional[List[Any]] = [
                 self._models.AdministratorDetails(
                     first_name=contact.first_name,
                     last_name=contact.last_name,
                     email_address=contact.email,
                     phone=contact.phone,
                 )
                 for contact in admin_contacts
-            ]  # type: Optional[List[Any]]
+            ]
         else:
             admin_details = None
         if organization_id or admin_details:
             organization_details = self._models.OrganizationDetails(id=organization_id, admin_details=admin_details)
         else:
             organization_details = None
         if enabled is not None:
@@ -937,15 +917,15 @@
             provider=provider,
             credentials=issuer_credentials,
             organization_details=organization_details,
             attributes=issuer_attributes,
         )
 
         issuer_bundle = self._client.set_certificate_issuer(
-            vault_base_url=self.vault_url, issuer_name=issuer_name, parameter=parameters, error_map=_error_map, **kwargs
+            vault_base_url=self.vault_url, issuer_name=issuer_name, parameter=parameters, **kwargs
         )
         return CertificateIssuer._from_issuer_bundle(issuer_bundle=issuer_bundle)
 
     @distributed_trace
     def update_issuer(self, issuer_name: str, **kwargs) -> CertificateIssuer:
         """Updates the specified certificate issuer. Requires certificates/setissuers permission.
 
@@ -972,23 +952,23 @@
         admin_contacts = kwargs.pop("admin_contacts", None)
 
         if account_id or password:
             issuer_credentials = self._models.IssuerCredentials(account_id=account_id, password=password)
         else:
             issuer_credentials = None
         if admin_contacts:
-            admin_details = [
+            admin_details: Optional[List[Any]] = [
                 self._models.AdministratorDetails(
                     first_name=contact.first_name,
                     last_name=contact.last_name,
                     email_address=contact.email,
                     phone=contact.phone,
                 )
                 for contact in admin_contacts
-            ]  # type: Optional[List[Any]]
+            ]
         else:
             admin_details = None
         if organization_id or admin_details:
             organization_details = self._models.OrganizationDetails(id=organization_id, admin_details=admin_details)
         else:
             organization_details = None
         if enabled is not None:
@@ -1000,15 +980,15 @@
             provider=kwargs.pop("provider", None),
             credentials=issuer_credentials,
             organization_details=organization_details,
             attributes=issuer_attributes,
         )
 
         issuer_bundle = self._client.update_certificate_issuer(
-            vault_base_url=self.vault_url, issuer_name=issuer_name, parameter=parameters, error_map=_error_map, **kwargs
+            vault_base_url=self.vault_url, issuer_name=issuer_name, parameter=parameters, **kwargs
         )
         return CertificateIssuer._from_issuer_bundle(issuer_bundle=issuer_bundle)
 
     @distributed_trace
     def delete_issuer(self, issuer_name: str, **kwargs) -> CertificateIssuer:
         """Deletes the specified certificate issuer.
 
@@ -1026,20 +1006,20 @@
                 :start-after: [START delete_issuer]
                 :end-before: [END delete_issuer]
                 :language: python
                 :caption: Delete an issuer
                 :dedent: 8
         """
         issuer_bundle = self._client.delete_certificate_issuer(
-            vault_base_url=self.vault_url, issuer_name=issuer_name, error_map=_error_map, **kwargs
+            vault_base_url=self.vault_url, issuer_name=issuer_name, **kwargs
         )
         return CertificateIssuer._from_issuer_bundle(issuer_bundle=issuer_bundle)
 
     @distributed_trace
-    def list_properties_of_issuers(self, **kwargs) -> "ItemPaged[IssuerProperties]":
+    def list_properties_of_issuers(self, **kwargs) -> ItemPaged[IssuerProperties]:
         """Lists properties of the certificate issuers for the key vault.
 
         Requires the certificates/manageissuers/getissuers permission.
 
         :return: An iterator-like instance of Issuers
         :rtype: ~azure.core.paging.ItemPaged[~azure.keyvault.certificates.CertificateIssuer]
 
@@ -1054,10 +1034,9 @@
                 :dedent: 8
         """
         max_page_size = kwargs.pop("max_page_size", None)
         return self._client.get_certificate_issuers(
             vault_base_url=self.vault_url,
             maxresults=max_page_size,
             cls=lambda objs: [IssuerProperties._from_issuer_item(issuer_item=x) for x in objs],
-            error_map=_error_map,
             **kwargs
         )
```

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_polling.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_polling.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,33 @@
 # ------------------------------------
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 # ------------------------------------
 import logging
 import time
+from typing import Any, Callable, Optional, Union
 
 from azure.core.polling import PollingMethod
-
-try:
-    from typing import TYPE_CHECKING
-except ImportError:
-    TYPE_CHECKING = False
-
-if TYPE_CHECKING:
-    # pylint: disable=ungrouped-imports
-    from typing import Any, Callable, Optional, Union
-    from azure.keyvault.certificates import KeyVaultCertificate, CertificateOperation
+from azure.keyvault.certificates._models import KeyVaultCertificate, CertificateOperation
 
 logger = logging.getLogger(__name__)
 
 
 class CreateCertificatePoller(PollingMethod):
-    def __init__(self, get_certificate_command: "Callable", interval: int = 5) -> None:
-        self._command = None  # type: Optional[Callable]
-        self._resource = None  # type: Optional[Union[CertificateOperation, KeyVaultCertificate]]
-        self._pending_certificate_op = None  # type: Optional[CertificateOperation]
+    def __init__(self, get_certificate_command: Callable, interval: int = 5) -> None:
+        self._command: Optional[Callable] = None
+        self._resource: Optional[Union[CertificateOperation, KeyVaultCertificate]] = None
+        self._pending_certificate_op: Optional[CertificateOperation] = None
         self._get_certificate_command = get_certificate_command
         self._polling_interval = interval
 
     def _update_status(self) -> None:
         self._pending_certificate_op = self._command() if self._command else None
 
-    def initialize(self, client: "Any", initial_response: "Any", _: "Callable") -> None:
+    def initialize(self, client: Any, initial_response: Any, _: Any) -> None:
         self._command = client
         self._pending_certificate_op = initial_response
 
     def run(self) -> None:
         try:
             while not self.finished():
                 self._update_status()
@@ -52,12 +44,12 @@
 
     def finished(self) -> bool:
         operation = self._pending_certificate_op
         if operation and operation.issuer_name and operation.issuer_name.lower() == "unknown":
             return True
         return self._pending_certificate_op.status.lower() != "inprogress"  # type: ignore
 
-    def resource(self) -> "Union[KeyVaultCertificate, CertificateOperation]":
+    def resource(self) -> Union[KeyVaultCertificate, CertificateOperation]:
         return self._resource  # type: ignore
 
     def status(self) -> str:
         return self._pending_certificate_op.status.lower()  # type: ignore
```

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_models.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 # ------------------------------------
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 # ------------------------------------
 # pylint: disable=too-many-lines,too-many-public-methods
+from typing import TYPE_CHECKING
+
 from . import _generated_models as models
 from ._shared import parse_key_vault_id
 from ._enums import(
     CertificatePolicyAction,
     KeyUsageType,
     KeyCurveName,
     KeyType,
     CertificateContentType,
     WellKnownIssuerNames
 )
 
-try:
-    from typing import TYPE_CHECKING
-except ImportError:
-    TYPE_CHECKING = False
-
 if TYPE_CHECKING:
-    from typing import Any, Dict, Optional, Union, List
+    from typing import Dict, Optional, Union, List
     from datetime import datetime
 
 
 class AdministratorContact(object):
     """Details of the organization administrator of the certificate issuer.
 
     :param first_name: First name of the issuer.
@@ -54,15 +51,14 @@
             f"AdministratorContact(first_name={self.first_name}, last_name={self.last_name}, "
             + f"email={self.email}, phone={self.phone})"
         )
         return result[:1024]
 
     @classmethod
     def _from_admin_detail(cls, admin_detail: models.AdministratorDetails) -> "AdministratorContact":
-        """Construct a AdministratorContact from an autorest-generated AdministratorDetailsBundle"""
         return cls(
             email=admin_detail.email_address,
             first_name=admin_detail.first_name,
             last_name=admin_detail.last_name,
             phone=admin_detail.phone,
         )
 
@@ -112,31 +108,34 @@
             inner_error=cls._from_error_bundle(error_bundle.inner_error)  # type: ignore
         )
 
     @property
     def code(self) -> str:
         """The error code.
 
+        :returns: The error code.
         :rtype: str
         """
         return self._code
 
     @property
     def message(self) -> str:
         """The error message.
 
+        :returns: The error message.
         :rtype: str
         """
         return self._message
 
     @property
     def inner_error(self) -> "CertificateOperationError":
-        """The error itself
+        """The error itself.
 
-        :return ~azure.keyvault.certificates.CertificateOperationError:
+        :returns: The error itself.
+        :rtype: :class:`~azure.keyvault.certificates.CertificateOperationError`
         """
         return self._inner_error
 
 
 class CertificateProperties(object):
     """Certificate properties consists of a certificates metadata."""
 
@@ -150,125 +149,148 @@
     def __repr__(self) -> str:
         return f"<CertificateProperties [{self.id}]>"[:1024]
 
     @classmethod
     def _from_certificate_item(
         cls, certificate_item: "Union[models.CertificateItem, models.CertificateBundle]"
     ) -> "CertificateProperties":
-        """Construct a CertificateProperties from an autorest-generated CertificateItem"""
         return cls(
             attributes=certificate_item.attributes,
             cert_id=certificate_item.id,
             x509_thumbprint=certificate_item.x509_thumbprint,
             tags=certificate_item.tags,
         )
 
     @property
     def id(self) -> str:
-        """Certificate identifier.
+        """The certificate identifier.
 
+        :returns: The certificate identifier.
         :rtype: str
         """
         return self._id
 
     @property
     def name(self) -> str:
         """The name of the certificate.
 
+        :returns: The name of the certificate.
         :rtype: str
         """
         return self._vault_id.name
 
     @property
     def enabled(self) -> "Optional[bool]":
         """Whether the certificate is enabled or not.
 
+        :returns: True if the certificate is enabled; False otherwise.
         :rtype: bool or None
         """
         return self._attributes.enabled if self._attributes else None
 
     @property
     def not_before(self) -> "Optional[datetime]":
         """The datetime before which the certificate is not valid.
 
+        :returns: A datetime representing the point in time when the certificate becomes valid.
         :rtype: ~datetime.datetime or None
         """
         return self._attributes.not_before if self._attributes else None
 
     @property
     def expires_on(self) -> "Optional[datetime]":
         """The datetime when the certificate expires.
 
+        :returns: A datetime representing the point in time when the certificate expires.
         :rtype: ~datetime.datetime or None
         """
         return self._attributes.expires if self._attributes else None
 
     @property
     def created_on(self) -> "Optional[datetime]":
         """The datetime when the certificate is created.
 
+        :returns: A datetime representing the certificate's creation time.
         :rtype: ~datetime.datetime or None
         """
         return self._attributes.created if self._attributes else None
 
     @property
     def updated_on(self) -> "Optional[datetime]":
         """The datetime when the certificate was last updated.
 
+        :returns: A datetime representing the time of the certificate's most recent update.
         :rtype: ~datetime.datetime or None
         """
         return self._attributes.updated if self._attributes else None
 
     @property
     def recoverable_days(self) -> "Optional[int]":
         """The number of days the certificate is retained before being deleted from a soft-delete enabled Key Vault.
 
+        :returns: The number of days remaining where the certificate can be restored.
         :rtype: int or None
         """
         # recoverable_days was added in 7.1-preview
         if self._attributes and hasattr(self._attributes, "recoverable_days"):
             return self._attributes.recoverable_days
         return None
 
     @property
     def recovery_level(self) -> "Optional[models.DeletionRecoveryLevel]":
         """The deletion recovery level currently in effect for the certificate.
 
+        :returns: The deletion recovery level currently in effect for the certificate.
         :rtype: models.DeletionRecoveryLevel or None
         """
         return self._attributes.recovery_level if self._attributes else None
 
     @property
     def vault_url(self) -> str:
-        """URL of the vault containing the certificate
+        """The URL of the vault containing the certificate.
 
+        :returns: The URL of the vault containing the certificate.
         :rtype: str
         """
         return self._vault_id.vault_url
 
     @property
     def x509_thumbprint(self) -> bytes:
-        """Thumbprint of the certificate.
+        """The certificate's thumbprint, in bytes.
 
+        :return: The certificate's thumbprint, in bytes.
         :rtype: bytes
         """
         return self._x509_thumbprint
 
     @property
+    def x509_thumbprint_string(self) -> str:
+        """The certificate's thumbprint, as a hexadecimal string.
+
+        The thumbprint is formatted without colon delimiters; e.g. 76E1819FADF06A55EF4B126A2EF743C2BAE8A151.
+
+        :return: The certificate's thumbprint, as a hexadecimal string.
+        :rtype: str
+        """
+        return self._x509_thumbprint.hex().upper()
+
+    @property
     def tags(self) -> "Optional[Dict[str, str]]":
         """Application specific metadata in the form of key-value pairs.
 
+        :returns: A dictionary of tags attached to the certificate.
         :rtype: dict[str, str] or None
         """
         return self._tags
 
     @property
     def version(self) -> "Optional[str]":
-        """The version of the certificate
+        """The version of the certificate.
 
+        :returns: The version of the certificate.
         :rtype: str or None
         """
         return self._vault_id.version
 
 
 class KeyVaultCertificate(object):
     """Consists of a certificate and its attributes
@@ -295,82 +317,90 @@
         self._cer = cer
 
     def __repr__(self) -> str:
         return f"<KeyVaultCertificate [{self.id}]>"[:1024]
 
     @classmethod
     def _from_certificate_bundle(cls, certificate_bundle: models.CertificateBundle) -> "KeyVaultCertificate":
-        """Construct a certificate from an autorest-generated certificateBundle"""
-        # pylint:disable=protected-access, line-too-long
+        # pylint:disable=protected-access
 
         if certificate_bundle.policy:
-            policy = CertificatePolicy._from_certificate_policy_bundle(certificate_bundle.policy)  # type: Optional[CertificatePolicy]
+            policy: "Optional[CertificatePolicy]" = CertificatePolicy._from_certificate_policy_bundle(
+                certificate_bundle.policy
+            )
         else:
             policy = None
 
         return cls(
             properties=CertificateProperties._from_certificate_item(certificate_bundle),
             key_id=certificate_bundle.kid,
             secret_id=certificate_bundle.sid,
             policy=policy,
             cer=certificate_bundle.cer,  # type: ignore
         )
 
     @property
     def id(self) -> "Optional[str]":
-        """Certificate identifier.
+        """The certificate identifier.
 
+        :returns: The certificate identifier.
         :rtype: str or None
         """
         return self._properties.id if self._properties else None
 
     @property
     def name(self) -> "Optional[str]":
         """The name of the certificate.
 
+        :returns: The name of the certificate.
         :rtype: str or None
         """
         return self._properties.name if self._properties else None
 
     @property
     def properties(self) -> "Optional[CertificateProperties]":
-        """The certificate's properties
+        """The certificate's properties.
 
+        :returns: The certificate's properties.
         :rtype: ~azure.keyvault.certificates.CertificateProperties or None
         """
         return self._properties
 
     @property
     def key_id(self) -> "Optional[str]":
         """The ID of the key associated with the certificate.
 
+        :returns: The ID of the key associated with the certificate.
         :rtype: str or None
         """
         return self._key_id
 
     @property
     def secret_id(self) -> "Optional[str]":
         """The ID of the secret associated with the certificate.
 
+        :returns: The ID of the secret associated with the certificate.
         :rtype: str or None
         """
         return self._secret_id
 
     @property
     def policy(self) -> "Optional[CertificatePolicy]":
         """The management policy of the certificate.
 
+        :returns: The management policy of the certificate.
         :rtype: ~azure.keyvault.certificates.CertificatePolicy or None
         """
         return self._policy
 
     @property
     def cer(self) -> "Optional[bytearray]":
         """The CER contents of the certificate.
 
+        :returns: The CER contents of the certificate.
         :rtype: bytearray or None
         """
         return self._cer
 
 
 class KeyVaultCertificateIdentifier(object):
     """Information about a KeyVaultCertificate parsed from a certificate ID.
@@ -468,15 +498,14 @@
     def __repr__(self) -> str:
         return f"<CertificateOperation [{self.id}]>"[:1024]
 
     @classmethod
     def _from_certificate_operation_bundle(
         cls, certificate_operation_bundle: models.CertificateOperation
     ) -> "CertificateOperation":
-        """Construct a CertificateOperation from an autorest-generated CertificateOperation"""
 
         issuer_parameters = certificate_operation_bundle.issuer_parameters
         return cls(
             cert_operation_id=certificate_operation_bundle.id,
             issuer_name=issuer_parameters.name if issuer_parameters else None,
             certificate_type=(
                 certificate_operation_bundle.issuer_parameters.certificate_type
@@ -493,98 +522,125 @@
                    if certificate_operation_bundle.error else None),
             target=certificate_operation_bundle.target,
             request_id=certificate_operation_bundle.request_id,
         )
 
     @property
     def id(self) -> "Optional[str]":
-        """:rtype: str or None"""
+        """The certificate ID.
+
+        :returns: The certificate ID.
+        :rtype: str or None
+        """
         return self._id
 
     @property
     def name(self) -> "Optional[str]":
-        """:rtype: str or None"""
+        """The certificate name.
+
+        :returns: The certificate name.
+        :rtype: str or None
+        """
         return self._vault_id.name if self._vault_id else None
 
     @property
     def vault_url(self) -> "Optional[str]":
-        """URL of the vault containing the CertificateOperation
+        """URL of the vault performing the certificate operation.
 
+        :returns: URL of the vault performing the certificate operation.
         :rtype: str or None
         """
         return self._vault_id.vault_url if self._vault_id else None
 
     @property
     def issuer_name(self) -> "Union[str, WellKnownIssuerNames, None]":
-        """The name of the issuer of the certificate.
+        """The name of the certificate issuer.
 
+        :returns: The name of the certificate issuer.
         :rtype: str or ~azure.keyvault.certificates.WellKnownIssuerNames or None
         """
         return self._issuer_name
 
     @property
     def certificate_type(self) -> "Optional[str]":
         """Type of certificate to be requested from the issuer provider.
 
+        :returns: Type of certificate to be requested from the issuer provider.
         :rtype: str or None
         """
         return self._certificate_type
 
     @property
     def certificate_transparency(self) -> "Optional[bool]":
-        """Whether certificates generated under this policy should be published to certificate
-        transparency logs.
+        """Whether certificates generated under this policy should be published to certificate transparency logs.
 
+        :returns: True if the certificates should be published to transparency logs; False otherwise.
         :rtype: bool or None
         """
         return self._certificate_transparency
 
     @property
     def csr(self) -> "Optional[bytes]":
         """The certificate signing request that is being used in this certificate operation.
 
+        :returns: The certificate signing request that is being used in this certificate operation.
         :rtype: bytes or None
         """
         return self._csr
 
     @property
     def cancellation_requested(self) -> "Optional[bool]":
         """Whether cancellation was requested on the certificate operation.
 
+        :returns: True if cancellation was requested; False otherwise.
         :rtype: bool or None
         """
         return self._cancellation_requested
 
     @property
     def status(self) -> "Optional[str]":
-        """:rtype: str or None"""
+        """The operation status.
+
+        :returns: The operation status.
+        :rtype: str or None
+        """
         return self._status
 
     @property
     def status_details(self) -> "Optional[str]":
-        """:rtype: str or None"""
+        """Details of the operation status.
+
+        :returns: Details of the operation status.
+        :rtype: str or None
+        """
         return self._status_details
 
     @property
     def error(self) -> "Optional[CertificateOperationError]":
-        """:rtype: ~azure.keyvault.certificates.CertificateOperationError or None"""
+        """Any error associated with the certificate operation.
+
+        :returns: Any error associated with the operation, as a
+            :class:`~azure.keyvault.certificates.CertificateOperationError`.
+        :rtype: ~azure.keyvault.certificates.CertificateOperationError or None"""
         return self._error
 
     @property
     def target(self) -> "Optional[str]":
         """Location which contains the result of the certificate operation.
 
+        :returns: Location which contains the result of the certificate operation.
         :rtype: str or None
         """
         return self._target
 
     @property
     def request_id(self) -> "Optional[str]":
         """Identifier for the certificate operation.
 
+        :returns: Identifier for the certificate operation.
         :rtype: str or None
         """
         return self._request_id
 
 
 class CertificatePolicy(object):
     """Management policy for a certificate.
@@ -664,21 +720,20 @@
     def get_default(cls) -> "CertificatePolicy":
         return cls(issuer_name=WellKnownIssuerNames.self, subject="CN=DefaultPolicy")
 
     def __repr__(self) -> str:
         return f"<CertificatePolicy [issuer_name: {self.issuer_name}]>"[:1024]
 
     def _to_certificate_policy_bundle(self) -> models.CertificatePolicy:
-        """Construct a version emulating the generated CertificatePolicy from a wrapped CertificatePolicy"""
         if self.issuer_name or self.certificate_type or self.certificate_transparency:
-            issuer_parameters = models.IssuerParameters(
+            issuer_parameters: "Optional[models.IssuerParameters]" = models.IssuerParameters(
                 name=self.issuer_name,
                 certificate_type=self.certificate_type,
                 certificate_transparency=self.certificate_transparency,  # 2016-10-01 model will ignore this
-            )  # type: Optional[models.IssuerParameters]
+            )
         else:
             issuer_parameters = None
 
         # pylint:disable=too-many-boolean-expressions
         if (
             self.enabled is not None
             or self.created_on is not None
@@ -714,84 +769,83 @@
             or self.key_usage
             or self.san_emails
             or self.san_user_principal_names
             or self.san_dns_names
             or self.validity_in_months
         ):
             if self.key_usage:
-                key_usage = [
+                key_usage: "Optional[List[Union[str, KeyUsageType]]]" = [
                     k.value if not isinstance(k, str) else k for k in self.key_usage
-                ]  # type: Optional[List[Union[str, KeyUsageType]]]
+                ]
             else:
                 key_usage = None
 
-            x509_certificate_properties = models.X509CertificateProperties(
+            x509_properties: "Optional[models.X509CertificateProperties]" = models.X509CertificateProperties(
                 subject=self.subject,
                 ekus=self.enhanced_key_usage,
                 subject_alternative_names=models.SubjectAlternativeNames(
                     emails=self.san_emails, upns=self.san_user_principal_names, dns_names=self.san_dns_names
                 ),
                 key_usage=key_usage,
                 validity_in_months=self.validity_in_months,
-            )  # type: Optional[models.X509CertificateProperties]
+            )
         else:
-            x509_certificate_properties = None
+            x509_properties = None
 
         if self.exportable or self.key_type or self.key_size or self.reuse_key or self.key_curve_name:
-            key_properties = models.KeyProperties(
+            key_properties: "Optional[models.KeyProperties]" = models.KeyProperties(
                 exportable=self.exportable,
                 key_type=self.key_type,
                 key_size=self.key_size,
                 reuse_key=self.reuse_key,
                 curve=self.key_curve_name,
-            )  # type: Optional[models.KeyProperties]
+            )
         else:
             key_properties = None
 
         if self.content_type:
-            secret_properties = models.SecretProperties(
+            secret_properties: "Optional[models.SecretProperties]" = models.SecretProperties(
                 content_type=self.content_type
-            )  # type: Optional[models.SecretProperties]
+            )
         else:
             secret_properties = None
 
         policy_bundle = models.CertificatePolicy(
             key_properties=key_properties,
             secret_properties=secret_properties,
-            x509_certificate_properties=x509_certificate_properties,
+            x509_certificate_properties=x509_properties,
             lifetime_actions=lifetime_actions,
             issuer_parameters=issuer_parameters,
             attributes=attributes,
         )
         return policy_bundle
 
     @classmethod
     def _from_certificate_policy_bundle(
         cls, certificate_policy_bundle: "Optional[models.CertificatePolicy]"
     ) -> "CertificatePolicy":
-        """Construct a CertificatePolicy from an autorest-generated CertificatePolicy"""
         if certificate_policy_bundle is None:
             return cls()
 
         if certificate_policy_bundle.lifetime_actions:
-            lifetime_actions = [
+            lifetime_actions: "Optional[List[LifetimeAction]]" = [
                 LifetimeAction(
                     action=CertificatePolicyAction(item.action.action_type) if item.action else None,
                     lifetime_percentage=item.trigger.lifetime_percentage if item.trigger else None,
                     days_before_expiry=item.trigger.days_before_expiry if item.trigger else None,
                 )
                 for item in certificate_policy_bundle.lifetime_actions
-            ]  # type: Optional[List[LifetimeAction]]
+            ]
         else:
             lifetime_actions = None
         x509_certificate_properties = certificate_policy_bundle.x509_certificate_properties
         if x509_certificate_properties and x509_certificate_properties.key_usage:
-            key_usage = [
+            key_usage: "Optional[List[KeyUsageType]]" = [
                 KeyUsageType(k) for k in x509_certificate_properties.key_usage
-            ]  # type: Optional[List[KeyUsageType]]
+            ]
         else:
             key_usage = None
         key_properties = certificate_policy_bundle.key_properties
         curve_name = getattr(key_properties, "curve", None)  # missing from 2016-10-01 KeyProperties
         if curve_name:
             curve_name = KeyCurveName(curve_name)
 
@@ -837,169 +891,186 @@
             ),
         )
 
     @property
     def exportable(self) -> "Optional[bool]":
         """Whether the private key can be exported.
 
+        :returns: True if the private key can be exported; False otherwise.
         :rtype: bool or None
         """
         return self._exportable
 
     @property
     def key_type(self) -> "Optional[KeyType]":
         """The type of key pair to be used for the certificate.
 
+        :returns: The type of key pair to be used for the certificate.
         :rtype: ~azure.keyvault.certificates.KeyType or None
         """
         return self._key_type
 
     @property
     def key_size(self) -> "Optional[int]":
         """The key size in bits.
 
+        :returns: The key size in bits.
         :rtype: int or None
         """
         return self._key_size
 
     @property
     def reuse_key(self) -> "Optional[bool]":
         """Whether the same key pair will be used on certificate renewal.
 
+        :returns: True if the same key pair will be used on certificate renewal; False otherwise.
         :rtype: bool or None
         """
         return self._reuse_key
 
     @property
     def key_curve_name(self) -> "Optional[KeyCurveName]":
         """Elliptic curve name.
 
+        :returns: Elliptic curve name.
         :rtype: ~azure.keyvault.certificates.KeyCurveName or None
         """
         return self._key_curve_name
 
     @property
     def enhanced_key_usage(self) -> "Optional[List[str]]":
         """The enhanced key usage.
 
+        :returns: The enhanced key usage.
         :rtype: list[str] or None
         """
         return self._enhanced_key_usage
 
     @property
     def key_usage(self) -> "Optional[List[KeyUsageType]]":
         """List of key usages.
 
+        :returns: List of key usages.
         :rtype: list[~azure.keyvault.certificates.KeyUsageType] or None
         """
         return self._key_usage
 
     @property
     def content_type(self) -> "Optional[CertificateContentType]":
         """The media type (MIME type).
 
+        :returns: The media type (MIME type).
         :rtype: ~azure.keyvault.certificates.CertificateContentType or None
         """
         return self._content_type
 
     @property
     def subject(self) -> "Optional[str]":
         """The subject name of the certificate.
 
+        :returns: The subject name of the certificate.
         :rtype: str or None
         """
         return self._subject
 
     @property
     def san_emails(self) -> "Optional[List[str]]":
         """The subject alternative email addresses.
 
+        :returns: The subject alternative email addresses, as a list.
         :rtype: list[str] or None
         """
         return self._san_emails
 
     @property
     def san_dns_names(self) -> "Optional[List[str]]":
         """The subject alternative domain names.
 
+        :returns: The subject alternative domain names, as a list.
         :rtype: list[str] or None
         """
         return self._san_dns_names
 
     @property
     def san_user_principal_names(self) -> "Optional[List[str]]":
         """The subject alternative user principal names.
 
+        :returns: The subject alternative user principal names, as a list.
         :rtype: list[str] or None
         """
         return self._san_user_principal_names
 
     @property
     def validity_in_months(self) -> "Optional[int]":
         """The duration that the certificate is valid for in months.
 
+        :returns: The duration that the certificate is valid for in months.
         :rtype: int or None
         """
         return self._validity_in_months
 
     @property
     def lifetime_actions(self) -> "Optional[List[LifetimeAction]]":
-        """Actions and their triggers that will be performed by Key Vault over
-        the lifetime of the certificate.
+        """Actions and their triggers that will be performed by Key Vault over the lifetime of the certificate.
 
+        :returns: Actions and their triggers that will be performed by Key Vault over the lifetime of the certificate.
         :rtype: list[~azure.keyvault.certificates.LifetimeAction] or None
         """
         return self._lifetime_actions
 
     @property
     def issuer_name(self) -> "Optional[str]":
-        """Name of the referenced issuer object or reserved names for the issuer
-        of the certificate.
+        """Name of the referenced issuer object or reserved names for the issuer of the certificate.
 
+        :returns: Name of the referenced issuer object or reserved names for the issuer of the certificate.
         :rtype: str or None
         """
         return self._issuer_name
 
     @property
     def certificate_type(self) -> "Optional[str]":
         """Type of certificate requested from the issuer provider.
 
+        :returns: Type of certificate requested from the issuer provider.
         :rtype: str or None
         """
         return self._certificate_type
 
     @property
     def certificate_transparency(self) -> "Optional[bool]":
-        """Whether the certificates generated under this policy should be published
-        to certificate transparency logs.
+        """Whether the certificates generated under this policy should be published to certificate transparency logs.
 
+        :returns: True if the certificates should be published to transparency logs; False otherwise.
         :rtype: bool or None
         """
         return self._certificate_transparency
 
     @property
     def enabled(self) -> "Optional[bool]":
         """Whether the certificate is enabled or not.
 
+        :returns: True if the certificate is enabled; False otherwise.
         :rtype: bool or None
         """
         return self._attributes.enabled if self._attributes else None
 
     @property
     def created_on(self) -> "Optional[datetime]":
         """The datetime when the certificate is created.
 
+        :returns: The datetime when the certificate is created.
         :rtype: ~datetime.datetime or None
         """
         return self._attributes.created if self._attributes else None
 
     @property
     def updated_on(self) -> "Optional[datetime]":
         """The datetime when the certificate was last updated.
 
+        :returns: The datetime when the certificate was last updated.
         :rtype: ~datetime.datetime or None
         """
         return self._attributes.updated if self._attributes else None
 
 
 class CertificateContact(object):
     """The contact information for the vault certificates.
@@ -1023,15 +1094,14 @@
         return f"CertificateContact(email={self.email}, name={self.name}, phone={self.phone})"[:1024]
 
     def _to_certificate_contacts_item(self) -> models.Contact:
         return models.Contact(email_address=self.email, name=self.name, phone=self.phone)
 
     @classmethod
     def _from_certificate_contacts_item(cls, contact_item: models.Contact) -> "CertificateContact":
-        """Construct a CertificateContact from an autorest-generated ContactItem."""
         return cls(email=contact_item.email_address, name=contact_item.name, phone=contact_item.phone)
 
     @property
     def email(self) -> "Optional[str]":
         """:rtype: str or None"""
         return self._email
 
@@ -1061,39 +1131,52 @@
     def __repr__(self) -> str:
         return f"IssuerProperties(issuer_id={self.id}, provider={self.provider})"[:1024]
 
     @classmethod
     def _from_issuer_item(
         cls, issuer_item: "Union[models.CertificateIssuerItem, models.IssuerBundle]"
     ) -> "IssuerProperties":
-        """Construct a IssuerProperties from an autorest-generated CertificateIssuerItem"""
         return cls(issuer_id=issuer_item.id, provider=issuer_item.provider)
 
     @property
     def id(self) -> "Optional[str]":
-        """:rtype: str or None"""
+        """The issuer ID.
+
+        :returns: The issuer ID.
+        :rtype: str or None
+        """
         return self._id
 
     @property
     def name(self) -> "Optional[str]":
-        """:rtype: str or None"""
+        """The issuer name.
+
+        :returns: The issuer name.
+        :rtype: str or None
+        """
         # Issuer name is listed under version under vault_id
         return self._vault_id.version
 
     @property
     def provider(self) -> "Optional[str]":
-        """:rtype: str or None"""
+        """The issuer provider.
+
+        :returns: The issuer provider.
+        :rtype: str or None
+        """
         return self._provider
 
 
 class CertificateIssuer(object):
     """The issuer for a Key Vault certificate.
 
     :param provider: The issuer provider
     :type provider: str or None
+    :param attributes: The issuer attributes.
+    :type attributes: ~azure.keyvault.certificates._generated_models.IssuerAttributes or None
     :param account_id: The username / account name / account id.
     :type account_id: str or None
     :param password: The password / secret / account key.
     :type password: str or None
     :param organization_id: The ID of the organization.
     :type organization_id: str or None
     :param admin_contacts: Details of the organization administrator.
@@ -1121,15 +1204,14 @@
         self._vault_id = parse_key_vault_id(self._id)
 
     def __repr__(self) -> str:
         return f"<CertificateIssuer [{self.id}]>"[:1024]
 
     @classmethod
     def _from_issuer_bundle(cls, issuer_bundle: models.IssuerBundle) -> "CertificateIssuer":
-        """Construct a CertificateIssuer from an autorest-generated IssuerBundle"""
         admin_contacts = []
         admin_details = (
             issuer_bundle.organization_details.admin_details if issuer_bundle.organization_details else None
         )
         if admin_details:
             # pylint:disable=protected-access
             for admin_detail in admin_details:
@@ -1142,83 +1224,102 @@
             organization_id=issuer_bundle.organization_details.id if issuer_bundle.organization_details else None,
             admin_contacts=admin_contacts,
             issuer_id=issuer_bundle.id,
         )
 
     @property
     def id(self) -> "Optional[str]":
-        """:rtype: str or None"""
+        """The issuer ID.
+
+        :returns: The issuer ID.
+        :rtype: str or None
+        """
         return self._id
 
     @property
     def name(self) -> "Optional[str]":
-        """:rtype: str or None"""
+        """The issuer name.
+
+        :returns: The issuer name.
+        :rtype: str or None
+        """
         # Issuer name is listed under version under vault_id.
         # This is because the id we pass to parse_key_vault_id has an extra segment, so where most cases the version of
         # the general pattern is certificates/name/version, but here we have certificates/issuers/name/version.
         # Issuers are not versioned.
         return self._vault_id.version
 
     @property
     def provider(self) -> "Optional[str]":
         """The issuer provider.
 
+        :returns: The issuer provider.
         :rtype: str or None
         """
         return self._provider
 
     @property
     def enabled(self) -> "Optional[bool]":
         """Whether the certificate is enabled or not.
 
+        :returns: True if the certificate is enabled; False otherwise.
         :rtype: bool or None
         """
         return self._attributes.enabled if self._attributes else None
 
     @property
     def created_on(self) -> "Optional[datetime]":
         """The datetime when the certificate is created.
 
+        :returns: The datetime when the certificate is created.
         :rtype: ~datetime.datetime or None
         """
         return self._attributes.created if self._attributes else None
 
     @property
     def updated_on(self) -> "Optional[datetime]":
         """The datetime when the certificate was last updated.
 
+        :returns: The datetime when the certificate was last updated.
         :rtype: ~datetime.datetime or None
         """
         return self._attributes.updated if self._attributes else None
 
     @property
     def account_id(self) -> "Optional[str]":
-        """The username/ account name/ account id.
+        """The username / account name / account id.
 
+        :returns: The username / account name / account id.
         :rtype: str or None
         """
         return self._account_id
 
     @property
     def password(self) -> "Optional[str]":
         """The password / secret / account key.
 
+        :returns: The password / secret / account key.
         :rtype: str or None
         """
         return self._password
 
     @property
     def organization_id(self) -> "Optional[str]":
-        """:rtype: str or None"""
+        """The issuer organization ID.
+
+        :returns: The issuer organization ID.
+        :rtype: str or None
+        """
         return self._organization_id
 
     @property
     def admin_contacts(self) -> "Optional[List[AdministratorContact]]":
-        """Contact details of the organization administrator of this issuer.
+        """Contact details of the organization administrator(s) of this issuer.
 
+        :returns: Contact details of the organization administrator(s) of this issuer.
         :rtype: list[~azure.keyvault.certificates.AdministratorContact] or None
         """
         return self._admin_contacts
 
 
 class LifetimeAction(object):
     """Action and its trigger that will be performed by certificate Vault over the lifetime of a certificate.
@@ -1250,48 +1351,55 @@
         )
         return result[:1024]
 
     @property
     def lifetime_percentage(self) -> "Optional[int]":
         """Percentage of lifetime at which to trigger.
 
+        :returns: Percentage of lifetime at which to trigger.
         :rtype: int or None
         """
         return self._lifetime_percentage
 
     @property
     def days_before_expiry(self) -> "Optional[int]":
         """Days before expiry to attempt renewal.
 
+        :returns: Days before expiry to attempt renewal.
         :rtype: int or None
         """
         return self._days_before_expiry
 
     @property
     def action(self) -> "Union[str, CertificatePolicyAction, None]":
-        """The type of the action that will be executed. Valid values are "EmailContacts" and "AutoRenew".
+        """The type of action that will be executed; see :class:`~azure.keyvault.certificates.CertificatePolicyAction`.
 
+        :returns: The type of action that will be executed; see
+            :class:`~azure.keyvault.certificates.CertificatePolicyAction`.
         :rtype: str or ~azure.keyvault.certificates.CertificatePolicyAction or None
         """
         return self._action
 
 
 class DeletedCertificate(KeyVaultCertificate):
     """A deleted Certificate consisting of its previous ID, attributes, tags, and information on when it will be purged.
 
+    :param properties: Properties of the deleted certificate.
+    :type properties: ~azure.keyvault.certificates.CertificateProperties
     :param policy: The management policy of the deleted certificate.
     :type policy: ~azure.keyvault.certificates.CertificatePolicy or None
     :param cer: CER contents of the X509 certificate.
     :type cer: bytearray or None
-    :param deleted_on: The time when the certificate was deleted, in UTC.
-    :type deleted_on: ~datetime.datetime or None
-    :param recovery_id: The url of the recovery object, used to identify and recover the deleted certificate.
-    :type recovery_id: str or None
-    :param scheduled_purge_date: The time when the certificate is scheduled to be purged, in UTC.
-    :type scheduled_purge_date: ~datetime.datetime or None
+
+    :keyword deleted_on: The time when the certificate was deleted, in UTC.
+    :paramtype deleted_on: ~datetime.datetime or None
+    :keyword recovery_id: The url of the recovery object, used to identify and recover the deleted certificate.
+    :paramtype recovery_id: str or None
+    :keyword scheduled_purge_date: The time when the certificate is scheduled to be purged, in UTC.
+    :paramtype scheduled_purge_date: ~datetime.datetime or None
     """
 
     def __init__(
         self,
         properties: "Optional[CertificateProperties]" = None,
         policy: "Optional[CertificatePolicy]" = None,
         cer: "Optional[bytearray]" = None,
@@ -1305,15 +1413,14 @@
     def __repr__(self) -> str:
         return f"<DeletedCertificate [{self.id}]>"[:1024]
 
     @classmethod
     def _from_deleted_certificate_item(
         cls, deleted_certificate_item: models.DeletedCertificateItem
     ) -> "DeletedCertificate":
-        """Construct a DeletedCertificate from an autorest-generated DeletedCertificateItem"""
         return cls(
             properties=CertificateProperties._from_certificate_item(  # pylint: disable=protected-access
                 deleted_certificate_item
             ),
             key_id=None,
             secret_id=None,
             policy=None,
@@ -1323,43 +1430,45 @@
             scheduled_purge_date=deleted_certificate_item.scheduled_purge_date,
         )
 
     @classmethod
     def _from_deleted_certificate_bundle(
         cls, deleted_certificate_bundle: models.DeletedCertificateBundle
     ) -> "DeletedCertificate":
-        """Construct a DeletedCertificate from an autorest-generated DeletedCertificateItem"""
         # pylint:disable=protected-access
         return cls(
             properties=CertificateProperties._from_certificate_item(deleted_certificate_bundle),
             key_id=deleted_certificate_bundle.kid,
             secret_id=deleted_certificate_bundle.sid,
             policy=CertificatePolicy._from_certificate_policy_bundle(deleted_certificate_bundle.policy),
             cer=deleted_certificate_bundle.cer,  # type: ignore
             deleted_on=deleted_certificate_bundle.deleted_date,
             recovery_id=deleted_certificate_bundle.recovery_id,
             scheduled_purge_date=deleted_certificate_bundle.scheduled_purge_date,
         )
 
     @property
     def deleted_on(self) -> "Optional[datetime]":
-        """The datetime that the certificate was deleted.
+        """The datetime when the certificate was deleted.
 
+        :returns: The datetime when the certificate was deleted.
         :rtype: ~datetime.datetime or None
         """
         return self._deleted_on
 
     @property
     def recovery_id(self) -> "Optional[str]":
-        """The url of the recovery object, used to identify and recover the deleted certificate.
+        """The URL of the recovery object, used to identify and recover the deleted certificate.
 
+        :returns: The URL of the recovery object, used to identify and recover the deleted certificate.
         :rtype: str or None
         """
         return self._recovery_id
 
     @property
     def scheduled_purge_date(self) -> "Optional[datetime]":
         """The datetime when the certificate is scheduled to be purged.
 
+        :returns: The datetime when the certificate is scheduled to be purged.
         :rtype: ~datetime.datetime or None
         """
         return self._scheduled_purge_date
```

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_enums.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_enums.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated_models.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated_models.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/__init__.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/http_challenge.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_shared/http_challenge.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,21 +6,29 @@
 from urllib import parse
 
 if TYPE_CHECKING:
     from typing import Dict, MutableMapping, Optional
 
 
 class HttpChallenge(object):
+    """An object representing the content of a Key Vault authentication challenge.
+
+    :param str request_uri: The URI of the HTTP request that prompted this challenge.
+    :param str challenge: The WWW-Authenticate header of the challenge response.
+    :param response_headers: Optional. The headers attached to the challenge response.
+    :type response_headers: MutableMapping[str, str] or None
+    """
+
     def __init__(
         self, request_uri: str, challenge: str, response_headers: "Optional[MutableMapping[str, str]]" = None
     ) -> None:
         """Parses an HTTP WWW-Authentication Bearer challenge from a server."""
         self.source_authority = self._validate_request_uri(request_uri)
         self.source_uri = request_uri
-        self._parameters = {}  # type: Dict[str, str]
+        self._parameters: "Dict[str, str]" = {}
 
         # get the scheme of the challenge and remove from the challenge string
         trimmed_challenge = self._validate_challenge(challenge)
         split_challenge = trimmed_challenge.split(" ", 1)
         self.scheme = split_challenge[0]
         trimmed_challenge = split_challenge[1]
 
@@ -43,75 +51,113 @@
         if "authorization" not in self._parameters and "authorization_uri" not in self._parameters:
             raise ValueError("Invalid challenge parameters")
 
         authorization_uri = self.get_authorization_server()
         # the authorization server URI should look something like https://login.windows.net/tenant-id
         raw_uri_path = str(parse.urlparse(authorization_uri).path)
         uri_path = raw_uri_path.lstrip("/")
-        self.tenant_id = uri_path.split("/")[0] or None
+        self.tenant_id = uri_path.split("/", maxsplit=1)[0] or None
 
         # if the response headers were supplied
         if response_headers:
             # get the message signing key and message key encryption key from the headers
             self.server_signature_key = response_headers.get("x-ms-message-signing-key", None)
             self.server_encryption_key = response_headers.get("x-ms-message-encryption-key", None)
 
     def is_bearer_challenge(self) -> bool:
-        """Tests whether the HttpChallenge a Bearer challenge."""
+        """Tests whether the HttpChallenge is a Bearer challenge.
+
+        :returns: True if the challenge is a Bearer challenge; False otherwise.
+        :rtype: bool
+        """
         if not self.scheme:
             return False
 
         return self.scheme.lower() == "bearer"
 
     def is_pop_challenge(self) -> bool:
-        """Tests whether the HttpChallenge is a proof of possession challenge."""
+        """Tests whether the HttpChallenge is a proof of possession challenge.
+
+        :returns: True if the challenge is a proof of possession challenge; False otherwise.
+        :rtype: bool
+        """
         if not self.scheme:
             return False
 
         return self.scheme.lower() == "pop"
 
     def get_value(self, key: str) -> "Optional[str]":
         return self._parameters.get(key)
 
-    def get_authorization_server(self) -> "Optional[str]":
-        """Returns the URI for the authorization server if present, otherwise empty string."""
+    def get_authorization_server(self) -> str:
+        """Returns the URI for the authorization server if present, otherwise an empty string.
+
+        :returns: The URI for the authorization server if present, otherwise an empty string.
+        :rtype: str
+        """
         value = ""
         for key in ["authorization_uri", "authorization"]:
             value = self.get_value(key) or ""
             if value:
                 break
         return value
 
     def get_resource(self) -> str:
-        """Returns the resource if present, otherwise empty string."""
+        """Returns the resource if present, otherwise an empty string.
+
+        :returns: The challenge resource if present, otherwise an empty string.
+        :rtype: str
+        """
         return self.get_value("resource") or ""
 
     def get_scope(self) -> str:
-        """Returns the scope if present, otherwise empty string."""
+        """Returns the scope if present, otherwise an empty string.
+
+        :returns: The challenge scope if present, otherwise an empty string.
+        :rtype: str
+        """
         return self.get_value("scope") or ""
 
     def supports_pop(self) -> bool:
-        """Returns True if challenge supports pop token auth else False."""
+        """Returns True if the challenge supports proof of possession token auth; False otherwise.
+
+        :returns: True if the challenge supports proof of possession token auth; False otherwise.
+        :rtype: bool
+        """
         return self._parameters.get("supportspop", "").lower() == "true"
 
     def supports_message_protection(self) -> bool:
-        """Returns True if challenge vault supports message protection."""
+        """Returns True if the challenge vault supports message protection; False otherwise.
+
+        :returns: True if the challenge vault supports message protection; False otherwise.
+        :rtype: bool
+        """
         return self.supports_pop() and self.server_encryption_key and self.server_signature_key  # type: ignore
 
-    # pylint:disable=no-self-use
-    def _validate_challenge(self, challenge: str) -> str:
-        """Verifies that the challenge is a valid auth challenge and returns the key=value pairs."""
+    def _validate_challenge(self, challenge: str) -> str:  # pylint:disable=bad-option-value,useless-option-value,no-self-use
+        """Verifies that the challenge is a valid auth challenge and returns the key=value pairs.
+
+        :param str challenge: The WWW-Authenticate header of the challenge response.
+
+        :returns: The challenge key/value pairs, with whitespace removed, as a string.
+        :rtype: str
+        """
         if not challenge:
             raise ValueError("Challenge cannot be empty")
 
         return challenge.strip()
 
-    # pylint:disable=no-self-use
-    def _validate_request_uri(self, uri: str) -> str:
-        """Extracts the host authority from the given URI."""
+    def _validate_request_uri(self, uri: str) -> str:  # pylint:disable=bad-option-value,useless-option-value,no-self-use
+        """Extracts the host authority from the given URI.
+
+        :param str uri: The URI of the HTTP request that prompted the challenge.
+
+        :returns: The challenge host authority.
+        :rtype: str
+        """
         if not uri:
             raise ValueError("request_uri cannot be empty")
 
         parsed = parse.urlparse(uri)
         if not parsed.netloc:
             raise ValueError("request_uri must be an absolute URI")
```

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/_polling.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_shared/_polling.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,26 +19,30 @@
     from typing import Any, Callable, Optional
 
 logger = logging.getLogger(__name__)
 
 
 class KeyVaultOperationPoller(LROPoller):
     """Poller for long running operations where calling result() doesn't wait for operation to complete.
+
+    :param polling_method: The poller's polling method.
+    :type polling_method: ~azure.core.polling.PollingMethod
     """
 
     # pylint: disable=arguments-differ
     def __init__(self, polling_method: PollingMethod) -> None:
         super(KeyVaultOperationPoller, self).__init__(None, None, lambda *_: None, NoPolling())
         self._polling_method = polling_method
 
     # pylint: disable=arguments-differ
     def result(self) -> "Any":  # type: ignore
         """Returns a representation of the final resource without waiting for the operation to complete.
 
         :returns: The deserialized resource of the long running operation
+        :rtype: Any
 
         :raises ~azure.core.exceptions.HttpResponseError: Server problem with the query.
         """
         return self._polling_method.resource()
 
     @distributed_trace
     def wait(self, timeout: "Optional[float]" = None) -> None:
@@ -75,14 +79,21 @@
     This works by polling for the existence of the deleted or recovered resource. When a resource is deleted, Key Vault
     immediately removes it from its collection. However, the resource will not immediately appear in the deleted
     collection. Key Vault will therefore respond 404 to GET requests for the deleted resource; when it responds 2xx,
     the resource exists in the deleted collection i.e. its deletion is complete.
 
     Similarly, while recovering a deleted resource, Key Vault will respond 404 to GET requests for the non-deleted
     resource; when it responds 2xx, the resource exists in the non-deleted collection, i.e. its recovery is complete.
+
+    :param command: A callable to invoke when polling.
+    :type command: Callable
+    :param final_resource: The final resource returned by the polling operation.
+    :type final_resource: Any
+    :param bool finished: Whether or not the polling operation is completed.
+    :param int interval: The polling interval, in seconds.
     """
     def __init__(self, command: "Callable", final_resource: "Any", finished: bool, interval: int = 2) -> None:
         self._command = command
         self._resource = final_resource
         self._polling_interval = interval
         self._finished = finished
```

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/_polling_async.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_shared/_polling_async.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 # ------------------------------------
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 # ------------------------------------
 
 import asyncio
 import logging
-from typing import TYPE_CHECKING
+from typing import Any, Callable
 
 from azure.core.polling import AsyncPollingMethod
 from azure.core.exceptions import ResourceNotFoundError, HttpResponseError
 
-if TYPE_CHECKING:
-    # pylint:disable=ungrouped-imports
-    from typing import Any, Callable, Union
-
 logger = logging.getLogger(__name__)
 
 
 class AsyncDeleteRecoverPollingMethod(AsyncPollingMethod):
     """Poller for deleting resources, and recovering deleted resources, in vaults with soft-delete enabled.
 
     This works by polling for the existence of the deleted or recovered resource. When a resource is deleted, Key Vault
     immediately removes it from its collection. However, the resource will not immediately appear in the deleted
     collection. Key Vault will therefore respond 404 to GET requests for the deleted resource; when it responds 2xx,
     the resource exists in the deleted collection i.e. its deletion is complete.
 
     Similarly, while recovering a deleted resource, Key Vault will respond 404 to GET requests for the non-deleted
     resource; when it responds 2xx, the resource exists in the non-deleted collection, i.e. its recovery is complete.
+
+    :param command: An awaitable to invoke when polling.
+    :type command: Callable
+    :param final_resource: The final resource returned by the polling operation.
+    :type final_resource: Any
+    :param bool finished: Whether or not the polling operation is completed.
+    :param int interval: The polling interval, in seconds.
     """
 
-    def __init__(self, command, final_resource, finished, interval=2):
+    def __init__(
+            self, command: Callable, final_resource: Any, finished: bool, interval: int = 2
+        ) -> None:
         self._command = command
         self._resource = final_resource
         self._polling_interval = interval
         self._finished = finished
 
     def initialize(self, client, initial_response, deserialization_callback):
         pass
@@ -61,12 +66,12 @@
         except Exception as e:
             logger.warning(str(e))
             raise
 
     def finished(self) -> bool:
         return self._finished
 
-    def resource(self) -> "Any":
+    def resource(self) -> Any:
         return self._resource
 
     def status(self) -> str:
         return "finished" if self._finished else "polling"
```

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/challenge_auth_policy.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_shared/challenge_auth_policy.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,60 +11,70 @@
 
 The policy caches the challenge and thus knows how to authenticate future requests. However, authentication
 requirements can change. For example, a vault may move to a new tenant. In such a case the policy will attempt the
 protocol again.
 """
 
 import time
+from typing import TYPE_CHECKING
 from urllib.parse import urlparse
 
 from azure.core.exceptions import ServiceRequestError
 from azure.core.pipeline import PipelineRequest
 from azure.core.pipeline.policies import BearerTokenCredentialPolicy
 
 from .http_challenge import HttpChallenge
 from . import http_challenge_cache as ChallengeCache
 
-try:
-    from typing import TYPE_CHECKING
-except ImportError:
-    TYPE_CHECKING = False
-
 if TYPE_CHECKING:
-    from typing import Any, Optional
+    from typing import Optional
     from azure.core.credentials import AccessToken, TokenCredential
     from azure.core.pipeline import PipelineResponse
 
 
 def _enforce_tls(request: PipelineRequest) -> None:
     if not request.http_request.url.lower().startswith("https"):
         raise ServiceRequestError(
             "Bearer token authentication is not permitted for non-TLS protected (non-https) URLs."
         )
 
 
 def _update_challenge(request: PipelineRequest, challenger: "PipelineResponse") -> HttpChallenge:
-    """Parse challenge from challenger, cache it, return it"""
+    """Parse challenge from a challenge response, cache it, and return it.
+
+    :param request: The pipeline request that prompted the challenge response.
+    :type request: :class:`~azure.core.pipeline.PipelineRequest`
+    :param challenger: The pipeline response containing the authentication challenge.
+    :type challenger: :class:`~azure.core.pipeline.PipelineResponse`
+
+    :returns: An HttpChallenge object representing the authentication challenge.
+    :rtype: HttpChallenge
+    """
 
     challenge = HttpChallenge(
         request.http_request.url,
         challenger.http_response.headers.get("WWW-Authenticate"),
         response_headers=challenger.http_response.headers,
     )
     ChallengeCache.set_challenge_for_url(request.http_request.url, challenge)
     return challenge
 
 
 class ChallengeAuthPolicy(BearerTokenCredentialPolicy):
-    """Policy for handling HTTP authentication challenges"""
+    """Policy for handling HTTP authentication challenges.
+
+    :param credential: An object which can provide an access token for the vault, such as a credential from
+        :mod:`azure.identity`
+    :type credential: :class:`~azure.core.credentials.TokenCredential`
+    """
 
     def __init__(self, credential: "TokenCredential", *scopes: str, **kwargs) -> None:
         super(ChallengeAuthPolicy, self).__init__(credential, *scopes, **kwargs)
         self._credential = credential
-        self._token = None  # type: Optional[AccessToken]
+        self._token: "Optional[AccessToken]" = None
         self._verify_challenge_resource = kwargs.pop("verify_challenge_resource", True)
 
     def on_request(self, request: PipelineRequest) -> None:
         _enforce_tls(request)
         challenge = ChallengeCache.get_challenge_for_url(request.http_request.url)
         if challenge:
             # Note that if the vault has moved to a new tenant since our last request for it, this request will fail.
```

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/async_client_base.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_shared/async_client_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,19 +55,19 @@
                 api_version=self.api_version,
                 authentication_policy=AsyncChallengeAuthPolicy(credential, verify_challenge_resource=verify_challenge),
                 sdk_moniker=SDK_MONIKER,
                 http_logging_policy=http_logging_policy,
                 **kwargs
             )
             self._models = _KeyVaultClient.models(api_version=self.api_version)
-        except ValueError:
+        except ValueError as exc:
             raise NotImplementedError(
                 f"This package doesn't support API version '{self.api_version}'. "
                 + f"Supported versions: {', '.join(v.value for v in ApiVersion)}"
-            )
+            ) from exc
 
     @property
     def vault_url(self) -> str:
         return self._vault_url
 
     async def __aenter__(self) -> "AsyncKeyVaultClientBase":
         await self._client.__aenter__()
```

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/http_challenge_cache.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_shared/http_challenge_cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 # ------------------------------------
 # Copyright (c) Microsoft Corporation.
 # Licensed under the MIT License.
 # ------------------------------------
 import threading
+from typing import TYPE_CHECKING
 from urllib import parse
 
-try:
-    from typing import TYPE_CHECKING
-except ImportError:
-    TYPE_CHECKING = False
-
 if TYPE_CHECKING:
     # pylint: disable=unused-import
     from typing import Dict, Optional
     from .http_challenge import HttpChallenge
 
 
-_cache = {}  # type: Dict[str, HttpChallenge]
+_cache: "Dict[str, HttpChallenge]" = {}
 _lock = threading.Lock()
 
 
 def get_challenge_for_url(url: str) -> "Optional[HttpChallenge]":
     """Gets the challenge for the cached URL.
 
     :param str url: the URL the challenge is cached for.
+
+    :returns: The challenge for the cached request URL, or None if the request URL isn't cached.
+    :rtype: HttpChallenge or None
     """
 
     if not url:
         raise ValueError("URL cannot be None")
 
     key = _get_cache_key(url)
 
@@ -37,15 +36,21 @@
 
 def _get_cache_key(url: str) -> str:
     """Use the URL's netloc as cache key except when the URL specifies the default port for its scheme. In that case
     use the netloc without the port. That is to say, https://foo.bar and https://foo.bar:443 are considered equivalent.
 
     This equivalency prevents an unnecessary challenge when using Key Vault's paging API. The Key Vault client doesn't
     specify ports, but Key Vault's next page links do, so a redundant challenge would otherwise be executed when the
-    client requests the next page."""
+    client requests the next page.
+
+    :param str url: The HTTP request URL.
+
+    :returns: The URL's `netloc`, minus any port attached to the URL.
+    :rtype: str
+    """
 
     parsed = parse.urlparse(url)
     if parsed.scheme == "https" and parsed.port == 443:
         return parsed.netloc[:-4]
     return parsed.netloc
```

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/async_challenge_auth_policy.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_shared/async_challenge_auth_policy.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,27 +20,32 @@
 
 from azure.core.pipeline.policies import AsyncBearerTokenCredentialPolicy
 
 from . import http_challenge_cache as ChallengeCache
 from .challenge_auth_policy import _enforce_tls, _update_challenge
 
 if TYPE_CHECKING:
-    from typing import Any, Optional
+    from typing import Optional
     from azure.core.credentials import AccessToken
     from azure.core.credentials_async import AsyncTokenCredential
     from azure.core.pipeline import PipelineRequest, PipelineResponse
 
 
 class AsyncChallengeAuthPolicy(AsyncBearerTokenCredentialPolicy):
-    """policy for handling HTTP authentication challenges"""
+    """Policy for handling HTTP authentication challenges.
+
+    :param credential: An object which can provide an access token for the vault, such as a credential from
+        :mod:`azure.identity.aio`
+    :type credential: :class:`~azure.core.credentials_async.AsyncTokenCredential`
+    """
 
     def __init__(self, credential: "AsyncTokenCredential", *scopes: str, **kwargs) -> None:
         super().__init__(credential, *scopes, **kwargs)
         self._credential = credential
-        self._token = None  # type: Optional[AccessToken]
+        self._token: "Optional[AccessToken]" = None
         self._verify_challenge_resource = kwargs.pop("verify_challenge_resource", True)
 
     async def on_request(self, request: "PipelineRequest") -> None:
         _enforce_tls(request)
         challenge = ChallengeCache.get_challenge_for_url(request.http_request.url)
         if challenge:
             # Note that if the vault has moved to a new tenant since our last request for it, this request will fail.
```

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/__init__.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_shared/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,16 +45,16 @@
         self.name = name
         self.version = version
 
 
 def parse_key_vault_id(source_id: str) -> KeyVaultResourceId:
     try:
         parsed_uri = parse.urlparse(source_id)
-    except Exception:  # pylint: disable=broad-except
-        raise ValueError(f"'{source_id}' is not a valid ID")
+    except Exception as exc:  # pylint: disable=broad-except
+        raise ValueError(f"'{source_id}' is not a valid ID") from exc
     if not (parsed_uri.scheme and parsed_uri.hostname):
         raise ValueError(f"'{source_id}' is not a valid ID")
 
     path = list(filter(None, parsed_uri.path.split("/")))
 
     if len(path) < 2 or len(path) > 3:
         raise ValueError(f"'{source_id}' is not a valid ID")
```

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_shared/client_base.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_shared/client_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,15 +38,23 @@
 DEFAULT_VERSION = ApiVersion.V7_4
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
 def _format_api_version(request: "HttpRequest", api_version: str) -> "HttpRequest":
-    """Returns a request copy that includes an api-version query parameter if one wasn't originally present."""
+    """Returns a request copy that includes an api-version query parameter if one wasn't originally present.
+
+    :param request: The HTTP request being sent.
+    :type request: :class:`~azure.core.rest.HttpRequest`
+    :param str api_version: The service API version that the request should include.
+
+    :returns: A copy of the request that includes an api-version query parameter.
+    :rtype: :class:`~azure.core.rest.HttpRequest`
+    """
     request_copy = deepcopy(request)
     params = {"api-version": api_version}  # By default, we want to use the client's API version
     query = urlparse(request_copy.url).query
 
     if query:
         request_copy.url = request_copy.url.partition("?")[0]
         existing_params = {p[0]: p[-1] for p in [p.partition("=") for p in query.split("&")]}
@@ -97,19 +105,19 @@
                 api_version=self.api_version,
                 authentication_policy=ChallengeAuthPolicy(credential, verify_challenge_resource=verify_challenge),
                 sdk_moniker=SDK_MONIKER,
                 http_logging_policy=http_logging_policy,
                 **kwargs
             )
             self._models = _KeyVaultClient.models(api_version=self.api_version)
-        except ValueError:
+        except ValueError as exc:
             raise NotImplementedError(
                 f"This package doesn't support API version '{self.api_version}'. "
                 + f"Supported versions: {', '.join(v.value for v in ApiVersion)}"
-            )
+            ) from exc
 
     @property
     def vault_url(self) -> str:
         return self._vault_url
 
     def __enter__(self) -> "KeyVaultClientBase":
         self._client.__enter__()
```

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/_operations_mixin.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/_operations_mixin.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/_configuration.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/_key_vault_client.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/_serialization.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/_serialization.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/__init__.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/_configuration.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/_patch.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/_key_vault_client.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/__init__.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/_vendor.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/operations/_key_vault_client_operations.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/operations/_key_vault_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/operations/_patch.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/operations/__init__.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/models/_patch.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/models/_key_vault_client_enums.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/models/_key_vault_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/models/_models_py3.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/models/__init__.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/_configuration.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/aio/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/_patch.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/_key_vault_client.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/aio/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/__init__.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/_vendor.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/aio/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/operations/_key_vault_client_operations.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/aio/operations/_key_vault_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/operations/_patch.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_0/aio/operations/__init__.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/aio/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/_configuration.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/_patch.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/_key_vault_client.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/__init__.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/_vendor.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/operations/_key_vault_client_operations.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/operations/_key_vault_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/operations/_patch.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/operations/__init__.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/models/_patch.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/models/_key_vault_client_enums.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/models/_key_vault_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/models/_models_py3.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/models/__init__.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/_configuration.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/aio/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/_patch.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/_key_vault_client.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/aio/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/__init__.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/_vendor.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/aio/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/operations/_key_vault_client_operations.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_1/aio/operations/_key_vault_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/operations/_patch.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_1/aio/operations/__init__.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/aio/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/_configuration.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/_patch.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/_key_vault_client.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/__init__.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/_vendor.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/operations/_key_vault_client_operations.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/operations/_key_vault_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/operations/_patch.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/operations/__init__.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/models/_patch.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/models/_key_vault_client_enums.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/models/_key_vault_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/models/_models_py3.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/models/__init__.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/_configuration.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/aio/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/_patch.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/_key_vault_client.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/aio/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/__init__.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/_vendor.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/aio/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/operations/_key_vault_client_operations.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_2/aio/operations/_key_vault_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/operations/_patch.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_2/aio/operations/__init__.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/aio/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/_configuration.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/_patch.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/_key_vault_client.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/__init__.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/_vendor.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/operations/_key_vault_client_operations.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/operations/_key_vault_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/operations/_patch.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/operations/__init__.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/models/_patch.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/models/_key_vault_client_enums.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/models/_key_vault_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/models/_models_py3.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/models/__init__.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/_configuration.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/aio/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/_patch.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/_key_vault_client.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/aio/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/__init__.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/_vendor.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/aio/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/operations/_key_vault_client_operations.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_3/aio/operations/_key_vault_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/operations/_patch.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_3/aio/operations/__init__.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/_configuration.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/_patch.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/_key_vault_client.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/__init__.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/_vendor.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/operations/_key_vault_client_operations.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/operations/_key_vault_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/operations/_patch.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/operations/__init__.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/models/_patch.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/models/_key_vault_client_enums.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/models/_key_vault_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/models/_models_py3.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/models/__init__.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/_configuration.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/aio/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/_patch.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/_key_vault_client.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/aio/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/__init__.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/_vendor.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/aio/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/_key_vault_client_operations.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/_key_vault_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/_patch.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v2016_10_01/aio/operations/__init__.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_0/aio/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/aio/_operations_mixin.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/aio/_operations_mixin.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/aio/_configuration.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/aio/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/aio/_key_vault_client.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/aio/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/aio/__init__.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/_configuration.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/_patch.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/_key_vault_client.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/__init__.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/_vendor.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/operations/_key_vault_client_operations.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/operations/_key_vault_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/operations/_patch.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/models/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/operations/__init__.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/models/_patch.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/models/_key_vault_client_enums.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/models/_key_vault_client_enums.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/models/_models_py3.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/models/_models_py3.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/models/__init__.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/models/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/_configuration.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/aio/_configuration.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/_patch.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/aio/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/_key_vault_client.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/aio/_key_vault_client.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/__init__.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/aio/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/_vendor.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/aio/_vendor.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/operations/_key_vault_client_operations.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/aio/operations/_key_vault_client_operations.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/operations/_patch.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/aio/operations/_patch.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/_generated/v7_4/aio/operations/__init__.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/_generated/v7_4/aio/operations/__init__.py`

 * *Files identical despite different names*

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/aio/_client.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/aio/_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     CertificateIssuer,
     IssuerProperties,
 )
 from ._polling_async import CreateCertificatePollerAsync
 from .._client import NO_SAN_OR_SUBJECT
 from .._shared import AsyncKeyVaultClientBase
 from .._shared._polling_async import AsyncDeleteRecoverPollingMethod
-from .._shared.exceptions import error_map as _error_map
 
 
 class CertificateClient(AsyncKeyVaultClientBase):
     """A high-level asynchronous interface for managing a vault's certificates.
 
     :param str vault_url: URL of the vault the client will access. This is also called the vault's "DNS Name".
         You should validate that this URL references a valid Key Vault resource. See https://aka.ms/azsdk/blog/vault-uri
@@ -108,28 +107,29 @@
             tags=kwargs.pop("tags", None),
         )
 
         cert_bundle = await self._client.create_certificate(
             vault_base_url=self.vault_url,
             certificate_name=certificate_name,
             parameters=parameters,
-            error_map=_error_map,
             **kwargs
         )
 
         create_certificate_operation = CertificateOperation._from_certificate_operation_bundle(cert_bundle)
 
         command = partial(self.get_certificate_operation, certificate_name=certificate_name, **kwargs)
 
         get_certificate_command = partial(self.get_certificate, certificate_name=certificate_name, **kwargs)
 
         create_certificate_polling = CreateCertificatePollerAsync(
             get_certificate_command=get_certificate_command, interval=polling_interval
         )
-        return await async_poller(command, create_certificate_operation, None, create_certificate_polling)
+        def no_op(*_, **__) -> Any:  # The deserialization callback is ignored based on polling implementation
+            pass
+        return await async_poller(command, create_certificate_operation, no_op, create_certificate_polling)
 
     @distributed_trace_async
     async def get_certificate(self, certificate_name: str, **kwargs) -> KeyVaultCertificate:
         """Gets a certificate with its management policy attached. Requires certificates/get permission.
 
         Does not accept the version of the certificate as a parameter. To get a specific version of the
         certificate, call :func:`get_certificate_version`.
@@ -151,15 +151,14 @@
                 :caption: Get a certificate
                 :dedent: 8
         """
         bundle = await self._client.get_certificate(
             vault_base_url=self.vault_url,
             certificate_name=certificate_name,
             certificate_version="",
-            error_map=_error_map,
             **kwargs
         )
         return KeyVaultCertificate._from_certificate_bundle(certificate_bundle=bundle)
 
     @distributed_trace_async
     async def get_certificate_version(
         self, certificate_name: str, version: str, **kwargs
@@ -187,15 +186,14 @@
                 :caption: Get a certificate with a specific version
                 :dedent: 8
         """
         bundle = await self._client.get_certificate(
             vault_base_url=self.vault_url,
             certificate_name=certificate_name,
             certificate_version=version,
-            error_map=_error_map,
             **kwargs
         )
         return KeyVaultCertificate._from_certificate_bundle(certificate_bundle=bundle)
 
     @distributed_trace_async
     async def delete_certificate(self, certificate_name: str, **kwargs) -> DeletedCertificate:
         """Delete all versions of a certificate. Requires certificates/delete permission.
@@ -219,15 +217,15 @@
                 :caption: Delete a certificate
                 :dedent: 8
         """
         polling_interval = kwargs.pop("_polling_interval", None)
         if polling_interval is None:
             polling_interval = 2
         deleted_cert_bundle = await self._client.delete_certificate(
-            vault_base_url=self.vault_url, certificate_name=certificate_name, error_map=_error_map, **kwargs
+            vault_base_url=self.vault_url, certificate_name=certificate_name, **kwargs
         )
         deleted_certificate = DeletedCertificate._from_deleted_certificate_bundle(deleted_cert_bundle)
 
         polling_method = AsyncDeleteRecoverPollingMethod(
             # no recovery ID means soft-delete is disabled, in which case we initialize the poller as finished
             finished=deleted_certificate.recovery_id is None,
             command=partial(self.get_deleted_certificate, certificate_name=certificate_name, **kwargs),
@@ -259,15 +257,15 @@
                 :start-after: [START get_deleted_certificate]
                 :end-before: [END get_deleted_certificate]
                 :language: python
                 :caption: Get a deleted certificate
                 :dedent: 8
         """
         bundle = await self._client.get_deleted_certificate(
-            vault_base_url=self.vault_url, certificate_name=certificate_name, error_map=_error_map, **kwargs
+            vault_base_url=self.vault_url, certificate_name=certificate_name, **kwargs
         )
         return DeletedCertificate._from_deleted_certificate_bundle(deleted_certificate_bundle=bundle)
 
     @distributed_trace_async
     async def purge_deleted_certificate(self, certificate_name: str, **kwargs) -> None:
         """Permanently deletes a deleted certificate. Possible only in vaults with soft-delete enabled.
 
@@ -281,15 +279,15 @@
 
         :return: None
         :rtype: None
 
         :raises: :class:`~azure.core.exceptions.HttpResponseError`
         """
         await self._client.purge_deleted_certificate(
-            vault_base_url=self.vault_url, certificate_name=certificate_name, error_map=_error_map, **kwargs
+            vault_base_url=self.vault_url, certificate_name=certificate_name, **kwargs
         )
 
     @distributed_trace_async
     async def recover_deleted_certificate(self, certificate_name: str, **kwargs) -> KeyVaultCertificate:
         """Recover a deleted certificate to its latest version. Possible only in a vault with soft-delete enabled.
 
         Requires certificates/recover permission. If the vault does not have soft-delete enabled,
@@ -311,15 +309,15 @@
                 :caption: Recover a deleted certificate
                 :dedent: 8
         """
         polling_interval = kwargs.pop("_polling_interval", None)
         if polling_interval is None:
             polling_interval = 2
         recovered_cert_bundle = await self._client.recover_deleted_certificate(
-            vault_base_url=self.vault_url, certificate_name=certificate_name, error_map=_error_map, **kwargs
+            vault_base_url=self.vault_url, certificate_name=certificate_name, **kwargs
         )
         recovered_certificate = KeyVaultCertificate._from_certificate_bundle(recovered_cert_bundle)
 
         command = partial(self.get_certificate, certificate_name=certificate_name, **kwargs)
         polling_method = AsyncDeleteRecoverPollingMethod(
             command=command, final_resource=recovered_certificate, finished=False, interval=polling_interval
         )
@@ -376,15 +374,14 @@
             tags=kwargs.pop("tags", None),
         )
 
         bundle = await self._client.import_certificate(
             vault_base_url=self.vault_url,
             certificate_name=certificate_name,
             parameters=parameters,
-            error_map=_error_map,
             **kwargs
         )
         return KeyVaultCertificate._from_certificate_bundle(certificate_bundle=bundle)
 
     @distributed_trace_async
     async def get_certificate_policy(self, certificate_name: str, **kwargs) -> CertificatePolicy:
         """Gets the policy for a certificate. Requires certificates/get permission.
@@ -395,15 +392,15 @@
 
         :return: The certificate policy
         :rtype: ~azure.keyvault.certificates.CertificatePolicy
 
         :raises: :class:`~azure.core.exceptions.HttpResponseError`
         """
         bundle = await self._client.get_certificate_policy(
-            vault_base_url=self.vault_url, certificate_name=certificate_name, error_map=_error_map, **kwargs
+            vault_base_url=self.vault_url, certificate_name=certificate_name, **kwargs
         )
         return CertificatePolicy._from_certificate_policy_bundle(certificate_policy_bundle=bundle)
 
     @distributed_trace_async
     async def update_certificate_policy(
         self, certificate_name: str, policy: CertificatePolicy, **kwargs
     ) -> CertificatePolicy:
@@ -420,15 +417,14 @@
 
         :raises: :class:`~azure.core.exceptions.HttpResponseError`
         """
         bundle = await self._client.update_certificate_policy(
             vault_base_url=self.vault_url,
             certificate_name=certificate_name,
             certificate_policy=policy._to_certificate_policy_bundle(),
-            error_map=_error_map,
             **kwargs
         )
         return CertificatePolicy._from_certificate_policy_bundle(certificate_policy_bundle=bundle)
 
     @distributed_trace_async
     async def update_certificate_properties(
         self, certificate_name: str, version: Optional[str] = None, **kwargs
@@ -468,15 +464,14 @@
         )
 
         bundle = await self._client.update_certificate(
             vault_base_url=self.vault_url,
             certificate_name=certificate_name,
             certificate_version=version or "",
             parameters=parameters,
-            error_map=_error_map,
             **kwargs
         )
         return KeyVaultCertificate._from_certificate_bundle(certificate_bundle=bundle)
 
     @distributed_trace_async
     async def backup_certificate(self, certificate_name: str, **kwargs) -> bytes:
         """Back up a certificate in a protected form useable only by Azure Key Vault.
@@ -500,15 +495,15 @@
                 :start-after: [START backup_certificate]
                 :end-before: [END backup_certificate]
                 :language: python
                 :caption: Get a certificate backup
                 :dedent: 8
         """
         backup_result = await self._client.backup_certificate(
-            vault_base_url=self.vault_url, certificate_name=certificate_name, error_map=_error_map, **kwargs
+            vault_base_url=self.vault_url, certificate_name=certificate_name, **kwargs
         )
         return backup_result.value
 
     @distributed_trace_async
     async def restore_certificate_backup(self, backup: bytes, **kwargs) -> KeyVaultCertificate:
         """Restore a certificate backup to the vault. Requires certificates/restore permission.
 
@@ -530,15 +525,14 @@
                 :language: python
                 :caption: Restore a certificate backup
                 :dedent: 8
         """
         bundle = await self._client.restore_certificate(
             vault_base_url=self.vault_url,
             parameters=self._models.CertificateRestoreParameters(certificate_bundle_backup=backup),
-            error_map=_error_map,
             **kwargs
         )
         return KeyVaultCertificate._from_certificate_bundle(certificate_bundle=bundle)
 
     @distributed_trace
     def list_deleted_certificates(self, **kwargs) -> AsyncItemPaged[DeletedCertificate]:
         """Lists the currently-recoverable deleted certificates. Possible only if vault is soft-delete enabled.
@@ -663,15 +657,14 @@
                 :language: python
                 :caption: Create contacts
                 :dedent: 8
         """
         new_contacts = await self._client.set_certificate_contacts(
             vault_base_url=self.vault_url,
             contacts=self._models.Contacts(contact_list=[c._to_certificate_contacts_item() for c in contacts]),
-            error_map=_error_map,
             **kwargs
         )
         return [
             CertificateContact._from_certificate_contacts_item(contact_item=item) for item in new_contacts.contact_list
         ]
 
     @distributed_trace_async
@@ -688,15 +681,15 @@
                 :start-after: [START get_contacts]
                 :end-before: [END get_contacts]
                 :language: python
                 :caption: Get contacts
                 :dedent: 8
         """
         contacts = await self._client.get_certificate_contacts(
-            vault_base_url=self._vault_url, error_map=_error_map, **kwargs
+            vault_base_url=self._vault_url, **kwargs
         )
         return [CertificateContact._from_certificate_contacts_item(contact_item=item) for item in contacts.contact_list]
 
     @distributed_trace_async
     async def delete_contacts(self, **kwargs) -> List[CertificateContact]:
         """Deletes the certificate contacts for the key vault. Requires the certificates/managecontacts permission.
 
@@ -710,15 +703,15 @@
                 :start-after: [START delete_contacts]
                 :end-before: [END delete_contacts]
                 :language: python
                 :caption: Delete contacts
                 :dedent: 8
         """
         contacts = await self._client.delete_certificate_contacts(
-            vault_base_url=self.vault_url, error_map=_error_map, **kwargs
+            vault_base_url=self.vault_url, **kwargs
         )
         return [CertificateContact._from_certificate_contacts_item(contact_item=item) for item in contacts.contact_list]
 
     @distributed_trace_async
     async def get_certificate_operation(self, certificate_name: str, **kwargs) -> CertificateOperation:
         """Gets the creation operation of a certificate. Requires the certificates/get permission.
 
@@ -729,15 +722,15 @@
 
         :raises:
             :class:`~azure.core.exceptions.ResourceNotFoundError` if the certificate doesn't exist,
             :class:`~azure.core.exceptions.HttpResponseError` for other errors
         """
 
         bundle = await self._client.get_certificate_operation(
-            vault_base_url=self.vault_url, certificate_name=certificate_name, error_map=_error_map, **kwargs
+            vault_base_url=self.vault_url, certificate_name=certificate_name, **kwargs
         )
         return CertificateOperation._from_certificate_operation_bundle(certificate_operation_bundle=bundle)
 
     @distributed_trace_async
     async def delete_certificate_operation(self, certificate_name: str, **kwargs) -> CertificateOperation:
         """Deletes and stops the creation operation for a specific certificate.
 
@@ -749,15 +742,15 @@
         :rtype: ~azure.keyvault.certificates.CertificateOperation
 
         :raises:
             :class:`~azure.core.exceptions.ResourceNotFoundError` if the operation doesn't exist,
             :class:`~azure.core.exceptions.HttpResponseError` for other errors
         """
         bundle = await self._client.delete_certificate_operation(
-            vault_base_url=self.vault_url, certificate_name=certificate_name, error_map=_error_map, **kwargs
+            vault_base_url=self.vault_url, certificate_name=certificate_name, **kwargs
         )
         return CertificateOperation._from_certificate_operation_bundle(certificate_operation_bundle=bundle)
 
     @distributed_trace_async
     async def cancel_certificate_operation(self, certificate_name: str, **kwargs) -> CertificateOperation:
         """Cancels an in-progress certificate operation. Requires the certificates/update permission.
 
@@ -768,15 +761,14 @@
 
         :raises: :class:`~azure.core.exceptions.HttpResponseError`
         """
         bundle = await self._client.update_certificate_operation(
             vault_base_url=self.vault_url,
             certificate_name=certificate_name,
             certificate_operation=self._models.CertificateOperationUpdateParameter(cancellation_requested=True),
-            error_map=_error_map,
             **kwargs
         )
         return CertificateOperation._from_certificate_operation_bundle(certificate_operation_bundle=bundle)
 
     @distributed_trace_async
     async def merge_certificate(
         self, certificate_name: str, x509_certificates: List[bytes], **kwargs
@@ -813,15 +805,14 @@
             x509_certificates=x509_certificates, certificate_attributes=attributes, tags=kwargs.pop("tags", None)
         )
 
         bundle = await self._client.merge_certificate(
             vault_base_url=self.vault_url,
             certificate_name=certificate_name,
             parameters=parameters,
-            error_map=_error_map,
             **kwargs
         )
         return KeyVaultCertificate._from_certificate_bundle(certificate_bundle=bundle)
 
     @distributed_trace_async
     async def get_issuer(self, issuer_name: str, **kwargs) -> CertificateIssuer:
         """Gets the specified certificate issuer. Requires certificates/manageissuers/getissuers permission.
@@ -840,15 +831,15 @@
                 :start-after: [START get_issuer]
                 :end-before: [END get_issuer]
                 :language: python
                 :caption: Get an issuer
                 :dedent: 8
         """
         issuer_bundle = await self._client.get_certificate_issuer(
-            vault_base_url=self.vault_url, issuer_name=issuer_name, error_map=_error_map, **kwargs
+            vault_base_url=self.vault_url, issuer_name=issuer_name, **kwargs
         )
         return CertificateIssuer._from_issuer_bundle(issuer_bundle=issuer_bundle)
 
     @distributed_trace_async
     async def create_issuer(self, issuer_name: str, provider: str, **kwargs) -> CertificateIssuer:
         """Sets the specified certificate issuer. Requires certificates/setissuers permission.
 
@@ -884,23 +875,23 @@
         admin_contacts = kwargs.pop("admin_contacts", None)
 
         if account_id or password:
             issuer_credentials = self._models.IssuerCredentials(account_id=account_id, password=password)
         else:
             issuer_credentials = None
         if admin_contacts:
-            admin_details = [
+            admin_details: Optional[List[Any]] = [
                 self._models.AdministratorDetails(
                     first_name=contact.first_name,
                     last_name=contact.last_name,
                     email_address=contact.email,
                     phone=contact.phone,
                 )
                 for contact in admin_contacts
-            ]  # type: Optional[List[Any]]
+            ]
         else:
             admin_details = None
         if organization_id or admin_details:
             organization_details = self._models.OrganizationDetails(id=organization_id, admin_details=admin_details)
         else:
             organization_details = None
         if enabled is not None:
@@ -912,15 +903,15 @@
             provider=provider,
             credentials=issuer_credentials,
             organization_details=organization_details,
             attributes=issuer_attributes,
         )
 
         issuer_bundle = await self._client.set_certificate_issuer(
-            vault_base_url=self.vault_url, issuer_name=issuer_name, parameter=parameters, error_map=_error_map, **kwargs
+            vault_base_url=self.vault_url, issuer_name=issuer_name, parameter=parameters, **kwargs
         )
         return CertificateIssuer._from_issuer_bundle(issuer_bundle=issuer_bundle)
 
     @distributed_trace_async
     async def update_issuer(self, issuer_name: str, **kwargs) -> CertificateIssuer:
         """Updates the specified certificate issuer. Requires certificates/setissuers permission.
 
@@ -948,23 +939,23 @@
         admin_contacts = kwargs.pop("admin_contacts", None)
 
         if account_id or password:
             issuer_credentials = self._models.IssuerCredentials(account_id=account_id, password=password)
         else:
             issuer_credentials = None
         if admin_contacts:
-            admin_details = list(
+            admin_details: Optional[List[Any]] = list(
                 self._models.AdministratorDetails(
                     first_name=contact.first_name,
                     last_name=contact.last_name,
                     email_address=contact.email,
                     phone=contact.phone,
                 )
                 for contact in admin_contacts
-            )  # type: Optional[List[Any]]
+            )
         else:
             admin_details = None
         if organization_id or admin_details:
             organization_details = self._models.OrganizationDetails(id=organization_id, admin_details=admin_details)
         else:
             organization_details = None
         if enabled is not None:
@@ -976,15 +967,15 @@
             provider=kwargs.pop("provider", None),
             credentials=issuer_credentials,
             organization_details=organization_details,
             attributes=issuer_attributes,
         )
 
         issuer_bundle = await self._client.update_certificate_issuer(
-            vault_base_url=self.vault_url, issuer_name=issuer_name, parameter=parameters, error_map=_error_map, **kwargs
+            vault_base_url=self.vault_url, issuer_name=issuer_name, parameter=parameters, **kwargs
         )
         return CertificateIssuer._from_issuer_bundle(issuer_bundle=issuer_bundle)
 
     @distributed_trace_async
     async def delete_issuer(self, issuer_name: str, **kwargs) -> CertificateIssuer:
         """Deletes the specified certificate issuer.
 
@@ -1002,15 +993,15 @@
                 :start-after: [START delete_issuer]
                 :end-before: [END delete_issuer]
                 :language: python
                 :caption: Delete an issuer
                 :dedent: 8
         """
         issuer_bundle = await self._client.delete_certificate_issuer(
-            vault_base_url=self.vault_url, issuer_name=issuer_name, error_map=_error_map, **kwargs
+            vault_base_url=self.vault_url, issuer_name=issuer_name, **kwargs
         )
         return CertificateIssuer._from_issuer_bundle(issuer_bundle=issuer_bundle)
 
     @distributed_trace
     def list_properties_of_issuers(self, **kwargs) -> AsyncItemPaged[IssuerProperties]:
         """Lists properties of the certificate issuers for the key vault.
```

## Comparing `azure-keyvault-certificates-4.8.0b1/azure/keyvault/certificates/aio/_polling_async.py` & `azure-keyvault-certificates-4.8.0b2/azure/keyvault/certificates/aio/_polling_async.py`

 * *Files identical despite different names*

