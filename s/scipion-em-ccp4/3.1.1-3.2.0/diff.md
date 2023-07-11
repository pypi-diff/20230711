# Comparing `tmp/scipion-em-ccp4-3.1.1.tar.gz` & `tmp/scipion-em-ccp4-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-ccp4-3.1.1.tar", last modified: Fri Dec 23 10:45:54 2022, max compression
+gzip compressed data, was "scipion-em-ccp4-3.2.0.tar", last modified: Tue Jul 11 11:56:18 2023, max compression
```

## Comparing `scipion-em-ccp4-3.1.1.tar` & `scipion-em-ccp4-3.2.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 10:45:54.646377 scipion-em-ccp4-3.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2022-12-23 10:41:49.000000 scipion-em-ccp4-3.1.1/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2022-12-23 10:41:49.000000 scipion-em-ccp4-3.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       72 2022-12-23 10:41:49.000000 scipion-em-ccp4-3.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2022-12-23 10:45:54.646377 scipion-em-ccp4-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2022-12-23 10:41:49.000000 scipion-em-ccp4-3.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 10:45:54.642377 scipion-em-ccp4-3.1.1/ccp4/
--rw-r--r--   0 runner    (1001) docker     (123)     6808 2022-12-23 10:41:49.000000 scipion-em-ccp4-3.1.1/ccp4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2022-12-23 10:41:49.000000 scipion-em-ccp4-3.1.1/ccp4/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2022-12-23 10:41:49.000000 scipion-em-ccp4-3.1.1/ccp4/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2022-12-23 10:41:49.000000 scipion-em-ccp4-3.1.1/ccp4/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 10:45:54.642377 scipion-em-ccp4-3.1.1/ccp4/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2022-12-23 10:41:49.000000 scipion-em-ccp4-3.1.1/ccp4/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32761 2022-12-23 10:41:49.000000 scipion-em-ccp4-3.1.1/ccp4/protocols/protocol_coot.py
--rw-r--r--   0 runner    (1001) docker     (123)    16309 2022-12-23 10:41:49.000000 scipion-em-ccp4-3.1.1/ccp4/protocols/protocol_refmac.py
--rw-r--r--   0 runner    (1001) docker     (123)     4919 2022-12-23 10:41:49.000000 scipion-em-ccp4-3.1.1/ccp4/protocols/refmac_template_map2mtz.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2022-12-23 10:41:49.000000 scipion-em-ccp4-3.1.1/ccp4/protocols/refmac_template_refine.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2022-12-23 10:41:49.000000 scipion-em-ccp4-3.1.1/ccp4/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 10:45:54.646377 scipion-em-ccp4-3.1.1/ccp4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2022-12-23 10:41:49.000000 scipion-em-ccp4-3.1.1/ccp4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32835 2022-12-23 10:41:49.000000 scipion-em-ccp4-3.1.1/ccp4/tests/test_protocol_coot_refmac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 10:45:54.646377 scipion-em-ccp4-3.1.1/ccp4/viewers/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2022-12-23 10:41:49.000000 scipion-em-ccp4-3.1.1/ccp4/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2022-12-23 10:41:49.000000 scipion-em-ccp4-3.1.1/ccp4/viewers/viewer_coot.py
--rw-r--r--   0 runner    (1001) docker     (123)    23750 2022-12-23 10:41:49.000000 scipion-em-ccp4-3.1.1/ccp4/viewers/viewer_refmac.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2022-12-23 10:41:49.000000 scipion-em-ccp4-3.1.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-23 10:45:54.646377 scipion-em-ccp4-3.1.1/scipion_em_ccp4.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2022-12-23 10:45:54.000000 scipion-em-ccp4-3.1.1/scipion_em_ccp4.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      712 2022-12-23 10:45:54.000000 scipion-em-ccp4-3.1.1/scipion_em_ccp4.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-23 10:45:54.000000 scipion-em-ccp4-3.1.1/scipion_em_ccp4.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2022-12-23 10:45:54.000000 scipion-em-ccp4-3.1.1/scipion_em_ccp4.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2022-12-23 10:45:54.000000 scipion-em-ccp4-3.1.1/scipion_em_ccp4.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2022-12-23 10:45:54.000000 scipion-em-ccp4-3.1.1/scipion_em_ccp4.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-23 10:45:54.646377 scipion-em-ccp4-3.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6511 2022-12-23 10:41:49.000000 scipion-em-ccp4-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:56:18.753704 scipion-em-ccp4-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-11 11:54:36.000000 scipion-em-ccp4-3.2.0/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-11 11:54:36.000000 scipion-em-ccp4-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 11:54:36.000000 scipion-em-ccp4-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-07-11 11:56:18.753704 scipion-em-ccp4-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-11 11:54:36.000000 scipion-em-ccp4-3.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:56:18.753704 scipion-em-ccp4-3.2.0/ccp4/
+-rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-07-11 11:54:36.000000 scipion-em-ccp4-3.2.0/ccp4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-07-11 11:54:36.000000 scipion-em-ccp4-3.2.0/ccp4/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-11 11:54:36.000000 scipion-em-ccp4-3.2.0/ccp4/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-11 11:54:36.000000 scipion-em-ccp4-3.2.0/ccp4/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:56:18.753704 scipion-em-ccp4-3.2.0/ccp4/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-11 11:54:36.000000 scipion-em-ccp4-3.2.0/ccp4/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33364 2023-07-11 11:54:36.000000 scipion-em-ccp4-3.2.0/ccp4/protocols/protocol_coot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16309 2023-07-11 11:54:36.000000 scipion-em-ccp4-3.2.0/ccp4/protocols/protocol_refmac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-07-11 11:54:36.000000 scipion-em-ccp4-3.2.0/ccp4/protocols/refmac_template_map2mtz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-07-11 11:54:36.000000 scipion-em-ccp4-3.2.0/ccp4/protocols/refmac_template_refine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-11 11:54:36.000000 scipion-em-ccp4-3.2.0/ccp4/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:56:18.753704 scipion-em-ccp4-3.2.0/ccp4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-11 11:54:36.000000 scipion-em-ccp4-3.2.0/ccp4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32835 2023-07-11 11:54:36.000000 scipion-em-ccp4-3.2.0/ccp4/tests/test_protocol_coot_refmac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:56:18.753704 scipion-em-ccp4-3.2.0/ccp4/viewers/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-11 11:54:36.000000 scipion-em-ccp4-3.2.0/ccp4/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-07-11 11:54:36.000000 scipion-em-ccp4-3.2.0/ccp4/viewers/viewer_coot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23750 2023-07-11 11:54:36.000000 scipion-em-ccp4-3.2.0/ccp4/viewers/viewer_refmac.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-11 11:54:36.000000 scipion-em-ccp4-3.2.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 11:56:18.753704 scipion-em-ccp4-3.2.0/scipion_em_ccp4.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-07-11 11:56:18.000000 scipion-em-ccp4-3.2.0/scipion_em_ccp4.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-11 11:56:18.000000 scipion-em-ccp4-3.2.0/scipion_em_ccp4.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 11:56:18.000000 scipion-em-ccp4-3.2.0/scipion_em_ccp4.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-11 11:56:18.000000 scipion-em-ccp4-3.2.0/scipion_em_ccp4.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-11 11:56:18.000000 scipion-em-ccp4-3.2.0/scipion_em_ccp4.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-11 11:56:18.000000 scipion-em-ccp4-3.2.0/scipion_em_ccp4.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 11:56:18.753704 scipion-em-ccp4-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6511 2023-07-11 11:54:36.000000 scipion-em-ccp4-3.2.0/setup.py
```

### Comparing `scipion-em-ccp4-3.1.1/LICENSE` & `scipion-em-ccp4-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-ccp4-3.1.1/PKG-INFO` & `scipion-em-ccp4-3.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: scipion-em-ccp4
-Version: 3.1.1
+Version: 3.2.0
 Summary: CCP4 model building programs in Scipion. Warning: Install CCP4 v. 7.0.56 or higher
 Home-page: https://github.com/scipion-em/scipion-em-ccp4
 Author: Roberto Marabini and Marta Martinez
 Author-email: scipion@cnb.csic.es
 License: UNKNOWN
 Description: ===================
         CCP4 scipion plugin
@@ -84,15 +84,15 @@
         
         
         
         ========
         Examples
         ========
         
-        See `Model Building Tutorial <https://github.com/I2PC/scipion/wiki/tutorials/tutorial_model_building_basic.pdf>`_
+        See `Model Building Tutorial <https://scipion-em.github.io/docs/release-3.0.0/docs/user/user-documentation.html#model-building>`_
         
         
         
         ===============
         Buildbot status
         ===============
```

### Comparing `scipion-em-ccp4-3.1.1/README.rst` & `scipion-em-ccp4-3.2.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
 
 
 ========
 Examples
 ========
 
-See `Model Building Tutorial <https://github.com/I2PC/scipion/wiki/tutorials/tutorial_model_building_basic.pdf>`_
+See `Model Building Tutorial <https://scipion-em.github.io/docs/release-3.0.0/docs/user/user-documentation.html#model-building>`_
 
 
 
 ===============
 Buildbot status
 ===============
```

### Comparing `scipion-em-ccp4-3.1.1/ccp4/__init__.py` & `scipion-em-ccp4-3.2.0/ccp4/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 import pyworkflow.utils as pwutils
 import getpass
 
 from ccp4.constants import *
 
 _references = ['Winn_2011']
 _logo = "ccp4_200.png"
-__version__ = "3.1.1"
+__version__ = "3.2.0"
 
 class Plugin(pwem.Plugin):
     _homeVar = CCP4_HOME_VARNAME
     _versions = {'CCP4': [V7_0]}
 
     @classmethod
     def _defineVariables(cls):
@@ -127,22 +127,22 @@
             'CCP4I_TOP': os.path.join(_ccp4_home, 'share', 'ccp4i'),
             # # MMCIFDIC: platform-dependent (not in $CLIBD) data file for
             # # the ccif library
             # export MMCIFDIC=$CLIB/ccp4/cif_mmdic.lib
             'MMCIFDIC': os.path.join(_ccp4_home, 'lib', 'cif_mmdic.lib'),
             # # CLIBD_MON: dictionary files for REFMAC5 (keep trailing /)
             # export CLIBD_MON=$CCP4/lib/data/monomers/
-            'CLIBD_MON': os.path.join(_ccp4_home, 'lib', 'data', 'monomers'),
+            'CLIBD_MON': os.path.join(_ccp4_home, 'lib', 'data', 'monomers/'),
             # # CRANK: location of Crank automation suite within ccp4i
             # export CRANK=$CCP4I_TOP/crank
             'CRANK': os.path.join(_ccp4_home, 'crank'),
             # # CCP4_HELPDIR: location of the VMS-style help file used
             # # by (ip)mosflm
             # export CCP4_HELPDIR=$CCP4/help/            # NB trailing /
-            'CCP4_HELPDIR': os.path.join(_ccp4_home, 'help'),
+            'CCP4_HELPDIR': os.path.join(_ccp4_home, 'help/'),
         }, position=pwutils.Environ.REPLACE)  # replace
 
         return environ
 
     @classmethod
     def isVersionActive(cls):
         return cls.getActiveVersion().startswith(V7_0)
```

### Comparing `scipion-em-ccp4-3.1.1/ccp4/bibtex.py` & `scipion-em-ccp4-3.2.0/ccp4/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-ccp4-3.1.1/ccp4/convert.py` & `scipion-em-ccp4-3.2.0/ccp4/convert.py`

 * *Files identical despite different names*

### Comparing `scipion-em-ccp4-3.1.1/ccp4/protocols/protocol_coot.py` & `scipion-em-ccp4-3.2.0/ccp4/protocols/protocol_coot.py`

 * *Files 3% similar despite different names*

```diff
@@ -275,15 +275,22 @@
         if len(self.phythonscript.get()) > 1:
             args += " --script {phythonscript}".format(
                 phythonscript=self.phythonscript.get())
         # script with auxiliary files
         self._log.info('Launching: ' + Plugin.getProgram(self.COOT) + ' ' + args)
 
         # run in the background
-        runCCP4Program(Plugin.getProgram(self.COOT), args)
+        try:
+            runCCP4Program(Plugin.getProgram(self.COOT), args)
+        except Exception as e:
+            print(pwutils.redStr("=============================================================="))
+            print(pwutils.redStr("ERROR: Coot execution failed"))
+            print(pwutils.redStr("Last SAVED atomic model will be shown if protocol is continued"))
+            print(pwutils.redStr("=============================================================="))
+ 
         self.createOutput()
 
     def createOutput(self):
         """ Copy the PDB structure and register the output object.
         """
         databasePath = self._getExtraPath(OUTPUTDATABASENAMESWITHLABELS)
         getModels(databasePath, DATABASETABLENAME)
@@ -444,16 +451,20 @@
         while os.path.isfile(template % counter):
             counter += 1
         return counter  # returns next free
 
 cootScriptHeader = '''import ConfigParser
 import os
 import subprocess
-import coot_python
-
+try:
+    import coot_python
+    has_gui = True
+except:
+    print("ERROR: coot_python module not found. If you are running in no gui mode this is OK")
+    has_gui = False
 mydict={{}}
 mydict['imol']={imol}
 mydict['aa_main_chain']="A"
 mydict['aa_auxiliary_chain']="AA"
 mydict['aaNumber']=17
 mydict['step']=5
 mydict['outfile'] = '{templateNameAtomStruct}'
@@ -658,20 +669,21 @@
     beep(0.1)
     coot_real_exit(0)
 
 
 # create scipion menu
 print("Loading Scipion Coot extensions...")
 
-menubar = coot_python.main_menubar()
-toolbar = coot_python.main_toolbar()
-menu = coot_menubar_menu("Scipion")
-add_simple_coot_menu_menuitem(menu, "write last active model", lambda func: _write(imol = -1))
-add_simple_coot_menu_menuitem(menu, "end protocol", lambda func: _finishProj())
-add_simple_coot_menu_menuitem(menu, "update cootini", lambda func: _updateMol())
+if has_gui: 
+    menubar = coot_python.main_menubar()
+    toolbar = coot_python.main_toolbar()
+    menu = coot_menubar_menu("Scipion")
+    add_simple_coot_menu_menuitem(menu, "write last active model", lambda func: _write(imol = -1))
+    add_simple_coot_menu_menuitem(menu, "end protocol", lambda func: _finishProj())
+    add_simple_coot_menu_menuitem(menu, "update cootini", lambda func: _updateMol())
 
 #change chain id
 add_key_binding("change_chain_id_down","x", lambda: _change_chain_id(-1))
 add_key_binding("change_chain_id_down","X", lambda: _change_chain_id(1))
 
 #refine aminoacid segment
 add_key_binding("refine zone m","z", lambda: _refine_zone(1))
```

### Comparing `scipion-em-ccp4-3.1.1/ccp4/protocols/protocol_refmac.py` & `scipion-em-ccp4-3.2.0/ccp4/protocols/protocol_refmac.py`

 * *Files identical despite different names*

### Comparing `scipion-em-ccp4-3.1.1/ccp4/protocols/refmac_template_map2mtz.py` & `scipion-em-ccp4-3.2.0/ccp4/protocols/refmac_template_map2mtz.py`

 * *Files identical despite different names*

### Comparing `scipion-em-ccp4-3.1.1/ccp4/protocols/refmac_template_refine.py` & `scipion-em-ccp4-3.2.0/ccp4/protocols/refmac_template_refine.py`

 * *Files identical despite different names*

### Comparing `scipion-em-ccp4-3.1.1/ccp4/protocols.conf` & `scipion-em-ccp4-3.2.0/ccp4/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-ccp4-3.1.1/ccp4/tests/test_protocol_coot_refmac.py` & `scipion-em-ccp4-3.2.0/ccp4/tests/test_protocol_coot_refmac.py`

 * *Files identical despite different names*

### Comparing `scipion-em-ccp4-3.1.1/ccp4/viewers/viewer_coot.py` & `scipion-em-ccp4-3.2.0/ccp4/viewers/viewer_coot.py`

 * *Files identical despite different names*

### Comparing `scipion-em-ccp4-3.1.1/ccp4/viewers/viewer_refmac.py` & `scipion-em-ccp4-3.2.0/ccp4/viewers/viewer_refmac.py`

 * *Files identical despite different names*

### Comparing `scipion-em-ccp4-3.1.1/scipion_em_ccp4.egg-info/PKG-INFO` & `scipion-em-ccp4-3.2.0/scipion_em_ccp4.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: scipion-em-ccp4
-Version: 3.1.1
+Version: 3.2.0
 Summary: CCP4 model building programs in Scipion. Warning: Install CCP4 v. 7.0.56 or higher
 Home-page: https://github.com/scipion-em/scipion-em-ccp4
 Author: Roberto Marabini and Marta Martinez
 Author-email: scipion@cnb.csic.es
 License: UNKNOWN
 Description: ===================
         CCP4 scipion plugin
@@ -84,15 +84,15 @@
         
         
         
         ========
         Examples
         ========
         
-        See `Model Building Tutorial <https://github.com/I2PC/scipion/wiki/tutorials/tutorial_model_building_basic.pdf>`_
+        See `Model Building Tutorial <https://scipion-em.github.io/docs/release-3.0.0/docs/user/user-documentation.html#model-building>`_
         
         
         
         ===============
         Buildbot status
         ===============
```

### Comparing `scipion-em-ccp4-3.1.1/scipion_em_ccp4.egg-info/SOURCES.txt` & `scipion-em-ccp4-3.2.0/scipion_em_ccp4.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-ccp4-3.1.1/setup.py` & `scipion-em-ccp4-3.2.0/setup.py`

 * *Files identical despite different names*

