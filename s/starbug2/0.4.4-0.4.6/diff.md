# Comparing `tmp/starbug2-0.4.4.tar.gz` & `tmp/starbug2-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starbug2-0.4.4.tar", last modified: Thu Jun 15 16:01:57 2023, max compression
+gzip compressed data, was "starbug2-0.4.6.tar", last modified: Tue Jul 11 10:35:29 2023, max compression
```

## Comparing `starbug2-0.4.4.tar` & `starbug2-0.4.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:01:57.097130 starbug2-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-15 16:01:45.000000 starbug2-0.4.4/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-15 16:01:45.000000 starbug2-0.4.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-15 16:01:45.000000 starbug2-0.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-06-15 16:01:57.097130 starbug2-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-06-15 16:01:45.000000 starbug2-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:01:57.093130 starbug2-0.4.4/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)    13797 2023-06-15 16:01:45.000000 starbug2-0.4.4/bin/starbug2
--rwxr-xr-x   0 runner    (1001) docker     (123)     7096 2023-06-15 16:01:45.000000 starbug2-0.4.4/bin/starbug2-match
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:01:57.093130 starbug2-0.4.4/extras/
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-06-15 16:01:45.000000 starbug2-0.4.4/extras/starbug2.completion
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-15 16:01:45.000000 starbug2-0.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-15 16:01:57.097130 starbug2-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-15 16:01:45.000000 starbug2-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:01:57.093130 starbug2-0.4.4/starbug2/
--rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-06-15 16:01:45.000000 starbug2-0.4.4/starbug2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-06-15 16:01:45.000000 starbug2-0.4.4/starbug2/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)    15388 2023-06-15 16:01:45.000000 starbug2-0.4.4/starbug2/matching.py
--rw-r--r--   0 runner    (1001) docker     (123)     6805 2023-06-15 16:01:45.000000 starbug2-0.4.4/starbug2/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:01:57.097130 starbug2-0.4.4/starbug2/param/
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-06-15 16:01:45.000000 starbug2-0.4.4/starbug2/param/default.param
--rw-r--r--   0 runner    (1001) docker     (123)    28598 2023-06-15 16:01:45.000000 starbug2-0.4.4/starbug2/routines.py
--rw-r--r--   0 runner    (1001) docker     (123)    31810 2023-06-15 16:01:45.000000 starbug2-0.4.4/starbug2/starbug.py
--rw-r--r--   0 runner    (1001) docker     (123)    10451 2023-06-15 16:01:45.000000 starbug2-0.4.4/starbug2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:01:57.097130 starbug2-0.4.4/starbug2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-06-15 16:01:57.000000 starbug2-0.4.4/starbug2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-15 16:01:57.000000 starbug2-0.4.4/starbug2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 16:01:57.000000 starbug2-0.4.4/starbug2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-15 16:01:57.000000 starbug2-0.4.4/starbug2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-15 16:01:57.000000 starbug2-0.4.4/starbug2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 16:01:57.097130 starbug2-0.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-15 16:01:45.000000 starbug2-0.4.4/tests/test_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-06-15 16:01:45.000000 starbug2-0.4.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:35:29.365796 starbug2-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-11 10:35:19.000000 starbug2-0.4.6/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-11 10:35:19.000000 starbug2-0.4.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-11 10:35:19.000000 starbug2-0.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-07-11 10:35:29.365796 starbug2-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-07-11 10:35:19.000000 starbug2-0.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:35:29.357796 starbug2-0.4.6/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13797 2023-07-11 10:35:19.000000 starbug2-0.4.6/bin/starbug2
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7121 2023-07-11 10:35:19.000000 starbug2-0.4.6/bin/starbug2-match
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:35:29.357796 starbug2-0.4.6/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-11 10:35:19.000000 starbug2-0.4.6/extras/starbug2.completion
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-11 10:35:19.000000 starbug2-0.4.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-11 10:35:29.365796 starbug2-0.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-11 10:35:19.000000 starbug2-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:35:29.361796 starbug2-0.4.6/starbug2/
+-rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-07-11 10:35:19.000000 starbug2-0.4.6/starbug2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-07-11 10:35:19.000000 starbug2-0.4.6/starbug2/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15746 2023-07-11 10:35:19.000000 starbug2-0.4.6/starbug2/matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-07-11 10:35:19.000000 starbug2-0.4.6/starbug2/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:35:29.361796 starbug2-0.4.6/starbug2/param/
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-07-11 10:35:19.000000 starbug2-0.4.6/starbug2/param/default.param
+-rw-r--r--   0 runner    (1001) docker     (123)    28598 2023-07-11 10:35:19.000000 starbug2-0.4.6/starbug2/routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31810 2023-07-11 10:35:19.000000 starbug2-0.4.6/starbug2/starbug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10543 2023-07-11 10:35:19.000000 starbug2-0.4.6/starbug2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:35:29.361796 starbug2-0.4.6/starbug2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-07-11 10:35:29.000000 starbug2-0.4.6/starbug2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-11 10:35:29.000000 starbug2-0.4.6/starbug2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 10:35:29.000000 starbug2-0.4.6/starbug2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-11 10:35:29.000000 starbug2-0.4.6/starbug2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 10:35:29.000000 starbug2-0.4.6/starbug2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 10:35:29.361796 starbug2-0.4.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-11 10:35:19.000000 starbug2-0.4.6/tests/test_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-07-11 10:35:19.000000 starbug2-0.4.6/tests/test_utils.py
```

### Comparing `starbug2-0.4.4/LICENSE.txt` & `starbug2-0.4.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `starbug2-0.4.4/PKG-INFO` & `starbug2-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starbug2
-Version: 0.4.4
+Version: 0.4.6
 Summary: JWST PSF photometry in complex crowded fields.
 Author: Conor Nally
 Author-email: conor.nally@ed.ac.uk
 License: GNU General Public License v3.0
 Description-Content-Type: text/markdown
 
 # StarBugII
```

### Comparing `starbug2-0.4.4/README.md` & `starbug2-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `starbug2-0.4.4/bin/starbug2` & `starbug2-0.4.6/bin/starbug2`

 * *Files identical despite different names*

### Comparing `starbug2-0.4.4/bin/starbug2-match` & `starbug2-0.4.6/bin/starbug2-match`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
             utils.perror("Unable to determine filter of \"%s\"\n"%args[i])
 
 
 if options & BANDMATCH:
     #filters=[]
     tomatch={ starbug2.NIRCAM:[], starbug2.MIRI:[] }
     fname=output if output else "out.fits"
-    _colnames=["RA","DEC"]
+    _colnames=["RA","DEC","flag"]
 
     for i,(tab,fltr) in enumerate(zip(tables,filters)):
         tomatch[starbug2.filters[fltr].instr].append(tab)
         _colnames+=([fltr,"e%s"%fltr])
     
     if tomatch[starbug2.NIRCAM] and tomatch[starbug2.MIRI]:
         utils.printf("Detected NIRCam to MIRI matching\n")
@@ -171,14 +171,15 @@
     if options & DITHERMATCH: av,full=matching.dither_match(tables, threshold=dthreshold, colnames=colnames)
     if options & GENERICMATCH: 
         options|=EXPFULL
         av,full=matching.generic_match(tables,threshold=dthreshold, add_src=True)
         #av=None#_=matching.finish_matching(full, colnames=tables[0].colnames)
     else:
         av,full=matching.cascade_match(tables, threshold=dthreshold, colnames=colnames)
+        print(av)
 
     dtypes=[]
     for name in full.colnames:
         if name=="Catalogue_Number": dtypes.append(str)
         elif name=="flag": dtypes.append(np.uint16)
         else: dtypes.append(float)
     full=Table(full,dtype=dtypes).filled(np.nan) ## fill empty values with null
```

### Comparing `starbug2-0.4.4/extras/starbug2.completion` & `starbug2-0.4.6/extras/starbug2.completion`

 * *Files identical despite different names*

### Comparing `starbug2-0.4.4/starbug2/__init__.py` & `starbug2-0.4.6/starbug2/__init__.py`

 * *Files identical despite different names*

### Comparing `starbug2-0.4.4/starbug2/mask.py` & `starbug2-0.4.6/starbug2/mask.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,62 +2,65 @@
 import numpy as np
 from matplotlib.path import Path
 from matplotlib.patches import Polygon
 from astropy.table import Table
 from starbug2.utils import tab2array, colour_index
 
 class Mask(object):
-    def __init__(self, bounds, keys, label=None):
+    colour='k'
+    def __init__(self, bounds, keys, label=None, **kwargs):
         self.path=Path(bounds)
         if len(keys)==2:
             self.keys=keys
         else: raise Exception
         self.label=label
+        
+        if "colour" in kwargs: self.colour=kwargs.get("colour")
+
 
     def apply(self, dat):
         d=tab2array(colour_index(dat,self.keys))
-        print(d)
         return self.path.contains_points(d)
     
     @staticmethod
     def from_file(fname):
         with open(fname) as fp:
             return Mask.from_string(fp.readline())
     @staticmethod
     def from_string(string):
         """
         String Format:
             [-x XCOL] [-y YCOL] [-l Label] : x1 y1 x2 y2 x3 y3 ...
         """
         label=None
         keys=[None,None]
+        colour='k'
         _opts,_coords=string.split(':')
-        opts,args=getopt.getopt(_opts.split(' '), "l:x:y:")
+        opts,args=getopt.getopt(_opts.split(' '), "c:l:x:y:")
         for opt,optarg in opts:
             if opt=="-x": keys[0]=optarg
             if opt=="-y": keys[1]=optarg
-            if opt=="-l": label=optarg
+            if opt=="-l": label=optarg.replace('_',' ')
+            if opt=="-c": colour=optarg
         coords=_coords.strip().rstrip().split(' ')
-        print(coords)
         points=np.array(coords, dtype=float).reshape((int(len(coords)/2),2))
-        return Mask(points,keys,label=label)
+        return Mask(points,keys,label=label, colour=colour)
 
     def plot(self, ax, **kwargs):
-        patch=Polygon(self.path._vertices, label=self.label, **kwargs)
+        patch=Polygon(self.path._vertices, label=self.label.replace('_',' '), **kwargs)
         ax.add_patch(patch)
         
 
 
 
 if __name__=="__main__":
     s="-yF115W -xF115W-F200W -lTestCut 0 20 1 21 1 24 0 24"
     t=Table.read("/home/conor/sci/proj/ngc6822/paper1/dat/ngc6822.fits",format="fits").filled(np.nan)
     m=Mask.from_string(s)
     mask=m.apply(t)
-    print(sum(mask))
     import matplotlib.pyplot as plt
     tt=colour_index(t,("F115W-F200W","F115W"))
     plt.scatter(tt["F115W-F200W"], tt["F115W"], c='k', lw=0, s=1)
     #plt.scatter(tt["F115W-F200W"][mask], tt["F115W"][mask], c='r', lw=0, s=1, label=m.label)
     m.plot( plt.gca(), fill=False, edgecolor="blue", label="test")
     plt.legend()
     plt.show()
```

### Comparing `starbug2-0.4.4/starbug2/matching.py` & `starbug2-0.4.6/starbug2/matching.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,14 +167,15 @@
         a left aligned catalogue of all the matched values
     """
     threshold*=u.arcsec
     colnames= list( name for name in catalogues[0].colnames if name in colnames)
     ncol=len(colnames)
     base=Table( None, meta=catalogues[0].meta)#, names=colnames )
     load=loading(sum([len(cat) for cat in catalogues[1:]]),"matching")
+    fltr=find_filter(catalogues[0])
 
     for n,cat in enumerate(catalogues,1):
         if n==1:
             tmp=cat[colnames].copy()
         else:
             idx,d2d,_=_match(base,cat)
             #tmp=Table(np.full((len(base),ncol),np.nan), names=colnames)
@@ -194,15 +195,15 @@
                         tmp[drow]=src[colnames]
                         drow+=1 
                     else: 
                         tmp.add_row(src[colnames]) ##i can purely use add_row to simplifiy the code
         tmp.rename_columns(colnames, list("%s_%d"%(name,n) for name in colnames))
         base=hcascade((base,tmp), colnames=colnames)
     base=Table(base,dtype=[float]*len(base.colnames)).filled(np.nan)
-    return finish_matching(base, colnames)
+    return finish_matching(base, colnames, fltr=fltr)
 
 def band_match(catalogues, colnames=("RA","DEC")):
     """
     Given a list of catalogues (with filter names in the meta data), match them
     in order of decreasing astrometric accuracy. 
     If F115W, F444W, F770W are input, the F115W centroid positions will be 
     taken as "correct". If a source is not resolved in this band, the next most 
@@ -266,15 +267,16 @@
         #base=hstack(( base,tmp[["flux","eflux"]] ))
         #mag,magerr=flux2ABmag(tmp["flux"], tmp["eflux"],fltr)
         #base.add_column(mag,name=fltr)
         #base.add_column(magerr,name="e%s"%fltr)
 
         #base.rename_column("flux","%s_flux"%fltr)
         #base.rename_column("eflux","%s_eflux"%fltr)
-        base=hstack(( base,tmp[[fltr,"e%s"%fltr]] ))#.filled(np.nan)
+        print(tmp.colnames)
+        base=hstack(( base,tmp[[fltr,"e%s"%fltr,"flag"]] ))#.filled(np.nan)
         base=Table(base,dtype=[float]*len(base.colnames)).filled(np.nan)
 
         ### Only keep the most astromectrically correct position
         if "RA" not in base.colnames: base=hstack(( tmp[["RA","DEC"]], base))
         else:
             _mask=np.logical_and( np.isnan(base["RA"]), tmp["RA"]!=np.nan)
             base["RA"][_mask]=tmp["RA"][_mask]
@@ -305,20 +307,24 @@
     tab.add_column(mask, name="MASK")
 
     print(tab)
     return tab 
 
 
 
-def finish_matching(tab, colnames):
+def finish_matching(tab, colnames, fltr=None):
     """
     Averaging all the values. Combining source flags and building a NUM column
     """
     flags=np.full(len(tab),starbug2.SRC_GOOD, dtype=np.uint16)
     av=Table(np.full((len(tab),len(colnames)),np.nan), names=colnames)
+    if not fltr:
+        if not (fltr:=tab.meta.get("FILTER")):
+            if not (fltr:=find_filter(tab)):
+                fltr=None
 
     for name in colnames:
         all_cols=find_colnames(tab,name)
         #if not (all_cols:=find_colnames(tab,name)): continue
         if not all_cols: continue
         col=Column(None, name=name)
         ar=tab2array(tab, colnames=all_cols)
@@ -337,17 +343,20 @@
             for fcol in ar.T: col|=fcol.astype(np.uint16)
         elif name=="NUM":
             col=Column(np.nansum(ar, axis=1), name=name)
         else: col=Column(np.nanmedian(ar, axis=1),name=name)
         
         av[name]=col
     if len(set(["flux","eflux"])&set(av.colnames))==2:
-        mag,magerr=flux2ABmag(av["flux"],av["eflux"], tab.meta["FILTER"])
-        av.add_column(mag,name=tab.meta["FILTER"])
-        av.add_column(magerr,name="e%s"%tab.meta["FILTER"])
+        #fltr=av.meta.get("FILTER")
+        if fltr: 
+            mag,magerr=flux2ABmag(av["flux"],av["eflux"], fltr)
+            #if fltr not in tab.colnames: ## I cant remember what this is for
+            av.add_column(mag,name=tab.meta["FILTER"])
+            av.add_column(magerr,name="e%s"%tab.meta["FILTER"])
     if "NUM" not in av.colnames:
         narr= np.nansum( np.invert( np.isnan(tab2array(tab,find_colnames(tab,colnames[0])))),axis=1)
         av.add_column(Column(narr, name="NUM"))
     return (av,tab)
 
 
 def remove_NUM(tab, N):
```

### Comparing `starbug2-0.4.4/starbug2/misc.py` & `starbug2-0.4.6/starbug2/misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
     """
     printf("Calculating instrumental zeropoint.\n")
     if fltr is None and not (fltr:=psftable.meta.get("FILTER")):
         perror("Unable to determine filter, set with '--set FILTER=F000W'.\n")
         return None
     
 
-    matched=generic_match((psftable, aptable), threshold=0.1, add_src=False)
+    _,matched=generic_match((psftable, aptable), threshold=0.1, add_src=False)
     dist=np.array((matched["%s_2"%fltr]-matched["%s_1"%fltr]).value)
     zp=np.nanmedian(dist)
     std=np.nanstd(dist)
     printf("-> zp=%.3f +/- %.2g\n"%(zp,std))
     return (zp,std)
 #def tmpfn(psftable, aptable):
 #    if "flux" in psftable.colnames and "flux" in aptable.colnames:
```

### Comparing `starbug2-0.4.4/starbug2/param/default.param` & `starbug2-0.4.6/starbug2/param/default.param`

 * *Files identical despite different names*

### Comparing `starbug2-0.4.4/starbug2/routines.py` & `starbug2-0.4.6/starbug2/routines.py`

 * *Files identical despite different names*

### Comparing `starbug2-0.4.4/starbug2/starbug.py` & `starbug2-0.4.6/starbug2/starbug.py`

 * *Files identical despite different names*

### Comparing `starbug2-0.4.4/starbug2/utils.py` & `starbug2-0.4.6/starbug2/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -326,14 +326,16 @@
     Find the unit scale factor to convert an image from MJy/sr to Jy
     """
     scalefactor=1
     if ext.header["BUNIT"]=="MJy/sr":
         scalefactor=1e6*float(ext.header["PIXAR_SR"])
     return scalefactor
 
+def find_filter(table):
+    return [set(table.colnames)&set(starbug2.filters.keys())].pop()
 
 
 
 if __name__ == "__main__":
     print(starbug2.logo)
     t=Table.read("test/dat/image-ap.fits",format="fits")
     print(colour_index( t, ("flux", "flux-eflux") ) )
```

### Comparing `starbug2-0.4.4/starbug2.egg-info/PKG-INFO` & `starbug2-0.4.6/starbug2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starbug2
-Version: 0.4.4
+Version: 0.4.6
 Summary: JWST PSF photometry in complex crowded fields.
 Author: Conor Nally
 Author-email: conor.nally@ed.ac.uk
 License: GNU General Public License v3.0
 Description-Content-Type: text/markdown
 
 # StarBugII
```

### Comparing `starbug2-0.4.4/tests/test_routines.py` & `starbug2-0.4.6/tests/test_routines.py`

 * *Files identical despite different names*

### Comparing `starbug2-0.4.4/tests/test_utils.py` & `starbug2-0.4.6/tests/test_utils.py`

 * *Files identical despite different names*

