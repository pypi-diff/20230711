# Comparing `tmp/panfeed-1.5.0.tar.gz` & `tmp/panfeed-1.5.1.tar.gz`

## Comparing `panfeed-1.5.0.tar` & `panfeed-1.5.1.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 panfeed-1.5.0/environment.yml
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 panfeed-1.5.0/panfeed-get-clusters-runner.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 panfeed-1.5.0/panfeed-get-kmers-runner.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 panfeed-1.5.0/panfeed-plot-runner.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 panfeed-1.5.0/panfeed-runner.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 panfeed-1.5.0/panfeed/__init__.py
--rw-r--r--   0        0        0    13003 2020-02-02 00:00:00.000000 panfeed-1.5.0/panfeed/__main__.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 panfeed-1.5.0/panfeed/classes.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 panfeed-1.5.0/panfeed/colorlog.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 panfeed-1.5.0/panfeed/get_clusters.py
--rw-r--r--   0        0        0     4491 2020-02-02 00:00:00.000000 panfeed-1.5.0/panfeed/get_kmers.py
--rw-r--r--   0        0        0    14576 2020-02-02 00:00:00.000000 panfeed-1.5.0/panfeed/input.py
--rw-r--r--   0        0        0     9235 2020-02-02 00:00:00.000000 panfeed-1.5.0/panfeed/panfeed.py
--rw-r--r--   0        0        0    17064 2020-02-02 00:00:00.000000 panfeed-1.5.0/panfeed/plot.py
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 panfeed-1.5.0/LICENSE
--rw-r--r--   0        0        0     6516 2020-02-02 00:00:00.000000 panfeed-1.5.0/README.md
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 panfeed-1.5.0/pyproject.toml
--rw-r--r--   0        0        0    20337 2020-02-02 00:00:00.000000 panfeed-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0    16384 2020-02-02 00:00:00.000000 panfeed-1.5.1/.CONTRIBUTING.md.swp
+-rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 panfeed-1.5.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 panfeed-1.5.1/environment.yml
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 panfeed-1.5.1/panfeed-get-clusters-runner.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 panfeed-1.5.1/panfeed-get-kmers-runner.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 panfeed-1.5.1/panfeed-plot-runner.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 panfeed-1.5.1/panfeed-runner.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 panfeed-1.5.1/panfeed/__init__.py
+-rw-r--r--   0        0        0    13003 2020-02-02 00:00:00.000000 panfeed-1.5.1/panfeed/__main__.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 panfeed-1.5.1/panfeed/classes.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 panfeed-1.5.1/panfeed/colorlog.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 panfeed-1.5.1/panfeed/get_clusters.py
+-rw-r--r--   0        0        0     4491 2020-02-02 00:00:00.000000 panfeed-1.5.1/panfeed/get_kmers.py
+-rw-r--r--   0        0        0    14576 2020-02-02 00:00:00.000000 panfeed-1.5.1/panfeed/input.py
+-rw-r--r--   0        0        0     9235 2020-02-02 00:00:00.000000 panfeed-1.5.1/panfeed/panfeed.py
+-rw-r--r--   0        0        0    16783 2020-02-02 00:00:00.000000 panfeed-1.5.1/panfeed/plot.py
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 panfeed-1.5.1/LICENSE
+-rw-r--r--   0        0        0     6743 2020-02-02 00:00:00.000000 panfeed-1.5.1/README.md
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 panfeed-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0    20564 2020-02-02 00:00:00.000000 panfeed-1.5.1/PKG-INFO
```

### Comparing `panfeed-1.5.0/panfeed/__main__.py` & `panfeed-1.5.1/panfeed/__main__.py`

 * *Files identical despite different names*

### Comparing `panfeed-1.5.0/panfeed/classes.py` & `panfeed-1.5.1/panfeed/classes.py`

 * *Files identical despite different names*

### Comparing `panfeed-1.5.0/panfeed/colorlog.py` & `panfeed-1.5.1/panfeed/colorlog.py`

 * *Files identical despite different names*

### Comparing `panfeed-1.5.0/panfeed/get_clusters.py` & `panfeed-1.5.1/panfeed/get_clusters.py`

 * *Files identical despite different names*

### Comparing `panfeed-1.5.0/panfeed/get_kmers.py` & `panfeed-1.5.1/panfeed/get_kmers.py`

 * *Files identical despite different names*

### Comparing `panfeed-1.5.0/panfeed/input.py` & `panfeed-1.5.1/panfeed/input.py`

 * *Files identical despite different names*

### Comparing `panfeed-1.5.0/panfeed/panfeed.py` & `panfeed-1.5.1/panfeed/panfeed.py`

 * *Files identical despite different names*

### Comparing `panfeed-1.5.0/panfeed/plot.py` & `panfeed-1.5.1/panfeed/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,19 +300,15 @@
                 t = t.reindex(sorted(t.index) + sorted(strains.difference(t.index)),
                               fill_value='-')
             if args.phenotype_column is None:
                 # sort the table by p-values
                 t = t.loc[g.index]
             else:
                 # sort by phenotype
-                df_sort = p.to_frame().join(g.fillna(0).T.max().to_frame(), how='outer')
-                df_sort.columns = ['pheno', 'pvalue']
-                df_sort = df_sort.fillna(0)
-                df_sort = df_sort.sort_values(['pheno', 'pvalue'], ascending=False)
-                t = t.loc[df_sort.index]
+                t = t.loc[p.index]
 
         # find the index for the gene start (if present)
         gene_start = [i for i, x in enumerate(g.columns)
                       if x == 0]
         if len(gene_start) > 0:
             gene_start = gene_start[0]
         else:
```

### Comparing `panfeed-1.5.0/LICENSE` & `panfeed-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `panfeed-1.5.0/README.md` & `panfeed-1.5.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # panfeed
 
+[![Anaconda-Server Badge](https://anaconda.org/bioconda/panfeed/badges/version.svg)](https://anaconda.org/bioconda/panfeed)
+
 `panfeed` is a k-mer streaming tool that works one gene cluster at a time.
 Starting from a list of annotated genome assemblies in GFF3 format and a gene presence absence matrix (as produced by
 [`roary`](https://github.com/sanger-pathogens/Roary), [`panaroo`](https://github.com/gtonkinhill/panaroo/)
 and [`ggCaller`](https://github.com/samhorsfield96/ggCaller)),
 `panfeed` generates a table with unique k-mer presence/absence patterns,
 which can be used for genome-wide associations (GWAS) using tools
 such as [`pyseer`](https://github.com/mgalardini/pyseer).
@@ -18,14 +20,18 @@
 
 # Installation
 
 `panfeed` can be installed using `pip`:
 
     python3 -m pip install panfeed
 
+Or through `conda` (or `mamba` to speed things up):
+
+    conda create -n panfeed -c bioconda panfeed
+
 Alternatively, we provide a `conda` recipe to create an environment 
 named `panfeed `. Download the
 [environment file](https://raw.githubusercontent.com/microbial-pangenomes-lab/panfeed/main/environment.yml)
 and then run:
 
     conda env create -f environment.yml
     conda activate panfeed
```

### Comparing `panfeed-1.5.0/pyproject.toml` & `panfeed-1.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `panfeed-1.5.0/PKG-INFO` & `panfeed-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panfeed
-Version: 1.5.0
+Version: 1.5.1
 Summary: Compute gene-cluster specific k-mers over a pangenome
 Project-URL: Homepage, https://github.com/microbial-pangenomes-lab/panfeed
 Project-URL: Bug Tracker, https://github.com/microbial-pangenomes-lab/panfeed/issues
 Author-email: Hannes Neubauer <neubauer.hannes@mh-hannover.de>, Marco Galardini <galardini.marco@mh-hannover.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -218,14 +218,16 @@
 Requires-Dist: pandas
 Requires-Dist: pyfaidx
 Requires-Dist: seaborn
 Description-Content-Type: text/markdown
 
 # panfeed
 
+[![Anaconda-Server Badge](https://anaconda.org/bioconda/panfeed/badges/version.svg)](https://anaconda.org/bioconda/panfeed)
+
 `panfeed` is a k-mer streaming tool that works one gene cluster at a time.
 Starting from a list of annotated genome assemblies in GFF3 format and a gene presence absence matrix (as produced by
 [`roary`](https://github.com/sanger-pathogens/Roary), [`panaroo`](https://github.com/gtonkinhill/panaroo/)
 and [`ggCaller`](https://github.com/samhorsfield96/ggCaller)),
 `panfeed` generates a table with unique k-mer presence/absence patterns,
 which can be used for genome-wide associations (GWAS) using tools
 such as [`pyseer`](https://github.com/mgalardini/pyseer).
@@ -240,14 +242,18 @@
 
 # Installation
 
 `panfeed` can be installed using `pip`:
 
     python3 -m pip install panfeed
 
+Or through `conda` (or `mamba` to speed things up):
+
+    conda create -n panfeed -c bioconda panfeed
+
 Alternatively, we provide a `conda` recipe to create an environment 
 named `panfeed `. Download the
 [environment file](https://raw.githubusercontent.com/microbial-pangenomes-lab/panfeed/main/environment.yml)
 and then run:
 
     conda env create -f environment.yml
     conda activate panfeed
```

