# Comparing `tmp/rateToolsAC4RM-0.44.tar.gz` & `tmp/rateToolsAC4RM-0.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rateToolsAC4RM-0.44.tar", last modified: Fri Jul  7 21:33:18 2023, max compression
+gzip compressed data, was "rateToolsAC4RM-0.45.tar", last modified: Tue Jul 11 21:43:53 2023, max compression
```

## Comparing `rateToolsAC4RM-0.44.tar` & `rateToolsAC4RM-0.45.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 tleitch1   (501) staff       (20)        0 2023-07-07 21:33:18.316271 rateToolsAC4RM-0.44/
--rw-r--r--   0 tleitch1   (501) staff       (20)      190 2023-07-07 21:33:18.316400 rateToolsAC4RM-0.44/PKG-INFO
-drwxr-xr-x   0 tleitch1   (501) staff       (20)        0 2023-07-07 21:33:18.313349 rateToolsAC4RM-0.44/rateToolsAC4RM/
--rw-rw-r--   0 tleitch1   (501) staff       (20)      443 2023-07-07 21:32:20.000000 rateToolsAC4RM-0.44/rateToolsAC4RM/__init__.py
--rw-r--r--   0 tleitch1   (501) staff       (20)     6789 2023-07-07 21:32:10.000000 rateToolsAC4RM-0.44/rateToolsAC4RM/rateTools.py
-drwxr-xr-x   0 tleitch1   (501) staff       (20)        0 2023-07-07 21:33:18.315951 rateToolsAC4RM-0.44/rateToolsAC4RM.egg-info/
--rw-r--r--   0 tleitch1   (501) staff       (20)      190 2023-07-07 21:33:18.000000 rateToolsAC4RM-0.44/rateToolsAC4RM.egg-info/PKG-INFO
--rw-r--r--   0 tleitch1   (501) staff       (20)      262 2023-07-07 21:33:18.000000 rateToolsAC4RM-0.44/rateToolsAC4RM.egg-info/SOURCES.txt
--rw-r--r--   0 tleitch1   (501) staff       (20)        1 2023-07-07 21:33:18.000000 rateToolsAC4RM-0.44/rateToolsAC4RM.egg-info/dependency_links.txt
--rw-r--r--   0 tleitch1   (501) staff       (20)        1 2023-06-20 03:42:27.000000 rateToolsAC4RM-0.44/rateToolsAC4RM.egg-info/not-zip-safe
--rw-r--r--   0 tleitch1   (501) staff       (20)       15 2023-07-07 21:33:18.000000 rateToolsAC4RM-0.44/rateToolsAC4RM.egg-info/top_level.txt
--rw-rw-r--   0 tleitch1   (501) staff       (20)       38 2023-07-07 21:33:18.317047 rateToolsAC4RM-0.44/setup.cfg
--rw-rw-r--   0 tleitch1   (501) staff       (20)      227 2023-07-07 21:32:38.000000 rateToolsAC4RM-0.44/setup.py
+drwxr-xr-x   0 tleitch1   (501) staff       (20)        0 2023-07-11 21:43:53.893619 rateToolsAC4RM-0.45/
+-rw-r--r--   0 tleitch1   (501) staff       (20)      190 2023-07-11 21:43:53.893750 rateToolsAC4RM-0.45/PKG-INFO
+drwxr-xr-x   0 tleitch1   (501) staff       (20)        0 2023-07-11 21:43:53.890273 rateToolsAC4RM-0.45/rateToolsAC4RM/
+-rw-rw-r--   0 tleitch1   (501) staff       (20)      480 2023-07-11 21:41:57.000000 rateToolsAC4RM-0.45/rateToolsAC4RM/__init__.py
+-rw-r--r--   0 tleitch1   (501) staff       (20)     8154 2023-07-11 21:41:20.000000 rateToolsAC4RM-0.45/rateToolsAC4RM/rateTools.py
+drwxr-xr-x   0 tleitch1   (501) staff       (20)        0 2023-07-11 21:43:53.893278 rateToolsAC4RM-0.45/rateToolsAC4RM.egg-info/
+-rw-r--r--   0 tleitch1   (501) staff       (20)      190 2023-07-11 21:43:53.000000 rateToolsAC4RM-0.45/rateToolsAC4RM.egg-info/PKG-INFO
+-rw-r--r--   0 tleitch1   (501) staff       (20)      262 2023-07-11 21:43:53.000000 rateToolsAC4RM-0.45/rateToolsAC4RM.egg-info/SOURCES.txt
+-rw-r--r--   0 tleitch1   (501) staff       (20)        1 2023-07-11 21:43:53.000000 rateToolsAC4RM-0.45/rateToolsAC4RM.egg-info/dependency_links.txt
+-rw-r--r--   0 tleitch1   (501) staff       (20)        1 2023-06-20 03:42:27.000000 rateToolsAC4RM-0.45/rateToolsAC4RM.egg-info/not-zip-safe
+-rw-r--r--   0 tleitch1   (501) staff       (20)       15 2023-07-11 21:43:53.000000 rateToolsAC4RM-0.45/rateToolsAC4RM.egg-info/top_level.txt
+-rw-rw-r--   0 tleitch1   (501) staff       (20)       38 2023-07-11 21:43:53.894511 rateToolsAC4RM-0.45/setup.cfg
+-rw-rw-r--   0 tleitch1   (501) staff       (20)      227 2023-07-11 21:43:19.000000 rateToolsAC4RM-0.45/setup.py
```

### Comparing `rateToolsAC4RM-0.44/rateToolsAC4RM/rateTools.py` & `rateToolsAC4RM-0.45/rateToolsAC4RM/rateTools.py`

 * *Files 8% similar despite different names*

```diff
@@ -203,15 +203,15 @@
   totCF=np.zeros(10)
   from operator import add
   for t,rate,cf in assets:
     cfa=np.array(cf)
     totCF[:len(cfa)]+=cfa
   return(totCF)
 
-
+#######################
 # Now we define a function that finds the hedges for the total cashflows
 # that breaks it into hedge ratios for each forward swap by starting at
 # the end and works into front of curve
 
 import pandas as pd
 def portfolioHedge(portFwd01,mktFwd01):
   hRatio=[]
@@ -221,17 +221,69 @@
     tmpMktFwd01=np.array(mktFwd01[i-1][2])
     hr=tmpPortFwd01/tmpMktFwd01[i]
     hRatio.insert(0,[i,i+1,hr])
   hrDF=pd.DataFrame(hRatio)
   hrDF.columns=["start","end","fwdHR"]
 
   return(hrDF)
-
+#######################
 # Now let's turn our hedge into an equivalent cashflow for our swaps hedges
 def hedgeCF(fwdMktCF,hedgeRatios):
   cfs=[]
   for cf,hr in zip(fwdMktCF,hedgeRatios):
     cfs.append([0,0,[ x * hr for x in cf ]])
   
   return(sumCF(cfs))
 
 
+# here we define a function to generate the 
+def psaSimulation(ppmts,psa,pSchedule,pmts,rate,up=1.5,dn=.5):
+  # ppmts - regular principal payments w/o prepay
+  # psa - periodic prepayment rates
+  # pSchedule - prinipal schedule assuming no prepay
+  # total - payment interest+principal for no prepay
+  # rate - mortgage rate
+  # up - up move multiplier for psa sim
+  # dn - dn move multiplier for psa sim
+
+  cfPSAup=[]
+  cfPSAdn=[]
+  cfPSA=[]
+  cf=[]
+
+  # initialize for loop
+  bal=balUp=balDn=1000
+  rateLoss=0
+  rateLossUp=0
+  rateLossDn=0
+  for ppmt,cpr,currBal,pmt in zip(ppmts,psa,principalSched['schedule'],pmts):
+    
+    tmpBal=bal+ppmt-cpr*bal-rateLoss
+    if tmpBal>0:
+      cfPSA.append(-pmt)
+      bal=tmpBal
+      rateLoss=(currBal-bal)*rate
+    else:
+      cfPSA.append(bal)
+      bal=0
+
+    tmpBalup=balUp+ppmt-up*cpr*balUp-rateLossUp
+    if tmpBalup>0:
+      cfPSAup.append(-pmt)
+      balUp=tmpBalup
+      rateLossUp=(currBal-balUp)*rate
+    else:
+      cfPSAup.append(balUp)
+      balUp=0
+
+    tmpBalDn=balDn+ppmt-dn*cpr*balDn-rateLossDn
+    if tmpBalDn>0:
+      cfPSAdn.append(-pmt)
+      balDn=tmpBalDn
+      rateLossDn=(currBal-balDn)*rate
+    else:
+      cfPSAdn.append(balDn)
+      balDn=0
+
+  psaSim=pd.DataFrame({'cf': -pmt,'psaCF':cfPSA,'psaUpCF':cfPSAup,'psaDnCF':cfPSAdn})
+  
+  return(psaSim)
```

