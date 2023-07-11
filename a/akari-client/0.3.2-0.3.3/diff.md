# Comparing `tmp/akari-client-0.3.2.tar.gz` & `tmp/akari-client-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "akari-client-0.3.2.tar", last modified: Mon May 22 02:20:15 2023, max compression
+gzip compressed data, was "akari-client-0.3.3.tar", last modified: Tue Jul 11 07:59:56 2023, max compression
```

## Comparing `akari-client-0.3.2.tar` & `akari-client-0.3.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 igarashi  (1002) igarashi  (1002)        0 2023-05-22 02:20:15.975682 akari-client-0.3.2/
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     1461 2023-05-22 02:20:15.975682 akari-client-0.3.2/PKG-INFO
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)      725 2023-05-22 00:31:41.000000 akari-client-0.3.2/README.md
-drwxrwxr-x   0 igarashi  (1002) igarashi  (1002)        0 2023-05-22 02:20:15.975682 akari-client-0.3.2/akari_client/
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)       87 2023-01-29 18:11:01.000000 akari-client-0.3.2/akari_client/__init__.py
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)      920 2023-01-29 18:11:01.000000 akari-client-0.3.2/akari_client/akari_client.py
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     2014 2023-01-29 18:11:01.000000 akari-client-0.3.2/akari_client/color.py
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     3717 2023-01-29 18:11:01.000000 akari-client-0.3.2/akari_client/config.py
-drwxrwxr-x   0 igarashi  (1002) igarashi  (1002)        0 2023-05-22 02:20:15.975682 akari-client-0.3.2/akari_client/grpc/
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)        0 2023-01-29 18:11:01.000000 akari-client-0.3.2/akari_client/grpc/__init__.py
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)      125 2023-01-29 18:11:01.000000 akari-client-0.3.2/akari_client/grpc/_error.py
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)      656 2023-01-29 18:11:01.000000 akari-client-0.3.2/akari_client/grpc/channel_pool.py
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     1434 2023-01-29 18:11:01.000000 akari-client-0.3.2/akari_client/grpc/factory.py
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     4096 2023-01-29 18:11:01.000000 akari-client-0.3.2/akari_client/grpc/joints_controller.py
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     4739 2023-05-22 00:31:41.000000 akari-client-0.3.2/akari_client/grpc/m5stack.py
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     2478 2023-01-29 18:11:01.000000 akari-client-0.3.2/akari_client/joint_controller.py
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     8960 2023-05-22 00:31:41.000000 akari-client-0.3.2/akari_client/joint_manager.py
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)    11435 2023-05-22 00:31:41.000000 akari-client-0.3.2/akari_client/m5stack_client.py
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)      374 2023-01-29 18:11:01.000000 akari-client-0.3.2/akari_client/position.py
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)        0 2023-01-29 18:11:01.000000 akari-client-0.3.2/akari_client/py.typed
-drwxrwxr-x   0 igarashi  (1002) igarashi  (1002)        0 2023-05-22 02:20:15.975682 akari-client-0.3.2/akari_client/serial/
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)        0 2023-01-29 18:11:01.000000 akari-client-0.3.2/akari_client/serial/__init__.py
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     6666 2023-01-29 18:11:01.000000 akari-client-0.3.2/akari_client/serial/dynamixel.py
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     4538 2023-01-29 18:11:01.000000 akari-client-0.3.2/akari_client/serial/dynamixel_communicator.py
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     1405 2023-01-29 18:11:01.000000 akari-client-0.3.2/akari_client/serial/factory.py
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     4599 2023-05-22 00:31:41.000000 akari-client-0.3.2/akari_client/serial/m5stack.py
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     4299 2023-05-22 00:31:41.000000 akari-client-0.3.2/akari_client/serial/m5stack_communicator.py
-drwxrwxr-x   0 igarashi  (1002) igarashi  (1002)        0 2023-05-22 02:20:15.975682 akari-client-0.3.2/akari_client.egg-info/
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     1461 2023-05-22 02:20:15.000000 akari-client-0.3.2/akari_client.egg-info/PKG-INFO
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)      843 2023-05-22 02:20:15.000000 akari-client-0.3.2/akari_client.egg-info/SOURCES.txt
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)        1 2023-05-22 02:20:15.000000 akari-client-0.3.2/akari_client.egg-info/dependency_links.txt
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)      157 2023-05-22 02:20:15.000000 akari-client-0.3.2/akari_client.egg-info/requires.txt
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)       13 2023-05-22 02:20:15.000000 akari-client-0.3.2/akari_client.egg-info/top_level.txt
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)       38 2023-05-22 02:20:15.975682 akari-client-0.3.2/setup.cfg
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     1316 2023-05-22 00:31:41.000000 akari-client-0.3.2/setup.py
+drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-07-11 07:59:56.810336 akari-client-0.3.3/
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1708 2023-07-11 07:59:56.810336 akari-client-0.3.3/PKG-INFO
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      725 2023-07-11 07:38:40.000000 akari-client-0.3.3/README.md
+drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-07-11 07:59:56.810336 akari-client-0.3.3/akari_client/
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       87 2022-07-18 04:31:24.000000 akari-client-0.3.3/akari_client/__init__.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      920 2022-11-11 00:49:49.000000 akari-client-0.3.3/akari_client/akari_client.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     2014 2022-12-31 07:02:59.000000 akari-client-0.3.3/akari_client/color.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     3717 2023-01-09 03:09:46.000000 akari-client-0.3.3/akari_client/config.py
+drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-07-11 07:59:56.810336 akari-client-0.3.3/akari_client/grpc/
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        0 2023-01-09 03:09:57.000000 akari-client-0.3.3/akari_client/grpc/__init__.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      125 2022-08-13 07:11:41.000000 akari-client-0.3.3/akari_client/grpc/_error.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      656 2022-08-13 07:11:41.000000 akari-client-0.3.3/akari_client/grpc/channel_pool.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1434 2022-08-13 07:11:41.000000 akari-client-0.3.3/akari_client/grpc/factory.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     4096 2022-11-07 07:21:30.000000 akari-client-0.3.3/akari_client/grpc/joints_controller.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     4739 2023-02-08 15:51:00.000000 akari-client-0.3.3/akari_client/grpc/m5stack.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     2478 2022-12-31 07:02:59.000000 akari-client-0.3.3/akari_client/joint_controller.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     9641 2023-07-11 07:38:40.000000 akari-client-0.3.3/akari_client/joint_manager.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)    11435 2023-02-08 15:51:00.000000 akari-client-0.3.3/akari_client/m5stack_client.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      374 2022-12-31 07:02:59.000000 akari-client-0.3.3/akari_client/position.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        0 2023-01-09 03:09:57.000000 akari-client-0.3.3/akari_client/py.typed
+drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-07-11 07:59:56.810336 akari-client-0.3.3/akari_client/serial/
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        0 2023-01-09 03:09:57.000000 akari-client-0.3.3/akari_client/serial/__init__.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     6666 2022-12-31 07:02:59.000000 akari-client-0.3.3/akari_client/serial/dynamixel.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     4538 2022-11-07 09:30:25.000000 akari-client-0.3.3/akari_client/serial/dynamixel_communicator.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1405 2022-08-13 07:11:41.000000 akari-client-0.3.3/akari_client/serial/factory.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     4599 2023-02-08 15:51:00.000000 akari-client-0.3.3/akari_client/serial/m5stack.py
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     4299 2023-07-11 07:38:40.000000 akari-client-0.3.3/akari_client/serial/m5stack_communicator.py
+drwxrwxr-x   0 igarashi  (1000) igarashi  (1000)        0 2023-07-11 07:59:56.810336 akari-client-0.3.3/akari_client.egg-info/
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1708 2023-07-11 07:59:56.000000 akari-client-0.3.3/akari_client.egg-info/PKG-INFO
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      843 2023-07-11 07:59:56.000000 akari-client-0.3.3/akari_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)        1 2023-07-11 07:59:56.000000 akari-client-0.3.3/akari_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)      157 2023-07-11 07:59:56.000000 akari-client-0.3.3/akari_client.egg-info/requires.txt
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       13 2023-07-11 07:59:56.000000 akari-client-0.3.3/akari_client.egg-info/top_level.txt
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)       38 2023-07-11 07:59:56.810336 akari-client-0.3.3/setup.cfg
+-rw-rw-r--   0 igarashi  (1000) igarashi  (1000)     1316 2023-07-11 07:38:40.000000 akari-client-0.3.3/setup.py
```

### Comparing `akari-client-0.3.2/PKG-INFO` & `akari-client-0.3.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 Metadata-Version: 2.1
 Name: akari-client
-Version: 0.3.2
+Version: 0.3.3
 Summary: Akari Python package
 Home-page: https://github.com/AkariGroup/akari_software
 Author: akari
 Author-email: akari.tmc@gmail.com
 License: Apache License 2.0
+Description: # akari\_client
+        
+        [AKARI](https://github.com/AkariGroup/) を使うためのクライアントライブラリ
+        
+        ## インストール
+        
+        ```sh
+        pip install akari_client
+        ```
+        
+        **注意:** `akari_client` を使う前に `AKARI` 本体の設定が完了している必要があります。
+        詳しくはオンラインドキュメントを参照してください。
+        
+        ## Getting Started: ディスプレイに文字を表示する
+        
+        ```py
+        with AkariClient() as akari:
+            m5 = akari.m5stack
+            m5.set_display_text("Hello, world!")
+        ```
+        
+        その他のサンプルや使い方はオンラインドキュメントを参照してください。
+        
+        ## ドキュメント
+        
+        [https://AkariGroup.github.io/docs](https://AkariGroup.github.io/docs)
+        
+        
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
 Provides-Extra: grpc
 Provides-Extra: depthai
-
-# akari\_client
-
-[AKARI](https://github.com/AkariGroup/) を使うためのクライアントライブラリ
-
-## インストール
-
-```sh
-pip install akari_client
-```
-
-**注意:** `akari_client` を使う前に `AKARI` 本体の設定が完了している必要があります。
-詳しくはオンラインドキュメントを参照してください。
-
-## Getting Started: ディスプレイに文字を表示する
-
-```py
-with AkariClient() as akari:
-    m5 = akari.m5stack
-    m5.set_display_text("Hello, world!")
-```
-
-その他のサンプルや使い方はオンラインドキュメントを参照してください。
-
-## ドキュメント
-
-[https://AkariGroup.github.io/docs](https://AkariGroup.github.io/docs)
-
```

### Comparing `akari-client-0.3.2/README.md` & `akari-client-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.2/akari_client/akari_client.py` & `akari-client-0.3.3/akari_client/akari_client.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.2/akari_client/color.py` & `akari-client-0.3.3/akari_client/color.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.2/akari_client/config.py` & `akari-client-0.3.3/akari_client/config.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.2/akari_client/grpc/channel_pool.py` & `akari-client-0.3.3/akari_client/grpc/channel_pool.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.2/akari_client/grpc/factory.py` & `akari-client-0.3.3/akari_client/grpc/factory.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.2/akari_client/grpc/joints_controller.py` & `akari-client-0.3.3/akari_client/grpc/joints_controller.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.2/akari_client/grpc/m5stack.py` & `akari-client-0.3.3/akari_client/grpc/m5stack.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.2/akari_client/joint_controller.py` & `akari-client-0.3.3/akari_client/joint_controller.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.2/akari_client/joint_manager.py` & `akari-client-0.3.3/akari_client/joint_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -273,7 +273,28 @@
             >>> joints = akari.joints
             >>> joints.disable_all_servo()
             # pan、tiltのサーボ両方を無効に設定
 
         """
         for joint in self._joints.values():
             joint.set_servo_enabled(False)
+
+    def get_moving_state(self) -> Dict[str, bool]:
+        """サーボが現在移動中かを取得する。
+            停止中ならTrue、移動中ならFalseを返す。
+
+        Returns:
+            サーボ名と現在状態のdict
+
+        Example:
+            >>> from akari_client import AkariClient
+            >>> akari = AkariClient()
+            >>> joints = akari.joints
+            >>> print(joints.get_moving_state())
+            # 各軸の現在状態が出力される
+
+        """
+        ret: Dict[str, bool] = {}
+        for joint_name, controller in self._joints.items():
+            ret[joint_name] = controller.get_moving_state()
+
+        return ret
```

### Comparing `akari-client-0.3.2/akari_client/m5stack_client.py` & `akari-client-0.3.3/akari_client/m5stack_client.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.2/akari_client/serial/dynamixel.py` & `akari-client-0.3.3/akari_client/serial/dynamixel.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.2/akari_client/serial/dynamixel_communicator.py` & `akari-client-0.3.3/akari_client/serial/dynamixel_communicator.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.2/akari_client/serial/factory.py` & `akari-client-0.3.3/akari_client/serial/factory.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.2/akari_client/serial/m5stack.py` & `akari-client-0.3.3/akari_client/serial/m5stack.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.2/akari_client/serial/m5stack_communicator.py` & `akari-client-0.3.3/akari_client/serial/m5stack_communicator.py`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.2/akari_client.egg-info/PKG-INFO` & `akari-client-0.3.3/akari_client.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 Metadata-Version: 2.1
 Name: akari-client
-Version: 0.3.2
+Version: 0.3.3
 Summary: Akari Python package
 Home-page: https://github.com/AkariGroup/akari_software
 Author: akari
 Author-email: akari.tmc@gmail.com
 License: Apache License 2.0
+Description: # akari\_client
+        
+        [AKARI](https://github.com/AkariGroup/) を使うためのクライアントライブラリ
+        
+        ## インストール
+        
+        ```sh
+        pip install akari_client
+        ```
+        
+        **注意:** `akari_client` を使う前に `AKARI` 本体の設定が完了している必要があります。
+        詳しくはオンラインドキュメントを参照してください。
+        
+        ## Getting Started: ディスプレイに文字を表示する
+        
+        ```py
+        with AkariClient() as akari:
+            m5 = akari.m5stack
+            m5.set_display_text("Hello, world!")
+        ```
+        
+        その他のサンプルや使い方はオンラインドキュメントを参照してください。
+        
+        ## ドキュメント
+        
+        [https://AkariGroup.github.io/docs](https://AkariGroup.github.io/docs)
+        
+        
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
 Provides-Extra: grpc
 Provides-Extra: depthai
-
-# akari\_client
-
-[AKARI](https://github.com/AkariGroup/) を使うためのクライアントライブラリ
-
-## インストール
-
-```sh
-pip install akari_client
-```
-
-**注意:** `akari_client` を使う前に `AKARI` 本体の設定が完了している必要があります。
-詳しくはオンラインドキュメントを参照してください。
-
-## Getting Started: ディスプレイに文字を表示する
-
-```py
-with AkariClient() as akari:
-    m5 = akari.m5stack
-    m5.set_display_text("Hello, world!")
-```
-
-その他のサンプルや使い方はオンラインドキュメントを参照してください。
-
-## ドキュメント
-
-[https://AkariGroup.github.io/docs](https://AkariGroup.github.io/docs)
-
```

### Comparing `akari-client-0.3.2/akari_client.egg-info/SOURCES.txt` & `akari-client-0.3.3/akari_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `akari-client-0.3.2/setup.py` & `akari-client-0.3.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="akari-client",
-    version="0.3.2",
+    version="0.3.3",
     packages=find_packages(exclude=["tests"]),
     description="Akari Python package",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="akari",
     author_email="akari.tmc@gmail.com",
     license="Apache License 2.0",
```

