# Comparing `tmp/PyGeopack-1.2.1.tar.gz` & `tmp/PyGeopack-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyGeopack-1.2.1.tar", last modified: Sun Jul  9 22:46:46 2023, max compression
+gzip compressed data, was "PyGeopack-1.2.2.tar", last modified: Mon Jul 10 22:51:19 2023, max compression
```

## Comparing `PyGeopack-1.2.1.tar` & `PyGeopack-1.2.2.tar`

### file list

```diff
@@ -1,327 +1,327 @@
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-09 22:46:46.154364 PyGeopack-1.2.1/
--rw-rw-r--   0 matt      (1000) matt      (1000)    35149 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/LICENSE
--rw-rw-r--   0 matt      (1000) matt      (1000)       45 2023-07-08 22:23:20.000000 PyGeopack-1.2.1/MANIFEST.in
--rw-rw-r--   0 matt      (1000) matt      (1000)    27842 2023-07-09 22:46:46.154364 PyGeopack-1.2.1/PKG-INFO
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-09 22:46:46.138364 PyGeopack-1.2.1/PyGeopack/
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-09 22:46:46.142364 PyGeopack-1.2.1/PyGeopack/Coords/
--rw-rw-r--   0 matt      (1000) matt      (1000)     1996 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Coords/ConvCoords.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1256 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Coords/GEItoGEO.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1258 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Coords/GEItoGSE.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1258 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Coords/GEItoGSM.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1258 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Coords/GEItoMAG.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1254 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Coords/GEItoSM.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1258 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Coords/GEOtoGEI.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1259 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Coords/GEOtoGSE.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1258 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Coords/GEOtoGSM.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2338 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Coords/GEOtoMAG.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1254 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Coords/GEOtoSM.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1258 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Coords/GSEtoGEI.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1258 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Coords/GSEtoGEO.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1262 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Coords/GSEtoGSM.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1267 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Coords/GSEtoMAG.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1254 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Coords/GSEtoSM.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1258 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Coords/GSMtoGEI.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1258 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Coords/GSMtoGEO.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1259 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Coords/GSMtoGSE.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1258 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Coords/GSMtoMAG.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1259 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Coords/GSMtoSM.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1263 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Coords/MAGtoGEI.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2354 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Coords/MAGtoGEO.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1257 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Coords/MAGtoGSE.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1257 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Coords/MAGtoGSM.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1253 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Coords/MAGtoSM.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1009 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Coords/MLONtoMLT.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1005 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Coords/MLTtoMLON.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1254 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Coords/SMtoGEI.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1254 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Coords/SMtoGEO.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1254 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Coords/SMtoGSE.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1254 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Coords/SMtoGSM.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1254 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Coords/SMtoMAG.py
--rw-rw-r--   0 matt      (1000) matt      (1000)    17085 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Coords/_CFunctions.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1034 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Coords/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)       86 2023-07-08 22:23:20.000000 PyGeopack-1.2.1/PyGeopack/Globals.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     4060 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/ModelField.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-09 22:46:46.142364 PyGeopack-1.2.1/PyGeopack/Params/
--rw-rw-r--   0 matt      (1000) matt      (1000)      149 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Params/FreeParams.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1232 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Params/GetDipoleTilt.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3014 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Params/GetModelParams.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      809 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Params/ReadTSData.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1313 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Params/UpdateParameters.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     5749 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Params/_CFunctions.py
--rw-rw-r--   0 matt      (1000) matt      (1000)    12461 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Params/_CalculateParameters.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1188 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Params/_DownloadTS05Data.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      202 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Params/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1676 2023-07-08 22:23:20.000000 PyGeopack-1.2.1/PyGeopack/ShueMP.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-09 22:46:46.142364 PyGeopack-1.2.1/PyGeopack/Test/
--rw-rw-r--   0 matt      (1000) matt      (1000)     6495 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Test/PlotTraces.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     4289 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Test/TestHarmonic.py
--rw-rw-r--   0 matt      (1000) matt      (1000)       86 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Test/__init__.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-09 22:46:46.142364 PyGeopack-1.2.1/PyGeopack/Tools/
--rw-rw-r--   0 matt      (1000) matt      (1000)      319 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Tools/GetLegendHandLab.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2795 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Tools/PlotPlanet.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2368 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Tools/T89CurrentSheet.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      123 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/Tools/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)    25228 2023-07-08 22:23:20.000000 PyGeopack-1.2.1/PyGeopack/TraceField.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3307 2023-07-08 22:23:20.000000 PyGeopack-1.2.1/PyGeopack/_CFunctions.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1982 2023-07-08 22:23:20.000000 PyGeopack-1.2.1/PyGeopack/_CheckFirstImport.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-09 22:46:46.138364 PyGeopack-1.2.1/PyGeopack/__data/
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-09 22:46:46.142364 PyGeopack-1.2.1/PyGeopack/__data/geopack/
--rw-rw-r--   0 matt      (1000) matt      (1000)     6148 2023-04-27 16:08:43.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/.DS_Store
--rw-rw-r--   0 matt      (1000) matt      (1000)       55 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/.git
--rw-rw-r--   0 matt      (1000) matt      (1000)      270 2023-07-07 22:53:29.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/.gitignore
--rw-rw-r--   0 matt      (1000) matt      (1000)      193 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/.gitmodules
--rw-rw-r--   0 matt      (1000) matt      (1000)    35149 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/LICENSE
--rw-rw-r--   0 matt      (1000) matt      (1000)       26 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/README.md
--rw-rw-r--   0 matt      (1000) matt      (1000)       39 2023-07-07 22:53:29.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/clean.bat
--rw-rw-r--   0 matt      (1000) matt      (1000)      273 2023-04-27 16:08:43.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/compile.bat
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-09 22:46:46.138364 PyGeopack-1.2.1/PyGeopack/__data/geopack/doc/
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-09 22:46:46.142364 PyGeopack-1.2.1/PyGeopack/__data/geopack/doc/equations/
--rw-rw-r--   0 matt      (1000) matt      (1000)    42484 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/doc/equations/agufull08.bst
--rw-rw-r--   0 matt      (1000) matt      (1000)      241 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/doc/equations/equations.aux
--rw-rw-r--   0 matt      (1000) matt      (1000)      277 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/doc/equations/equations.bbl
--rw-rw-r--   0 matt      (1000) matt      (1000)     1024 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/doc/equations/equations.blg
--rw-rw-r--   0 matt      (1000) matt      (1000)     8018 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/doc/equations/equations.log
--rw-rw-r--   0 matt      (1000) matt      (1000)   101849 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/doc/equations/equations.pdf
--rw-rw-r--   0 matt      (1000) matt      (1000)    17156 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/doc/equations/equations.synctex.gz
--rw-rw-r--   0 matt      (1000) matt      (1000)     3123 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/doc/equations/equations.tex
--rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/doc/equations/ref.bib
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-09 22:46:46.142364 PyGeopack-1.2.1/PyGeopack/__data/geopack/include/
--rw-rw-r--   0 matt      (1000) matt      (1000)    48264 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/include/geopack.h
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-09 22:46:46.138364 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-09 22:46:46.142364 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/
--rw-rw-r--   0 matt      (1000) matt      (1000)       82 2023-04-27 13:15:08.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/.git
--rw-rw-r--   0 matt      (1000) matt      (1000)      270 2023-07-07 22:53:44.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/.gitignore
--rw-rw-r--   0 matt      (1000) matt      (1000)     1070 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/LICENSE
--rw-rw-r--   0 matt      (1000) matt      (1000)     3277 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/README.md
--rw-rw-r--   0 matt      (1000) matt      (1000)       49 2023-07-07 22:53:44.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/clean.bat
--rw-rw-r--   0 matt      (1000) matt      (1000)       45 2023-04-27 16:08:43.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/compile.bat
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-09 22:46:46.142364 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/include/
--rw-rw-r--   0 matt      (1000) matt      (1000)    17194 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/include/datetime.h
--rw-rw-r--   0 matt      (1000) matt      (1000)     1138 2023-07-07 22:53:44.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/makefile
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-09 22:46:46.146364 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/
--rw-rw-r--   0 matt      (1000) matt      (1000)     1070 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/BubbleSort.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      758 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/BubbleSort.h
--rw-rw-r--   0 matt      (1000) matt      (1000)     6290 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/ContUT.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)     2294 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/ContUT.h
--rw-rw-r--   0 matt      (1000) matt      (1000)      942 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/DateDifference.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      690 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/DateDifference.h
--rw-rw-r--   0 matt      (1000) matt      (1000)     1262 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/DateJoin.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)     1203 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/DateJoin.h
--rw-rw-r--   0 matt      (1000) matt      (1000)     1309 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/DateSplit.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)     1227 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/DateSplit.h
--rw-rw-r--   0 matt      (1000) matt      (1000)     1942 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/DayNo.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)     1174 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/DayNo.h
--rw-rw-r--   0 matt      (1000) matt      (1000)     1034 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/JulDay.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      654 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/JulDay.h
--rw-rw-r--   0 matt      (1000) matt      (1000)     1335 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/JulDaytoDate.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      681 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/JulDaytoDate.h
--rw-rw-r--   0 matt      (1000) matt      (1000)      636 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/LeapYear.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      560 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/LeapYear.h
--rw-rw-r--   0 matt      (1000) matt      (1000)     1256 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/MidTime.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      809 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/MidTime.h
--rw-rw-r--   0 matt      (1000) matt      (1000)      818 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/MinusDay.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      576 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/MinusDay.h
--rw-rw-r--   0 matt      (1000) matt      (1000)     1097 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/NearestTimeIndex.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      876 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/NearestTimeIndex.h
--rw-rw-r--   0 matt      (1000) matt      (1000)      700 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/PlusDay.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      568 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/PlusDay.h
--rw-rw-r--   0 matt      (1000) matt      (1000)      851 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/TimeDifference.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      772 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/TimeDifference.h
--rw-rw-r--   0 matt      (1000) matt      (1000)      912 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/Unique.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      638 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/Unique.h
--rw-rw-r--   0 matt      (1000) matt      (1000)     5735 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/UnixTime.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)     2300 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/UnixTime.h
--rw-rw-r--   0 matt      (1000) matt      (1000)      690 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/WhereEq.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      752 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/WhereEq.h
--rw-rw-r--   0 matt      (1000) matt      (1000)     1238 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/WithinTimeRange.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      968 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/WithinTimeRange.h
--rw-rw-r--   0 matt      (1000) matt      (1000)      118 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/compile.bat
--rw-rw-r--   0 matt      (1000) matt      (1000)     1192 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/compileobj.bat
--rw-rw-r--   0 matt      (1000) matt      (1000)     1695 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/hhmm.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)     1351 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/hhmm.h
--rw-rw-r--   0 matt      (1000) matt      (1000)      734 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/makefile
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-09 22:46:46.146364 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/test/
--rw-rw-r--   0 matt      (1000) matt      (1000)      443 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/test/makefile
--rw-rw-r--   0 matt      (1000) matt      (1000)      258 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/test/test.bat
--rw-rw-r--   0 matt      (1000) matt      (1000)     6611 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/test/testc.c
--rw-rw-r--   0 matt      (1000) matt      (1000)     7893 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/test/testcc.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)       27 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/test.bat
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-09 22:46:46.146364 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/libspline/
--rw-rw-r--   0 matt      (1000) matt      (1000)       83 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/libspline/.git
--rw-rw-r--   0 matt      (1000) matt      (1000)      270 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/libspline/.gitignore
--rw-rw-r--   0 matt      (1000) matt      (1000)     1070 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/libspline/LICENSE
--rw-rw-r--   0 matt      (1000) matt      (1000)     2122 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/libspline/README.md
--rw-rw-r--   0 matt      (1000) matt      (1000)        5 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/libspline/VERSION
--rw-rw-r--   0 matt      (1000) matt      (1000)       47 2023-07-07 22:53:44.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/libspline/clean.bat
--rw-rw-r--   0 matt      (1000) matt      (1000)       44 2023-04-27 16:08:43.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/libspline/compile.bat
--rw-rw-r--   0 matt      (1000) matt      (1000)     2815 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/libspline/generateheader.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-09 22:46:46.146364 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/libspline/include/
--rw-rw-r--   0 matt      (1000) matt      (1000)      612 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/libspline/include/spline.h
--rw-rw-r--   0 matt      (1000) matt      (1000)      139 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/libspline/install.bat
--rw-rw-r--   0 matt      (1000) matt      (1000)     1442 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/libspline/makefile
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-09 22:46:46.146364 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/libspline/src/
--rw-rw-r--   0 matt      (1000) matt      (1000)      127 2023-04-27 16:08:43.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/libspline/src/compile.bat
--rw-rw-r--   0 matt      (1000) matt      (1000)      165 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/libspline/src/compileobj.bat
--rw-rw-r--   0 matt      (1000) matt      (1000)      238 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/libspline/src/libspline.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      213 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/libspline/src/libspline.h
--rw-rw-r--   0 matt      (1000) matt      (1000)      682 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/libspline/src/makefile
--rw-rw-r--   0 matt      (1000) matt      (1000)     2856 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/libspline/src/spline.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      345 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/libspline/src/spline.h
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-09 22:46:46.146364 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/libspline/test/
--rw-rw-r--   0 matt      (1000) matt      (1000)      714 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/libspline/test/cpptest.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      665 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/libspline/test/ctest.c
--rw-rw-r--   0 matt      (1000) matt      (1000)      543 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/libspline/test/makefile
--rw-rw-r--   0 matt      (1000) matt      (1000)    37488 2023-07-07 22:53:44.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/libspline/test/testspline.png
--rw-rw-r--   0 matt      (1000) matt      (1000)     2881 2023-04-27 13:15:09.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/libspline/test/testspline.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     1413 2023-07-07 22:53:29.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/makefile
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-09 22:46:46.146364 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/
--rw-rw-r--   0 matt      (1000) matt      (1000)     8196 2023-04-27 16:08:43.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/.DS_Store
--rw-rw-r--   0 matt      (1000) matt      (1000)    71079 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/ConvCoords.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)    38295 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/ConvCoords.h
--rw-rw-r--   0 matt      (1000) matt      (1000)      478 2023-07-06 20:58:23.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/compile.bat
--rw-rw-r--   0 matt      (1000) matt      (1000)      145 2023-04-27 16:08:43.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/compileobj.bat
--rw-rw-r--   0 matt      (1000) matt      (1000)      213 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/dummyfunc.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      231 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/dummyfunc.h
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-09 22:46:46.150364 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/fortran/
--rw-rw-r--   0 matt      (1000) matt      (1000)    85665 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/fortran/Geopack-2008_mkj_dp.f
--rw-rw-r--   0 matt      (1000) matt      (1000)    86704 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/fortran/T01_01.f
--rwxrwxr-x   0 matt      (1000) matt      (1000)    15845 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/fortran/T89c.f
--rw-rw-r--   0 matt      (1000) matt      (1000)    93009 2023-07-09 21:12:38.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/fortran/T96.f
--rw-rw-r--   0 matt      (1000) matt      (1000)    86349 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/fortran/TS04c.f
--rw-rw-r--   0 matt      (1000) matt      (1000)     7715 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/fortran/bessel.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)     3579 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/fortran/bessel.h
--rw-rw-r--   0 matt      (1000) matt      (1000)      517 2023-07-09 21:12:38.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/fortran/compile.bat
--rw-rw-r--   0 matt      (1000) matt      (1000)     2694 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/fortran/geopack.h
--rw-rw-r--   0 matt      (1000) matt      (1000)      574 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/fortran/makefile
--rw-rw-r--   0 matt      (1000) matt      (1000)    13276 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/fortran/t89.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)     1527 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/fortran/t89.h
--rw-rw-r--   0 matt      (1000) matt      (1000)    18547 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/fortran/t89params.ods
--rw-rw-r--   0 matt      (1000) matt      (1000)     4252 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/fortran/t96.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)     5185 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/fortran/wparams.f95
--rw-rw-r--   0 matt      (1000) matt      (1000)      745 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/getdipoletilt.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      420 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/getdipoletilt.h
--rw-rw-r--   0 matt      (1000) matt      (1000)     1632 2023-04-28 08:59:56.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/makefile
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-09 22:46:46.150364 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/matrix/
--rw-rw-r--   0 matt      (1000) matt      (1000)      415 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/matrix/compile.bat
--rw-rw-r--   0 matt      (1000) matt      (1000)      148 2023-04-27 16:08:43.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/matrix/compileobj.bat
--rw-rw-r--   0 matt      (1000) matt      (1000)      160 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/matrix/identity.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      139 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/matrix/identity.h
--rw-rw-r--   0 matt      (1000) matt      (1000)      908 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/matrix/libmatrix.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      394 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/matrix/libmatrix.h
--rwxrwxr-x   0 matt      (1000) matt      (1000)   292104 2023-04-27 16:08:43.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/matrix/libmatrix.so
--rw-rw-r--   0 matt      (1000) matt      (1000)     1040 2023-04-27 16:08:43.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/matrix/makefile
--rw-rw-r--   0 matt      (1000) matt      (1000)    11820 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/matrix/matrix.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)     2001 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/matrix/matrix.h
--rw-rw-r--   0 matt      (1000) matt      (1000)     4285 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/matrix/matrixarray.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)     1036 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/matrix/matrixarray.h
--rw-rw-r--   0 matt      (1000) matt      (1000)    20389 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/matrix/matrixmath.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)     4198 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/matrix/matrixmath.h
--rw-rw-r--   0 matt      (1000) matt      (1000)     2161 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/matrix/rotmatrix.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)     1407 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/matrix/rotmatrix.h
--rw-rw-r--   0 matt      (1000) matt      (1000)     2392 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/matrix/testmatrix.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     3480 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/modelfield.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)     1770 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/modelfield.h
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-09 22:46:46.150364 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/modelparams/
--rw-rw-r--   0 matt      (1000) matt      (1000)     1242 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/modelparams/calculateg.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      268 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/modelparams/calculateg.h
--rw-rw-r--   0 matt      (1000) matt      (1000)     7507 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/modelparams/calculatew.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      458 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/modelparams/calculatew.h
--rw-rw-r--   0 matt      (1000) matt      (1000)      385 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/modelparams/checkv.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      249 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/modelparams/checkv.h
--rw-rw-r--   0 matt      (1000) matt      (1000)      367 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/modelparams/compile.bat
--rw-rw-r--   0 matt      (1000) matt      (1000)      148 2023-04-27 16:08:43.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/modelparams/compileobj.bat
--rw-rw-r--   0 matt      (1000) matt      (1000)     1103 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/modelparams/fillinkp.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      249 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/modelparams/fillinkp.h
--rw-rw-r--   0 matt      (1000) matt      (1000)      511 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/modelparams/makefile
--rw-rw-r--   0 matt      (1000) matt      (1000)     6281 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/modelparams/modelparams.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)     1922 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/modelparams/modelparams.h
--rw-rw-r--   0 matt      (1000) matt      (1000)    12057 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/modelparams/tsygdata.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)     2203 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/modelparams/tsygdata.h
--rw-rw-r--   0 matt      (1000) matt      (1000)     1081 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/recalc.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      331 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/recalc.h
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-09 22:46:46.150364 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tools/
--rw-rw-r--   0 matt      (1000) matt      (1000)     1203 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tools/BubbleArgSort.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      574 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tools/BubbleArgSort.h
--rw-rw-r--   0 matt      (1000) matt      (1000)     2243 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tools/BubbleSort.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)     1353 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tools/BubbleSort.h
--rw-rw-r--   0 matt      (1000) matt      (1000)      250 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tools/argmax.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      144 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tools/argmax.h
--rw-rw-r--   0 matt      (1000) matt      (1000)      433 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tools/carttospherical.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      223 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tools/carttospherical.h
--rw-rw-r--   0 matt      (1000) matt      (1000)      339 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tools/compile.bat
--rw-rw-r--   0 matt      (1000) matt      (1000)      148 2023-04-27 16:08:43.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tools/compileobj.bat
--rw-rw-r--   0 matt      (1000) matt      (1000)      165 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tools/linterp.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      169 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tools/linterp.h
--rw-rw-r--   0 matt      (1000) matt      (1000)      488 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tools/makefile
--rw-rw-r--   0 matt      (1000) matt      (1000)      193 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tools/reverseelements.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      147 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tools/reverseelements.h
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-09 22:46:46.154364 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/
--rw-rw-r--   0 matt      (1000) matt      (1000)     2755 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/calculatehalpha.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      810 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/calculatehalpha.h
--rw-rw-r--   0 matt      (1000) matt      (1000)      949 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/compile.bat
--rw-rw-r--   0 matt      (1000) matt      (1000)      148 2023-04-27 16:08:43.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/compileobj.bat
--rw-rw-r--   0 matt      (1000) matt      (1000)     2143 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/converttracecoords.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      543 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/converttracecoords.h
--rw-rw-r--   0 matt      (1000) matt      (1000)      490 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/fieldlinedist.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      192 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/fieldlinedist.h
--rw-rw-r--   0 matt      (1000) matt      (1000)      718 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/fieldlinemidpoint.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      255 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/fieldlinemidpoint.h
--rw-rw-r--   0 matt      (1000) matt      (1000)      381 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/fieldliner.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      183 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/fieldliner.h
--rw-rw-r--   0 matt      (1000) matt      (1000)      352 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/fieldlinernorm.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      176 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/fieldlinernorm.h
--rw-rw-r--   0 matt      (1000) matt      (1000)     3099 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/getmagequatorfp.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      577 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/getmagequatorfp.h
--rw-rw-r--   0 matt      (1000) matt      (1000)     8254 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/interptraceclosestpos.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)     1299 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/interptraceclosestpos.h
--rw-rw-r--   0 matt      (1000) matt      (1000)     1145 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/latlonlt.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      400 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/latlonlt.h
--rw-rw-r--   0 matt      (1000) matt      (1000)     1039 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/makefile
--rw-rw-r--   0 matt      (1000) matt      (1000)    23270 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/trace.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)     5486 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/trace.h
--rw-rw-r--   0 matt      (1000) matt      (1000)     4920 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/traceclosestpos.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)     1428 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/traceclosestpos.h
--rw-rw-r--   0 matt      (1000) matt      (1000)     5011 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/tracefield.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)     2796 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/tracefield.h
--rw-rw-r--   0 matt      (1000) matt      (1000)     1561 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/tracefieldline.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      494 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/tracefieldline.h
--rw-rw-r--   0 matt      (1000) matt      (1000)     3859 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/tracefootprints.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      812 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/tracefootprints.h
--rw-rw-r--   0 matt      (1000) matt      (1000)      953 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/tracerotationmatrices.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      291 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/tracerotationmatrices.h
--rw-rw-r--   0 matt      (1000) matt      (1000)      539 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/withinmp.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      196 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/src/withinmp.h
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-09 22:46:46.154364 PyGeopack-1.2.1/PyGeopack/__data/geopack/test/
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-09 22:46:46.154364 PyGeopack-1.2.1/PyGeopack/__data/geopack/test/fortran/
--rwxrwxr-x   0 matt      (1000) matt      (1000)    15356 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/test/fortran/T89c.f
--rw-rw-r--   0 matt      (1000) matt      (1000)      859 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/test/fortran/makefile
--rw-rw-r--   0 matt      (1000) matt      (1000)     1047 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/test/fortran/testfortran.cc
--rw-rw-r--   0 matt      (1000) matt      (1000)      705 2023-04-27 16:08:43.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/test/makefile
--rw-rw-r--   0 matt      (1000) matt      (1000)     2112 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/test/test.c
--rw-rw-r--   0 matt      (1000) matt      (1000)     1489 2023-04-27 13:13:19.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/test/test.cc
--rwxrwxr-x   0 matt      (1000) matt      (1000)    21104 2023-07-06 20:58:23.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/test/testc
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-09 22:46:46.138364 PyGeopack-1.2.1/PyGeopack/__data/geopack/test/testc.dSYM/
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-09 22:46:46.154364 PyGeopack-1.2.1/PyGeopack/__data/geopack/test/testc.dSYM/Contents/
--rw-rw-r--   0 matt      (1000) matt      (1000)      634 2023-04-27 16:08:43.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/test/testc.dSYM/Contents/Info.plist
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-09 22:46:46.138364 PyGeopack-1.2.1/PyGeopack/__data/geopack/test/testc.dSYM/Contents/Resources/
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-09 22:46:46.154364 PyGeopack-1.2.1/PyGeopack/__data/geopack/test/testc.dSYM/Contents/Resources/DWARF/
--rw-rw-r--   0 matt      (1000) matt      (1000)    12741 2023-04-27 16:08:43.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/test/testc.dSYM/Contents/Resources/DWARF/testc
--rwxrwxr-x   0 matt      (1000) matt      (1000)    30672 2023-07-06 20:58:23.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/test/testcc
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-09 22:46:46.138364 PyGeopack-1.2.1/PyGeopack/__data/geopack/test/testcc.dSYM/
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-09 22:46:46.154364 PyGeopack-1.2.1/PyGeopack/__data/geopack/test/testcc.dSYM/Contents/
--rw-rw-r--   0 matt      (1000) matt      (1000)      635 2023-04-27 16:08:43.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/test/testcc.dSYM/Contents/Info.plist
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-09 22:46:46.138364 PyGeopack-1.2.1/PyGeopack/__data/geopack/test/testcc.dSYM/Contents/Resources/
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-09 22:46:46.154364 PyGeopack-1.2.1/PyGeopack/__data/geopack/test/testcc.dSYM/Contents/Resources/DWARF/
--rw-rw-r--   0 matt      (1000) matt      (1000)    16387 2023-04-27 16:08:43.000000 PyGeopack-1.2.1/PyGeopack/__data/geopack/test/testcc.dSYM/Contents/Resources/DWARF/testcc
--rw-rw-r--   0 matt      (1000) matt      (1000)       98 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/__del__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)      345 2023-07-09 21:12:53.000000 PyGeopack-1.2.1/PyGeopack/__init__.py
--rw-rw-r--   0 matt      (1000) matt      (1000)     2737 2023-04-27 13:12:39.000000 PyGeopack-1.2.1/PyGeopack/ct.py
-drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-09 22:46:46.138364 PyGeopack-1.2.1/PyGeopack.egg-info/
--rw-rw-r--   0 matt      (1000) matt      (1000)    27842 2023-07-09 22:46:46.000000 PyGeopack-1.2.1/PyGeopack.egg-info/PKG-INFO
--rw-rw-r--   0 matt      (1000) matt      (1000)    12965 2023-07-09 22:46:46.000000 PyGeopack-1.2.1/PyGeopack.egg-info/SOURCES.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)        1 2023-07-09 22:46:46.000000 PyGeopack-1.2.1/PyGeopack.egg-info/dependency_links.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       83 2023-07-09 22:46:46.000000 PyGeopack-1.2.1/PyGeopack.egg-info/requires.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)       10 2023-07-09 22:46:46.000000 PyGeopack-1.2.1/PyGeopack.egg-info/top_level.txt
--rw-rw-r--   0 matt      (1000) matt      (1000)    27376 2023-07-08 22:23:20.000000 PyGeopack-1.2.1/README.md
--rw-rw-r--   0 matt      (1000) matt      (1000)       38 2023-07-09 22:46:46.154364 PyGeopack-1.2.1/setup.cfg
--rw-rw-r--   0 matt      (1000) matt      (1000)     2075 2023-07-08 22:23:20.000000 PyGeopack-1.2.1/setup.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-10 22:51:19.678129 PyGeopack-1.2.2/
+-rw-rw-r--   0 matt      (1000) matt      (1000)    35149 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/LICENSE
+-rw-rw-r--   0 matt      (1000) matt      (1000)       45 2023-07-08 22:23:20.000000 PyGeopack-1.2.2/MANIFEST.in
+-rw-rw-r--   0 matt      (1000) matt      (1000)    28455 2023-07-10 22:51:19.678129 PyGeopack-1.2.2/PKG-INFO
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-10 22:51:19.666128 PyGeopack-1.2.2/PyGeopack/
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-10 22:51:19.666128 PyGeopack-1.2.2/PyGeopack/Coords/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1996 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Coords/ConvCoords.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1256 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Coords/GEItoGEO.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1258 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Coords/GEItoGSE.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1258 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Coords/GEItoGSM.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1258 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Coords/GEItoMAG.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1254 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Coords/GEItoSM.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1258 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Coords/GEOtoGEI.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1259 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Coords/GEOtoGSE.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1258 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Coords/GEOtoGSM.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2338 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Coords/GEOtoMAG.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1254 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Coords/GEOtoSM.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1258 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Coords/GSEtoGEI.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1258 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Coords/GSEtoGEO.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1262 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Coords/GSEtoGSM.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1267 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Coords/GSEtoMAG.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1254 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Coords/GSEtoSM.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1258 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Coords/GSMtoGEI.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1258 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Coords/GSMtoGEO.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1259 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Coords/GSMtoGSE.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1258 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Coords/GSMtoMAG.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1259 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Coords/GSMtoSM.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1263 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Coords/MAGtoGEI.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2354 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Coords/MAGtoGEO.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1257 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Coords/MAGtoGSE.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1257 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Coords/MAGtoGSM.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1253 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Coords/MAGtoSM.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1009 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Coords/MLONtoMLT.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1005 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Coords/MLTtoMLON.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1254 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Coords/SMtoGEI.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1254 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Coords/SMtoGEO.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1254 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Coords/SMtoGSE.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1254 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Coords/SMtoGSM.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1254 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Coords/SMtoMAG.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)    17085 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Coords/_CFunctions.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1034 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Coords/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       86 2023-07-08 22:23:20.000000 PyGeopack-1.2.2/PyGeopack/Globals.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4060 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/ModelField.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-10 22:51:19.666128 PyGeopack-1.2.2/PyGeopack/Params/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      149 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Params/FreeParams.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1232 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Params/GetDipoleTilt.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3014 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Params/GetModelParams.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      809 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Params/ReadTSData.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1313 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Params/UpdateParameters.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     5749 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Params/_CFunctions.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)    12461 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Params/_CalculateParameters.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1188 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Params/_DownloadTS05Data.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      202 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Params/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1676 2023-07-08 22:23:20.000000 PyGeopack-1.2.2/PyGeopack/ShueMP.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-10 22:51:19.666128 PyGeopack-1.2.2/PyGeopack/Test/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     6495 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Test/PlotTraces.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4289 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Test/TestHarmonic.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)       86 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Test/__init__.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-10 22:51:19.666128 PyGeopack-1.2.2/PyGeopack/Tools/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      319 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Tools/GetLegendHandLab.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2795 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Tools/PlotPlanet.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2368 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Tools/T89CurrentSheet.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      123 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/Tools/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)    25228 2023-07-08 22:23:20.000000 PyGeopack-1.2.2/PyGeopack/TraceField.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3438 2023-07-10 22:31:54.000000 PyGeopack-1.2.2/PyGeopack/_CFunctions.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2576 2023-07-10 22:30:13.000000 PyGeopack-1.2.2/PyGeopack/_CheckFirstImport.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-10 22:51:19.658129 PyGeopack-1.2.2/PyGeopack/__data/
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-10 22:51:19.666128 PyGeopack-1.2.2/PyGeopack/__data/geopack/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     6148 2023-04-27 16:08:43.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/.DS_Store
+-rw-rw-r--   0 matt      (1000) matt      (1000)       55 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/.git
+-rw-rw-r--   0 matt      (1000) matt      (1000)      270 2023-07-07 22:53:29.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/.gitignore
+-rw-rw-r--   0 matt      (1000) matt      (1000)      193 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/.gitmodules
+-rw-rw-r--   0 matt      (1000) matt      (1000)    35149 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/LICENSE
+-rw-rw-r--   0 matt      (1000) matt      (1000)       26 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/README.md
+-rw-rw-r--   0 matt      (1000) matt      (1000)       39 2023-07-07 22:53:29.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/clean.bat
+-rw-rw-r--   0 matt      (1000) matt      (1000)      273 2023-04-27 16:08:43.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/compile.bat
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-10 22:51:19.658129 PyGeopack-1.2.2/PyGeopack/__data/geopack/doc/
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-10 22:51:19.670129 PyGeopack-1.2.2/PyGeopack/__data/geopack/doc/equations/
+-rw-rw-r--   0 matt      (1000) matt      (1000)    42484 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/doc/equations/agufull08.bst
+-rw-rw-r--   0 matt      (1000) matt      (1000)      241 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/doc/equations/equations.aux
+-rw-rw-r--   0 matt      (1000) matt      (1000)      277 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/doc/equations/equations.bbl
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1024 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/doc/equations/equations.blg
+-rw-rw-r--   0 matt      (1000) matt      (1000)     8018 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/doc/equations/equations.log
+-rw-rw-r--   0 matt      (1000) matt      (1000)   101849 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/doc/equations/equations.pdf
+-rw-rw-r--   0 matt      (1000) matt      (1000)    17156 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/doc/equations/equations.synctex.gz
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3123 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/doc/equations/equations.tex
+-rw-rw-r--   0 matt      (1000) matt      (1000)        0 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/doc/equations/ref.bib
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-10 22:51:19.670129 PyGeopack-1.2.2/PyGeopack/__data/geopack/include/
+-rw-rw-r--   0 matt      (1000) matt      (1000)    48264 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/include/geopack.h
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-10 22:51:19.658129 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-10 22:51:19.670129 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/
+-rw-rw-r--   0 matt      (1000) matt      (1000)       82 2023-04-27 13:15:08.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/.git
+-rw-rw-r--   0 matt      (1000) matt      (1000)      270 2023-07-07 22:53:44.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/.gitignore
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1070 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/LICENSE
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3277 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/README.md
+-rw-rw-r--   0 matt      (1000) matt      (1000)       49 2023-07-07 22:53:44.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/clean.bat
+-rw-rw-r--   0 matt      (1000) matt      (1000)       45 2023-04-27 16:08:43.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/compile.bat
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-10 22:51:19.670129 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/include/
+-rw-rw-r--   0 matt      (1000) matt      (1000)    17194 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/include/datetime.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1138 2023-07-07 22:53:44.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/makefile
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-10 22:51:19.670129 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1070 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/BubbleSort.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      758 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/BubbleSort.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)     6290 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/ContUT.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2294 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/ContUT.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)      942 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/DateDifference.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      690 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/DateDifference.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1262 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/DateJoin.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1203 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/DateJoin.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1309 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/DateSplit.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1227 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/DateSplit.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1942 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/DayNo.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1174 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/DayNo.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1034 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/JulDay.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      654 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/JulDay.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1335 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/JulDaytoDate.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      681 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/JulDaytoDate.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)      636 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/LeapYear.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      560 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/LeapYear.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1256 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/MidTime.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      809 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/MidTime.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)      818 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/MinusDay.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      576 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/MinusDay.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1097 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/NearestTimeIndex.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      876 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/NearestTimeIndex.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)      700 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/PlusDay.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      568 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/PlusDay.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)      851 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/TimeDifference.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      772 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/TimeDifference.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)      912 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/Unique.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      638 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/Unique.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)     5735 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/UnixTime.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2300 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/UnixTime.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)      690 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/WhereEq.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      752 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/WhereEq.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1238 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/WithinTimeRange.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      968 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/WithinTimeRange.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)      118 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/compile.bat
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1192 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/compileobj.bat
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1695 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/hhmm.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1351 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/hhmm.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)      734 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/makefile
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-10 22:51:19.670129 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/test/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      443 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/test/makefile
+-rw-rw-r--   0 matt      (1000) matt      (1000)      258 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/test/test.bat
+-rw-rw-r--   0 matt      (1000) matt      (1000)     6611 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/test/testc.c
+-rw-rw-r--   0 matt      (1000) matt      (1000)     7893 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/test/testcc.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)       27 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/test.bat
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-10 22:51:19.670129 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/libspline/
+-rw-rw-r--   0 matt      (1000) matt      (1000)       83 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/libspline/.git
+-rw-rw-r--   0 matt      (1000) matt      (1000)      270 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/libspline/.gitignore
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1070 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/libspline/LICENSE
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2122 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/libspline/README.md
+-rw-rw-r--   0 matt      (1000) matt      (1000)        5 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/libspline/VERSION
+-rw-rw-r--   0 matt      (1000) matt      (1000)       47 2023-07-07 22:53:44.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/libspline/clean.bat
+-rw-rw-r--   0 matt      (1000) matt      (1000)       44 2023-04-27 16:08:43.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/libspline/compile.bat
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2815 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/libspline/generateheader.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-10 22:51:19.670129 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/libspline/include/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      612 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/libspline/include/spline.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)      139 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/libspline/install.bat
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1442 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/libspline/makefile
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-10 22:51:19.670129 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/libspline/src/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      127 2023-04-27 16:08:43.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/libspline/src/compile.bat
+-rw-rw-r--   0 matt      (1000) matt      (1000)      165 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/libspline/src/compileobj.bat
+-rw-rw-r--   0 matt      (1000) matt      (1000)      238 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/libspline/src/libspline.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      213 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/libspline/src/libspline.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)      682 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/libspline/src/makefile
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2856 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/libspline/src/spline.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      345 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/libspline/src/spline.h
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-10 22:51:19.674129 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/libspline/test/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      714 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/libspline/test/cpptest.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      665 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/libspline/test/ctest.c
+-rw-rw-r--   0 matt      (1000) matt      (1000)      543 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/libspline/test/makefile
+-rw-rw-r--   0 matt      (1000) matt      (1000)    37488 2023-07-07 22:53:44.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/libspline/test/testspline.png
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2881 2023-04-27 13:15:09.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/libspline/test/testspline.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1413 2023-07-07 22:53:29.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/makefile
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-10 22:51:19.674129 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     8196 2023-04-27 16:08:43.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/.DS_Store
+-rw-rw-r--   0 matt      (1000) matt      (1000)    71079 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/ConvCoords.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)    38295 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/ConvCoords.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)      478 2023-07-06 20:58:23.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/compile.bat
+-rw-rw-r--   0 matt      (1000) matt      (1000)      145 2023-04-27 16:08:43.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/compileobj.bat
+-rw-rw-r--   0 matt      (1000) matt      (1000)      213 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/dummyfunc.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      231 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/dummyfunc.h
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-10 22:51:19.674129 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/fortran/
+-rw-rw-r--   0 matt      (1000) matt      (1000)    85665 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/fortran/Geopack-2008_mkj_dp.f
+-rw-rw-r--   0 matt      (1000) matt      (1000)    86704 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/fortran/T01_01.f
+-rwxrwxr-x   0 matt      (1000) matt      (1000)    15845 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/fortran/T89c.f
+-rw-rw-r--   0 matt      (1000) matt      (1000)    93009 2023-07-09 21:12:38.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/fortran/T96.f
+-rw-rw-r--   0 matt      (1000) matt      (1000)    86349 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/fortran/TS04c.f
+-rw-rw-r--   0 matt      (1000) matt      (1000)     7715 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/fortran/bessel.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3579 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/fortran/bessel.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)      517 2023-07-09 21:12:38.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/fortran/compile.bat
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2694 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/fortran/geopack.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)      574 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/fortran/makefile
+-rw-rw-r--   0 matt      (1000) matt      (1000)    13276 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/fortran/t89.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1527 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/fortran/t89.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)    18547 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/fortran/t89params.ods
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4252 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/fortran/t96.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)     5185 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/fortran/wparams.f95
+-rw-rw-r--   0 matt      (1000) matt      (1000)      745 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/getdipoletilt.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      420 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/getdipoletilt.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1632 2023-04-28 08:59:56.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/makefile
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-10 22:51:19.674129 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/matrix/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      415 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/matrix/compile.bat
+-rw-rw-r--   0 matt      (1000) matt      (1000)      148 2023-04-27 16:08:43.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/matrix/compileobj.bat
+-rw-rw-r--   0 matt      (1000) matt      (1000)      160 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/matrix/identity.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      139 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/matrix/identity.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)      908 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/matrix/libmatrix.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      394 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/matrix/libmatrix.h
+-rwxrwxr-x   0 matt      (1000) matt      (1000)   292104 2023-04-27 16:08:43.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/matrix/libmatrix.so
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1040 2023-04-27 16:08:43.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/matrix/makefile
+-rw-rw-r--   0 matt      (1000) matt      (1000)    11820 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/matrix/matrix.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2001 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/matrix/matrix.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4285 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/matrix/matrixarray.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1036 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/matrix/matrixarray.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)    20389 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/matrix/matrixmath.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4198 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/matrix/matrixmath.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2161 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/matrix/rotmatrix.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1407 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/matrix/rotmatrix.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2392 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/matrix/testmatrix.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3480 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/modelfield.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1770 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/modelfield.h
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-10 22:51:19.674129 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/modelparams/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1242 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/modelparams/calculateg.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      268 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/modelparams/calculateg.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)     7507 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/modelparams/calculatew.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      458 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/modelparams/calculatew.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)      385 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/modelparams/checkv.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      249 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/modelparams/checkv.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)      367 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/modelparams/compile.bat
+-rw-rw-r--   0 matt      (1000) matt      (1000)      148 2023-04-27 16:08:43.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/modelparams/compileobj.bat
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1103 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/modelparams/fillinkp.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      249 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/modelparams/fillinkp.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)      511 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/modelparams/makefile
+-rw-rw-r--   0 matt      (1000) matt      (1000)     6281 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/modelparams/modelparams.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1922 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/modelparams/modelparams.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)    12057 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/modelparams/tsygdata.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2203 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/modelparams/tsygdata.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1081 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/recalc.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      331 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/recalc.h
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-10 22:51:19.678129 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tools/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1203 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tools/BubbleArgSort.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      574 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tools/BubbleArgSort.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2243 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tools/BubbleSort.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1353 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tools/BubbleSort.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)      250 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tools/argmax.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      144 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tools/argmax.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)      433 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tools/carttospherical.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      223 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tools/carttospherical.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)      339 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tools/compile.bat
+-rw-rw-r--   0 matt      (1000) matt      (1000)      148 2023-04-27 16:08:43.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tools/compileobj.bat
+-rw-rw-r--   0 matt      (1000) matt      (1000)      165 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tools/linterp.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      169 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tools/linterp.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)      488 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tools/makefile
+-rw-rw-r--   0 matt      (1000) matt      (1000)      193 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tools/reverseelements.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      147 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tools/reverseelements.h
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-10 22:51:19.678129 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2755 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/calculatehalpha.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      810 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/calculatehalpha.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)      949 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/compile.bat
+-rw-rw-r--   0 matt      (1000) matt      (1000)      148 2023-04-27 16:08:43.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/compileobj.bat
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2143 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/converttracecoords.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      543 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/converttracecoords.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)      490 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/fieldlinedist.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      192 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/fieldlinedist.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)      718 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/fieldlinemidpoint.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      255 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/fieldlinemidpoint.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)      381 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/fieldliner.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      183 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/fieldliner.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)      352 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/fieldlinernorm.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      176 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/fieldlinernorm.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3099 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/getmagequatorfp.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      577 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/getmagequatorfp.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)     8254 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/interptraceclosestpos.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1299 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/interptraceclosestpos.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1145 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/latlonlt.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      400 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/latlonlt.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1039 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/makefile
+-rw-rw-r--   0 matt      (1000) matt      (1000)    23270 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/trace.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)     5486 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/trace.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)     4920 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/traceclosestpos.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1428 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/traceclosestpos.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)     5011 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/tracefield.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2796 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/tracefield.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1561 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/tracefieldline.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      494 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/tracefieldline.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)     3859 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/tracefootprints.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      812 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/tracefootprints.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)      953 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/tracerotationmatrices.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      291 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/tracerotationmatrices.h
+-rw-rw-r--   0 matt      (1000) matt      (1000)      539 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/withinmp.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      196 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/src/withinmp.h
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-10 22:51:19.678129 PyGeopack-1.2.2/PyGeopack/__data/geopack/test/
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-10 22:51:19.678129 PyGeopack-1.2.2/PyGeopack/__data/geopack/test/fortran/
+-rwxrwxr-x   0 matt      (1000) matt      (1000)    15356 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/test/fortran/T89c.f
+-rw-rw-r--   0 matt      (1000) matt      (1000)      859 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/test/fortran/makefile
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1047 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/test/fortran/testfortran.cc
+-rw-rw-r--   0 matt      (1000) matt      (1000)      705 2023-04-27 16:08:43.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/test/makefile
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2112 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/test/test.c
+-rw-rw-r--   0 matt      (1000) matt      (1000)     1489 2023-04-27 13:13:19.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/test/test.cc
+-rwxrwxr-x   0 matt      (1000) matt      (1000)    21104 2023-07-06 20:58:23.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/test/testc
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-10 22:51:19.658129 PyGeopack-1.2.2/PyGeopack/__data/geopack/test/testc.dSYM/
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-10 22:51:19.678129 PyGeopack-1.2.2/PyGeopack/__data/geopack/test/testc.dSYM/Contents/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      634 2023-04-27 16:08:43.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/test/testc.dSYM/Contents/Info.plist
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-10 22:51:19.658129 PyGeopack-1.2.2/PyGeopack/__data/geopack/test/testc.dSYM/Contents/Resources/
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-10 22:51:19.678129 PyGeopack-1.2.2/PyGeopack/__data/geopack/test/testc.dSYM/Contents/Resources/DWARF/
+-rw-rw-r--   0 matt      (1000) matt      (1000)    12741 2023-04-27 16:08:43.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/test/testc.dSYM/Contents/Resources/DWARF/testc
+-rwxrwxr-x   0 matt      (1000) matt      (1000)    30672 2023-07-06 20:58:23.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/test/testcc
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-10 22:51:19.662129 PyGeopack-1.2.2/PyGeopack/__data/geopack/test/testcc.dSYM/
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-10 22:51:19.678129 PyGeopack-1.2.2/PyGeopack/__data/geopack/test/testcc.dSYM/Contents/
+-rw-rw-r--   0 matt      (1000) matt      (1000)      635 2023-04-27 16:08:43.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/test/testcc.dSYM/Contents/Info.plist
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-10 22:51:19.662129 PyGeopack-1.2.2/PyGeopack/__data/geopack/test/testcc.dSYM/Contents/Resources/
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-10 22:51:19.678129 PyGeopack-1.2.2/PyGeopack/__data/geopack/test/testcc.dSYM/Contents/Resources/DWARF/
+-rw-rw-r--   0 matt      (1000) matt      (1000)    16387 2023-04-27 16:08:43.000000 PyGeopack-1.2.2/PyGeopack/__data/geopack/test/testcc.dSYM/Contents/Resources/DWARF/testcc
+-rw-rw-r--   0 matt      (1000) matt      (1000)       98 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/__del__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)      345 2023-07-10 22:41:03.000000 PyGeopack-1.2.2/PyGeopack/__init__.py
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2737 2023-04-27 13:12:39.000000 PyGeopack-1.2.2/PyGeopack/ct.py
+drwxrwxr-x   0 matt      (1000) matt      (1000)        0 2023-07-10 22:51:19.666128 PyGeopack-1.2.2/PyGeopack.egg-info/
+-rw-rw-r--   0 matt      (1000) matt      (1000)    28455 2023-07-10 22:51:19.000000 PyGeopack-1.2.2/PyGeopack.egg-info/PKG-INFO
+-rw-rw-r--   0 matt      (1000) matt      (1000)    12965 2023-07-10 22:51:19.000000 PyGeopack-1.2.2/PyGeopack.egg-info/SOURCES.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)        1 2023-07-10 22:51:19.000000 PyGeopack-1.2.2/PyGeopack.egg-info/dependency_links.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)       83 2023-07-10 22:51:19.000000 PyGeopack-1.2.2/PyGeopack.egg-info/requires.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)       10 2023-07-10 22:51:19.000000 PyGeopack-1.2.2/PyGeopack.egg-info/top_level.txt
+-rw-rw-r--   0 matt      (1000) matt      (1000)    27989 2023-07-10 22:50:52.000000 PyGeopack-1.2.2/README.md
+-rw-rw-r--   0 matt      (1000) matt      (1000)       38 2023-07-10 22:51:19.678129 PyGeopack-1.2.2/setup.cfg
+-rw-rw-r--   0 matt      (1000) matt      (1000)     2075 2023-07-08 22:23:20.000000 PyGeopack-1.2.2/setup.py
```

### Comparing `PyGeopack-1.2.1/LICENSE` & `PyGeopack-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PKG-INFO` & `PyGeopack-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyGeopack
-Version: 1.2.1
+Version: 1.2.2
 Summary: Geopack08 wrapper for Python
 Home-page: https://github.com/mattkjames7/PyGeopack
 Author: Matthew Knight James
 Author-email: mattkjames7@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -63,28 +63,30 @@
 ```
 pip3 install PyGeopack --user
 ```
 
 or by downloading the latest release on GitHub and running:
 
 ```
-pip3 install PyGeopack-1.2.0.tar.gz --user
+pip3 install PyGeopack-1.2.2.tar.gz --user
 ```
 
 NOTE: You should uninstall any previous versions before installing this. If you had a version installed before 0.0.12 - you will need to remove the old shared object files - they are likely to be contained somewhere like (depending on the Python version used):
 
 ```
 ~/.local/lib/python3.10/site-packages/PyGeopack/
 ```
 
 It's best just to remove everything within that folder!
 
 ### 2.2 Windows
 
-Install TDM-GCC (make sure to select `g++` and `gfortran`), install anaconda and then install the package in an anaconda power shell session using `pip3` as in the Linux instructions. The same environment variables will need to be set as those in the Linux instructions. This package has only briefly been tested in Windows 10 x64, mileage may vary with other versions of Windows. It also appears that other Windows compilers may not be able to compile the code, if you do come across such a problem please feel free to raise an issue so I can have a look into it.
+Install TDM-GCC (make sure to select `g++` and `gfortran`), install anaconda and then install the package in an anaconda power shell session using `pip3` as in the Linux instructions. The same environment variables will need to be set as those in the Linux instructions. This package has only briefly been tested in Windows 10 x64, mileage may vary with other versions of Windows. This code has also been successfully built using the Strawberry Perl compilers.
+
+It appears that `ctypes` doesn't necessarily search the directories listed within the `$PATH` environment variable for the C++ dependencies on some versions of Python. To hack myself around this, I have added a function which with scan all of the directories within `$PATH` for `libstdc++*.dll`; if found then the paths which it is found in will be added using `os.add_dll_directory()`. If the directory of your compiler's libraries is not listed within `$PATH`, this may be the cause of any failures at build time or importing the library. If you have multiple compilers installed, then I am unsure what will happen! Feel free to post an issue if you encounter any errors, or if you have any suggestions for fixes.
 
 ### 2.3 Mac
 
 This module should work on MacOS as it does on Linux, with the same requirements. I have tested it using MacOS Big Sur.
 
 ## 3 Post-install
```

### Comparing `PyGeopack-1.2.1/PyGeopack/Coords/ConvCoords.py` & `PyGeopack-1.2.2/PyGeopack/Coords/ConvCoords.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Coords/GEItoGEO.py` & `PyGeopack-1.2.2/PyGeopack/Coords/GEItoGEO.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Coords/GEItoGSE.py` & `PyGeopack-1.2.2/PyGeopack/Coords/GEItoGSE.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Coords/GEItoGSM.py` & `PyGeopack-1.2.2/PyGeopack/Coords/GEItoGSM.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Coords/GEItoMAG.py` & `PyGeopack-1.2.2/PyGeopack/Coords/GEItoMAG.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Coords/GEItoSM.py` & `PyGeopack-1.2.2/PyGeopack/Coords/GEItoSM.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Coords/GEOtoGEI.py` & `PyGeopack-1.2.2/PyGeopack/Coords/GEOtoGEI.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Coords/GEOtoGSE.py` & `PyGeopack-1.2.2/PyGeopack/Coords/GEOtoGSE.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Coords/GEOtoGSM.py` & `PyGeopack-1.2.2/PyGeopack/Coords/GEOtoGSM.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Coords/GEOtoMAG.py` & `PyGeopack-1.2.2/PyGeopack/Coords/GEOtoMAG.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Coords/GEOtoSM.py` & `PyGeopack-1.2.2/PyGeopack/Coords/GEOtoSM.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Coords/GSEtoGEI.py` & `PyGeopack-1.2.2/PyGeopack/Coords/GSEtoGEI.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Coords/GSEtoGEO.py` & `PyGeopack-1.2.2/PyGeopack/Coords/GSEtoGEO.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Coords/GSEtoGSM.py` & `PyGeopack-1.2.2/PyGeopack/Coords/GSEtoGSM.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Coords/GSEtoMAG.py` & `PyGeopack-1.2.2/PyGeopack/Coords/GSEtoMAG.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Coords/GSEtoSM.py` & `PyGeopack-1.2.2/PyGeopack/Coords/GSEtoSM.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Coords/GSMtoGEI.py` & `PyGeopack-1.2.2/PyGeopack/Coords/GSMtoGEI.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Coords/GSMtoGEO.py` & `PyGeopack-1.2.2/PyGeopack/Coords/GSMtoGEO.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Coords/GSMtoGSE.py` & `PyGeopack-1.2.2/PyGeopack/Coords/GSMtoGSE.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Coords/GSMtoMAG.py` & `PyGeopack-1.2.2/PyGeopack/Coords/GSMtoMAG.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Coords/GSMtoSM.py` & `PyGeopack-1.2.2/PyGeopack/Coords/GSMtoSM.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Coords/MAGtoGEI.py` & `PyGeopack-1.2.2/PyGeopack/Coords/MAGtoGEI.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Coords/MAGtoGEO.py` & `PyGeopack-1.2.2/PyGeopack/Coords/MAGtoGEO.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Coords/MAGtoGSE.py` & `PyGeopack-1.2.2/PyGeopack/Coords/MAGtoGSE.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Coords/MAGtoGSM.py` & `PyGeopack-1.2.2/PyGeopack/Coords/MAGtoGSM.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Coords/MAGtoSM.py` & `PyGeopack-1.2.2/PyGeopack/Coords/MAGtoSM.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Coords/MLONtoMLT.py` & `PyGeopack-1.2.2/PyGeopack/Coords/MLONtoMLT.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Coords/MLTtoMLON.py` & `PyGeopack-1.2.2/PyGeopack/Coords/MLTtoMLON.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Coords/SMtoGEI.py` & `PyGeopack-1.2.2/PyGeopack/Coords/SMtoGEI.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Coords/SMtoGEO.py` & `PyGeopack-1.2.2/PyGeopack/Coords/SMtoGEO.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Coords/SMtoGSE.py` & `PyGeopack-1.2.2/PyGeopack/Coords/SMtoGSE.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Coords/SMtoGSM.py` & `PyGeopack-1.2.2/PyGeopack/Coords/SMtoGSM.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Coords/SMtoMAG.py` & `PyGeopack-1.2.2/PyGeopack/Coords/SMtoMAG.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Coords/_CFunctions.py` & `PyGeopack-1.2.2/PyGeopack/Coords/_CFunctions.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Coords/__init__.py` & `PyGeopack-1.2.2/PyGeopack/Coords/__init__.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/ModelField.py` & `PyGeopack-1.2.2/PyGeopack/ModelField.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Params/GetDipoleTilt.py` & `PyGeopack-1.2.2/PyGeopack/Params/GetDipoleTilt.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Params/GetModelParams.py` & `PyGeopack-1.2.2/PyGeopack/Params/GetModelParams.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Params/ReadTSData.py` & `PyGeopack-1.2.2/PyGeopack/Params/ReadTSData.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Params/UpdateParameters.py` & `PyGeopack-1.2.2/PyGeopack/Params/UpdateParameters.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Params/_CFunctions.py` & `PyGeopack-1.2.2/PyGeopack/Params/_CFunctions.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Params/_CalculateParameters.py` & `PyGeopack-1.2.2/PyGeopack/Params/_CalculateParameters.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Params/_DownloadTS05Data.py` & `PyGeopack-1.2.2/PyGeopack/Params/_DownloadTS05Data.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/ShueMP.py` & `PyGeopack-1.2.2/PyGeopack/ShueMP.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Test/PlotTraces.py` & `PyGeopack-1.2.2/PyGeopack/Test/PlotTraces.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Test/TestHarmonic.py` & `PyGeopack-1.2.2/PyGeopack/Test/TestHarmonic.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Tools/PlotPlanet.py` & `PyGeopack-1.2.2/PyGeopack/Tools/PlotPlanet.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/Tools/T89CurrentSheet.py` & `PyGeopack-1.2.2/PyGeopack/Tools/T89CurrentSheet.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/TraceField.py` & `PyGeopack-1.2.2/PyGeopack/TraceField.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/_CFunctions.py` & `PyGeopack-1.2.2/PyGeopack/_CFunctions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import numpy as np
 import ctypes
 import os
 from . import Globals
 from .ct import c_char_p,c_bool,c_bool_ptr,c_int,c_int_ptr
 from .ct import c_float,c_float_ptr,c_double,c_double_ptr,c_double_ptr_ptr
-from ._CheckFirstImport import getLibFilename
+from ._CheckFirstImport import getLibFilename,addWindowsSearchPaths
 import platform
 
 
 try:
 	if platform.system() == 'Darwin':
 		cwd = os.getcwd()
 		os.chdir(Globals.ModulePath + '__data/geopack/lib/')
 		libgeopack = ctypes.CDLL(getLibFilename(True))
 		os.chdir(cwd)
+	elif platform.system() == 'Windows':
+		addWindowsSearchPaths()
+		libgeopack = ctypes.CDLL(getLibFilename())
 	else:
 		libgeopack = ctypes.CDLL(getLibFilename())
 except:
 	print('Importing '+getLibFilename(isShort=True)+' failed, please reinstall')
 	raise SystemError
```

### Comparing `PyGeopack-1.2.1/PyGeopack/_CheckFirstImport.py` & `PyGeopack-1.2.2/PyGeopack/_CheckFirstImport.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import subprocess
 import numpy as np
 from . import Globals
 from . import ct
 import platform
-
+import fnmatch
 
 def getLibFilename(isShort=False):
     """
     Return library filename string
     
     Inputs
     ======
@@ -42,14 +42,40 @@
 
 def checkLibExists():
     """Check if library file exist, and start compilation script if not."""
     if not os.path.isfile(getLibFilename()):
         print(getLibFilename(isShort=True)+" not found, try reinstalling")
         raise SystemError
 
+def getWindowsSearchPaths():
+    '''Scan the directories within PATH and look for std C++ libs'''
+    paths = os.getenv('PATH')
+    paths = paths.split(';')
+
+    pattern = 'libstdc++*.dll'
+
+    out = []
+    for p in paths:
+        if os.path.isdir(p):
+            files = os.listdir(p)
+            mch = any(fnmatch.fnmatch(f,pattern) for f in files)
+            if mch:
+                out.append(p)
+    
+    return out
+
+def addWindowsSearchPaths():
+
+    paths = getWindowsSearchPaths()
+    for p in paths:
+        if os.path.isdir(p):
+            os.add_dll_directory(p)
+
+    
+
 
 
 def _CheckFirstImport():
     #first of all - check if the shared object exists
     checkLibExists()
 
     #Check if the GEOPACK_PATH variable has been set
```

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/.DS_Store` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/.DS_Store`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/LICENSE` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/LICENSE`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/doc/equations/agufull08.bst` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/doc/equations/agufull08.bst`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/doc/equations/equations.blg` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/doc/equations/equations.blg`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/doc/equations/equations.log` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/doc/equations/equations.log`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/doc/equations/equations.pdf` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/doc/equations/equations.pdf`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/doc/equations/equations.synctex.gz` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/doc/equations/equations.synctex.gz`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/doc/equations/equations.tex` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/doc/equations/equations.tex`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/include/geopack.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/include/geopack.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/LICENSE` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/LICENSE`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/README.md` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/README.md`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/include/datetime.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/include/datetime.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/makefile` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/makefile`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/BubbleSort.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/BubbleSort.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/BubbleSort.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/BubbleSort.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/ContUT.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/ContUT.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/ContUT.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/ContUT.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/DateDifference.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/DateDifference.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/DateDifference.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/DateDifference.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/DateJoin.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/DateJoin.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/DateJoin.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/DateJoin.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/DateSplit.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/DateSplit.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/DateSplit.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/DateSplit.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/DayNo.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/DayNo.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/DayNo.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/DayNo.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/JulDay.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/JulDay.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/JulDay.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/JulDay.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/JulDaytoDate.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/JulDaytoDate.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/JulDaytoDate.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/JulDaytoDate.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/LeapYear.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/LeapYear.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/LeapYear.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/LeapYear.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/MidTime.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/MidTime.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/MidTime.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/MidTime.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/MinusDay.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/MinusDay.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/MinusDay.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/MinusDay.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/NearestTimeIndex.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/NearestTimeIndex.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/NearestTimeIndex.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/NearestTimeIndex.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/PlusDay.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/PlusDay.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/PlusDay.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/PlusDay.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/TimeDifference.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/TimeDifference.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/TimeDifference.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/TimeDifference.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/Unique.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/Unique.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/Unique.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/Unique.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/UnixTime.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/UnixTime.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/UnixTime.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/UnixTime.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/WhereEq.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/WhereEq.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/WhereEq.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/WhereEq.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/WithinTimeRange.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/WithinTimeRange.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/WithinTimeRange.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/WithinTimeRange.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/compileobj.bat` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/compileobj.bat`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/hhmm.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/hhmm.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/hhmm.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/hhmm.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/src/makefile` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/src/makefile`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/test/testc.c` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/test/testc.c`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/datetime/test/testcc.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/datetime/test/testcc.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/libspline/LICENSE` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/libspline/LICENSE`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/libspline/README.md` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/libspline/README.md`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/libspline/generateheader.py` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/libspline/generateheader.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/libspline/include/spline.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/libspline/include/spline.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/libspline/makefile` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/libspline/makefile`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/libspline/src/makefile` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/libspline/src/makefile`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/libspline/src/spline.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/libspline/src/spline.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/libspline/test/cpptest.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/libspline/test/cpptest.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/libspline/test/ctest.c` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/libspline/test/ctest.c`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/libspline/test/makefile` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/libspline/test/makefile`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/libspline/test/testspline.png` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/libspline/test/testspline.png`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/lib/libspline/test/testspline.py` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/lib/libspline/test/testspline.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/makefile` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/makefile`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/.DS_Store` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/ConvCoords.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/ConvCoords.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/ConvCoords.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/ConvCoords.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/fortran/Geopack-2008_mkj_dp.f` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/fortran/Geopack-2008_mkj_dp.f`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/fortran/T01_01.f` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/fortran/T01_01.f`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/fortran/T89c.f` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/fortran/T89c.f`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/fortran/T96.f` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/fortran/T96.f`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/fortran/TS04c.f` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/fortran/TS04c.f`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/fortran/bessel.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/fortran/bessel.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/fortran/bessel.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/fortran/bessel.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/fortran/compile.bat` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/fortran/compile.bat`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/fortran/geopack.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/fortran/geopack.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/fortran/makefile` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/fortran/makefile`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/fortran/t89.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/fortran/t89.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/fortran/t89.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/fortran/t89.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/fortran/t89params.ods` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/fortran/t89params.ods`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/fortran/t96.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/fortran/t96.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/fortran/wparams.f95` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/fortran/wparams.f95`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/getdipoletilt.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/getdipoletilt.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/makefile` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/makefile`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/matrix/libmatrix.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/matrix/libmatrix.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/matrix/libmatrix.so` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/matrix/libmatrix.so`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/matrix/makefile` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/matrix/makefile`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/matrix/matrix.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/matrix/matrix.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/matrix/matrix.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/matrix/matrix.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/matrix/matrixarray.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/matrix/matrixarray.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/matrix/matrixarray.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/matrix/matrixarray.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/matrix/matrixmath.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/matrix/matrixmath.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/matrix/matrixmath.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/matrix/matrixmath.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/matrix/rotmatrix.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/matrix/rotmatrix.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/matrix/rotmatrix.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/matrix/rotmatrix.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/matrix/testmatrix.py` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/matrix/testmatrix.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/modelfield.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/modelfield.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/modelfield.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/modelfield.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/modelparams/calculateg.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/modelparams/calculateg.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/modelparams/calculatew.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/modelparams/calculatew.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/modelparams/fillinkp.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/modelparams/fillinkp.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/modelparams/modelparams.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/modelparams/modelparams.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/modelparams/modelparams.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/modelparams/modelparams.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/modelparams/tsygdata.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/modelparams/tsygdata.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/modelparams/tsygdata.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/modelparams/tsygdata.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/recalc.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/recalc.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tools/BubbleArgSort.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tools/BubbleArgSort.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tools/BubbleArgSort.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tools/BubbleArgSort.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tools/BubbleSort.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tools/BubbleSort.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tools/BubbleSort.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tools/BubbleSort.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/calculatehalpha.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/calculatehalpha.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/calculatehalpha.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/calculatehalpha.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/compile.bat` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/compile.bat`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/converttracecoords.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/converttracecoords.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/converttracecoords.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/converttracecoords.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/fieldlinemidpoint.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/fieldlinemidpoint.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/getmagequatorfp.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/getmagequatorfp.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/getmagequatorfp.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/getmagequatorfp.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/interptraceclosestpos.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/interptraceclosestpos.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/interptraceclosestpos.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/interptraceclosestpos.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/latlonlt.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/latlonlt.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/makefile` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/makefile`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/trace.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/trace.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/trace.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/trace.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/traceclosestpos.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/traceclosestpos.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/traceclosestpos.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/traceclosestpos.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/tracefield.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/tracefield.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/tracefield.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/tracefield.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/tracefieldline.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/tracefieldline.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/tracefootprints.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/tracefootprints.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/tracefootprints.h` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/tracefootprints.h`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/tracing/tracerotationmatrices.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/tracing/tracerotationmatrices.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/src/withinmp.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/src/withinmp.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/test/fortran/T89c.f` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/test/fortran/T89c.f`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/test/fortran/makefile` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/test/fortran/makefile`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/test/fortran/testfortran.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/test/fortran/testfortran.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/test/makefile` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/test/makefile`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/test/test.c` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/test/test.c`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/test/test.cc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/test/test.cc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/test/testc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/test/testc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/test/testc.dSYM/Contents/Info.plist` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/test/testc.dSYM/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/test/testc.dSYM/Contents/Resources/DWARF/testc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/test/testc.dSYM/Contents/Resources/DWARF/testc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/test/testcc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/test/testcc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/test/testcc.dSYM/Contents/Info.plist` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/test/testcc.dSYM/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/__data/geopack/test/testcc.dSYM/Contents/Resources/DWARF/testcc` & `PyGeopack-1.2.2/PyGeopack/__data/geopack/test/testcc.dSYM/Contents/Resources/DWARF/testcc`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack/ct.py` & `PyGeopack-1.2.2/PyGeopack/ct.py`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/PyGeopack.egg-info/PKG-INFO` & `PyGeopack-1.2.2/PyGeopack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyGeopack
-Version: 1.2.1
+Version: 1.2.2
 Summary: Geopack08 wrapper for Python
 Home-page: https://github.com/mattkjames7/PyGeopack
 Author: Matthew Knight James
 Author-email: mattkjames7@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -63,28 +63,30 @@
 ```
 pip3 install PyGeopack --user
 ```
 
 or by downloading the latest release on GitHub and running:
 
 ```
-pip3 install PyGeopack-1.2.0.tar.gz --user
+pip3 install PyGeopack-1.2.2.tar.gz --user
 ```
 
 NOTE: You should uninstall any previous versions before installing this. If you had a version installed before 0.0.12 - you will need to remove the old shared object files - they are likely to be contained somewhere like (depending on the Python version used):
 
 ```
 ~/.local/lib/python3.10/site-packages/PyGeopack/
 ```
 
 It's best just to remove everything within that folder!
 
 ### 2.2 Windows
 
-Install TDM-GCC (make sure to select `g++` and `gfortran`), install anaconda and then install the package in an anaconda power shell session using `pip3` as in the Linux instructions. The same environment variables will need to be set as those in the Linux instructions. This package has only briefly been tested in Windows 10 x64, mileage may vary with other versions of Windows. It also appears that other Windows compilers may not be able to compile the code, if you do come across such a problem please feel free to raise an issue so I can have a look into it.
+Install TDM-GCC (make sure to select `g++` and `gfortran`), install anaconda and then install the package in an anaconda power shell session using `pip3` as in the Linux instructions. The same environment variables will need to be set as those in the Linux instructions. This package has only briefly been tested in Windows 10 x64, mileage may vary with other versions of Windows. This code has also been successfully built using the Strawberry Perl compilers.
+
+It appears that `ctypes` doesn't necessarily search the directories listed within the `$PATH` environment variable for the C++ dependencies on some versions of Python. To hack myself around this, I have added a function which with scan all of the directories within `$PATH` for `libstdc++*.dll`; if found then the paths which it is found in will be added using `os.add_dll_directory()`. If the directory of your compiler's libraries is not listed within `$PATH`, this may be the cause of any failures at build time or importing the library. If you have multiple compilers installed, then I am unsure what will happen! Feel free to post an issue if you encounter any errors, or if you have any suggestions for fixes.
 
 ### 2.3 Mac
 
 This module should work on MacOS as it does on Linux, with the same requirements. I have tested it using MacOS Big Sur.
 
 ## 3 Post-install
```

### Comparing `PyGeopack-1.2.1/PyGeopack.egg-info/SOURCES.txt` & `PyGeopack-1.2.2/PyGeopack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyGeopack-1.2.1/README.md` & `PyGeopack-1.2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -48,28 +48,30 @@
 ```
 pip3 install PyGeopack --user
 ```
 
 or by downloading the latest release on GitHub and running:
 
 ```
-pip3 install PyGeopack-1.2.0.tar.gz --user
+pip3 install PyGeopack-1.2.2.tar.gz --user
 ```
 
 NOTE: You should uninstall any previous versions before installing this. If you had a version installed before 0.0.12 - you will need to remove the old shared object files - they are likely to be contained somewhere like (depending on the Python version used):
 
 ```
 ~/.local/lib/python3.10/site-packages/PyGeopack/
 ```
 
 It's best just to remove everything within that folder!
 
 ### 2.2 Windows
 
-Install TDM-GCC (make sure to select `g++` and `gfortran`), install anaconda and then install the package in an anaconda power shell session using `pip3` as in the Linux instructions. The same environment variables will need to be set as those in the Linux instructions. This package has only briefly been tested in Windows 10 x64, mileage may vary with other versions of Windows. It also appears that other Windows compilers may not be able to compile the code, if you do come across such a problem please feel free to raise an issue so I can have a look into it.
+Install TDM-GCC (make sure to select `g++` and `gfortran`), install anaconda and then install the package in an anaconda power shell session using `pip3` as in the Linux instructions. The same environment variables will need to be set as those in the Linux instructions. This package has only briefly been tested in Windows 10 x64, mileage may vary with other versions of Windows. This code has also been successfully built using the Strawberry Perl compilers.
+
+It appears that `ctypes` doesn't necessarily search the directories listed within the `$PATH` environment variable for the C++ dependencies on some versions of Python. To hack myself around this, I have added a function which with scan all of the directories within `$PATH` for `libstdc++*.dll`; if found then the paths which it is found in will be added using `os.add_dll_directory()`. If the directory of your compiler's libraries is not listed within `$PATH`, this may be the cause of any failures at build time or importing the library. If you have multiple compilers installed, then I am unsure what will happen! Feel free to post an issue if you encounter any errors, or if you have any suggestions for fixes.
 
 ### 2.3 Mac
 
 This module should work on MacOS as it does on Linux, with the same requirements. I have tested it using MacOS Big Sur.
 
 ## 3 Post-install
```

### Comparing `PyGeopack-1.2.1/setup.py` & `PyGeopack-1.2.2/setup.py`

 * *Files identical despite different names*

