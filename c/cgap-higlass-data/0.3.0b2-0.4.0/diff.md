# Comparing `tmp/cgap_higlass_data-0.3.0b2.tar.gz` & `tmp/cgap_higlass_data-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgap_higlass_data-0.3.0b2.tar", max compression
+gzip compressed data, was "cgap_higlass_data-0.4.0.tar", max compression
```

## Comparing `cgap_higlass_data-0.3.0b2.tar` & `cgap_higlass_data-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1090 2022-10-11 17:52:02.790519 cgap_higlass_data-0.3.0b2/LICENSE
--rw-r--r--   0        0        0     2437 2023-04-04 16:01:10.419959 cgap_higlass_data-0.3.0b2/README.md
--rw-r--r--   0        0        0        1 2022-07-04 15:38:47.258048 cgap_higlass_data-0.3.0b2/higlass_data/__init__.py
--rw-r--r--   0        0        0     1284 2023-03-31 12:32:02.123669 cgap_higlass_data-0.3.0b2/higlass_data/conversions.py
--rw-r--r--   0        0        0    12387 2023-05-30 20:44:29.463446 cgap_higlass_data-0.3.0b2/higlass_data/create_cohort_vcf.py
--rw-r--r--   0        0        0     4087 2023-05-30 20:01:11.774635 cgap_higlass_data-0.3.0b2/higlass_data/create_coverage_bed.py
--rw-r--r--   0        0        0     6148 2023-03-30 11:53:56.872920 cgap_higlass_data-0.3.0b2/higlass_data/data/.DS_Store
--rw-r--r--   0        0        0        1 2023-03-31 11:14:40.069331 cgap_higlass_data-0.3.0b2/higlass_data/data/__init__.py
--rw-r--r--   0        0        0    11672 2021-12-08 21:46:49.672243 cgap_higlass_data-0.3.0b2/higlass_data/data/hg38.chromsizes
--rw-r--r--   0        0        0      364 2023-05-16 19:46:21.634852 cgap_higlass_data-0.3.0b2/higlass_data/data/hg38.mod.chromsizes
--rw-r--r--   0        0        0      160 2023-03-30 12:48:34.735812 cgap_higlass_data-0.3.0b2/higlass_data/utils.py
--rw-r--r--   0        0        0     1445 2023-05-30 20:44:44.697995 cgap_higlass_data-0.3.0b2/pyproject.toml
--rw-r--r--   0        0        0     3612 1970-01-01 00:00:00.000000 cgap_higlass_data-0.3.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1090 2022-10-11 17:52:02.790519 cgap_higlass_data-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2604 2023-07-11 18:18:18.869192 cgap_higlass_data-0.4.0/README.md
+-rw-r--r--   0        0        0        1 2022-07-04 15:38:47.258048 cgap_higlass_data-0.4.0/higlass_data/__init__.py
+-rw-r--r--   0        0        0     1284 2023-03-31 12:32:02.123669 cgap_higlass_data-0.4.0/higlass_data/conversions.py
+-rw-r--r--   0        0        0    14849 2023-07-11 18:03:10.913668 cgap_higlass_data-0.4.0/higlass_data/create_cohort_vcf.py
+-rw-r--r--   0        0        0     4087 2023-05-30 20:01:11.774635 cgap_higlass_data-0.4.0/higlass_data/create_coverage_bed.py
+-rw-r--r--   0        0        0     6148 2023-03-30 11:53:56.872920 cgap_higlass_data-0.4.0/higlass_data/data/.DS_Store
+-rw-r--r--   0        0        0        1 2023-03-31 11:14:40.069331 cgap_higlass_data-0.4.0/higlass_data/data/__init__.py
+-rw-r--r--   0        0        0    11672 2021-12-08 21:46:49.672243 cgap_higlass_data-0.4.0/higlass_data/data/hg38.chromsizes
+-rw-r--r--   0        0        0      364 2023-05-16 19:46:21.634852 cgap_higlass_data-0.4.0/higlass_data/data/hg38.mod.chromsizes
+-rw-r--r--   0        0        0      470 2023-07-11 17:43:29.635667 cgap_higlass_data-0.4.0/higlass_data/utils.py
+-rw-r--r--   0        0        0     1443 2023-07-11 18:23:13.033164 cgap_higlass_data-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3777 1970-01-01 00:00:00.000000 cgap_higlass_data-0.4.0/PKG-INFO
```

### Comparing `cgap_higlass_data-0.3.0b2/LICENSE` & `cgap_higlass_data-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cgap_higlass_data-0.3.0b2/README.md` & `cgap_higlass_data-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,16 @@
 
 ```
 # -i input VCF path
 # -o output VCF path
 # -c info field in the input VCF that ranks the variants
 # -m maximal tile values per consequence. Controls how may variants are displayed at once and a certain zoom level
 # -q quiet True / False. Toggles verbose output
+# -w chromosome-wise True / False. Significantly less memory intensive, but slightly slower.
+# -t index output. True / False. If true, the output vcf will be indexed.
 create-cohort-vcf -i ./PATH/input.vcf \
                   -o ./PATH/output.vcf \
                   -c p_value_negative_log_10 \
                   -q True
 
 ```
```

### Comparing `cgap_higlass_data-0.3.0b2/higlass_data/conversions.py` & `cgap_higlass_data-0.4.0/higlass_data/conversions.py`

 * *Files identical despite different names*

### Comparing `cgap_higlass_data-0.3.0b2/higlass_data/create_cohort_vcf.py` & `cgap_higlass_data-0.4.0/higlass_data/create_cohort_vcf.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,48 @@
 import click
 import vcf
 import pandas as pd
-import copy
+import copy, os
+import os.path
 import negspy.coordinates as nc
+from higlass_data.utils import does_tool_exist, get_chroms, get_vcf_header
 
 TILE_SIZE = 1024  # Higlass tile size for 1D tracks
 MAX_ZOOM_LEVEL = 23
 CONSEQUENCE_LEVELS = ["HIGH", "LOW", "MODERATE", "MODIFIER"]
 
 
 class MultiResVcf:
 
-    input_filepath = ""
-    output_filepath = ""
-    max_variants_per_tile = 0
-    chromosomes = []
-    variants = []
-    variants_multires = []
-    variants_df = []
-    variants_by_id = {}
-    tile_sizes = []
-    chrom_info = ""
-    quiet = True
-
+    
     def __init__(
         self,
         input_filepath,
         output_filepath,
         importance_column,
         max_variants_per_tile,
+        chrom,
         quiet,
     ):
         self.input_filepath = input_filepath
         self.output_filepath = output_filepath
         self.max_variants_per_tile = max_variants_per_tile
         self.importance_column = importance_column
         self.quiet = quiet
-        self.variants = self.load_variants()
+        self.variants = self.load_variants(chrom)
+        self.variants_multires = []
+        self.variants_df = []
+        self.variants_by_id = {}
         self.chromosomes = self.get_chromosomes()
         self.tile_sizes = [TILE_SIZE * (2**i) for i in range(0, MAX_ZOOM_LEVEL)]
         self.chrom_info = nc.get_chrominfo("hg38")
 
     def create_multires_vcf(self):
+        if len(self.variants) == 0:
+            return
         self.assign_ids()
         self.index_variants_by_id()
         self.create_variants_dataframe()
         self.split_variants()
         self.aggregate()
         self.write_vcf()
 
@@ -147,25 +144,28 @@
                     ] = tile_data
                     hierarchical_variant_data[
                         f"{new_zoom_level}.{2*i_tile+1}"
                     ] = tile_data
 
         self.variants_df_hierarchical = hierarchical_variant_data
 
-    def load_variants(self):
+    def load_variants(self, chrom):
         if not self.quiet:
             print("Loading variants...")
         variants = []
-        vcf_reader = vcf.Reader(open(self.input_filepath, "r"))
+        vcf_reader = vcf.Reader(filename=self.input_filepath)
 
         for record in vcf_reader:
-            variants.append(record)
+            if not chrom:
+                variants.append(record)
+            elif chrom and record.CHROM == chrom:
+                variants.append(record)
 
         if not self.quiet:
-            print("Loading variants complete.")
+            print(f"Loading variants complete. Loaded {len(variants)} variants")
         return variants
 
     def index_variants_by_id(self):
         for variant in self.variants:
             self.variants_by_id[variant.ID] = variant
 
     def importance(self, importance_value):
@@ -212,22 +212,23 @@
             "absPos": absPos,
             "consequence": consequence,
             "importance": importance,
         }
         self.variants_df = pd.DataFrame(data=d)
 
     def write_vcf(self):
-        vcf_reader = vcf.Reader(open(self.input_filepath, "r"))
+        vcf_reader = vcf.Reader(filename=self.input_filepath)
 
-        with open(self.output_filepath, "w") as output:
+        with open("tmp.output.vcf", "w") as output:
             vcf_writer = vcf.Writer(output, vcf_reader)
-
             for variant in self.variants_multires:
                 vcf_writer.write_record(variant)
                 vcf_writer.flush()
+        
+
 
     def get_chromosomes(self):
         if not self.quiet:
             print("Extracting chromosomes...")
         chrs = list(set(map(lambda v: v.CHROM, self.variants)))
         if "chrM" in chrs:
             chrs.remove("chrM")
@@ -300,31 +301,87 @@
     required=True,
     type=str,
     help="Value in the info field of the VCF that should be sorted by",
 )
 @click.option(
     "-m", "--max-tile-values-per-consequence", default=50, required=False, type=int
 )
+@click.option(
+    "-w", "--chromosome-wise", default=False, required=False, type=bool
+)
+@click.option("-t", "--index-output", required=False, default=True, type=bool)
 @click.option("-q", "--quiet", required=False, default=True, type=bool)
 def create_cohort_vcf(
-    input_vcf, output_vcf, importance_column, max_tile_values_per_consequence, quiet
+    input_vcf, output_vcf, importance_column, max_tile_values_per_consequence, chromosome_wise, index_output, quiet
 ):
     input_filepath = input_vcf
     output_vcf_filepath = output_vcf
     max_variants_per_tile = max_tile_values_per_consequence
 
-    mrv = MultiResVcf(
-        input_filepath,
-        output_vcf_filepath,
-        importance_column,
-        max_variants_per_tile,
-        quiet,
-    )
-    if output_vcf_filepath:
-        mrv.create_multires_vcf()
+    if not does_tool_exist("bgzip"):
+        raise Exception("bgzip is not installed.")
+    if not does_tool_exist("tabix"):
+        raise Exception("tabix is not installed.")
+
+    if chromosome_wise:
+        vcf_header = get_vcf_header()
+        cmd = f"echo '{vcf_header}' > vcf_header.vcf"
+        os.system(cmd)
+        cmd = f"cat vcf_header.vcf | gzip > hgdata.tmp.header.vcf.gz"
+        os.system(cmd)
+
+        for chrom in get_chroms():
+            mrv = MultiResVcf(
+                input_filepath,
+                f"hgdata.tmp.{chrom}.{output_vcf_filepath}",
+                importance_column,
+                max_variants_per_tile,
+                chrom,
+                quiet,
+            )
+            if output_vcf_filepath:
+                mrv.create_multires_vcf()
+                if os.path.exists("tmp.output.vcf"):
+                    tmp_filename = f"hgdata.tmp.{chrom}.{output_vcf_filepath}"
+                    cmd = f"cat tmp.output.vcf | tail -n +3 | gzip > {tmp_filename} || exit 1"
+                    cmd_result = os.system(cmd)
+                    if cmd_result > 0:
+                        raise Exception(f"{cmd} failed.")
+                    os.system(f"rm -f tmp.output.vcf")
+
+        os.system(f"cat hgdata.tmp.header.vcf.gz hgdata.tmp* > multires.tmp.gz || exit 1") 
+        os.system(f"rm -f hgdata.tmp*") 
+
+        #Recompress with bgzip
+        cmd_result = os.system(f"gzip -cd multires.tmp.gz | bgzip --threads 6 -c > {output_vcf_filepath} || exit 1")
+        if cmd_result > 0:
+            raise Exception(f"Recompression failed.")
+        os.system(f"rm -f multires.tmp.gz")
+
+
+    else:
+        mrv = MultiResVcf(
+            input_filepath,
+            output_vcf_filepath,
+            importance_column,
+            max_variants_per_tile,
+            None,
+            quiet,
+        )
+        if output_vcf_filepath:
+            mrv.create_multires_vcf()
+            cmd_result = os.system(f"cat tmp.output.vcf | bgzip --threads 6 -c > {output_vcf_filepath} || exit 1")
+            if cmd_result > 0:
+                raise Exception(f"Compression failed.")
+
+    if index_output:
+        cmd = f"tabix -p vcf {output_vcf_filepath} || exit 1"
+        cmd_result = os.system(cmd)
+        if cmd_result > 0:
+            raise Exception(f"{cmd} failed.")
 
 
 if __name__ == "__main__":
     """
     Example:
     python create_cohort_vcf.py -i joint_calling_results.vcf -o joint_calling_results.multires.vcf -c regenie_log10p -q False
     """
```

### Comparing `cgap_higlass_data-0.3.0b2/higlass_data/create_coverage_bed.py` & `cgap_higlass_data-0.4.0/higlass_data/create_coverage_bed.py`

 * *Files identical despite different names*

### Comparing `cgap_higlass_data-0.3.0b2/higlass_data/data/.DS_Store` & `cgap_higlass_data-0.4.0/higlass_data/data/.DS_Store`

 * *Files identical despite different names*

### Comparing `cgap_higlass_data-0.3.0b2/higlass_data/data/hg38.chromsizes` & `cgap_higlass_data-0.4.0/higlass_data/data/hg38.chromsizes`

 * *Files identical despite different names*

### Comparing `cgap_higlass_data-0.3.0b2/pyproject.toml` & `cgap_higlass_data-0.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cgap-higlass-data"
-version = "0.3.0b2"
+version = "0.4.0"
 description = "Data file generation for CGAP's Higlass browsers"
 authors = ["Alexander Veit <alexander_veit@hms.harvard.edu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/dbmi-bgm/higlass-data"
 repository = "https://github.com/dbmi-bgm/higlass-data"
 packages = [
```

### Comparing `cgap_higlass_data-0.3.0b2/PKG-INFO` & `cgap_higlass_data-0.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgap-higlass-data
-Version: 0.3.0b2
+Version: 0.4.0
 Summary: Data file generation for CGAP's Higlass browsers
 Home-page: https://github.com/dbmi-bgm/higlass-data
 License: MIT
 Author: Alexander Veit
 Author-email: alexander_veit@hms.harvard.edu
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -72,14 +72,16 @@
 
 ```
 # -i input VCF path
 # -o output VCF path
 # -c info field in the input VCF that ranks the variants
 # -m maximal tile values per consequence. Controls how may variants are displayed at once and a certain zoom level
 # -q quiet True / False. Toggles verbose output
+# -w chromosome-wise True / False. Significantly less memory intensive, but slightly slower.
+# -t index output. True / False. If true, the output vcf will be indexed.
 create-cohort-vcf -i ./PATH/input.vcf \
                   -o ./PATH/output.vcf \
                   -c p_value_negative_log_10 \
                   -q True
 
 ```
```

