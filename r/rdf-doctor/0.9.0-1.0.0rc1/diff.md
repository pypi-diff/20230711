# Comparing `tmp/rdf_doctor-0.9.0-py3-none-any.whl.zip` & `tmp/rdf_doctor-1.0.0rc1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 23562 bytes, number of entries: 12
--rw-r--r--  2.0 unx       22 b- defN 23-Jul-10 00:48 doctor/__init__.py
+Zip file size: 23547 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       25 b- defN 23-Jul-11 07:23 doctor/__init__.py
 -rw-r--r--  2.0 unx      631 b- defN 23-Jul-10 00:40 doctor/consts.py
--rw-r--r--  2.0 unx    36220 b- defN 23-Jul-10 00:40 doctor/doctor.py
--rw-r--r--  2.0 unx    43474 b- defN 23-Jul-10 00:40 doctor/reference/prefixes.tsv
+-rw-r--r--  2.0 unx    36512 b- defN 23-Jul-11 06:03 doctor/doctor.py
+-rw-r--r--  2.0 unx    43474 b- defN 23-Jul-11 05:56 doctor/reference/prefixes.tsv
 -rw-r--r--  2.0 unx       90 b- defN 23-Jul-10 00:40 doctor/reference/refine-class-uris.tsv
--rw-r--r--  2.0 unx      679 b- defN 23-Jul-10 00:40 doctor/reference/refine-prefix-uris.tsv
--rw-r--r--  2.0 unx     1061 b- defN 23-Jul-10 00:54 rdf_doctor-0.9.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     9892 b- defN 23-Jul-10 00:54 rdf_doctor-0.9.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-10 00:54 rdf_doctor-0.9.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 23-Jul-10 00:54 rdf_doctor-0.9.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-Jul-10 00:54 rdf_doctor-0.9.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      992 b- defN 23-Jul-10 00:54 rdf_doctor-0.9.0.dist-info/RECORD
-12 files, 93212 bytes uncompressed, 21882 bytes compressed:  76.5%
+-rw-r--r--  2.0 unx      577 b- defN 23-Jul-10 05:15 doctor/reference/refine-prefix-uris.tsv
+-rw-r--r--  2.0 unx     1061 b- defN 23-Jul-11 07:28 rdf_doctor-1.0.0rc1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8514 b- defN 23-Jul-11 07:28 rdf_doctor-1.0.0rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-11 07:28 rdf_doctor-1.0.0rc1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       52 b- defN 23-Jul-11 07:28 rdf_doctor-1.0.0rc1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-Jul-11 07:28 rdf_doctor-1.0.0rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1010 b- defN 23-Jul-11 07:28 rdf_doctor-1.0.0rc1.dist-info/RECORD
+12 files, 92045 bytes uncompressed, 21831 bytes compressed:  76.3%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: doctor/reference/refine-class-uris.tsv
 Comment: 
 
 Filename: doctor/reference/refine-prefix-uris.tsv
 Comment: 
 
-Filename: rdf_doctor-0.9.0.dist-info/LICENSE
+Filename: rdf_doctor-1.0.0rc1.dist-info/LICENSE
 Comment: 
 
-Filename: rdf_doctor-0.9.0.dist-info/METADATA
+Filename: rdf_doctor-1.0.0rc1.dist-info/METADATA
 Comment: 
 
-Filename: rdf_doctor-0.9.0.dist-info/WHEEL
+Filename: rdf_doctor-1.0.0rc1.dist-info/WHEEL
 Comment: 
 
-Filename: rdf_doctor-0.9.0.dist-info/entry_points.txt
+Filename: rdf_doctor-1.0.0rc1.dist-info/entry_points.txt
 Comment: 
 
-Filename: rdf_doctor-0.9.0.dist-info/top_level.txt
+Filename: rdf_doctor-1.0.0rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: rdf_doctor-0.9.0.dist-info/RECORD
+Filename: rdf_doctor-1.0.0rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## doctor/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "0.9.0"
+__version__ = "1.0.0rc1"
```

## doctor/doctor.py

```diff
@@ -154,27 +154,27 @@
                         nargs="+",
                         help="set the target classes to be inspected to one of: all (defalut) or URL1, URL2,...",
                         metavar="URL")
 
     # Prefix URI dictionary file path(-p, --prefix-dict [FILE]、default: reference/refine-prefix-uris.tsv)
     parser.add_argument("-p","--prefix-dict", type=str,
                         default=str(Path(__file__).resolve().parent.joinpath(REFINE_PREFIX_URIS_FILE_PATH)),
-                        help='(only when md(same as "markdown") is specified with -r, --report option) path to a tab delimited file listing candidate pairs of URI rewrite source and rewrite destination for the prefix (default: predefined file in rdf-doctor)',
+                        help='(only when "-r md"(same as "-r markdown") is specified) path to a tab delimited file listing candidate pairs of URI rewrite source and rewrite destination for the prefix (default: predefined file in rdf-doctor: https://github.com/dbcls/rdf-doctor/blob/main/doctor/reference/refine-prefix-uris.tsv)',
                         metavar="FILE")
 
     # Class URI dictionary file path(-l, --class-dict [FILE]、default: reference/refine-class-uris.tsv)
     parser.add_argument("-l","--class-dict", type=str,
                         default=str(Path(__file__).resolve().parent.joinpath(REFINE_CLASS_URIS_FILE_PATH)),
-                        help='(only when md(same as "markdown") is specified with -r, --report option) path to a tab delimited file listing candidate pairs of URI rewrite source and rewrite destination for the class (default: predefined file in rdf-doctor)',
+                        help='(only when "-r md"(same as "-r markdown") is specified) path to a tab delimited file listing candidate pairs of URI rewrite source and rewrite destination for the class (default: predefined file in rdf-doctor: https://github.com/dbcls/rdf-doctor/blob/main/doctor/reference/refine-class-uris.tsv)',
                         metavar="FILE")
 
     # Prefix list file path(-x, --prefix-list [FILE]、default: reference/prefixes.tsv)
     parser.add_argument("-x","--prefix-list", type=str,
                         default=str(Path(__file__).resolve().parent.joinpath(PREFIXES_FILE_PATH)),
-                        help="list of prefixes (default: predefined file in rdf-doctor)",
+                        help="list of prefixes (default: predefined file in rdf-doctor: https://github.com/dbcls/rdf-doctor/blob/main/doctor/reference/prefixes.tsv)",
                         metavar="FILE")
 
     # input format (-f、--format [INPUT_FORMAT]、default: Standard output)
     parser.add_argument("-f","--force-format", type=str,
                         help='This option should not normally be used. Because the input format is automatically determined by the file extension. Use it only when you want to force specification. If used, "turtle" or "nt" can be specified.',
                         metavar="INPUT-FORMAT")
 
@@ -359,31 +359,31 @@
         result_duplicated_prefixes.extend(["# " + s for s in duplicated_prefixes])
         result_duplicated_prefixes.append("\n\n")
 
     # Suggest QName based on URI of validation expression output by sheXer and prefixes.tsv
     if args.verbose:
         print_overwrite(get_dt_now() + " -- Creating suggestions for QName...")
 
-    result_suggested_qname = []
+    result_widely_used_qname = []
     widely_used_prefixes = get_widely_used_prefixes(args.prefix_list)
-    suggested_qname = get_suggested_qname(shaper_result, input_prefixes, widely_used_prefixes)
-    if len(suggested_qname) != 0:
-        result_suggested_qname.append("# There is a more widely used QName.\n\n")
-        result_suggested_qname.append("# Input-QName\tWidely-used-QName\tURI\n")
-        result_suggested_qname.extend(["# " + s for s in suggested_qname])
-        result_suggested_qname.append("\n")
+    widely_used_qname = get_widely_used_qname(shaper_result, input_prefixes, widely_used_prefixes)
+    if len(widely_used_qname) != 0:
+        result_widely_used_qname.append("# There is a more widely used QName.\n\n")
+        result_widely_used_qname.append("# Input-QName\tWidely-used-QName\tURI\n")
+        result_widely_used_qname.extend(["# " + s for s in widely_used_qname])
+        result_widely_used_qname.append("\n")
 
     # List for storing the final result
     shex_final_result = []
     shex_final_result.extend(shaper_result)
     if len(result_duplicated_prefixes) != 0:
         shex_final_result.extend(result_duplicated_prefixes)
 
-    if len(result_suggested_qname) != 0:
-        shex_final_result.extend(result_suggested_qname)
+    if len(result_widely_used_qname) != 0:
+        shex_final_result.extend(result_widely_used_qname)
 
     result_queue.put(shex_final_result)
 
 
 # Processing when the report format is "md/markdown"
 def get_markdown_result(args, input_format, compression_mode, result_queue):
 
@@ -701,16 +701,16 @@
         widely_used_prefixes = [row for row in tsv_reader]
 
     return widely_used_prefixes
 
 
 # Compare the URI of the validation expression in the shexer output with the URI of the prepared prefix list
 # and get the matching QName from the prefix list
-def get_suggested_qname(shaper_result, input_prefixes, widely_used_prefixes):
-    suggest_qname = []
+def get_widely_used_qname(shaper_result, input_prefixes, widely_used_prefixes):
+    widely_used_qname = []
 
     # Comparison of prefix list and minimal URI detected by shaXer
     for line in shaper_result.splitlines():
         if ("[<http" in line and ">~]" in line):
             exists_in_input_prefix = False
             shaper_result_uri = line[line.find("[<http")+2:line.find(">~]")]
 
@@ -719,56 +719,56 @@
             input_qname = "Undefined"
             for input_prefix in input_prefixes:
                 if shaper_result_uri == input_prefix[1]:
                     exists_in_input_prefix = True
                     input_qname = input_prefix[0]
                     break
 
-            tmp_suggest_qname = []
+            tmp_widely_used_qname = []
             is_included_list = False
             for widely_used_prefix in widely_used_prefixes:
                 append_str = input_qname + "\t" + widely_used_prefix[0]+"\t"+shaper_result_uri+"\n"
-                if shaper_result_uri == widely_used_prefix[1] and append_str not in suggest_qname:
+                if shaper_result_uri == widely_used_prefix[1] and append_str not in widely_used_qname:
                     if exists_in_input_prefix:
                         # If the prefixes defined in the input file include those with the same URI,
                         # add them to the list only if the QName is different
                         if widely_used_prefix[0] != input_qname:
-                            tmp_suggest_qname.append(append_str)
+                            tmp_widely_used_qname.append(append_str)
                         else:
                             # If the QName defined in the input file is also included in the prefix list,
                             # do not suggest another QName with the same URI in the prefix list
                             is_included_list = True
                             break
                     else:
-                        suggest_qname.append(append_str)
+                        widely_used_qname.append(append_str)
 
             if is_included_list == False:
-                suggest_qname.extend(tmp_suggest_qname)
+                widely_used_qname.extend(tmp_widely_used_qname)
 
     # Comparing of prefix list and prefixes in input file
     for input_prefix in input_prefixes:
-        tmp_suggest_qname = []
+        tmp_widely_used_qname = []
         is_included_list = False
         for widely_used_prefix in widely_used_prefixes:
             append_str = input_prefix[0] + "\t" + widely_used_prefix[0]+"\t"+input_prefix[1]+"\n"
-            if input_prefix[1] == widely_used_prefix[1] and append_str not in suggest_qname:
+            if input_prefix[1] == widely_used_prefix[1] and append_str not in widely_used_qname:
                 # If the prefixes defined in the input file include those with the same URI,
                 # add them to the list only if the QName is different
                 if input_prefix[0] != widely_used_prefix[0]:
-                    tmp_suggest_qname.append(append_str)
+                    tmp_widely_used_qname.append(append_str)
                 else:
                     # If the QName defined in the input file is also included in the prefix list,
                     # do not suggest another QName with the same URI in the prefix list
                     is_included_list = True
                     break
 
         if is_included_list == False:
-            suggest_qname.extend(tmp_suggest_qname)
+            widely_used_qname.extend(tmp_widely_used_qname)
 
-    return suggest_qname
+    return widely_used_qname
 
 
 # Generates a key from the received string, excluding case differences, symbols, control characters, etc.
 # Values that contain only the most valuable or meaningful part of the string will have the same key
 # returned by this method, useful for clustering.
 # Detailed explanation：https://openrefine.org/docs/technical-reference/clustering-in-depth#fingerprint
 def fingerprint(string):
```

## doctor/reference/refine-prefix-uris.tsv

```diff
@@ -1,10 +1,8 @@
 http://www.ebi.ac.uk/chebi/searchId.do?chebiId=CHEBI%3A	http://purl.obolibrary.org/obo/CHEBI_
-http://rdf.ebi.ac.uk/resource/chembl/molecule/	
 http://identifiers.org/dbsnp/	https://identifiers.org/dbsnp:
 http://identifiers.org/dbsnp	https://identifiers.org/dbsnp:
 http://purl.jp/bio/10/dbsnp/	https://identifiers.org/dbsnp:
 http://identifiers.org/chebi/CHEBI:	http://purl.obolibrary.org/obo/CHEBI_
 http://purl.obolibrary.org/obo/chebi/	http://purl.obolibrary.org/obo/CHEBI_
 http://purl.obolibrary.org/obo/chebi.	http://purl.obolibrary.org/obo/CHEBI_
 http://purl.obolibrary.org/obo/chebi#	http://purl.obolibrary.org/obo/CHEBI_
-http://rdf.ebi.ac.uk/resource/chembl/molecule/CHEMBL
```

## Comparing `rdf_doctor-0.9.0.dist-info/LICENSE` & `rdf_doctor-1.0.0rc1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rdf_doctor-0.9.0.dist-info/RECORD` & `rdf_doctor-1.0.0rc1.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-doctor/__init__.py,sha256=H9NWRZb7NbeRRPLP_V1fARmLNXranorVM-OOY-8_2ug,22
+doctor/__init__.py,sha256=iwDi0TUz45SMYIlshEAh-UPerqIe7nxUavbLYwEgSR8,25
 doctor/consts.py,sha256=g8qN1vFAkkiFWF_HMGBpkoED0SdtPsxNUc33fcyLeow,631
-doctor/doctor.py,sha256=bEKsaQ2wbgcZYG7z9ACYYi5S0FZF7gkCLf-ziIWYP1s,36220
+doctor/doctor.py,sha256=O5kON__m9JjcLgjnP1sNpq4GoxD5fGhKPrctstKH5yw,36512
 doctor/reference/prefixes.tsv,sha256=9zIvWdCO3X65YnULmiBEsIapiZvmplZbB6MywGJp54s,43474
 doctor/reference/refine-class-uris.tsv,sha256=pd_nOSjR7bia96u9hhcjhBg9J6LUAuDFlyy-JE9tsys,90
-doctor/reference/refine-prefix-uris.tsv,sha256=B5iok0_4VqdBNLn4_Auwx5gSwAnxgIh6OoQ4cgebERY,679
-rdf_doctor-0.9.0.dist-info/LICENSE,sha256=e5qMQtuffizvdi23h6MoQ37f3xmNY0VBq8V0tgWuZNg,1061
-rdf_doctor-0.9.0.dist-info/METADATA,sha256=qGj9toPi3Kvu624mWNo0yoPeR_OJe9GoOZZINj-KD5g,9892
-rdf_doctor-0.9.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-rdf_doctor-0.9.0.dist-info/entry_points.txt,sha256=1vHyYdY5pMK7zOINHh2ymwU_Uid1YzZx7Vte5tjHCls,52
-rdf_doctor-0.9.0.dist-info/top_level.txt,sha256=8awHkjBkPxJ8N_ygAwmuUTUz5ZKfy9aqNcWTSI_Ma_8,7
-rdf_doctor-0.9.0.dist-info/RECORD,,
+doctor/reference/refine-prefix-uris.tsv,sha256=KY5PZ4WCaLeB0APNBjAWq7_Q5Whc6FLg9ncX7BSPeuw,577
+rdf_doctor-1.0.0rc1.dist-info/LICENSE,sha256=e5qMQtuffizvdi23h6MoQ37f3xmNY0VBq8V0tgWuZNg,1061
+rdf_doctor-1.0.0rc1.dist-info/METADATA,sha256=f2ZSFlrGkOv9M6BSq7v_VsukppP5FuOOGLnl8JdYQ8Q,8514
+rdf_doctor-1.0.0rc1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+rdf_doctor-1.0.0rc1.dist-info/entry_points.txt,sha256=1vHyYdY5pMK7zOINHh2ymwU_Uid1YzZx7Vte5tjHCls,52
+rdf_doctor-1.0.0rc1.dist-info/top_level.txt,sha256=8awHkjBkPxJ8N_ygAwmuUTUz5ZKfy9aqNcWTSI_Ma_8,7
+rdf_doctor-1.0.0rc1.dist-info/RECORD,,
```

