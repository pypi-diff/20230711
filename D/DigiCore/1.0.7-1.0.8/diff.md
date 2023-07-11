# Comparing `tmp/DigiCore-1.0.7.tar.gz` & `tmp/DigiCore-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\DigiCore-1.0.7.tar", last modified: Wed Jul  5 06:41:51 2023, max compression
+gzip compressed data, was "dist\DigiCore-1.0.8.tar", last modified: Tue Jul 11 08:09:26 2023, max compression
```

## Comparing `DigiCore-1.0.7.tar` & `DigiCore-1.0.8.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 06:41:51.756384 DigiCore-1.0.7/
-drwxrwxrwx   0        0        0        0 2023-07-05 06:41:51.615870 DigiCore-1.0.7/DigiCore.egg-info/
--rw-rw-rw-   0        0        0     4014 2023-07-05 06:41:51.000000 DigiCore-1.0.7/DigiCore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1142 2023-07-05 06:41:51.000000 DigiCore-1.0.7/DigiCore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 06:41:51.000000 DigiCore-1.0.7/DigiCore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      585 2023-07-05 06:41:51.000000 DigiCore-1.0.7/DigiCore.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-07-05 06:41:51.000000 DigiCore-1.0.7/DigiCore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-07-05 06:41:51.000000 DigiCore-1.0.7/DigiCore.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1104 2023-05-20 03:41:32.000000 DigiCore-1.0.7/LICENSE
--rw-rw-rw-   0        0        0     4014 2023-07-05 06:41:51.756384 DigiCore-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2670 2023-05-20 03:41:32.000000 DigiCore-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-05 06:41:51.646140 DigiCore-1.0.7/digiCore/
--rw-rw-rw-   0        0        0     1382 2023-07-05 06:14:20.000000 DigiCore-1.0.7/digiCore/__init__.py
--rw-rw-rw-   0        0        0     3056 2023-07-05 06:35:37.000000 DigiCore-1.0.7/digiCore/db_init.py
--rw-rw-rw-   0        0        0     4901 2023-06-14 02:12:46.000000 DigiCore-1.0.7/digiCore/dsd_kafka.py
--rw-rw-rw-   0        0        0     3450 2023-07-05 06:40:33.000000 DigiCore-1.0.7/digiCore/dsd_mongodb.py
--rw-rw-rw-   0        0        0     6853 2023-06-14 02:12:46.000000 DigiCore-1.0.7/digiCore/dsd_mysql.py
--rw-rw-rw-   0        0        0     4457 2023-07-05 06:40:33.000000 DigiCore-1.0.7/digiCore/dsd_redis.py
--rw-rw-rw-   0        0        0     4632 2023-07-04 08:04:47.000000 DigiCore-1.0.7/digiCore/lingxing_api_scheduler.py
--rw-rw-rw-   0        0        0     3558 2023-07-05 06:40:33.000000 DigiCore-1.0.7/digiCore/model.py
--rw-rw-rw-   0        0        0     3739 2023-06-29 02:25:55.000000 DigiCore-1.0.7/digiCore/send_to_group.py
--rw-rw-rw-   0        0        0     5984 2023-07-04 09:09:42.000000 DigiCore-1.0.7/digiCore/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-05 06:41:51.661785 DigiCore-1.0.7/k3cloud_webapi_sdk/
--rw-rw-rw-   0        0        0       29 2023-06-15 03:25:11.000000 DigiCore-1.0.7/k3cloud_webapi_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-05 06:41:51.679110 DigiCore-1.0.7/k3cloud_webapi_sdk/const/
--rw-rw-rw-   0        0        0       16 2023-06-15 03:25:11.000000 DigiCore-1.0.7/k3cloud_webapi_sdk/const/__init__.py
--rw-rw-rw-   0        0        0      418 2023-06-15 03:25:11.000000 DigiCore-1.0.7/k3cloud_webapi_sdk/const/const_define.py
--rw-rw-rw-   0        0        0      500 2023-06-15 03:25:11.000000 DigiCore-1.0.7/k3cloud_webapi_sdk/const/header_param.py
-drwxrwxrwx   0        0        0        0 2023-07-05 06:41:51.693136 DigiCore-1.0.7/k3cloud_webapi_sdk/core/
--rw-rw-rw-   0        0        0       15 2023-06-15 03:25:11.000000 DigiCore-1.0.7/k3cloud_webapi_sdk/core/__init__.py
--rw-rw-rw-   0        0        0     8162 2023-06-15 03:25:11.000000 DigiCore-1.0.7/k3cloud_webapi_sdk/core/webapi_client.py
--rw-rw-rw-   0        0        0     7910 2023-06-15 03:25:11.000000 DigiCore-1.0.7/k3cloud_webapi_sdk/main.py
-drwxrwxrwx   0        0        0        0 2023-07-05 06:41:51.726665 DigiCore-1.0.7/k3cloud_webapi_sdk/model/
--rw-rw-rw-   0        0        0       16 2023-06-15 03:25:11.000000 DigiCore-1.0.7/k3cloud_webapi_sdk/model/__init__.py
--rw-rw-rw-   0        0        0      433 2023-06-15 03:25:11.000000 DigiCore-1.0.7/k3cloud_webapi_sdk/model/api_config.py
--rw-rw-rw-   0        0        0     1109 2023-06-15 03:25:11.000000 DigiCore-1.0.7/k3cloud_webapi_sdk/model/cookie.py
--rw-rw-rw-   0        0        0      327 2023-06-15 03:25:11.000000 DigiCore-1.0.7/k3cloud_webapi_sdk/model/cookie_store.py
--rw-rw-rw-   0        0        0      411 2023-06-15 03:25:11.000000 DigiCore-1.0.7/k3cloud_webapi_sdk/model/identity.py
--rw-rw-rw-   0        0        0      197 2023-06-15 03:25:11.000000 DigiCore-1.0.7/k3cloud_webapi_sdk/model/query_param.py
--rw-rw-rw-   0        0        0     4385 2023-06-15 03:25:11.000000 DigiCore-1.0.7/k3cloud_webapi_sdk/sample.py
-drwxrwxrwx   0        0        0        0 2023-07-05 06:41:51.756384 DigiCore-1.0.7/k3cloud_webapi_sdk/util/
--rw-rw-rw-   0        0        0       15 2023-06-15 03:25:11.000000 DigiCore-1.0.7/k3cloud_webapi_sdk/util/__init__.py
--rw-rw-rw-   0        0        0     2001 2023-06-15 03:25:11.000000 DigiCore-1.0.7/k3cloud_webapi_sdk/util/base64_util.py
--rw-rw-rw-   0        0        0     2671 2023-06-15 03:25:11.000000 DigiCore-1.0.7/k3cloud_webapi_sdk/util/config_util.py
--rw-rw-rw-   0        0        0     1654 2023-06-15 03:25:11.000000 DigiCore-1.0.7/k3cloud_webapi_sdk/util/encode_util.py
--rw-rw-rw-   0        0        0      420 2023-06-15 03:25:11.000000 DigiCore-1.0.7/k3cloud_webapi_sdk/util/hmac_util.py
--rw-rw-rw-   0        0        0       42 2023-07-05 06:41:51.756384 DigiCore-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     3015 2023-07-05 06:41:44.000000 DigiCore-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 08:09:26.383488 DigiCore-1.0.8/
+drwxrwxrwx   0        0        0        0 2023-07-11 08:09:26.334572 DigiCore-1.0.8/DigiCore.egg-info/
+-rw-rw-rw-   0        0        0     4014 2023-07-11 08:09:26.000000 DigiCore-1.0.8/DigiCore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1142 2023-07-11 08:09:26.000000 DigiCore-1.0.8/DigiCore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 08:09:26.000000 DigiCore-1.0.8/DigiCore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      585 2023-07-11 08:09:26.000000 DigiCore-1.0.8/DigiCore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-07-11 08:09:26.000000 DigiCore-1.0.8/DigiCore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-07-11 08:09:26.000000 DigiCore-1.0.8/DigiCore.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1104 2023-05-20 03:41:32.000000 DigiCore-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0     4014 2023-07-11 08:09:26.382485 DigiCore-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2670 2023-05-20 03:41:32.000000 DigiCore-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 08:09:26.350854 DigiCore-1.0.8/digiCore/
+-rw-rw-rw-   0        0        0     1382 2023-07-05 07:14:07.000000 DigiCore-1.0.8/digiCore/__init__.py
+-rw-rw-rw-   0        0        0     3056 2023-07-05 06:47:32.000000 DigiCore-1.0.8/digiCore/db_init.py
+-rw-rw-rw-   0        0        0     4914 2023-07-11 07:59:45.000000 DigiCore-1.0.8/digiCore/dsd_kafka.py
+-rw-rw-rw-   0        0        0     3450 2023-07-05 06:47:32.000000 DigiCore-1.0.8/digiCore/dsd_mongodb.py
+-rw-rw-rw-   0        0        0     6853 2023-07-05 06:45:24.000000 DigiCore-1.0.8/digiCore/dsd_mysql.py
+-rw-rw-rw-   0        0        0     4457 2023-07-11 08:03:54.000000 DigiCore-1.0.8/digiCore/dsd_redis.py
+-rw-rw-rw-   0        0        0     4632 2023-07-05 06:47:32.000000 DigiCore-1.0.8/digiCore/lingxing_api_scheduler.py
+-rw-rw-rw-   0        0        0     3558 2023-07-05 06:47:32.000000 DigiCore-1.0.8/digiCore/model.py
+-rw-rw-rw-   0        0        0     3739 2023-07-05 06:45:24.000000 DigiCore-1.0.8/digiCore/send_to_group.py
+-rw-rw-rw-   0        0        0     5984 2023-07-05 06:47:32.000000 DigiCore-1.0.8/digiCore/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-11 08:09:26.355961 DigiCore-1.0.8/k3cloud_webapi_sdk/
+-rw-rw-rw-   0        0        0       29 2023-07-05 06:45:24.000000 DigiCore-1.0.8/k3cloud_webapi_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 08:09:26.360476 DigiCore-1.0.8/k3cloud_webapi_sdk/const/
+-rw-rw-rw-   0        0        0       16 2023-07-05 06:45:24.000000 DigiCore-1.0.8/k3cloud_webapi_sdk/const/__init__.py
+-rw-rw-rw-   0        0        0      418 2023-07-05 06:45:24.000000 DigiCore-1.0.8/k3cloud_webapi_sdk/const/const_define.py
+-rw-rw-rw-   0        0        0      500 2023-07-05 06:45:24.000000 DigiCore-1.0.8/k3cloud_webapi_sdk/const/header_param.py
+drwxrwxrwx   0        0        0        0 2023-07-11 08:09:26.362803 DigiCore-1.0.8/k3cloud_webapi_sdk/core/
+-rw-rw-rw-   0        0        0       15 2023-07-05 06:45:24.000000 DigiCore-1.0.8/k3cloud_webapi_sdk/core/__init__.py
+-rw-rw-rw-   0        0        0     8162 2023-07-05 06:45:24.000000 DigiCore-1.0.8/k3cloud_webapi_sdk/core/webapi_client.py
+-rw-rw-rw-   0        0        0     7910 2023-07-05 06:45:24.000000 DigiCore-1.0.8/k3cloud_webapi_sdk/main.py
+drwxrwxrwx   0        0        0        0 2023-07-11 08:09:26.373110 DigiCore-1.0.8/k3cloud_webapi_sdk/model/
+-rw-rw-rw-   0        0        0       16 2023-07-05 06:45:24.000000 DigiCore-1.0.8/k3cloud_webapi_sdk/model/__init__.py
+-rw-rw-rw-   0        0        0      433 2023-07-05 06:45:24.000000 DigiCore-1.0.8/k3cloud_webapi_sdk/model/api_config.py
+-rw-rw-rw-   0        0        0     1109 2023-07-05 06:45:24.000000 DigiCore-1.0.8/k3cloud_webapi_sdk/model/cookie.py
+-rw-rw-rw-   0        0        0      327 2023-07-05 06:45:24.000000 DigiCore-1.0.8/k3cloud_webapi_sdk/model/cookie_store.py
+-rw-rw-rw-   0        0        0      411 2023-07-05 06:45:24.000000 DigiCore-1.0.8/k3cloud_webapi_sdk/model/identity.py
+-rw-rw-rw-   0        0        0      197 2023-07-05 06:45:24.000000 DigiCore-1.0.8/k3cloud_webapi_sdk/model/query_param.py
+-rw-rw-rw-   0        0        0     4385 2023-07-05 06:45:24.000000 DigiCore-1.0.8/k3cloud_webapi_sdk/sample.py
+drwxrwxrwx   0        0        0        0 2023-07-11 08:09:26.381485 DigiCore-1.0.8/k3cloud_webapi_sdk/util/
+-rw-rw-rw-   0        0        0       15 2023-07-05 06:45:24.000000 DigiCore-1.0.8/k3cloud_webapi_sdk/util/__init__.py
+-rw-rw-rw-   0        0        0     2001 2023-07-05 06:45:24.000000 DigiCore-1.0.8/k3cloud_webapi_sdk/util/base64_util.py
+-rw-rw-rw-   0        0        0     2671 2023-07-05 06:45:24.000000 DigiCore-1.0.8/k3cloud_webapi_sdk/util/config_util.py
+-rw-rw-rw-   0        0        0     1654 2023-07-05 06:45:24.000000 DigiCore-1.0.8/k3cloud_webapi_sdk/util/encode_util.py
+-rw-rw-rw-   0        0        0      420 2023-07-05 06:45:24.000000 DigiCore-1.0.8/k3cloud_webapi_sdk/util/hmac_util.py
+-rw-rw-rw-   0        0        0       42 2023-07-11 08:09:26.383488 DigiCore-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     3015 2023-07-11 08:08:14.000000 DigiCore-1.0.8/setup.py
```

### Comparing `DigiCore-1.0.7/DigiCore.egg-info/PKG-INFO` & `DigiCore-1.0.8/DigiCore.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DigiCore
-Version: 1.0.7
+Version: 1.0.8
 Summary: DigiCore是一个基于Python的数字化支持部第三方库，旨在为数据处理和开发提供完备的工具集和服务。
 Home-page: UNKNOWN
 Author: yarm
 Author-email: yangyang@doocn.com
 License: MIT License
 Keywords: digicore是服务于道诚集团数字化支持部的自建第三方库项目
 Platform: any
```

### Comparing `DigiCore-1.0.7/DigiCore.egg-info/SOURCES.txt` & `DigiCore-1.0.8/DigiCore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.7/DigiCore.egg-info/requires.txt` & `DigiCore-1.0.8/DigiCore.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.7/LICENSE` & `DigiCore-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.7/PKG-INFO` & `DigiCore-1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DigiCore
-Version: 1.0.7
+Version: 1.0.8
 Summary: DigiCore是一个基于Python的数字化支持部第三方库，旨在为数据处理和开发提供完备的工具集和服务。
 Home-page: UNKNOWN
 Author: yarm
 Author-email: yangyang@doocn.com
 License: MIT License
 Keywords: digicore是服务于道诚集团数字化支持部的自建第三方库项目
 Platform: any
```

### Comparing `DigiCore-1.0.7/README.md` & `DigiCore-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.7/digiCore/__init__.py` & `DigiCore-1.0.8/digiCore/__init__.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.7/digiCore/db_init.py` & `DigiCore-1.0.8/digiCore/db_init.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.7/digiCore/dsd_kafka.py` & `DigiCore-1.0.8/digiCore/dsd_kafka.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
                 "default.topic.config": {"auto.offset.reset": "latest"}  # 从提交的offset取数据，未有提交的，从最新的offset开始取数
                 }
 
         topic_part = TopicPartition(self.kafka_topic, self.partition)  # 配置主题+分区
         subscriber = Consumer(conf)  # 配置topic——config
         topic_part_out = subscriber.committed([topic_part])  # 提交主题+分区
         init_offset = topic_part_out[0].offset  # 获取当前offest位置
-        topic_part_new = TopicPartition(self.kafka_topic, 0,
+        topic_part_new = TopicPartition(self.kafka_topic, self.partition,
                                         init_offset - 10)  # 将0位置设置为当前的位置，指针回调kafka_consumer_batch
         subscriber.commit(offsets=[topic_part_new])  # 提交最新offset
         subscriber.assign([topic_part])  # 手动分配 主题+分区
         return subscriber
 
     def consume_data_from_kafka(self):
         """
```

### Comparing `DigiCore-1.0.7/digiCore/dsd_mongodb.py` & `DigiCore-1.0.8/digiCore/dsd_mongodb.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.7/digiCore/dsd_mysql.py` & `DigiCore-1.0.8/digiCore/dsd_mysql.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.7/digiCore/dsd_redis.py` & `DigiCore-1.0.8/digiCore/dsd_redis.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.7/digiCore/lingxing_api_scheduler.py` & `DigiCore-1.0.8/digiCore/lingxing_api_scheduler.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.7/digiCore/model.py` & `DigiCore-1.0.8/digiCore/model.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.7/digiCore/send_to_group.py` & `DigiCore-1.0.8/digiCore/send_to_group.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.7/digiCore/utils.py` & `DigiCore-1.0.8/digiCore/utils.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.7/k3cloud_webapi_sdk/core/webapi_client.py` & `DigiCore-1.0.8/k3cloud_webapi_sdk/core/webapi_client.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.7/k3cloud_webapi_sdk/main.py` & `DigiCore-1.0.8/k3cloud_webapi_sdk/main.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.7/k3cloud_webapi_sdk/model/cookie.py` & `DigiCore-1.0.8/k3cloud_webapi_sdk/model/cookie.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.7/k3cloud_webapi_sdk/sample.py` & `DigiCore-1.0.8/k3cloud_webapi_sdk/sample.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.7/k3cloud_webapi_sdk/util/base64_util.py` & `DigiCore-1.0.8/k3cloud_webapi_sdk/util/base64_util.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.7/k3cloud_webapi_sdk/util/config_util.py` & `DigiCore-1.0.8/k3cloud_webapi_sdk/util/config_util.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.7/k3cloud_webapi_sdk/util/encode_util.py` & `DigiCore-1.0.8/k3cloud_webapi_sdk/util/encode_util.py`

 * *Files identical despite different names*

### Comparing `DigiCore-1.0.7/setup.py` & `DigiCore-1.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 "tzdata==2023.3",
 "urllib3==2.0.2",
 "win32-setctime==1.1.0"
 ]
 
 setup(
     name="DigiCore",
-    version="1.0.7",
+    version="1.0.8",
     description="DigiCore是一个基于Python的数字化支持部第三方库，旨在为数据处理和开发提供完备的工具集和服务。",
     long_description=README,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Programming Language :: Python",
```

