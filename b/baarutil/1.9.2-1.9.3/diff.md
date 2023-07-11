# Comparing `tmp/baarutil-1.9.2.tar.gz` & `tmp/baarutil-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\baarutil-1.9.2.tar", last modified: Wed Mar  8 15:06:57 2023, max compression
+gzip compressed data, was "dist\baarutil-1.9.3.tar", last modified: Tue Jul 11 10:02:49 2023, max compression
```

## Comparing `baarutil-1.9.2.tar` & `baarutil-1.9.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-03-08 15:06:57.000000 baarutil-1.9.2/
--rw-rw-rw-   0        0        0    23826 2023-03-08 15:06:57.000000 baarutil-1.9.2/PKG-INFO
--rw-rw-rw-   0        0        0    19211 2023-03-08 15:05:50.000000 baarutil-1.9.2/README.md
--rw-rw-rw-   0        0        0      108 2022-05-17 16:01:08.000000 baarutil-1.9.2/pyproject.toml
--rw-rw-rw-   0        0        0      904 2023-03-08 15:06:57.000000 baarutil-1.9.2/setup.cfg
--rw-rw-rw-   0        0        0     1177 2023-03-08 14:42:12.000000 baarutil-1.9.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:06:57.000000 baarutil-1.9.2/src/
-drwxrwxrwx   0        0        0        0 2023-03-08 15:06:57.000000 baarutil-1.9.2/src/baarutil/
--rw-rw-rw-   0        0        0       32 2022-11-04 10:25:03.000000 baarutil-1.9.2/src/baarutil/__init__.py
--rw-rw-rw-   0        0        0    11242 2023-03-08 14:02:35.000000 baarutil-1.9.2/src/baarutil/baarlocker.py
--rw-rw-rw-   0        0        0     2828 2023-03-08 14:09:20.000000 baarutil-1.9.2/src/baarutil/chromedriver_downloader.py
--rw-rw-rw-   0        0        0    29817 2023-03-08 15:00:57.000000 baarutil-1.9.2/src/baarutil/converter.py
-drwxrwxrwx   0        0        0        0 2023-03-08 15:06:57.000000 baarutil-1.9.2/src/baarutil.egg-info/
--rw-rw-rw-   0        0        0    23826 2023-03-08 15:06:57.000000 baarutil-1.9.2/src/baarutil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-03-08 15:06:57.000000 baarutil-1.9.2/src/baarutil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-08 15:06:57.000000 baarutil-1.9.2/src/baarutil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      154 2023-03-08 15:06:57.000000 baarutil-1.9.2/src/baarutil.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-08 15:06:57.000000 baarutil-1.9.2/src/baarutil.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 10:02:49.000000 baarutil-1.9.3/
+-rw-rw-rw-   0        0        0    24131 2023-07-11 10:02:49.000000 baarutil-1.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0    19458 2023-07-11 10:01:38.000000 baarutil-1.9.3/README.md
+-rw-rw-rw-   0        0        0      108 2022-05-17 16:01:08.000000 baarutil-1.9.3/pyproject.toml
+-rw-rw-rw-   0        0        0      866 2023-07-11 10:02:49.000000 baarutil-1.9.3/setup.cfg
+-rw-rw-rw-   0        0        0     1139 2023-07-11 09:55:49.000000 baarutil-1.9.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:02:47.000000 baarutil-1.9.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-11 10:02:49.000000 baarutil-1.9.3/src/baarutil/
+-rw-rw-rw-   0        0        0       32 2022-11-04 10:25:03.000000 baarutil-1.9.3/src/baarutil/__init__.py
+-rw-rw-rw-   0        0        0    11242 2023-03-08 14:02:35.000000 baarutil-1.9.3/src/baarutil/baarlocker.py
+-rw-rw-rw-   0        0        0     2828 2023-03-08 14:09:20.000000 baarutil-1.9.3/src/baarutil/chromedriver_downloader.py
+-rw-rw-rw-   0        0        0    30067 2023-07-11 09:41:40.000000 baarutil-1.9.3/src/baarutil/converter.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:02:49.000000 baarutil-1.9.3/src/baarutil.egg-info/
+-rw-rw-rw-   0        0        0    24131 2023-07-11 10:02:47.000000 baarutil-1.9.3/src/baarutil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-07-11 10:02:47.000000 baarutil-1.9.3/src/baarutil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 10:02:47.000000 baarutil-1.9.3/src/baarutil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      154 2023-07-11 10:02:47.000000 baarutil-1.9.3/src/baarutil.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-11 10:02:47.000000 baarutil-1.9.3/src/baarutil.egg-info/top_level.txt
```

### Comparing `baarutil-1.9.2/PKG-INFO` & `baarutil-1.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,40 @@
 Metadata-Version: 2.1
 Name: baarutil
-Version: 1.9.2
+Version: 1.9.3
 Summary: Utility functions for BAAR developers
 Home-page: https://github.com/Allied-Media/baarutil
-Author: Zhaoyu Xu, Souvik Roy
-Author-email: zhaoyu.xu@alliedmedia.com, souvik.roy@alliedmedia.com
+Author: Souvik Roy
+Author-email: souvik.roy@alliedmedia.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Allied-Media/baarutil/issues
 Description: # BAARUtil
         
-        **Version: 1.9.2**
+        **Version: 1.9.3**
+        
+        Minor Update - Contains bug fixes.
+        
+        Details: df_to_string() function now supports latest pandas versions (*i.e. pandas==2.0.3*)
         
         **This Custom Library is specifically created for the developers/users who use BAAR. Which is a product of [BAAR Technologies](https://www.baar.ai/) aka [Allied Media Inc](https://www.alliedmedia.com/).**
         
         <h2>
-        Authors:
+        Primary Author and Contributor:
         </h2>
         
         **Souvik Roy  [sroy-2019](https://github.com/sroy-2019)**
         
+        <h3>
+        Co-contributors:
+        </h3>
+        
+        **Saikat Dey**
+        **Debapriya Palai**
+        **Avignan Nag**
+        
         <h2>
         Installation:
         </h2>
         
         ~~~
         pip install baarutil
         ~~~
@@ -45,17 +57,17 @@
         ~~~
         
         <h2>
         Checking version:
         </h2>
         
         ~~~
-        import baarutil
+        import baarutil as bu
         
-        version = baarutil.version
+        version = bu.version()
         ~~~
         
         <h2>
         Table of Contents:
         </h2>
         
         1. [read_convert](#read_convert)
```

### Comparing `baarutil-1.9.2/README.md` & `baarutil-1.9.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,31 @@
 # BAARUtil
 
-**Version: 1.9.2**
+**Version: 1.9.3**
+
+Minor Update - Contains bug fixes.
+
+Details: df_to_string() function now supports latest pandas versions (*i.e. pandas==2.0.3*)
 
 **This Custom Library is specifically created for the developers/users who use BAAR. Which is a product of [BAAR Technologies](https://www.baar.ai/) aka [Allied Media Inc](https://www.alliedmedia.com/).**
 
 <h2>
-Authors:
+Primary Author and Contributor:
 </h2>
 
 **Souvik Roy  [sroy-2019](https://github.com/sroy-2019)**
 
+<h3>
+Co-contributors:
+</h3>
+
+**Saikat Dey**
+**Debapriya Palai**
+**Avignan Nag**
+
 <h2>
 Installation:
 </h2>
 
 ~~~
 pip install baarutil
 ~~~
@@ -36,17 +48,17 @@
 ~~~
 
 <h2>
 Checking version:
 </h2>
 
 ~~~
-import baarutil
+import baarutil as bu
 
-version = baarutil.version
+version = bu.version()
 ~~~
 
 <h2>
 Table of Contents:
 </h2>
 
 1. [read_convert](#read_convert)
```

#### html2text {}

```diff
@@ -1,23 +1,27 @@
-# BAARUtil **Version: 1.9.2** **This Custom Library is specifically created for
-the developers/users who use BAAR. Which is a product of [BAAR Technologies]
-(https://www.baar.ai/) aka [Allied Media Inc](https://www.alliedmedia.com/).**
-***** Authors: *****
+# BAARUtil **Version: 1.9.3** Minor Update - Contains bug fixes. Details:
+df_to_string() function now supports latest pandas versions (*i.e.
+pandas==2.0.3*) **This Custom Library is specifically created for the
+developers/users who use BAAR. Which is a product of [BAAR Technologies](https:
+//www.baar.ai/) aka [Allied Media Inc](https://www.alliedmedia.com/).**
+***** Primary Author and Contributor: *****
 **Souvik Roy [sroy-2019](https://github.com/sroy-2019)**
+**** Co-contributors: ****
+**Saikat Dey** **Debapriya Palai** **Avignan Nag**
 ***** Installation: *****
 ~~~ pip install baarutil ~~~
 ***** Importing: *****
 ~~~ import baarutil as bu ~~~
 ***** Additional Info: *****
 The string structure that follows is a streamlined structure that the
 developers/users follow throughout an automation workflow designed in BAAR: ~~~
 "Column_1__=__abc__$$__Column_2__=__def__::
 __Column_1__=__hello__$$__Column_2__=__world" ~~~
 ***** Checking version: *****
-~~~ import baarutil version = baarutil.version ~~~
+~~~ import baarutil as bu version = bu.version() ~~~
 ***** Table of Contents: *****
 1. [read_convert](#read_convert) 2. [write_convert](#write_convert) 3.
 [string_to_df](#string_to_df) 4. [df_to_string](#df_to_string) 5.
 [df_to_listdict](#df_to_listdict) 6. [decrypt_vault](#decrypt_vault) 7.
 [generate_password](#generate_password) 8. [generate_report](#generate_report)
 9. [string_to_report](#string_to_report) 10. [clean_directory]
 (#clean_directory) 11. [archive](#archive) 12. [download_chromedriver]
```

### Comparing `baarutil-1.9.2/setup.cfg` & `baarutil-1.9.3/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,55 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 6161 7275 7469 6c0d 0a76 6572   = baarutil..ver
-00000020: 7369 6f6e 203d 2031 2e39 2e32 0d0a 6175  sion = 1.9.2..au
-00000030: 7468 6f72 203d 205a 6861 6f79 7520 5875  thor = Zhaoyu Xu
-00000040: 2c20 536f 7576 696b 2052 6f79 0d0a 6175  , Souvik Roy..au
-00000050: 7468 6f72 5f65 6d61 696c 203d 207a 6861  thor_email = zha
-00000060: 6f79 752e 7875 4061 6c6c 6965 646d 6564  oyu.xu@alliedmed
-00000070: 6961 2e63 6f6d 2c20 736f 7576 696b 2e72  ia.com, souvik.r
-00000080: 6f79 4061 6c6c 6965 646d 6564 6961 2e63  oy@alliedmedia.c
-00000090: 6f6d 0d0a 6465 7363 7269 7074 696f 6e20  om..description 
-000000a0: 3d20 5574 696c 6974 7920 6675 6e63 7469  = Utility functi
-000000b0: 6f6e 7320 666f 7220 4241 4152 2064 6576  ons for BAAR dev
-000000c0: 656c 6f70 6572 730d 0a6c 6f6e 675f 6465  elopers..long_de
-000000d0: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
-000000e0: 3a20 5245 4144 4d45 2e6d 640d 0a6c 6f6e  : README.md..lon
-000000f0: 675f 6465 7363 7269 7074 696f 6e5f 636f  g_description_co
-00000100: 6e74 656e 745f 7479 7065 203d 2074 6578  ntent_type = tex
-00000110: 742f 6d61 726b 646f 776e 0d0a 7572 6c20  t/markdown..url 
-00000120: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
-00000130: 2e63 6f6d 2f41 6c6c 6965 642d 4d65 6469  .com/Allied-Medi
-00000140: 612f 6261 6172 7574 696c 0d0a 7072 6f6a  a/baarutil..proj
-00000150: 6563 745f 7572 6c73 203d 200d 0a09 4275  ect_urls = ...Bu
-00000160: 6720 5472 6163 6b65 7220 3d20 6874 7470  g Tracker = http
-00000170: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f41  s://github.com/A
-00000180: 6c6c 6965 642d 4d65 6469 612f 6261 6172  llied-Media/baar
-00000190: 7574 696c 2f69 7373 7565 730d 0a63 6c61  util/issues..cla
-000001a0: 7373 6966 6965 7273 203d 200d 0a09 5072  ssifiers = ...Pr
-000001b0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-000001c0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-000001d0: 332e 370d 0a09 4c69 6365 6e73 6520 3a3a  3.7...License ::
-000001e0: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
-000001f0: 204d 4954 204c 6963 656e 7365 0d0a 094f   MIT License...O
-00000200: 7065 7261 7469 6e67 2053 7973 7465 6d20  perating System 
-00000210: 3a3a 204f 5320 496e 6465 7065 6e64 656e  :: OS Independen
-00000220: 740d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  t....[options]..
-00000230: 7061 636b 6167 655f 6469 7220 3d20 0d0a  package_dir = ..
-00000240: 093d 2073 7263 0d0a 7061 636b 6167 6573  .= src..packages
-00000250: 203d 2066 696e 643a 0d0a 696e 7374 616c   = find:..instal
-00000260: 6c5f 7265 7175 6972 6573 203d 200d 0a09  l_requires = ...
-00000270: 6e75 6d70 793e 3d31 2e31 382e 340d 0a09  numpy>=1.18.4...
-00000280: 7061 6e64 6173 3e3d 312e 302e 330d 0a09  pandas>=1.0.3...
-00000290: 7079 6372 7970 746f 646f 6d65 3e3d 332e  pycryptodome>=3.
-000002a0: 390d 0a09 7079 6261 7365 3634 3d3d 312e  9...pybase64==1.
-000002b0: 322e 300d 0a09 6173 6e31 6372 7970 746f  2.0...asn1crypto
-000002c0: 3d3d 302e 3234 2e30 0d0a 0972 6f62 6f74  ==0.24.0...robot
-000002d0: 6672 616d 6577 6f72 6b2d 6372 7970 746f  framework-crypto
-000002e0: 3d3d 302e 332e 300d 0a09 7265 7175 6573  ==0.3.0...reques
-000002f0: 7473 3e3d 322e 3238 2e31 0d0a 0977 6765  ts>=2.28.1...wge
-00000300: 743e 3d33 2e32 0d0a 0972 6571 7565 7374  t>=3.2...request
-00000310: 733e 3d32 2e32 382e 310d 0a70 7974 686f  s>=2.28.1..pytho
-00000320: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
-00000330: 2e37 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  .7....[options.p
-00000340: 6163 6b61 6765 732e 6669 6e64 5d0d 0a77  ackages.find]..w
-00000350: 6865 7265 203d 2073 7263 0d0a 0d0a 5b65  here = src....[e
-00000360: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
-00000370: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
-00000380: 203d 2030 0d0a 0d0a                       = 0....
+00000020: 7369 6f6e 203d 2031 2e39 2e33 0d0a 6175  sion = 1.9.3..au
+00000030: 7468 6f72 203d 2053 6f75 7669 6b20 526f  thor = Souvik Ro
+00000040: 790d 0a61 7574 686f 725f 656d 6169 6c20  y..author_email 
+00000050: 3d20 736f 7576 696b 2e72 6f79 4061 6c6c  = souvik.roy@all
+00000060: 6965 646d 6564 6961 2e63 6f6d 0d0a 6465  iedmedia.com..de
+00000070: 7363 7269 7074 696f 6e20 3d20 5574 696c  scription = Util
+00000080: 6974 7920 6675 6e63 7469 6f6e 7320 666f  ity functions fo
+00000090: 7220 4241 4152 2064 6576 656c 6f70 6572  r BAAR developer
+000000a0: 730d 0a6c 6f6e 675f 6465 7363 7269 7074  s..long_descript
+000000b0: 696f 6e20 3d20 6669 6c65 3a20 5245 4144  ion = file: READ
+000000c0: 4d45 2e6d 640d 0a6c 6f6e 675f 6465 7363  ME.md..long_desc
+000000d0: 7269 7074 696f 6e5f 636f 6e74 656e 745f  ription_content_
+000000e0: 7479 7065 203d 2074 6578 742f 6d61 726b  type = text/mark
+000000f0: 646f 776e 0d0a 7572 6c20 3d20 6874 7470  down..url = http
+00000100: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f41  s://github.com/A
+00000110: 6c6c 6965 642d 4d65 6469 612f 6261 6172  llied-Media/baar
+00000120: 7574 696c 0d0a 7072 6f6a 6563 745f 7572  util..project_ur
+00000130: 6c73 203d 200d 0a09 4275 6720 5472 6163  ls = ...Bug Trac
+00000140: 6b65 7220 3d20 6874 7470 733a 2f2f 6769  ker = https://gi
+00000150: 7468 7562 2e63 6f6d 2f41 6c6c 6965 642d  thub.com/Allied-
+00000160: 4d65 6469 612f 6261 6172 7574 696c 2f69  Media/baarutil/i
+00000170: 7373 7565 730d 0a63 6c61 7373 6966 6965  ssues..classifie
+00000180: 7273 203d 200d 0a09 5072 6f67 7261 6d6d  rs = ...Programm
+00000190: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000001a0: 5079 7468 6f6e 203a 3a20 332e 370d 0a09  Python :: 3.7...
+000001b0: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
+000001c0: 7070 726f 7665 6420 3a3a 204d 4954 204c  pproved :: MIT L
+000001d0: 6963 656e 7365 0d0a 094f 7065 7261 7469  icense...Operati
+000001e0: 6e67 2053 7973 7465 6d20 3a3a 204f 5320  ng System :: OS 
+000001f0: 496e 6465 7065 6e64 656e 740d 0a0d 0a5b  Independent....[
+00000200: 6f70 7469 6f6e 735d 0d0a 7061 636b 6167  options]..packag
+00000210: 655f 6469 7220 3d20 0d0a 093d 2073 7263  e_dir = ...= src
+00000220: 0d0a 7061 636b 6167 6573 203d 2066 696e  ..packages = fin
+00000230: 643a 0d0a 696e 7374 616c 6c5f 7265 7175  d:..install_requ
+00000240: 6972 6573 203d 200d 0a09 6e75 6d70 793e  ires = ...numpy>
+00000250: 3d31 2e31 382e 340d 0a09 7061 6e64 6173  =1.18.4...pandas
+00000260: 3e3d 312e 302e 330d 0a09 7079 6372 7970  >=1.0.3...pycryp
+00000270: 746f 646f 6d65 3e3d 332e 390d 0a09 7079  todome>=3.9...py
+00000280: 6261 7365 3634 3d3d 312e 322e 300d 0a09  base64==1.2.0...
+00000290: 6173 6e31 6372 7970 746f 3d3d 302e 3234  asn1crypto==0.24
+000002a0: 2e30 0d0a 0972 6f62 6f74 6672 616d 6577  .0...robotframew
+000002b0: 6f72 6b2d 6372 7970 746f 3d3d 302e 332e  ork-crypto==0.3.
+000002c0: 300d 0a09 7265 7175 6573 7473 3e3d 322e  0...requests>=2.
+000002d0: 3238 2e31 0d0a 0977 6765 743e 3d33 2e32  28.1...wget>=3.2
+000002e0: 0d0a 0972 6571 7565 7374 733e 3d32 2e32  ...requests>=2.2
+000002f0: 382e 310d 0a70 7974 686f 6e5f 7265 7175  8.1..python_requ
+00000300: 6972 6573 203d 203e 3d33 2e37 0d0a 0d0a  ires = >=3.7....
+00000310: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
+00000320: 732e 6669 6e64 5d0d 0a77 6865 7265 203d  s.find]..where =
+00000330: 2073 7263 0d0a 0d0a 5b65 6767 5f69 6e66   src....[egg_inf
+00000340: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
+00000350: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
+00000360: 0d0a                                     ..
```

### Comparing `baarutil-1.9.2/setup.py` & `baarutil-1.9.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="baarutil",
-    version="1.9.2",
-    author="Zhaoyu Xu, Souvik Roy",
-    author_email="zhaoyu.xu@alliedmedia.com, souvik.roy@alliedmedia.com",
+    version="1.9.3",
+    author="Souvik Roy",
+    author_email="souvik.roy@alliedmedia.com",
     description="Utility functions for BAAR developers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Allied-Media/baarutil",
     project_urls={
         "Bug Tracker": "https://github.com/Allied-Media/baarutil/issues",
     },
```

### Comparing `baarutil-1.9.2/src/baarutil/baarlocker.py` & `baarutil-1.9.3/src/baarutil/baarlocker.py`

 * *Files identical despite different names*

### Comparing `baarutil-1.9.2/src/baarutil/chromedriver_downloader.py` & `baarutil-1.9.3/src/baarutil/chromedriver_downloader.py`

 * *Files identical despite different names*

### Comparing `baarutil-1.9.2/src/baarutil/converter.py` & `baarutil-1.9.3/src/baarutil/converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,19 @@
         if len(rename_cols) != 0:
             try:
                 input_df = input_df.rename(rename_cols, axis=1)
             except Exception as e:
                 print(traceback.format_exc(), flush=True)
         if drop_dupes:
             input_df = input_df.drop_duplicates()
-        for data_dict in input_df.to_dict('r'):
+        try:
+            input_records = input_df.to_dict('records')
+        except Exception as e:
+            input_records = input_df.to_dict('r')
+        for data_dict in input_records:
             for key in data_dict.keys():
                 final_string += str(key) + '__=__' + \
                     str(data_dict[key]) + '__$$__'
             final_string += '__::__'
     except Exception as e:
         print(traceback.format_exc(), flush=True)
     return final_string
@@ -132,15 +136,18 @@
         if len(rename_cols) != 0:
             try:
                 input_df = input_df.rename(rename_cols, axis=1)
             except Exception as e:
                 print(traceback.format_exc(), flush=True)
         if drop_dupes:
             input_df = input_df.drop_duplicates()
-        final_list = input_df.to_dict('r')
+        try:
+            final_list = input_df.to_dict('records')
+        except Exception as e:
+            final_list = input_df.to_dict('r')
     except Exception as e:
         print(traceback.format_exc(), flush=True)
     return final_list
 
 
 @keyword("Perform Base Decryption")
 def perform_base_decryption(encrypted_message: str, config_file: str = 'baarutil_config.json') -> str:
```

### Comparing `baarutil-1.9.2/src/baarutil.egg-info/PKG-INFO` & `baarutil-1.9.3/src/baarutil.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,40 @@
 Metadata-Version: 2.1
 Name: baarutil
-Version: 1.9.2
+Version: 1.9.3
 Summary: Utility functions for BAAR developers
 Home-page: https://github.com/Allied-Media/baarutil
-Author: Zhaoyu Xu, Souvik Roy
-Author-email: zhaoyu.xu@alliedmedia.com, souvik.roy@alliedmedia.com
+Author: Souvik Roy
+Author-email: souvik.roy@alliedmedia.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Allied-Media/baarutil/issues
 Description: # BAARUtil
         
-        **Version: 1.9.2**
+        **Version: 1.9.3**
+        
+        Minor Update - Contains bug fixes.
+        
+        Details: df_to_string() function now supports latest pandas versions (*i.e. pandas==2.0.3*)
         
         **This Custom Library is specifically created for the developers/users who use BAAR. Which is a product of [BAAR Technologies](https://www.baar.ai/) aka [Allied Media Inc](https://www.alliedmedia.com/).**
         
         <h2>
-        Authors:
+        Primary Author and Contributor:
         </h2>
         
         **Souvik Roy  [sroy-2019](https://github.com/sroy-2019)**
         
+        <h3>
+        Co-contributors:
+        </h3>
+        
+        **Saikat Dey**
+        **Debapriya Palai**
+        **Avignan Nag**
+        
         <h2>
         Installation:
         </h2>
         
         ~~~
         pip install baarutil
         ~~~
@@ -45,17 +57,17 @@
         ~~~
         
         <h2>
         Checking version:
         </h2>
         
         ~~~
-        import baarutil
+        import baarutil as bu
         
-        version = baarutil.version
+        version = bu.version()
         ~~~
         
         <h2>
         Table of Contents:
         </h2>
         
         1. [read_convert](#read_convert)
```

