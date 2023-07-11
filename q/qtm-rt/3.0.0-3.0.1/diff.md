# Comparing `tmp/qtm_rt-3.0.0-py3-none-any.whl.zip` & `tmp/qtm_rt-3.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 3109015 bytes, number of entries: 15
--rw-rw-rw-  2.0 fat      703 b- defN 23-Jun-12 07:33 qtm_rt/__init__.py
--rw-rw-rw-  2.0 fat      677 b- defN 23-Jun-12 07:33 qtm_rt/control.py
--rw-rw-rw-  2.0 fat     2994 b- defN 23-Jun-12 07:34 qtm_rt/discovery.py
--rw-rw-rw-  2.0 fat    24141 b- defN 23-Jun-12 07:34 qtm_rt/packet.py
--rw-rw-rw-  2.0 fat     5985 b- defN 23-Jun-12 07:34 qtm_rt/protocol.py
--rw-rw-rw-  2.0 fat    13639 b- defN 23-Jun-12 07:35 qtm_rt/qrt.py
--rw-rw-rw-  2.0 fat      928 b- defN 23-Jun-12 07:36 qtm_rt/reboot.py
--rw-rw-rw-  2.0 fat     1570 b- defN 23-Jun-12 07:36 qtm_rt/receiver.py
--rw-rw-rw-  2.0 fat  4259840 b- defN 23-Jun-09 15:07 qtm_rt/data/demo.qtm
--rw-rw-rw-  2.0 fat     1101 b- defN 23-Jun-12 08:01 qtm_rt-3.0.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      773 b- defN 23-Jun-12 08:01 qtm_rt-3.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-12 08:01 qtm_rt-3.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Jun-12 08:01 qtm_rt-3.0.0.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-Jun-12 07:58 qtm_rt-3.0.0.dist-info/zip-safe
-?rw-rw-r--  2.0 fat     1134 b- defN 23-Jun-12 08:01 qtm_rt-3.0.0.dist-info/RECORD
-15 files, 4313586 bytes uncompressed, 3107173 bytes compressed:  28.0%
+Zip file size: 3109054 bytes, number of entries: 15
+-rw-rw-rw-  2.0 fat      703 b- defN 23-Jul-11 13:29 qtm_rt/__init__.py
+-rw-rw-rw-  2.0 fat      677 b- defN 23-Jul-11 13:29 qtm_rt/control.py
+-rw-rw-rw-  2.0 fat     3120 b- defN 23-Jul-11 13:29 qtm_rt/discovery.py
+-rw-rw-rw-  2.0 fat    24141 b- defN 23-Jul-11 13:29 qtm_rt/packet.py
+-rw-rw-rw-  2.0 fat     5985 b- defN 23-Jul-11 13:29 qtm_rt/protocol.py
+-rw-rw-rw-  2.0 fat    13639 b- defN 23-Jul-11 13:29 qtm_rt/qrt.py
+-rw-rw-rw-  2.0 fat      928 b- defN 23-Jul-11 13:29 qtm_rt/reboot.py
+-rw-rw-rw-  2.0 fat     1570 b- defN 23-Jul-11 13:29 qtm_rt/receiver.py
+-rw-rw-rw-  2.0 fat  4259840 b- defN 23-Jul-11 13:29 qtm_rt/data/demo.qtm
+-rw-rw-rw-  2.0 fat     1101 b- defN 23-Jul-11 13:38 qtm_rt-3.0.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      797 b- defN 23-Jul-11 13:38 qtm_rt-3.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-11 13:38 qtm_rt-3.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Jul-11 13:38 qtm_rt-3.0.1.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-Jun-28 10:39 qtm_rt-3.0.1.dist-info/zip-safe
+-rw-rw-r--  2.0 fat     1134 b- defN 23-Jul-11 13:38 qtm_rt-3.0.1.dist-info/RECORD
+15 files, 4313736 bytes uncompressed, 3107212 bytes compressed:  28.0%
```

## zipnote {}

```diff
@@ -21,26 +21,26 @@
 
 Filename: qtm_rt/receiver.py
 Comment: 
 
 Filename: qtm_rt/data/demo.qtm
 Comment: 
 
-Filename: qtm_rt-3.0.0.dist-info/LICENSE
+Filename: qtm_rt-3.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: qtm_rt-3.0.0.dist-info/METADATA
+Filename: qtm_rt-3.0.1.dist-info/METADATA
 Comment: 
 
-Filename: qtm_rt-3.0.0.dist-info/WHEEL
+Filename: qtm_rt-3.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: qtm_rt-3.0.0.dist-info/top_level.txt
+Filename: qtm_rt-3.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: qtm_rt-3.0.0.dist-info/zip-safe
+Filename: qtm_rt-3.0.1.dist-info/zip-safe
 Comment: 
 
-Filename: qtm_rt-3.0.0.dist-info/RECORD
+Filename: qtm_rt-3.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qtm_rt/discovery.py

```diff
@@ -48,17 +48,21 @@
             return
 
         self.transport.sendto(
             QRTDiscoveryP1.pack(
                 QRTDiscoveryPacketSize, QRTPacketType.PacketDiscover.value
             )
             + QRTDiscoveryP2.pack(self.port),
-            ("<broadcast>", 22226),
+            ("255.255.255.255", 22226)
         )
 
+    def error_received(self, error):
+        """ On error """
+        LOG.exception("QRTDiscoveryProtocol %s", error)
+
 class Discover:
     """async discovery of qtm instances"""
 
     def __init__(self, ip_address):
         self.ip_address = ip_address
         self.queue = asyncio.Queue()
         self.first = True
```

## Comparing `qtm_rt-3.0.0.dist-info/LICENSE` & `qtm_rt-3.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `qtm_rt-3.0.0.dist-info/METADATA` & `qtm_rt-3.0.1.dist-info/METADATA`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,22 @@
-Metadata-Version: 2.1
-Name: qtm-rt
-Version: 3.0.0
-Summary: QTM Python SDK
-Home-page: https://github.com/qualisys/qualisys_python_sdk
-Author: Martin Gejke
-Author-email: support@qualisys.com
-License: MIT
-Download-URL: https://github.com/qualisys/qualisys_python_sdk/tarball/3.0.0
-Platform: UNKNOWN
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Utilities
-Requires-Python: >=3.5.3
-
-For older versions, see "qtm" package.
-
-
+Metadata-Version: 2.1
+Name: qtm-rt
+Version: 3.0.1
+Summary: QTM Python SDK
+Home-page: https://github.com/qualisys/qualisys_python_sdk
+Download-URL: https://github.com/qualisys/qualisys_python_sdk/tarball/3.0.1
+Author: Martin Gejke
+Author-email: support@qualisys.com
+License: MIT
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Utilities
+Requires-Python: >=3.5.3
+License-File: LICENSE
+
+For older versions, see "qtm" package.
```

## Comparing `qtm_rt-3.0.0.dist-info/RECORD` & `qtm_rt-3.0.1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 qtm_rt/__init__.py,sha256=jOVTUFmuvGc-O8YzCWEXMwMSO0yndPvEONvlFOz99k4,703
 qtm_rt/control.py,sha256=PTm4gje0XinVk1AMHL7XyxRumPjrcR3s9r0lfCxxEAY,677
-qtm_rt/discovery.py,sha256=IZr5KoqEVLGcA5j_7HaVLTWWocYYqLh8UeF__0pfJ8E,2994
+qtm_rt/discovery.py,sha256=k6Q5DKzg9ojNBgYPoDlyE62tPx_EKghh23F9N-BdVB4,3120
 qtm_rt/packet.py,sha256=kGYmKLR9T-oQPtt2DX8D2BMpoMDvAsWaNl1fHTkUywA,24141
 qtm_rt/protocol.py,sha256=j3GzuJIO43NcFSWAg4Pp1cSTmsQd3Fn7_ltkraJlKis,5985
 qtm_rt/qrt.py,sha256=wttyTnhySA_0At1OYYPFdNJwA2tIn5akunK9OfYnYxk,13639
 qtm_rt/reboot.py,sha256=I695niOpIN_rFoJiWNaPzhrTtteqX5MDl49CSgTt4dw,928
 qtm_rt/receiver.py,sha256=i1CFBIOLKXPPbE64VRdrWjYQ9nrxLOFK2Qb86J0i854,1570
 qtm_rt/data/demo.qtm,sha256=sYOMHapSu1WyN88VFiZup2t12AlR1ObR_gd_D7eNL4s,4259840
-qtm_rt-3.0.0.dist-info/LICENSE,sha256=kJwS4jkbWBWIO7Fa5CpKY-42ShVC2K-z9kDhOclXTQ4,1101
-qtm_rt-3.0.0.dist-info/METADATA,sha256=ZDmMfe3E3jcsbV-rc7rwv3620bsT6Krf5S0JH4WA1ms,773
-qtm_rt-3.0.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-qtm_rt-3.0.0.dist-info/top_level.txt,sha256=Z2enVWPFHgBc2CtZe2KvK1az3NA1-hqOEkT8ZEmKiF8,7
-qtm_rt-3.0.0.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-qtm_rt-3.0.0.dist-info/RECORD,,
+qtm_rt-3.0.1.dist-info/LICENSE,sha256=kJwS4jkbWBWIO7Fa5CpKY-42ShVC2K-z9kDhOclXTQ4,1101
+qtm_rt-3.0.1.dist-info/METADATA,sha256=r9webrvAXzWN_i0RBuwV4TJwg-o1kA9bTyELq6fsHMI,797
+qtm_rt-3.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+qtm_rt-3.0.1.dist-info/top_level.txt,sha256=Z2enVWPFHgBc2CtZe2KvK1az3NA1-hqOEkT8ZEmKiF8,7
+qtm_rt-3.0.1.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
+qtm_rt-3.0.1.dist-info/RECORD,,
```

