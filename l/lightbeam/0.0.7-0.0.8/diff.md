# Comparing `tmp/lightbeam-0.0.7-py3-none-any.whl.zip` & `tmp/lightbeam-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 30090 bytes, number of entries: 17
+Zip file size: 30145 bytes, number of entries: 17
 -rw-r--r--  2.0 unx        0 b- defN 22-Sep-16 20:03 lightbeam/__init__.py
 -rw-r--r--  2.0 unx     4806 b- defN 23-Jun-13 20:45 lightbeam/__main__.py
 -rw-r--r--  2.0 unx    18633 b- defN 23-Jun-13 20:45 lightbeam/api.py
 -rw-r--r--  2.0 unx     8914 b- defN 23-Jan-25 19:00 lightbeam/delete.py
 -rw-r--r--  2.0 unx      672 b- defN 22-Sep-19 14:49 lightbeam/hashlog.py
 -rw-r--r--  2.0 unx    10226 b- defN 23-Jun-13 20:45 lightbeam/lightbeam.py
--rw-r--r--  2.0 unx    11064 b- defN 23-Jun-13 21:40 lightbeam/send.py
+-rw-r--r--  2.0 unx    11283 b- defN 23-Jul-11 15:17 lightbeam/send.py
 -rw-r--r--  2.0 unx     1329 b- defN 22-Sep-21 16:31 lightbeam/util.py
 -rw-r--r--  2.0 unx     5888 b- defN 22-Sep-20 13:42 lightbeam/validate.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Jun-28 14:58 lightbeam/resources/__init__.py
--rwxrwxrwx  2.0 unx    11349 b- defN 23-Jun-13 21:49 lightbeam-0.0.7.dist-info/LICENSE
--rw-r--r--  2.0 unx    15234 b- defN 23-Jun-13 21:49 lightbeam-0.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 21:49 lightbeam-0.0.7.dist-info/WHEEL
--rwxrwxrwx  2.0 unx      132 b- defN 23-Jun-13 21:49 lightbeam-0.0.7.dist-info/dependency_links.txt
--rwxrwxrwx  2.0 unx       54 b- defN 23-Jun-13 21:49 lightbeam-0.0.7.dist-info/entry_points.txt
--rwxrwxrwx  2.0 unx       10 b- defN 23-Jun-13 21:49 lightbeam-0.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1368 b- defN 23-Jun-13 21:49 lightbeam-0.0.7.dist-info/RECORD
-17 files, 89771 bytes uncompressed, 27852 bytes compressed:  69.0%
+-rwxrwxrwx  2.0 unx    11349 b- defN 23-Jul-11 15:31 lightbeam-0.0.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx    15234 b- defN 23-Jul-11 15:31 lightbeam-0.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-11 15:31 lightbeam-0.0.8.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx      132 b- defN 23-Jul-11 15:31 lightbeam-0.0.8.dist-info/dependency_links.txt
+-rwxrwxrwx  2.0 unx       54 b- defN 23-Jul-11 15:31 lightbeam-0.0.8.dist-info/entry_points.txt
+-rwxrwxrwx  2.0 unx       10 b- defN 23-Jul-11 15:31 lightbeam-0.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1368 b- defN 23-Jul-11 15:31 lightbeam-0.0.8.dist-info/RECORD
+17 files, 89990 bytes uncompressed, 27907 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -24,29 +24,29 @@
 
 Filename: lightbeam/validate.py
 Comment: 
 
 Filename: lightbeam/resources/__init__.py
 Comment: 
 
-Filename: lightbeam-0.0.7.dist-info/LICENSE
+Filename: lightbeam-0.0.8.dist-info/LICENSE
 Comment: 
 
-Filename: lightbeam-0.0.7.dist-info/METADATA
+Filename: lightbeam-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: lightbeam-0.0.7.dist-info/WHEEL
+Filename: lightbeam-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: lightbeam-0.0.7.dist-info/dependency_links.txt
+Filename: lightbeam-0.0.8.dist-info/dependency_links.txt
 Comment: 
 
-Filename: lightbeam-0.0.7.dist-info/entry_points.txt
+Filename: lightbeam-0.0.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: lightbeam-0.0.7.dist-info/top_level.txt
+Filename: lightbeam-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: lightbeam-0.0.7.dist-info/RECORD
+Filename: lightbeam-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lightbeam/send.py

```diff
@@ -62,15 +62,20 @@
                             file_metadata.update({
                                 "count": num_errs,
                                 "line_numbers": ",".join(str(x) for x in file_metadata["line_numbers"])
                             })
                             total_num_errs += num_errs
                     status_metadata.update({"count": total_num_errs})
         
+        ### Create structured output results_file if necessary
         if self.lightbeam.results_file:
+            
+            # create directory if not exists
+            os.makedirs(os.path.dirname(self.lightbeam.results_file), exist_ok=True)
+            
             with open(self.lightbeam.results_file, 'w') as fp:
                 fp.write(json.dumps(self.metadata, indent=4))
 
         if self.metadata["total_records_processed"] == self.metadata["total_records_skipped"]:
             self.logger.info("all payloads skipped")
             exit(99) # signal to downstream tasks (in Airflow) all payloads skipped
```

## Comparing `lightbeam-0.0.7.dist-info/LICENSE` & `lightbeam-0.0.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `lightbeam-0.0.7.dist-info/METADATA` & `lightbeam-0.0.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightbeam
-Version: 0.0.7
+Version: 0.0.8
 Summary: Sends JSONL data into an Ed-Fi API
 Home-page: https://github.com/edanalytics/lightbeam
 Download-URL: https://github.com/edanalytics/lightbeam/archive/0.0.1.tar.gz
 Author: Tom Reitz
 Author-email: treitz@edanalytics.org
 License: Apache 2.0
 Keywords: data,transmission,api,edfi
```

## Comparing `lightbeam-0.0.7.dist-info/RECORD` & `lightbeam-0.0.8.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 lightbeam/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 lightbeam/__main__.py,sha256=n_GcH5OcHNr0LyU5o8dGbVrDEQwlEK6SsAxpKLM4voA,4806
 lightbeam/api.py,sha256=Hj-_8AXi74iK0b1guiIVwALaE9YeKseTgoI3UFJ11fM,18633
 lightbeam/delete.py,sha256=_2AfXRswfFsV3dhd0ZYHFnEPJMxCmWaUwSK8a_vF8os,8914
 lightbeam/hashlog.py,sha256=K6A0xXhkoWgOpjg6WlF5_bp-YvinH27lOhPb815shrs,672
 lightbeam/lightbeam.py,sha256=MOS11VQfQIInDz2aU0P7VESaeB4hwKAIr1mT6NvLhGA,10226
-lightbeam/send.py,sha256=Otn3dO-YKbwJfappmMswHhBTIUduz_yfBtEVO0pwV-k,11064
+lightbeam/send.py,sha256=zMhxxZBXRG-0rq64JHUwBPVtsO1YYUD9p-zmiIuivug,11283
 lightbeam/util.py,sha256=Nem1rzVdcPya1g6rY_fxGm3QRQnrqHR4PAHy9KOdE9I,1329
 lightbeam/validate.py,sha256=96fcQAMT8jAcp_pz3uDTAoc9YHbQJbSE_GYc88siFO4,5888
 lightbeam/resources/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-lightbeam-0.0.7.dist-info/LICENSE,sha256=QoIB1PHNf6dGs6i0VkXumtNelR-vv2rfNMAHMnlaIDw,11349
-lightbeam-0.0.7.dist-info/METADATA,sha256=bqvweTpVjqlhHiR4DIIG97KsIZmpjpozvmsx-mYT9DI,15234
-lightbeam-0.0.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-lightbeam-0.0.7.dist-info/dependency_links.txt,sha256=zaXVnhNfDDVKDG63P2d5g3NMI6enCOEsVLmo7bmHAjA,132
-lightbeam-0.0.7.dist-info/entry_points.txt,sha256=BbLylxOffnTGU7NfApSlFKDf_C0S-fqE_mcvz0iuuKA,54
-lightbeam-0.0.7.dist-info/top_level.txt,sha256=k8DpVRedspxz4O88pMNN_ClMaC22KtuvkF1HHsxiUow,10
-lightbeam-0.0.7.dist-info/RECORD,,
+lightbeam-0.0.8.dist-info/LICENSE,sha256=QoIB1PHNf6dGs6i0VkXumtNelR-vv2rfNMAHMnlaIDw,11349
+lightbeam-0.0.8.dist-info/METADATA,sha256=6IyaeawrCLtqGdWMXJyVgFzfVGcyT4YHaKlhmct9ISY,15234
+lightbeam-0.0.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+lightbeam-0.0.8.dist-info/dependency_links.txt,sha256=zaXVnhNfDDVKDG63P2d5g3NMI6enCOEsVLmo7bmHAjA,132
+lightbeam-0.0.8.dist-info/entry_points.txt,sha256=BbLylxOffnTGU7NfApSlFKDf_C0S-fqE_mcvz0iuuKA,54
+lightbeam-0.0.8.dist-info/top_level.txt,sha256=k8DpVRedspxz4O88pMNN_ClMaC22KtuvkF1HHsxiUow,10
+lightbeam-0.0.8.dist-info/RECORD,,
```

