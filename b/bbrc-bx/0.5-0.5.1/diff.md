# Comparing `tmp/bbrc-bx-0.5.tar.gz` & `tmp/bbrc-bx-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbrc-bx-0.5.tar", last modified: Thu Feb  9 15:04:52 2023, max compression
+gzip compressed data, was "bbrc-bx-0.5.1.tar", last modified: Tue Jul 11 17:09:34 2023, max compression
```

## Comparing `bbrc-bx-0.5.tar` & `bbrc-bx-0.5.1.tar`

### file list

```diff
@@ -1,101 +1,106 @@
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-02-09 15:04:52.148724 bbrc-bx-0.5/
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)       71 2023-02-09 15:02:03.000000 bbrc-bx-0.5/MANIFEST.in
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    19972 2023-02-09 15:04:52.148724 bbrc-bx-0.5/PKG-INFO
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    15851 2023-02-09 15:02:03.000000 bbrc-bx-0.5/README.md
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-02-09 15:04:52.148724 bbrc-bx-0.5/bbrc_bx.egg-info/
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    19972 2023-02-09 15:04:52.000000 bbrc-bx-0.5/bbrc_bx.egg-info/PKG-INFO
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2365 2023-02-09 15:04:52.000000 bbrc-bx-0.5/bbrc_bx.egg-info/SOURCES.txt
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)        1 2023-02-09 15:04:52.000000 bbrc-bx-0.5/bbrc_bx.egg-info/dependency_links.txt
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      216 2023-02-09 15:04:52.000000 bbrc-bx-0.5/bbrc_bx.egg-info/requires.txt
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)        3 2023-02-09 15:04:52.000000 bbrc-bx-0.5/bbrc_bx.egg-info/top_level.txt
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-02-09 15:04:52.148724 bbrc-bx-0.5/bin/
--rwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)     1375 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bin/bx
--rwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)     2466 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bin/dump
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-02-09 15:04:52.148724 bbrc-bx-0.5/bx/
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)       20 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/__init__.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1504 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/ants.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      931 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/archiving.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1856 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/ashs.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2140 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/bamos.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3957 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/basil.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     6820 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/braak.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     5996 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/cache.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2031 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/cat12.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1276 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/command.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3292 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/dartel.py
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-02-09 15:04:52.148724 bbrc-bx-0.5/bx/data/
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-02-09 15:04:52.148724 bbrc-bx-0.5/bx/data/aal2/
--rwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)  1805610 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/aal2/AAL2.nii
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-02-09 15:04:52.148724 bbrc-bx-0.5/bx/data/braak/
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    21375 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/braak/Braak_III_IV.nii.gz
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     8550 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/braak/Braak_I_II.nii.gz
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    43647 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/braak/Braak_V_VI.nii.gz
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-02-09 15:04:52.148724 bbrc-bx-0.5/bx/data/dickerson/
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-02-09 15:04:52.148724 bbrc-bx-0.5/bx/data/dickerson/ad/
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)  1311029 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/ad/lh.adsig.annot
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   380865 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/ad/lh.adsig.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    46377 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/ad/lh.ag.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    40669 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/ad/lh.ifs.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    38156 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/ad/lh.itg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    36485 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/ad/lh.mtl.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    25301 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/ad/lh.precun.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    31448 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/ad/lh.sfg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    57883 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/ad/lh.smg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    64177 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/ad/lh.spl.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    40731 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/ad/lh.tpole.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      340 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/ad/readme.txt
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)  1311029 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/ad/rh.adsig.annot
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   309446 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/ad/rh.adsig.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    57185 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/ad/rh.ag.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    36739 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/ad/rh.ifs.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    21554 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/ad/rh.itg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    17927 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/ad/rh.mtl.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    27041 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/ad/rh.precun.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    21679 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/ad/rh.sfg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    35083 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/ad/rh.smg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    47767 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/ad/rh.spl.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    44831 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/ad/rh.tpole.label
-drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-02-09 15:04:52.148724 bbrc-bx-0.5/bx/data/dickerson/aging/
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    47465 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/aging/lh.ag.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    61217 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/aging/lh.calcarine.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    45075 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/aging/lh.cfusi.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    61186 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/aging/lh.cinsula.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    17689 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/aging/lh.cmfg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    57934 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/aging/lh.cuneus.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    35857 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/aging/lh.ifg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    94600 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/aging/lh.loccip.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   103129 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/aging/lh.msfg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   266555 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/aging/lh.precent.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    37420 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/aging/lh.smg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    49122 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/aging/rh.ag.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    66055 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/aging/rh.calcarine.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    34255 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/aging/rh.cfusi.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    40799 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/aging/rh.cinsula.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    14089 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/aging/rh.cmfg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    83947 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/aging/rh.cuneus.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    51217 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/aging/rh.ifg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   159303 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/aging/rh.loccip.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   108346 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/aging/rh.msfg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    92440 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/aging/rh.precent.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    26292 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/dickerson/aging/rh.smg.label
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      240 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/data/logo
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2252 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/dcm.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2028 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/donsurf.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    12505 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/download.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1678 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/dtifit.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3094 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/dump.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     6393 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/freesurfer.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1082 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/id.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    69038 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/lists.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2761 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/nifti.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     8829 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/parse.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     8139 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/pet.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2969 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/qsmxt.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      700 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/scandates.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     8148 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/signature.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2552 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/spm12.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2826 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/validation.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1464 2023-02-09 15:02:03.000000 bbrc-bx-0.5/bx/xnat.py
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      216 2023-02-09 15:02:03.000000 bbrc-bx-0.5/requirements.txt
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)       38 2023-02-09 15:04:52.148724 bbrc-bx-0.5/setup.cfg
--rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1792 2023-02-09 15:02:03.000000 bbrc-bx-0.5/setup.py
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-11 17:09:34.118265 bbrc-bx-0.5.1/
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)       71 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/MANIFEST.in
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    20834 2023-07-11 17:09:34.118265 bbrc-bx-0.5.1/PKG-INFO
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    16563 2023-07-11 17:06:38.000000 bbrc-bx-0.5.1/README.md
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-11 17:09:34.108265 bbrc-bx-0.5.1/bbrc_bx.egg-info/
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    20834 2023-07-11 17:09:34.000000 bbrc-bx-0.5.1/bbrc_bx.egg-info/PKG-INFO
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2443 2023-07-11 17:09:34.000000 bbrc-bx-0.5.1/bbrc_bx.egg-info/SOURCES.txt
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)        1 2023-07-11 17:09:34.000000 bbrc-bx-0.5.1/bbrc_bx.egg-info/dependency_links.txt
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      216 2023-07-11 17:09:34.000000 bbrc-bx-0.5.1/bbrc_bx.egg-info/requires.txt
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)        3 2023-07-11 17:09:34.000000 bbrc-bx-0.5.1/bbrc_bx.egg-info/top_level.txt
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-11 17:09:34.108265 bbrc-bx-0.5.1/bin/
+-rwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)     1375 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bin/bx
+-rwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)     2466 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bin/dump
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-11 17:09:34.108265 bbrc-bx-0.5.1/bx/
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)       22 2023-07-11 17:06:38.000000 bbrc-bx-0.5.1/bx/__init__.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1504 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/ants.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      931 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/archiving.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1856 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/ashs.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2140 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/bamos.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3957 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/basil.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     6820 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/braak.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     5996 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/cache.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2031 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/cat12.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1276 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/command.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3477 2023-07-11 17:06:38.000000 bbrc-bx-0.5.1/bx/dartel.py
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-11 17:09:34.108265 bbrc-bx-0.5.1/bx/data/
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-11 17:09:34.108265 bbrc-bx-0.5.1/bx/data/aal2/
+-rwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)  1805610 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/aal2/AAL2.nii
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-11 17:09:34.108265 bbrc-bx-0.5.1/bx/data/braak/
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    21375 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/braak/Braak_III_IV.nii.gz
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     8550 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/braak/Braak_I_II.nii.gz
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    43647 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/braak/Braak_V_VI.nii.gz
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-11 17:09:34.108265 bbrc-bx-0.5.1/bx/data/dickerson/
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-11 17:09:34.118265 bbrc-bx-0.5.1/bx/data/dickerson/ad/
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)  1311029 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.adsig.annot
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   380865 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.adsig.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    46377 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.ag.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    40669 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.ifs.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    38156 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.itg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    36485 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.mtl.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    25301 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.precun.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    31448 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.sfg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    57883 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.smg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    64177 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.spl.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    40731 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.tpole.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      340 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/readme.txt
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)  1311029 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.adsig.annot
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   309446 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.adsig.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    57185 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.ag.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    36739 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.ifs.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    21554 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.itg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    17927 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.mtl.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    27041 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.precun.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    21679 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.sfg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    35083 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.smg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    47767 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.spl.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    44831 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.tpole.label
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-11 17:09:34.118265 bbrc-bx-0.5.1/bx/data/dickerson/aging/
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    47465 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.ag.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    61217 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.calcarine.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    45075 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.cfusi.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    61186 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.cinsula.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    17689 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.cmfg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    57934 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.cuneus.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    35857 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.ifg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    94600 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.loccip.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   103129 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.msfg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   266555 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.precent.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    37420 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.smg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    49122 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.ag.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    66055 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.calcarine.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    34255 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.cfusi.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    40799 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.cinsula.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    14089 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.cmfg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    83947 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.cuneus.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    51217 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.ifg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   159303 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.loccip.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   108346 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.msfg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    92440 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.precent.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    26292 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.smg.label
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      240 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/data/logo
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-11 17:09:34.118265 bbrc-bx-0.5.1/bx/data/masks/
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)   902981 2023-07-11 17:06:38.000000 bbrc-bx-0.5.1/bx/data/masks/fdg_aging_mask.nii
+drwxr-xr-x   0 jhuguet   (1000) jhuguet   (1000)        0 2023-07-11 17:09:34.118265 bbrc-bx-0.5.1/bx/data/mrtrix3/
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     6193 2023-07-11 17:06:38.000000 bbrc-bx-0.5.1/bx/data/mrtrix3/fs_default.txt
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2252 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/dcm.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2028 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/donsurf.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    13464 2023-07-11 17:06:38.000000 bbrc-bx-0.5.1/bx/download.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1678 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/dtifit.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3118 2023-07-11 17:06:38.000000 bbrc-bx-0.5.1/bx/dump.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     6393 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/freesurfer.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1082 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/id.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)    75188 2023-07-11 17:06:38.000000 bbrc-bx-0.5.1/bx/lists.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     3200 2023-07-11 17:06:38.000000 bbrc-bx-0.5.1/bx/mrtrix3.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2761 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/nifti.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     8829 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/parse.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     8455 2023-07-11 17:06:38.000000 bbrc-bx-0.5.1/bx/pet.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2882 2023-07-11 17:06:38.000000 bbrc-bx-0.5.1/bx/qsmxt.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      700 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/scandates.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     8148 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/signature.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2552 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/spm12.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     2826 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/validation.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1464 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/bx/xnat.py
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)      216 2023-02-09 15:02:03.000000 bbrc-bx-0.5.1/requirements.txt
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)       38 2023-07-11 17:09:34.118265 bbrc-bx-0.5.1/setup.cfg
+-rw-r--r--   0 jhuguet   (1000) jhuguet   (1000)     1792 2023-07-11 17:06:38.000000 bbrc-bx-0.5.1/setup.py
```

### Comparing `bbrc-bx-0.5/PKG-INFO` & `bbrc-bx-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: bbrc-bx
-Version: 0.5
+Version: 0.5.1
 Summary: BarcelonaBeta + XNAT = bx
 Home-page: https://gitlab.com/bbrc/xnat/bx
 Author: Greg Operto, Jordi Huguet
 Author-email: goperto@barcelonabeta.org
 License: UNKNOWN
-Download-URL: https://gitlab.com/bbrc/xnat/bx/-/archive/v0.5/bx-v0.5.tar.gz
+Download-URL: https://gitlab.com/bbrc/xnat/bx/-/archive/v0.5.1/bx-v0.5.1.tar.gz
 Description: # bx
         
         [![pipeline status](https://gitlab.com/bbrc/xnat/bx/badges/master/pipeline.svg)](https://gitlab.com/bbrc/xnat/bx/commits/master)
         [![coverage report](https://gitlab.com/bbrc/xnat/bx/badges/master/coverage.svg)](https://gitlab.com/bbrc/xnat/bx/commits/master)
         [![downloads](https://img.shields.io/pypi/dm/bbrc-bx.svg)](https://pypi.org/project/bbrc-bx/)
         [![python versions](https://img.shields.io/pypi/pyversions/bbrc-bx.svg)](https://pypi.org/project/bbrc-bx/)
         [![pypi version](https://img.shields.io/pypi/v/bbrc-bx.svg)](https://pypi.org/project/bbrc-bx/)
@@ -296,14 +296,31 @@
         
             Available subcommands:
              `show`:		display all existing lists (usage: bx lists show)
         
             Usage:
              bx lists <subcommand>
         
+        ### **`MRTRIX3`**:
+        
+        MRtrix3 - Diffusion MRI tractography and structural connectivity.
+        
+            Available subcommands:
+             connectome:	download the structural connectivity matrices (Desikan-Killiany atlas)
+             `files`:		download all MRTRIX3 outputs (streamlines, segmentations, everything...)
+             `report`:		download the validation report issued by `MRtrix3Validator`
+             `snapshot`:	download snapshots from the MRTRIX3 pipeline
+             `tests`:		create an Excel table with all automatic tests outcomes from bbrc-validator
+        
+            Usage:
+             bx mrtrix3 <subcommand> <resource_id>
+        
+            References:
+            - Tournier JD et al., NeuroImage 202 (2019).
+            
         ### **`NIFTI`**:
         
         Download NIfTI images from a given sequence (`SeriesDesc`).
         
             Available subcommands:
              `usable`:		download `usable` images (default)
              `all`:			download all images found
@@ -318,14 +335,15 @@
         18F-fluorodeoxyglucose PET imaging data
         
             Available subcommands:
              `landau`:		creates an Excel table with the Landau's metaROI signature
              `maps`:		download the normalized FDG maps
              `tests`:		collect all automatic tests outcomes from `PetSessionValidator`
              `mri`:			creates an Excel table with details from associated MRI sessions
+             `aging`:		creates an Excel table with the aging composite ROI
         
             Usage:
              bx fdg <subcommand> <resource_id>
         
             Reference:
             - Landau et al., Ann Neurol., 2012
         
@@ -444,10 +462,10 @@
         [![BarcelonaBeta](https://www.barcelonabeta.org/sites/default/files/logo-barcelona-beta_0.png)](https://www.barcelonabeta.org/)
         
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
```

### Comparing `bbrc-bx-0.5/README.md` & `bbrc-bx-0.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -287,14 +287,31 @@
 
     Available subcommands:
      `show`:		display all existing lists (usage: bx lists show)
 
     Usage:
      bx lists <subcommand>
 
+### **`MRTRIX3`**:
+
+MRtrix3 - Diffusion MRI tractography and structural connectivity.
+
+    Available subcommands:
+     connectome:	download the structural connectivity matrices (Desikan-Killiany atlas)
+     `files`:		download all MRTRIX3 outputs (streamlines, segmentations, everything...)
+     `report`:		download the validation report issued by `MRtrix3Validator`
+     `snapshot`:	download snapshots from the MRTRIX3 pipeline
+     `tests`:		create an Excel table with all automatic tests outcomes from bbrc-validator
+
+    Usage:
+     bx mrtrix3 <subcommand> <resource_id>
+
+    References:
+    - Tournier JD et al., NeuroImage 202 (2019).
+    
 ### **`NIFTI`**:
 
 Download NIfTI images from a given sequence (`SeriesDesc`).
 
     Available subcommands:
      `usable`:		download `usable` images (default)
      `all`:			download all images found
@@ -309,14 +326,15 @@
 18F-fluorodeoxyglucose PET imaging data
 
     Available subcommands:
      `landau`:		creates an Excel table with the Landau's metaROI signature
      `maps`:		download the normalized FDG maps
      `tests`:		collect all automatic tests outcomes from `PetSessionValidator`
      `mri`:			creates an Excel table with details from associated MRI sessions
+     `aging`:		creates an Excel table with the aging composite ROI
 
     Usage:
      bx fdg <subcommand> <resource_id>
 
     Reference:
     - Landau et al., Ann Neurol., 2012
```

### Comparing `bbrc-bx-0.5/bbrc_bx.egg-info/PKG-INFO` & `bbrc-bx-0.5.1/bbrc_bx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: bbrc-bx
-Version: 0.5
+Version: 0.5.1
 Summary: BarcelonaBeta + XNAT = bx
 Home-page: https://gitlab.com/bbrc/xnat/bx
 Author: Greg Operto, Jordi Huguet
 Author-email: goperto@barcelonabeta.org
 License: UNKNOWN
-Download-URL: https://gitlab.com/bbrc/xnat/bx/-/archive/v0.5/bx-v0.5.tar.gz
+Download-URL: https://gitlab.com/bbrc/xnat/bx/-/archive/v0.5.1/bx-v0.5.1.tar.gz
 Description: # bx
         
         [![pipeline status](https://gitlab.com/bbrc/xnat/bx/badges/master/pipeline.svg)](https://gitlab.com/bbrc/xnat/bx/commits/master)
         [![coverage report](https://gitlab.com/bbrc/xnat/bx/badges/master/coverage.svg)](https://gitlab.com/bbrc/xnat/bx/commits/master)
         [![downloads](https://img.shields.io/pypi/dm/bbrc-bx.svg)](https://pypi.org/project/bbrc-bx/)
         [![python versions](https://img.shields.io/pypi/pyversions/bbrc-bx.svg)](https://pypi.org/project/bbrc-bx/)
         [![pypi version](https://img.shields.io/pypi/v/bbrc-bx.svg)](https://pypi.org/project/bbrc-bx/)
@@ -296,14 +296,31 @@
         
             Available subcommands:
              `show`:		display all existing lists (usage: bx lists show)
         
             Usage:
              bx lists <subcommand>
         
+        ### **`MRTRIX3`**:
+        
+        MRtrix3 - Diffusion MRI tractography and structural connectivity.
+        
+            Available subcommands:
+             connectome:	download the structural connectivity matrices (Desikan-Killiany atlas)
+             `files`:		download all MRTRIX3 outputs (streamlines, segmentations, everything...)
+             `report`:		download the validation report issued by `MRtrix3Validator`
+             `snapshot`:	download snapshots from the MRTRIX3 pipeline
+             `tests`:		create an Excel table with all automatic tests outcomes from bbrc-validator
+        
+            Usage:
+             bx mrtrix3 <subcommand> <resource_id>
+        
+            References:
+            - Tournier JD et al., NeuroImage 202 (2019).
+            
         ### **`NIFTI`**:
         
         Download NIfTI images from a given sequence (`SeriesDesc`).
         
             Available subcommands:
              `usable`:		download `usable` images (default)
              `all`:			download all images found
@@ -318,14 +335,15 @@
         18F-fluorodeoxyglucose PET imaging data
         
             Available subcommands:
              `landau`:		creates an Excel table with the Landau's metaROI signature
              `maps`:		download the normalized FDG maps
              `tests`:		collect all automatic tests outcomes from `PetSessionValidator`
              `mri`:			creates an Excel table with details from associated MRI sessions
+             `aging`:		creates an Excel table with the aging composite ROI
         
             Usage:
              bx fdg <subcommand> <resource_id>
         
             Reference:
             - Landau et al., Ann Neurol., 2012
         
@@ -444,10 +462,10 @@
         [![BarcelonaBeta](https://www.barcelonabeta.org/sites/default/files/logo-barcelona-beta_0.png)](https://www.barcelonabeta.org/)
         
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
```

### Comparing `bbrc-bx-0.5/bbrc_bx.egg-info/SOURCES.txt` & `bbrc-bx-0.5.1/bbrc_bx.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 bx/donsurf.py
 bx/download.py
 bx/dtifit.py
 bx/dump.py
 bx/freesurfer.py
 bx/id.py
 bx/lists.py
+bx/mrtrix3.py
 bx/nifti.py
 bx/parse.py
 bx/pet.py
 bx/qsmxt.py
 bx/scandates.py
 bx/signature.py
 bx/spm12.py
@@ -82,8 +83,10 @@
 bx/data/dickerson/aging/rh.cinsula.label
 bx/data/dickerson/aging/rh.cmfg.label
 bx/data/dickerson/aging/rh.cuneus.label
 bx/data/dickerson/aging/rh.ifg.label
 bx/data/dickerson/aging/rh.loccip.label
 bx/data/dickerson/aging/rh.msfg.label
 bx/data/dickerson/aging/rh.precent.label
-bx/data/dickerson/aging/rh.smg.label
+bx/data/dickerson/aging/rh.smg.label
+bx/data/masks/fdg_aging_mask.nii
+bx/data/mrtrix3/fs_default.txt
```

### Comparing `bbrc-bx-0.5/bin/bx` & `bbrc-bx-0.5.1/bin/bx`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bin/dump` & `bbrc-bx-0.5.1/bin/dump`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/ants.py` & `bbrc-bx-0.5.1/bx/ants.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/archiving.py` & `bbrc-bx-0.5.1/bx/archiving.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/ashs.py` & `bbrc-bx-0.5.1/bx/ashs.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/bamos.py` & `bbrc-bx-0.5.1/bx/bamos.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/basil.py` & `bbrc-bx-0.5.1/bx/basil.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/braak.py` & `bbrc-bx-0.5.1/bx/braak.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/cache.py` & `bbrc-bx-0.5.1/bx/cache.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/cat12.py` & `bbrc-bx-0.5.1/bx/cat12.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/command.py` & `bbrc-bx-0.5.1/bx/command.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/dartel.py` & `bbrc-bx-0.5.1/bx/dartel.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,15 +61,19 @@
     filename = 'smw*'
 
     for e in tqdm(experiments):
         log.debug('Experiment {}:'.format(e['ID']))
         try:
             r = x.select.experiment(e['ID']).resource(resource_name)
             f = list(r.files(filename))[0]
-            f.get(op.join(destdir, f.label()))
+
+            fn = 'smwc1_{}_{}_{}.nii.gz'.format(e['subject_label'],
+                                                e['label'],
+                                                resource_name)
+            f.get(op.join(destdir, fn))
         except IndexError:
             log.error('Failed for {}. Skipping it.'.format(e['ID']))
 
 
 def download_template(x, template_label, resource_name, destdir):
     import os.path as op
```

### Comparing `bbrc-bx-0.5/bx/data/aal2/AAL2.nii` & `bbrc-bx-0.5.1/bx/data/aal2/AAL2.nii`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/braak/Braak_III_IV.nii.gz` & `bbrc-bx-0.5.1/bx/data/braak/Braak_III_IV.nii.gz`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/braak/Braak_I_II.nii.gz` & `bbrc-bx-0.5.1/bx/data/braak/Braak_I_II.nii.gz`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/braak/Braak_V_VI.nii.gz` & `bbrc-bx-0.5.1/bx/data/braak/Braak_V_VI.nii.gz`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/ad/lh.adsig.annot` & `bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.adsig.annot`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/ad/lh.adsig.label` & `bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.adsig.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/ad/lh.ag.label` & `bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.ag.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/ad/lh.ifs.label` & `bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.ifs.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/ad/lh.itg.label` & `bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.itg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/ad/lh.mtl.label` & `bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.mtl.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/ad/lh.precun.label` & `bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.precun.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/ad/lh.sfg.label` & `bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.sfg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/ad/lh.smg.label` & `bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.smg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/ad/lh.spl.label` & `bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.spl.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/ad/lh.tpole.label` & `bbrc-bx-0.5.1/bx/data/dickerson/ad/lh.tpole.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/ad/rh.adsig.annot` & `bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.adsig.annot`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/ad/rh.adsig.label` & `bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.adsig.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/ad/rh.ag.label` & `bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.ag.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/ad/rh.ifs.label` & `bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.ifs.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/ad/rh.itg.label` & `bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.itg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/ad/rh.mtl.label` & `bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.mtl.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/ad/rh.precun.label` & `bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.precun.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/ad/rh.sfg.label` & `bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.sfg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/ad/rh.smg.label` & `bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.smg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/ad/rh.spl.label` & `bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.spl.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/ad/rh.tpole.label` & `bbrc-bx-0.5.1/bx/data/dickerson/ad/rh.tpole.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/aging/lh.ag.label` & `bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.ag.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/aging/lh.calcarine.label` & `bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.calcarine.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/aging/lh.cfusi.label` & `bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.cfusi.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/aging/lh.cinsula.label` & `bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.cinsula.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/aging/lh.cmfg.label` & `bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.cmfg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/aging/lh.cuneus.label` & `bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.cuneus.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/aging/lh.ifg.label` & `bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.ifg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/aging/lh.loccip.label` & `bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.loccip.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/aging/lh.msfg.label` & `bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.msfg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/aging/lh.precent.label` & `bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.precent.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/aging/lh.smg.label` & `bbrc-bx-0.5.1/bx/data/dickerson/aging/lh.smg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/aging/rh.ag.label` & `bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.ag.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/aging/rh.calcarine.label` & `bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.calcarine.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/aging/rh.cfusi.label` & `bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.cfusi.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/aging/rh.cinsula.label` & `bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.cinsula.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/aging/rh.cmfg.label` & `bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.cmfg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/aging/rh.cuneus.label` & `bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.cuneus.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/aging/rh.ifg.label` & `bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.ifg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/aging/rh.loccip.label` & `bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.loccip.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/aging/rh.msfg.label` & `bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.msfg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/aging/rh.precent.label` & `bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.precent.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/data/dickerson/aging/rh.smg.label` & `bbrc-bx-0.5.1/bx/data/dickerson/aging/rh.smg.label`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/dcm.py` & `bbrc-bx-0.5.1/bx/dcm.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/donsurf.py` & `bbrc-bx-0.5.1/bx/donsurf.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/download.py` & `bbrc-bx-0.5.1/bx/download.py`

 * *Files 4% similar despite different names*

```diff
@@ -137,21 +137,21 @@
 
 def __fix_volumes__(volumes):
     """Remove incorrect volumes by FREESURFER6_HIRES as mentioned in the
     following page.
 
     Reference: https://surfer.nmr.mgh.harvard.edu/fswiki/BrainVolStatsFixed
     """
-    measurements = ['BrainSegVol', 'BrainSegVolNotVent', 'SupraTentorialVol',
-                    'lhCerebralWhiteMatterVol', 'rhCerebralWhiteMatterVol',
-                    'CerebralWhiteMatterVol', 'TotalGrayVol', 'SubCortGrayVol',
-                    'SupraTentorialVolNotVent', 'MaskVol', 'MaskVol-to-eTIV',
-                    'BrainSegVol-to-eTIV', 'lhCortexVol', 'rhCortexVol',
-                    'CortexVol']
-    volumes = volumes.drop(volumes.query('region.isin(@measurements)').index)
+    metrics = ['BrainSegVol', 'BrainSegVolNotVent', 'SupraTentorialVol',
+               'lhCerebralWhiteMatterVol', 'rhCerebralWhiteMatterVol',
+               'CerebralWhiteMatterVol', 'TotalGrayVol', 'SubCortGrayVol',
+               'SupraTentorialVolNotVent', 'MaskVol', 'MaskVol-to-eTIV',
+               'BrainSegVol-to-eTIV', 'lhCortexVol', 'rhCortexVol',
+               'CortexVol']
+    volumes = volumes.drop(volumes.query('region.isin(@metrics)').index)
     return volumes
 
 
 def __braak_fdg__(x, e_id, r):
     import bx
     import numpy as np
     import pandas as pd
@@ -244,19 +244,45 @@
     for label in n_labels:
         perf_values.append(np.mean(m[atlas == label]))
     df['value'] = perf_values
     os.remove(fp)
     return df
 
 
+def __aging_fdg__(x, e_id, r):
+    import bx
+    import numpy as np
+    import pandas as pd
+    import tempfile
+    import nibabel as nib
+    resource_name = 'FDG_QUANTIFICATION'
+    fh, fp = tempfile.mkstemp(suffix='.nii.gz')
+    os.close(fh)
+    r = x.select.experiment(e_id).resource(resource_name)
+    f = r.file('woptimized_static_pet_scaled_pons.nii.gz')
+    f.get(fp)
+
+    cols = ['optimized_pet', 'region', 'reference_region', 'measurement', 'value']
+    row = [True, 'aging_fdg_composite', 'pons', 'suvr', None]
+    df = pd.DataFrame(data=[row], index=[e_id], columns=cols)
+    aging_regions = op.join(op.dirname(bx.__file__), 'data',
+                            'masks', 'fdg_aging_mask.nii')
+    ag_im = nib.load(aging_regions)
+    ag_regs = np.array(ag_im.dataobj)
+    m = np.array(nib.load(fp).dataobj)
+    assert (m.shape == ag_regs.shape)
+    df['value'] = np.mean(m[ag_regs == 1])
+    os.remove(fp)
+    return df
+
+
 def measurements(x, experiments, subfunc, resource_name='FREESURFER6',
                  debug=False):
     """ Collect measurements for a set of experiments by calling some specific
     pyxnat resource-based function (e.g. aseg, aparc, centiloids, etc)"""
-    from tqdm import tqdm
     import pandas as pd
 
     table = []
     for e in tqdm(experiments):
         log.debug(e)
         try:
             s = e['subject_label']
@@ -299,14 +325,16 @@
                 volumes = __braak_fdg__(x, e_id, r)
             elif subfunc == 'basil_perfusion':
                 volumes = r.perfusion()
             elif subfunc in ['basil_stats', 'qsmxt_stats']:
                 volumes = r.stats()
             elif subfunc == 'basil_aal':
                 volumes = __perfusion__(x, e_id, r)
+            elif subfunc == 'aging':
+                volumes = __aging_fdg__(x, e_id, r)
             elif subfunc in ['brainstem', 'thalamus', 'hypothalamus']:
                 cmd = {'brainstem': 'brainstem_substructures_volumes',
                        'thalamus': 'thalamic_nuclei_volumes',
                        'hypothalamus': 'hypothalamic_subunits_volumes'}
                 volumes = eval('r.{}()'.format(cmd[subfunc]))
             volumes['subject'] = s
             volumes['ID'] = e['ID']
```

### Comparing `bbrc-bx-0.5/bx/dtifit.py` & `bbrc-bx-0.5.1/bx/dtifit.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/dump.py` & `bbrc-bx-0.5.1/bx/dump.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     signatures, Braak regions, etc). This results in a collection of
     spreadsheets to be served by dashboards."""
     import os
     import os.path as op
     import tempfile
     import bx
 
-    alfa_projects = ['VBM_ALFA_PLUS_20221215', 'ALFA_20220301']
+    alfa_projects = ['ALFA_PLUS_V1_20230518', 'ALFA_20220301', 'ALFA_PLUS_V2_20230518']
     fh, fp = tempfile.mkstemp(suffix='.sh')
     print(fp)
     os.close(fh)
     w = open(fp, 'w')
     cmd = 'mkdir %s' % op.join(wd, 'bx.new')
     w.write('export BX_DUMP=1\n')
     bx_fp = op.join(op.dirname(op.dirname(bx.__file__)), 'bin', 'bx')
```

### Comparing `bbrc-bx-0.5/bx/freesurfer.py` & `bbrc-bx-0.5.1/bx/freesurfer.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/id.py` & `bbrc-bx-0.5.1/bx/id.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/lists.py` & `bbrc-bx-0.5.1/bx/lists.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 from bx.command import Command
 
 
 VBM_ALFA_PLUS_AAIC2020_20201202 = ["BBRC02_E00960", "BBRC_E00046", "BBRC02_E06149", "BBRC02_E07242", "BBRC_E02026", "BBRC_E02142", "BBRC_E02507", "BBRC_E01935", "BBRC02_E06157", "BBRC_E00300", "BBRC_E02031", "BBRC_E01500", "BBRC02_E00078", "BBRC02_E00117", "BBRC02_E00962", "BBRC02_E02380", "BBRC_E01055", "BBRC02_E02410", "BBRC02_E01262", "BBRC02_E01373", "BBRC02_E00586", "BBRC_E00148", "BBRC02_E00509", "BBRC02_E00385", "BBRC02_E03378", "BBRC02_E01010", "BBRC02_E00966", "BBRC_E00108", "BBRC02_E00645", "BBRC02_E05047", "BBRC_E00087", "BBRC_E02019", "BBRC02_E01348", "BBRC_E01378", "BBRC02_E00671", "BBRC02_E06010", "BBRC02_E05089", "BBRC_E00052", "BBRC_E00089", "BBRC02_E03383", "BBRC02_E02349", "BBRC02_E00501", "BBRC02_E08296", "BBRC02_E05220", "BBRC02_E06766", "BBRC02_E00631", "BBRC02_E00619", "BBRC_E01025", "BBRC_E01946", "BBRC02_E06171", "BBRC02_E05107", "BBRC02_E03356", "BBRC02_E00292", "BBRC_E01529", "BBRC02_E00936", "BBRC02_E07284", "BBRC02_E05054", "BBRC_E02015", "BBRC02_E00461", "BBRC02_E00487", "BBRC02_E00378", "BBRC02_E00505", "BBRC02_E03621", "BBRC_E02205", "BBRC02_E00380", "BBRC02_E01301", "BBRC02_E01298", "BBRC_E02014", "BBRC02_E00482", "BBRC02_E00588", "BBRC02_E06197", "BBRC_E01367", "BBRC_E02602", "BBRC02_E05095", "BBRC02_E00110", "BBRC_E02017", "BBRC_E01977", "BBRC_E02009", "BBRC02_E07283", "BBRC02_E00559", "BBRC02_E00605", "BBRC02_E07230", "BBRC_E00100", "BBRC02_E00503", "BBRC02_E07189", "BBRC02_E00512", "BBRC02_E06054", "BBRC02_E00669", "BBRC02_E00299", "BBRC02_E01388", "BBRC02_E00498", "BBRC02_E07290", "BBRC_E02109", "BBRC_E02087", "BBRC02_E03949", "BBRC_E00283", "BBRC02_E00454", "BBRC_E01932", "BBRC02_E00481", "BBRC_E02600", "BBRC02_E00594", "BBRC02_E01239", "BBRC_E02598", "BBRC_E00339", "BBRC_E01379", "BBRC_E00098", "BBRC_E00062", "BBRC02_E00234", "BBRC_E02005", "BBRC02_E00504", "BBRC02_E00500", "BBRC_E02160", "BBRC02_E06048", "BBRC02_E01174", "BBRC02_E05529", "BBRC02_E02334", "BBRC_E02524", "BBRC02_E05262", "BBRC02_E06561", "BBRC02_E07248", "BBRC_E00281", "BBRC02_E05484", "BBRC_E02011", "BBRC02_E00387", "BBRC_E00967", "BBRC02_E01045", "BBRC02_E02523", "BBRC_E00117", "BBRC02_E07196", "BBRC02_E03666", "BBRC02_E00269", "BBRC02_E00497", "BBRC_E00113", "BBRC_E02541", "BBRC02_E00453", "BBRC02_E07646", "BBRC_E00107", "BBRC_E01944", "BBRC_E02161", "BBRC02_E03950", "BBRC02_E05114", "BBRC02_E01245", "BBRC02_E00925", "BBRC02_E00068", "BBRC_E00080", "BBRC02_E00318", "BBRC02_E07639", "BBRC02_E00381", "BBRC_E01545", "BBRC02_E01268", "BBRC02_E00379", "BBRC02_E05055", "BBRC02_E03411", "BBRC02_E06900", "BBRC_E00063", "BBRC02_E01001", "BBRC_E00067", "BBRC_E01910", "BBRC02_E00074", "BBRC_E02229", "BBRC02_E00659", "BBRC02_E07703", "BBRC02_E02522", "BBRC_E02023", "BBRC02_E05936", "BBRC02_E00300", "BBRC02_E00931", "BBRC02_E03615", "BBRC_E00325", "BBRC_E00078", "BBRC02_E00391", "BBRC_E00079", "BBRC_E02025", "BBRC02_E01195", "BBRC02_E01316", "BBRC_E02018", "BBRC02_E00511", "BBRC_E02233", "BBRC02_E01032", "BBRC02_E07233", "BBRC_E00292", "BBRC02_E02284", "BBRC_E02070", "BBRC_E02012", "BBRC02_E02473", "BBRC02_E02384", "BBRC02_E01292", "BBRC02_E05873", "BBRC02_E06154", "BBRC02_E00965", "BBRC_E02072", "BBRC02_E00288", "BBRC02_E06070", "BBRC02_E00942", "BBRC02_E03908", "BBRC02_E00604", "BBRC02_E05229", "BBRC02_E00348", "BBRC02_E01280", "BBRC02_E07235", "BBRC_E01538", "BBRC_E02136", "BBRC02_E02480", "BBRC02_E00064", "BBRC02_E03886", "BBRC02_E03655", "BBRC02_E03373", "BBRC02_E00499", "BBRC02_E00531", "BBRC_E00045", "BBRC02_E03402", "BBRC02_E00390", "BBRC_E02108", "BBRC02_E01042", "BBRC_E00112", "BBRC_E00216", "BBRC02_E07244", "BBRC02_E01238", "BBRC_E00115", "BBRC_E02478", "BBRC02_E06151", "BBRC02_E02274", "BBRC02_E05930", "BBRC02_E06586", "BBRC02_E02452", "BBRC_E02024", "BBRC02_E00496", "BBRC02_E03907", "BBRC02_E06088", "BBRC02_E07025", "BBRC02_E00490", "BBRC02_E06899", "BBRC02_E06004", "BBRC02_E00554", "BBRC02_E00388", "BBRC02_E02370", "BBRC_E00103", "BBRC02_E00293", "BBRC_E00116", "BBRC_E00077", "BBRC_E02562", "BBRC02_E06164", "BBRC02_E06199", "BBRC_E00462", "BBRC02_E07251", "BBRC02_E06124", "BBRC02_E00445", "BBRC02_E00928", "BBRC02_E03716", "BBRC_E02238", "BBRC02_E06584", "BBRC02_E01249", "BBRC02_E02322", "BBRC02_E02387", "BBRC02_E02347", "BBRC02_E00418", "BBRC02_E00383", "BBRC02_E00438", "BBRC02_E03656", "BBRC02_E00382", "BBRC02_E06761", "BBRC_E00106", "BBRC_E00102", "BBRC02_E06152", "BBRC02_E00491", "BBRC02_E00295", "BBRC_E01031", "BBRC_E00095", "BBRC02_E00298", "BBRC02_E00066", "BBRC02_E06118", "BBRC02_E00502", "BBRC_E02575", "BBRC02_E01043", "BBRC02_E00638", "BBRC02_E00510", "BBRC02_E00987", "BBRC02_E00095", "BBRC02_E01357", "BBRC_E02016", "BBRC_E00096", "BBRC02_E00680", "BBRC02_E05967", "BBRC02_E00949", "BBRC_E00212", "BBRC02_E00118", "BBRC02_E06456", "BBRC02_E03885", "BBRC_E02480", "BBRC02_E01302", "BBRC02_E03413", "BBRC02_E07197", "BBRC02_E06161", "BBRC02_E03912", "BBRC02_E00964", "BBRC02_E07221", "BBRC02_E00917", "BBRC02_E00340", "BBRC02_E02467", "BBRC02_E00017", "BBRC02_E02382", "BBRC02_E05261", "BBRC02_E02345", "BBRC_E02333", "BBRC_E00126", "BBRC_E00070", "BBRC02_E03581", "BBRC02_E06100", "BBRC02_E00392", "BBRC02_E00488", "BBRC_E02065", "BBRC02_E06448", "BBRC_E00053", "BBRC02_E00484", "BBRC02_E06117", "BBRC_E00071", "BBRC02_E03586", "BBRC02_E08052", "BBRC02_E05938", "BBRC_E02241", "BBRC02_E03919", "BBRC_E02105", "BBRC02_E00073", "BBRC02_E00489", "BBRC_E02008", "BBRC_E01044", "BBRC_E01039", "BBRC_E00055", "BBRC_E01366", "BBRC02_E00395", "BBRC02_E03823", "BBRC02_E05528", "BBRC_E00338", "BBRC02_E02342", "BBRC02_E01391", "BBRC02_E01269", "BBRC02_E01038", "BBRC_E02525", "BBRC_E02526", "BBRC02_E00626", "BBRC_E01108", "BBRC_E02603", "BBRC02_E05105", "BBRC02_E06687", "BBRC02_E01331", "BBRC02_E02317", "BBRC_E00068", "BBRC_E02007", "BBRC02_E07285", "BBRC02_E00397", "BBRC02_E00394", "BBRC02_E01434", "BBRC_E02225", "BBRC02_E03654", "BBRC02_E03610", "BBRC_E02067", "BBRC02_E01365", "BBRC02_E01257", "BBRC_E01941", "BBRC02_E00508", "BBRC02_E01217", "BBRC02_E06198", "BBRC02_E06129", "BBRC02_E05872", "BBRC_E02021", "BBRC_E00110", "BBRC02_E00232", "BBRC02_E06125", "BBRC02_E00479", "BBRC_E02479", "BBRC_E00114", "BBRC_E00099", "BBRC02_E05256", "BBRC02_E00569", "BBRC_E00101", "BBRC02_E00294", "BBRC02_E05113", "BBRC02_E00485", "BBRC02_E08038", "BBRC_E02631", "BBRC02_E03569", "BBRC02_E00483", "BBRC02_E00989", "BBRC_E00109", "BBRC02_E01030", "BBRC_E00075", "BBRC02_E05112", "BBRC_E01377", "BBRC02_E05078", "BBRC02_E07186", "BBRC02_E00384", "BBRC02_E00940", "BBRC02_E01323", "BBRC02_E00386", "BBRC02_E05070", "BBRC02_E00572", "BBRC02_E01050", "BBRC_E00111", "BBRC_E02020", "BBRC_E01778", "BBRC02_E00016", "BBRC_E00093", "BBRC02_E02282", "BBRC_E02511", "BBRC02_E00643", "BBRC_E02004", "BBRC_E00074", "BBRC02_E00296", "BBRC02_E01342", "BBRC02_E05202", "BBRC02_E00282", "BBRC_E01043", "BBRC_E01046", "BBRC02_E00524", "BBRC02_E00393", "BBRC02_E01175", "BBRC_E02528", "BBRC_E00073", "BBRC02_E00988", "BBRC_E02022", "BBRC02_E05125", "BBRC02_E00389", "BBRC02_E07599", "BBRC_E00097", "BBRC02_E00297", "BBRC_E00155", "BBRC_E01351", "BBRC_E00054"]
 
 VBM_ALFA_PLUS_20221215 = ["BBRC02_E00960", "BBRC_E00046", "BBRC02_E06149", "BBRC02_E07242", "BBRC_E02026", "BBRC_E02142", "BBRC_E02507", "BBRC_E01935", "BBRC02_E06157", "BBRC_E00300", "BBRC_E02031", "BBRC_E01500", "BBRC02_E00078", "BBRC02_E00117", "BBRC02_E00962", "BBRC02_E02380", "BBRC_E01055", "BBRC02_E02410", "BBRC02_E01262", "BBRC02_E01373", "BBRC02_E00586", "BBRC02_E03929", "BBRC02_E00509", "BBRC02_E00385", "BBRC02_E03378", "BBRC02_E06131", "BBRC02_E00966", "BBRC_E00108", "BBRC02_E00645", "BBRC02_E05047", "BBRC_E00087", "BBRC_E02019", "BBRC02_E01348", "BBRC_E01378", "BBRC02_E00671", "BBRC02_E06010", "BBRC02_E05089", "BBRC_E00052", "BBRC_E00089", "BBRC02_E03383", "BBRC02_E02349", "BBRC02_E00501", "BBRC02_E08296", "BBRC02_E05220", "BBRC02_E06766", "BBRC02_E00631", "BBRC02_E00619", "BBRC_E01025", "BBRC_E01946", "BBRC02_E06171", "BBRC02_E05107", "BBRC02_E03356", "BBRC02_E00292", "BBRC02_E07310", "BBRC02_E00936", "BBRC02_E07284", "BBRC02_E05054", "BBRC_E02015", "BBRC02_E00461", "BBRC02_E00487", "BBRC02_E00378", "BBRC02_E00505", "BBRC02_E03621", "BBRC02_E03705", "BBRC02_E00380", "BBRC02_E01301", "BBRC02_E01298", "BBRC_E02014", "BBRC02_E00482", "BBRC02_E00588", "BBRC02_E06197", "BBRC_E01367", "BBRC_E02602", "BBRC02_E05095", "BBRC02_E00110", "BBRC_E02017", "BBRC02_E06200", "BBRC_E02009", "BBRC02_E07283", "BBRC02_E00559", "BBRC02_E00605", "BBRC02_E07230", "BBRC_E00100", "BBRC02_E00503", "BBRC02_E07189", "BBRC02_E00512", "BBRC02_E06054", "BBRC02_E00669", "BBRC02_E00299", "BBRC02_E01388", "BBRC02_E00498", "BBRC02_E07290", "BBRC_E02109", "BBRC_E02087", "BBRC02_E03949", "BBRC_E00283", "BBRC02_E00454", "BBRC_E01932", "BBRC02_E00481", "BBRC_E02600", "BBRC02_E00594", "BBRC02_E01239", "BBRC_E02598", "BBRC_E00339", "BBRC_E01379", "BBRC_E00098", "BBRC_E00062", "BBRC02_E00234", "BBRC_E02005", "BBRC02_E00504", "BBRC02_E00500", "BBRC_E02160", "BBRC02_E06048", "BBRC02_E01174", "BBRC02_E05529", "BBRC02_E02334", "BBRC_E02524", "BBRC02_E05262", "BBRC02_E06561", "BBRC02_E07248", "BBRC_E00281", "BBRC02_E05484", "BBRC_E02011", "BBRC02_E00387", "BBRC_E00967", "BBRC02_E01045", "BBRC02_E02523", "BBRC_E00117", "BBRC02_E07196", "BBRC02_E03666", "BBRC02_E00269", "BBRC02_E00497", "BBRC_E00113", "BBRC02_E03896", "BBRC02_E00453", "BBRC02_E07646", "BBRC_E00107", "BBRC_E01944", "BBRC_E02161", "BBRC02_E03950", "BBRC02_E05114", "BBRC02_E01245", "BBRC02_E00925", "BBRC02_E00068", "BBRC_E00080", "BBRC02_E00318", "BBRC02_E07639", "BBRC02_E00381", "BBRC_E01545", "BBRC02_E01268", "BBRC02_E00379", "BBRC02_E05055", "BBRC02_E03411", "BBRC02_E06900", "BBRC_E00063", "BBRC02_E01001", "BBRC_E00067", "BBRC02_E03385", "BBRC02_E00074", "BBRC_E02229", "BBRC02_E00659", "BBRC02_E07703", "BBRC02_E02522", "BBRC_E02023", "BBRC02_E05936", "BBRC02_E00300", "BBRC02_E00931", "BBRC02_E03615", "BBRC_E00325", "BBRC_E00078", "BBRC02_E00391", "BBRC_E00079", "BBRC02_E03644", "BBRC02_E01195", "BBRC02_E01316", "BBRC_E02018", "BBRC02_E00511", "BBRC_E02233", "BBRC02_E01032", "BBRC02_E07233", "BBRC_E00292", "BBRC02_E02284", "BBRC_E02070", "BBRC_E02012", "BBRC02_E02473", "BBRC02_E02384", "BBRC02_E01292", "BBRC02_E05873", "BBRC02_E06154", "BBRC02_E00965", "BBRC_E02072", "BBRC02_E00288", "BBRC02_E06070", "BBRC02_E00942", "BBRC02_E03908", "BBRC02_E00604", "BBRC02_E05229", "BBRC02_E00348", "BBRC02_E01280", "BBRC02_E07235", "BBRC_E01538", "BBRC_E02136", "BBRC02_E02480", "BBRC02_E00064", "BBRC02_E03886", "BBRC02_E03655", "BBRC02_E03373", "BBRC02_E00499", "BBRC02_E00531", "BBRC_E00045", "BBRC02_E03402", "BBRC02_E00390", "BBRC_E02108", "BBRC02_E01042", "BBRC_E00112", "BBRC_E00216", "BBRC02_E07244", "BBRC02_E01238", "BBRC_E00115", "BBRC_E02478", "BBRC02_E06151", "BBRC02_E02274", "BBRC02_E05930", "BBRC02_E06586", "BBRC02_E02452", "BBRC_E02024", "BBRC02_E00496", "BBRC02_E03907", "BBRC02_E06088", "BBRC02_E07025", "BBRC02_E00490", "BBRC02_E06899", "BBRC02_E06004", "BBRC02_E00554", "BBRC02_E00388", "BBRC02_E02370", "BBRC_E00103", "BBRC02_E00293", "BBRC_E00116", "BBRC_E00077", "BBRC_E02562", "BBRC02_E06164", "BBRC02_E06199", "BBRC_E00462", "BBRC02_E07251", "BBRC02_E06124", "BBRC02_E00445", "BBRC02_E00928", "BBRC02_E03716", "BBRC_E02238", "BBRC02_E06584", "BBRC02_E01249", "BBRC02_E02322", "BBRC02_E02387", "BBRC02_E02347", "BBRC02_E05046", "BBRC02_E00383", "BBRC02_E00438", "BBRC02_E03656", "BBRC02_E00382", "BBRC02_E06761", "BBRC_E00106", "BBRC_E00102", "BBRC02_E06152", "BBRC02_E00491", "BBRC02_E00295", "BBRC_E01031", "BBRC_E00095", "BBRC02_E00298", "BBRC02_E00066", "BBRC02_E06118", "BBRC02_E00502", "BBRC02_E03921", "BBRC02_E01043", "BBRC02_E00638", "BBRC02_E00510", "BBRC02_E00987", "BBRC02_E00095", "BBRC02_E01357", "BBRC_E02016", "BBRC_E00096", "BBRC02_E00680", "BBRC02_E05967", "BBRC02_E00949", "BBRC_E00212", "BBRC02_E00118", "BBRC02_E06456", "BBRC02_E03885", "BBRC_E02480", "BBRC02_E01302", "BBRC02_E03413", "BBRC02_E07197", "BBRC02_E06161", "BBRC02_E03912", "BBRC02_E00964", "BBRC02_E07221", "BBRC02_E00917", "BBRC02_E00340", "BBRC02_E02467", "BBRC02_E00017", "BBRC02_E02382", "BBRC02_E05261", "BBRC02_E02345", "BBRC02_E03809", "BBRC02_E05240", "BBRC_E00070", "BBRC02_E03581", "BBRC02_E06100", "BBRC02_E00392", "BBRC02_E00488", "BBRC_E02065", "BBRC02_E06448", "BBRC_E00053", "BBRC02_E00484", "BBRC02_E06117", "BBRC_E00071", "BBRC02_E03586", "BBRC02_E08052", "BBRC02_E05938", "BBRC_E02241", "BBRC02_E03919", "BBRC_E02105", "BBRC02_E00073", "BBRC02_E00489", "BBRC_E02008", "BBRC_E01044", "BBRC_E01039", "BBRC_E00055", "BBRC_E01366", "BBRC02_E00395", "BBRC02_E03823", "BBRC02_E05528", "BBRC_E00338", "BBRC02_E02342", "BBRC02_E01391", "BBRC02_E01269", "BBRC02_E01038", "BBRC_E02525", "BBRC_E02526", "BBRC02_E00626", "BBRC_E01108", "BBRC_E02603", "BBRC02_E05105", "BBRC02_E06687", "BBRC02_E01331", "BBRC02_E02317", "BBRC_E00068", "BBRC_E02007", "BBRC02_E07285", "BBRC02_E00397", "BBRC02_E00394", "BBRC02_E01434", "BBRC_E02225", "BBRC02_E03654", "BBRC02_E03610", "BBRC_E02067", "BBRC02_E01365", "BBRC02_E01257", "BBRC02_E03567", "BBRC02_E03946", "BBRC02_E06126", "BBRC02_E06198", "BBRC02_E06129", "BBRC02_E05872", "BBRC_E02021", "BBRC_E00110", "BBRC02_E00232", "BBRC02_E06125", "BBRC02_E00479", "BBRC_E02479", "BBRC_E00114", "BBRC_E00099", "BBRC02_E05256", "BBRC02_E00569", "BBRC_E00101", "BBRC02_E00294", "BBRC02_E05113", "BBRC02_E00485", "BBRC02_E08038", "BBRC_E02631", "BBRC02_E03569", "BBRC02_E00483", "BBRC02_E00989", "BBRC_E00109", "BBRC02_E01030", "BBRC_E00075", "BBRC02_E05112", "BBRC_E01377", "BBRC02_E05078", "BBRC02_E07186", "BBRC02_E00384", "BBRC02_E00940", "BBRC02_E01323", "BBRC02_E00386", "BBRC02_E05070", "BBRC02_E00572", "BBRC02_E01050", "BBRC_E00111", "BBRC_E02020", "BBRC_E01778", "BBRC02_E00016", "BBRC_E00093", "BBRC02_E02282", "BBRC_E02511", "BBRC02_E00643", "BBRC_E02004", "BBRC_E00074", "BBRC02_E00296", "BBRC02_E01342", "BBRC02_E05202", "BBRC02_E00282", "BBRC_E01043", "BBRC_E01046", "BBRC02_E00524", "BBRC02_E00393", "BBRC02_E01175", "BBRC_E02528", "BBRC_E00073", "BBRC02_E00988", "BBRC_E02022", "BBRC02_E05125", "BBRC02_E00389", "BBRC02_E07599", "BBRC_E00097", "BBRC02_E00297", "BBRC02_E01267", "BBRC_E01351", "BBRC_E00054"]
 
+# case reincluded (28/04/2023), considered suitable for neuroimaging analyses
+ALFA_PLUS_V1_20230518 = VBM_ALFA_PLUS_20221215 + ['BBRC_E00050']
+
 DEV = ['BBRCDEV_E02443', 'BBRCDEV_E01613']
 
 ALFA_20201001 = ["BBRC02_E00002", "BBRC02_E00003", "BBRC02_E00006", "BBRC02_E00007", "BBRC02_E00008", "BBRC02_E00011", "BBRC02_E00014", "BBRC02_E00016", "BBRC02_E00017", "BBRC02_E00037", "BBRC02_E00038", "BBRC02_E00039", "BBRC02_E00042", "BBRC02_E00043", "BBRC02_E00044", "BBRC02_E00045", "BBRC02_E00046", "BBRC02_E00047", "BBRC02_E00048", "BBRC02_E00049", "BBRC02_E00050", "BBRC02_E00058", "BBRC02_E00059", "BBRC02_E00064", "BBRC02_E00066", "BBRC02_E00068", "BBRC02_E00072", "BBRC02_E00073", "BBRC02_E00074", "BBRC02_E00077", "BBRC02_E00078", "BBRC02_E00079", "BBRC02_E00086", "BBRC02_E00090", "BBRC02_E00092", "BBRC02_E00093", "BBRC02_E00095", "BBRC02_E00101", "BBRC02_E00105", "BBRC02_E00110", "BBRC02_E00117", "BBRC02_E00118", "BBRC02_E00195", "BBRC02_E00198", "BBRC02_E00201", "BBRC02_E00206", "BBRC02_E00210", "BBRC02_E00218", "BBRC02_E00220", "BBRC02_E00222", "BBRC02_E00224", "BBRC02_E00232", "BBRC02_E00233", "BBRC02_E00234", "BBRC02_E00267", "BBRC02_E00268", "BBRC02_E00269", "BBRC02_E00274", "BBRC02_E00275", "BBRC02_E00276", "BBRC02_E00277", "BBRC02_E00278", "BBRC02_E00279", "BBRC02_E00282", "BBRC02_E00283", "BBRC02_E00284", "BBRC02_E00285", "BBRC02_E00288", "BBRC02_E00291", "BBRC02_E00292", "BBRC02_E00293", "BBRC02_E00294", "BBRC02_E00295", "BBRC02_E00296", "BBRC02_E00297", "BBRC02_E00298", "BBRC02_E00299", "BBRC02_E00300", "BBRC02_E00302", "BBRC02_E00317", "BBRC02_E00318", "BBRC02_E00327", "BBRC02_E00340", "BBRC02_E00348", "BBRC02_E00378", "BBRC02_E00379", "BBRC02_E00380", "BBRC02_E00381", "BBRC02_E00382", "BBRC02_E00383", "BBRC02_E00384", "BBRC02_E00385", "BBRC02_E00386", "BBRC02_E00387", "BBRC02_E00388", "BBRC02_E00389", "BBRC02_E00390", "BBRC02_E00391", "BBRC02_E00392", "BBRC02_E00393", "BBRC02_E00394", "BBRC02_E00395", "BBRC02_E00397", "BBRC02_E00405", "BBRC02_E00407", "BBRC02_E00415", "BBRC02_E00428", "BBRC02_E00432", "BBRC02_E00437", "BBRC02_E00438", "BBRC02_E00445", "BBRC02_E00453", "BBRC02_E00454", "BBRC02_E00455", "BBRC02_E00456", "BBRC02_E00457", "BBRC02_E00458", "BBRC02_E00459", "BBRC02_E00461", "BBRC02_E00466", "BBRC02_E00467", "BBRC02_E00468", "BBRC02_E00469", "BBRC02_E00479", "BBRC02_E00481", "BBRC02_E00482", "BBRC02_E00483", "BBRC02_E00484", "BBRC02_E00485", "BBRC02_E00486", "BBRC02_E00487", "BBRC02_E00488", "BBRC02_E00489", "BBRC02_E00490", "BBRC02_E00491", "BBRC02_E00496", "BBRC02_E00497", "BBRC02_E00498", "BBRC02_E00499", "BBRC02_E00500", "BBRC02_E00501", "BBRC02_E00502", "BBRC02_E00503", "BBRC02_E00504", "BBRC02_E00505", "BBRC02_E00507", "BBRC02_E00509", "BBRC02_E00510", "BBRC02_E00511", "BBRC02_E00512", "BBRC02_E00517", "BBRC02_E00524", "BBRC02_E00529", "BBRC02_E00530", "BBRC02_E00531", "BBRC02_E00533", "BBRC02_E00554", "BBRC02_E00559", "BBRC02_E00563", "BBRC02_E00569", "BBRC02_E00572", "BBRC02_E00573", "BBRC02_E00574", "BBRC02_E00575", "BBRC02_E00580", "BBRC02_E00581", "BBRC02_E00582", "BBRC02_E00583", "BBRC02_E00584", "BBRC02_E00585", "BBRC02_E00586", "BBRC02_E00588", "BBRC02_E00594", "BBRC02_E00600", "BBRC02_E00601", "BBRC02_E00604", "BBRC02_E00605", "BBRC02_E00608", "BBRC02_E00609", "BBRC02_E00610", "BBRC02_E00619", "BBRC02_E00624", "BBRC02_E00625", "BBRC02_E00626", "BBRC02_E00628", "BBRC02_E00631", "BBRC02_E00636", "BBRC02_E00637", "BBRC02_E00638", "BBRC02_E00643", "BBRC02_E00644", "BBRC02_E00645", "BBRC02_E00651", "BBRC02_E00654", "BBRC02_E00656", "BBRC02_E00657", "BBRC02_E00659", "BBRC02_E00660", "BBRC02_E00661", "BBRC02_E00662", "BBRC02_E00663", "BBRC02_E00664", "BBRC02_E00665", "BBRC02_E00667", "BBRC02_E00669", "BBRC02_E00670", "BBRC02_E00671", "BBRC02_E00680", "BBRC02_E00681", "BBRC02_E00693", "BBRC02_E00699", "BBRC02_E00700", "BBRC02_E00701", "BBRC02_E00702", "BBRC02_E00703", "BBRC02_E00704", "BBRC02_E00709", "BBRC02_E00710", "BBRC02_E00711", "BBRC02_E00712", "BBRC02_E00713", "BBRC02_E00714", "BBRC02_E00715", "BBRC02_E00716", "BBRC02_E00717", "BBRC02_E00718", "BBRC02_E00719", "BBRC02_E00720", "BBRC02_E00721", "BBRC02_E00722", "BBRC02_E00723", "BBRC02_E00724", "BBRC02_E00725", "BBRC02_E00726", "BBRC02_E00727", "BBRC02_E00728", "BBRC02_E00729", "BBRC02_E00730", "BBRC02_E00731", "BBRC02_E00732", "BBRC02_E00734", "BBRC02_E00735", "BBRC02_E00736", "BBRC02_E00737", "BBRC02_E00738", "BBRC02_E00745", "BBRC02_E00746", "BBRC02_E00747", "BBRC02_E00748", "BBRC02_E00749", "BBRC02_E00750", "BBRC02_E00751", "BBRC02_E00752", "BBRC02_E00753", "BBRC02_E00754", "BBRC02_E00755", "BBRC02_E00756", "BBRC02_E00757", "BBRC02_E00758", "BBRC02_E00759", "BBRC02_E00760", "BBRC02_E00761", "BBRC02_E00762", "BBRC02_E00763", "BBRC02_E00764", "BBRC02_E00765", "BBRC02_E00766", "BBRC02_E00767", "BBRC02_E00768", "BBRC02_E00769", "BBRC02_E00770", "BBRC02_E00771", "BBRC02_E00772", "BBRC02_E00773", "BBRC02_E00774", "BBRC02_E00775", "BBRC02_E00777", "BBRC02_E00779", "BBRC02_E00780", "BBRC02_E00781", "BBRC02_E00782", "BBRC02_E00783", "BBRC02_E00784", "BBRC02_E00785", "BBRC02_E00786", "BBRC02_E00787", "BBRC02_E00788", "BBRC02_E00789", "BBRC02_E00790", "BBRC02_E00791", "BBRC02_E00792", "BBRC02_E00793", "BBRC02_E00794", "BBRC02_E00797", "BBRC02_E00798", "BBRC02_E00799", "BBRC02_E00800", "BBRC02_E00801", "BBRC02_E00802", "BBRC02_E00803", "BBRC02_E00804", "BBRC02_E00805", "BBRC02_E00806", "BBRC02_E00807", "BBRC02_E00808", "BBRC02_E00809", "BBRC02_E00810", "BBRC02_E00811", "BBRC02_E00812", "BBRC02_E00813", "BBRC02_E00814", "BBRC02_E00815", "BBRC02_E00816", "BBRC02_E00817", "BBRC02_E00818", "BBRC02_E00819", "BBRC02_E00820", "BBRC02_E00821", "BBRC02_E00822", "BBRC02_E00823", "BBRC02_E00824", "BBRC02_E00825", "BBRC02_E00826", "BBRC02_E00827", "BBRC02_E00828", "BBRC02_E00829", "BBRC02_E00830", "BBRC02_E00831", "BBRC02_E00832", "BBRC02_E00833", "BBRC02_E00834", "BBRC02_E00835", "BBRC02_E00836", "BBRC02_E00837", "BBRC02_E00838", "BBRC02_E00839", "BBRC02_E00840", "BBRC02_E00841", "BBRC02_E00842", "BBRC02_E00843", "BBRC02_E00844", "BBRC02_E00845", "BBRC02_E00846", "BBRC02_E00847", "BBRC02_E00848", "BBRC02_E00849", "BBRC02_E00850", "BBRC02_E00851", "BBRC02_E00852", "BBRC02_E00853", "BBRC02_E00854", "BBRC02_E00855", "BBRC02_E00856", "BBRC02_E00857", "BBRC02_E00858", "BBRC02_E00859", "BBRC02_E00860", "BBRC02_E00861", "BBRC02_E00862", "BBRC02_E00863", "BBRC02_E00864", "BBRC02_E00865", "BBRC02_E00866", "BBRC02_E00867", "BBRC02_E00868", "BBRC02_E00869", "BBRC02_E00870", "BBRC02_E00871", "BBRC02_E00872", "BBRC02_E00873", "BBRC02_E00874", "BBRC02_E00875", "BBRC02_E00876", "BBRC02_E00877", "BBRC02_E00878", "BBRC02_E00879", "BBRC02_E00880", "BBRC02_E00881", "BBRC02_E00882", "BBRC02_E00883", "BBRC02_E00884", "BBRC02_E00885", "BBRC02_E00886", "BBRC02_E00887", "BBRC02_E00888", "BBRC02_E00889", "BBRC02_E00890", "BBRC02_E00891", "BBRC02_E00892", "BBRC02_E00893", "BBRC02_E00894", "BBRC02_E00895", "BBRC02_E00896", "BBRC02_E00897", "BBRC02_E00898", "BBRC02_E00899", "BBRC02_E00900", "BBRC02_E00901", "BBRC02_E00902", "BBRC02_E00903", "BBRC02_E00904", "BBRC02_E00905", "BBRC02_E00906", "BBRC02_E00907", "BBRC02_E00908", "BBRC02_E00912", "BBRC02_E00917", "BBRC02_E00925", "BBRC02_E00926", "BBRC02_E00928", "BBRC02_E00929", "BBRC02_E00931", "BBRC02_E00934", "BBRC02_E00936", "BBRC02_E00937", "BBRC02_E00940", "BBRC02_E00942", "BBRC02_E00944", "BBRC02_E00949", "BBRC02_E00950", "BBRC02_E00951", "BBRC02_E00955", "BBRC02_E00959", "BBRC02_E00960", "BBRC02_E00961", "BBRC02_E00962", "BBRC02_E00964", "BBRC02_E00965", "BBRC02_E00966", "BBRC02_E00975", "BBRC02_E00987", "BBRC02_E00988", "BBRC02_E00989", "BBRC02_E00990", "BBRC02_E00991", "BBRC02_E00993", "BBRC02_E00994", "BBRC02_E00996", "BBRC02_E01000", "BBRC02_E01001", "BBRC02_E01006", "BBRC02_E01007", "BBRC02_E01008", "BBRC02_E01012", "BBRC02_E01013", "BBRC02_E01014", "BBRC02_E01015", "BBRC02_E01016", "BBRC02_E01023", "BBRC02_E01027", "BBRC02_E01030", "BBRC02_E01031", "BBRC02_E01032", "BBRC02_E01037", "BBRC02_E01038", "BBRC02_E01039", "BBRC02_E01042", "BBRC02_E01043", "BBRC02_E01045", "BBRC02_E01046", "BBRC02_E01048", "BBRC02_E01050", "BBRC02_E01053", "BBRC02_E01058", "BBRC02_E01173", "BBRC02_E01174", "BBRC02_E01175", "BBRC02_E01176", "BBRC02_E01182", "BBRC02_E01195", "BBRC02_E01237", "BBRC02_E01238", "BBRC02_E01239", "BBRC02_E01245", "BBRC02_E01247", "BBRC02_E01249", "BBRC02_E01250", "BBRC02_E01253", "BBRC02_E01257", "BBRC02_E01261", "BBRC02_E01262", "BBRC02_E01263", "BBRC02_E01268", "BBRC02_E01269", "BBRC02_E01271", "BBRC02_E01280", "BBRC02_E01281", "BBRC02_E01282", "BBRC02_E01283", "BBRC02_E01292", "BBRC02_E01293", "BBRC02_E01297", "BBRC02_E01298", "BBRC02_E01301", "BBRC02_E01302", "BBRC02_E01308", "BBRC02_E01316", "BBRC02_E01317", "BBRC02_E01322", "BBRC02_E01323", "BBRC02_E01324", "BBRC02_E01325", "BBRC02_E01331", "BBRC02_E01339", "BBRC02_E01342", "BBRC02_E01343", "BBRC02_E01348", "BBRC02_E01356", "BBRC02_E01357", "BBRC02_E01358", "BBRC02_E01359", "BBRC02_E01365", "BBRC02_E01366", "BBRC02_E01373", "BBRC02_E01374", "BBRC02_E01376", "BBRC02_E01378", "BBRC02_E01381", "BBRC02_E01384", "BBRC02_E01388", "BBRC02_E01391", "BBRC02_E01394", "BBRC02_E01401", "BBRC02_E01422", "BBRC02_E01423", "BBRC02_E01427", "BBRC02_E01428", "BBRC02_E01435", "BBRC02_E02263", "BBRC02_E02264", "BBRC02_E02265", "BBRC02_E02266", "BBRC02_E02267", "BBRC02_E02268", "BBRC02_E02273", "BBRC02_E02274", "BBRC02_E02278", "BBRC02_E02279", "BBRC02_E02282", "BBRC02_E02284", "BBRC02_E02285", "BBRC02_E02287", "BBRC02_E02288", "BBRC02_E02289", "BBRC02_E02290", "BBRC02_E02291", "BBRC02_E02292", "BBRC02_E02293", "BBRC02_E02294", "BBRC02_E02295", "BBRC02_E02296", "BBRC02_E02297", "BBRC02_E02298", "BBRC02_E02299", "BBRC02_E02307", "BBRC02_E02316", "BBRC02_E02317", "BBRC02_E02318", "BBRC02_E02319", "BBRC02_E02322", "BBRC02_E02324", "BBRC02_E02325", "BBRC02_E02334", "BBRC02_E02335", "BBRC02_E02342", "BBRC02_E02345", "BBRC02_E02347", "BBRC02_E02349", "BBRC02_E02350", "BBRC02_E02351", "BBRC02_E02352", "BBRC02_E02353", "BBRC02_E02354", "BBRC02_E02355", "BBRC02_E02356", "BBRC02_E02370", "BBRC02_E02371", "BBRC02_E02380", "BBRC02_E02381", "BBRC02_E02382", "BBRC02_E02384", "BBRC02_E02387", "BBRC02_E02388", "BBRC02_E02395", "BBRC02_E02396", "BBRC02_E02397", "BBRC02_E02410", "BBRC02_E02411", "BBRC02_E02412", "BBRC02_E02432", "BBRC02_E02438", "BBRC02_E02443", "BBRC02_E02452", "BBRC02_E02467", "BBRC02_E02468", "BBRC02_E02469", "BBRC02_E02473", "BBRC02_E02474", "BBRC02_E02475", "BBRC02_E02476", "BBRC02_E02480", "BBRC02_E02506", "BBRC02_E02516", "BBRC02_E02523", "BBRC02_E02524", "BBRC02_E02848", "BBRC02_E03353", "BBRC02_E03354", "BBRC02_E03355", "BBRC02_E03356", "BBRC02_E03357", "BBRC02_E03358", "BBRC02_E03367", "BBRC02_E03376", "BBRC02_E03378", "BBRC02_E03379", "BBRC02_E03380", "BBRC02_E03383", "BBRC02_E03384", "BBRC02_E03387", "BBRC02_E03388", "BBRC02_E03389", "BBRC02_E03400", "BBRC02_E03401", "BBRC02_E03402", "BBRC02_E03404", "BBRC02_E03405", "BBRC02_E03406", "BBRC02_E03411", "BBRC02_E03413", "BBRC02_E03415", "BBRC02_E03500", "BBRC02_E03502", "BBRC02_E03565", "BBRC02_E03569", "BBRC02_E03570", "BBRC02_E03571", "BBRC02_E03576", "BBRC02_E03581", "BBRC02_E03582", "BBRC02_E03586", "BBRC02_E03587", "BBRC02_E03597", "BBRC02_E03598", "BBRC02_E03599", "BBRC02_E03610", "BBRC02_E03615", "BBRC02_E03616", "BBRC02_E03623", "BBRC02_E03654", "BBRC02_E03655", "BBRC02_E03656", "BBRC02_E03657", "BBRC02_E03658", "BBRC02_E03666", "BBRC02_E03674", "BBRC02_E03675", "BBRC02_E03676", "BBRC02_E03682", "BBRC02_E03683", "BBRC02_E03696", "BBRC02_E03697", "BBRC02_E03698", "BBRC02_E03700", "BBRC02_E03707", "BBRC02_E03716", "BBRC02_E03720", "BBRC02_E03722", "BBRC02_E03724", "BBRC02_E03725", "BBRC02_E03726", "BBRC02_E03730", "BBRC02_E03731", "BBRC02_E03799", "BBRC02_E03801", "BBRC02_E03805", "BBRC02_E03806", "BBRC02_E03807", "BBRC02_E03819", "BBRC02_E03820", "BBRC02_E03823", "BBRC02_E03824", "BBRC02_E03825", "BBRC02_E03826", "BBRC02_E03829", "BBRC02_E03830", "BBRC02_E03833", "BBRC02_E03843", "BBRC02_E03849", "BBRC02_E03854", "BBRC02_E03861", "BBRC02_E03867", "BBRC02_E03868", "BBRC02_E03877", "BBRC02_E03879", "BBRC02_E03886", "BBRC02_E03887", "BBRC02_E03892", "BBRC02_E03897", "BBRC02_E03902", "BBRC02_E03907", "BBRC02_E03919", "BBRC02_E03928", "BBRC02_E03930", "BBRC02_E03931", "BBRC02_E03932", "BBRC02_E03942", "BBRC02_E03943", "BBRC02_E03945", "BBRC02_E03947", "BBRC02_E03948", "BBRC02_E03958", "BBRC02_E03959", "BBRC02_E03972", "BBRC02_E03973", "BBRC02_E04835", "BBRC02_E04930", "BBRC02_E04931", "BBRC02_E04932", "BBRC02_E04933", "BBRC02_E04958", "BBRC02_E04959", "BBRC02_E04971", "BBRC02_E05055", "BBRC02_E05057", "BBRC02_E05070", "BBRC02_E05078", "BBRC02_E05082", "BBRC02_E05089", "BBRC02_E05095", "BBRC02_E05107", "BBRC02_E05112", "BBRC02_E05113", "BBRC02_E05119", "BBRC02_E05125", "BBRC02_E05202", "BBRC02_E05220", "BBRC02_E05221", "BBRC02_E05229", "BBRC02_E05256", "BBRC02_E05262", "BBRC02_E05456", "BBRC02_E05458", "BBRC02_E05461", "BBRC02_E05481", "BBRC02_E05482", "BBRC02_E05484", "BBRC02_E05488", "BBRC02_E05492", "BBRC02_E05495", "BBRC02_E05496", "BBRC02_E05498", "BBRC02_E05502", "BBRC02_E05503", "BBRC02_E05509", "BBRC02_E05516", "BBRC02_E05519", "BBRC02_E05522", "BBRC02_E05528", "BBRC02_E05529", "BBRC02_E05540", "BBRC02_E05696", "BBRC02_E05867", "BBRC02_E05868", "BBRC02_E05872", "BBRC02_E05873", "BBRC02_E05877", "BBRC02_E05879", "BBRC02_E05913", "BBRC02_E05914", "BBRC02_E05923", "BBRC02_E05928", "BBRC02_E05930", "BBRC02_E05935", "BBRC02_E05936", "BBRC02_E05938", "BBRC02_E05943", "BBRC02_E05950", "BBRC02_E05953", "BBRC02_E05954", "BBRC02_E05961", "BBRC02_E05962", "BBRC02_E05967", "BBRC02_E05981", "BBRC02_E05999", "BBRC02_E06000", "BBRC02_E06006", "BBRC02_E06010", "BBRC02_E06014", "BBRC02_E06015", "BBRC02_E06024", "BBRC02_E06029", "BBRC02_E06031", "BBRC02_E06038", "BBRC02_E06048", "BBRC02_E06053", "BBRC02_E06057", "BBRC02_E06074", "BBRC02_E06082", "BBRC02_E06084", "BBRC02_E06088", "BBRC02_E06090", "BBRC02_E06093", "BBRC02_E06097", "BBRC02_E06098", "BBRC02_E06107", "BBRC02_E06117", "BBRC02_E06118", "BBRC02_E06120", "BBRC02_E06124", "BBRC02_E06125", "BBRC02_E06128", "BBRC02_E06129", "BBRC02_E06138", "BBRC02_E06149", "BBRC02_E06151", "BBRC02_E06152", "BBRC02_E06154", "BBRC02_E06155", "BBRC02_E06159", "BBRC02_E06171", "BBRC02_E06197", "BBRC02_E06198", "BBRC02_E06199", "BBRC02_E06202", "BBRC02_E06218", "BBRC02_E06433", "BBRC02_E06561", "BBRC02_E06584", "BBRC02_E06585", "BBRC02_E06586", "BBRC02_E06760", "BBRC02_E06766", "BBRC02_E06899", "BBRC02_E06900", "BBRC02_E07026", "BBRC02_E07185", "BBRC02_E07189", "BBRC02_E07196", "BBRC02_E07197", "BBRC02_E07198", "BBRC02_E07221", "BBRC02_E07229", "BBRC02_E07230", "BBRC02_E07234", "BBRC02_E07242", "BBRC02_E07243", "BBRC02_E07244", "BBRC02_E07246", "BBRC02_E07248", "BBRC02_E07259", "BBRC02_E07260", "BBRC02_E07283", "BBRC02_E07284", "BBRC02_E07285", "BBRC02_E07286", "BBRC02_E07290", "BBRC02_E07305", "BBRC02_E07311", "BBRC02_E07312", "BBRC02_E07326", "BBRC02_E07340", "BBRC02_E07341", "BBRC02_E07343", "BBRC02_E07344", "BBRC02_E07346", "BBRC02_E07350", "BBRC02_E07351", "BBRC02_E07358", "BBRC02_E07361", "BBRC02_E07364", "BBRC02_E07366", "BBRC02_E07372", "BBRC02_E07373", "BBRC02_E07374", "BBRC02_E07378", "BBRC02_E07598", "BBRC02_E07599", "BBRC02_E07608", "BBRC02_E07612", "BBRC02_E07618", "BBRC02_E07619", "BBRC02_E07625", "BBRC02_E07630", "BBRC02_E07634", "BBRC02_E07635", "BBRC02_E07638", "BBRC02_E07639", "BBRC02_E07646", "BBRC02_E07647", "BBRC02_E07649", "BBRC02_E07654", "BBRC02_E07665", "BBRC02_E07701", "BBRC02_E07703", "BBRC02_E07707", "BBRC02_E07717", "BBRC02_E07718", "BBRC02_E07734", "BBRC02_E07743", "BBRC02_E07746", "BBRC02_E07756", "BBRC02_E07757", "BBRC02_E07758", "BBRC02_E07762", "BBRC02_E07764", "BBRC02_E07834", "BBRC02_E07838", "BBRC02_E07846", "BBRC02_E07847", "BBRC02_E07854", "BBRC02_E07858", "BBRC02_E07859", "BBRC02_E07860", "BBRC02_E07867", "BBRC02_E07869", "BBRC02_E07872", "BBRC02_E07873", "BBRC02_E07883", "BBRC02_E07884", "BBRC02_E07885", "BBRC02_E07886", "BBRC02_E07887", "BBRC02_E07890", "BBRC02_E07898", "BBRC02_E07910", "BBRC02_E07911", "BBRC02_E07912", "BBRC02_E07913", "BBRC02_E07914", "BBRC02_E07915", "BBRC02_E07917", "BBRC02_E07918", "BBRC02_E07919", "BBRC02_E07925", "BBRC02_E07926", "BBRC02_E07927", "BBRC02_E07928", "BBRC02_E07929", "BBRC02_E07930", "BBRC02_E07931", "BBRC02_E07932", "BBRC02_E08038", "BBRC02_E08052", "BBRC02_E08296", "BBRC02_E08538", "BBRC02_E08687", "BBRC02_E08688", "BBRC02_E08689", "BBRC02_E08690", "BBRC_E00045", "BBRC_E00046", "BBRC_E00048", "BBRC_E00049", "BBRC_E00050", "BBRC_E00051", "BBRC_E00052", "BBRC_E00053", "BBRC_E00054", "BBRC_E00055", "BBRC_E00062", "BBRC_E00063", "BBRC_E00067", "BBRC_E00068", "BBRC_E00070", "BBRC_E00071", "BBRC_E00073", "BBRC_E00074", "BBRC_E00075", "BBRC_E00077", "BBRC_E00078", "BBRC_E00079", "BBRC_E00080", "BBRC_E00087", "BBRC_E00089", "BBRC_E00093", "BBRC_E00095", "BBRC_E00096", "BBRC_E00097", "BBRC_E00098", "BBRC_E00099", "BBRC_E00100", "BBRC_E00101", "BBRC_E00102", "BBRC_E00103", "BBRC_E00106", "BBRC_E00107", "BBRC_E00108", "BBRC_E00109", "BBRC_E00110", "BBRC_E00111", "BBRC_E00112", "BBRC_E00113", "BBRC_E00114", "BBRC_E00115", "BBRC_E00116", "BBRC_E00117", "BBRC_E00185", "BBRC_E00186", "BBRC_E00187", "BBRC_E00188", "BBRC_E00189", "BBRC_E00190", "BBRC_E00191", "BBRC_E00192", "BBRC_E00193", "BBRC_E00194", "BBRC_E00195", "BBRC_E00196", "BBRC_E00197", "BBRC_E00198", "BBRC_E00199", "BBRC_E00200", "BBRC_E00201", "BBRC_E00202", "BBRC_E00203", "BBRC_E00204", "BBRC_E00205", "BBRC_E00206", "BBRC_E00207", "BBRC_E00208", "BBRC_E00209", "BBRC_E00210", "BBRC_E00211", "BBRC_E00212", "BBRC_E00213", "BBRC_E00214", "BBRC_E00215", "BBRC_E00216", "BBRC_E00217", "BBRC_E00218", "BBRC_E00219", "BBRC_E00220", "BBRC_E00221", "BBRC_E00222", "BBRC_E00223", "BBRC_E00224", "BBRC_E00225", "BBRC_E00226", "BBRC_E00227", "BBRC_E00228", "BBRC_E00229", "BBRC_E00230", "BBRC_E00231", "BBRC_E00232", "BBRC_E00234", "BBRC_E00235", "BBRC_E00237", "BBRC_E00238", "BBRC_E00240", "BBRC_E00241", "BBRC_E00242", "BBRC_E00244", "BBRC_E00245", "BBRC_E00246", "BBRC_E00247", "BBRC_E00248", "BBRC_E00249", "BBRC_E00250", "BBRC_E00251", "BBRC_E00252", "BBRC_E00253", "BBRC_E00255", "BBRC_E00256", "BBRC_E00257", "BBRC_E00258", "BBRC_E00259", "BBRC_E00263", "BBRC_E00264", "BBRC_E00265", "BBRC_E00266", "BBRC_E00267", "BBRC_E00268", "BBRC_E00269", "BBRC_E00271", "BBRC_E00272", "BBRC_E00273", "BBRC_E00274", "BBRC_E00275", "BBRC_E00276", "BBRC_E00277", "BBRC_E00278", "BBRC_E00279", "BBRC_E00280", "BBRC_E00281", "BBRC_E00282", "BBRC_E00283", "BBRC_E00284", "BBRC_E00285", "BBRC_E00286", "BBRC_E00287", "BBRC_E00288", "BBRC_E00289", "BBRC_E00290", "BBRC_E00291", "BBRC_E00292", "BBRC_E00293", "BBRC_E00294", "BBRC_E00295", "BBRC_E00296", "BBRC_E00297", "BBRC_E00298", "BBRC_E00299", "BBRC_E00300", "BBRC_E00301", "BBRC_E00302", "BBRC_E00303", "BBRC_E00304", "BBRC_E00305", "BBRC_E00306", "BBRC_E00307", "BBRC_E00308", "BBRC_E00310", "BBRC_E00311", "BBRC_E00312", "BBRC_E00313", "BBRC_E00314", "BBRC_E00315", "BBRC_E00316", "BBRC_E00317", "BBRC_E00318", "BBRC_E00319", "BBRC_E00320", "BBRC_E00321", "BBRC_E00322", "BBRC_E00323", "BBRC_E00324", "BBRC_E00325", "BBRC_E00326", "BBRC_E00327", "BBRC_E00328", "BBRC_E00329", "BBRC_E00330", "BBRC_E00331", "BBRC_E00332", "BBRC_E00333", "BBRC_E00334", "BBRC_E00335", "BBRC_E00337", "BBRC_E00338", "BBRC_E00339", "BBRC_E00340", "BBRC_E00341", "BBRC_E00342", "BBRC_E00343", "BBRC_E00344", "BBRC_E00345", "BBRC_E00346", "BBRC_E00347", "BBRC_E00348", "BBRC_E00349", "BBRC_E00350", "BBRC_E00351", "BBRC_E00352", "BBRC_E00353", "BBRC_E00354", "BBRC_E00355", "BBRC_E00356", "BBRC_E00357", "BBRC_E00358", "BBRC_E00359", "BBRC_E00360", "BBRC_E00361", "BBRC_E00362", "BBRC_E00363", "BBRC_E00364", "BBRC_E00365", "BBRC_E00366", "BBRC_E00367", "BBRC_E00368", "BBRC_E00369", "BBRC_E00370", "BBRC_E00371", "BBRC_E00372", "BBRC_E00373", "BBRC_E00374", "BBRC_E00375", "BBRC_E00376", "BBRC_E00377", "BBRC_E00378", "BBRC_E00379", "BBRC_E00380", "BBRC_E00381", "BBRC_E00382", "BBRC_E00383", "BBRC_E00384", "BBRC_E00385", "BBRC_E00386", "BBRC_E00387", "BBRC_E00388", "BBRC_E00389", "BBRC_E00390", "BBRC_E00391", "BBRC_E00392", "BBRC_E00393", "BBRC_E00394", "BBRC_E00395", "BBRC_E00396", "BBRC_E00397", "BBRC_E00398", "BBRC_E00399", "BBRC_E00400", "BBRC_E00401", "BBRC_E00402", "BBRC_E00403", "BBRC_E00404", "BBRC_E00405", "BBRC_E00406", "BBRC_E00407", "BBRC_E00408", "BBRC_E00409", "BBRC_E00410", "BBRC_E00411", "BBRC_E00412", "BBRC_E00413", "BBRC_E00414", "BBRC_E00415", "BBRC_E00416", "BBRC_E00417", "BBRC_E00418", "BBRC_E00419", "BBRC_E00420", "BBRC_E00421", "BBRC_E00422", "BBRC_E00423", "BBRC_E00424", "BBRC_E00425", "BBRC_E00426", "BBRC_E00427", "BBRC_E00428", "BBRC_E00429", "BBRC_E00430", "BBRC_E00431", "BBRC_E00432", "BBRC_E00433", "BBRC_E00434", "BBRC_E00435", "BBRC_E00436", "BBRC_E00437", "BBRC_E00438", "BBRC_E00439", "BBRC_E00440", "BBRC_E00441", "BBRC_E00442", "BBRC_E00443", "BBRC_E00444", "BBRC_E00445", "BBRC_E00446", "BBRC_E00447", "BBRC_E00448", "BBRC_E00449", "BBRC_E00450", "BBRC_E00451", "BBRC_E00452", "BBRC_E00453", "BBRC_E00454", "BBRC_E00455", "BBRC_E00456", "BBRC_E00457", "BBRC_E00458", "BBRC_E00459", "BBRC_E00460", "BBRC_E00461", "BBRC_E00462", "BBRC_E00463", "BBRC_E00464", "BBRC_E00465", "BBRC_E00466", "BBRC_E00467", "BBRC_E00468", "BBRC_E00469", "BBRC_E00470", "BBRC_E00471", "BBRC_E00472", "BBRC_E00473", "BBRC_E00474", "BBRC_E00475", "BBRC_E00476", "BBRC_E00477", "BBRC_E00478", "BBRC_E00479", "BBRC_E00480", "BBRC_E00481", "BBRC_E00482", "BBRC_E00483", "BBRC_E00484", "BBRC_E00485", "BBRC_E00486", "BBRC_E00487", "BBRC_E00488", "BBRC_E00489", "BBRC_E00490", "BBRC_E00491", "BBRC_E00492", "BBRC_E00493", "BBRC_E00494", "BBRC_E00495", "BBRC_E00496", "BBRC_E00497", "BBRC_E00498", "BBRC_E00499", "BBRC_E00500", "BBRC_E00501", "BBRC_E00502", "BBRC_E00503", "BBRC_E00504", "BBRC_E00505", "BBRC_E00506", "BBRC_E00507", "BBRC_E00508", "BBRC_E00509", "BBRC_E00510", "BBRC_E00511", "BBRC_E00512", "BBRC_E00513", "BBRC_E00514", "BBRC_E00515", "BBRC_E00516", "BBRC_E00517", "BBRC_E00518", "BBRC_E00519", "BBRC_E00520", "BBRC_E00521", "BBRC_E00522", "BBRC_E00523", "BBRC_E00524", "BBRC_E00525", "BBRC_E00526", "BBRC_E00527", "BBRC_E00528", "BBRC_E00529", "BBRC_E00530", "BBRC_E00531", "BBRC_E00532", "BBRC_E00533", "BBRC_E00535", "BBRC_E00967", "BBRC_E01025", "BBRC_E01031", "BBRC_E01039", "BBRC_E01042", "BBRC_E01043", "BBRC_E01044", "BBRC_E01045", "BBRC_E01046", "BBRC_E01048", "BBRC_E01051", "BBRC_E01053", "BBRC_E01054", "BBRC_E01055", "BBRC_E01108", "BBRC_E01120", "BBRC_E01128", "BBRC_E01148", "BBRC_E01215", "BBRC_E01274", "BBRC_E01317", "BBRC_E01318", "BBRC_E01324", "BBRC_E01325", "BBRC_E01326", "BBRC_E01351", "BBRC_E01352", "BBRC_E01356", "BBRC_E01360", "BBRC_E01364", "BBRC_E01366", "BBRC_E01367", "BBRC_E01377", "BBRC_E01378", "BBRC_E01379", "BBRC_E01500", "BBRC_E01537", "BBRC_E01538", "BBRC_E01545", "BBRC_E01554", "BBRC_E01576", "BBRC_E01590", "BBRC_E01607", "BBRC_E01626", "BBRC_E01778", "BBRC_E01932", "BBRC_E01935", "BBRC_E01944", "BBRC_E01946", "BBRC_E01971", "BBRC_E01985", "BBRC_E01991", "BBRC_E01992", "BBRC_E01993", "BBRC_E01994", "BBRC_E02004", "BBRC_E02005", "BBRC_E02007", "BBRC_E02008", "BBRC_E02009", "BBRC_E02010", "BBRC_E02011", "BBRC_E02012", "BBRC_E02014", "BBRC_E02015", "BBRC_E02016", "BBRC_E02017", "BBRC_E02018", "BBRC_E02019", "BBRC_E02020", "BBRC_E02021", "BBRC_E02022", "BBRC_E02023", "BBRC_E02024", "BBRC_E02026", "BBRC_E02030", "BBRC_E02031", "BBRC_E02036", "BBRC_E02041", "BBRC_E02043", "BBRC_E02044", "BBRC_E02045", "BBRC_E02046", "BBRC_E02047", "BBRC_E02048", "BBRC_E02065", "BBRC_E02066", "BBRC_E02067", "BBRC_E02070", "BBRC_E02071", "BBRC_E02072", "BBRC_E02076", "BBRC_E02079", "BBRC_E02080", "BBRC_E02081", "BBRC_E02082", "BBRC_E02083", "BBRC_E02084", "BBRC_E02085", "BBRC_E02086", "BBRC_E02087", "BBRC_E02088", "BBRC_E02089", "BBRC_E02102", "BBRC_E02105", "BBRC_E02108", "BBRC_E02109", "BBRC_E02110", "BBRC_E02111", "BBRC_E02115", "BBRC_E02116", "BBRC_E02118", "BBRC_E02119", "BBRC_E02120", "BBRC_E02124", "BBRC_E02136", "BBRC_E02142", "BBRC_E02155", "BBRC_E02156", "BBRC_E02158", "BBRC_E02159", "BBRC_E02160", "BBRC_E02161", "BBRC_E02173", "BBRC_E02174", "BBRC_E02175", "BBRC_E02176", "BBRC_E02177", "BBRC_E02178", "BBRC_E02189", "BBRC_E02190", "BBRC_E02191", "BBRC_E02192", "BBRC_E02193", "BBRC_E02194", "BBRC_E02195", "BBRC_E02225", "BBRC_E02229", "BBRC_E02233", "BBRC_E02238", "BBRC_E02241", "BBRC_E02478", "BBRC_E02479", "BBRC_E02480", "BBRC_E02502", "BBRC_E02503", "BBRC_E02507", "BBRC_E02511", "BBRC_E02512", "BBRC_E02513", "BBRC_E02514", "BBRC_E02515", "BBRC_E02516", "BBRC_E02524", "BBRC_E02525", "BBRC_E02526", "BBRC_E02528", "BBRC_E02529", "BBRC_E02562", "BBRC_E02573", "BBRC_E02577", "BBRC_E02585", "BBRC_E02587", "BBRC_E02591", "BBRC_E02592", "BBRC_E02593", "BBRC_E02594", "BBRC_E02598", "BBRC_E02599", "BBRC_E02600", "BBRC_E02601", "BBRC_E02602", "BBRC_E02603", "BBRC_E02607", "BBRC_E02608", "BBRC_E02614", "BBRC_E02615", "BBRC_E02616", "BBRC_E02617", "BBRC_E02618", "BBRC_E02619", "BBRC_E02626", "BBRC_E02627", "BBRC_E02628", "BBRC_E02629", "BBRC_E02631"]
 
 ALFA_20220301 = ALFA_20201001 + ['BBRC2_E00696', 'BBRC2_E02291']
 
 DARTEL_ALFA_20220301 = list(set(ALFA_20220301) - {'BBRC02_E00764', 'BBRC_E02577', 'BBRC02_E00851', 'BBRC02_E07915'})
@@ -26,14 +29,15 @@
 
 LONG_V2_MRI_ALFA_PET_FTM_202202810 = ['BBRC2_E00145', 'BBRC2_E00231', 'BBRC2_E00692', 'BBRC2_E00325', 'BBRC2_E02381', 'BBRC02_E08581', 'BBRC2_E00519', 'BBRC2_E00118', 'BBRC2_E00606', 'BBRC2_E01035', 'BBRC2_E00957', 'BBRC2_E00624', 'BBRC2_E00193', 'BBRC2_E02206', 'BBRC2_E02166', 'BBRC02_E08529', 'BBRC2_E01756', 'BBRC2_E00909', 'BBRC2_E00875', 'BBRC2_E02390', 'BBRC2_E01483', 'BBRC2_E01484', 'BBRC2_E00905', 'BBRC2_E01625', 'BBRC2_E01761', 'BBRC2_E01112', 'BBRC2_E00755', 'BBRC2_E02817', 'BBRC2_E00487', 'BBRC2_E03394', 'BBRC2_E00774', 'BBRC2_E00599', 'BBRC2_E01066', 'BBRC2_E01850', 'BBRC2_E04156', 'BBRC2_E00904', 'BBRC2_E00860', 'BBRC2_E01123', 'BBRC2_E00654', 'BBRC2_E02730', 'BBRC2_E00326', 'BBRC2_E02034', 'BBRC2_E03261', 'BBRC2_E02015', 'BBRC2_E00593', 'BBRC2_E00769', 'BBRC02_E08446', 'BBRC2_E00483', 'BBRC2_E01019', 'BBRC2_E00802', 'BBRC2_E00563', 'BBRC2_E00578', 'BBRC2_E00577', 'BBRC2_E01485', 'BBRC2_E00355', 'BBRC2_E02177', 'BBRC2_E02980', 'BBRC2_E03653', 'BBRC2_E01936', 'BBRC2_E00101', 'BBRC2_E00155', 'BBRC2_E01424', 'BBRC2_E00645', 'BBRC2_E00789', 'BBRC2_E03023', 'BBRC2_E00598', 'BBRC2_E03252', 'BBRC02_E08159', 'BBRC2_E00381', 'BBRC2_E02245', 'BBRC2_E00745', 'BBRC2_E02006', 'BBRC2_E00656', 'BBRC2_E00553', 'BBRC2_E00618', 'BBRC2_E01154', 'BBRC2_E01516', 'BBRC02_E08569', 'BBRC2_E00824', 'BBRC2_E00458', 'BBRC2_E00926', 'BBRC2_E01927', 'BBRC2_E01530', 'BBRC2_E01417', 'BBRC02_E08586', 'BBRC2_E02331', 'BBRC2_E02050', 'BBRC2_E00250', 'BBRC2_E00971', 'BBRC2_E00439', 'BBRC2_E01745', 'BBRC2_E02044', 'BBRC2_E01134', 'BBRC2_E02763', 'BBRC2_E01370', 'BBRC2_E03402', 'BBRC2_E02322', 'BBRC2_E00340', 'BBRC2_E03017', 'BBRC2_E00636', 'BBRC2_E01135', 'BBRC2_E00756', 'BBRC02_E08609', 'BBRC2_E01071', 'BBRC02_E08324', 'BBRC2_E00838', 'BBRC2_E03074', 'BBRC2_E03060', 'BBRC2_E00395', 'BBRC2_E00794', 'BBRC2_E01472', 'BBRC2_E00413', 'BBRC2_E02950', 'BBRC2_E02207', 'BBRC2_E02214', 'BBRC2_E00657', 'BBRC2_E00810', 'BBRC2_E00989', 'BBRC2_E01528', 'BBRC2_E00182', 'BBRC2_E00621', 'BBRC2_E02226', 'BBRC2_E00159', 'BBRC2_E02309', 'BBRC2_E02382', 'BBRC2_E00672', 'BBRC2_E02340', 'BBRC2_E00677', 'BBRC2_E00716', 'BBRC2_E00658', 'BBRC2_E00676', 'BBRC2_E00111', 'BBRC2_E03269', 'BBRC2_E00943', 'BBRC2_E01492', 'BBRC02_E08614', 'BBRC2_E02811', 'BBRC2_E00970', 'BBRC2_E01377', 'BBRC2_E02921', 'BBRC2_E02299', 'BBRC2_E00938', 'BBRC2_E01931', 'BBRC2_E01722', 'BBRC2_E00584', 'BBRC2_E02347', 'BBRC2_E01119', 'BBRC2_E01974', 'BBRC2_E01521', 'BBRC02_E08397', 'BBRC2_E02422', 'BBRC2_E01460', 'BBRC2_E00516', 'BBRC2_E00633', 'BBRC2_E00289', 'BBRC2_E00301', 'BBRC2_E04109', 'BBRC02_E08610', 'BBRC2_E03058', 'BBRC02_E08516', 'BBRC2_E01128', 'BBRC2_E00874', 'BBRC2_E00153', 'BBRC2_E00531', 'BBRC2_E04517', 'BBRC2_E00428', 'BBRC2_E00897', 'BBRC2_E01012', 'BBRC2_E02323', 'BBRC2_E04203', 'BBRC2_E01778', 'BBRC2_E00937', 'BBRC2_E03011', 'BBRC2_E02765', 'BBRC2_E01494', 'BBRC2_E03645', 'BBRC2_E03006', 'BBRC2_E00724', 'BBRC2_E00552', 'BBRC2_E03014', 'BBRC2_E00877', 'BBRC02_E08632', 'BBRC2_E00134', 'BBRC2_E02054', 'BBRC2_E00232', 'BBRC2_E00310', 'BBRC02_E08436', 'BBRC2_E01869', 'BBRC02_E08442', 'BBRC2_E03233', 'BBRC2_E02165', 'BBRC2_E02864', 'BBRC2_E00942', 'BBRC2_E00164', 'BBRC2_E01092', 'BBRC2_E00136', 'BBRC02_E08382', 'BBRC2_E02406', 'BBRC2_E04313', 'BBRC2_E00394', 'BBRC2_E01007', 'BBRC2_E00701', 'BBRC2_E01508', 'BBRC2_E00271', 'BBRC2_E00790', 'BBRC2_E01184', 'BBRC02_E08387', 'BBRC2_E01937', 'BBRC2_E00278', 'BBRC02_E08473', 'BBRC2_E02296']
 
 PENSA_MRI_V1_20220330 = ['BBRC02_E08311', 'BBRC02_E08312', 'BBRC02_E08319', 'BBRC02_E08357', 'BBRC02_E08361', 'BBRC02_E08367', 'BBRC02_E08371', 'BBRC02_E08381', 'BBRC02_E08383', 'BBRC02_E08386', 'BBRC02_E08396', 'BBRC02_E08410', 'BBRC02_E08430', 'BBRC02_E08448', 'BBRC02_E08475', 'BBRC02_E08476', 'BBRC02_E08478', 'BBRC02_E08500', 'BBRC02_E08512', 'BBRC02_E08537', 'BBRC02_E08513', 'BBRC02_E08531', 'BBRC2_E00049', 'BBRC2_E00063', 'BBRC2_E00064', 'BBRC2_E00659', 'BBRC2_E01121', 'BBRC2_E00137', 'BBRC2_E00098', 'BBRC2_E00103', 'BBRC2_E00104', 'BBRC2_E00121', 'BBRC2_E00131', 'BBRC2_E00222', 'BBRC2_E00251', 'BBRC2_E00269', 'BBRC2_E00275', 'BBRC2_E00295', 'BBRC2_E00296', 'BBRC2_E00299', 'BBRC2_E00300', 'BBRC2_E00302', 'BBRC2_E00324', 'BBRC2_E00339', 'BBRC2_E00365', 'BBRC2_E00379', 'BBRC2_E00380', 'BBRC2_E00402', 'BBRC2_E00403', 'BBRC2_E00404', 'BBRC2_E00405', 'BBRC2_E00406', 'BBRC2_E00438', 'BBRC2_E00459', 'BBRC2_E00469', 'BBRC2_E00508', 'BBRC2_E00511', 'BBRC2_E00513', 'BBRC2_E00521', 'BBRC2_E00524', 'BBRC2_E00526', 'BBRC2_E00527', 'BBRC2_E00533', 'BBRC2_E00537', 'BBRC2_E00543', 'BBRC2_E00550', 'BBRC2_E00554', 'BBRC2_E00556', 'BBRC2_E00557', 'BBRC2_E00564', 'BBRC2_E00566', 'BBRC2_E00572', 'BBRC2_E00573', 'BBRC2_E00581', 'BBRC2_E00582', 'BBRC2_E00592', 'BBRC2_E00608', 'BBRC2_E00617', 'BBRC2_E00622', 'BBRC2_E00634', 'BBRC2_E00644', 'BBRC2_E00653', 'BBRC2_E00666', 'BBRC2_E00674', 'BBRC2_E00697', 'BBRC2_E00698', 'BBRC2_E00702', 'BBRC2_E00709', 'BBRC2_E00725', 'BBRC2_E00741', 'BBRC2_E00742', 'BBRC2_E00743', 'BBRC2_E00749', 'BBRC2_E00775', 'BBRC2_E00788', 'BBRC2_E00792', 'BBRC2_E00795', 'BBRC2_E00798', 'BBRC2_E00823', 'BBRC2_E00825', 'BBRC2_E00839', 'BBRC2_E00846', 'BBRC2_E00849', 'BBRC2_E00859', 'BBRC2_E00878', 'BBRC2_E00879', 'BBRC2_E00920', 'BBRC2_E00939', 'BBRC2_E00944', 'BBRC2_E00954', 'BBRC2_E00955', 'BBRC2_E00962', 'BBRC2_E00964', 'BBRC2_E00972', 'BBRC2_E00990', 'BBRC2_E00992', 'BBRC2_E01020', 'BBRC2_E01027', 'BBRC2_E01030', 'BBRC2_E01038', 'BBRC2_E01039', 'BBRC2_E01052', 'BBRC2_E01072', 'BBRC2_E01077', 'BBRC2_E01078', 'BBRC2_E01104', 'BBRC2_E01111', 'BBRC2_E01113', 'BBRC2_E01127', 'BBRC2_E01129', 'BBRC2_E01155', 'BBRC2_E01161', 'BBRC2_E01185', 'BBRC2_E01391', 'BBRC2_E01423', 'BBRC2_E01495', 'BBRC2_E01522', 'BBRC2_E01532', 'BBRC2_E01540', 'BBRC2_E01627', 'BBRC2_E01626', 'BBRC2_E01659', 'BBRC2_E01724', 'BBRC2_E01725', 'BBRC2_E01733', 'BBRC2_E01775', 'BBRC2_E01783', 'BBRC2_E01821', 'BBRC2_E01834', 'BBRC2_E01837', 'BBRC2_E01839', 'BBRC2_E01846', 'BBRC2_E01941', 'BBRC2_E02009', 'BBRC2_E02198']
 
 PENSA_MRI_V2_20220330 = ['BBRC2_E02175', 'BBRC2_E01511', 'BBRC2_E01453', 'BBRC2_E01519', 'BBRC2_E01462', 'BBRC2_E01416', 'BBRC2_E01459', 'BBRC2_E02247', 'BBRC2_E01510', 'BBRC2_E01542', 'BBRC2_E01445', 'BBRC2_E02353', 'BBRC2_E02267', 'BBRC2_E02303', 'BBRC2_E01471', 'BBRC2_E01539', 'BBRC2_E02338', 'BBRC2_E02647', 'BBRC2_E02119', 'BBRC2_E02212']
 
+ALFA_PLUS_V2_20230518 = ['BBRC02_E08585', 'BBRC2_E00145', 'BBRC2_E03092', 'BBRC2_E00231', 'BBRC2_E00571', 'BBRC2_E00382', 'BBRC2_E00325', 'BBRC2_E02381', 'BBRC02_E08581', 'BBRC2_E00519', 'BBRC2_E00464', 'BBRC2_E00118', 'BBRC2_E00606', 'BBRC2_E01035', 'BBRC2_E01028', 'BBRC2_E00544', 'BBRC2_E00957', 'BBRC2_E01407', 'BBRC2_E00624', 'BBRC2_E04182', 'BBRC2_E00193', 'BBRC2_E02206', 'BBRC2_E00700', 'BBRC2_E02166', 'BBRC02_E08529', 'BBRC2_E00092', 'BBRC2_E00909', 'BBRC2_E00746', 'BBRC2_E00875', 'BBRC2_E02390', 'BBRC2_E01483', 'BBRC02_E08541', 'BBRC2_E00905', 'BBRC2_E01625', 'BBRC2_E04436', 'BBRC2_E01761', 'BBRC2_E02939', 'BBRC2_E01112', 'BBRC2_E05018', 'BBRC2_E00347', 'BBRC2_E00755', 'BBRC2_E02817', 'BBRC2_E01533', 'BBRC2_E02288', 'BBRC2_E00487', 'BBRC2_E02804', 'BBRC2_E02101', 'BBRC2_E03358', 'BBRC2_E02199', 'BBRC02_E08670', 'BBRC2_E00599', 'BBRC2_E00549', 'BBRC2_E02875', 'BBRC2_E01066', 'BBRC2_E01850', 'BBRC2_E04156', 'BBRC2_E00201', 'BBRC2_E00904', 'BBRC2_E00860', 'BBRC2_E00422', 'BBRC2_E00448', 'BBRC2_E00536', 'BBRC2_E02730', 'BBRC2_E00326', 'BBRC2_E00635', 'BBRC2_E01512', 'BBRC2_E01070', 'BBRC2_E03261', 'BBRC2_E02015', 'BBRC2_E04754', 'BBRC2_E00593', 'BBRC2_E00769', 'BBRC2_E03344', 'BBRC02_E08446', 'BBRC2_E01389', 'BBRC2_E00483', 'BBRC2_E03298', 'BBRC2_E00616', 'BBRC2_E00188', 'BBRC2_E01019', 'BBRC2_E04802', 'BBRC2_E03371', 'BBRC2_E00354', 'BBRC2_E00563', 'BBRC2_E04165', 'BBRC02_E08351', 'BBRC2_E00578', 'BBRC2_E00451', 'BBRC2_E02332', 'BBRC2_E00471', 'BBRC2_E01087', 'BBRC2_E04861', 'BBRC2_E00577', 'BBRC2_E00463', 'BBRC02_E08314', 'BBRC02_E08613', 'BBRC2_E01476', 'BBRC2_E00466', 'BBRC2_E00876', 'BBRC2_E00355', 'BBRC2_E02717', 'BBRC2_E01107', 'BBRC2_E02177', 'BBRC2_E01094', 'BBRC2_E00535', 'BBRC2_E02024', 'BBRC2_E02980', 'BBRC2_E03653', 'BBRC2_E00240', 'BBRC2_E01936', 'BBRC2_E00101', 'BBRC2_E00155', 'BBRC2_E00580', 'BBRC2_E00868', 'BBRC02_E08504', 'BBRC2_E03325', 'BBRC2_E00645', 'BBRC2_E00789', 'BBRC02_E08310', 'BBRC2_E03023', 'BBRC2_E00598', 'BBRC2_E03252', 'BBRC02_E08159', 'BBRC2_E00381', 'BBRC2_E01981', 'BBRC2_E02245', 'BBRC2_E00745', 'BBRC2_E00681', 'BBRC2_E00421', 'BBRC02_E08482', 'BBRC2_E00656', 'BBRC2_E04884', 'BBRC2_E01050', 'BBRC2_E00553', 'BBRC2_E00294', 'BBRC2_E01154', 'BBRC2_E01516', 'BBRC2_E04250', 'BBRC02_E08569', 'BBRC2_E00824', 'BBRC2_E00458', 'BBRC2_E03243', 'BBRC2_E04897', 'BBRC2_E00926', 'BBRC2_E01927', 'BBRC2_E00200', 'BBRC2_E01530', 'BBRC2_E01417', 'BBRC02_E08586', 'BBRC02_E08118', 'BBRC2_E00235', 'BBRC2_E01536', 'BBRC2_E02331', 'BBRC2_E02364', 'BBRC2_E01925', 'BBRC2_E00602', 'BBRC2_E02050', 'BBRC2_E04892', 'BBRC2_E04396', 'BBRC02_E08466', 'BBRC2_E00971', 'BBRC2_E00439', 'BBRC2_E01745', 'BBRC2_E02044', 'BBRC2_E01134', 'BBRC2_E02763', 'BBRC2_E02851', 'BBRC2_E01370', 'BBRC2_E00420', 'BBRC2_E01102', 'BBRC2_E02935', 'BBRC2_E01383', 'BBRC2_E02236', 'BBRC2_E00532', 'BBRC2_E03402', 'BBRC2_E04275', 'BBRC2_E02322', 'BBRC2_E00340', 'BBRC2_E00590', 'BBRC2_E01384', 'BBRC2_E00636', 'BBRC2_E01135', 'BBRC02_E08454', 'BBRC2_E03365', 'BBRC2_E00708', 'BBRC2_E00756', 'BBRC02_E08609', 'BBRC2_E04658', 'BBRC2_E01071', 'BBRC02_E08324', 'BBRC02_E08546', 'BBRC2_E03295', 'BBRC2_E00838', 'BBRC02_E08305', 'BBRC2_E02917', 'BBRC2_E01168', 'BBRC2_E03074', 'BBRC2_E01447', 'BBRC2_E05679', 'BBRC2_E00723', 'BBRC2_E02038', 'BBRC2_E03060', 'BBRC2_E00319', 'BBRC2_E03629', 'BBRC2_E00395', 'BBRC2_E00794', 'BBRC02_E08458', 'BBRC2_E01982', 'BBRC2_E04372', 'BBRC02_E08275', 'BBRC2_E00413', 'BBRC2_E02950', 'BBRC2_E02396', 'BBRC2_E00143', 'BBRC2_E02207', 'BBRC2_E04454', 'BBRC2_E02214', 'BBRC2_E00657', 'BBRC2_E01975', 'BBRC2_E00689', 'BBRC2_E02951', 'BBRC2_E00810', 'BBRC2_E00989', 'BBRC2_E01528', 'BBRC2_E02265', 'BBRC2_E00182', 'BBRC2_E00621', 'BBRC02_E08283', 'BBRC2_E00159', 'BBRC2_E02309', 'BBRC02_E08260', 'BBRC2_E00541', 'BBRC2_E02382', 'BBRC2_E00672', 'BBRC02_E08359', 'BBRC2_E02340', 'BBRC2_E00677', 'BBRC2_E00716', 'BBRC2_E00658', 'BBRC2_E00744', 'BBRC2_E00676', 'BBRC2_E00751', 'BBRC2_E00111', 'BBRC02_E08337', 'BBRC2_E00917', 'BBRC2_E00943', 'BBRC02_E08479', 'BBRC02_E08614', 'BBRC2_E02811', 'BBRC2_E00472', 'BBRC2_E00970', 'BBRC2_E01377', 'BBRC2_E03354', 'BBRC2_E02921', 'BBRC2_E02299', 'BBRC2_E00938', 'BBRC2_E01931', 'BBRC2_E01489', 'BBRC2_E01722', 'BBRC2_E00584', 'BBRC2_E04249', 'BBRC2_E02347', 'BBRC2_E01119', 'BBRC2_E01963', 'BBRC2_E02968', 'BBRC2_E01426', 'BBRC2_E02964', 'BBRC2_E00799', 'BBRC2_E01974', 'BBRC2_E01521', 'BBRC2_E02850', 'BBRC02_E08397', 'BBRC2_E02422', 'BBRC02_E08323', 'BBRC2_E01460', 'BBRC2_E04567', 'BBRC2_E01717', 'BBRC2_E02074', 'BBRC2_E00516', 'BBRC2_E00633', 'BBRC2_E00270', 'BBRC2_E00289', 'BBRC2_E00301', 'BBRC2_E04109', 'BBRC02_E08610', 'BBRC2_E00306', 'BBRC2_E00389', 'BBRC2_E03058', 'BBRC02_E08516', 'BBRC2_E01452', 'BBRC2_E01128', 'BBRC2_E00874', 'BBRC2_E00153', 'BBRC2_E00531', 'BBRC2_E00667', 'BBRC2_E00423', 'BBRC2_E00428', 'BBRC2_E02118', 'BBRC2_E00897', 'BBRC2_E01012', 'BBRC2_E04932', 'BBRC2_E02323', 'BBRC2_E04203', 'BBRC2_E00891', 'BBRC2_E00392', 'BBRC2_E00525', 'BBRC2_E01029', 'BBRC2_E00457', 'BBRC2_E00854', 'BBRC2_E00937', 'BBRC2_E03011', 'BBRC2_E02765', 'BBRC2_E01494', 'BBRC2_E03645', 'BBRC2_E03006', 'BBRC02_E08356', 'BBRC2_E00694', 'BBRC2_E02634', 'BBRC2_E00724', 'BBRC2_E00552', 'BBRC02_E08307', 'BBRC2_E03014', 'BBRC2_E00877', 'BBRC02_E08632', 'BBRC2_E00134', 'BBRC2_E01517', 'BBRC2_E00179', 'BBRC2_E04808', 'BBRC2_E00232', 'BBRC2_E01390', 'BBRC2_E00310', 'BBRC2_E00412', 'BBRC02_E08436', 'BBRC2_E01869', 'BBRC02_E08442', 'BBRC2_E03233', 'BBRC2_E00479', 'BBRC2_E02165', 'BBRC2_E02864', 'BBRC2_E00652', 'BBRC2_E00164', 'BBRC02_E08285', 'BBRC2_E00664', 'BBRC02_E08362', 'BBRC2_E00136', 'BBRC2_E04933', 'BBRC2_E02395', 'BBRC02_E08382', 'BBRC2_E02406', 'BBRC2_E03043', 'BBRC2_E04313', 'BBRC2_E02916', 'BBRC2_E00205', 'BBRC2_E00394', 'BBRC2_E01007', 'BBRC2_E04343', 'BBRC2_E00701', 'BBRC2_E01508', 'BBRC2_E00271', 'BBRC2_E00223', 'BBRC2_E00790', 'BBRC2_E01184', 'BBRC02_E08387', 'BBRC2_E00447', 'BBRC2_E01937', 'BBRC2_E00278', 'BBRC2_E04695', 'BBRC02_E08473', 'BBRC2_E02296', 'BBRC2_E00629', 'BBRC02_E08534']
 
 class ListsCommand(Command):
     """Manage experiment lists curated by BarcelonaBeta.
 
     Available subcommands:
      show:\t\tdisplay all existing lists (usage: bx lists show)
```

### Comparing `bbrc-bx-0.5/bx/nifti.py` & `bbrc-bx-0.5.1/bx/nifti.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/parse.py` & `bbrc-bx-0.5.1/bx/parse.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/pet.py` & `bbrc-bx-0.5.1/bx/pet.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,23 +8,24 @@
     """18F-fluorodeoxyglucose PET imaging data
 
     Available subcommands:
      landau:\t\tcreates an Excel table with the Landau's metaROI signature
      maps:\t\tdownload the normalized FDG maps
      tests:\t\tcollect all automatic tests outcomes from `PetSessionValidator`
      mri:\t\tcreates an Excel table with details from associated MRI sessions
+     aging:\t\tcreates an Excel table with the aging composite ROI
 
     Usage:
      bx fdg <subcommand> <resource_id>
 
     Reference:
     - Landau et al., Ann Neurol., 2012
     """
     nargs = 2
-    subcommands = ['tests', 'landau', 'maps', 'mri']
+    subcommands = ['tests', 'landau', 'maps', 'mri', 'aging']
     resource_name = 'FDG_QUANTIFICATION'
     url = 'https://gitlab.com/bbrc/xnat/xnat-pipelines/-/tree/master/pet'
 
     def __init__(self, *args, **kwargs):
         super(FdgCommand, self).__init__(*args, **kwargs)
 
     def parse(self):
@@ -51,15 +52,19 @@
             fp = get_filepath(self.resource_name, debug=debug)
             self.run_id(id, download_pet, resource_name=self.resource_name,
                         filename=fp, destdir=self.destdir,
                         subcommand=subcommand)
         elif subcommand == 'mri':
             df = self.run_id(id, get_mri_table, validator=validator_name)
             self.to_excel(df)
-
+        elif subcommand == 'aging':
+            df = self.run_id(id, dl.measurements,
+                             resource_name=self.resource_name,
+                             subfunc=subcommand, max_rows=10)
+            self.to_excel(df)
 
 class FtmCommand(Command):
     """18F-flutemetamol PET imaging data
 
     Available subcommands:
      centiloids:\tcreates an Excel table with centiloid scales
      maps:\t\tdownload the normalized FTM maps
```

### Comparing `bbrc-bx-0.5/bx/qsmxt.py` & `bbrc-bx-0.5.1/bx/qsmxt.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,17 +38,16 @@
         if subcommand == 'stats':
             sf = 'qsmxt_%s' % subcommand
             df = self.run_id(id, dl.measurements, subfunc=sf,
                              resource_name='QSMXT', max_rows=10)
             self.to_excel(df)
 
         elif subcommand == 'maps':
-            debug = bool(os.environ.get('CI_TEST', None))
             self.run_id(id, download_qsm, resource_name=self.resource_name,
-                        destdir=self.destdir, subcommand=subcommand)
+                        destdir=self.destdir)
 
         elif subcommand in ['files', 'report']:
             self.run_id(id, dl.download, resource_name=self.resource_name,
                         validator=self.validator, destdir=self.destdir,
                         subcommand=subcommand)
 
         elif subcommand == 'tests':
@@ -57,15 +56,15 @@
             from bx import validation as val
             df = self.run_id(id, val.validation_scores,
                              validator=self.validator,
                              version=version, max_rows=25)
             self.to_excel(df)
 
 
-def download_qsm(x, experiments, resource_name, destdir, subcommand):
+def download_qsm(x, experiments, resource_name, destdir):
 
     import os.path as op
     from tqdm import tqdm
     from pyxnat.core.errors import DataError
 
     filename = 'qsm/*_part-phase_MEGRE_scaled_qsm-filled_000_average.nii.gz'
 
@@ -76,8 +75,8 @@
         files = r.files(filename)
 
         for f in files:
             fn = op.basename(f.label())
             try:
                 f.get(op.join(destdir, fn))
             except DataError as exc:
-                log.error('Failed for %s. Skipping it. (%s)' % (e, exc))
+                log.error('Failed for %s. Skipping it. (%s)' % (e['ID'], exc))
```

### Comparing `bbrc-bx-0.5/bx/scandates.py` & `bbrc-bx-0.5.1/bx/scandates.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/signature.py` & `bbrc-bx-0.5.1/bx/signature.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/spm12.py` & `bbrc-bx-0.5.1/bx/spm12.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/validation.py` & `bbrc-bx-0.5.1/bx/validation.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/bx/xnat.py` & `bbrc-bx-0.5.1/bx/xnat.py`

 * *Files identical despite different names*

### Comparing `bbrc-bx-0.5/setup.py` & `bbrc-bx-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,12 +40,12 @@
     author_email='goperto@barcelonabeta.org',
     url='https://gitlab.com/bbrc/xnat/bx',
     download_url=download_url,
     classifiers=['Intended Audience :: Science/Research',
                  'Intended Audience :: Developers',
                  'Topic :: Scientific/Engineering',
                  'Operating System :: Unix',
-                 'Programming Language :: Python :: 3.7',
-                 'Programming Language :: Python :: 3.8'],
+                 'Programming Language :: Python :: 3.8',
+                 'Programming Language :: Python :: 3.9'],
     include_package_data=True
 
 )
```

