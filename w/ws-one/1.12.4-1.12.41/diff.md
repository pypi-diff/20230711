# Comparing `tmp/ws_one-1.12.4-py3-none-any.whl.zip` & `tmp/ws_one-1.12.41-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 13805 bytes, number of entries: 34
+Zip file size: 13817 bytes, number of entries: 34
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Sep-30 05:48 ws_one_stable/__init__.py
 -rw-rw-rw-  2.0 fat      609 b- defN 22-Mar-29 12:06 ws_one_stable/errors.py
--rw-rw-rw-  2.0 fat     4155 b- defN 23-Jul-11 07:59 ws_one_stable/main.py
+-rw-rw-rw-  2.0 fat     4162 b- defN 23-Jul-11 09:04 ws_one_stable/main.py
 -rw-rw-rw-  2.0 fat      149 b- defN 21-Nov-29 08:04 ws_one_stable/server_test.py
 -rw-rw-rw-  2.0 fat      492 b- defN 21-Sep-30 05:48 ws_one_stable/settings.py
 -rw-rw-rw-  2.0 fat     1117 b- defN 21-Nov-29 08:04 ws_one_stable/support_functions.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Sep-30 05:48 ws_one_stable/terminals/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Sep-30 05:48 ws_one_stable/terminals/A12E/__init__.py
 -rw-rw-rw-  2.0 fat      754 b- defN 22-Aug-02 11:37 ws_one_stable/terminals/A12E/functions.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Feb-07 12:22 ws_one_stable/terminals/Art/__init__.py
@@ -24,13 +24,13 @@
 -rw-rw-rw-  2.0 fat      590 b- defN 22-Nov-14 05:04 ws_one_stable/terminals/Uvzo/functions.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-19 12:59 ws_one_stable/terminals/middle_mi010/__init__.py
 -rw-rw-rw-  2.0 fat      449 b- defN 23-Apr-19 13:34 ws_one_stable/terminals/middle_mi010/functions.py
 -rw-rw-rw-  2.0 fat        0 b- defN 21-Sep-30 05:48 ws_one_stable/tests/__init__.py
 -rw-rw-rw-  2.0 fat      145 b- defN 21-Sep-30 05:48 ws_one_stable/tests/client_test.py
 -rw-rw-rw-  2.0 fat       68 b- defN 21-Sep-30 05:48 ws_one_stable/tests/settings_test.py
 -rw-rw-rw-  2.0 fat      651 b- defN 21-Sep-30 05:48 ws_one_stable/tests/support_functions_tests.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Jul-11 08:00 ws_one-1.12.4.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1063 b- defN 23-Jul-11 08:00 ws_one-1.12.4.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-11 08:00 ws_one-1.12.4.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 23-Jul-11 08:00 ws_one-1.12.4.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     3084 b- defN 23-Jul-11 08:00 ws_one-1.12.4.dist-info/RECORD
-34 files, 17907 bytes uncompressed, 8687 bytes compressed:  51.5%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Jul-11 09:05 ws_one-1.12.41.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1064 b- defN 23-Jul-11 09:05 ws_one-1.12.41.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-11 09:05 ws_one-1.12.41.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 23-Jul-11 09:05 ws_one-1.12.41.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     3089 b- defN 23-Jul-11 09:05 ws_one-1.12.41.dist-info/RECORD
+34 files, 17920 bytes uncompressed, 8689 bytes compressed:  51.5%
```

## zipnote {}

```diff
@@ -81,23 +81,23 @@
 
 Filename: ws_one_stable/tests/settings_test.py
 Comment: 
 
 Filename: ws_one_stable/tests/support_functions_tests.py
 Comment: 
 
-Filename: ws_one-1.12.4.dist-info/LICENSE
+Filename: ws_one-1.12.41.dist-info/LICENSE
 Comment: 
 
-Filename: ws_one-1.12.4.dist-info/METADATA
+Filename: ws_one-1.12.41.dist-info/METADATA
 Comment: 
 
-Filename: ws_one-1.12.4.dist-info/WHEEL
+Filename: ws_one-1.12.41.dist-info/WHEEL
 Comment: 
 
-Filename: ws_one-1.12.4.dist-info/top_level.txt
+Filename: ws_one-1.12.41.dist-info/top_level.txt
 Comment: 
 
-Filename: ws_one-1.12.4.dist-info/RECORD
+Filename: ws_one-1.12.41.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ws_one_stable/main.py

```diff
@@ -25,15 +25,15 @@
         pass
 
     def make_new_record(self, car_number, carrier, record_id):
         self.round_info['car_number'] = car_number
         self.round_info['carrier'] = carrier
         self.round_info['record_id'] = record_id
 
-    def make_final_record(self, weight, **kwargs):
+    def make_final_record(self, weight, *args, **kwargs):
         self.round_info['weight'] = weight
 
     def turn_off_logging(self):
         pass
 
     def make_log(self, message, level='error'):
         if self.logger and level == 'critical':
```

## Comparing `ws_one-1.12.4.dist-info/LICENSE` & `ws_one-1.12.41.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ws_one-1.12.4.dist-info/METADATA` & `ws_one-1.12.41.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ws-one
-Version: 1.12.4
+Version: 1.12.41
 Author: PunchyArchy
 Author-email: ksmdrmvscthny@gmail.com
 License-File: LICENSE
 Requires-Dist: pyserial
 Requires-Dist: pds-one (==1.4.0)
 
 PDS (Port Data Splitter) - это программный разветлитель данных, реализованный в виде TCP сервера,
```

## Comparing `ws_one-1.12.4.dist-info/RECORD` & `ws_one-1.12.41.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ws_one_stable/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ws_one_stable/errors.py,sha256=fUBLIgJTpcuwoH2UBWUc6fUTiMd3Wre_-EX0AP3zn90,609
-ws_one_stable/main.py,sha256=7TX4K0FrRaPnJMAbtK90NXthPKePk4DpoUa3hh2dK2M,4155
+ws_one_stable/main.py,sha256=XOwXXQeiheT1kArvPYytkA-UATqF3ncM0tA9Xg0QUqo,4162
 ws_one_stable/server_test.py,sha256=CYjXceXg5g7A_9Y6nHIUhbbpCUcMdT3HHNF62C_i-7I,149
 ws_one_stable/settings.py,sha256=GfZtA-2BkL1WshrpD3MSBMQlZ5ZNkcJ4oi7aLop0aVk,492
 ws_one_stable/support_functions.py,sha256=3SFbEHTtqWvGq8vynn-Qy2zuHVZfL1S7fe384lMeznA,1117
 ws_one_stable/terminals/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ws_one_stable/terminals/A12E/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ws_one_stable/terminals/A12E/functions.py,sha256=2avi3S23LS4Yi5RjfUcGaA7ENoyqp4EIKFBMPDBVwrc,754
 ws_one_stable/terminals/Art/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -23,12 +23,12 @@
 ws_one_stable/terminals/Uvzo/functions.py,sha256=IKBj2mvpcVXQDwLqw2Uua99Z8bCIiE22TVwP2R-7RtA,590
 ws_one_stable/terminals/middle_mi010/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ws_one_stable/terminals/middle_mi010/functions.py,sha256=rhorjJzlm3-2LbdPIldrGdwALlDzX9eNZyiHT_PWMqM,449
 ws_one_stable/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ws_one_stable/tests/client_test.py,sha256=2xT9G4dOB66pYp7pQ4pjiRdihGioz3gUo9k-TcWcbaw,145
 ws_one_stable/tests/settings_test.py,sha256=uhQjp-fDlMZW3_Q0uDFRBg_bjujcUNSnk8tGqXEjgo4,68
 ws_one_stable/tests/support_functions_tests.py,sha256=u_7UqjhrUqjUlFQi8x4gVQ2ERqe54NMVXRdZmI57cqw,651
-ws_one-1.12.4.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-ws_one-1.12.4.dist-info/METADATA,sha256=4YslhAazlBK7U8EogstSF7CFK2m86D19bfo4OLQVc04,1063
-ws_one-1.12.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ws_one-1.12.4.dist-info/top_level.txt,sha256=VucC9pCRaAyG119eEE7EoLBql-CDOLFUfKGqOxGIA8Q,14
-ws_one-1.12.4.dist-info/RECORD,,
+ws_one-1.12.41.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+ws_one-1.12.41.dist-info/METADATA,sha256=6LM1DaUO_92CTSSE9HPk9uZaZKMGs4uTfFvL5KxFQk0,1064
+ws_one-1.12.41.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ws_one-1.12.41.dist-info/top_level.txt,sha256=VucC9pCRaAyG119eEE7EoLBql-CDOLFUfKGqOxGIA8Q,14
+ws_one-1.12.41.dist-info/RECORD,,
```

