# Comparing `tmp/tja2fumen-0.5.0.tar.gz` & `tmp/tja2fumen-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tja2fumen-0.5.0.tar", last modified: Mon Jul 10 00:07:13 2023, max compression
+gzip compressed data, was "tja2fumen-0.5.1.tar", last modified: Tue Jul 11 12:16:47 2023, max compression
```

## Comparing `tja2fumen-0.5.0.tar` & `tja2fumen-0.5.1.tar`

### file list

```diff
@@ -1,38 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 00:07:13.200594 tja2fumen-0.5.0/
--rw-rw-rw-   0        0        0     1083 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/LICENSE.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4388 2023-07-10 00:07:13.200594 tja2fumen-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     2669 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/README.md
--rw-rw-rw-   0        0        0      897 2023-07-10 00:07:01.000000 tja2fumen-0.5.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-10 00:07:13.200594 tja2fumen-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0       98 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 00:07:13.184971 tja2fumen-0.5.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-10 00:07:13.184971 tja2fumen-0.5.0/src/tja2fumen/
--rw-rw-rw-   0        0        0     1825 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/src/tja2fumen/__init__.py
--rw-rw-rw-   0        0        0     3856 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/src/tja2fumen/constants.py
--rw-rw-rw-   0        0        0    17917 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/src/tja2fumen/converters.py
--rw-rw-rw-   0        0        0    19863 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/src/tja2fumen/parsers.py
-drwxrwxrwx   0        0        0        0 2023-07-10 00:07:13.200594 tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/
--rw-rw-rw-   0        0        0    23889 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Easy-1.csv
--rw-rw-rw-   0        0        0    23889 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Easy-2-3.csv
--rw-rw-rw-   0        0        0    23890 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Easy-4-5.csv
--rw-rw-rw-   0        0        0    23886 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Hard-1-2.csv
--rw-rw-rw-   0        0        0    23884 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Hard-3.csv
--rw-rw-rw-   0        0        0    23884 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Hard-4.csv
--rw-rw-rw-   0        0        0    23883 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Hard-5-8.csv
--rw-rw-rw-   0        0        0    23889 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Normal-1-2.csv
--rw-rw-rw-   0        0        0    23889 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Normal-3.csv
--rw-rw-rw-   0        0        0    23887 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Normal-4.csv
--rw-rw-rw-   0        0        0    23886 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Normal-5-7.csv
--rw-rw-rw-   0        0        0    23880 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Oni-1-7.csv
--rw-rw-rw-   0        0        0    23872 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Oni-8.csv
--rw-rw-rw-   0        0        0    23869 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Oni-9-10.csv
--rw-rw-rw-   0        0        0     3308 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/src/tja2fumen/utils.py
--rw-rw-rw-   0        0        0     2910 2023-07-10 00:06:07.000000 tja2fumen-0.5.0/src/tja2fumen/writers.py
-drwxrwxrwx   0        0        0        0 2023-07-10 00:07:13.184971 tja2fumen-0.5.0/src/tja2fumen.egg-info/
--rw-rw-rw-   0        0        0     4388 2023-07-10 00:07:13.000000 tja2fumen-0.5.0/src/tja2fumen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1017 2023-07-10 00:07:13.000000 tja2fumen-0.5.0/src/tja2fumen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 00:07:13.000000 tja2fumen-0.5.0/src/tja2fumen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-10 00:07:13.000000 tja2fumen-0.5.0/src/tja2fumen.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       47 2023-07-10 00:07:13.000000 tja2fumen-0.5.0/src/tja2fumen.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-10 00:07:13.000000 tja2fumen-0.5.0/src/tja2fumen.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 12:16:47.455071 tja2fumen-0.5.1/
+-rw-rw-rw-   0        0        0     1083 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4388 2023-07-11 12:16:47.455071 tja2fumen-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2669 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/README.md
+-rw-rw-rw-   0        0        0      897 2023-07-11 12:16:33.000000 tja2fumen-0.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-11 12:16:47.455071 tja2fumen-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0       98 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 12:16:47.407547 tja2fumen-0.5.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-11 12:16:47.423106 tja2fumen-0.5.1/src/tja2fumen/
+-rw-rw-rw-   0        0        0     1732 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/__init__.py
+-rw-rw-rw-   0        0        0     3856 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/constants.py
+-rw-rw-rw-   0        0        0    18157 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/converters.py
+-rw-rw-rw-   0        0        0    19863 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/parsers.py
+drwxrwxrwx   0        0        0        0 2023-07-11 12:16:47.455071 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/
+-rw-rw-rw-   0        0        0    20989 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Easy-1.csv
+-rw-rw-rw-   0        0        0    20505 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Easy-2-3.csv
+-rw-rw-rw-   0        0        0    21140 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Easy-4-5.csv
+-rw-rw-rw-   0        0        0    20349 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Hard-1-2.csv
+-rw-rw-rw-   0        0        0    20328 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Hard-3.csv
+-rw-rw-rw-   0        0        0    20390 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Hard-4.csv
+-rw-rw-rw-   0        0        0    20545 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Hard-5-8.csv
+-rw-rw-rw-   0        0        0    20516 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Normal-1-2.csv
+-rw-rw-rw-   0        0        0    20482 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Normal-3.csv
+-rw-rw-rw-   0        0        0    20393 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Normal-4.csv
+-rw-rw-rw-   0        0        0    21000 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Normal-5-7.csv
+-rw-rw-rw-   0        0        0    20458 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Oni-1-7.csv
+-rw-rw-rw-   0        0        0    20435 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Oni-8.csv
+-rw-rw-rw-   0        0        0    20464 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1213_Oni-9-10.csv
+-rw-rw-rw-   0        0        0    20661 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Easy-1.csv
+-rw-rw-rw-   0        0        0    20385 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Easy-2-3.csv
+-rw-rw-rw-   0        0        0    20976 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Easy-4-5.csv
+-rw-rw-rw-   0        0        0    20222 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Hard-1-2.csv
+-rw-rw-rw-   0        0        0    20145 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Hard-3.csv
+-rw-rw-rw-   0        0        0    20136 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Hard-4.csv
+-rw-rw-rw-   0        0        0    20182 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Hard-5-8.csv
+-rw-rw-rw-   0        0        0    20294 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Normal-1-2.csv
+-rw-rw-rw-   0        0        0    20289 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Normal-3.csv
+-rw-rw-rw-   0        0        0    20245 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Normal-4.csv
+-rw-rw-rw-   0        0        0    20715 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Normal-5-7.csv
+-rw-rw-rw-   0        0        0    19707 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Oni-1-7.csv
+-rw-rw-rw-   0        0        0    19785 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Oni-8.csv
+-rw-rw-rw-   0        0        0    19777 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte1617_Oni-9-10.csv
+-rw-rw-rw-   0        0        0    23889 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Easy-1.csv
+-rw-rw-rw-   0        0        0    23889 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Easy-2-3.csv
+-rw-rw-rw-   0        0        0    23890 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Easy-4-5.csv
+-rw-rw-rw-   0        0        0    23886 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Hard-1-2.csv
+-rw-rw-rw-   0        0        0    23884 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Hard-3.csv
+-rw-rw-rw-   0        0        0    23884 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Hard-4.csv
+-rw-rw-rw-   0        0        0    23883 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Hard-5-8.csv
+-rw-rw-rw-   0        0        0    23889 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Normal-1-2.csv
+-rw-rw-rw-   0        0        0    23889 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Normal-3.csv
+-rw-rw-rw-   0        0        0    23887 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Normal-4.csv
+-rw-rw-rw-   0        0        0    23886 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Normal-5-7.csv
+-rw-rw-rw-   0        0        0    23880 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Oni-1-7.csv
+-rw-rw-rw-   0        0        0    23872 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Oni-8.csv
+-rw-rw-rw-   0        0        0    23869 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Oni-9-10.csv
+-rw-rw-rw-   0        0        0     4363 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/utils.py
+-rw-rw-rw-   0        0        0     2910 2023-07-11 12:15:24.000000 tja2fumen-0.5.1/src/tja2fumen/writers.py
+drwxrwxrwx   0        0        0        0 2023-07-11 12:16:47.423106 tja2fumen-0.5.1/src/tja2fumen.egg-info/
+-rw-rw-rw-   0        0        0     4388 2023-07-11 12:16:47.000000 tja2fumen-0.5.1/src/tja2fumen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2559 2023-07-11 12:16:47.000000 tja2fumen-0.5.1/src/tja2fumen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 12:16:47.000000 tja2fumen-0.5.1/src/tja2fumen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-11 12:16:47.000000 tja2fumen-0.5.1/src/tja2fumen.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       47 2023-07-11 12:16:47.000000 tja2fumen-0.5.1/src/tja2fumen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-11 12:16:47.000000 tja2fumen-0.5.1/src/tja2fumen.egg-info/top_level.txt
```

### Comparing `tja2fumen-0.5.0/LICENSE.txt` & `tja2fumen-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.0/PKG-INFO` & `tja2fumen-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tja2fumen
-Version: 0.5.0
+Version: 0.5.1
 Summary: Convert TJA chart files into fumen (.bin) chart files
 License: MIT License
         
         Copyright (c) 2023 Vivaria
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `tja2fumen-0.5.0/README.md` & `tja2fumen-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.0/pyproject.toml` & `tja2fumen-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tja2fumen"
-version = "0.5.0"
+version = "0.5.1"
 description = "Convert TJA chart files into fumen (.bin) chart files"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE.txt"}
 keywords = ["taiko", "tatsujin", "fumen", "TJA"]
 
 [project.urls]  # Optional
```

### Comparing `tja2fumen-0.5.0/src/tja2fumen/__init__.py` & `tja2fumen-0.5.1/src/tja2fumen/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,51 +5,47 @@
 from tja2fumen.parsers import parseTJA
 from tja2fumen.writers import writeFumen
 from tja2fumen.converters import convertTJAToFumen
 from tja2fumen.constants import COURSE_IDS
 
 
 def main(argv=None):
-    # NB: We want to return variables during testing, but not during CLI (or else they will be printed to stderr)
-    if argv:
-        return_vars = True
-    else:
+    if not argv:
         argv = sys.argv[1:]
-        return_vars = False
 
     parser = argparse.ArgumentParser(
         description="tja2fumen"
     )
     parser.add_argument(
         "file.tja",
         help="Path to a Taiko no Tatsujin TJA file.",
     )
     args = parser.parse_args(argv)
     fnameTJA = getattr(args, "file.tja")
+    baseName = os.path.splitext(fnameTJA)[0]
 
-    # Convert TJA data to fumen data
-    parsedSongsTJA = parseTJA(fnameTJA)
-    parsedSongsFumen = {course: convertTJAToFumen(tjaData)
-                        for course, tjaData in parsedSongsTJA.items()}
+    # Parse lines in TJA file
+    parsedTJACourses = parseTJA(fnameTJA)
 
-    # Generate output filenames
-    baseName = os.path.splitext(fnameTJA)[0]
-    outputFilenames = []
-    for courseName, fumenData in parsedSongsFumen.items():
-        if len(parsedSongsTJA) == 1:
-            outputName = f"{baseName}.bin"
-        else:
-            splitName = courseName.split("P")  # e.g. 'OniP2' -> ['Oni', '2'], 'Oni' -> ['Oni']
-            outputName = f"{baseName}_{COURSE_IDS[splitName[0]]}"
-            if len(splitName) == 2:
-                outputName += f"_{splitName[1]}"  # Add "_1" or "_2" if P1/P2 chart
-            outputName += ".bin"
-        outputFilenames.append(outputName)
-        writeFumen(outputName, fumenData)
+    # Convert parsed TJA courses to Fumen data, and write each course to `.bin` files
+    for parsedCourse in parsedTJACourses.items():
+        convert_and_write(parsedCourse, baseName, singleCourse=(len(parsedTJACourses) == 1))
 
-    if return_vars:
-        return parsedSongsTJA, parsedSongsFumen, outputFilenames
+
+def convert_and_write(parsedCourse, baseName, singleCourse=False):
+    courseName, tjaData = parsedCourse
+    fumenData = convertTJAToFumen(tjaData)
+    # Add course ID (e.g. '_x', '_x_1', '_x_2') to the output file's base name
+    outputName = baseName
+    if singleCourse:
+        pass  # Replicate tja2bin.exe behavior by excluding course ID if there's only one course
+    else:
+        splitName = courseName.split("P")  # e.g. 'OniP2' -> ['Oni', '2'], 'Oni' -> ['Oni']
+        outputName += f"_{COURSE_IDS[splitName[0]]}"
+        if len(splitName) == 2:
+            outputName += f"_{splitName[1]}"  # Add "_1" or "_2" if P1/P2 chart
+    writeFumen(f"{outputName}.bin", fumenData)
 
 
 # NB: This entry point is necessary for the Pyinstaller executable
 if __name__ == "__main__":
     main()
```

### Comparing `tja2fumen-0.5.0/src/tja2fumen/constants.py` & `tja2fumen-0.5.1/src/tja2fumen/constants.py`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.0/src/tja2fumen/converters.py` & `tja2fumen-0.5.1/src/tja2fumen/converters.py`

 * *Files 2% similar despite different names*

```diff
@@ -282,19 +282,25 @@
             measureFumen[currentBranch]['length'] = note_counter
             total_notes += note_counter
 
     # Take a stock header metadata sample and add song-specific metadata
     headerMetadata = sampleHeaderMetadata.copy()
     headerMetadata[8] = DIFFICULTY_BYTES[tja['metadata']['course']][0]
     headerMetadata[9] = DIFFICULTY_BYTES[tja['metadata']['course']][1]
-    headerMetadata[20], headerMetadata[21] = computeSoulGaugeBytes(
+    soulGaugeBytes = computeSoulGaugeBytes(
         n_notes=total_notes,
         difficulty=tja['metadata']['course'],
         stars=tja['metadata']['level']
     )
+    headerMetadata[12] = soulGaugeBytes[0]
+    headerMetadata[13] = soulGaugeBytes[1]
+    headerMetadata[16] = soulGaugeBytes[2]
+    headerMetadata[17] = soulGaugeBytes[3]
+    headerMetadata[20] = soulGaugeBytes[4]
+    headerMetadata[21] = soulGaugeBytes[5]
     tjaConverted['headerMetadata'] = b"".join(i.to_bytes(1, 'little') for i in headerMetadata)
     tjaConverted['headerPadding'] = simpleHeaders[0]  # Use a basic, known set of header bytes
     tjaConverted['order'] = '<'
     tjaConverted['unknownMetadata'] = 0
     tjaConverted['branches'] = all([len(b) for b in tja['branches'].values()])
     tjaConverted['scoreInit'] = tja['metadata']['scoreInit']
     tjaConverted['scoreDiff'] = tja['metadata']['scoreDiff']
```

### Comparing `tja2fumen-0.5.0/src/tja2fumen/parsers.py` & `tja2fumen-0.5.1/src/tja2fumen/parsers.py`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Easy-1.csv` & `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Easy-1.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Easy-2-3.csv` & `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Easy-2-3.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Easy-4-5.csv` & `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Easy-4-5.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Hard-1-2.csv` & `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Hard-1-2.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Hard-3.csv` & `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Hard-3.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Hard-4.csv` & `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Hard-4.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Hard-5-8.csv` & `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Hard-5-8.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Normal-1-2.csv` & `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Normal-1-2.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Normal-3.csv` & `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Normal-3.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Normal-4.csv` & `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Normal-4.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Normal-5-7.csv` & `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Normal-5-7.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Oni-1-7.csv` & `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Oni-1-7.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Oni-8.csv` & `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Oni-8.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.0/src/tja2fumen/soulgauge_LUTs/Oni-9-10.csv` & `tja2fumen-0.5.1/src/tja2fumen/soulgauge_LUTs/byte2021_Oni-9-10.csv`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.0/src/tja2fumen/utils.py` & `tja2fumen-0.5.1/src/tja2fumen/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -32,23 +32,45 @@
     elif difficulty == 'Easy':
         if 4 <= stars:
             key = "Easy-4-5"
         elif 2 <= stars <= 3:
             key = "Easy-2-3"
         elif stars <= 1:
             key = "Easy-1"
+    # Set default values for soul gauge bytes.
+    # NB: These will only be used if n_notes > 2500 (i.e. the most extreme, impossible case, beyond all official charts)
+    soulGaugeByte12 = 255
+    soulGaugeByte13 = 3
+    soulGaugeByte16 = 255
+    soulGaugeByte17 = 2
+    soulGaugeByte20 = 255
+    soulGaugeByte21 = 253
     pkg_dir = os.path.dirname(os.path.realpath(__file__))
-    with open(os.path.join(pkg_dir, "soulgauge_LUTs", f"{key}.csv"), newline='') as csvfile:
+    with open(os.path.join(pkg_dir, "soulgauge_LUTs", f"byte1213_{key}.csv"), newline='') as csvfile:
+        lut_reader = csv.reader(csvfile, delimiter=',')
+        for row in lut_reader:
+            if int(row[0]) == n_notes:
+                soulGaugeByte12 = int(row[1]) % 255
+                soulGaugeByte13 = int(row[1]) // 255
+                break
+    with open(os.path.join(pkg_dir, "soulgauge_LUTs", f"byte1617_{key}.csv"), newline='') as csvfile:
+        lut_reader = csv.reader(csvfile, delimiter=',')
+        for row in lut_reader:
+            if int(row[0]) == n_notes:
+                soulGaugeByte16 = int(row[1]) % 255
+                soulGaugeByte17 = int(row[1]) // 255
+                break
+    with open(os.path.join(pkg_dir, "soulgauge_LUTs", f"byte2021_{key}.csv"), newline='') as csvfile:
         lut_reader = csv.reader(csvfile, delimiter=',')
         for row in lut_reader:
             if int(row[0]) == n_notes:
                 soulGaugeByte20 = int(row[1]) % 255
                 soulGaugeByte21 = 253 + (int(row[1]) // 255)
-                return soulGaugeByte20, soulGaugeByte21
-        raise ValueError(f"n_notes value '{n_notes}' not in lookup table (1-2500)")
+                break
+    return soulGaugeByte12, soulGaugeByte13, soulGaugeByte16, soulGaugeByte17, soulGaugeByte20, soulGaugeByte21
 
 
 def readStruct(file, order, format_string, seek=None):
     """
     Interpret bytes as packed binary data.
 
     Arguments:
```

### Comparing `tja2fumen-0.5.0/src/tja2fumen/writers.py` & `tja2fumen-0.5.1/src/tja2fumen/writers.py`

 * *Files identical despite different names*

### Comparing `tja2fumen-0.5.0/src/tja2fumen.egg-info/PKG-INFO` & `tja2fumen-0.5.1/src/tja2fumen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tja2fumen
-Version: 0.5.0
+Version: 0.5.1
 Summary: Convert TJA chart files into fumen (.bin) chart files
 License: MIT License
         
         Copyright (c) 2023 Vivaria
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

