# Comparing `tmp/geneinfo-3.4.2.tar.gz` & `tmp/geneinfo-3.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geneinfo-3.4.2.tar", last modified: Mon Apr 10 18:15:11 2023, max compression
+gzip compressed data, was "geneinfo-3.4.3.tar", last modified: Tue Jul 11 09:40:11 2023, max compression
```

## Comparing `geneinfo-3.4.2.tar` & `geneinfo-3.4.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 kmt       (6358) kmt       (6358)        0 2023-04-10 18:15:11.124297 geneinfo-3.4.2/
--rw-rw-r--   0 kmt       (6358) kmt       (6358)     1069 2023-04-10 18:12:55.000000 geneinfo-3.4.2/LICENSE
--rw-rw-r--   0 kmt       (6358) kmt       (6358)      491 2023-04-10 18:15:11.113297 geneinfo-3.4.2/PKG-INFO
--rw-rw-r--   0 kmt       (6358) kmt       (6358)      174 2023-04-10 18:12:55.000000 geneinfo-3.4.2/README.md
-drwxrwxr-x   0 kmt       (6358) kmt       (6358)        0 2023-04-10 18:15:10.529286 geneinfo-3.4.2/geneinfo/
--rw-rw-r--   0 kmt       (6358) kmt       (6358)    52344 2023-04-10 18:13:17.000000 geneinfo-3.4.2/geneinfo/__init__.py
--rw-rw-r--   0 kmt       (6358) kmt       (6358)     3385 2023-04-10 18:12:56.000000 geneinfo-3.4.2/geneinfo/intervals.py
-drwxrwxr-x   0 kmt       (6358) kmt       (6358)        0 2023-04-10 18:15:11.019295 geneinfo-3.4.2/geneinfo.egg-info/
--rw-rw-r--   0 kmt       (6358) kmt       (6358)      491 2023-04-10 18:15:09.000000 geneinfo-3.4.2/geneinfo.egg-info/PKG-INFO
--rw-rw-r--   0 kmt       (6358) kmt       (6358)      228 2023-04-10 18:15:10.000000 geneinfo-3.4.2/geneinfo.egg-info/SOURCES.txt
--rw-rw-r--   0 kmt       (6358) kmt       (6358)        1 2023-04-10 18:15:09.000000 geneinfo-3.4.2/geneinfo.egg-info/dependency_links.txt
--rw-rw-r--   0 kmt       (6358) kmt       (6358)       68 2023-04-10 18:15:09.000000 geneinfo-3.4.2/geneinfo.egg-info/requires.txt
--rw-rw-r--   0 kmt       (6358) kmt       (6358)        9 2023-04-10 18:15:09.000000 geneinfo-3.4.2/geneinfo.egg-info/top_level.txt
--rw-rw-r--   0 kmt       (6358) kmt       (6358)       38 2023-04-10 18:15:11.147297 geneinfo-3.4.2/setup.cfg
--rw-rw-r--   0 kmt       (6358) kmt       (6358)      862 2023-04-10 18:13:45.000000 geneinfo-3.4.2/setup.py
+drwxrwxr-x   0 kmt       (6358) kmt       (6358)        0 2023-07-11 09:40:11.091822 geneinfo-3.4.3/
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)     1069 2023-04-25 13:25:03.000000 geneinfo-3.4.3/LICENSE
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)      491 2023-07-11 09:40:11.091822 geneinfo-3.4.3/PKG-INFO
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)      174 2023-04-25 13:25:03.000000 geneinfo-3.4.3/README.md
+drwxrwxr-x   0 kmt       (6358) kmt       (6358)        0 2023-07-11 09:40:11.087822 geneinfo-3.4.3/geneinfo/
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)    52678 2023-05-02 20:23:42.000000 geneinfo-3.4.3/geneinfo/__init__.py
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)     3385 2023-04-25 13:25:04.000000 geneinfo-3.4.3/geneinfo/intervals.py
+drwxrwxr-x   0 kmt       (6358) kmt       (6358)        0 2023-07-11 09:40:11.090822 geneinfo-3.4.3/geneinfo.egg-info/
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)      491 2023-07-11 09:40:11.000000 geneinfo-3.4.3/geneinfo.egg-info/PKG-INFO
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)      228 2023-07-11 09:40:11.000000 geneinfo-3.4.3/geneinfo.egg-info/SOURCES.txt
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)        1 2023-07-11 09:40:11.000000 geneinfo-3.4.3/geneinfo.egg-info/dependency_links.txt
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)       68 2023-07-11 09:40:11.000000 geneinfo-3.4.3/geneinfo.egg-info/requires.txt
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)        9 2023-07-11 09:40:11.000000 geneinfo-3.4.3/geneinfo.egg-info/top_level.txt
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)       38 2023-07-11 09:40:11.091822 geneinfo-3.4.3/setup.cfg
+-rw-rw-r--   0 kmt       (6358) kmt       (6358)      862 2023-07-11 09:38:22.000000 geneinfo-3.4.3/setup.py
```

### Comparing `geneinfo-3.4.2/LICENSE` & `geneinfo-3.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `geneinfo-3.4.2/geneinfo/__init__.py` & `geneinfo-3.4.3/geneinfo/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -349,15 +349,15 @@
 
     if plotted_intervals:
         offset = max(plotted_intervals.keys())
     else:
         offset = 1
 
     if hard_limits:
-        axex[-1].set_xlim(start, end)
+        axes[-1].set_xlim(start, end)
     else:
         s, e = axes[-1].get_xlim()
         axes[-1].set_xlim(min(s-label_width/2, start), max(e, end))
 
     axes[-1].set_ylim(-2, offset+2)
     axes[-1].get_yaxis().set_visible(False)
     axes[-1].invert_yaxis()
@@ -368,15 +368,18 @@
     for ax in axes[:-1]:
         ax.set_xlim(axes[-1].get_xlim())
 
         if despine:
             ax.spines['top'].set_visible(False)
             ax.spines['right'].set_visible(False)
     
-    return axes[:-1]
+    if return_axes == 1:
+        return axes[0]
+    else:
+        return axes[:-1]
 
 
 ##################################################################################
 # Map between assembly coordinates
 ##################################################################################
 
 def map_interval(chrom, start, end, strand, map_from, map_to, species='homo_sapiens'):
@@ -593,24 +596,30 @@
 
 
 def _cached_symbol2ncbi(symbols, taxid=9606):
 
     symbol2ncbi_file = f'geneinfo_cache/{taxid}_symbol2ncbi.h5'
     symbol2ncbi = pd.read_hdf(symbol2ncbi_file, 'symbol2ncbi')
     try:    
-        return symbol2ncbi.loc[symbols].tolist()
+        return symbol2ncbi.loc[symbols].tolist() 
     except KeyError:
         geneids = []
         for symbol in symbols:
             try:
                 geneids.append(symbol2ncbi.loc[symbol])
             except KeyError:
                 try:
-                    geneids.append(symbol2ncbi.loc[hgcn_symbol(symbol)])
-                    # geneids.append(ensembl2ncbi(ensembl_id(symbol)))
+                    ncbi_id = hgcn_symbol(symbol)
+                    if ncbi_id not in symbol2ncbi.index:
+                        print(ncbi_id, 'not in symbol2ncbi index')
+                        raise NotFound
+                        
+                        
+                    geneids.append(symbol2ncbi.loc[ncbi_id])
+                    # geneids.append(ensembl2ncbi(ensembl_id(symbol)))                    
                 except NotFound:
                     print(f'Could not map "{symbol}" to ncbi id', file=sys.stderr)
         return geneids
 
 
 def _cached_ncbi2symbol(geneids, taxid=9606):
```

### Comparing `geneinfo-3.4.2/geneinfo/intervals.py` & `geneinfo-3.4.3/geneinfo/intervals.py`

 * *Files identical despite different names*

### Comparing `geneinfo-3.4.2/setup.py` & `geneinfo-3.4.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name="geneinfo",
-    version="3.4.2",
+    version="3.4.3",
     author="Kasper Munch",
     author_email="kaspermunch@birc.au.dk",
     description="Functions for showing gene information in jupyter notebooks.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kaspermunch/geneinfo",
     packages=setuptools.find_packages(),
```

