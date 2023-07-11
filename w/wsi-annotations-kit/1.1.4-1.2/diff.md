# Comparing `tmp/wsi-annotations-kit-1.1.4.tar.gz` & `tmp/wsi-annotations-kit-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wsi-annotations-kit-1.1.4.tar", last modified: Wed May 24 19:15:40 2023, max compression
+gzip compressed data, was "dist\wsi-annotations-kit-1.2.tar", last modified: Tue Jul 11 14:45:27 2023, max compression
```

## Comparing `wsi-annotations-kit-1.1.4.tar` & `wsi-annotations-kit-1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 19:15:40.000000 wsi-annotations-kit-1.1.4/
--rw-rw-rw-   0        0        0     1086 2023-05-17 21:36:33.000000 wsi-annotations-kit-1.1.4/LICENSE
--rw-rw-rw-   0        0        0      745 2023-05-24 19:15:40.000000 wsi-annotations-kit-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-05-24 18:16:19.000000 wsi-annotations-kit-1.1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-24 19:15:40.000000 wsi-annotations-kit-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0      866 2023-05-24 19:14:41.000000 wsi-annotations-kit-1.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 19:15:40.000000 wsi-annotations-kit-1.1.4/wsi_annotations_kit/
--rw-rw-rw-   0        0        0        0 2023-05-17 21:25:38.000000 wsi-annotations-kit-1.1.4/wsi_annotations_kit/__init__.py
--rw-rw-rw-   0        0        0    21082 2023-05-19 18:42:29.000000 wsi-annotations-kit-1.1.4/wsi_annotations_kit/wsi_annotations_kit.py
-drwxrwxrwx   0        0        0        0 2023-05-24 19:15:40.000000 wsi-annotations-kit-1.1.4/wsi_annotations_kit.egg-info/
--rw-rw-rw-   0        0        0      745 2023-05-24 19:15:40.000000 wsi-annotations-kit-1.1.4/wsi_annotations_kit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-05-24 19:15:40.000000 wsi-annotations-kit-1.1.4/wsi_annotations_kit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 19:15:40.000000 wsi-annotations-kit-1.1.4/wsi_annotations_kit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-24 19:15:40.000000 wsi-annotations-kit-1.1.4/wsi_annotations_kit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-05-24 19:15:40.000000 wsi-annotations-kit-1.1.4/wsi_annotations_kit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 14:45:27.000000 wsi-annotations-kit-1.2/
+-rw-rw-rw-   0        0        0     1086 2023-05-17 21:36:33.000000 wsi-annotations-kit-1.2/LICENSE
+-rw-rw-rw-   0        0        0      743 2023-07-11 14:45:27.000000 wsi-annotations-kit-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-05-24 18:16:19.000000 wsi-annotations-kit-1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-11 14:45:27.000000 wsi-annotations-kit-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      864 2023-07-11 14:44:00.000000 wsi-annotations-kit-1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 14:45:27.000000 wsi-annotations-kit-1.2/wsi_annotations_kit/
+-rw-rw-rw-   0        0        0        0 2023-05-17 21:25:38.000000 wsi-annotations-kit-1.2/wsi_annotations_kit/__init__.py
+-rw-rw-rw-   0        0        0    21896 2023-07-11 14:43:21.000000 wsi-annotations-kit-1.2/wsi_annotations_kit/wsi_annotations_kit.py
+drwxrwxrwx   0        0        0        0 2023-07-11 14:45:27.000000 wsi-annotations-kit-1.2/wsi_annotations_kit.egg-info/
+-rw-rw-rw-   0        0        0      743 2023-07-11 14:45:26.000000 wsi-annotations-kit-1.2/wsi_annotations_kit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-07-11 14:45:26.000000 wsi-annotations-kit-1.2/wsi_annotations_kit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 14:45:26.000000 wsi-annotations-kit-1.2/wsi_annotations_kit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-07-11 14:45:26.000000 wsi-annotations-kit-1.2/wsi_annotations_kit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-11 14:45:26.000000 wsi-annotations-kit-1.2/wsi_annotations_kit.egg-info/top_level.txt
```

### Comparing `wsi-annotations-kit-1.1.4/LICENSE` & `wsi-annotations-kit-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wsi-annotations-kit-1.1.4/PKG-INFO` & `wsi-annotations-kit-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsi-annotations-kit
-Version: 1.1.4
+Version: 1.2
 Summary: Utility functions for generating, saving, and converting annotation files
 Home-page: https://github.com/spborder/wsi_annotations_kit
 Author: Sam Border
 Author-email: sam.border2256@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `wsi-annotations-kit-1.1.4/setup.py` & `wsi-annotations-kit-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="wsi-annotations-kit",
-    version="1.1.4",
+    version="1.2",
     author="Sam Border",
     author_email="sam.border2256@gmail.com",
     description="Utility functions for generating, saving, and converting annotation files",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/spborder/wsi_annotations_kit",
     install_requires=[
```

### Comparing `wsi-annotations-kit-1.1.4/wsi_annotations_kit/wsi_annotations_kit.py` & `wsi-annotations-kit-1.2/wsi_annotations_kit/wsi_annotations_kit.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,20 +22,22 @@
 
 
 class Object:
     def __init__(self,
                  shape_structure,
                  location,
                  structure_name,
-                 name):
+                 name,
+                 properties = None):
     
         self.poly = shape_structure
         self.crs = location
         self.structure = structure_name
         self.name = name
+        self.properties = properties
 
         # If not specified just pick something general
         if self.structure is None:
             self.structure = 'Structure'
         if self.name is None:
             self.name = uuid.uuid4().hex[:24]
 
@@ -131,15 +133,14 @@
                                                     'Y':str(pt[0]),
                                                     'Z':'0'})
         
         ET.SubElement(vertices,'Vertex',attrib={'X':str(scaled_poly_coords[0][1]),
                                                 'Y':str(scaled_poly_coords[0][0]),
                                                 'Z':'0'})
         
-    
 class GeoJSON:
     def __init__(self,
                  annotations,
                  verbose = True):
         
         self.annotations = annotations
 
@@ -166,19 +167,25 @@
         
         # Shifting object into global crs
         poly_coords = list(obj.poly.exterior.coords)
         scaled_poly_coords = [(int(i[0]+obj.crs[0]),int(i[1]+obj.crs[1])) for i in poly_coords]
 
         new_poly = Polygon(scaled_poly_coords)
 
-
-        self.geojson['features'].append(
-            Feature(geometry=new_poly,properties={'label':obj.name,'structure':obj.structure})
-        )
-    
+        if obj.properties is None:
+            self.geojson['features'].append(
+                Feature(geometry=new_poly,properties={'label':obj.name,'structure':obj.structure})
+            )
+        else:
+            prop_dict = obj.properties
+            prop_dict['label'] = obj.name
+            prop_dict['structure'] = obj.structure
+            self.geojson['features'].append(
+                Feature(geometry = new_poly, properties=prop_dict)
+            )    
 
 class Histomics:
     def __init__(self,
                annotations,
                verbose = True):
         
         self.annotations = annotations
@@ -208,24 +215,36 @@
 
         # Shifting object into global crs 
         poly_coords = list(obj.poly.exterior.coords)
         scaled_poly_coords = [(int(i[0]+obj.crs[0]),int(i[1]+obj.crs[1])) for i in poly_coords]
 
         new_poly = Polygon(scaled_poly_coords)
 
-        new_struct_dict = {
-            'type':'polyline',
-            'points':list(new_poly.exterior.coords),
-            'id':uuid.uuid4().hex[:24],
-            'closed':True,
-            'user': {
-                'name': obj.name,
-                'structure': obj.structure
+        if obj.properties is None:
+            new_struct_dict = {
+                'type':'polyline',
+                'points':[i+[0] for i in list(new_poly.exterior.coords)],
+                'id':uuid.uuid4().hex[:24],
+                'closed':True,
+                'user': {
+                    'name': obj.name,
+                    'structure': obj.structure
+                }
+            }
+        else:
+            prop_dict = obj.properties
+            prop_dict['name'] = obj.name
+            prop_dict['structure'] = obj.structure
+            new_struct_dict = {
+                'type':'polyline',
+                'points':[i+[0] for i in list(new_poly.exterior.coords)],
+                'id':uuid.uuid4().hex[:24],
+                'closed':True,
+                'user': prop_dict
             }
-        }
 
         return new_struct_dict
 
 
 class Annotation:
     def __init__(self,
                  mpp = None,
@@ -236,19 +255,17 @@
 
         self.mpp = mpp
         self.min_size = min_size
     
     def __str__(self):
         
         if len(list(self.objects.keys()))==0:
-            print('Empty annotation object')
+            return 'Empty annotation object'
         else:
-            print(f'Annotation object containing: {len(list(self.objects.keys()))}')
-            for n in self.objects:
-                print(f'{n}: {len(self.objects[n])}')
+            return f'Annotation object containing: {len(list(self.objects.keys()))}'
 
     def add_shape(self, poly, box_crs, structure = None, name = None):
         
         # poly = shapely polygon or other geometry
         # box_crs = upper left corner for location that this object is in 
         # structure = structure name (which structure is this in general)
         # name = shape name (individual object name)
```

### Comparing `wsi-annotations-kit-1.1.4/wsi_annotations_kit.egg-info/PKG-INFO` & `wsi-annotations-kit-1.2/wsi_annotations_kit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wsi-annotations-kit
-Version: 1.1.4
+Version: 1.2
 Summary: Utility functions for generating, saving, and converting annotation files
 Home-page: https://github.com/spborder/wsi_annotations_kit
 Author: Sam Border
 Author-email: sam.border2256@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

