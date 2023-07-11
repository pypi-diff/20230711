# Comparing `tmp/proxifier_cli-1.0.2-py3-none-any.whl.zip` & `tmp/proxifier_cli-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 3600 bytes, number of entries: 9
+Zip file size: 3576 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat       43 b- defN 23-Jun-24 20:28 proxifier_cli/__init__.py
--rw-rw-rw-  2.0 fat      358 b- defN 23-Jul-11 12:58 proxifier_cli/license.py
+-rw-rw-rw-  2.0 fat      313 b- defN 23-Jul-11 16:59 proxifier_cli/license.py
 -rw-rw-rw-  2.0 fat      465 b- defN 23-Jun-24 13:59 proxifier_cli/process.py
 -rw-rw-rw-  2.0 fat     1385 b- defN 23-Jun-24 13:21 proxifier_cli/profile.ppx
 -rw-rw-rw-  2.0 fat     1075 b- defN 23-Jun-24 20:26 proxifier_cli/profiles.py
--rw-rw-rw-  2.0 fat      509 b- defN 23-Jul-11 13:00 proxifier_cli-1.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-11 13:00 proxifier_cli-1.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 23-Jul-11 13:00 proxifier_cli-1.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      725 b- defN 23-Jul-11 13:00 proxifier_cli-1.0.2.dist-info/RECORD
-9 files, 4666 bytes uncompressed, 2344 bytes compressed:  49.8%
+-rw-rw-rw-  2.0 fat      509 b- defN 23-Jul-11 17:00 proxifier_cli-1.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-11 17:00 proxifier_cli-1.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 23-Jul-11 17:00 proxifier_cli-1.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      725 b- defN 23-Jul-11 17:00 proxifier_cli-1.0.3.dist-info/RECORD
+9 files, 4621 bytes uncompressed, 2320 bytes compressed:  49.8%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: proxifier_cli/profile.ppx
 Comment: 
 
 Filename: proxifier_cli/profiles.py
 Comment: 
 
-Filename: proxifier_cli-1.0.2.dist-info/METADATA
+Filename: proxifier_cli-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: proxifier_cli-1.0.2.dist-info/WHEEL
+Filename: proxifier_cli-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: proxifier_cli-1.0.2.dist-info/top_level.txt
+Filename: proxifier_cli-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: proxifier_cli-1.0.2.dist-info/RECORD
+Filename: proxifier_cli-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## proxifier_cli/license.py

```diff
@@ -1,11 +1,9 @@
 import winreg as wrg
 
 
-def install_license(key, owner):
-    location = wrg.HKEY_CURRENT_USER
-    soft = wrg.OpenKeyEx(location, r"SOFTWARE\\")
-    key = wrg.CreateKey(soft, "Initex\\Proxifier\\License")
-    wrg.SetValueEx(key, "Key", 0, wrg.REG_SZ, key)
+def install_license(license_key, owner):
+    key = wrg.CreateKey(wrg.HKEY_CURRENT_USER, r"SOFTWARE\\Initex\\Proxifier\\License")
+    wrg.SetValueEx(key, "Key", 0, wrg.REG_SZ, license_key)
     wrg.SetValueEx(key, "Owner", 0, wrg.REG_SZ, owner)
     if key:
         wrg.CloseKey(key)
```

## Comparing `proxifier_cli-1.0.2.dist-info/RECORD` & `proxifier_cli-1.0.3.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 proxifier_cli/__init__.py,sha256=FoTwuY8SWjdzdbAsvqrnHlpjAQRveel3VnUvh_qPYD0,43
-proxifier_cli/license.py,sha256=YPbiL5pCEfntlyTcuhx3enIBiY-JmBudEHlDI99mgNo,358
+proxifier_cli/license.py,sha256=_2b_JVAJq8i7KouCUPd68ZWGDt4XFpx38xU_bbjrd-Q,313
 proxifier_cli/process.py,sha256=_hycOlWqbcvz7_DZytFOSIjol36bcPYItO99PdGInsA,465
 proxifier_cli/profile.ppx,sha256=oRHbifT36DTd0ye4EdniRLuHVYzxwyMeRri1ho_PyQE,1385
 proxifier_cli/profiles.py,sha256=iiZWh1hLYqp9yemyykJw4sKHmBvqFb3geqKwVM8yS70,1075
-proxifier_cli-1.0.2.dist-info/METADATA,sha256=kG7iI3KurStp5VKB7l7JjQVkHRMSP0Ta3sfYwhn605U,509
-proxifier_cli-1.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-proxifier_cli-1.0.2.dist-info/top_level.txt,sha256=40Z6DIj9TQnJwgHXSPSfjWs3keZPMmkcVzUPfWpaaQU,14
-proxifier_cli-1.0.2.dist-info/RECORD,,
+proxifier_cli-1.0.3.dist-info/METADATA,sha256=uTO7CsEzsFPc784U963T-nNLi2N9ArqWv1pHK6lvBgM,509
+proxifier_cli-1.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+proxifier_cli-1.0.3.dist-info/top_level.txt,sha256=40Z6DIj9TQnJwgHXSPSfjWs3keZPMmkcVzUPfWpaaQU,14
+proxifier_cli-1.0.3.dist-info/RECORD,,
```

