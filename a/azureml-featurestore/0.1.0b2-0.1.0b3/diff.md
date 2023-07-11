# Comparing `tmp/azureml_featurestore-0.1.0b2-py3-none-any.whl.zip` & `tmp/azureml_featurestore-0.1.0b3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,58 +1,76 @@
-Zip file size: 68490 bytes, number of entries: 56
--rw-rw-rw-  2.0 fat      267 b- defN 23-Jun-14 19:40 azureml/__init__.py
--rw-rw-rw-  2.0 fat      917 b- defN 23-Jun-14 19:40 azureml/featurestore/__init__.py
--rw-rw-rw-  2.0 fat    21202 b- defN 23-Jun-14 19:40 azureml/featurestore/_feature_set.py
--rw-rw-rw-  2.0 fat       21 b- defN 23-Jun-14 19:50 azureml/featurestore/_version.py
--rw-rw-rw-  2.0 fat     1108 b- defN 23-Jun-14 19:40 azureml/featurestore/abstract_feature_store.py
--rw-rw-rw-  2.0 fat    25045 b- defN 23-Jun-14 19:40 azureml/featurestore/feature_set_spec.py
--rw-rw-rw-  2.0 fat    26844 b- defN 23-Jun-14 19:40 azureml/featurestore/feature_store_client.py
--rw-rw-rw-  2.0 fat      410 b- defN 23-Jun-14 19:40 azureml/featurestore/_identity/__init__.py
--rw-rw-rw-  2.0 fat     6334 b- defN 23-Jun-14 19:40 azureml/featurestore/_identity/aml_hobospark_on_behalf_of.py
--rw-rw-rw-  2.0 fat      455 b- defN 23-Jun-14 19:40 azureml/featurestore/_offline_query/__init__.py
--rw-rw-rw-  2.0 fat      401 b- defN 23-Jun-14 19:40 azureml/featurestore/_offline_query/offline_retrieval_job.py
--rw-rw-rw-  2.0 fat    10931 b- defN 23-Jun-14 19:40 azureml/featurestore/_offline_query/point_at_time.py
--rw-rw-rw-  2.0 fat      267 b- defN 23-Jun-14 19:40 azureml/featurestore/_utils/__init__.py
--rw-rw-rw-  2.0 fat     1694 b- defN 23-Jun-14 19:40 azureml/featurestore/_utils/_constants.py
--rw-rw-rw-  2.0 fat      398 b- defN 23-Jun-14 19:40 azureml/featurestore/_utils/_preview_method.py
--rw-rw-rw-  2.0 fat     7359 b- defN 23-Jun-14 19:40 azureml/featurestore/_utils/arm_id_utils.py
--rw-rw-rw-  2.0 fat     2564 b- defN 23-Jun-14 19:40 azureml/featurestore/_utils/error_constants.py
--rw-rw-rw-  2.0 fat     5732 b- defN 23-Jun-14 19:40 azureml/featurestore/_utils/materialize.py
--rw-rw-rw-  2.0 fat     9728 b- defN 23-Jun-14 19:40 azureml/featurestore/_utils/spark_utils.py
--rw-rw-rw-  2.0 fat     2370 b- defN 23-Jun-14 19:40 azureml/featurestore/_utils/type_map.py
--rw-rw-rw-  2.0 fat    15684 b- defN 23-Jun-14 19:40 azureml/featurestore/_utils/utils.py
--rw-rw-rw-  2.0 fat      681 b- defN 23-Jun-14 19:40 azureml/featurestore/contracts/__init__.py
--rw-rw-rw-  2.0 fat     1243 b- defN 23-Jun-14 19:40 azureml/featurestore/contracts/column.py
--rw-rw-rw-  2.0 fat     1058 b- defN 23-Jun-14 19:40 azureml/featurestore/contracts/datetimeoffset.py
--rw-rw-rw-  2.0 fat     3593 b- defN 23-Jun-14 19:40 azureml/featurestore/contracts/feature.py
--rw-rw-rw-  2.0 fat     9258 b- defN 23-Jun-14 19:40 azureml/featurestore/contracts/feature_retrieval_spec.py
--rw-rw-rw-  2.0 fat     2846 b- defN 23-Jun-14 19:40 azureml/featurestore/contracts/feature_source.py
--rw-rw-rw-  2.0 fat     2019 b- defN 23-Jun-14 19:40 azureml/featurestore/contracts/offline_store.py
--rw-rw-rw-  2.0 fat      646 b- defN 23-Jun-14 19:40 azureml/featurestore/contracts/online_store.py
--rw-rw-rw-  2.0 fat      694 b- defN 23-Jun-14 19:40 azureml/featurestore/contracts/partition.py
--rw-rw-rw-  2.0 fat     1230 b- defN 23-Jun-14 19:40 azureml/featurestore/contracts/store_connection.py
--rw-rw-rw-  2.0 fat      753 b- defN 23-Jun-14 19:40 azureml/featurestore/contracts/timestamp_column.py
--rw-rw-rw-  2.0 fat     2530 b- defN 23-Jun-14 19:40 azureml/featurestore/contracts/transformation_code.py
--rw-rw-rw-  2.0 fat      294 b- defN 23-Jun-14 19:40 azureml/featurestore/grpc/__init__.py
--rw-rw-rw-  2.0 fat     1364 b- defN 23-Jun-14 19:40 azureml/featurestore/grpc/_flight_feature_retrieval_client.py
--rw-rw-rw-  2.0 fat     3276 b- defN 23-Jun-14 19:40 azureml/featurestore/grpc/_flight_feature_retrieval_server.py
--rw-rw-rw-  2.0 fat     5923 b- defN 23-Jun-14 19:40 azureml/featurestore/grpc/_flight_helper.py
--rw-rw-rw-  2.0 fat      934 b- defN 23-Jun-14 19:40 azureml/featurestore/grpc/_inline_feature_retrieval_client.py
--rw-rw-rw-  2.0 fat      391 b- defN 23-Jun-14 19:40 azureml/featurestore/offline_store/__init__.py
--rw-rw-rw-  2.0 fat     9020 b- defN 23-Jun-14 19:40 azureml/featurestore/offline_store/azure_data_lake_offline_store.py
--rw-rw-rw-  2.0 fat      367 b- defN 23-Jun-14 19:40 azureml/featurestore/offline_store/partition/__init__.py
--rw-rw-rw-  2.0 fat     2381 b- defN 23-Jun-14 19:40 azureml/featurestore/offline_store/partition/timestamp_partition.py
--rw-rw-rw-  2.0 fat      242 b- defN 23-Jun-14 19:40 azureml/featurestore/online/__init__.py
--rw-rw-rw-  2.0 fat     5515 b- defN 23-Jun-14 19:40 azureml/featurestore/online/_online_feature_getter.py
--rw-rw-rw-  2.0 fat     5571 b- defN 23-Jun-14 19:40 azureml/featurestore/online/_online_feature_materialization.py
--rw-rw-rw-  2.0 fat     1669 b- defN 23-Jun-14 19:40 azureml/featurestore/online/_redis_client_pool.py
--rw-rw-rw-  2.0 fat     1055 b- defN 23-Jun-14 19:40 azureml/featurestore/online/_utils.py
--rw-rw-rw-  2.0 fat      267 b- defN 23-Jun-14 19:40 azureml/featurestore/schema/__init__.py
--rw-rw-rw-  2.0 fat     1655 b- defN 23-Jun-14 19:40 azureml/featurestore/schema/feature_retrieval_spec_schema.py
--rw-rw-rw-  2.0 fat     5944 b- defN 23-Jun-14 19:40 azureml/featurestore/schema/feature_set_schema.py
--rw-rw-rw-  2.0 fat     1047 b- defN 23-Jun-14 19:53 azureml_featurestore-0.1.0b2.dist-info/DESCRIPTION.rst
--rw-rw-rw-  2.0 fat     1142 b- defN 23-Jun-14 19:53 azureml_featurestore-0.1.0b2.dist-info/metadata.json
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-14 19:53 azureml_featurestore-0.1.0b2.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat       97 b- defN 23-Jun-14 19:53 azureml_featurestore-0.1.0b2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat     2145 b- defN 23-Jun-14 19:53 azureml_featurestore-0.1.0b2.dist-info/METADATA
--rw-rw-rw-  2.0 fat     5804 b- defN 23-Jun-14 19:53 azureml_featurestore-0.1.0b2.dist-info/RECORD
-56 files, 222393 bytes uncompressed, 58954 bytes compressed:  73.5%
+Zip file size: 84379 bytes, number of entries: 74
+-rw-rw-rw-  2.0 fat      267 b- defN 23-Jul-11 01:12 azureml/__init__.py
+-rw-rw-rw-  2.0 fat      917 b- defN 23-Jul-11 01:12 azureml/featurestore/__init__.py
+-rw-rw-rw-  2.0 fat    21202 b- defN 23-Jul-11 01:12 azureml/featurestore/_feature_set.py
+-rw-rw-rw-  2.0 fat       21 b- defN 23-Jul-11 01:19 azureml/featurestore/_version.py
+-rw-rw-rw-  2.0 fat     1108 b- defN 23-Jul-11 01:12 azureml/featurestore/abstract_feature_store.py
+-rw-rw-rw-  2.0 fat    25045 b- defN 23-Jul-11 01:12 azureml/featurestore/feature_set_spec.py
+-rw-rw-rw-  2.0 fat    26844 b- defN 23-Jul-11 01:12 azureml/featurestore/feature_store_client.py
+-rw-rw-rw-  2.0 fat      410 b- defN 23-Jul-11 01:12 azureml/featurestore/_identity/__init__.py
+-rw-rw-rw-  2.0 fat     6334 b- defN 23-Jul-11 01:12 azureml/featurestore/_identity/aml_hobospark_on_behalf_of.py
+-rw-rw-rw-  2.0 fat      455 b- defN 23-Jul-11 01:12 azureml/featurestore/_offline_query/__init__.py
+-rw-rw-rw-  2.0 fat      399 b- defN 23-Jul-11 01:12 azureml/featurestore/_offline_query/offline_retrieval_job.py
+-rw-rw-rw-  2.0 fat    10931 b- defN 23-Jul-11 01:12 azureml/featurestore/_offline_query/point_at_time.py
+-rw-rw-rw-  2.0 fat      267 b- defN 23-Jul-11 01:12 azureml/featurestore/_utils/__init__.py
+-rw-rw-rw-  2.0 fat     1694 b- defN 23-Jul-11 01:12 azureml/featurestore/_utils/_constants.py
+-rw-rw-rw-  2.0 fat      398 b- defN 23-Jul-11 01:12 azureml/featurestore/_utils/_preview_method.py
+-rw-rw-rw-  2.0 fat     7359 b- defN 23-Jul-11 01:12 azureml/featurestore/_utils/arm_id_utils.py
+-rw-rw-rw-  2.0 fat     2564 b- defN 23-Jul-11 01:12 azureml/featurestore/_utils/error_constants.py
+-rw-rw-rw-  2.0 fat     5732 b- defN 23-Jul-11 01:12 azureml/featurestore/_utils/materialize.py
+-rw-rw-rw-  2.0 fat     9728 b- defN 23-Jul-11 01:12 azureml/featurestore/_utils/spark_utils.py
+-rw-rw-rw-  2.0 fat     2370 b- defN 23-Jul-11 01:12 azureml/featurestore/_utils/type_map.py
+-rw-rw-rw-  2.0 fat    14558 b- defN 23-Jul-11 01:12 azureml/featurestore/_utils/utils.py
+-rw-rw-rw-  2.0 fat      681 b- defN 23-Jul-11 01:12 azureml/featurestore/contracts/__init__.py
+-rw-rw-rw-  2.0 fat     1243 b- defN 23-Jul-11 01:12 azureml/featurestore/contracts/column.py
+-rw-rw-rw-  2.0 fat     1058 b- defN 23-Jul-11 01:12 azureml/featurestore/contracts/datetimeoffset.py
+-rw-rw-rw-  2.0 fat     3593 b- defN 23-Jul-11 01:12 azureml/featurestore/contracts/feature.py
+-rw-rw-rw-  2.0 fat     9258 b- defN 23-Jul-11 01:12 azureml/featurestore/contracts/feature_retrieval_spec.py
+-rw-rw-rw-  2.0 fat     2846 b- defN 23-Jul-11 01:12 azureml/featurestore/contracts/feature_source.py
+-rw-rw-rw-  2.0 fat      489 b- defN 23-Jul-11 01:12 azureml/featurestore/contracts/feature_transformation.py
+-rw-rw-rw-  2.0 fat     2019 b- defN 23-Jul-11 01:12 azureml/featurestore/contracts/offline_store.py
+-rw-rw-rw-  2.0 fat      646 b- defN 23-Jul-11 01:12 azureml/featurestore/contracts/online_store.py
+-rw-rw-rw-  2.0 fat      694 b- defN 23-Jul-11 01:12 azureml/featurestore/contracts/partition.py
+-rw-rw-rw-  2.0 fat     1230 b- defN 23-Jul-11 01:12 azureml/featurestore/contracts/store_connection.py
+-rw-rw-rw-  2.0 fat      753 b- defN 23-Jul-11 01:12 azureml/featurestore/contracts/timestamp_column.py
+-rw-rw-rw-  2.0 fat     2640 b- defN 23-Jul-11 01:12 azureml/featurestore/contracts/transformation_code.py
+-rw-rw-rw-  2.0 fat      294 b- defN 23-Jul-11 01:12 azureml/featurestore/grpc/__init__.py
+-rw-rw-rw-  2.0 fat     1364 b- defN 23-Jul-11 01:12 azureml/featurestore/grpc/_flight_feature_retrieval_client.py
+-rw-rw-rw-  2.0 fat     3276 b- defN 23-Jul-11 01:12 azureml/featurestore/grpc/_flight_feature_retrieval_server.py
+-rw-rw-rw-  2.0 fat     5923 b- defN 23-Jul-11 01:12 azureml/featurestore/grpc/_flight_helper.py
+-rw-rw-rw-  2.0 fat      934 b- defN 23-Jul-11 01:12 azureml/featurestore/grpc/_inline_feature_retrieval_client.py
+-rw-rw-rw-  2.0 fat      391 b- defN 23-Jul-11 01:12 azureml/featurestore/offline_store/__init__.py
+-rw-rw-rw-  2.0 fat     9020 b- defN 23-Jul-11 01:12 azureml/featurestore/offline_store/azure_data_lake_offline_store.py
+-rw-rw-rw-  2.0 fat      367 b- defN 23-Jul-11 01:12 azureml/featurestore/offline_store/partition/__init__.py
+-rw-rw-rw-  2.0 fat     2381 b- defN 23-Jul-11 01:12 azureml/featurestore/offline_store/partition/timestamp_partition.py
+-rw-rw-rw-  2.0 fat      242 b- defN 23-Jul-11 01:12 azureml/featurestore/online/__init__.py
+-rw-rw-rw-  2.0 fat     5515 b- defN 23-Jul-11 01:12 azureml/featurestore/online/_online_feature_getter.py
+-rw-rw-rw-  2.0 fat     5573 b- defN 23-Jul-11 01:12 azureml/featurestore/online/_online_feature_materialization.py
+-rw-rw-rw-  2.0 fat     1669 b- defN 23-Jul-11 01:12 azureml/featurestore/online/_redis_client_pool.py
+-rw-rw-rw-  2.0 fat     1053 b- defN 23-Jul-11 01:12 azureml/featurestore/online/_utils.py
+-rw-rw-rw-  2.0 fat      267 b- defN 23-Jul-11 01:12 azureml/featurestore/schema/__init__.py
+-rw-rw-rw-  2.0 fat     1655 b- defN 23-Jul-11 01:12 azureml/featurestore/schema/feature_retrieval_spec_schema.py
+-rw-rw-rw-  2.0 fat     5944 b- defN 23-Jul-11 01:12 azureml/featurestore/schema/feature_set_schema.py
+-rw-rw-rw-  2.0 fat      183 b- defN 23-Jul-11 01:12 azureml/featurestore/transformation/__init__.py
+-rw-rw-rw-  2.0 fat      425 b- defN 23-Jul-11 01:12 azureml/featurestore/transformation/aggregation_function.py
+-rw-rw-rw-  2.0 fat      382 b- defN 23-Jul-11 01:12 azureml/featurestore/transformation/transformation_expression.py
+-rw-rw-rw-  2.0 fat      959 b- defN 23-Jul-11 01:12 azureml/featurestore/transformation/transformation_expression_collection.py
+-rw-rw-rw-  2.0 fat     1380 b- defN 23-Jul-11 01:12 azureml/featurestore/transformation/window_aggregation.py
+-rw-rw-rw-  2.0 fat      267 b- defN 23-Jul-11 01:12 tests/__init__.py
+-rw-rw-rw-  2.0 fat      267 b- defN 23-Jul-11 01:12 tests/e2etest/__init__.py
+-rw-rw-rw-  2.0 fat      221 b- defN 23-Jul-11 01:12 tests/e2etest/conftest.py
+-rw-rw-rw-  2.0 fat     5392 b- defN 23-Jul-11 01:12 tests/e2etest/spark_e2e_test_base.py
+-rw-rw-rw-  2.0 fat      901 b- defN 23-Jul-11 01:12 tests/e2etest/test_feature_store_e2e.py
+-rw-rw-rw-  2.0 fat      267 b- defN 23-Jul-11 01:12 tests/unittest/__init__.py
+-rw-rw-rw-  2.0 fat      221 b- defN 23-Jul-11 01:12 tests/unittest/conftest.py
+-rw-rw-rw-  2.0 fat    10395 b- defN 23-Jul-11 01:12 tests/unittest/test_feature_set.py
+-rw-rw-rw-  2.0 fat    10645 b- defN 23-Jul-11 01:12 tests/unittest/test_feature_set_spec.py
+-rw-rw-rw-  2.0 fat    14853 b- defN 23-Jul-11 01:12 tests/unittest/test_feature_store_client.py
+-rw-rw-rw-  2.0 fat      790 b- defN 23-Jul-11 01:12 tests/unittest/test_transformation.py
+-rw-rw-rw-  2.0 fat     6790 b- defN 23-Jul-11 01:12 tests/unittest/test_utils.py
+-rw-rw-rw-  2.0 fat     1093 b- defN 23-Jul-11 01:22 azureml_featurestore-0.1.0b3.dist-info/DESCRIPTION.rst
+-rw-rw-rw-  2.0 fat     1142 b- defN 23-Jul-11 01:22 azureml_featurestore-0.1.0b3.dist-info/metadata.json
+-rw-rw-rw-  2.0 fat       14 b- defN 23-Jul-11 01:22 azureml_featurestore-0.1.0b3.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jul-11 01:22 azureml_featurestore-0.1.0b3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     2191 b- defN 23-Jul-11 01:22 azureml_featurestore-0.1.0b3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat     7573 b- defN 23-Jul-11 01:22 azureml_featurestore-0.1.0b3.dist-info/RECORD
+74 files, 278069 bytes uncompressed, 72009 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -75,14 +75,17 @@
 
 Filename: azureml/featurestore/contracts/feature_retrieval_spec.py
 Comment: 
 
 Filename: azureml/featurestore/contracts/feature_source.py
 Comment: 
 
+Filename: azureml/featurestore/contracts/feature_transformation.py
+Comment: 
+
 Filename: azureml/featurestore/contracts/offline_store.py
 Comment: 
 
 Filename: azureml/featurestore/contracts/online_store.py
 Comment: 
 
 Filename: azureml/featurestore/contracts/partition.py
@@ -144,26 +147,77 @@
 
 Filename: azureml/featurestore/schema/feature_retrieval_spec_schema.py
 Comment: 
 
 Filename: azureml/featurestore/schema/feature_set_schema.py
 Comment: 
 
-Filename: azureml_featurestore-0.1.0b2.dist-info/DESCRIPTION.rst
+Filename: azureml/featurestore/transformation/__init__.py
+Comment: 
+
+Filename: azureml/featurestore/transformation/aggregation_function.py
+Comment: 
+
+Filename: azureml/featurestore/transformation/transformation_expression.py
+Comment: 
+
+Filename: azureml/featurestore/transformation/transformation_expression_collection.py
+Comment: 
+
+Filename: azureml/featurestore/transformation/window_aggregation.py
+Comment: 
+
+Filename: tests/__init__.py
+Comment: 
+
+Filename: tests/e2etest/__init__.py
+Comment: 
+
+Filename: tests/e2etest/conftest.py
+Comment: 
+
+Filename: tests/e2etest/spark_e2e_test_base.py
+Comment: 
+
+Filename: tests/e2etest/test_feature_store_e2e.py
+Comment: 
+
+Filename: tests/unittest/__init__.py
+Comment: 
+
+Filename: tests/unittest/conftest.py
+Comment: 
+
+Filename: tests/unittest/test_feature_set.py
+Comment: 
+
+Filename: tests/unittest/test_feature_set_spec.py
+Comment: 
+
+Filename: tests/unittest/test_feature_store_client.py
+Comment: 
+
+Filename: tests/unittest/test_transformation.py
+Comment: 
+
+Filename: tests/unittest/test_utils.py
+Comment: 
+
+Filename: azureml_featurestore-0.1.0b3.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: azureml_featurestore-0.1.0b2.dist-info/metadata.json
+Filename: azureml_featurestore-0.1.0b3.dist-info/metadata.json
 Comment: 
 
-Filename: azureml_featurestore-0.1.0b2.dist-info/top_level.txt
+Filename: azureml_featurestore-0.1.0b3.dist-info/top_level.txt
 Comment: 
 
-Filename: azureml_featurestore-0.1.0b2.dist-info/WHEEL
+Filename: azureml_featurestore-0.1.0b3.dist-info/WHEEL
 Comment: 
 
-Filename: azureml_featurestore-0.1.0b2.dist-info/METADATA
+Filename: azureml_featurestore-0.1.0b3.dist-info/METADATA
 Comment: 
 
-Filename: azureml_featurestore-0.1.0b2.dist-info/RECORD
+Filename: azureml_featurestore-0.1.0b3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## azureml/featurestore/_version.py

```diff
@@ -1 +1 @@
-VERSION = "0.1.0b2"
+VERSION = "0.1.0b3"
```

## azureml/featurestore/_offline_query/offline_retrieval_job.py

```diff
@@ -3,12 +3,11 @@
 # ---------------------------------------------------------
 from abc import ABC
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from pyspark.sql import DataFrame
 
-class OfflineRetrievalJob(ABC):
 
+class OfflineRetrievalJob(ABC):
     def to_spark_dataframe(self) -> "DataFrame":
         pass
-
```

## azureml/featurestore/_utils/utils.py

```diff
@@ -6,38 +6,44 @@
 
 import os
 import re
 import shutil
 import uuid
 from collections import Counter, defaultdict
 from dataclasses import asdict, dataclass
+from enum import Enum
 from typing import TYPE_CHECKING, List, Optional
 
+from azureml.dataprep.rslex import Copier
 from azureml.featurestore._utils._constants import AZUREML_URI_PATTERNS, CLOUD_URI_PATTERNS, STORAGE_URI_PATTERNS
 from azureml.featurestore._utils.error_constants import (
     EMPTY_FEATURE_MESSAGE,
     FEATURE_NAME_COLLISION_MESSAGE,
     INVALID_FEATURE_URI_MESSAGE,
     SCHEMA_ERROR_MISSING_COLUMNS,
     UNSUPORTED_STORAGE_TYPE_MESSAGE,
 )
 
+from azure.ai.ml._artifacts._artifact_utilities import (
+    download_artifact_from_aml_uri,
+    download_artifact_from_storage_url,
+)
 from azure.ai.ml._telemetry.logging_handler import get_appinsights_log_handler
 from azure.ai.ml._user_agent import USER_AGENT
 from azure.ai.ml._utils._logger_utils import OpsLogger
 from azure.ai.ml.entities._assets._artifacts.artifact import ArtifactStorageInfo
 from azure.ai.ml.exceptions import ErrorCategory, ErrorTarget, ValidationErrorType, ValidationException
 from azure.ai.ml.operations import DatastoreOperations
 
 if TYPE_CHECKING:
     from azureml.featurestore._feature_set import FeatureSet
     from azureml.featurestore.contracts.feature import Feature
 
 
-class PathType:
+class PathType(Enum):
     azureml = 1
     cloud = 2
     local = 3
     storage = 4
 
 
 def _process_path(path: str, datastore_operations: DatastoreOperations = None):
@@ -68,20 +74,20 @@
     path_type: PathType,
     target_path: str = None,
     datastore_operations: DatastoreOperations = None,
 ):
     from tempfile import mkdtemp
 
     # normalize path to yaml config path
-    normalized_path = path.rstrip("/")
+    normalized_path = path.rstrip("/\\")
     local_path = mkdtemp() if not target_path else target_path
 
     if not datastore_operations:
         from azureml.dataprep.api._rslex_executor import ensure_rslex_environment
-        from azureml.dataprep.rslex import Copier, PyIfDestinationExists, PyLocationInfo
+        from azureml.dataprep.rslex import PyIfDestinationExists, PyLocationInfo
 
         ensure_rslex_environment()
 
         if_destination_exists = PyIfDestinationExists.MERGE_WITH_OVERWRITE
         try:
             Copier.copy_uri(PyLocationInfo("Local", local_path, {}), normalized_path, if_destination_exists, "")
         except Exception as e:
@@ -90,71 +96,37 @@
             elif "StreamError(NotFound)" in e.args[0]:
                 raise ValueError(f"{e.args[0]}; Not able to find path: {normalized_path}")
             elif "PermissionDenied" in e.args[0]:
                 raise PermissionError(f"{e.args[0]}; No permission to access path: {normalized_path}")
             else:
                 raise SystemError(f"{e.args[0]}, uri: {normalized_path}")
 
-        local_path = os.path.join(local_path, re.split(normalized_path, r"/\\")[-1])
+        local_path = os.path.join(local_path, re.split(r"/|\\", normalized_path)[-1])
     else:
-        from azure.ai.ml._artifacts._artifact_utilities import (
-            download_artifact_from_aml_uri,
-            download_artifact_from_storage_url,
-        )
-
         if path_type == PathType.cloud:
             local_path = download_artifact_from_storage_url(
                 blob_url=normalized_path,
                 destination=local_path,
                 datastore_operation=datastore_operations,
                 datastore_name=None,
             )
         elif path_type == PathType.azureml:
             local_path = download_artifact_from_aml_uri(
                 uri=normalized_path, destination=local_path, datastore_operation=datastore_operations
             )
         elif path_type == PathType.local:
-            return local_path
+            local_path = path
         else:
-            raise Exception(f"Can't download from path: {normalized_path}")
+            raise Exception(
+                f"Can't download from path: {normalized_path}, path type: {path_type.name} is not supported"
+            )
 
     return local_path
 
 
-def _list_files(parent_uri: str, file: str):
-    from azureml.dataprep.api._rslex_executor import ensure_rslex_environment
-    from azureml.dataprep.rslex import Copier, PyIfDestinationExists, PyLocationInfo
-
-    ensure_rslex_environment()
-
-    # normalize path to file path
-    normalized_path = "{}/{}".format(parent_uri.rstrip("/"), file)
-    if_destination_exists = PyIfDestinationExists.MERGE_WITH_OVERWRITE
-    try:
-
-        from tempfile import mkdtemp
-
-        local_path = mkdtemp()
-        Copier.copy_uri(PyLocationInfo("Local", local_path, {}), normalized_path, if_destination_exists, "")
-
-        file_list = os.listdir(local_path)
-
-        file_paths = list(map(lambda i: "/".join([parent_uri.rstrip("/"), i]), file_list))
-        shutil.rmtree(local_path)
-
-        return file_paths
-    except Exception as e:
-        if "InvalidUriScheme" in e.args[0] or "DataAccessError(NotFound)" in e.args[0]:
-            raise ValueError(f"{e.args[0]}, uri: {normalized_path}")
-        elif "StreamError(NotFound)" in e.args[0]:
-            raise ValueError(f"{e.args[0]}; Not able to find path: {normalized_path}")
-        else:
-            raise SystemError(f"{e.args[0]}, uri: {normalized_path}")
-
-
 def _ensure_azureml_full_path(path: str, subscription_id: str, resource_group: str, workspace_name: str):
     res = path
     if path.startswith("azureml://") and not path.startswith("azureml://subscriptions"):
         path = path.split("azureml://", 1)[1]
         res = f"azureml://subscriptions/{subscription_id}/resourcegroups/{resource_group}/workspaces/{workspace_name}/{path}"
 
     return res
```

## azureml/featurestore/contracts/transformation_code.py

```diff
@@ -8,25 +8,27 @@
 from azureml.featurestore._utils.utils import (
     PathType,
     _download_file,
     _parse_path_format,
     _strip_local_path,
     copy_rename_and_zip,
 )
+from azureml.featurestore.contracts.feature_transformation import FeatureTransformation
 
 from azure.ai.ml.exceptions import ErrorCategory, ErrorTarget, ValidationErrorType, ValidationException
 from azure.ai.ml.operations import DatastoreOperations
 
 
-class TransformationCode(object):
+class TransformationCode(FeatureTransformation):
     """Feature transformation code representation
     :param type: The source type
     :type type: str, required
     :param path: The source data path
-    :type path: str, required"""
+    :type path: str, required
+    """
 
     def __init__(self, *, path, transformer_class):
         self.path = path
         self.transformer_class = transformer_class
 
     def __repr__(self):
         return f"TransformationCode(Path={self.path},TransformerClass={self.transformer_class})"
```

## azureml/featurestore/online/_online_feature_materialization.py

```diff
@@ -2,15 +2,16 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # ---------------------------------------------------------
 
 from azureml.featurestore._feature_set import FeatureSet
 from azureml.featurestore._utils._constants import TIME_TO_LIVE
 from azureml.featurestore.contracts.store_connection import OnlineStoreType
 from azureml.featurestore.online._redis_client_pool import _get_redis_connection_string
-from ._utils import _get_lookup_key, _get_lookup_key_udf, _get_lookup_key_pattern
+
+from ._utils import _get_lookup_key, _get_lookup_key_pattern, _get_lookup_key_udf
 
 
 def materialize_online(feature_set, dataframe_to_store, upsert):
     # Do the 3 steps
     from pyspark.sql import SparkSession
 
     spark = SparkSession.builder.getOrCreate()
```

## azureml/featurestore/online/_utils.py

```diff
@@ -15,17 +15,18 @@
     for index_column in suffix_column_names:
         suffix_parts.append(index_column)
         suffix_parts.append(row[index_column])
 
     suffix = ":".join(suffix_parts)
     return f"{prefix}:{suffix}"
 
+
 def _get_lookup_key_pattern(featureset):
     prefix = f"featurestore:{featureset.feature_store_guid}:featureset:{featureset.name}:version:{featureset.version}"
 
     suffix_column_names = []
 
     for entity in featureset.entities:
         for index_column in entity.index_columns:
             suffix_column_names.append(index_column.name)
-    
+
     return prefix, suffix_column_names
```

## Comparing `azureml_featurestore-0.1.0b2.dist-info/DESCRIPTION.rst` & `azureml_featurestore-0.1.0b3.dist-info/DESCRIPTION.rst`

 * *Files 27% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 You can install the package via ` pip install azureml-featurestore `
 
 To learn more about Azure ML managed feature store visit https://aka.ms/featurestore-get-started
 
 
 # Change Log
 
+## 0.1.0b3 (2023.07.10)
+
+- Various bug fixes
+
 ## 0.1.0b2 (2023.06.13)
 
 **New Features:**
 
 - [Private preview] Added online store support. Online store supports materialization and online feature values retrieval from Redis cache for batch scoring.
 
 - Various bug fixes
```

## Comparing `azureml_featurestore-0.1.0b2.dist-info/metadata.json` & `azureml_featurestore-0.1.0b3.dist-info/metadata.json`

 * *Files 0% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.1.0b3'"}*

```diff
@@ -53,9 +53,9 @@
                 "pandas (>=1.5.3)",
                 "pyarrow (>=9.0.0)",
                 "redis (>=4.5.1)"
             ]
         }
     ],
     "summary": "Azure Machine Learning Feature Store SDK",
-    "version": "0.1.0b2"
+    "version": "0.1.0b3"
 }
```

## Comparing `azureml_featurestore-0.1.0b2.dist-info/METADATA` & `azureml_featurestore-0.1.0b3.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.0
 Name: azureml-featurestore
-Version: 0.1.0b2
+Version: 0.1.0b3
 Summary: Azure Machine Learning Feature Store SDK
 Home-page: https://aka.ms/featurestore-get-started
 Author: Microsoft Corporation
 License: MIT License
 Keywords: AzureMachineLearning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -43,14 +43,18 @@
 You can install the package via ` pip install azureml-featurestore `
 
 To learn more about Azure ML managed feature store visit https://aka.ms/featurestore-get-started
 
 
 # Change Log
 
+## 0.1.0b3 (2023.07.10)
+
+- Various bug fixes
+
 ## 0.1.0b2 (2023.06.13)
 
 **New Features:**
 
 - [Private preview] Added online store support. Online store supports materialization and online feature values retrieval from Redis cache for batch scoring.
 
 - Various bug fixes
```

## Comparing `azureml_featurestore-0.1.0b2.dist-info/RECORD` & `azureml_featurestore-0.1.0b3.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,74 @@
 azureml/__init__.py,sha256=d5b08hPILQxNDQ9p22-0d5Fl-90qmLEP7axZw6c0Ryw,267
 azureml/featurestore/__init__.py,sha256=ylJkgOMGGuhcMDPqQTq_L046QWfueUh2OsSgGc0POvA,917
 azureml/featurestore/_feature_set.py,sha256=FGzW1WyCyN75lYZjTgElMk_oBTK2ozgduOZp9tNteFg,21202
-azureml/featurestore/_version.py,sha256=FfhzaecOVVhP5q8jtt3aeOI4NfHslas-hIspKiWrpuA,21
+azureml/featurestore/_version.py,sha256=SoLjvM6wgmDPtERh6AGYPWxUyTJf0Hd5nuuYMzBke3E,21
 azureml/featurestore/abstract_feature_store.py,sha256=HyH-wGhFvD0312T691b4H2YSyXdqZzQQgoq5GAp6qvU,1108
 azureml/featurestore/feature_set_spec.py,sha256=EzkmBl2pZeXVgJBX09Iod8uKdlu2f235O9DUh3tiP38,25045
 azureml/featurestore/feature_store_client.py,sha256=JWnEZiTDtM5x2YgwUVPHbm-tQHhF0tZ_SlLGDqDWBIw,26844
 azureml/featurestore/_identity/__init__.py,sha256=ySOoGimIHBlawW86oB_PtMBD7KZf9z4eVwKBRR1TNIY,410
 azureml/featurestore/_identity/aml_hobospark_on_behalf_of.py,sha256=jD_CsUBz2rIxS8_ld11eeu3bE9zzg2HZQ8F9bm6K1w0,6334
 azureml/featurestore/_offline_query/__init__.py,sha256=Q5ZiXWuLnEFEcp0JcWjUfF5i5qj5SSFP_S1bE6Dmqvk,455
-azureml/featurestore/_offline_query/offline_retrieval_job.py,sha256=yBxyvbn__cFZGZS7cZmwbRDQk9snKWjvpMMHWCcHjMo,401
+azureml/featurestore/_offline_query/offline_retrieval_job.py,sha256=UeXEN6TT7PazFcml4-hon3epQCGMETfgWRyXlglGQlM,399
 azureml/featurestore/_offline_query/point_at_time.py,sha256=bHRVx5Ug3TQiFceW2_MRRNoex80iyWO7YhceKruuQcU,10931
 azureml/featurestore/_utils/__init__.py,sha256=d5b08hPILQxNDQ9p22-0d5Fl-90qmLEP7axZw6c0Ryw,267
 azureml/featurestore/_utils/_constants.py,sha256=QkBJDIzHHi8sBQkHY0NSyubkwoFmpdH71EcObgLNXMY,1694
 azureml/featurestore/_utils/_preview_method.py,sha256=Tzop4bo0FIMJ4MrOoOpqOqDaznKaK5XamRfnDD2cO5M,398
 azureml/featurestore/_utils/arm_id_utils.py,sha256=vgC0CkCMxz8aeVhZABPIO6lm9n6rsXkoX02HYMl71uk,7359
 azureml/featurestore/_utils/error_constants.py,sha256=3dZzSmutEGFo3FmGsyi5qhMT4nU1ps5Qk3pbz_5_k_o,2564
 azureml/featurestore/_utils/materialize.py,sha256=HH-mq_suK-Pq4fxys6MhdX7NiWgDuhAX698IcINXXzU,5732
 azureml/featurestore/_utils/spark_utils.py,sha256=DIJZvOsIxnPBmaxvr4jGofmi_wBWIAUxSuxH8esaBoU,9728
 azureml/featurestore/_utils/type_map.py,sha256=-8261UWjeCmYvIvyfT_b361D6uq70bo_TKBTsq-yFik,2370
-azureml/featurestore/_utils/utils.py,sha256=Ve4EBnL-7A7pPmSNDNsbpfDfSIysy_HJS7dtjvpI0Bc,15684
+azureml/featurestore/_utils/utils.py,sha256=V6i0Hjx3RzlWlbSJX6_cN32soGiGz8vvsOkpfgTe5Ks,14558
 azureml/featurestore/contracts/__init__.py,sha256=XQSdeiXkhQz-pnsGpzjlHyEYl68HcS3hC86_0yrLTdk,681
 azureml/featurestore/contracts/column.py,sha256=tpF4lio6z-8y50Ynh_km_qUv7UHDBl3RnyHjlRQ1C-M,1243
 azureml/featurestore/contracts/datetimeoffset.py,sha256=zTYYHbuPLAAK1YuLXQMWDlhWnIYpjtImBfbJg4Gtao8,1058
 azureml/featurestore/contracts/feature.py,sha256=BAKqtAQJLowuuXEszG_dsF5xRSDEb7NpDHII1ixWK34,3593
 azureml/featurestore/contracts/feature_retrieval_spec.py,sha256=5VzYQxU_NKv3roARIghn_7k58EPgEsDBcmOnaWIhHrk,9258
 azureml/featurestore/contracts/feature_source.py,sha256=HOF3LfzTmZOea9Liz6hCzyRR3SzrdyFoimUE-U2lxCA,2846
+azureml/featurestore/contracts/feature_transformation.py,sha256=ENunrBkolwA56FH47NTmtRCw5rzcPZLYwvD_N9O9Ws0,489
 azureml/featurestore/contracts/offline_store.py,sha256=QSVo_s_WV6Ajc-ba6CRuFs8okE0_gw7R0fyajpTsDF8,2019
 azureml/featurestore/contracts/online_store.py,sha256=ZY5QlYQQT2WcVc6fwc3RYHzHESEH_mcwlYybUlFtUnU,646
 azureml/featurestore/contracts/partition.py,sha256=99PGUsY7a0gY8HYazLR-qjb68RNNDNb1Wbc8_SM-15E,694
 azureml/featurestore/contracts/store_connection.py,sha256=Jtt2sCgCtz8pKh6cQT4lnaL7IQ1_tPm341Gv4fmW6Ps,1230
 azureml/featurestore/contracts/timestamp_column.py,sha256=vDoNgsMbKbd527VKmmMPRAlbNnXiSaiAa0UrLPBk_as,753
-azureml/featurestore/contracts/transformation_code.py,sha256=C4Yablh-LDWjyB-U3qPrQbDwgFRGD07kTvWnr0VhSNo,2530
+azureml/featurestore/contracts/transformation_code.py,sha256=3Eoy1_lI9tnss14vyWWuvk06d2iD9MEr153I5rMYLs0,2640
 azureml/featurestore/grpc/__init__.py,sha256=5MSlWALp5Ta6ZqnzvuEFoQTiZmIphmkNxFAThYLiBMU,294
 azureml/featurestore/grpc/_flight_feature_retrieval_client.py,sha256=8UlYrzJ8aFu8-63_cYt0UYrUjbyZdMic5Jxlqw0Oe64,1364
 azureml/featurestore/grpc/_flight_feature_retrieval_server.py,sha256=hxHPmLiIOUVE-6na0Q53bUTp7c_qOsVtCzO9MTaHKUQ,3276
 azureml/featurestore/grpc/_flight_helper.py,sha256=uhOZjxyPJXgYg86cLpCEEFwLuuf_BUeKRntA0OIAOaY,5923
 azureml/featurestore/grpc/_inline_feature_retrieval_client.py,sha256=Yx-lxrx5mW1NgBFpqstGBAqfk7dV09Ux4bCSVLZEe48,934
 azureml/featurestore/offline_store/__init__.py,sha256=ZoGnMoKGPd8cOJXODpYbg1ebH3t1wwTDJ7OBtvACdEQ,391
 azureml/featurestore/offline_store/azure_data_lake_offline_store.py,sha256=SL7SsC-onnkqyHVzR7dBTPdm11qvmeqOn3aUzCzHplc,9020
 azureml/featurestore/offline_store/partition/__init__.py,sha256=iUJezOoUcCW5AK9LI-CJBaL8sdxUVk8fAoaOqm1vqUc,367
 azureml/featurestore/offline_store/partition/timestamp_partition.py,sha256=yrDH_0Skft27Yp8noNMV97LVx178zp2tdzPA8imFb9s,2381
 azureml/featurestore/online/__init__.py,sha256=GQg_cumJmcHWx9a02jhxSJLfXfIJmlA7RjYGa_W-4yg,242
 azureml/featurestore/online/_online_feature_getter.py,sha256=iff73LgZHYJyQBWtUakrqUVLVK6M92OXxnaK99yDzAc,5515
-azureml/featurestore/online/_online_feature_materialization.py,sha256=IFkeAysD022RxkZ-5Fx4FmvuNfZsvwXcyo8BKuAPf98,5571
+azureml/featurestore/online/_online_feature_materialization.py,sha256=0KcvMbmakeNVD9JNm6L67TMT7QAkaOXrtHkdGVjab9M,5573
 azureml/featurestore/online/_redis_client_pool.py,sha256=aBSngwCq20fQFlqiKD9VIoUSW1ulWtD7WGuYpmzLkDQ,1669
-azureml/featurestore/online/_utils.py,sha256=vGo7Vur-skAY-hefHOrAbB-X5ZNgcRcHG9B7foqT8Nk,1055
+azureml/featurestore/online/_utils.py,sha256=LExgq8AU65MiwROAwtxxt58FGxHNHpNgKUhrztNAQm4,1053
 azureml/featurestore/schema/__init__.py,sha256=d5b08hPILQxNDQ9p22-0d5Fl-90qmLEP7axZw6c0Ryw,267
 azureml/featurestore/schema/feature_retrieval_spec_schema.py,sha256=I3e63kdZQUHIlfx5Y3cEkUyQqIqJwvXtSWhv21nZxgg,1655
 azureml/featurestore/schema/feature_set_schema.py,sha256=36GiLZrjZPWqejS_PA7iOUdOZT2E-HU5Ti2yWlYVj2Y,5944
-azureml_featurestore-0.1.0b2.dist-info/DESCRIPTION.rst,sha256=F6R6tlHXSN2NIDDf3lCz_IqwdoN5V2-j4dDtPE49V4U,1047
-azureml_featurestore-0.1.0b2.dist-info/METADATA,sha256=rXQrCejZu4Eskmagp0Aco02Fi0cN59ZL4VLiGxoFKiY,2145
-azureml_featurestore-0.1.0b2.dist-info/RECORD,,
-azureml_featurestore-0.1.0b2.dist-info/WHEEL,sha256=Vlaj2XNMTTJ893zWX-JvKeZUIs7q5E7d7Gise2Vouzc,97
-azureml_featurestore-0.1.0b2.dist-info/metadata.json,sha256=iDFDzwS1pWREm4kKWsAn7Zbm6U6X-rSJT4RU_8_MUfM,1142
-azureml_featurestore-0.1.0b2.dist-info/top_level.txt,sha256=ZOeEa0TAXo6i5wOjwBoqfIGEuxOcKuscGgNSpizqREY,8
+azureml/featurestore/transformation/__init__.py,sha256=JlCCObuOLZyNhIZlsoL51KtFxiY4xKIIzIRDBcdeu6Y,183
+azureml/featurestore/transformation/aggregation_function.py,sha256=9Gn7DQdf5G_7BWTmqHnnuc4u1TpuNoYoC6wHpYj1pQA,425
+azureml/featurestore/transformation/transformation_expression.py,sha256=YuVSdMSEKPS5qPygNa77Y9cDb74XdF2AtiKlegnveoY,382
+azureml/featurestore/transformation/transformation_expression_collection.py,sha256=bZ2BlS_pAMJr704gKx4rb9aD48VuRQVTQhD4-6EPYhE,959
+azureml/featurestore/transformation/window_aggregation.py,sha256=BA_FmmypFwJnat0ItdJhvEcJwYOVzKSCPtiDpx0dOPw,1380
+azureml_featurestore-0.1.0b3.dist-info/DESCRIPTION.rst,sha256=tVZrUOA_JTwFLkHJqJputAYIHmiqS6p3FFEed-QEyic,1093
+azureml_featurestore-0.1.0b3.dist-info/METADATA,sha256=ZGjWGKSdutwFwiMZAKzXp9WHIdZcPSE6CmYWuKFAp3Y,2191
+azureml_featurestore-0.1.0b3.dist-info/RECORD,,
+azureml_featurestore-0.1.0b3.dist-info/WHEEL,sha256=Vlaj2XNMTTJ893zWX-JvKeZUIs7q5E7d7Gise2Vouzc,97
+azureml_featurestore-0.1.0b3.dist-info/metadata.json,sha256=V5pRguEern4Zyzqk2nrgdOXqLvCRq0Z4KDTI_0KFDlI,1142
+azureml_featurestore-0.1.0b3.dist-info/top_level.txt,sha256=YGbVVonfOvHBwpsDBTpLWbK7KEdGg0m7LlGFY7j0SCw,14
+tests/__init__.py,sha256=d5b08hPILQxNDQ9p22-0d5Fl-90qmLEP7axZw6c0Ryw,267
+tests/e2etest/__init__.py,sha256=d5b08hPILQxNDQ9p22-0d5Fl-90qmLEP7axZw6c0Ryw,267
+tests/e2etest/conftest.py,sha256=RKeM5J1OW9W5V0iNURUynNtpW92GTKFJTHtXjeHss50,221
+tests/e2etest/spark_e2e_test_base.py,sha256=NUSnE77zbgtj56rlVC8oHSRlUQ_7JZaQAUvxWX6Fd1Q,5392
+tests/e2etest/test_feature_store_e2e.py,sha256=0qrjsHu_jEnji8_FjN4LlKtU9cb-0TjKyUcutiWLIWM,901
+tests/unittest/__init__.py,sha256=d5b08hPILQxNDQ9p22-0d5Fl-90qmLEP7axZw6c0Ryw,267
+tests/unittest/conftest.py,sha256=RKeM5J1OW9W5V0iNURUynNtpW92GTKFJTHtXjeHss50,221
+tests/unittest/test_feature_set.py,sha256=5Nq5No3BCMl6ICL--Kz6D9QzxfNUjbNcfLSggKBJcwo,10395
+tests/unittest/test_feature_set_spec.py,sha256=RPDOMvrfYne2_HHVMOIx5QodjpMIOq1L6RDvYaKMphM,10645
+tests/unittest/test_feature_store_client.py,sha256=KsRUvIAd3Ov8DuxuHex7SCExFuObIqRirn5khbKpbrY,14853
+tests/unittest/test_transformation.py,sha256=Zrzk6F34Hqzht_Bfi3lBCy1cCLMVg-aWzSSBsRkxPso,790
+tests/unittest/test_utils.py,sha256=D2ib1WTGIhRRt01zmtmjViOYXL68vZ-g-TbeFizN8B8,6790
```

