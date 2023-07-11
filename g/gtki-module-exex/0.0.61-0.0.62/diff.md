# Comparing `tmp/gtki_module_exex-0.0.61-py3-none-any.whl.zip` & `tmp/gtki_module_exex-0.0.62-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 6795 bytes, number of entries: 11
+Zip file size: 6839 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Jun-09 04:59 gtki_module_exex/__init__.py
--rw-rw-rw-  2.0 fat    11924 b- defN 23-Jul-06 12:22 gtki_module_exex/main.py
+-rw-rw-rw-  2.0 fat    12133 b- defN 23-Jul-11 13:27 gtki_module_exex/main.py
 -rw-rw-rw-  2.0 fat     1431 b- defN 23-Jun-15 14:51 gtki_module_exex/mixins.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Jun-09 05:22 gtki_module_exex/tests/__init__.py
 -rw-rw-rw-  2.0 fat     2251 b- defN 23-Jul-06 07:30 gtki_module_exex/tests/main_tests.py
 -rw-rw-rw-  2.0 fat     1007 b- defN 22-Jun-09 05:55 gtki_module_exex/tests/mixins_tests.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Jul-06 12:26 gtki_module_exex-0.0.61.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      280 b- defN 23-Jul-06 12:26 gtki_module_exex-0.0.61.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-06 12:26 gtki_module_exex-0.0.61.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-06 12:26 gtki_module_exex-0.0.61.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      958 b- defN 23-Jul-06 12:26 gtki_module_exex-0.0.61.dist-info/RECORD
-11 files, 19051 bytes uncompressed, 5147 bytes compressed:  73.0%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Jul-11 13:29 gtki_module_exex-0.0.62.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      280 b- defN 23-Jul-11 13:29 gtki_module_exex-0.0.62.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-11 13:29 gtki_module_exex-0.0.62.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-11 13:29 gtki_module_exex-0.0.62.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      958 b- defN 23-Jul-11 13:29 gtki_module_exex-0.0.62.dist-info/RECORD
+11 files, 19260 bytes uncompressed, 5191 bytes compressed:  73.0%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: gtki_module_exex/tests/main_tests.py
 Comment: 
 
 Filename: gtki_module_exex/tests/mixins_tests.py
 Comment: 
 
-Filename: gtki_module_exex-0.0.61.dist-info/LICENSE
+Filename: gtki_module_exex-0.0.62.dist-info/LICENSE
 Comment: 
 
-Filename: gtki_module_exex-0.0.61.dist-info/METADATA
+Filename: gtki_module_exex-0.0.62.dist-info/METADATA
 Comment: 
 
-Filename: gtki_module_exex-0.0.61.dist-info/WHEEL
+Filename: gtki_module_exex-0.0.62.dist-info/WHEEL
 Comment: 
 
-Filename: gtki_module_exex-0.0.61.dist-info/top_level.txt
+Filename: gtki_module_exex-0.0.62.dist-info/top_level.txt
 Comment: 
 
-Filename: gtki_module_exex-0.0.61.dist-info/RECORD
+Filename: gtki_module_exex-0.0.62.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gtki_module_exex/main.py

```diff
@@ -152,22 +152,28 @@
         start_row = self.set_column_names()
         new_row = start_row
         for tc in ["ТКО", "ПО", "Хвосты", "Прочее"]:
             new_row = self.operate_trash_cat(tc, day.strftime("%Y.%m.%d"),
                                              start_row=new_row)
             amounts.append(new_row + 2)
             new_row += 1
-        row = self.add_hyundai(day, new_row)
-        amounts.append(row + 2)
-        row = self.add_phys(day, row + 2)
-        amounts.append(row + 2)
-        row = self.add_recyclables(day, row + 2)
-        amounts.append(row + 2)
+        hyn_row = self.add_hyundai(day, new_row)
+        if hyn_row:
+            amounts.append(hyn_row + 2)
+            new_row = hyn_row
+        phys_row = self.add_phys(day, new_row + 2)
+        if phys_row:
+            amounts.append(phys_row + 2)
+            new_row = phys_row
+        rec_row = self.add_recyclables(day, new_row + 2)
+        if rec_row:
+            amounts.append(rec_row + 2)
+            new_row = phys_row
         row = self.set_amount(start_record_row=start_row,
-                              end_record_row=row + 2, alias="ВСЕГО")
+                              end_record_row=new_row + 2, alias="ВСЕГО")
         row = self.set_final_amount(row, amounts)
         self.set_borders(row + 1)
         self.add_user_info(row)
         self.workbook.close()
 
     def add_user_info(self, row):
         row += 3
```

## Comparing `gtki_module_exex-0.0.61.dist-info/LICENSE` & `gtki_module_exex-0.0.62.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gtki_module_exex-0.0.61.dist-info/RECORD` & `gtki_module_exex-0.0.62.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 gtki_module_exex/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-gtki_module_exex/main.py,sha256=HeGMlomUDQFjXxQIbNkj5kZy5C8JvmugvAx6Tf0D39E,11924
+gtki_module_exex/main.py,sha256=OAnFMjHweOA2RgoICmiaeifZWcDsCsBpkGWLTDBrMPo,12133
 gtki_module_exex/mixins.py,sha256=nKYRHMoFYSva364Q2WyH30SefjAxi5xGXekgLmRAyXk,1431
 gtki_module_exex/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 gtki_module_exex/tests/main_tests.py,sha256=ZTo-ylgaHZCNeMuVtoktNdEzwioc9r6XU7EWCgpVfGw,2251
 gtki_module_exex/tests/mixins_tests.py,sha256=8oogAhtkQgyhB3sUEsIvQpvA1a7YrRPc76bDHKsxodI,1007
-gtki_module_exex-0.0.61.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-gtki_module_exex-0.0.61.dist-info/METADATA,sha256=JjdAoTwWqcumhK0MQjWtoMpBZ7B_KZ4qQ_5XzT-t828,280
-gtki_module_exex-0.0.61.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-gtki_module_exex-0.0.61.dist-info/top_level.txt,sha256=5fDck53WZ0oTnmcblVZKn9XwbA-Uqijh0L93F1ml9Bc,17
-gtki_module_exex-0.0.61.dist-info/RECORD,,
+gtki_module_exex-0.0.62.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+gtki_module_exex-0.0.62.dist-info/METADATA,sha256=FlVsj1Ya1lMBtYMspb17NMslCY9H14tdN0QSI8Zaaf8,280
+gtki_module_exex-0.0.62.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+gtki_module_exex-0.0.62.dist-info/top_level.txt,sha256=5fDck53WZ0oTnmcblVZKn9XwbA-Uqijh0L93F1ml9Bc,17
+gtki_module_exex-0.0.62.dist-info/RECORD,,
```

