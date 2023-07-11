# Comparing `tmp/gispandas-0.1.6.tar.gz` & `tmp/gispandas-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gispandas-0.1.6.tar", last modified: Mon Jul  3 12:45:32 2023, max compression
+gzip compressed data, was "gispandas-0.1.7.tar", last modified: Tue Jul 11 13:42:10 2023, max compression
```

## Comparing `gispandas-0.1.6.tar` & `gispandas-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 12:45:32.715837 gispandas-0.1.6/
--rw-rw-rw-   0        0        0     1027 2023-07-03 12:45:32.715837 gispandas-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      737 2023-07-03 09:54:38.000000 gispandas-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 12:45:32.706862 gispandas-0.1.6/gispandas/
--rw-rw-rw-   0        0        0       31 2023-07-03 12:41:13.000000 gispandas-0.1.6/gispandas/__init__.py
--rw-rw-rw-   0        0        0     2652 2023-06-29 06:54:45.000000 gispandas-0.1.6/gispandas/gispandas.py
-drwxrwxrwx   0        0        0        0 2023-07-03 12:45:32.713842 gispandas-0.1.6/gispandas.egg-info/
--rw-rw-rw-   0        0        0     1027 2023-07-03 12:45:32.000000 gispandas-0.1.6/gispandas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-07-03 12:45:32.000000 gispandas-0.1.6/gispandas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 12:45:32.000000 gispandas-0.1.6/gispandas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-03 12:45:32.000000 gispandas-0.1.6/gispandas.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-07-03 12:45:32.000000 gispandas-0.1.6/gispandas.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 12:45:32.715837 gispandas-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      863 2023-07-03 12:43:04.000000 gispandas-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 13:42:10.708968 gispandas-0.1.7/
+-rw-rw-rw-   0        0        0     1204 2023-07-11 13:42:10.707971 gispandas-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      909 2023-07-11 13:32:05.000000 gispandas-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 13:42:10.696003 gispandas-0.1.7/gispandas/
+-rw-rw-rw-   0        0        0      366 2023-07-11 13:17:54.000000 gispandas-0.1.7/gispandas/__init__.py
+-rw-rw-rw-   0        0        0    11760 2023-07-11 13:09:28.000000 gispandas-0.1.7/gispandas/gago_gdal.py
+-rw-rw-rw-   0        0        0     2056 2023-07-11 13:36:06.000000 gispandas-0.1.7/gispandas/geemerge.py
+-rw-rw-rw-   0        0        0     3326 2023-07-11 13:35:49.000000 gispandas-0.1.7/gispandas/mxgdal.py
+-rw-rw-rw-   0        0        0     2561 2023-07-11 12:53:22.000000 gispandas-0.1.7/gispandas/shpinfo.py
+-rw-rw-rw-   0        0        0     3280 2023-07-11 13:02:48.000000 gispandas-0.1.7/gispandas/tifarea.py
+-rw-rw-rw-   0        0        0     1642 2023-07-11 13:35:08.000000 gispandas-0.1.7/gispandas/tifchange.py
+drwxrwxrwx   0        0        0        0 2023-07-11 13:42:10.705977 gispandas-0.1.7/gispandas.egg-info/
+-rw-rw-rw-   0        0        0     1204 2023-07-11 13:42:10.000000 gispandas-0.1.7/gispandas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      365 2023-07-11 13:42:10.000000 gispandas-0.1.7/gispandas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 13:42:10.000000 gispandas-0.1.7/gispandas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-11 13:42:10.000000 gispandas-0.1.7/gispandas.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2023-07-11 13:42:10.000000 gispandas-0.1.7/gispandas.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 13:42:10.708968 gispandas-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      870 2023-07-11 13:41:16.000000 gispandas-0.1.7/setup.py
```

### Comparing `gispandas-0.1.6/PKG-INFO` & `gispandas-0.1.7/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,15 @@
-Metadata-Version: 2.1
-Name: gispandas
-Version: 0.1.6
-Summary: gispandas
-Home-page: https://github.com/mxhou/gispandas/
-Author: HMX
-Author-email: kzdhb8023@163.com
-License: MIT
-Keywords: gis,geo,tif,json
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
-# GisPandas针对栅格数据进行统计的python包
-GisPandas是一个为栅格数据处理、分析和可视化而开发的Python包。GisPandas为常见栅格数据进行行政区划统计提供了快速而简洁的方法。GisPandas为遥感影像分类的后处理过程提供高效的处理，代码简洁、高效、灵活、易用，可以用简洁的代码实现复杂的数据任务。
-# 主要功能
-目前，GisPandas主要提供以下方法：
-栅格数据进行阿尔伯斯等面积投影，根据矢量区划会计算面积导出json。
-# 安装
-pip install gispandas
-# 相关链接
-本项目的github页面：https://github.com/mxhou/gispandas
-
-有bug请在这个页面提交：https://github.com/mxhou/gispandas/issues
+# GisPandas针对栅格数据进行统计的python包
+GisPandas是一个为栅格、矢量数据处理、分析以及可视化而开发的Python包。GisPandas为常见栅格矢量数据提供了快速而简洁的gis操作方法，代码简洁、高效、灵活、易用，可以用简洁的代码实现复杂的数据任务。
+# 主要功能
+目前，GisPandas主要提供以下方法：
+1.栅格数据进行阿尔伯斯等面积投影，根据矢量区划计算面积并导出json。
+2.种植结构变化。
+3.gee栅格数据镶嵌并压缩。
+4.矢量数据写入四至、置信等属性，矢量简化，文本矢量化等。
+5.栅格数据像素对齐、裁剪、重采样、投影、插值、切片、格式转换等。
+# 安装
+pip install gispandas
+# 相关链接
+本项目的github页面：https://github.com/mxhou/gispandas
+
+有bug请在这个页面提交：https://github.com/mxhou/gispandas/issues
```

### Comparing `gispandas-0.1.6/gispandas/gispandas.py` & `gispandas-0.1.7/gispandas/tifarea.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- encoding: utf-8 -*-
 '''
-@File    :   tif2json.py
+@File    :   tifarea.py
 @Time    :   2023/03/31 16:04:48
 @Author  :   HMX
 @Version :   1.0
 @Contact :   kzdhb8023@163.com
 '''
 
 # here put the import lib
@@ -16,17 +16,27 @@
 import rasterio
 import rasterio.mask
 from rasterio.warp import Resampling, calculate_default_transform, reproject
 from rasterstats import zonal_stats
 
 
 def tif2area(intif,inshp,class_dic,outjson,resolution=10,year=time.strftime('%Y'),code = 'code',name = 'name'):
+    '''根据矢量区划统计tif数据的面积
 
+    :param intif: 待统计的栅格数据
+    :param inshp: 待统计的矢量区划
+    :param class_dic: 作物类别和栅格像元值
+    :param outjson: 输出的统计json文件,注意导出的area单位默认为亩
+    :param resolution: 分辨率, defaults to 10
+    :param year: 数据年份, defaults to time.strftime('%Y')
+    :param code: 矢量数据里行政区划代码的字段名称, defaults to 'code'
+    :param name: 矢量数据里行政区划名称的字段名称, defaults to 'name'
+    :return: 输出的统计json文件
+    '''
     # 投影
-
     # 投影矢量
     dst_crs = '+proj=aea +lat_1=25 +lat_2=47 +lat_0=0 +lon_0=105 +x_0=0 +y_0=0 +datum=WGS84 +units=m +no_defs'
     gdf = gpd.read_file(inshp)
     gdf.to_crs(dst_crs,inplace=True)
 
     # 投影栅格
     with rasterio.open(intif) as src:
@@ -50,15 +60,15 @@
             src_crs=src.crs,
             dst_transform=dst_transform,
             dst_crs=dst_crs,
             resampling=Resampling.nearest
         )
 
     # 空间统计
-    dx_re, dy_re = 10,10
+    dx_re, dy_re = resolution,resolution
     ks = list(class_dic.keys())
     vs = list(class_dic.values())
     stats = zonal_stats(gdf, dst_arr
     , stats=" mean count"
     , nodata=src.nodata
     , categorical=True
     , category_map=class_dic
```

### Comparing `gispandas-0.1.6/setup.py` & `gispandas-0.1.7/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 filepath = path.join(this_directory, 'README.md')
-VERSION = '0.1.6'
+VERSION = '0.1.7'
 setup(
     name='gispandas',  # package name
     version=VERSION,  # package version
     author="HMX",
     author_email="kzdhb8023@163.com",
     description='gispandas',  # package description
     packages=find_packages(),
     url="https://github.com/mxhou/gispandas/",
     zip_safe=False,
     # What packages are required for this module to be executed?
-    REQUIRED = ['geopandas', 'numpy','json','rasterio','rasterstats'],
+    REQUIRED = ['geopandas', 'numpy','json','rasterio','rasterstats','gdal'],
     license='MIT',
     python_requires=">=3.6",
     keywords=['gis','geo','tif','json'],
     data_files=[filepath],
     long_description=open(filepath, encoding='utf-8').read(),
     long_description_content_type='text/markdown'
 )
```

