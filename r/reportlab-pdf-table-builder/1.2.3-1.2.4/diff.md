# Comparing `tmp/reportlab-pdf-table-builder-1.2.3.tar.gz` & `tmp/reportlab-pdf-table-builder-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reportlab-pdf-table-builder-1.2.3.tar", last modified: Tue Jul  4 08:07:08 2023, max compression
+gzip compressed data, was "reportlab-pdf-table-builder-1.2.4.tar", last modified: Tue Jul 11 14:11:51 2023, max compression
```

## Comparing `reportlab-pdf-table-builder-1.2.3.tar` & `reportlab-pdf-table-builder-1.2.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 08:07:08.101185 reportlab-pdf-table-builder-1.2.3/
--rw-rw-rw-   0        0        0     1091 2022-07-14 09:41:45.000000 reportlab-pdf-table-builder-1.2.3/LICENSE
--rw-rw-rw-   0        0        0       39 2022-07-14 09:41:45.000000 reportlab-pdf-table-builder-1.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3274 2023-07-04 08:07:08.101185 reportlab-pdf-table-builder-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     2717 2023-07-04 08:02:39.000000 reportlab-pdf-table-builder-1.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-04 08:07:08.080257 reportlab-pdf-table-builder-1.2.3/pdf_table_builder/
--rw-rw-rw-   0        0        0        0 2022-07-14 09:41:45.000000 reportlab-pdf-table-builder-1.2.3/pdf_table_builder/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 08:07:08.090157 reportlab-pdf-table-builder-1.2.3/pdf_table_builder/__pycache__/
--rw-rw-rw-   0        0        0      204 2022-07-14 10:06:18.000000 reportlab-pdf-table-builder-1.2.3/pdf_table_builder/__pycache__/__init__.cpython-38.pyc
--rw-rw-rw-   0        0        0      225 2023-07-04 07:09:43.000000 reportlab-pdf-table-builder-1.2.3/pdf_table_builder/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     8532 2022-10-11 13:50:30.000000 reportlab-pdf-table-builder-1.2.3/pdf_table_builder/__pycache__/builder.cpython-38.pyc
--rw-rw-rw-   0        0        0     8555 2023-07-04 07:09:43.000000 reportlab-pdf-table-builder-1.2.3/pdf_table_builder/__pycache__/builder.cpython-39.pyc
--rw-rw-rw-   0        0        0      561 2022-07-25 14:50:28.000000 reportlab-pdf-table-builder-1.2.3/pdf_table_builder/__pycache__/helpers.cpython-38.pyc
--rw-rw-rw-   0        0        0      582 2023-07-04 07:09:43.000000 reportlab-pdf-table-builder-1.2.3/pdf_table_builder/__pycache__/helpers.cpython-39.pyc
--rw-rw-rw-   0        0        0    12302 2022-10-11 13:50:27.000000 reportlab-pdf-table-builder-1.2.3/pdf_table_builder/builder.py
--rw-rw-rw-   0        0        0      710 2022-07-14 09:41:45.000000 reportlab-pdf-table-builder-1.2.3/pdf_table_builder/consts.py
-drwxrwxrwx   0        0        0        0 2023-07-04 08:07:08.093226 reportlab-pdf-table-builder-1.2.3/pdf_table_builder/fonts/
--rw-rw-rw-   0        0        0   455164 2022-07-14 09:41:45.000000 reportlab-pdf-table-builder-1.2.3/pdf_table_builder/fonts/NotoSans-Bold.ttf
--rw-rw-rw-   0        0        0   455188 2022-07-14 09:41:45.000000 reportlab-pdf-table-builder-1.2.3/pdf_table_builder/fonts/NotoSans-Regular.ttf
--rw-rw-rw-   0        0        0     1000 2022-07-25 14:50:28.000000 reportlab-pdf-table-builder-1.2.3/pdf_table_builder/helpers.py
-drwxrwxrwx   0        0        0        0 2023-07-04 08:07:08.094759 reportlab-pdf-table-builder-1.2.3/pdf_table_builder/utils/
--rw-rw-rw-   0        0        0     1388 2022-07-14 09:41:45.000000 reportlab-pdf-table-builder-1.2.3/pdf_table_builder/utils/helpers.py
-drwxrwxrwx   0        0        0        0 2023-07-04 08:07:08.100188 reportlab-pdf-table-builder-1.2.3/reportlab_pdf_table_builder.egg-info/
--rw-rw-rw-   0        0        0     3274 2023-07-04 08:07:08.000000 reportlab-pdf-table-builder-1.2.3/reportlab_pdf_table_builder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      850 2023-07-04 08:07:08.000000 reportlab-pdf-table-builder-1.2.3/reportlab_pdf_table_builder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 08:07:08.000000 reportlab-pdf-table-builder-1.2.3/reportlab_pdf_table_builder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-07-04 08:07:08.000000 reportlab-pdf-table-builder-1.2.3/reportlab_pdf_table_builder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-07-04 08:07:08.000000 reportlab-pdf-table-builder-1.2.3/reportlab_pdf_table_builder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-04 08:07:08.101185 reportlab-pdf-table-builder-1.2.3/setup.cfg
--rw-rw-rw-   0        0        0      857 2023-07-04 08:06:38.000000 reportlab-pdf-table-builder-1.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 14:11:51.694649 reportlab-pdf-table-builder-1.2.4/
+-rw-rw-rw-   0        0        0     1091 2022-07-14 09:41:45.000000 reportlab-pdf-table-builder-1.2.4/LICENSE
+-rw-rw-rw-   0        0        0       39 2022-07-14 09:41:45.000000 reportlab-pdf-table-builder-1.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3233 2023-07-11 14:11:51.693650 reportlab-pdf-table-builder-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2717 2023-07-04 08:02:39.000000 reportlab-pdf-table-builder-1.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 14:11:51.662742 reportlab-pdf-table-builder-1.2.4/pdf_table_builder/
+-rw-rw-rw-   0        0        0        0 2022-07-14 09:41:45.000000 reportlab-pdf-table-builder-1.2.4/pdf_table_builder/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 14:11:51.677693 reportlab-pdf-table-builder-1.2.4/pdf_table_builder/__pycache__/
+-rw-rw-rw-   0        0        0      204 2022-07-14 10:06:18.000000 reportlab-pdf-table-builder-1.2.4/pdf_table_builder/__pycache__/__init__.cpython-38.pyc
+-rw-rw-rw-   0        0        0      225 2023-07-04 07:09:43.000000 reportlab-pdf-table-builder-1.2.4/pdf_table_builder/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     8532 2022-10-11 13:50:30.000000 reportlab-pdf-table-builder-1.2.4/pdf_table_builder/__pycache__/builder.cpython-38.pyc
+-rw-rw-rw-   0        0        0     9651 2023-07-11 12:29:55.000000 reportlab-pdf-table-builder-1.2.4/pdf_table_builder/__pycache__/builder.cpython-39.pyc
+-rw-rw-rw-   0        0        0      561 2022-07-25 14:50:28.000000 reportlab-pdf-table-builder-1.2.4/pdf_table_builder/__pycache__/helpers.cpython-38.pyc
+-rw-rw-rw-   0        0        0      582 2023-07-04 07:09:43.000000 reportlab-pdf-table-builder-1.2.4/pdf_table_builder/__pycache__/helpers.cpython-39.pyc
+-rw-rw-rw-   0        0        0    14530 2023-07-11 12:29:04.000000 reportlab-pdf-table-builder-1.2.4/pdf_table_builder/builder.py
+-rw-rw-rw-   0        0        0      710 2022-07-14 09:41:45.000000 reportlab-pdf-table-builder-1.2.4/pdf_table_builder/consts.py
+drwxrwxrwx   0        0        0        0 2023-07-11 14:11:51.682712 reportlab-pdf-table-builder-1.2.4/pdf_table_builder/fonts/
+-rw-rw-rw-   0        0        0   455164 2022-07-14 09:41:45.000000 reportlab-pdf-table-builder-1.2.4/pdf_table_builder/fonts/NotoSans-Bold.ttf
+-rw-rw-rw-   0        0        0   455188 2022-07-14 09:41:45.000000 reportlab-pdf-table-builder-1.2.4/pdf_table_builder/fonts/NotoSans-Regular.ttf
+-rw-rw-rw-   0        0        0     1000 2022-07-25 14:50:28.000000 reportlab-pdf-table-builder-1.2.4/pdf_table_builder/helpers.py
+drwxrwxrwx   0        0        0        0 2023-07-11 14:11:51.684674 reportlab-pdf-table-builder-1.2.4/pdf_table_builder/utils/
+-rw-rw-rw-   0        0        0     1388 2022-07-14 09:41:45.000000 reportlab-pdf-table-builder-1.2.4/pdf_table_builder/utils/helpers.py
+drwxrwxrwx   0        0        0        0 2023-07-11 14:11:51.692654 reportlab-pdf-table-builder-1.2.4/reportlab_pdf_table_builder.egg-info/
+-rw-rw-rw-   0        0        0     3233 2023-07-11 14:11:51.000000 reportlab-pdf-table-builder-1.2.4/reportlab_pdf_table_builder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      850 2023-07-11 14:11:51.000000 reportlab-pdf-table-builder-1.2.4/reportlab_pdf_table_builder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 14:11:51.000000 reportlab-pdf-table-builder-1.2.4/reportlab_pdf_table_builder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-07-11 14:11:51.000000 reportlab-pdf-table-builder-1.2.4/reportlab_pdf_table_builder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-11 14:11:51.000000 reportlab-pdf-table-builder-1.2.4/reportlab_pdf_table_builder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 14:11:51.694649 reportlab-pdf-table-builder-1.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      857 2023-07-11 14:11:42.000000 reportlab-pdf-table-builder-1.2.4/setup.py
```

### Comparing `reportlab-pdf-table-builder-1.2.3/LICENSE` & `reportlab-pdf-table-builder-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `reportlab-pdf-table-builder-1.2.3/PKG-INFO` & `reportlab-pdf-table-builder-1.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: reportlab-pdf-table-builder
-Version: 1.2.3
+Version: 1.2.4
 Summary: A simple pdf table builder using the ReportLab Toolkit
 Home-page: https://github.com/timossavva/reportlab-pdf-table-builder
 Author: Timotheos Savva
 Author-email: timotheos.savva12@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -84,9 +82,7 @@
 
 table = pfd_table_builder(data)
 
 pdfbuilder = ReportLabPDFBuilder()
 pdfbuilder.add_to_story(table)
 pdfbuilder.save_pdf_file('a.pdf')
 ```
-
-
```

### Comparing `reportlab-pdf-table-builder-1.2.3/README.md` & `reportlab-pdf-table-builder-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `reportlab-pdf-table-builder-1.2.3/pdf_table_builder/__pycache__/builder.cpython-38.pyc` & `reportlab-pdf-table-builder-1.2.4/pdf_table_builder/__pycache__/builder.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `reportlab-pdf-table-builder-1.2.3/pdf_table_builder/__pycache__/builder.cpython-39.pyc` & `reportlab-pdf-table-builder-1.2.4/pdf_table_builder/__pycache__/builder.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Oct 11 13:50:27 2022 UTC, .py size: 12302 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-00000000: 610d 0d0a 0000 0000 a374 4563 0e30 0000  a........tEc.0..
+00000000: 610d 0d0a 0000 0000 104b ad64 c238 0000  a........K.d.8..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0008 0000 0040 0000 0073 c401 0000 6400  .....@...s....d.
+00000020: 0008 0000 0040 0000 0073 cc01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c00  d.l.m.Z...d.d.l.
 00000050: 6d04 5a04 0100 6400 6404 6c05 6d06 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c08 6d09 5a09 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6406 6c0a 6d0b 5a0b 0100 6400 6407 6c0c  d.l.m.Z...d.d.l.
 00000080: 6d0d 5a0d 0100 6400 6408 6c0e 6d0f 5a0f  m.Z...d.d.l.m.Z.
 00000090: 0100 6400 6409 6c10 6d11 5a11 0100 6400  ..d.d.l.m.Z...d.
@@ -13,523 +13,592 @@
 000000c0: 6d06 5a06 0100 6400 640d 6c16 6d18 5a18  m.Z...d.d.l.m.Z.
 000000d0: 6d19 5a19 0100 6400 640e 6c16 6d1a 5a1a  m.Z...d.d.l.m.Z.
 000000e0: 6d1b 5a1b 6d1c 5a1c 0100 6400 640f 6c1d  m.Z.m.Z...d.d.l.
 000000f0: 6d1e 5a1e 0100 650f 8300 5a1f 651f 6410  m.Z...e...Z.e.d.
 00000100: 1900 5a20 651f 6411 1900 5a21 650d 6400  ..Z e.d...Z!e.d.
 00000110: 1900 6412 1800 5a22 650d 6413 1900 6414  ..d...Z"e.d...d.
 00000120: 1b00 6415 1800 5a23 6416 5a24 6417 5a25  ..d...Z#d.Z$d.Z%
-00000130: 6418 5a26 6419 5a27 641a 5a28 6416 5a29  d.Z&d.Z'd.Z(d.Z)
-00000140: 6416 5a2a 6401 612b 6401 612c 641b 612d  d.Z*d.a+d.a,d.a-
-00000150: 641c 612e 6501 6a2f a030 6501 6a2f a031  d.a.e.j/.0e.j/.1
-00000160: 6501 a032 a100 6501 6a2f a033 6534 a101  e..2..e.j/.3e4..
-00000170: a102 a101 5a35 4700 641d 641e 8400 641e  ....Z5G.d.d...d.
-00000180: 8302 5a36 4700 641f 6420 8400 6420 8302  ..Z6G.d.d ..d ..
-00000190: 5a37 4700 6421 6422 8400 6422 8302 5a38  Z7G.d!d"..d"..Z8
-000001a0: 4700 6423 6424 8400 6424 8302 5a39 4700  G.d#d$..d$..Z9G.
-000001b0: 6425 6426 8400 6426 8302 5a3a 6427 6428  d%d&..d&..Z:d'd(
-000001c0: 8400 5a3b 6433 6429 642a 8401 5a3c 642b  ..Z;d3d)d*..Z<d+
-000001d0: 642c 8400 5a3d 642d 642e 8400 5a3e 642f  d,..Z=d-d...Z>d/
-000001e0: 6430 8400 5a3f 6431 6432 8400 5a40 6401  d0..Z?d1d2..Z@d.
-000001f0: 5300 2934 e900 0000 004e 2901 da07 7061  S.)4.....N)...pa
-00000200: 7274 6961 6c29 01da 0742 7974 6573 494f  rtial)...BytesIO
-00000210: 2901 da05 496d 6167 6529 01da 0663 6f6c  )...Image)...col
-00000220: 6f72 7329 01da 0754 415f 4c45 4654 2901  ors)...TA_LEFT).
-00000230: da02 4134 2901 da13 6765 7453 616d 706c  ..A4)...getSampl
-00000240: 6553 7479 6c65 5368 6565 7429 01da 0b49  eStyleSheet)...I
-00000250: 6d61 6765 5265 6164 6572 2901 da0a 7064  mageReader)...pd
-00000260: 666d 6574 7269 6373 2901 da06 5454 466f  fmetrics)...TTFo
-00000270: 6e74 2902 da0f 4261 7365 446f 6354 656d  nt)...BaseDocTem
-00000280: 706c 6174 6572 0400 0000 2902 da05 4672  plater....)...Fr
-00000290: 616d 65da 0c50 6167 6554 656d 706c 6174  ame..PageTemplat
-000002a0: 6529 03da 0950 6172 6167 7261 7068 da05  e)...Paragraph..
-000002b0: 5461 626c 65da 0a54 6162 6c65 5374 796c  Table..TableStyl
-000002c0: 6529 01da 3063 616c 6375 6c61 7465 5f69  e)..0calculate_i
-000002d0: 6d61 6765 5f64 696d 656e 7369 6f6e 735f  mage_dimensions_
-000002e0: 616e 645f 6b65 6570 5f61 7370 6563 745f  and_keep_aspect_
-000002f0: 7261 7469 6fda 064e 6f72 6d61 6cda 0848  ratio..Normal..H
-00000300: 6561 6469 6e67 31e9 a000 0000 e901 0000  eading1.........
-00000310: 00e9 0200 0000 e9aa 0000 00e9 1e00 0000  ................
-00000320: e908 0000 0069 1202 0000 69ee 0200 0069  .....i....i....i
-00000330: da02 0000 e9b4 0000 007a 0d50 4446 2054  .........z.PDF T
-00000340: 6162 2054 6974 6c65 6300 0000 0000 0000  ab Titlec.......
-00000350: 0000 0000 0000 0000 000a 0000 0040 0000  .............@..
-00000360: 0073 4200 0000 6500 5a01 6400 5a02 6401  .sB...e.Z.d.Z.d.
-00000370: 6401 6503 6504 6402 6402 6403 6403 6403  d.e.e.d.d.d.d.d.
-00000380: 6403 660a 6404 6405 8401 5a05 6406 6407  d.f.d.d...Z.d.d.
-00000390: 8400 5a06 6408 6409 8400 5a07 640a 640b  ..Z.d.d...Z.d.d.
-000003a0: 8400 5a08 6401 5300 290c da13 5265 706f  ..Z.d.S.)...Repo
-000003b0: 7274 4c61 6250 4446 4275 696c 6465 724e  rtLabPDFBuilderN
-000003c0: 7201 0000 0072 1900 0000 630b 0000 0000  r....r....c.....
-000003d0: 0000 0000 0000 000e 0000 000a 0000 0043  ...............C
-000003e0: 0000 0073 7800 0000 7c01 6100 7c02 6101  ...sx...|.a.|.a.
-000003f0: 7402 8300 6103 7c03 6104 7c04 6105 7406  t...a.|.a.|.a.t.
-00000400: 8300 7c00 5f07 7408 7c00 6a07 7409 6401  ..|._.t.|.j.t.d.
-00000410: 8d02 7c00 5f0a 740b 740c 740d 740e 740f  ..|._.t.t.t.t.t.
-00000420: 7c07 7c0a 7c08 7c09 6402 8d08 7d0b 7410  |.|.|.|.d...}.t.
-00000430: 7411 7c05 7c06 8303 7d0c 7412 6403 7c0b  t.|.|...}.t.d.|.
-00000440: 7c0c 6404 8d03 7d0d 7c00 6a0a a013 7c0d  |.d...}.|.j...|.
-00000450: 6701 a101 0100 6700 7c00 5f14 6400 5300  g.....g.|._.d.S.
-00000460: 2905 4e29 01da 0870 6167 6573 697a 6529  ).N)...pagesize)
-00000470: 06da 0577 6964 7468 da06 6865 6967 6874  ...width..height
-00000480: da0b 6c65 6674 5061 6464 696e 67da 0d62  ..leftPadding..b
-00000490: 6f74 746f 6d50 6164 6469 6e67 da0c 7269  ottomPadding..ri
-000004a0: 6768 7450 6164 6469 6e67 da0a 746f 7050  ghtPadding..topP
-000004b0: 6164 6469 6e67 5a09 616c 6c5f 7061 6765  addingZ.all_page
-000004c0: 7329 03da 0269 64da 0666 7261 6d65 73da  s)...id..frames.
-000004d0: 066f 6e50 6167 6529 15da 094c 4f47 4f5f  .onPage)...LOGO_
-000004e0: 5041 5448 da09 5741 5445 524d 4152 4bda  PATH..WATERMARK.
-000004f0: 0e67 6574 5f62 6f64 795f 7374 796c 655a  .get_body_styleZ
-00000500: 0a42 4f44 595f 5354 594c 45da 0d50 4446  .BODY_STYLE..PDF
-00000510: 5f54 4142 5f54 4954 4c45 da0f 4c4f 474f  _TAB_TITLE..LOGO
-00000520: 5f42 4153 455f 5749 4454 4872 0300 0000  _BASE_WIDTHr....
-00000530: da0a 7064 665f 6275 6666 6572 720c 0000  ..pdf_bufferr...
-00000540: 0072 0700 0000 da03 7064 6672 0d00 0000  .r......pdfr....
-00000550: da08 4652 414d 455f 5831 da08 4652 414d  ..FRAME_X1..FRAM
-00000560: 455f 5931 da0a 5041 4745 5f57 4944 5448  E_Y1..PAGE_WIDTH
-00000570: da0b 5041 4745 5f48 4549 4748 5472 0200  ..PAGE_HEIGHTr..
-00000580: 0000 da11 6865 6164 6572 5f61 6e64 5f66  ....header_and_f
-00000590: 6f6f 7465 7272 0e00 0000 da10 6164 6450  ooterr......addP
-000005a0: 6167 6554 656d 706c 6174 6573 da05 7374  ageTemplates..st
-000005b0: 6f72 7929 0eda 0473 656c 665a 096c 6f67  ory)...selfZ.log
-000005c0: 6f5f 7061 7468 5a09 7761 7465 726d 6172  o_pathZ.watermar
-000005d0: 6b5a 0d70 6466 5f74 6162 5f74 6974 6c65  kZ.pdf_tab_title
-000005e0: 5a0f 6c6f 676f 5f62 6173 655f 7769 6474  Z.logo_base_widt
-000005f0: 68da 0d6c 6f67 6f5f 6361 6e76 6173 5f78  h..logo_canvas_x
-00000600: da0d 6c6f 676f 5f63 616e 7661 735f 795a  ..logo_canvas_yZ
-00000610: 1266 7261 6d65 5f6c 6566 745f 7061 6464  .frame_left_padd
-00000620: 696e 675a 1366 7261 6d65 5f72 6967 6874  ingZ.frame_right
-00000630: 5f70 6164 6469 6e67 5a11 6672 616d 655f  _paddingZ.frame_
-00000640: 746f 705f 7061 6464 696e 675a 1466 7261  top_paddingZ.fra
-00000650: 6d65 5f62 6f74 746f 6d5f 7061 6464 696e  me_bottom_paddin
-00000660: 67da 0566 7261 6d65 5a19 6865 6164 6572  g..frameZ.header
-00000670: 5f61 6e64 5f66 6f6f 7465 725f 7061 7274  _and_footer_part
-00000680: 6961 6cda 0874 656d 706c 6174 65a9 0072  ial..template..r
-00000690: 3a00 0000 fa85 433a 5c55 7365 7273 5c4c  :.....C:\Users\L
-000006a0: 6976 655c 446f 6375 6d65 6e74 735c 5072  ive\Documents\Pr
-000006b0: 6f6a 6563 7473 5c50 726f 6772 616d 6d69  ojects\Programmi
-000006c0: 6e67 5c4d 4353 202d 2050 6572 736f 6e61  ng\MCS - Persona
-000006d0: 6c5c 5079 7468 6f6e 5c23 5061 636b 6167  l\Python\#Packag
-000006e0: 6573 5c72 6570 6f72 746c 6162 2d70 6466  es\reportlab-pdf
-000006f0: 2d74 6162 6c65 2d62 7569 6c64 6572 5c70  -table-builder\p
-00000700: 6466 5f74 6162 6c65 5f62 7569 6c64 6572  df_table_builder
-00000710: 5c62 7569 6c64 6572 2e70 79da 085f 5f69  \builder.py..__i
-00000720: 6e69 745f 5f2d 0000 0073 2a00 0000 0009  nit__-...s*.....
-00000730: 0401 0401 0601 0401 0402 0801 1001 0201  ................
-00000740: 0201 0201 0201 0201 0201 0201 0201 02f8  ................
-00000750: 060a 0c01 0e01 0e01 7a1c 5265 706f 7274  ........z.Report
-00000760: 4c61 6250 4446 4275 696c 6465 722e 5f5f  LabPDFBuilder.__
-00000770: 696e 6974 5f5f 6302 0000 0000 0000 0000  init__c.........
-00000780: 0000 0003 0000 0004 0000 0043 0000 0073  ...........C...s
-00000790: 3200 0000 7400 7c01 7401 8302 7222 7c01  2...t.|.t...r"|.
-000007a0: 4400 5d10 7d02 7c00 6a02 a003 7c02 a101  D.].}.|.j...|...
-000007b0: 0100 710e 6e0c 7c00 6a02 a003 7c01 a101  ..q.n.|.j...|...
-000007c0: 0100 6400 5300 a901 4e29 04da 0a69 7369  ..d.S...N)...isi
-000007d0: 6e73 7461 6e63 65da 046c 6973 7472 3400  nstance..listr4.
-000007e0: 0000 da06 6170 7065 6e64 2903 7235 0000  ....append).r5..
-000007f0: 00da 036f 626a da01 7872 3a00 0000 723a  ...obj..xr:...r:
-00000800: 0000 0072 3b00 0000 da0c 6164 645f 746f  ...r;.....add_to
-00000810: 5f73 746f 7279 4d00 0000 7308 0000 0000  _storyM...s.....
-00000820: 010a 0108 0110 027a 2052 6570 6f72 744c  .......z ReportL
-00000830: 6162 5044 4642 7569 6c64 6572 2e61 6464  abPDFBuilder.add
-00000840: 5f74 6f5f 7374 6f72 7963 0100 0000 0000  _to_storyc......
-00000850: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
-00000860: 0000 7326 0000 007c 006a 00a0 017c 006a  ..s&...|.j...|.j
-00000870: 02a1 0101 007c 006a 03a0 04a1 007d 017c  .....|.j.....}.|
-00000880: 006a 03a0 05a1 0001 007c 0153 0072 3d00  .j.......|.S.r=.
-00000890: 0000 2906 722d 0000 00da 0562 7569 6c64  ..).r-.....build
-000008a0: 7234 0000 0072 2c00 0000 da08 6765 7476  r4...r,.....getv
-000008b0: 616c 7565 da05 636c 6f73 6529 0272 3500  alue..close).r5.
-000008c0: 0000 5a09 7064 665f 7661 6c75 6572 3a00  ..Z.pdf_valuer:.
-000008d0: 0000 723a 0000 0072 3b00 0000 da0d 6765  ..r:...r;.....ge
-000008e0: 745f 7064 665f 7661 6c75 6554 0000 0073  t_pdf_valueT...s
-000008f0: 0800 0000 0001 0e01 0a01 0a01 7a21 5265  ............z!Re
-00000900: 706f 7274 4c61 6250 4446 4275 696c 6465  portLabPDFBuilde
-00000910: 722e 6765 745f 7064 665f 7661 6c75 6563  r.get_pdf_valuec
-00000920: 0200 0000 0000 0000 0000 0000 0300 0000  ................
-00000930: 0800 0000 4300 0000 7356 0000 007c 006a  ....C...sV...|.j
-00000940: 00a0 017c 006a 02a1 0101 0074 037c 0164  ...|.j.....t.|.d
-00000950: 0183 028f 2a7d 027c 006a 04a0 0574 066a  ....*}.|.j...t.j
-00000960: 07a1 0101 007c 02a0 087c 006a 04a1 0101  .....|...|.j....
-00000970: 0057 0064 0004 0004 0083 0301 006e 1031  .W.d.........n.1
-00000980: 0073 4830 0001 0001 0001 0059 0001 0064  .sH0.......Y...d
-00000990: 0053 0029 024e da02 7762 2909 722d 0000  .S.).N..wb).r-..
-000009a0: 0072 4400 0000 7234 0000 00da 046f 7065  .rD...r4.....ope
-000009b0: 6e72 2c00 0000 da04 7365 656b da02 696f  nr,.....seek..io
-000009c0: da08 5345 454b 5f53 4554 da0a 7772 6974  ..SEEK_SET..writ
-000009d0: 656c 696e 6573 2903 7235 0000 00da 0966  elines).r5.....f
-000009e0: 696c 655f 6e61 6d65 da01 6672 3a00 0000  ile_name..fr:...
-000009f0: 723a 0000 0072 3b00 0000 da0d 7361 7665  r:...r;.....save
-00000a00: 5f70 6466 5f66 696c 655a 0000 0073 0800  _pdf_fileZ...s..
-00000a10: 0000 0001 0e01 0c01 0e01 7a21 5265 706f  ..........z!Repo
-00000a20: 7274 4c61 6250 4446 4275 696c 6465 722e  rtLabPDFBuilder.
-00000a30: 7361 7665 5f70 6466 5f66 696c 6529 09da  save_pdf_file)..
-00000a40: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-00000a50: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-00000a60: 655f 5f72 2a00 0000 722b 0000 0072 3c00  e__r*...r+...r<.
-00000a70: 0000 7243 0000 0072 4700 0000 7250 0000  ..rC...rG...rP..
-00000a80: 0072 3a00 0000 723a 0000 0072 3a00 0000  .r:...r:...r:...
-00000a90: 723b 0000 0072 1c00 0000 2b00 0000 730e  r;...r....+...s.
-00000aa0: 0000 0008 0208 010a 0102 fe0a 2008 0708  ............ ...
-00000ab0: 0672 1c00 0000 6300 0000 0000 0000 0000  .r....c.........
-00000ac0: 0000 0000 0000 0007 0000 0040 0000 0073  ...........@...s
-00000ad0: 2c00 0000 6500 5a01 6400 5a02 6401 6401  ,...e.Z.d.Z.d.d.
-00000ae0: 6401 6401 6402 6503 6401 6607 6403 6404  d.d.d.e.d.f.d.d.
-00000af0: 8401 5a04 6405 6406 8400 5a05 6401 5300  ..Z.d.d...Z.d.S.
-00000b00: 2907 da03 526f 774e 4663 0900 0000 0000  )...RowNFc......
-00000b10: 0000 0000 0000 0900 0000 0200 0000 4300  ..............C.
-00000b20: 0000 7334 0000 007c 017c 005f 007c 027c  ..s4...|.|._.|.|
-00000b30: 005f 017c 037c 005f 027c 047c 005f 037c  ._.|.|._.|.|._.|
-00000b40: 057c 005f 047c 077c 005f 057c 067c 005f  .|._.|.|._.|.|._
-00000b50: 067c 087c 005f 0764 0053 0072 3d00 0000  .|.|._.d.S.r=...
-00000b60: 2908 da07 636f 6c75 6d6e 73da 046c 696e  )...columns..lin
-00000b70: 65da 0467 7269 64da 1062 6163 6b67 726f  e..grid..backgro
-00000b80: 756e 645f 636f 6c6f 72da 0a74 6578 745f  und_color..text_
-00000b90: 636f 6c6f 72da 0561 6c69 676e da0a 6675  color..align..fu
-00000ba0: 6c6c 5f77 6964 7468 da06 7661 6c69 676e  ll_width..valign
-00000bb0: 2909 7235 0000 0072 5500 0000 7256 0000  ).r5...rU...rV..
-00000bc0: 0072 5700 0000 7258 0000 0072 5900 0000  .rW...rX...rY...
-00000bd0: 725b 0000 0072 5a00 0000 725c 0000 0072  r[...rZ...r\...r
-00000be0: 3a00 0000 723a 0000 0072 3b00 0000 723c  :...r:...r;...r<
-00000bf0: 0000 0062 0000 0073 1000 0000 0002 0601  ...b...s........
-00000c00: 0601 0601 0601 0601 0601 0601 7a0c 526f  ............z.Ro
-00000c10: 772e 5f5f 696e 6974 5f5f 6301 0000 0000  w.__init__c.....
-00000c20: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
-00000c30: 0000 0073 0a00 0000 7400 7c00 6a01 8301  ...s....t.|.j...
-00000c40: 5300 723d 0000 0029 02da 036c 656e 7255  S.r=...)...lenrU
-00000c50: 0000 0029 0172 3500 0000 723a 0000 0072  ...).r5...r:...r
-00000c60: 3a00 0000 723b 0000 00da 1567 6574 5f6e  :...r;.....get_n
-00000c70: 756d 6265 725f 6f66 5f63 6f6c 756d 6e73  umber_of_columns
-00000c80: 6d00 0000 7302 0000 0000 017a 1952 6f77  m...s......z.Row
-00000c90: 2e67 6574 5f6e 756d 6265 725f 6f66 5f63  .get_number_of_c
-00000ca0: 6f6c 756d 6e73 2906 7251 0000 0072 5200  olumns).rQ...rR.
-00000cb0: 0000 7253 0000 0072 0600 0000 723c 0000  ..rS...r....r<..
-00000cc0: 0072 5e00 0000 723a 0000 0072 3a00 0000  .r^...r:...r:...
-00000cd0: 723a 0000 0072 3b00 0000 7254 0000 0061  r:...r;...rT...a
-00000ce0: 0000 0073 0800 0000 0801 0a01 04ff 0a0b  ...s............
-00000cf0: 7254 0000 0063 0000 0000 0000 0000 0000  rT...c..........
-00000d00: 0000 0000 0000 0900 0000 4000 0000 7328  ..........@...s(
-00000d10: 0000 0065 005a 0164 005a 0264 0164 0264  ...e.Z.d.Z.d.d.d
-00000d20: 0264 0264 0264 0364 0365 0364 0266 0964  .d.d.d.d.e.d.f.d
-00000d30: 0464 0584 015a 0464 0253 0029 06da 0643  .d...Z.d.S.)...C
-00000d40: 6f6c 756d 6eda 004e e932 0000 0063 0a00  olumn..N.2...c..
-00000d50: 0000 0000 0000 0000 0000 0a00 0000 0200  ................
-00000d60: 0000 4300 0000 733a 0000 007c 017c 005f  ..C...s:...|.|._
-00000d70: 007c 027c 005f 017c 037c 005f 027c 047c  .|.|._.|.|._.|.|
-00000d80: 005f 037c 057c 005f 047c 067c 005f 057c  ._.|.|._.|.|._.|
-00000d90: 077c 005f 067c 087c 005f 077c 097c 005f  .|._.|.|._.|.|._
-00000da0: 0864 0153 0029 0261 d601 0000 0a0a 2020  .d.S.).a......  
-00000db0: 2020 2020 2020 3a70 6172 616d 2063 6f6e        :param con
-00000dc0: 7465 6e74 3a20 5468 6973 2076 6172 6961  tent: This varia
-00000dd0: 626c 6527 7320 6461 7461 2077 696c 6c20  ble's data will 
-00000de0: 6265 2070 6173 7365 6420 696e 746f 2074  be passed into t
-00000df0: 6865 2052 6570 6f72 746c 6162 2773 2050  he Reportlab's P
-00000e00: 6172 6167 7261 7068 2043 6c61 7373 2c20  aragraph Class, 
-00000e10: 6f72 2069 6620 6974 7320 4279 7465 7349  or if its BytesI
-00000e20: 4f0a 2020 2020 2020 2020 2020 2020 2020  O.              
-00000e30: 2020 2020 2020 2020 2020 6f62 6a65 6374            object
-00000e40: 2077 696c 6c20 6265 2070 6173 7365 6420   will be passed 
-00000e50: 696e 2061 2052 6570 6f72 746c 6162 2773  in a Reportlab's
-00000e60: 2049 6d61 6765 2043 6c61 7373 206f 626a   Image Class obj
-00000e70: 6563 7420 616e 6420 6170 7065 6e64 6564  ect and appended
-00000e80: 2069 6e20 7468 6520 7461 626c 652e 0a20   in the table.. 
-00000e90: 2020 2020 2020 203a 7061 7261 6d20 6772         :param gr
-00000ea0: 6964 3a0a 2020 2020 2020 2020 3a70 6172  id:.        :par
-00000eb0: 616d 2062 6163 6b67 726f 756e 645f 636f  am background_co
-00000ec0: 6c6f 723a 0a20 2020 2020 2020 203a 7061  lor:.        :pa
-00000ed0: 7261 6d20 7465 7874 5f63 6f6c 6f72 3a0a  ram text_color:.
-00000ee0: 2020 2020 2020 2020 3a70 6172 616d 2069          :param i
-00000ef0: 6d61 6765 5f77 6964 7468 3a0a 2020 2020  mage_width:.    
-00000f00: 2020 2020 3a70 6172 616d 2069 6d61 6765      :param image
-00000f10: 5f68 6569 6768 743a 0a20 2020 2020 2020  _height:.       
-00000f20: 203a 7061 7261 6d20 616c 6967 6e3a 2041   :param align: A
-00000f30: 6c69 676e 206f 7074 696f 6e73 2028 6672  lign options (fr
-00000f40: 6f6d 2052 6570 6f72 744c 6162 2920 2d3e  om ReportLab) ->
-00000f50: 2054 415f 4c45 4654 2c20 5441 5f43 454e   TA_LEFT, TA_CEN
-00000f60: 5445 522c 2054 415f 5249 4748 542c 2054  TER, TA_RIGHT, T
-00000f70: 415f 4a55 5354 4946 590a 2020 2020 2020  A_JUSTIFY.      
-00000f80: 2020 4e29 09da 0763 6f6e 7465 6e74 7256    N)...contentrV
-00000f90: 0000 0072 5700 0000 7258 0000 0072 5900  ...rW...rX...rY.
-00000fa0: 0000 da0b 696d 6167 655f 7769 6474 68da  ....image_width.
-00000fb0: 0c69 6d61 6765 5f68 6569 6768 7472 5a00  .image_heightrZ.
-00000fc0: 0000 725c 0000 0029 0a72 3500 0000 7262  ..r\...).r5...rb
-00000fd0: 0000 0072 5600 0000 7257 0000 0072 5800  ...rV...rW...rX.
-00000fe0: 0000 7259 0000 0072 6300 0000 7264 0000  ..rY...rc...rd..
-00000ff0: 0072 5a00 0000 725c 0000 0072 3a00 0000  .rZ...r\...r:...
-00001000: 723a 0000 0072 3b00 0000 723c 0000 0073  r:...r;...r<...s
-00001010: 0000 0073 1200 0000 000d 0601 0601 0601  ...s............
-00001020: 0601 0601 0601 0601 0601 7a0f 436f 6c75  ..........z.Colu
-00001030: 6d6e 2e5f 5f69 6e69 745f 5f29 0572 5100  mn.__init__).rQ.
-00001040: 0000 7252 0000 0072 5300 0000 7206 0000  ..rR...rS...r...
-00001050: 0072 3c00 0000 723a 0000 0072 3a00 0000  .r<...r:...r:...
-00001060: 723a 0000 0072 3b00 0000 725f 0000 0071  r:...r;...r_...q
-00001070: 0000 0073 0600 0000 0802 0c01 06ff 725f  ...s..........r_
-00001080: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00001090: 0000 0000 0300 0000 4000 0000 731c 0000  ........@...s...
-000010a0: 0065 005a 0164 005a 0264 0165 036a 0466  .e.Z.d.Z.d.e.j.f
-000010b0: 0264 0264 0384 015a 0564 0453 0029 05da  .d.d...Z.d.S.)..
-000010c0: 0447 7269 64e7 0000 0000 0000 e03f 6303  .Grid........?c.
-000010d0: 0000 0000 0000 0000 0000 0003 0000 0002  ................
-000010e0: 0000 0043 0000 0073 1000 0000 7c01 7c00  ...C...s....|.|.
-000010f0: 5f00 7c02 7c00 5f01 6400 5300 723d 0000  _.|.|._.d.S.r=..
-00001100: 0029 02da 0a6c 696e 655f 7769 6474 68da  .)...line_width.
-00001110: 0a6c 696e 655f 636f 6c6f 7229 0372 3500  .line_color).r5.
-00001120: 0000 7267 0000 0072 6800 0000 723a 0000  ..rg...rh...r:..
-00001130: 0072 3a00 0000 723b 0000 0072 3c00 0000  .r:...r;...r<...
-00001140: 8c00 0000 7304 0000 0000 0106 017a 0d47  ....s........z.G
-00001150: 7269 642e 5f5f 696e 6974 5f5f 4ea9 0672  rid.__init__N..r
-00001160: 5100 0000 7252 0000 0072 5300 0000 7205  Q...rR...rS...r.
-00001170: 0000 00da 0467 7261 7972 3c00 0000 723a  .....grayr<...r:
-00001180: 0000 0072 3a00 0000 723a 0000 0072 3b00  ...r:...r:...r;.
-00001190: 0000 7265 0000 008b 0000 0073 0200 0000  ..re.......s....
-000011a0: 0801 7265 0000 0063 0000 0000 0000 0000  ..re...c........
-000011b0: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
-000011c0: 731e 0000 0065 005a 0164 005a 0264 0164  s....e.Z.d.Z.d.d
-000011d0: 0265 036a 0466 0364 0364 0484 015a 0564  .e.j.f.d.d...Z.d
-000011e0: 0553 0029 06da 044c 696e 65da 094c 494e  .S.)...Line..LIN
-000011f0: 4542 454c 4f57 7266 0000 0063 0400 0000  EBELOWrf...c....
-00001200: 0000 0000 0000 0000 0400 0000 0200 0000  ................
-00001210: 4300 0000 7316 0000 007c 017c 005f 007c  C...s....|.|._.|
-00001220: 027c 005f 017c 037c 005f 0264 0053 0072  .|._.|.|._.d.S.r
-00001230: 3d00 0000 2903 da0d 6c69 6e65 5f70 6f73  =...)...line_pos
-00001240: 6974 696f 6e72 6700 0000 7268 0000 0029  itionrg...rh...)
-00001250: 0472 3500 0000 726d 0000 0072 6700 0000  .r5...rm...rg...
-00001260: 7268 0000 0072 3a00 0000 723a 0000 0072  rh...r:...r:...r
-00001270: 3b00 0000 723c 0000 0092 0000 0073 0600  ;...r<.......s..
-00001280: 0000 0001 0601 0601 7a0d 4c69 6e65 2e5f  ........z.Line._
-00001290: 5f69 6e69 745f 5f4e 7269 0000 0072 3a00  _init__Nri...r:.
-000012a0: 0000 723a 0000 0072 3a00 0000 723b 0000  ..r:...r:...r;..
-000012b0: 0072 6b00 0000 9100 0000 7302 0000 0008  .rk.......s.....
-000012c0: 0172 6b00 0000 6301 0000 0000 0000 0000  .rk...c.........
-000012d0: 0000 0001 0000 0005 0000 0043 0000 0073  ...........C...s
-000012e0: 0e00 0000 6401 a000 7c00 6402 6402 a103  ....d...|.d.d...
-000012f0: 5300 2903 4e7a 743c 7061 7261 2061 7574  S.).Nzt<para aut
-00001300: 6f4c 6561 6469 6e67 3d22 6f66 6622 2066  oLeading="off" f
-00001310: 6f6e 7453 697a 653d 3132 3e54 6869 7320  ontSize=12>This 
-00001320: 266c 743b 696d 672f 2667 743b 203c 696d  &lt;img/&gt; <im
-00001330: 670a 7372 633d 227b 307d 2220 7661 6c69  g.src="{0}" vali
-00001340: 676e 3d22 746f 7022 2077 6964 7468 3d22  gn="top" width="
-00001350: 7b31 7d22 2068 6569 6768 743d 227b 327d  {1}" height="{2}
-00001360: 222f 3e20 3c2f 7061 7261 3ee9 6400 0000  "/> </para>.d...
-00001370: a901 da06 666f 726d 6174 2901 5a08 696d  ....format).Z.im
-00001380: 675f 7061 7468 723a 0000 0072 3a00 0000  g_pathr:...r:...
-00001390: 723b 0000 00da 0767 6574 5f69 6d67 9800  r;.....get_img..
-000013a0: 0000 7306 0000 0000 0604 0106 ff72 7100  ..s..........rq.
-000013b0: 0000 6302 0000 0000 0000 0000 0000 0016  ..c.............
-000013c0: 0000 0009 0000 0043 0000 0073 0603 0000  .......C...s....
-000013d0: 7c01 6400 7500 720c 6700 7d01 7c01 4400  |.d.u.r.g.}.|.D.
-000013e0: 5d0e 7d02 7400 a001 7c02 a101 0100 7110  ].}.t...|.....q.
-000013f0: 6700 7d03 7402 7c00 8301 4400 5dd8 5c02  g.}.t.|...D.].\.
-00001400: 7d04 7d05 7403 7c05 7404 8302 72f8 6700  }.}.t.|.t...r.g.
-00001410: 7d06 7402 7c05 6a05 8301 4400 5d9e 5c02  }.t.|.j...D.].\.
-00001420: 7d07 7d08 7406 8300 7d09 7c08 6a07 726a  }.}.t...}.|.j.rj
-00001430: 7c08 6a07 7c09 5f08 6e0e 7c05 6a07 7278  |.j.|._.n.|.j.rx
-00001440: 7c05 6a07 7c09 5f08 7c08 6a09 7288 7c08  |.j.|._.|.j.r.|.
-00001450: 6a09 7c09 5f0a 6e0e 7c05 6a09 7296 7c05  j.|._.n.|.j.r.|.
-00001460: 6a09 7c09 5f0a 7403 7c08 6a0b 740c 8302  j.|._.t.|.j.t...
-00001470: 72b8 740d 7c08 6a0b 7c08 6a0e 7c08 6a0f  r.t.|.j.|.j.|.j.
-00001480: 6401 8d03 7d0a 6e28 7403 7c08 6a0b 7410  d...}.n(t.|.j.t.
-00001490: 8302 72da 7411 6402 a012 7c08 6a0b 6403  ..r.t.d...|.j.d.
-000014a0: a102 7c09 8302 7d0a 6e06 7c08 6a0b 7d0a  ..|...}.n.|.j.}.
-000014b0: 7c06 a013 7c0a a101 0100 714c 7c03 a013  |...|.....qL|...
-000014c0: 7c06 a101 0100 712c 7c03 a013 7c05 6701  |.....q,|...|.g.
-000014d0: a101 0100 712c 7414 8300 7d0b 7402 7c00  ....q,t...}.t.|.
-000014e0: 8301 4400 9001 5dd8 5c02 7d04 7d05 7403  ..D...].\.}.}.t.
-000014f0: 7c05 7404 8302 9001 7214 7402 7c05 6a05  |.t.....r.t.|.j.
-00001500: 8301 4400 9001 5db4 5c02 7d07 7d0c 6404  ..D...].\.}.}.d.
-00001510: 7d0d 6400 7d0e 7c0c 6a15 9001 725a 6405  }.d.}.|.j...rZd.
-00001520: 7d0d 7c0c 6a15 7d0e 6e12 7c05 6a15 9001  }.|.j.}.n.|.j...
-00001530: 726c 6405 7d0d 7c05 6a15 7d0e 7c0d 9001  rld.}.|.j.}.|...
-00001540: 728a 7c0b a016 6406 7c07 7c04 6602 7c07  r.|...d.|.|.f.|.
-00001550: 7c04 6602 7c0e a104 0100 6404 7d0d 6400  |.f.|.....d.}.d.
-00001560: 7d0f 6400 7d10 7c0c 6a17 9001 72b4 6405  }.d.}.|.j...r.d.
-00001570: 7d0d 7c0c 6a17 6a18 7d0f 7c0c 6a17 6a19  }.|.j.j.}.|.j.j.
-00001580: 7d10 6e1c 7c05 6a17 9001 72d0 6405 7d0d  }.n.|.j...r.d.}.
-00001590: 7c05 6a17 6a18 7d0f 7c05 6a17 6a19 7d10  |.j.j.}.|.j.j.}.
-000015a0: 7c0d 9001 72f0 7c0b a016 6407 7c07 7c04  |...r.|...d.|.|.
-000015b0: 6602 7c07 7c04 6602 7c10 7c0f a105 0100  f.|.|.f.|.|.....
-000015c0: 6404 7d0d 6400 7d11 6400 7d12 6400 7d13  d.}.d.}.d.}.d.}.
-000015d0: 7c0c 6a1a 9002 7226 6405 7d0d 7c0c 6a1a  |.j...r&d.}.|.j.
-000015e0: 6a18 7d11 7c0c 6a1a 6a19 7d12 7c0c 6a1a  j.}.|.j.j.}.|.j.
-000015f0: 6a1b 7d13 6e24 7c05 6a1a 9002 724a 6405  j.}.n$|.j...rJd.
-00001600: 7d0d 7c05 6a1a 6a18 7d11 7c05 6a1a 6a19  }.|.j.j.}.|.j.j.
-00001610: 7d12 7c05 6a1a 6a1b 7d13 7c0d 9002 726a  }.|.j.j.}.|...rj
-00001620: 7c0b a016 7c13 7c07 7c04 6602 7c07 7c04  |...|.|.|.f.|.|.
-00001630: 6602 7c12 7c11 a105 0100 7c05 6a1c 9002  f.|.|.....|.j...
-00001640: 7288 7c0b a016 6408 7c07 7c04 6602 6409  r.|...d.|.|.f.d.
-00001650: 7c04 6602 a103 0100 6404 7d0d 6400 7d14  |.f.....d.}.d.}.
-00001660: 7c0c 6a1d 9002 72ae 6405 7d0d 7c0c 6a1d  |.j...r.d.}.|.j.
-00001670: 7d14 741e 640a 7c14 8302 0100 6e1c 7c05  }.t.d.|.....n.|.
-00001680: 6a1d 9002 72ca 6405 7d0d 7c05 6a1d 7d14  j...r.d.}.|.j.}.
-00001690: 741e 640b 7c14 8302 0100 7c0d 9001 7234  t.d.|.....|...r4
-000016a0: 7c0b a016 640c 7c07 7c04 6602 7c07 7c04  |...d.|.|.f.|.|.
-000016b0: 6602 7c14 a104 0100 9001 7134 9001 7114  f.|.......q4..q.
-000016c0: 741f 7c03 8301 7d15 7c15 a020 7c0b a101  t.|...}.|.. |...
-000016d0: 0100 7c15 5300 290d 4e29 0272 1e00 0000  ..|.S.).N).r....
-000016e0: 721f 0000 007a 027b 7d7a 034e 2f41 4654  r....z.{}z.N/AFT
-000016f0: da0a 4241 434b 4752 4f55 4e44 da04 4752  ..BACKGROUND..GR
-00001700: 4944 da04 5350 414e e9ff ffff ff7a 0443  ID..SPAN.....z.C
-00001710: 4f4c 3a7a 0452 4f57 3ada 0656 414c 4947  OL:z.ROW:..VALIG
-00001720: 4e29 2172 0a00 0000 da0c 7265 6769 7374  N)!r......regist
-00001730: 6572 466f 6e74 da09 656e 756d 6572 6174  erFont..enumerat
-00001740: 6572 3e00 0000 7254 0000 0072 5500 0000  er>...rT...rU...
-00001750: 7229 0000 0072 5a00 0000 da09 616c 6967  r)...rZ.....alig
-00001760: 6e6d 656e 7472 5900 0000 da09 7465 7874  nmentrY.....text
-00001770: 436f 6c6f 7272 6200 0000 7203 0000 0072  Colorrb...r....r
-00001780: 0400 0000 7263 0000 0072 6400 0000 da03  ....rc...rd.....
-00001790: 7374 7272 0f00 0000 7270 0000 0072 4000  strr....rp...r@.
-000017a0: 0000 7211 0000 0072 5800 0000 da03 6164  ..r....rX.....ad
-000017b0: 6472 5700 0000 7268 0000 0072 6700 0000  drW...rh...rg...
-000017c0: 7256 0000 0072 6d00 0000 725b 0000 0072  rV...rm...r[...r
-000017d0: 5c00 0000 da05 7072 696e 7472 1000 0000  \.....printr....
-000017e0: da08 7365 7453 7479 6c65 2916 da04 6461  ..setStyle)...da
-000017f0: 7461 da05 666f 6e74 73da 0466 6f6e 745a  ta..fonts..fontZ
-00001800: 0a74 6162 6c65 5f64 6174 615a 0772 6f77  .table_dataZ.row
-00001810: 5f63 7472 5a07 726f 775f 6f62 6a5a 0c63  _ctrZ.row_objZ.c
-00001820: 6f6c 756d 6e5f 6669 6e61 6c5a 0763 6f6c  olumn_finalZ.col
-00001830: 5f63 7472 da03 636f 6cda 0573 7479 6c65  _ctr..col..style
-00001840: 5a04 5f63 6f6c 5a0c 7461 626c 655f 7374  Z._colZ.table_st
-00001850: 796c 6573 5a07 636f 6c5f 6f62 6a5a 0b61  ylesZ.col_objZ.a
-00001860: 7070 6c79 5f73 7479 6c65 7258 0000 005a  pply_stylerX...Z
-00001870: 0f67 7269 645f 6c69 6e65 5f63 6f6c 6f72  .grid_line_color
-00001880: 5a0f 6772 6964 5f6c 696e 655f 7769 6474  Z.grid_line_widt
-00001890: 6872 6800 0000 7267 0000 0072 6d00 0000  hrh...rg...rm...
-000018a0: 725c 0000 00da 0174 723a 0000 0072 3a00  r\.....tr:...r:.
-000018b0: 0000 723b 0000 00da 1170 6664 5f74 6162  ..r;.....pfd_tab
-000018c0: 6c65 5f62 7569 6c64 6572 a200 0000 73ac  le_builder....s.
-000018d0: 0000 0000 0108 0104 0108 010c 0204 0110  ................
-000018e0: 010a 0104 0112 0106 0506 010a 0106 0108  ................
-000018f0: 0206 010a 0106 0108 030c 0116 010c 0116  ................
-00001900: 0306 020c 020c 020e 0306 0112 010c 0414  ................
-00001910: 0104 0204 0108 0104 0108 0108 0104 0106  ................
-00001920: 0106 0118 0204 0104 0104 0108 0104 0108  ................
-00001930: 010a 0108 0104 0108 0108 0106 011a 0204  ................
-00001940: 0104 0104 0104 0108 0104 0108 0108 010a  ................
-00001950: 0108 0104 0108 0108 0108 0106 011a 0208  ................
-00001960: 0116 0204 0104 0108 0104 0106 010c 0108  ................
-00001970: 0104 0106 010a 0106 0120 0108 010a 0172  ......... .....r
-00001980: 8500 0000 6304 0000 0000 0000 0000 0000  ....c...........
-00001990: 0009 0000 0008 0000 0043 0000 0073 aa00  .........C...s..
-000019a0: 0000 7c02 a000 7401 a101 0100 7402 7254  ..|...t.....t.rT
-000019b0: 7403 a004 7402 a101 7d04 7405 7c04 6a06  t...t...}.t.|.j.
-000019c0: 6401 1900 7c04 6a06 6402 1900 7407 6403  d...|.j.d...t.d.
-000019d0: 8d03 5c02 7d05 7d06 7408 7c04 8301 7d07  ..\.}.}.t.|...}.
-000019e0: 7c02 6a09 7c07 7c00 7c01 7c05 7c06 6404  |.j.|.|.|.|.|.d.
-000019f0: 6405 8d06 0100 7c02 a00a 6406 6407 a102  d.....|...d.d...
-00001a00: 0100 6408 7c03 6a0b 1600 7d08 7c02 a00c  ..d.|.j...}.|...
-00001a10: 6409 6407 640a 7c08 1700 640a 1700 a103  d.d.d.|...d.....
-00001a20: 0100 740d 7292 7c02 a00c 640b 6407 740d  ..t.r.|...d.d.t.
-00001a30: a103 0100 7c02 a00e 740f 640c 7410 740f  ....|...t.d.t.t.
-00001a40: 1700 640c a104 0100 6400 5300 290d 4e72  ..d.....d.S.).Nr
-00001a50: 0100 0000 7216 0000 0029 035a 0969 6d67  ....r....).Z.img
-00001a60: 5f77 6964 7468 5a0a 696d 675f 6865 6967  _widthZ.img_heig
-00001a70: 6874 5a11 696d 675f 6465 7369 7265 645f  htZ.img_desired_
-00001a80: 7769 6474 68da 0461 7574 6f29 0372 1e00  width..auto).r..
-00001a90: 0000 721f 0000 00da 046d 6173 6b7a 0e48  ..r......maskz.H
-00001aa0: 656c 7665 7469 6361 2d42 6f6c 6472 1a00  elvetica-Boldr..
-00001ab0: 0000 7a02 2564 6927 0100 00fa 012d 69fb  ..z.%di'.....-i.
-00001ac0: 0100 00e9 1400 0000 2911 da08 7365 7454  ........)...setT
-00001ad0: 6974 6c65 722a 0000 0072 2700 0000 da05  itler*...r'.....
-00001ae0: 7069 6c69 6d72 4900 0000 7212 0000 00da  pilimrI...r.....
-00001af0: 0473 697a 6572 2b00 0000 7209 0000 00da  .sizer+...r.....
-00001b00: 0964 7261 7749 6d61 6765 da07 7365 7446  .drawImage..setF
-00001b10: 6f6e 74da 0470 6167 65da 1164 7261 7743  ont..page..drawC
-00001b20: 656e 7472 6564 5374 7269 6e67 7228 0000  entredStringr(..
-00001b30: 0072 5600 0000 da0c 4241 5349 435f 4d41  .rV.....BASIC_MA
-00001b40: 5247 494e 7230 0000 0029 0972 3600 0000  RGINr0...).r6...
-00001b50: 7237 0000 00da 0663 616e 7661 7372 2d00  r7.....canvasr-.
-00001b60: 0000 da02 696d 5a0b 7072 696e 745f 7769  ....imZ.print_wi
-00001b70: 6474 685a 0c70 7269 6e74 5f68 6569 6768  dthZ.print_heigh
-00001b80: 745a 0770 696c 5f69 6d67 5a10 7061 6765  tZ.pil_imgZ.page
-00001b90: 5f6e 756d 6265 725f 7465 7874 723a 0000  _number_textr:..
-00001ba0: 0072 3a00 0000 723b 0000 0072 3200 0000  .r:...r;...r2...
-00001bb0: 1201 0000 732e 0000 0000 010a 0304 010a  ....s...........
-00001bc0: 0102 0108 0108 0102 fd0a 0508 0104 0102  ................
-00001bd0: 0102 0102 0102 0102 0102 fa06 0c0c 020a  ................
-00001be0: 0116 0204 010e 0272 3200 0000 6300 0000  .......r2...c...
-00001bf0: 0000 0000 0000 0000 0002 0000 0008 0000  ................
-00001c00: 0043 0000 0073 5200 0000 7400 8300 7d00  .C...sR...t...}.
-00001c10: 7c00 6401 1900 7d01 7401 7c01 5f02 7403  |.d...}.t.|._.t.
-00001c20: a004 7405 6402 7406 6a07 a008 7409 6403  ..t.d.t.j...t.d.
-00001c30: a102 8302 a101 0100 7403 a004 7405 6404  ........t...t.d.
-00001c40: 7406 6a07 a008 7409 6405 a102 8302 a101  t.j...t.d.......
-00001c50: 0100 6402 7c01 5f0a 7c01 5300 2906 4eda  ..d.|._.|.S.).N.
-00001c60: 0842 6f64 7954 6578 745a 084e 6f74 6f53  .BodyTextZ.NotoS
-00001c70: 616e 737a 1a66 6f6e 7473 2f4e 6f74 6f53  ansz.fonts/NotoS
-00001c80: 616e 732d 5265 6775 6c61 722e 7474 665a  ans-Regular.ttfZ
-00001c90: 0c4e 6f74 6f53 616e 7342 6f6c 647a 1766  .NotoSansBoldz.f
-00001ca0: 6f6e 7473 2f4e 6f74 6f53 616e 732d 426f  onts/NotoSans-Bo
-00001cb0: 6c64 2e74 7466 290b 7208 0000 00da 0e42  ld.ttf).r......B
-00001cc0: 4f44 595f 464f 4e54 5f53 495a 45da 0866  ODY_FONT_SIZE..f
-00001cd0: 6f6e 7453 697a 6572 0a00 0000 7277 0000  ontSizer....rw..
-00001ce0: 0072 0b00 0000 da02 6f73 da04 7061 7468  .r......os..path
-00001cf0: da04 6a6f 696e da0c 5f5f 6c6f 6361 7469  ..join..__locati
-00001d00: 6f6e 5f5f da08 666f 6e74 4e61 6d65 2902  on__..fontName).
-00001d10: 5a12 7361 6d70 6c65 5f73 7479 6c65 5f73  Z.sample_style_s
-00001d20: 6865 6574 5a0a 626f 6479 5f73 7479 6c65  heetZ.body_style
-00001d30: 723a 0000 0072 3a00 0000 723b 0000 0072  r:...r:...r;...r
-00001d40: 2900 0000 3501 0000 730e 0000 0000 0106  )...5...s.......
-00001d50: 0108 0106 011a 011a 0106 0172 2900 0000  ...........r)...
-00001d60: 6301 0000 0000 0000 0000 0000 0005 0000  c...............
-00001d70: 0004 0000 0043 0000 0073 3e00 0000 6401  .....C...s>...d.
-00001d80: 7d01 7400 7c00 8301 4400 5d2c 5c02 7d02  }.t.|...D.],\.}.
-00001d90: 7d03 7401 7c03 7402 8302 7228 7403 7c03  }.t.|.t...r(t.|.
-00001da0: 6a04 8301 6e02 6402 7d04 7c04 7c01 6b04  j...n.d.}.|.|.k.
-00001db0: 720c 7c04 7d01 710c 7c01 5300 2903 4e72  r.|.}.q.|.S.).Nr
-00001dc0: 0100 0000 7216 0000 0029 0572 7800 0000  ....r....).rx...
-00001dd0: 723e 0000 0072 5400 0000 725d 0000 0072  r>...rT...r]...r
-00001de0: 5500 0000 2905 727f 0000 005a 0f6d 6178  U...).r....Z.max
-00001df0: 5f6e 756d 5f6f 665f 636f 6c73 5a0b 726f  _num_of_colsZ.ro
-00001e00: 775f 636f 756e 7465 72da 0372 6f77 5a0b  w_counter..rowZ.
-00001e10: 6e75 6d5f 6f66 5f63 6f6c 7372 3a00 0000  num_of_colsr:...
-00001e20: 723a 0000 0072 3b00 0000 da17 6669 6e64  r:...r;.....find
-00001e30: 5f6d 6178 5f6e 756d 5f6f 665f 636f 6c75  _max_num_of_colu
-00001e40: 6d6e 733f 0100 0073 0c00 0000 0001 0401  mns?...s........
-00001e50: 1001 1801 0801 0601 729d 0000 0063 0100  ........r....c..
-00001e60: 0000 0000 0000 0000 0000 0100 0000 0300  ................
-00001e70: 0000 4300 0000 730a 0000 0064 01a0 007c  ..C...s....d...|
-00001e80: 00a1 0153 0029 024e 7a03 7b7d 3a72 6f00  ...S.).Nz.{}:ro.
-00001e90: 0000 2901 da05 7061 7261 6d72 3a00 0000  ..)...paramr:...
-00001ea0: 723a 0000 0072 3b00 0000 da0c 6170 7065  r:...r;.....appe
-00001eb0: 6e64 5f63 6f6c 6f6e 4801 0000 7302 0000  nd_colonH...s...
-00001ec0: 0000 0172 9f00 0000 2901 4e29 4172 4b00  ...r....).N)ArK.
-00001ed0: 0000 7297 0000 00da 0966 756e 6374 6f6f  ..r......functoo
-00001ee0: 6c73 7202 0000 0072 0300 0000 da03 5049  lsr....r......PI
-00001ef0: 4c72 0400 0000 728b 0000 00da 0d72 6570  Lr....r......rep
-00001f00: 6f72 746c 6162 2e6c 6962 7205 0000 00da  ortlab.libr.....
-00001f10: 1372 6570 6f72 746c 6162 2e6c 6962 2e65  .reportlab.lib.e
-00001f20: 6e75 6d73 7206 0000 005a 1772 6570 6f72  numsr....Z.repor
-00001f30: 746c 6162 2e6c 6962 2e70 6167 6573 697a  tlab.lib.pagesiz
-00001f40: 6573 7207 0000 00da 1472 6570 6f72 746c  esr......reportl
-00001f50: 6162 2e6c 6962 2e73 7479 6c65 7372 0800  ab.lib.stylesr..
-00001f60: 0000 da13 7265 706f 7274 6c61 622e 6c69  ....reportlab.li
-00001f70: 622e 7574 696c 7372 0900 0000 da11 7265  b.utilsr......re
-00001f80: 706f 7274 6c61 622e 7064 6662 6173 6572  portlab.pdfbaser
-00001f90: 0a00 0000 5a19 7265 706f 7274 6c61 622e  ....Z.reportlab.
-00001fa0: 7064 6662 6173 652e 7474 666f 6e74 7372  pdfbase.ttfontsr
-00001fb0: 0b00 0000 da12 7265 706f 7274 6c61 622e  ......reportlab.
-00001fc0: 706c 6174 7970 7573 720c 0000 0072 0d00  platypusr....r..
-00001fd0: 0000 720e 0000 0072 0f00 0000 7210 0000  ..r....r....r...
-00001fe0: 0072 1100 0000 5a19 7064 665f 7461 626c  .r....Z.pdf_tabl
-00001ff0: 655f 6275 696c 6465 722e 6865 6c70 6572  e_builder.helper
-00002000: 7372 1200 0000 da06 7374 796c 6573 5a06  sr......stylesZ.
-00002010: 7374 796c 654e 5a06 7374 796c 6548 5a13  styleNZ.styleHZ.
-00002020: 4445 5349 5245 445f 5048 4f54 4f5f 5749  DESIRED_PHOTO_WI
-00002030: 4454 485a 1444 4553 4952 4544 5f50 484f  DTHZ.DESIRED_PHO
-00002040: 544f 5f48 4549 4748 5472 9100 0000 7295  TO_HEIGHTr....r.
-00002050: 0000 0072 3000 0000 7231 0000 005a 064c  ...r0...r1...Z.L
-00002060: 494e 455f 5972 2e00 0000 722f 0000 0072  INE_Yr....r/...r
-00002070: 2800 0000 7227 0000 0072 2b00 0000 722a  (...r'...r+...r*
-00002080: 0000 0072 9800 0000 da08 7265 616c 7061  ...r......realpa
-00002090: 7468 7299 0000 00da 0667 6574 6377 64da  thr......getcwd.
-000020a0: 0764 6972 6e61 6d65 da08 5f5f 6669 6c65  .dirname..__file
-000020b0: 5f5f 729a 0000 0072 1c00 0000 7254 0000  __r....r....rT..
-000020c0: 0072 5f00 0000 7265 0000 0072 6b00 0000  .r_...re...rk...
-000020d0: 7271 0000 0072 8500 0000 7232 0000 0072  rq...r....r2...r
-000020e0: 2900 0000 729d 0000 0072 9f00 0000 723a  )...r....r....r:
-000020f0: 0000 0072 3a00 0000 723a 0000 0072 3b00  ...r:...r:...r;.
-00002100: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00002110: 7356 0000 0008 0108 010c 010c 020c 010c  sV..............
-00002120: 010c 010c 010c 010c 010c 010c 0110 0110  ................
-00002130: 0114 020c 0206 0108 0108 020c 0110 0204  ................
-00002140: 0104 0104 0104 0104 0204 0104 0204 0104  ................
-00002150: 0104 0104 0122 030e 360e 100e 1a0e 060e  ....."..6.......
-00002160: 0708 0a0a 7008 2308 0a08 09              ....p.#....
+00000130: 650d 6400 1900 5a26 650d 6413 1900 5a27  e.d...Z&e.d...Z'
+00000140: 6418 5a28 6416 5a29 6416 5a2a 6401 612b  d.Z(d.Z)d.Z*d.a+
+00000150: 6401 612c 6419 612d 641a 612e 6501 6a2f  d.a,d.a-d.a.e.j/
+00000160: a030 6501 6a2f a031 6501 a032 a100 6501  .0e.j/.1e..2..e.
+00000170: 6a2f a033 6534 a101 a102 a101 5a35 4700  j/.3e4......Z5G.
+00000180: 641b 641c 8400 641c 8302 5a36 4700 641d  d.d...d...Z6G.d.
+00000190: 641e 8400 641e 8302 5a37 4700 641f 6420  d...d...Z7G.d.d 
+000001a0: 8400 6420 8302 5a38 4700 6421 6422 8400  ..d ..Z8G.d!d"..
+000001b0: 6422 8302 5a39 4700 6423 6424 8400 6424  d"..Z9G.d#d$..d$
+000001c0: 8302 5a3a 6425 6426 8400 5a3b 6431 6427  ..Z:d%d&..Z;d1d'
+000001d0: 6428 8401 5a3c 6429 642a 8400 5a3d 642b  d(..Z<d)d*..Z=d+
+000001e0: 642c 8400 5a3e 642d 642e 8400 5a3f 642f  d,..Z>d-d...Z?d/
+000001f0: 6430 8400 5a40 6401 5300 2932 e900 0000  d0..Z@d.S.)2....
+00000200: 004e 2901 da07 7061 7274 6961 6c29 01da  .N)...partial)..
+00000210: 0742 7974 6573 494f 2901 da05 496d 6167  .BytesIO)...Imag
+00000220: 6529 01da 0663 6f6c 6f72 7329 01da 0754  e)...colors)...T
+00000230: 415f 4c45 4654 2901 da02 4134 2901 da13  A_LEFT)...A4)...
+00000240: 6765 7453 616d 706c 6553 7479 6c65 5368  getSampleStyleSh
+00000250: 6565 7429 01da 0b49 6d61 6765 5265 6164  eet)...ImageRead
+00000260: 6572 2901 da0a 7064 666d 6574 7269 6373  er)...pdfmetrics
+00000270: 2901 da06 5454 466f 6e74 2902 da0f 4261  )...TTFont)...Ba
+00000280: 7365 446f 6354 656d 706c 6174 6572 0400  seDocTemplater..
+00000290: 0000 2902 da05 4672 616d 65da 0c50 6167  ..)...Frame..Pag
+000002a0: 6554 656d 706c 6174 6529 03da 0950 6172  eTemplate)...Par
+000002b0: 6167 7261 7068 da05 5461 626c 65da 0a54  agraph..Table..T
+000002c0: 6162 6c65 5374 796c 6529 01da 3063 616c  ableStyle)..0cal
+000002d0: 6375 6c61 7465 5f69 6d61 6765 5f64 696d  culate_image_dim
+000002e0: 656e 7369 6f6e 735f 616e 645f 6b65 6570  ensions_and_keep
+000002f0: 5f61 7370 6563 745f 7261 7469 6fda 064e  _aspect_ratio..N
+00000300: 6f72 6d61 6cda 0848 6561 6469 6e67 31e9  ormal..Heading1.
+00000310: a000 0000 e901 0000 00e9 0200 0000 e9aa  ................
+00000320: 0000 00e9 1e00 0000 e908 0000 0069 da02  .............i..
+00000330: 0000 e9b4 0000 007a 0d50 4446 2054 6162  .......z.PDF Tab
+00000340: 2054 6974 6c65 6300 0000 0000 0000 0000   Titlec.........
+00000350: 0000 0000 0000 000d 0000 0040 0000 0073  ...........@...s
+00000360: 5000 0000 6500 5a01 6400 5a02 6401 6401  P...e.Z.d.Z.d.d.
+00000370: 6503 6504 6402 6402 6403 6403 6403 6403  e.e.d.d.d.d.d.d.
+00000380: 6404 6401 6401 660d 6405 6406 8401 5a05  d.d.d.f.d.d...Z.
+00000390: 6407 6408 8400 5a06 6409 640a 8400 5a07  d.d...Z.d.d...Z.
+000003a0: 640b 640c 8400 5a08 640d 640e 8400 5a09  d.d...Z.d.d...Z.
+000003b0: 6401 5300 290f da13 5265 706f 7274 4c61  d.S.)...ReportLa
+000003c0: 6250 4446 4275 696c 6465 724e 7201 0000  bPDFBuilderNr...
+000003d0: 0072 1900 0000 5463 0e00 0000 0000 0000  .r....Tc........
+000003e0: 0000 0000 1700 0000 0a00 0000 4300 0000  ............C...
+000003f0: 730a 0100 007c 0161 007c 0261 0174 0283  s....|.a.|.a.t..
+00000400: 0061 037c 0361 047c 0461 0574 0683 007c  .a.|.a.|.a.t...|
+00000410: 005f 0774 087c 006a 0774 0964 018d 027c  ._.t.|.j.t.d...|
+00000420: 005f 0a64 027d 0e64 027d 0f74 0072 6274  ._.d.}.d.}.t.rbt
+00000430: 0ba0 0c74 00a1 017d 1074 0d7c 106a 0e64  ...t...}.t.|.j.d
+00000440: 0219 007c 106a 0e64 0319 0074 0564 048d  ...|.j.d...t.d..
+00000450: 035c 027d 0e7d 0f74 0f7c 0f18 0064 0518  .\.}.}.t.|...d..
+00000460: 007d 117c 0c72 9c64 027d 127c 0c44 005d  .}.|.r.d.}.|.D.]
+00000470: 207d 137c 1372 7a7c 1264 026b 0472 927c   }.|.rz|.d.k.r.|
+00000480: 1164 0638 007d 117c 1264 0337 007d 1271  .d.8.}.|.d.7.}.q
+00000490: 7a7c 0b72 a87c 1164 0638 007d 1174 1064  z|.r.|.d.8.}.t.d
+000004a0: 0264 0274 0f7c 1118 0018 0064 0717 0074  .d.t.|.....d...t
+000004b0: 1174 0f7c 077c 0a7c 087c 0964 088d 087d  .t.|.|.|.|.d...}
+000004c0: 1474 1274 137c 057c 067c 0b7c 117c 0e7c  .t.t.|.|.|.|.|.|
+000004d0: 0f7c 0c7c 0d83 097d 1574 1464 097c 147c  .|.|...}.t.d.|.|
+000004e0: 1564 0a8d 037d 167c 006a 0aa0 157c 1667  .d...}.|.j...|.g
+000004f0: 01a1 0101 0067 007c 005f 1664 0053 0029  .....g.|._.d.S.)
+00000500: 0b4e 2901 da08 7061 6765 7369 7a65 7201  .N)...pagesizer.
+00000510: 0000 0072 1600 0000 2903 5a09 696d 675f  ...r....).Z.img_
+00000520: 7769 6474 685a 0a69 6d67 5f68 6569 6768  widthZ.img_heigh
+00000530: 745a 1169 6d67 5f64 6573 6972 6564 5f77  tZ.img_desired_w
+00000540: 6964 7468 7219 0000 00e9 0c00 0000 e914  idthr...........
+00000550: 0000 0029 06da 0577 6964 7468 da06 6865  ...)...width..he
+00000560: 6967 6874 da0b 6c65 6674 5061 6464 696e  ight..leftPaddin
+00000570: 67da 0d62 6f74 746f 6d50 6164 6469 6e67  g..bottomPadding
+00000580: da0c 7269 6768 7450 6164 6469 6e67 da0a  ..rightPadding..
+00000590: 746f 7050 6164 6469 6e67 5a09 616c 6c5f  topPaddingZ.all_
+000005a0: 7061 6765 7329 03da 0269 64da 0666 7261  pages)...id..fra
+000005b0: 6d65 73da 066f 6e50 6167 6529 17da 094c  mes..onPage)...L
+000005c0: 4f47 4f5f 5041 5448 da09 5741 5445 524d  OGO_PATH..WATERM
+000005d0: 4152 4bda 0e67 6574 5f62 6f64 795f 7374  ARK..get_body_st
+000005e0: 796c 655a 0a42 4f44 595f 5354 594c 45da  yleZ.BODY_STYLE.
+000005f0: 0d50 4446 5f54 4142 5f54 4954 4c45 da0f  .PDF_TAB_TITLE..
+00000600: 4c4f 474f 5f42 4153 455f 5749 4454 4872  LOGO_BASE_WIDTHr
+00000610: 0300 0000 da0a 7064 665f 6275 6666 6572  ......pdf_buffer
+00000620: 720c 0000 0072 0700 0000 da03 7064 66da  r....r......pdf.
+00000630: 0570 696c 696d da04 6f70 656e 7212 0000  .pilim..openr...
+00000640: 00da 0473 697a 65da 0b50 4147 455f 4845  ...size..PAGE_HE
+00000650: 4947 4854 720d 0000 00da 0a50 4147 455f  IGHTr......PAGE_
+00000660: 5749 4454 4872 0200 0000 da11 6865 6164  WIDTHr......head
+00000670: 6572 5f61 6e64 5f66 6f6f 7465 7272 0e00  er_and_footerr..
+00000680: 0000 da10 6164 6450 6167 6554 656d 706c  ....addPageTempl
+00000690: 6174 6573 da05 7374 6f72 7929 17da 0473  ates..story)...s
+000006a0: 656c 66da 096c 6f67 6f5f 7061 7468 5a09  elf..logo_pathZ.
+000006b0: 7761 7465 726d 6172 6b5a 0d70 6466 5f74  watermarkZ.pdf_t
+000006c0: 6162 5f74 6974 6c65 5a0f 6c6f 676f 5f62  ab_titleZ.logo_b
+000006d0: 6173 655f 7769 6474 68da 0d6c 6f67 6f5f  ase_width..logo_
+000006e0: 6361 6e76 6173 5f78 da0d 6c6f 676f 5f63  canvas_x..logo_c
+000006f0: 616e 7661 735f 795a 1266 7261 6d65 5f6c  anvas_yZ.frame_l
+00000700: 6566 745f 7061 6464 696e 675a 1366 7261  eft_paddingZ.fra
+00000710: 6d65 5f72 6967 6874 5f70 6164 6469 6e67  me_right_padding
+00000720: 5a11 6672 616d 655f 746f 705f 7061 6464  Z.frame_top_padd
+00000730: 696e 675a 1466 7261 6d65 5f62 6f74 746f  ingZ.frame_botto
+00000740: 6d5f 7061 6464 696e 67da 1768 6176 655f  m_padding..have_
+00000750: 6865 6164 6572 5f62 6f74 746f 6d5f 6c69  header_bottom_li
+00000760: 6e65 da0c 636f 6d70 616e 795f 696e 666f  ne..company_info
+00000770: da0b 666f 6f74 6572 5f74 6578 74da 106c  ..footer_text..l
+00000780: 6f67 6f5f 7072 696e 745f 7769 6474 68da  ogo_print_width.
+00000790: 116c 6f67 6f5f 7072 696e 745f 6865 6967  .logo_print_heig
+000007a0: 6874 da02 696d da05 746f 705f 79da 0169  ht..im..top_y..i
+000007b0: da05 7661 6c75 65da 0566 7261 6d65 5a19  ..value..frameZ.
+000007c0: 6865 6164 6572 5f61 6e64 5f66 6f6f 7465  header_and_foote
+000007d0: 725f 7061 7274 6961 6cda 0874 656d 706c  r_partial..templ
+000007e0: 6174 65a9 0072 4700 0000 fa85 433a 5c55  ate..rG.....C:\U
+000007f0: 7365 7273 5c4c 6976 655c 446f 6375 6d65  sers\Live\Docume
+00000800: 6e74 735c 5072 6f6a 6563 7473 5c50 726f  nts\Projects\Pro
+00000810: 6772 616d 6d69 6e67 5c4d 4353 202d 2050  gramming\MCS - P
+00000820: 6572 736f 6e61 6c5c 5079 7468 6f6e 5c23  ersonal\Python\#
+00000830: 5061 636b 6167 6573 5c72 6570 6f72 746c  Packages\reportl
+00000840: 6162 2d70 6466 2d74 6162 6c65 2d62 7569  ab-pdf-table-bui
+00000850: 6c64 6572 5c70 6466 5f74 6162 6c65 5f62  lder\pdf_table_b
+00000860: 7569 6c64 6572 5c62 7569 6c64 6572 2e70  uilder\builder.p
+00000870: 79da 085f 5f69 6e69 745f 5f2d 0000 0073  y..__init__-...s
+00000880: 6400 0000 0009 0401 0401 0601 0401 0402  d...............
+00000890: 0801 1002 0401 0401 0401 0a01 0201 0801  ................
+000008a0: 0801 02fd 0a06 0c01 0401 0401 0801 0401  ................
+000008b0: 0801 0801 0a02 0401 0802 0201 0201 0e01  ................
+000008c0: 0201 0201 0201 0201 0201 02f8 060a 0201  ................
+000008d0: 0201 0201 0201 0201 0201 0201 0201 0201  ................
+000008e0: 02f7 040b 0e01 0e01 7a1c 5265 706f 7274  ........z.Report
+000008f0: 4c61 6250 4446 4275 696c 6465 722e 5f5f  LabPDFBuilder.__
+00000900: 696e 6974 5f5f 6302 0000 0000 0000 0000  init__c.........
+00000910: 0000 0003 0000 0004 0000 0043 0000 0073  ...........C...s
+00000920: 3200 0000 7400 7c01 7401 8302 7222 7c01  2...t.|.t...r"|.
+00000930: 4400 5d10 7d02 7c00 6a02 a003 7c02 a101  D.].}.|.j...|...
+00000940: 0100 710e 6e0c 7c00 6a02 a003 7c01 a101  ..q.n.|.j...|...
+00000950: 0100 6400 5300 a901 4e29 04da 0a69 7369  ..d.S...N)...isi
+00000960: 6e73 7461 6e63 65da 046c 6973 7472 3700  nstance..listr7.
+00000970: 0000 da06 6170 7065 6e64 2903 7238 0000  ....append).r8..
+00000980: 00da 036f 626a da01 7872 4700 0000 7247  ...obj..xrG...rG
+00000990: 0000 0072 4800 0000 da0c 6164 645f 746f  ...rH.....add_to
+000009a0: 5f73 746f 7279 6e00 0000 7308 0000 0000  _storyn...s.....
+000009b0: 010a 0108 0110 027a 2052 6570 6f72 744c  .......z ReportL
+000009c0: 6162 5044 4642 7569 6c64 6572 2e61 6464  abPDFBuilder.add
+000009d0: 5f74 6f5f 7374 6f72 7963 0100 0000 0000  _to_storyc......
+000009e0: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
+000009f0: 0000 7326 0000 007c 006a 00a0 017c 006a  ..s&...|.j...|.j
+00000a00: 02a1 0101 007c 006a 03a0 04a1 007d 017c  .....|.j.....}.|
+00000a10: 006a 03a0 05a1 0001 007c 0153 0072 4a00  .j.......|.S.rJ.
+00000a20: 0000 2906 722f 0000 00da 0562 7569 6c64  ..).r/.....build
+00000a30: 7237 0000 0072 2e00 0000 da08 6765 7476  r7...r......getv
+00000a40: 616c 7565 da05 636c 6f73 6529 0272 3800  alue..close).r8.
+00000a50: 0000 5a09 7064 665f 7661 6c75 6572 4700  ..Z.pdf_valuerG.
+00000a60: 0000 7247 0000 0072 4800 0000 da0d 6765  ..rG...rH.....ge
+00000a70: 745f 7064 665f 7661 6c75 6575 0000 0073  t_pdf_valueu...s
+00000a80: 0800 0000 0001 0e01 0a01 0a01 7a21 5265  ............z!Re
+00000a90: 706f 7274 4c61 6250 4446 4275 696c 6465  portLabPDFBuilde
+00000aa0: 722e 6765 745f 7064 665f 7661 6c75 6563  r.get_pdf_valuec
+00000ab0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000ac0: 0300 0000 4300 0000 731e 0000 007c 006a  ....C...s....|.j
+00000ad0: 00a0 017c 006a 02a1 0101 007c 006a 03a0  ...|.j.....|.j..
+00000ae0: 04a1 0001 007c 006a 0353 0072 4a00 0000  .....|.j.S.rJ...
+00000af0: 2905 722f 0000 0072 5100 0000 7237 0000  ).r/...rQ...r7..
+00000b00: 0072 2e00 0000 7253 0000 00a9 0172 3800  .r....rS.....r8.
+00000b10: 0000 7247 0000 0072 4700 0000 7248 0000  ..rG...rG...rH..
+00000b20: 00da 0e67 6574 5f70 6466 5f62 7566 6665  ...get_pdf_buffe
+00000b30: 727b 0000 0073 0600 0000 0001 0e01 0a01  r{...s..........
+00000b40: 7a22 5265 706f 7274 4c61 6250 4446 4275  z"ReportLabPDFBu
+00000b50: 696c 6465 722e 6765 745f 7064 665f 6275  ilder.get_pdf_bu
+00000b60: 6666 6572 6302 0000 0000 0000 0000 0000  fferc...........
+00000b70: 0003 0000 0008 0000 0043 0000 0073 5600  .........C...sV.
+00000b80: 0000 7c00 6a00 a001 7c00 6a02 a101 0100  ..|.j...|.j.....
+00000b90: 7403 7c01 6401 8302 8f2a 7d02 7c00 6a04  t.|.d....*}.|.j.
+00000ba0: a005 7406 6a07 a101 0100 7c02 a008 7c00  ..t.j.....|...|.
+00000bb0: 6a04 a101 0100 5700 6400 0400 0400 8303  j.....W.d.......
+00000bc0: 0100 6e10 3100 7348 3000 0100 0100 0100  ..n.1.sH0.......
+00000bd0: 5900 0100 6400 5300 2902 4eda 0277 6229  Y...d.S.).N..wb)
+00000be0: 0972 2f00 0000 7251 0000 0072 3700 0000  .r/...rQ...r7...
+00000bf0: 7231 0000 0072 2e00 0000 da04 7365 656b  r1...r......seek
+00000c00: da02 696f da08 5345 454b 5f53 4554 da0a  ..io..SEEK_SET..
+00000c10: 7772 6974 656c 696e 6573 2903 7238 0000  writelines).r8..
+00000c20: 00da 0966 696c 655f 6e61 6d65 da01 6672  ...file_name..fr
+00000c30: 4700 0000 7247 0000 0072 4800 0000 da0d  G...rG...rH.....
+00000c40: 7361 7665 5f70 6466 5f66 696c 6580 0000  save_pdf_file...
+00000c50: 0073 0800 0000 0001 0e01 0c01 0e01 7a21  .s............z!
+00000c60: 5265 706f 7274 4c61 6250 4446 4275 696c  ReportLabPDFBuil
+00000c70: 6465 722e 7361 7665 5f70 6466 5f66 696c  der.save_pdf_fil
+00000c80: 6529 0ada 085f 5f6e 616d 655f 5fda 0a5f  e)...__name__.._
+00000c90: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00000ca0: 6c6e 616d 655f 5f72 2c00 0000 722d 0000  lname__r,...r-..
+00000cb0: 0072 4900 0000 7250 0000 0072 5400 0000  .rI...rP...rT...
+00000cc0: 7256 0000 0072 5e00 0000 7247 0000 0072  rV...r^...rG...r
+00000cd0: 4700 0000 7247 0000 0072 4800 0000 721c  G...rG...rH...r.
+00000ce0: 0000 002b 0000 0073 1000 0000 0802 0801  ...+...s........
+00000cf0: 0a01 08fe 0a41 0807 0806 0805 721c 0000  .....A......r...
+00000d00: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00000d10: 0000 0700 0000 4000 0000 732c 0000 0065  ......@...s,...e
+00000d20: 005a 0164 005a 0264 0164 0164 0164 0164  .Z.d.Z.d.d.d.d.d
+00000d30: 0265 0364 0166 0764 0364 0484 015a 0464  .e.d.f.d.d...Z.d
+00000d40: 0564 0684 005a 0564 0153 0029 07da 0352  .d...Z.d.S.)...R
+00000d50: 6f77 4e46 6309 0000 0000 0000 0000 0000  owNFc...........
+00000d60: 0009 0000 0002 0000 0043 0000 0073 3400  .........C...s4.
+00000d70: 0000 7c01 7c00 5f00 7c02 7c00 5f01 7c03  ..|.|._.|.|._.|.
+00000d80: 7c00 5f02 7c04 7c00 5f03 7c05 7c00 5f04  |._.|.|._.|.|._.
+00000d90: 7c07 7c00 5f05 7c06 7c00 5f06 7c08 7c00  |.|._.|.|._.|.|.
+00000da0: 5f07 6400 5300 724a 0000 0029 08da 0763  _.d.S.rJ...)...c
+00000db0: 6f6c 756d 6e73 da04 6c69 6e65 da04 6772  olumns..line..gr
+00000dc0: 6964 da10 6261 636b 6772 6f75 6e64 5f63  id..background_c
+00000dd0: 6f6c 6f72 da0a 7465 7874 5f63 6f6c 6f72  olor..text_color
+00000de0: da05 616c 6967 6eda 0a66 756c 6c5f 7769  ..align..full_wi
+00000df0: 6474 68da 0676 616c 6967 6e29 0972 3800  dth..valign).r8.
+00000e00: 0000 7263 0000 0072 6400 0000 7265 0000  ..rc...rd...re..
+00000e10: 0072 6600 0000 7267 0000 0072 6900 0000  .rf...rg...ri...
+00000e20: 7268 0000 0072 6a00 0000 7247 0000 0072  rh...rj...rG...r
+00000e30: 4700 0000 7248 0000 0072 4900 0000 8800  G...rH...rI.....
+00000e40: 0000 7310 0000 0000 0206 0106 0106 0106  ..s.............
+00000e50: 0106 0106 0106 017a 0c52 6f77 2e5f 5f69  .......z.Row.__i
+00000e60: 6e69 745f 5f63 0100 0000 0000 0000 0000  nit__c..........
+00000e70: 0000 0100 0000 0200 0000 4300 0000 730a  ..........C...s.
+00000e80: 0000 0074 007c 006a 0183 0153 0072 4a00  ...t.|.j...S.rJ.
+00000e90: 0000 2902 da03 6c65 6e72 6300 0000 7255  ..)...lenrc...rU
+00000ea0: 0000 0072 4700 0000 7247 0000 0072 4800  ...rG...rG...rH.
+00000eb0: 0000 da15 6765 745f 6e75 6d62 6572 5f6f  ....get_number_o
+00000ec0: 665f 636f 6c75 6d6e 7393 0000 0073 0200  f_columns....s..
+00000ed0: 0000 0001 7a19 526f 772e 6765 745f 6e75  ....z.Row.get_nu
+00000ee0: 6d62 6572 5f6f 665f 636f 6c75 6d6e 7329  mber_of_columns)
+00000ef0: 0672 5f00 0000 7260 0000 0072 6100 0000  .r_...r`...ra...
+00000f00: 7206 0000 0072 4900 0000 726c 0000 0072  r....rI...rl...r
+00000f10: 4700 0000 7247 0000 0072 4700 0000 7248  G...rG...rG...rH
+00000f20: 0000 0072 6200 0000 8700 0000 7308 0000  ...rb.......s...
+00000f30: 0008 010a 0104 ff0a 0b72 6200 0000 6300  .........rb...c.
+00000f40: 0000 0000 0000 0000 0000 0000 0000 0009  ................
+00000f50: 0000 0040 0000 0073 2800 0000 6500 5a01  ...@...s(...e.Z.
+00000f60: 6400 5a02 6401 6402 6402 6402 6402 6403  d.Z.d.d.d.d.d.d.
+00000f70: 6403 6503 6402 6609 6404 6405 8401 5a04  d.e.d.f.d.d...Z.
+00000f80: 6402 5300 2906 da06 436f 6c75 6d6e da00  d.S.)...Column..
+00000f90: 4ee9 3200 0000 630a 0000 0000 0000 0000  N.2...c.........
+00000fa0: 0000 000a 0000 0002 0000 0043 0000 0073  ...........C...s
+00000fb0: 3a00 0000 7c01 7c00 5f00 7c02 7c00 5f01  :...|.|._.|.|._.
+00000fc0: 7c03 7c00 5f02 7c04 7c00 5f03 7c05 7c00  |.|._.|.|._.|.|.
+00000fd0: 5f04 7c06 7c00 5f05 7c07 7c00 5f06 7c08  _.|.|._.|.|._.|.
+00000fe0: 7c00 5f07 7c09 7c00 5f08 6401 5300 2902  |._.|.|._.d.S.).
+00000ff0: 61d6 0100 000a 0a20 2020 2020 2020 203a  a......        :
+00001000: 7061 7261 6d20 636f 6e74 656e 743a 2054  param content: T
+00001010: 6869 7320 7661 7269 6162 6c65 2773 2064  his variable's d
+00001020: 6174 6120 7769 6c6c 2062 6520 7061 7373  ata will be pass
+00001030: 6564 2069 6e74 6f20 7468 6520 5265 706f  ed into the Repo
+00001040: 7274 6c61 6227 7320 5061 7261 6772 6170  rtlab's Paragrap
+00001050: 6820 436c 6173 732c 206f 7220 6966 2069  h Class, or if i
+00001060: 7473 2042 7974 6573 494f 0a20 2020 2020  ts BytesIO.     
+00001070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001080: 2020 206f 626a 6563 7420 7769 6c6c 2062     object will b
+00001090: 6520 7061 7373 6564 2069 6e20 6120 5265  e passed in a Re
+000010a0: 706f 7274 6c61 6227 7320 496d 6167 6520  portlab's Image 
+000010b0: 436c 6173 7320 6f62 6a65 6374 2061 6e64  Class object and
+000010c0: 2061 7070 656e 6465 6420 696e 2074 6865   appended in the
+000010d0: 2074 6162 6c65 2e0a 2020 2020 2020 2020   table..        
+000010e0: 3a70 6172 616d 2067 7269 643a 0a20 2020  :param grid:.   
+000010f0: 2020 2020 203a 7061 7261 6d20 6261 636b       :param back
+00001100: 6772 6f75 6e64 5f63 6f6c 6f72 3a0a 2020  ground_color:.  
+00001110: 2020 2020 2020 3a70 6172 616d 2074 6578        :param tex
+00001120: 745f 636f 6c6f 723a 0a20 2020 2020 2020  t_color:.       
+00001130: 203a 7061 7261 6d20 696d 6167 655f 7769   :param image_wi
+00001140: 6474 683a 0a20 2020 2020 2020 203a 7061  dth:.        :pa
+00001150: 7261 6d20 696d 6167 655f 6865 6967 6874  ram image_height
+00001160: 3a0a 2020 2020 2020 2020 3a70 6172 616d  :.        :param
+00001170: 2061 6c69 676e 3a20 416c 6967 6e20 6f70   align: Align op
+00001180: 7469 6f6e 7320 2866 726f 6d20 5265 706f  tions (from Repo
+00001190: 7274 4c61 6229 202d 3e20 5441 5f4c 4546  rtLab) -> TA_LEF
+000011a0: 542c 2054 415f 4345 4e54 4552 2c20 5441  T, TA_CENTER, TA
+000011b0: 5f52 4947 4854 2c20 5441 5f4a 5553 5449  _RIGHT, TA_JUSTI
+000011c0: 4659 0a20 2020 2020 2020 204e 2909 da07  FY.        N)...
+000011d0: 636f 6e74 656e 7472 6400 0000 7265 0000  contentrd...re..
+000011e0: 0072 6600 0000 7267 0000 00da 0b69 6d61  .rf...rg.....ima
+000011f0: 6765 5f77 6964 7468 da0c 696d 6167 655f  ge_width..image_
+00001200: 6865 6967 6874 7268 0000 0072 6a00 0000  heightrh...rj...
+00001210: 290a 7238 0000 0072 7000 0000 7264 0000  ).r8...rp...rd..
+00001220: 0072 6500 0000 7266 0000 0072 6700 0000  .re...rf...rg...
+00001230: 7271 0000 0072 7200 0000 7268 0000 0072  rq...rr...rh...r
+00001240: 6a00 0000 7247 0000 0072 4700 0000 7248  j...rG...rG...rH
+00001250: 0000 0072 4900 0000 9900 0000 7312 0000  ...rI.......s...
+00001260: 0000 0d06 0106 0106 0106 0106 0106 0106  ................
+00001270: 0106 017a 0f43 6f6c 756d 6e2e 5f5f 696e  ...z.Column.__in
+00001280: 6974 5f5f 2905 725f 0000 0072 6000 0000  it__).r_...r`...
+00001290: 7261 0000 0072 0600 0000 7249 0000 0072  ra...r....rI...r
+000012a0: 4700 0000 7247 0000 0072 4700 0000 7248  G...rG...rG...rH
+000012b0: 0000 0072 6d00 0000 9700 0000 7306 0000  ...rm.......s...
+000012c0: 0008 020c 0106 ff72 6d00 0000 6300 0000  .......rm...c...
+000012d0: 0000 0000 0000 0000 0000 0000 0003 0000  ................
+000012e0: 0040 0000 0073 1c00 0000 6500 5a01 6400  .@...s....e.Z.d.
+000012f0: 5a02 6401 6503 6a04 6602 6402 6403 8401  Z.d.e.j.f.d.d...
+00001300: 5a05 6404 5300 2905 da04 4772 6964 e700  Z.d.S.)...Grid..
+00001310: 0000 0000 00e0 3f63 0300 0000 0000 0000  ......?c........
+00001320: 0000 0000 0300 0000 0200 0000 4300 0000  ............C...
+00001330: 7310 0000 007c 017c 005f 007c 027c 005f  s....|.|._.|.|._
+00001340: 0164 0053 0072 4a00 0000 2902 da0a 6c69  .d.S.rJ...)...li
+00001350: 6e65 5f77 6964 7468 da0a 6c69 6e65 5f63  ne_width..line_c
+00001360: 6f6c 6f72 2903 7238 0000 0072 7500 0000  olor).r8...ru...
+00001370: 7276 0000 0072 4700 0000 7247 0000 0072  rv...rG...rG...r
+00001380: 4800 0000 7249 0000 00b2 0000 0073 0400  H...rI.......s..
+00001390: 0000 0001 0601 7a0d 4772 6964 2e5f 5f69  ......z.Grid.__i
+000013a0: 6e69 745f 5f4e a906 725f 0000 0072 6000  nit__N..r_...r`.
+000013b0: 0000 7261 0000 0072 0500 0000 da04 6772  ..ra...r......gr
+000013c0: 6179 7249 0000 0072 4700 0000 7247 0000  ayrI...rG...rG..
+000013d0: 0072 4700 0000 7248 0000 0072 7300 0000  .rG...rH...rs...
+000013e0: b100 0000 7302 0000 0008 0172 7300 0000  ....s......rs...
+000013f0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00001400: 0003 0000 0040 0000 0073 1e00 0000 6500  .....@...s....e.
+00001410: 5a01 6400 5a02 6401 6402 6503 6a04 6603  Z.d.Z.d.d.e.j.f.
+00001420: 6403 6404 8401 5a05 6405 5300 2906 da04  d.d...Z.d.S.)...
+00001430: 4c69 6e65 da09 4c49 4e45 4245 4c4f 5772  Line..LINEBELOWr
+00001440: 7400 0000 6304 0000 0000 0000 0000 0000  t...c...........
+00001450: 0004 0000 0002 0000 0043 0000 0073 1600  .........C...s..
+00001460: 0000 7c01 7c00 5f00 7c02 7c00 5f01 7c03  ..|.|._.|.|._.|.
+00001470: 7c00 5f02 6401 5300 2902 7ae9 0a20 2020  |._.d.S.).z..   
+00001480: 2020 2020 203a 7061 7261 6d20 6c69 6e65       :param line
+00001490: 5f70 6f73 6974 696f 6e3a 2043 616e 2062  _position: Can b
+000014a0: 6520 4c49 4e45 4245 4c4f 572c 204c 494e  e LINEBELOW, LIN
+000014b0: 4541 424f 5645 2c20 4c49 4e45 4245 464f  EABOVE, LINEBEFO
+000014c0: 5245 2c20 4c49 4e45 4146 5445 520a 2020  RE, LINEAFTER.  
+000014d0: 2020 2020 2020 3a70 6172 616d 206c 696e        :param lin
+000014e0: 655f 7769 6474 683a 2043 616e 2062 6520  e_width: Can be 
+000014f0: 302e 352c 2031 2c20 3220 6574 632e 0a20  0.5, 1, 2 etc.. 
+00001500: 2020 2020 2020 203a 7061 7261 6d20 6c69         :param li
+00001510: 6e65 5f63 6f6c 6f72 3a20 4361 6e20 6265  ne_color: Can be
+00001520: 2063 6f6c 6f72 732e 6772 6179 2c20 636f   colors.gray, co
+00001530: 6c6f 7273 2e62 6c61 636b 2065 7463 2e20  lors.black etc. 
+00001540: 6f72 2048 4558 2063 6f6c 6f72 206c 696b  or HEX color lik
+00001550: 6520 2723 3030 3030 3030 272e 0a20 2020  e '#000000'..   
+00001560: 2020 2020 204e 2903 da0d 6c69 6e65 5f70       N)...line_p
+00001570: 6f73 6974 696f 6e72 7500 0000 7276 0000  ositionru...rv..
+00001580: 0029 0472 3800 0000 727b 0000 0072 7500  .).r8...r{...ru.
+00001590: 0000 7276 0000 0072 4700 0000 7247 0000  ..rv...rG...rG..
+000015a0: 0072 4800 0000 7249 0000 00b8 0000 0073  .rH...rI.......s
+000015b0: 0600 0000 0006 0601 0601 7a0d 4c69 6e65  ..........z.Line
+000015c0: 2e5f 5f69 6e69 745f 5f4e 7277 0000 0072  .__init__Nrw...r
+000015d0: 4700 0000 7247 0000 0072 4700 0000 7248  G...rG...rG...rH
+000015e0: 0000 0072 7900 0000 b700 0000 7302 0000  ...ry.......s...
+000015f0: 0008 0172 7900 0000 6301 0000 0000 0000  ...ry...c.......
+00001600: 0000 0000 0001 0000 0005 0000 0043 0000  .............C..
+00001610: 0073 0e00 0000 6401 a000 7c00 6402 6402  .s....d...|.d.d.
+00001620: a103 5300 2903 4e7a 743c 7061 7261 2061  ..S.).Nzt<para a
+00001630: 7574 6f4c 6561 6469 6e67 3d22 6f66 6622  utoLeading="off"
+00001640: 2066 6f6e 7453 697a 653d 3132 3e54 6869   fontSize=12>Thi
+00001650: 7320 266c 743b 696d 672f 2667 743b 203c  s &lt;img/&gt; <
+00001660: 696d 670a 7372 633d 227b 307d 2220 7661  img.src="{0}" va
+00001670: 6c69 676e 3d22 746f 7022 2077 6964 7468  lign="top" width
+00001680: 3d22 7b31 7d22 2068 6569 6768 743d 227b  ="{1}" height="{
+00001690: 327d 222f 3e20 3c2f 7061 7261 3ee9 6400  2}"/> </para>.d.
+000016a0: 0000 a901 da06 666f 726d 6174 2901 5a08  ......format).Z.
+000016b0: 696d 675f 7061 7468 7247 0000 0072 4700  img_pathrG...rG.
+000016c0: 0000 7248 0000 00da 0767 6574 5f69 6d67  ..rH.....get_img
+000016d0: c300 0000 7306 0000 0000 0604 0106 ff72  ....s..........r
+000016e0: 7f00 0000 6302 0000 0000 0000 0000 0000  ....c...........
+000016f0: 0016 0000 0009 0000 0043 0000 0073 0203  .........C...s..
+00001700: 0000 7c01 6400 7500 720c 6700 7d01 7c01  ..|.d.u.r.g.}.|.
+00001710: 4400 5d0e 7d02 7400 a001 7c02 a101 0100  D.].}.t...|.....
+00001720: 7110 6700 7d03 7402 7c00 8301 4400 5de8  q.g.}.t.|...D.].
+00001730: 5c02 7d04 7d05 7403 7c05 7404 8302 72f8  \.}.}.t.|.t...r.
+00001740: 6700 7d06 7402 7c05 6a05 8301 4400 5d9e  g.}.t.|.j...D.].
+00001750: 5c02 7d07 7d08 7406 8300 7d09 7c08 6a07  \.}.}.t...}.|.j.
+00001760: 726a 7c08 6a07 7c09 5f08 6e0e 7c05 6a07  rj|.j.|._.n.|.j.
+00001770: 7278 7c05 6a07 7c09 5f08 7c08 6a09 7288  rx|.j.|._.|.j.r.
+00001780: 7c08 6a09 7c09 5f0a 6e0e 7c05 6a09 7296  |.j.|._.n.|.j.r.
+00001790: 7c05 6a09 7c09 5f0a 7403 7c08 6a0b 740c  |.j.|._.t.|.j.t.
+000017a0: 8302 72b8 740d 7c08 6a0b 7c08 6a0e 7c08  ..r.t.|.j.|.j.|.
+000017b0: 6a0f 6401 8d03 7d0a 6e28 7403 7c08 6a0b  j.d...}.n(t.|.j.
+000017c0: 7410 8302 72da 7411 6402 a012 7c08 6a0b  t...r.t.d...|.j.
+000017d0: 6403 a102 7c09 8302 7d0a 6e06 7c08 6a0b  d...|...}.n.|.j.
+000017e0: 7d0a 7c06 a013 7c0a a101 0100 714c 7c03  }.|...|.....qL|.
+000017f0: a013 7c06 a101 0100 712c 7414 6404 8301  ..|.....q,t.d...
+00001800: 0100 7414 7c05 8301 0100 7c03 a013 7c05  ..t.|.....|...|.
+00001810: 6701 a101 0100 712c 7415 8300 7d0b 7402  g.....q,t...}.t.
+00001820: 7c00 8301 4400 9001 5dc4 5c02 7d04 7d05  |...D...].\.}.}.
+00001830: 7403 7c05 7404 8302 9001 7224 7402 7c05  t.|.t.....r$t.|.
+00001840: 6a05 8301 4400 9001 5da0 5c02 7d07 7d0c  j...D...].\.}.}.
+00001850: 6405 7d0d 6400 7d0e 7c0c 6a16 9001 726a  d.}.d.}.|.j...rj
+00001860: 6406 7d0d 7c0c 6a16 7d0e 6e12 7c05 6a16  d.}.|.j.}.n.|.j.
+00001870: 9001 727c 6406 7d0d 7c05 6a16 7d0e 7c0d  ..r|d.}.|.j.}.|.
+00001880: 9001 729a 7c0b a017 6407 7c07 7c04 6602  ..r.|...d.|.|.f.
+00001890: 7c07 7c04 6602 7c0e a104 0100 6405 7d0d  |.|.f.|.....d.}.
+000018a0: 6400 7d0f 6400 7d10 7c0c 6a18 9001 72c4  d.}.d.}.|.j...r.
+000018b0: 6406 7d0d 7c0c 6a18 6a19 7d0f 7c0c 6a18  d.}.|.j.j.}.|.j.
+000018c0: 6a1a 7d10 6e1c 7c05 6a18 9001 72e0 6406  j.}.n.|.j...r.d.
+000018d0: 7d0d 7c05 6a18 6a19 7d0f 7c05 6a18 6a1a  }.|.j.j.}.|.j.j.
+000018e0: 7d10 7c0d 9002 7200 7c0b a017 6408 7c07  }.|...r.|...d.|.
+000018f0: 7c04 6602 7c07 7c04 6602 7c10 7c0f a105  |.f.|.|.f.|.|...
+00001900: 0100 6405 7d0d 6400 7d11 6400 7d12 6400  ..d.}.d.}.d.}.d.
+00001910: 7d13 7c0c 6a1b 9002 7236 6406 7d0d 7c0c  }.|.j...r6d.}.|.
+00001920: 6a1b 6a19 7d11 7c0c 6a1b 6a1a 7d12 7c0c  j.j.}.|.j.j.}.|.
+00001930: 6a1b 6a1c 7d13 6e24 7c05 6a1b 9002 725a  j.j.}.n$|.j...rZ
+00001940: 6406 7d0d 7c05 6a1b 6a19 7d11 7c05 6a1b  d.}.|.j.j.}.|.j.
+00001950: 6a1a 7d12 7c05 6a1b 6a1c 7d13 7c0d 9002  j.}.|.j.j.}.|...
+00001960: 727a 7c0b a017 7c13 7c07 7c04 6602 7c07  rz|...|.|.|.f.|.
+00001970: 7c04 6602 7c12 7c11 a105 0100 7c05 6a1d  |.f.|.|.....|.j.
+00001980: 9002 7298 7c0b a017 6409 7c07 7c04 6602  ..r.|...d.|.|.f.
+00001990: 640a 7c04 6602 a103 0100 6405 7d0d 6400  d.|.f.....d.}.d.
+000019a0: 7d14 7c0c 6a1e 9002 72b4 6406 7d0d 7c0c  }.|.j...r.d.}.|.
+000019b0: 6a1e 7d14 6e12 7c05 6a1e 9002 72c6 6406  j.}.n.|.j...r.d.
+000019c0: 7d0d 7c05 6a1e 7d14 7c0d 9001 7244 7c0b  }.|.j.}.|...rD|.
+000019d0: a017 640b 7c07 7c04 6602 7c07 7c04 6602  ..d.|.|.f.|.|.f.
+000019e0: 7c14 a104 0100 9001 7144 9001 7124 741f  |.......qD..q$t.
+000019f0: 7c03 8301 7d15 7c15 a020 7c0b a101 0100  |...}.|.. |.....
+00001a00: 7c15 5300 290c 4e29 0272 2000 0000 7221  |.S.).N).r ...r!
+00001a10: 0000 007a 027b 7d7a 034e 2f41 7a0e 534f  ...z.{}z.N/Az.SO
+00001a20: 4d45 5448 494e 4720 454c 5345 4654 da0a  METHING ELSEFT..
+00001a30: 4241 434b 4752 4f55 4e44 da04 4752 4944  BACKGROUND..GRID
+00001a40: da04 5350 414e e9ff ffff ffda 0656 414c  ..SPAN.......VAL
+00001a50: 4947 4e29 2172 0a00 0000 da0c 7265 6769  IGN)!r......regi
+00001a60: 7374 6572 466f 6e74 da09 656e 756d 6572  sterFont..enumer
+00001a70: 6174 6572 4b00 0000 7262 0000 0072 6300  aterK...rb...rc.
+00001a80: 0000 722b 0000 0072 6800 0000 da09 616c  ..r+...rh.....al
+00001a90: 6967 6e6d 656e 7472 6700 0000 da09 7465  ignmentrg.....te
+00001aa0: 7874 436f 6c6f 7272 7000 0000 7203 0000  xtColorrp...r...
+00001ab0: 0072 0400 0000 7271 0000 0072 7200 0000  .r....rq...rr...
+00001ac0: da03 7374 7272 0f00 0000 727e 0000 0072  ..strr....r~...r
+00001ad0: 4d00 0000 da05 7072 696e 7472 1100 0000  M.....printr....
+00001ae0: 7266 0000 00da 0361 6464 7265 0000 0072  rf.....addre...r
+00001af0: 7600 0000 7275 0000 0072 6400 0000 727b  v...ru...rd...r{
+00001b00: 0000 0072 6900 0000 726a 0000 0072 1000  ...ri...rj...r..
+00001b10: 0000 da08 7365 7453 7479 6c65 2916 da04  ....setStyle)...
+00001b20: 6461 7461 da05 666f 6e74 73da 0466 6f6e  data..fonts..fon
+00001b30: 745a 0a74 6162 6c65 5f64 6174 615a 0772  tZ.table_dataZ.r
+00001b40: 6f77 5f63 7472 5a07 726f 775f 6f62 6a5a  ow_ctrZ.row_objZ
+00001b50: 0c63 6f6c 756d 6e5f 6669 6e61 6c5a 0763  .column_finalZ.c
+00001b60: 6f6c 5f63 7472 da03 636f 6cda 0573 7479  ol_ctr..col..sty
+00001b70: 6c65 5a04 5f63 6f6c 5a0c 7461 626c 655f  leZ._colZ.table_
+00001b80: 7374 796c 6573 5a07 636f 6c5f 6f62 6a5a  stylesZ.col_objZ
+00001b90: 0b61 7070 6c79 5f73 7479 6c65 7266 0000  .apply_stylerf..
+00001ba0: 005a 0f67 7269 645f 6c69 6e65 5f63 6f6c  .Z.grid_line_col
+00001bb0: 6f72 5a0f 6772 6964 5f6c 696e 655f 7769  orZ.grid_line_wi
+00001bc0: 6474 6872 7600 0000 7275 0000 0072 7b00  dthrv...ru...r{.
+00001bd0: 0000 726a 0000 00da 0174 7247 0000 0072  ..rj.....trG...r
+00001be0: 4700 0000 7248 0000 00da 1170 6664 5f74  G...rH.....pfd_t
+00001bf0: 6162 6c65 5f62 7569 6c64 6572 cd00 0000  able_builder....
+00001c00: 73ac 0000 0000 0108 0104 0108 010c 0204  s...............
+00001c10: 0110 010a 0104 0112 0106 0506 010a 0106  ................
+00001c20: 0108 0206 010a 0106 0108 030c 0116 010c  ................
+00001c30: 0116 0206 020c 020c 0208 0108 020e 0306  ................
+00001c40: 0112 010c 0414 0104 0204 0108 0104 0108  ................
+00001c50: 0108 0104 0106 0106 0118 0204 0104 0104  ................
+00001c60: 0108 0104 0108 010a 0108 0104 0108 0108  ................
+00001c70: 0106 011a 0204 0104 0104 0104 0108 0104  ................
+00001c80: 0108 0108 010a 0108 0104 0108 0108 0108  ................
+00001c90: 0106 011a 0208 0116 0204 0104 0108 0104  ................
+00001ca0: 0108 0108 0104 0106 0106 0120 0108 010a  ........... ....
+00001cb0: 0172 9300 0000 630a 0000 0000 0000 0000  .r....c.........
+00001cc0: 0000 0010 0000 0008 0000 0043 0000 0073  ...........C...s
+00001cd0: 8e01 0000 7c08 a000 7401 a101 0100 7402  ....|...t.....t.
+00001ce0: 7236 7403 a004 7402 a101 7d0a 7405 7c0a  r6t...t...}.t.|.
+00001cf0: 8301 7d0b 7c08 6a06 7c0b 7c00 7c01 7c04  ..}.|.j.|.|.|.|.
+00001d00: 7c05 6401 6402 8d06 0100 7407 7c05 1800  |.d.d.....t.|...
+00001d10: 6403 1800 7d03 7c06 72a2 7c08 a008 6404  d...}.|.r.|...d.
+00001d20: 6405 a102 0100 6406 7d0c 7c06 4400 5d46  d.....d.}.|.D.]F
+00001d30: 7d0d 7c0d 725a 7c0c 6406 6b02 727e 7c08  }.|.rZ|.d.k.r~|.
+00001d40: a009 740a 7c03 7c0d a00b a100 a103 0100  ..t.|.|.........
+00001d50: 6e1a 7c03 6407 3800 7d03 7c08 a009 740a  n.|.d.8.}.|...t.
+00001d60: 7c03 7c0d a00b a100 a103 0100 7c0c 6408  |.|.........|.d.
+00001d70: 3700 7d0c 715a 7c02 72c2 7c03 6407 3800  7.}.qZ|.r.|.d.8.
+00001d80: 7d03 7c08 a00c 740a 7c03 740d 740a 1800  }.|...t.|.t.t...
+00001d90: 7c03 a104 0100 6409 7d0e 640a 7c09 6a0e  |.....d.}.d.|.j.
+00001da0: 1600 7d0f 7c08 a00f 640b 7c0e 640c 7c0f  ..}.|...d.|.d.|.
+00001db0: 1700 640c 1700 a103 0100 7c07 9001 7262  ..d.......|...rb
+00001dc0: 7c08 a008 6404 6409 a102 0100 7c0e 640d  |...d.d.....|.d.
+00001dd0: 7410 7c07 8301 6407 1400 1700 3700 7d0e  t.|...d.....7.}.
+00001de0: 6406 7d0c 7c07 4400 5d4c 7d0d 7c0d 9001  d.}.|.D.]L}.|...
+00001df0: 7214 7c0c 6406 6b02 9001 723c 7c08 a009  r.|.d.k...r<|...
+00001e00: 740a 7c0e 7c0d a00b a100 a103 0100 6e1a  t.|.|.........n.
+00001e10: 7c0e 6407 3800 7d0e 7c08 a009 740a 7c0e  |.d.8.}.|...t.|.
+00001e20: 7c0d a00b a100 a103 0100 7c0c 6408 3700  |.........|.d.7.
+00001e30: 7d0c 9001 7114 7411 9001 7276 7c08 a00f  }...q.t...rv|...
+00001e40: 640e 6409 7411 a103 0100 7c08 a00c 740a  d.d.t.....|...t.
+00001e50: 640f 740d 740a 1700 640f a104 0100 6400  d.t.t...d.....d.
+00001e60: 5300 2910 4eda 0461 7574 6f29 0372 2000  S.).N..auto).r .
+00001e70: 0000 7221 0000 00da 046d 6173 6b72 1900  ..r!.....maskr..
+00001e80: 0000 da08 4e6f 746f 5361 6e73 e909 0000  ....NotoSans....
+00001e90: 0072 0100 0000 721e 0000 0072 1600 0000  .r....r....r....
+00001ea0: 721a 0000 007a 0225 6469 2701 0000 fa01  r....z.%di'.....
+00001eb0: 2de9 0500 0000 69fb 0100 0072 1f00 0000  -.....i....r....
+00001ec0: 2912 da08 7365 7454 6974 6c65 722c 0000  )...setTitler,..
+00001ed0: 0072 2900 0000 7230 0000 0072 3100 0000  .r)...r0...r1...
+00001ee0: 7209 0000 00da 0964 7261 7749 6d61 6765  r......drawImage
+00001ef0: 7233 0000 00da 0773 6574 466f 6e74 da0a  r3.....setFont..
+00001f00: 6472 6177 5374 7269 6e67 da0c 4241 5349  drawString..BASI
+00001f10: 435f 4d41 5247 494e da05 7374 7269 7072  C_MARGIN..stripr
+00001f20: 6400 0000 7234 0000 00da 0470 6167 65da  d...r4.....page.
+00001f30: 1164 7261 7743 656e 7472 6564 5374 7269  .drawCentredStri
+00001f40: 6e67 726b 0000 0072 2a00 0000 2910 723a  ngrk...r*...).r:
+00001f50: 0000 0072 3b00 0000 723c 0000 0072 4200  ...r;...r<...rB.
+00001f60: 0000 723f 0000 0072 4000 0000 723d 0000  ..r?...r@...r=..
+00001f70: 0072 3e00 0000 da06 6361 6e76 6173 722f  .r>.....canvasr/
+00001f80: 0000 0072 4100 0000 5a07 7069 6c5f 696d  ...rA...Z.pil_im
+00001f90: 6772 4300 0000 7244 0000 005a 0862 6f74  grC...rD...Z.bot
+00001fa0: 746f 6d5f 795a 1070 6167 655f 6e75 6d62  tom_yZ.page_numb
+00001fb0: 6572 5f74 6578 7472 4700 0000 7247 0000  er_textrG...rG..
+00001fc0: 0072 4800 0000 7235 0000 003d 0100 0073  .rH...r5...=...s
+00001fd0: 5600 0000 0002 0a03 0401 0a01 0801 0401  V...............
+00001fe0: 0201 0201 0201 0201 0201 02fa 060a 0c01  ................
+00001ff0: 0401 0c01 0401 0801 0401 0801 1402 0801  ................
+00002000: 1201 0a02 0401 0801 1403 0402 0a01 1603  ................
+00002010: 0601 0c01 1401 0401 0801 0601 0a01 1402  ................
+00002020: 0801 1201 0c03 0601 0e02 7235 0000 0063  ..........r5...c
+00002030: 0000 0000 0000 0000 0000 0000 0200 0000  ................
+00002040: 0800 0000 4300 0000 7352 0000 0074 0083  ....C...sR...t..
+00002050: 007d 007c 0064 0119 007d 0174 017c 015f  .}.|.d...}.t.|._
+00002060: 0274 03a0 0474 0564 0274 066a 07a0 0874  .t...t.d.t.j...t
+00002070: 0964 03a1 0283 02a1 0101 0074 03a0 0474  .d.........t...t
+00002080: 0564 0474 066a 07a0 0874 0964 05a1 0283  .d.t.j...t.d....
+00002090: 02a1 0101 0064 027c 015f 0a7c 0153 0029  .....d.|._.|.S.)
+000020a0: 064e da08 426f 6479 5465 7874 7296 0000  .N..BodyTextr...
+000020b0: 007a 1a66 6f6e 7473 2f4e 6f74 6f53 616e  .z.fonts/NotoSan
+000020c0: 732d 5265 6775 6c61 722e 7474 665a 0c4e  s-Regular.ttfZ.N
+000020d0: 6f74 6f53 616e 7342 6f6c 647a 1766 6f6e  otoSansBoldz.fon
+000020e0: 7473 2f4e 6f74 6f53 616e 732d 426f 6c64  ts/NotoSans-Bold
+000020f0: 2e74 7466 290b 7208 0000 00da 0e42 4f44  .ttf).r......BOD
+00002100: 595f 464f 4e54 5f53 495a 45da 0866 6f6e  Y_FONT_SIZE..fon
+00002110: 7453 697a 6572 0a00 0000 7285 0000 0072  tSizer....r....r
+00002120: 0b00 0000 da02 6f73 da04 7061 7468 da04  ......os..path..
+00002130: 6a6f 696e da0c 5f5f 6c6f 6361 7469 6f6e  join..__location
+00002140: 5f5f da08 666f 6e74 4e61 6d65 2902 5a12  __..fontName).Z.
+00002150: 7361 6d70 6c65 5f73 7479 6c65 5f73 6865  sample_style_she
+00002160: 6574 5a0a 626f 6479 5f73 7479 6c65 7247  etZ.body_stylerG
+00002170: 0000 0072 4700 0000 7248 0000 0072 2b00  ...rG...rH...r+.
+00002180: 0000 7b01 0000 730e 0000 0000 0106 0108  ..{...s.........
+00002190: 0106 011a 011a 0106 0172 2b00 0000 6301  .........r+...c.
+000021a0: 0000 0000 0000 0000 0000 0005 0000 0004  ................
+000021b0: 0000 0043 0000 0073 3e00 0000 6401 7d01  ...C...s>...d.}.
+000021c0: 7400 7c00 8301 4400 5d2c 5c02 7d02 7d03  t.|...D.],\.}.}.
+000021d0: 7401 7c03 7402 8302 7228 7403 7c03 6a04  t.|.t...r(t.|.j.
+000021e0: 8301 6e02 6402 7d04 7c04 7c01 6b04 720c  ..n.d.}.|.|.k.r.
+000021f0: 7c04 7d01 710c 7c01 5300 2903 4e72 0100  |.}.q.|.S.).Nr..
+00002200: 0000 7216 0000 0029 0572 8600 0000 724b  ..r....).r....rK
+00002210: 0000 0072 6200 0000 726b 0000 0072 6300  ...rb...rk...rc.
+00002220: 0000 2905 728d 0000 005a 0f6d 6178 5f6e  ..).r....Z.max_n
+00002230: 756d 5f6f 665f 636f 6c73 5a0b 726f 775f  um_of_colsZ.row_
+00002240: 636f 756e 7465 72da 0372 6f77 5a0b 6e75  counter..rowZ.nu
+00002250: 6d5f 6f66 5f63 6f6c 7372 4700 0000 7247  m_of_colsrG...rG
+00002260: 0000 0072 4800 0000 da17 6669 6e64 5f6d  ...rH.....find_m
+00002270: 6178 5f6e 756d 5f6f 665f 636f 6c75 6d6e  ax_num_of_column
+00002280: 7385 0100 0073 0c00 0000 0001 0401 1001  s....s..........
+00002290: 1801 0801 0601 72ac 0000 0063 0100 0000  ......r....c....
+000022a0: 0000 0000 0000 0000 0100 0000 0300 0000  ................
+000022b0: 4300 0000 730a 0000 0064 01a0 007c 00a1  C...s....d...|..
+000022c0: 0153 0029 024e 7a03 7b7d 3a72 7d00 0000  .S.).Nz.{}:r}...
+000022d0: 2901 da05 7061 7261 6d72 4700 0000 7247  )...paramrG...rG
+000022e0: 0000 0072 4800 0000 da0c 6170 7065 6e64  ...rH.....append
+000022f0: 5f63 6f6c 6f6e 8e01 0000 7302 0000 0000  _colon....s.....
+00002300: 0172 ae00 0000 2901 4e29 4172 5900 0000  .r....).N)ArY...
+00002310: 72a6 0000 00da 0966 756e 6374 6f6f 6c73  r......functools
+00002320: 7202 0000 0072 0300 0000 da03 5049 4c72  r....r......PILr
+00002330: 0400 0000 7230 0000 00da 0d72 6570 6f72  ....r0.....repor
+00002340: 746c 6162 2e6c 6962 7205 0000 00da 1372  tlab.libr......r
+00002350: 6570 6f72 746c 6162 2e6c 6962 2e65 6e75  eportlab.lib.enu
+00002360: 6d73 7206 0000 00da 1772 6570 6f72 746c  msr......reportl
+00002370: 6162 2e6c 6962 2e70 6167 6573 697a 6573  ab.lib.pagesizes
+00002380: 7207 0000 00da 1472 6570 6f72 746c 6162  r......reportlab
+00002390: 2e6c 6962 2e73 7479 6c65 7372 0800 0000  .lib.stylesr....
+000023a0: da13 7265 706f 7274 6c61 622e 6c69 622e  ..reportlab.lib.
+000023b0: 7574 696c 7372 0900 0000 da11 7265 706f  utilsr......repo
+000023c0: 7274 6c61 622e 7064 6662 6173 6572 0a00  rtlab.pdfbaser..
+000023d0: 0000 5a19 7265 706f 7274 6c61 622e 7064  ..Z.reportlab.pd
+000023e0: 6662 6173 652e 7474 666f 6e74 7372 0b00  fbase.ttfontsr..
+000023f0: 0000 da12 7265 706f 7274 6c61 622e 706c  ....reportlab.pl
+00002400: 6174 7970 7573 720c 0000 0072 0d00 0000  atypusr....r....
+00002410: 720e 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
+00002420: 1100 0000 5a19 7064 665f 7461 626c 655f  ....Z.pdf_table_
+00002430: 6275 696c 6465 722e 6865 6c70 6572 7372  builder.helpersr
+00002440: 1200 0000 da06 7374 796c 6573 5a06 7374  ......stylesZ.st
+00002450: 796c 654e 5a06 7374 796c 6548 5a13 4445  yleNZ.styleHZ.DE
+00002460: 5349 5245 445f 5048 4f54 4f5f 5749 4454  SIRED_PHOTO_WIDT
+00002470: 485a 1444 4553 4952 4544 5f50 484f 544f  HZ.DESIRED_PHOTO
+00002480: 5f48 4549 4748 5472 9e00 0000 72a4 0000  _HEIGHTr....r...
+00002490: 0072 3400 0000 7233 0000 005a 064c 494e  .r4...r3...Z.LIN
+000024a0: 455f 595a 0846 5241 4d45 5f58 315a 0846  E_YZ.FRAME_X1Z.F
+000024b0: 5241 4d45 5f59 3172 2a00 0000 7229 0000  RAME_Y1r*...r)..
+000024c0: 0072 2d00 0000 722c 0000 0072 a700 0000  .r-...r,...r....
+000024d0: da08 7265 616c 7061 7468 72a8 0000 00da  ..realpathr.....
+000024e0: 0667 6574 6377 64da 0764 6972 6e61 6d65  .getcwd..dirname
+000024f0: da08 5f5f 6669 6c65 5f5f 72a9 0000 0072  ..__file__r....r
+00002500: 1c00 0000 7262 0000 0072 6d00 0000 7273  ....rb...rm...rs
+00002510: 0000 0072 7900 0000 727f 0000 0072 9300  ...ry...r....r..
+00002520: 0000 7235 0000 0072 2b00 0000 72ac 0000  ..r5...r+...r...
+00002530: 0072 ae00 0000 7247 0000 0072 4700 0000  .r....rG...rG...
+00002540: 7247 0000 0072 4800 0000 da08 3c6d 6f64  rG...rH.....<mod
+00002550: 756c 653e 0100 0000 7356 0000 0008 0108  ule>....sV......
+00002560: 010c 010c 020c 010c 010c 010c 010c 010c  ................
+00002570: 010c 010c 0110 0110 0114 020c 0206 0108  ................
+00002580: 0108 020c 0110 0204 0104 0108 0108 0104  ................
+00002590: 0204 0104 0204 0104 0104 0104 0122 030e  ............."..
+000025a0: 5c0e 100e 1a0e 060e 0c08 0a0a 7008 3e08  \...........p.>.
+000025b0: 0a08 09                                  ...
```

### Comparing `reportlab-pdf-table-builder-1.2.3/pdf_table_builder/__pycache__/helpers.cpython-38.pyc` & `reportlab-pdf-table-builder-1.2.4/pdf_table_builder/__pycache__/helpers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `reportlab-pdf-table-builder-1.2.3/pdf_table_builder/__pycache__/helpers.cpython-39.pyc` & `reportlab-pdf-table-builder-1.2.4/pdf_table_builder/__pycache__/helpers.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `reportlab-pdf-table-builder-1.2.3/pdf_table_builder/builder.py` & `reportlab-pdf-table-builder-1.2.4/pdf_table_builder/builder.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 styleH = styles['Heading1']
 
 DESIRED_PHOTO_WIDTH = A4[0] - 160
 DESIRED_PHOTO_HEIGHT = A4[1] / 2 - 170
 
 BASIC_MARGIN = 30
 BODY_FONT_SIZE = 8
-PAGE_WIDTH = 530
-PAGE_HEIGHT = 750
+PAGE_WIDTH = A4[0]
+PAGE_HEIGHT = A4[1]
 LINE_Y = 730
 
 FRAME_X1 = 30
 FRAME_Y1 = 30
 
 WATERMARK = None
 LOGO_PATH = None
@@ -40,40 +40,73 @@
 __location__ = os.path.realpath(os.path.join(os.getcwd(), os.path.dirname(__file__)))
 
 
 class ReportLabPDFBuilder:
 
     def __init__(self, logo_path=None, watermark=None, pdf_tab_title=PDF_TAB_TITLE, logo_base_width=LOGO_BASE_WIDTH,
                  logo_canvas_x=0, logo_canvas_y=0, frame_left_padding=30, frame_right_padding=30, frame_top_padding=30,
-                 frame_bottom_padding=30):
+                 frame_bottom_padding=30, have_header_bottom_line=True, company_info=None, footer_text=None, ):
         global WATERMARK
         global LOGO_PATH
         global BODY_STYLE
         global PDF_TAB_TITLE
         global LOGO_BASE_WIDTH
 
         LOGO_PATH = logo_path
         WATERMARK = watermark
         BODY_STYLE = get_body_style()
         PDF_TAB_TITLE = pdf_tab_title
         LOGO_BASE_WIDTH = logo_base_width
 
         self.pdf_buffer = BytesIO()
         self.pdf = BaseDocTemplate(self.pdf_buffer, pagesize=A4)
+
+        logo_print_width = 0
+        logo_print_height = 0
+        if LOGO_PATH:
+            im = pilim.open(LOGO_PATH)
+            logo_print_width, logo_print_height = calculate_image_dimensions_and_keep_aspect_ratio(
+                img_width=im.size[0],
+                img_height=im.size[1],
+                img_desired_width=LOGO_BASE_WIDTH
+            )
+
+        top_y = PAGE_HEIGHT - logo_print_height - 30
+        if company_info:
+            i = 0
+            for value in company_info:
+                if value:
+                    if i > 0:
+                        top_y -= 12
+                    i += 1
+
+        if have_header_bottom_line:
+            top_y -= 12
+
         frame = Frame(
-            FRAME_X1,
-            FRAME_Y1,
+            0,
+            0 - (PAGE_HEIGHT - top_y) + 20,
             width=PAGE_WIDTH,
             height=PAGE_HEIGHT,
             leftPadding=frame_left_padding,
             bottomPadding=frame_bottom_padding,
             rightPadding=frame_right_padding,
             topPadding=frame_top_padding
         )
-        header_and_footer_partial = partial(header_and_footer, logo_canvas_x, logo_canvas_y)
+        header_and_footer_partial = partial(
+            header_and_footer,
+            logo_canvas_x,
+            logo_canvas_y,
+            have_header_bottom_line,
+            top_y,
+            logo_print_width,
+            logo_print_height,
+            company_info,
+            footer_text
+        )
         template = PageTemplate(id='all_pages', frames=frame, onPage=header_and_footer_partial)
         self.pdf.addPageTemplates([template])
         self.story = []
 
     def add_to_story(self, obj):
         if isinstance(obj, list):
             for x in obj:
@@ -83,14 +116,19 @@
 
     def get_pdf_value(self):
         self.pdf.build(self.story)
         pdf_value = self.pdf_buffer.getvalue()
         self.pdf_buffer.close()
         return pdf_value
 
+    def get_pdf_buffer(self):
+        self.pdf.build(self.story)
+        self.pdf_buffer.close()
+        return self.pdf_buffer
+
     def save_pdf_file(self, file_name):
         self.pdf.build(self.story)
         with open(file_name, "wb") as f:
             self.pdf_buffer.seek(io.SEEK_SET)
             f.writelines(self.pdf_buffer)
 
 
@@ -140,14 +178,19 @@
     def __init__(self, line_width=0.5, line_color=colors.gray):
         self.line_width = line_width
         self.line_color = line_color
 
 
 class Line:
     def __init__(self, line_position='LINEBELOW', line_width=0.5, line_color=colors.gray):
+        """
+        :param line_position: Can be LINEBELOW, LINEABOVE, LINEBEFORE, LINEAFTER
+        :param line_width: Can be 0.5, 1, 2 etc.
+        :param line_color: Can be colors.gray, colors.black etc. or HEX color like '#000000'.
+        """
         self.line_position = line_position
         self.line_width = line_width
         self.line_color = line_color
 
 
 def get_img(img_path):
     # buff1 = BytesIO()
@@ -187,21 +230,23 @@
 
                 # print("type:", type(col.content))
                 if isinstance(col.content, BytesIO):
                     _col = Image(col.content, width=col.image_width, height=col.image_height)
                 elif isinstance(col.content, str):
                     _col = Paragraph('{}'.format(col.content, 'N/A'), style)
                 else:
-                    # print("SOMETHING ELSE")
                     _col = col.content
 
                 column_final.append(_col)
 
             table_data.append(column_final)
         else:
+            print("SOMETHING ELSE")
+            print(row_obj)
+
             table_data.append([row_obj])
 
     # ------------------ STYLE
     table_styles = TableStyle()
     for row_ctr, row_obj in enumerate(data):
         if isinstance(row_obj, Row):
             # Loop through all the cells and apply the styles on cell level if declared
@@ -255,55 +300,80 @@
                     table_styles.add('SPAN', (col_ctr, row_ctr), (-1, row_ctr))
                 # VALIGN
                 apply_style = False
                 valign = None
                 if col_obj.valign:
                     apply_style = True
                     valign = col_obj.valign
-                    print('COL:', valign)
                 elif row_obj.valign:
                     apply_style = True
                     valign = row_obj.valign
-                    print('ROW:', valign)
                 if apply_style:
                     table_styles.add('VALIGN', (col_ctr, row_ctr), (col_ctr, row_ctr), valign)
     t = Table(table_data)
     t.setStyle(table_styles)
     return t
 
 
-def header_and_footer(logo_canvas_x, logo_canvas_y, canvas, pdf):
+def header_and_footer(logo_canvas_x, logo_canvas_y, have_header_bottom_line, top_y, logo_print_width, logo_print_height,
+                      company_info, footer_text, canvas, pdf):
     canvas.setTitle(PDF_TAB_TITLE)
 
     # LOGO
     if LOGO_PATH:
         im = pilim.open(LOGO_PATH)
-        print_width, print_height = calculate_image_dimensions_and_keep_aspect_ratio(
-            img_width=im.size[0],
-            img_height=im.size[1],
-            img_desired_width=LOGO_BASE_WIDTH
-        )
         pil_img = ImageReader(im)
         canvas.drawImage(
             pil_img,
             logo_canvas_x,
             logo_canvas_y,
-            width=print_width,
-            height=print_height,
+            width=logo_print_width,
+            height=logo_print_height,
             mask='auto'
         )
 
-    # canvas.line(BASIC_MARGIN, LINE_Y, PAGE_WIDTH + BASIC_MARGIN, LINE_Y)
+    # COMPANY'S INFO
+    top_y = PAGE_HEIGHT - logo_print_height - 30
+    if company_info:
+        canvas.setFont('NotoSans', 9)
+        i = 0
+        for value in company_info:
+            if value:
+                if i == 0:
+                    canvas.drawString(BASIC_MARGIN, top_y, value.strip())
+                else:
+                    top_y -= 12
+                    canvas.drawString(BASIC_MARGIN, top_y, value.strip())
+                i += 1
+
+    if have_header_bottom_line:
+        top_y -= 12
+        canvas.line(BASIC_MARGIN, top_y, PAGE_WIDTH - BASIC_MARGIN, top_y)
 
     # ----------------------- FOOTER ----------------------- #
-    canvas.setFont('Helvetica-Bold', 8)
-    # page number
+    bottom_y = 8
+    # Page number.
     page_number_text = "%d" % pdf.page
-    canvas.drawCentredString(295, 8, '-' + page_number_text + '-')
-    # watermark
+    canvas.drawCentredString(295, bottom_y, '-' + page_number_text + '-')
+
+    # Footer text.
+    if footer_text:
+        canvas.setFont('NotoSans', 8)
+        bottom_y += 5 + (len(footer_text) * 12)
+        i = 0
+        for value in footer_text:
+            if value:
+                if i == 0:
+                    canvas.drawString(BASIC_MARGIN, bottom_y, value.strip())
+                else:
+                    bottom_y -= 12
+                    canvas.drawString(BASIC_MARGIN, bottom_y, value.strip())
+                i += 1
+
+    # Watermark.
     if WATERMARK:
         canvas.drawCentredString(507, 8, WATERMARK)
 
     canvas.line(BASIC_MARGIN, 20, PAGE_WIDTH + BASIC_MARGIN, 20)
 
 
 def get_body_style():
```

### Comparing `reportlab-pdf-table-builder-1.2.3/pdf_table_builder/consts.py` & `reportlab-pdf-table-builder-1.2.4/pdf_table_builder/consts.py`

 * *Files identical despite different names*

### Comparing `reportlab-pdf-table-builder-1.2.3/pdf_table_builder/fonts/NotoSans-Bold.ttf` & `reportlab-pdf-table-builder-1.2.4/pdf_table_builder/fonts/NotoSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `reportlab-pdf-table-builder-1.2.3/pdf_table_builder/fonts/NotoSans-Regular.ttf` & `reportlab-pdf-table-builder-1.2.4/pdf_table_builder/fonts/NotoSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `reportlab-pdf-table-builder-1.2.3/pdf_table_builder/helpers.py` & `reportlab-pdf-table-builder-1.2.4/pdf_table_builder/helpers.py`

 * *Files identical despite different names*

### Comparing `reportlab-pdf-table-builder-1.2.3/pdf_table_builder/utils/helpers.py` & `reportlab-pdf-table-builder-1.2.4/pdf_table_builder/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `reportlab-pdf-table-builder-1.2.3/reportlab_pdf_table_builder.egg-info/PKG-INFO` & `reportlab-pdf-table-builder-1.2.4/reportlab_pdf_table_builder.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: reportlab-pdf-table-builder
-Version: 1.2.3
+Version: 1.2.4
 Summary: A simple pdf table builder using the ReportLab Toolkit
 Home-page: https://github.com/timossavva/reportlab-pdf-table-builder
 Author: Timotheos Savva
 Author-email: timotheos.savva12@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -84,9 +82,7 @@
 
 table = pfd_table_builder(data)
 
 pdfbuilder = ReportLabPDFBuilder()
 pdfbuilder.add_to_story(table)
 pdfbuilder.save_pdf_file('a.pdf')
 ```
-
-
```

### Comparing `reportlab-pdf-table-builder-1.2.3/reportlab_pdf_table_builder.egg-info/SOURCES.txt` & `reportlab-pdf-table-builder-1.2.4/reportlab_pdf_table_builder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reportlab-pdf-table-builder-1.2.3/setup.py` & `reportlab-pdf-table-builder-1.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="reportlab-pdf-table-builder",
-    version="1.2.3",
+    version="1.2.4",
     author="Timotheos Savva",
     author_email="timotheos.savva12@gmail.com",
     description="A simple pdf table builder using the ReportLab Toolkit",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/timossavva/reportlab-pdf-table-builder",
     packages=setuptools.find_packages(),
```

