# Comparing `tmp/KofiPyQtHelper-0.0.6.tar.gz` & `tmp/KofiPyQtHelper-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/KofiPyQtHelper-0.0.6.tar", last modified: Tue Jul 11 09:55:40 2023, max compression
+gzip compressed data, was "dist/KofiPyQtHelper-0.0.7.tar", last modified: Tue Jul 11 15:21:23 2023, max compression
```

## Comparing `KofiPyQtHelper-0.0.6.tar` & `KofiPyQtHelper-0.0.7.tar`

### file list

```diff
@@ -1,51 +1,11 @@
-drwxr-xr-x   0 kofi       (501) staff       (20)        0 2023-07-11 09:55:40.000000 KofiPyQtHelper-0.0.6/
-drwxr-xr-x   0 kofi       (501) staff       (20)        0 2023-07-11 09:55:40.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper/
--rw-r--r--   0 kofi       (501) staff       (20)      262 2023-07-11 09:55:29.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper/__init__.py
--rw-r--r--   0 kofi       (501) staff       (20)      922 2023-07-11 06:59:52.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper/app.py
-drwxr-xr-x   0 kofi       (501) staff       (20)        0 2023-07-11 09:55:40.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper/components/
--rw-r--r--   0 kofi       (501) staff       (20)     7287 2023-07-11 06:59:13.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper/components/BaseWidget.py
--rw-r--r--   0 kofi       (501) staff       (20)     6337 2023-07-11 06:59:13.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper/components/CustomGraphics.py
--rw-r--r--   0 kofi       (501) staff       (20)     3567 2023-07-11 06:59:13.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper/components/FlowLayout.py
--rw-r--r--   0 kofi       (501) staff       (20)     5170 2023-07-11 06:59:13.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper/components/MatplotlibFigure.py
--rw-r--r--   0 kofi       (501) staff       (20)      172 2023-07-11 06:59:13.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper/components/__init__.py
-drwxr-xr-x   0 kofi       (501) staff       (20)        0 2023-07-11 09:55:40.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper/enums/
--rw-r--r--   0 kofi       (501) staff       (20)      380 2023-07-11 06:59:13.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper/enums/ColumnType.py
--rw-r--r--   0 kofi       (501) staff       (20)      294 2023-07-11 06:59:13.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper/enums/ComboboxValueType.py
--rw-r--r--   0 kofi       (501) staff       (20)      497 2023-07-11 06:59:13.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper/enums/SetupEnums.py
--rw-r--r--   0 kofi       (501) staff       (20)      171 2023-07-11 06:59:13.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper/enums/__init__.py
-drwxr-xr-x   0 kofi       (501) staff       (20)        0 2023-07-11 09:55:40.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper/models/
--rw-r--r--   0 kofi       (501) staff       (20)     1664 2023-07-11 06:59:13.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper/models/PlotModel.py
--rw-r--r--   0 kofi       (501) staff       (20)      171 2023-07-11 06:59:13.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper/models/__init__.py
-drwxr-xr-x   0 kofi       (501) staff       (20)        0 2023-07-11 09:55:40.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper/utils/
--rw-r--r--   0 kofi       (501) staff       (20)    12905 2023-07-11 06:59:13.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper/utils/Command.py
-drwxr-xr-x   0 kofi       (501) staff       (20)        0 2023-07-11 09:55:40.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper/utils/Commands/
--rw-r--r--   0 kofi       (501) staff       (20)    12401 2023-07-11 06:59:13.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper/utils/Commands/GraphCommand.py
--rw-r--r--   0 kofi       (501) staff       (20)     5073 2023-07-11 06:59:13.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper/utils/Commands/HistoryCommand.py
--rw-r--r--   0 kofi       (501) staff       (20)     1022 2023-07-11 06:59:13.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper/utils/Commands/PdfCommand.py
--rw-r--r--   0 kofi       (501) staff       (20)     4830 2023-07-11 06:59:13.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper/utils/Commands/WidgetCommand.py
--rw-r--r--   0 kofi       (501) staff       (20)      172 2023-07-11 06:59:13.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper/utils/Commands/__init__.py
--rw-r--r--   0 kofi       (501) staff       (20)     1610 2023-07-11 06:59:13.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper/utils/CommonHelper.py
--rw-r--r--   0 kofi       (501) staff       (20)     1055 2023-07-11 06:59:13.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper/utils/ExcelHelper.py
-drwxr-xr-x   0 kofi       (501) staff       (20)        0 2023-07-11 09:55:40.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper/utils/Ui/
--rw-r--r--   0 kofi       (501) staff       (20)    10072 2023-07-11 08:22:10.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper/utils/Ui/ComponentHelper.py
--rw-r--r--   0 kofi       (501) staff       (20)     4430 2023-07-11 07:25:27.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper/utils/Ui/LayoutHelper.py
--rw-r--r--   0 kofi       (501) staff       (20)     1576 2023-07-11 07:23:48.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper/utils/Ui/UiCommon.py
--rw-r--r--   0 kofi       (501) staff       (20)      172 2023-07-11 07:20:31.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper/utils/Ui/__init__.py
-drwxr-xr-x   0 kofi       (501) staff       (20)        0 2023-07-11 09:55:40.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper/utils/Ui/component/
--rw-r--r--   0 kofi       (501) staff       (20)     1472 2023-07-11 07:35:36.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper/utils/Ui/component/ListviewHelper.py
--rw-r--r--   0 kofi       (501) staff       (20)     3179 2023-07-11 08:22:39.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper/utils/Ui/component/TableHelper.py
--rw-r--r--   0 kofi       (501) staff       (20)     1124 2023-07-11 07:33:01.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper/utils/Ui/component/TreeHelper.py
--rw-r--r--   0 kofi       (501) staff       (20)     3002 2023-07-11 08:11:22.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper/utils/Ui/component/ValueHelper.py
--rw-r--r--   0 kofi       (501) staff       (20)      172 2023-07-11 07:27:10.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper/utils/Ui/component/__init__.py
--rw-r--r--   0 kofi       (501) staff       (20)     3186 2023-07-11 07:20:06.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper/utils/UiHelper.py
--rw-r--r--   0 kofi       (501) staff       (20)      171 2023-07-11 06:59:13.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper/utils/__init__.py
-drwxr-xr-x   0 kofi       (501) staff       (20)        0 2023-07-11 09:55:40.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper.egg-info/
--rw-r--r--   0 kofi       (501) staff       (20)      267 2023-07-11 09:55:40.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper.egg-info/PKG-INFO
--rw-r--r--   0 kofi       (501) staff       (20)     1475 2023-07-11 09:55:40.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper.egg-info/SOURCES.txt
--rw-r--r--   0 kofi       (501) staff       (20)        1 2023-07-11 09:55:40.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper.egg-info/dependency_links.txt
--rw-r--r--   0 kofi       (501) staff       (20)      134 2023-07-11 09:55:40.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper.egg-info/requires.txt
--rw-r--r--   0 kofi       (501) staff       (20)       15 2023-07-11 09:55:40.000000 KofiPyQtHelper-0.0.6/KofiPyQtHelper.egg-info/top_level.txt
--rw-r--r--   0 kofi       (501) staff       (20)      267 2023-07-11 09:55:40.000000 KofiPyQtHelper-0.0.6/PKG-INFO
--rw-r--r--   0 kofi       (501) staff       (20)      107 2023-07-11 09:01:08.000000 KofiPyQtHelper-0.0.6/README.md
--rw-r--r--   0 kofi       (501) staff       (20)       38 2023-07-11 09:55:40.000000 KofiPyQtHelper-0.0.6/setup.cfg
--rw-r--r--   0 kofi       (501) staff       (20)      892 2023-07-11 09:55:36.000000 KofiPyQtHelper-0.0.6/setup.py
+drwxr-xr-x   0 kofi       (501) staff       (20)        0 2023-07-11 15:21:23.000000 KofiPyQtHelper-0.0.7/
+drwxr-xr-x   0 kofi       (501) staff       (20)        0 2023-07-11 15:21:23.000000 KofiPyQtHelper-0.0.7/KofiPyQtHelper.egg-info/
+-rw-r--r--   0 kofi       (501) staff       (20)      267 2023-07-11 15:21:23.000000 KofiPyQtHelper-0.0.7/KofiPyQtHelper.egg-info/PKG-INFO
+-rw-r--r--   0 kofi       (501) staff       (20)      207 2023-07-11 15:21:23.000000 KofiPyQtHelper-0.0.7/KofiPyQtHelper.egg-info/SOURCES.txt
+-rw-r--r--   0 kofi       (501) staff       (20)        1 2023-07-11 15:21:23.000000 KofiPyQtHelper-0.0.7/KofiPyQtHelper.egg-info/dependency_links.txt
+-rw-r--r--   0 kofi       (501) staff       (20)      134 2023-07-11 15:21:23.000000 KofiPyQtHelper-0.0.7/KofiPyQtHelper.egg-info/requires.txt
+-rw-r--r--   0 kofi       (501) staff       (20)        1 2023-07-11 15:21:23.000000 KofiPyQtHelper-0.0.7/KofiPyQtHelper.egg-info/top_level.txt
+-rw-r--r--   0 kofi       (501) staff       (20)      267 2023-07-11 15:21:23.000000 KofiPyQtHelper-0.0.7/PKG-INFO
+-rw-r--r--   0 kofi       (501) staff       (20)      107 2023-07-11 09:01:08.000000 KofiPyQtHelper-0.0.7/README.md
+-rw-r--r--   0 kofi       (501) staff       (20)       38 2023-07-11 15:21:23.000000 KofiPyQtHelper-0.0.7/setup.cfg
+-rw-r--r--   0 kofi       (501) staff       (20)      881 2023-07-11 15:17:38.000000 KofiPyQtHelper-0.0.7/setup.py
```

### Comparing `KofiPyQtHelper-0.0.6/setup.py` & `KofiPyQtHelper-0.0.7/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 """
 Author       : Kofi
 Date         : 2023-07-11 16:54:03
 LastEditors  : Kofi
 LastEditTime : 2023-07-11 16:54:03
 Description  : 
 """
-
 from setuptools import setup, find_packages
 
+
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="KofiPyQtHelper",
-    version="0.0.6",
+    version="0.0.7",
     author="Kofi",
     author_email="aliwkxqq@163.com",
     description="PyQt 的快速布局工具",
     long_description=long_description,
     license="BSD License",
-    packages=find_packages(),
+    packages=[""],
     # data_files=[("Lib/site-packages/your-module-name", ["file"])],
     install_requires=[
         "Jinja2==3.1.2",
         "loguru==0.6.0",
         "matplotlib==3.5.3",
         "numpy==1.21.4",
         "pandas==1.3.4",
```

