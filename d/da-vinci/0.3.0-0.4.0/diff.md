# Comparing `tmp/da-vinci-0.3.0.tar.gz` & `tmp/da-vinci-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/da-vinci-0.3.0.tar", last modified: Wed Oct 21 02:49:58 2020, max compression
+gzip compressed data, was "da-vinci-0.4.0.tar", last modified: Tue Jul 11 13:36:40 2023, max compression
```

## Comparing `da-vinci-0.3.0.tar` & `da-vinci-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2020-10-21 02:49:58.000000 da-vinci-0.3.0/
--rw-r--r--   0 selwin     (501) staff       (20)     2614 2020-10-21 02:49:58.000000 da-vinci-0.3.0/PKG-INFO
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2020-10-21 02:49:58.000000 da-vinci-0.3.0/da_vinci/
--rw-r--r--   0 selwin     (501) staff       (20)      383 2020-10-21 02:44:33.000000 da-vinci-0.3.0/da_vinci/compat.py
--rw-r--r--   0 selwin     (501) staff       (20)       46 2020-10-21 02:45:53.000000 da-vinci-0.3.0/da_vinci/__init__.py
--rw-r--r--   0 selwin     (501) staff       (20)     2728 2020-10-21 02:44:33.000000 da-vinci-0.3.0/da_vinci/utils.py
--rw-r--r--   0 selwin     (501) staff       (20)      363 2020-10-21 02:44:33.000000 da-vinci-0.3.0/da_vinci/formats.py
--rw-r--r--   0 selwin     (501) staff       (20)     6945 2020-10-21 02:44:33.000000 da-vinci-0.3.0/da_vinci/images.py
--rw-r--r--   0 selwin     (501) staff       (20)     1095 2020-10-21 02:46:33.000000 da-vinci-0.3.0/setup.py
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2020-10-21 02:49:58.000000 da-vinci-0.3.0/da_vinci.egg-info/
--rw-r--r--   0 selwin     (501) staff       (20)     2614 2020-10-21 02:49:58.000000 da-vinci-0.3.0/da_vinci.egg-info/PKG-INFO
--rw-r--r--   0 selwin     (501) staff       (20)        1 2020-10-21 02:49:58.000000 da-vinci-0.3.0/da_vinci.egg-info/not-zip-safe
--rw-r--r--   0 selwin     (501) staff       (20)      275 2020-10-21 02:49:58.000000 da-vinci-0.3.0/da_vinci.egg-info/SOURCES.txt
--rw-r--r--   0 selwin     (501) staff       (20)        9 2020-10-21 02:49:58.000000 da-vinci-0.3.0/da_vinci.egg-info/top_level.txt
--rw-r--r--   0 selwin     (501) staff       (20)        1 2020-10-21 02:49:58.000000 da-vinci-0.3.0/da_vinci.egg-info/dependency_links.txt
--rw-r--r--   0 selwin     (501) staff       (20)       38 2020-10-21 02:49:58.000000 da-vinci-0.3.0/setup.cfg
--rw-r--r--   0 selwin     (501) staff       (20)     1336 2020-10-21 02:45:48.000000 da-vinci-0.3.0/README.rst
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-07-11 13:36:40.925344 da-vinci-0.4.0/
+-rw-r--r--   0 selwin     (501) staff       (20)     2434 2023-07-11 13:36:40.925252 da-vinci-0.4.0/PKG-INFO
+-rw-r--r--   0 selwin     (501) staff       (20)     1428 2023-07-11 13:35:28.000000 da-vinci-0.4.0/README.rst
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-07-11 13:36:40.924596 da-vinci-0.4.0/da_vinci/
+-rw-r--r--   0 selwin     (501) staff       (20)       46 2023-07-11 13:35:44.000000 da-vinci-0.4.0/da_vinci/__init__.py
+-rw-r--r--   0 selwin     (501) staff       (20)      383 2020-10-21 02:44:33.000000 da-vinci-0.4.0/da_vinci/compat.py
+-rw-r--r--   0 selwin     (501) staff       (20)      363 2020-10-21 02:44:33.000000 da-vinci-0.4.0/da_vinci/formats.py
+-rw-r--r--   0 selwin     (501) staff       (20)     7189 2023-07-11 13:32:21.000000 da-vinci-0.4.0/da_vinci/images.py
+-rw-r--r--   0 selwin     (501) staff       (20)     2728 2020-10-21 02:44:33.000000 da-vinci-0.4.0/da_vinci/utils.py
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-07-11 13:36:40.925120 da-vinci-0.4.0/da_vinci.egg-info/
+-rw-r--r--   0 selwin     (501) staff       (20)     2434 2023-07-11 13:36:40.000000 da-vinci-0.4.0/da_vinci.egg-info/PKG-INFO
+-rw-r--r--   0 selwin     (501) staff       (20)      275 2023-07-11 13:36:40.000000 da-vinci-0.4.0/da_vinci.egg-info/SOURCES.txt
+-rw-r--r--   0 selwin     (501) staff       (20)        1 2023-07-11 13:36:40.000000 da-vinci-0.4.0/da_vinci.egg-info/dependency_links.txt
+-rw-r--r--   0 selwin     (501) staff       (20)        1 2020-10-21 02:49:58.000000 da-vinci-0.4.0/da_vinci.egg-info/not-zip-safe
+-rw-r--r--   0 selwin     (501) staff       (20)        9 2023-07-11 13:36:40.000000 da-vinci-0.4.0/da_vinci.egg-info/top_level.txt
+-rw-r--r--   0 selwin     (501) staff       (20)       38 2023-07-11 13:36:40.925372 da-vinci-0.4.0/setup.cfg
+-rw-r--r--   0 selwin     (501) staff       (20)     1258 2023-07-11 13:34:21.000000 da-vinci-0.4.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `da-vinci-0.3.0/PKG-INFO` & `da-vinci-0.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,73 +1,81 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: da-vinci
-Version: 0.3.0
+Version: 0.4.0
 Summary: A simple image manipulation library aiming to make common image tasks easy.
 Home-page: https://github.com/ui/da-vinci
 Author: Selwin Ong
 Author-email: selwin.ong@gmail.com
 License: MIT
-Description: A simple image manipulation library aiming to make common image/photo
-        manipulation tasks easy. This library is still under development,
-        API may also change at any time.
-        
-        Requires PIL/Pillow.
-        
-        Example usage::
-        
-            from da_vinci import Image
-        
-            image = Image('lena.jpg')
-            image.flip('horizontal')
-            image.resize(width=10, height=10)
-            image.save()
-        
-            # Opening an image from URL, rotating and change it's format
-            image = Image('http://stamps.co.id/static/merchants/img/logo.png')
-            image.rotate(degrees=90)
-            image.set(format='jpg', quality=85)
-            image.save() # Creates a file logo.jpg
-        
-            # Manipulating saturation, brightness, contrast and sharpness
-            # Accepts values range from -100 (decrease) to 100 (increase)
-            image.adjust(saturation=-100)
-            image.adjust(brightness=-75, contrast=50, sharpness=-20)
-        
-        
-        If you need more extensive manipulation, an escape hatch to PIL
-        is also available::
-        
-            image = image.from_file('a.jpg')
-            pil_image = image.get_pil_image()
-            # Do whatever you need to do with the pil image
-            # And if you want to convert this back to a da_vinci image
-            image.set_pil_image(pil_image)
-        
-        Tests
-        
-        To run tests::
-        
-            python -m unittest tests
-        
-        Changelog
-        ---------
-        
-        Version 0.3.0
-        =============
-        * Added webp extension support
-        
-        Version 0.2.2
-        =============
-        * Added bmp extension support
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Multimedia :: Graphics
+
+A simple image manipulation library aiming to make common image/photo
+manipulation tasks easy. This library is still under development,
+API may also change at any time.
+
+Requires PIL/Pillow.
+
+Example usage::
+
+    from da_vinci import Image
+
+    image = Image('lena.jpg')
+    image.flip('horizontal')
+    image.resize(width=10, height=10)
+    image.save()
+
+    # Opening an image from URL, rotating and change it's format
+    image = Image('http://stamps.co.id/static/merchants/img/logo.png')
+    image.rotate(degrees=90)
+    image.set(format='jpg', quality=85)
+    image.save() # Creates a file logo.jpg
+
+    # Manipulating saturation, brightness, contrast and sharpness
+    # Accepts values range from -100 (decrease) to 100 (increase)
+    image.adjust(saturation=-100)
+    image.adjust(brightness=-75, contrast=50, sharpness=-20)
+
+
+If you need more extensive manipulation, an escape hatch to PIL
+is also available::
+
+    image = image.from_file('a.jpg')
+    pil_image = image.get_pil_image()
+    # Do whatever you need to do with the pil image
+    # And if you want to convert this back to a da_vinci image
+    image.set_pil_image(pil_image)
+
+Tests
+
+To run tests::
+
+    python -m unittest tests
+
+Changelog
+---------
+
+Version 0.4.0
+=============
+* Support Pillow 10
+* Preserve EXIF data when image is rotated
+
+Version 0.3.0
+=============
+* Added webp extension support
+
+Version 0.2.2
+=============
+* Added bmp extension support
```

### Comparing `da-vinci-0.3.0/da_vinci/utils.py` & `da-vinci-0.4.0/da_vinci/utils.py`

 * *Files identical despite different names*

### Comparing `da-vinci-0.3.0/da_vinci/images.py` & `da-vinci-0.4.0/da_vinci/images.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import division
 
 import io
 import os
 
 from PIL import Image as PILImage
-from PIL import ImageEnhance
+from PIL import ImageEnhance, ImageOps
 
 from . import formats
 from .compat import string_types, urlopen, urlparse
 from .utils import (calculate_dimensions, convert_to_pil_factor,
                     get_box_dimensions, parse_dimension)
 
 
@@ -28,18 +28,19 @@
         if result is not None and result.scheme in ('http', 'https'):
             file = io.BytesIO(urlopen(path_or_url).read())
             self._pil_image = PILImage.open(file)
             self.filename = None
             self.name = os.path.basename(path_or_url)
         else:
             self._pil_image = PILImage.open(path_or_url)
-            self.filename = self._pil_image.filename
+            self.filename = self._pil_image.filename if self._pil_image.filename else path_or_url.name
             self.name = os.path.basename(self.filename)
 
         self._format = self._pil_image.format
+        self._pil_image = ImageOps.exif_transpose(self._pil_image)
         self._quality = None
 
     @property
     def width(self):
         return self._pil_image.size[0]
 
     @property
@@ -142,18 +143,23 @@
           regardless of aspect ratio
         - "fit" resizes image to the largest size such that both its width
           and height fit inside the specified dimension, keeps aspect ratio.
         - "fill" resizes image to be as large as possible so that the specified
           dimension is completely covered. Aspect ratio is preserved, parts of
           the image may not be within the specified dimension.
         """
+        try:
+            resample = PILImage.ANTIALIAS
+        except AttributeError:
+            resample = PILImage.LANCZOS
+
         self._pil_image = self._pil_image.resize(
             calculate_dimensions(width, height, self.width, self.height,
                                  method=method),
-            resample=PILImage.ANTIALIAS
+            resample=resample
         )
 
     def crop(self, width, height, center=('50%', '50%'),
              shape='rectangle'):
         center = (
             parse_dimension(center[0], self.width),
             parse_dimension(center[1], self.height)
```

### Comparing `da-vinci-0.3.0/setup.py` & `da-vinci-0.4.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 setup(
     name='da-vinci',
-    version='0.3.0',
+    version='0.4.0',
     author='Selwin Ong',
     author_email='selwin.ong@gmail.com',
     packages=['da_vinci'],
     url='https://github.com/ui/da-vinci',
     license='MIT',
     description='A simple image manipulation library aiming to make common image tasks easy.',
     long_description=open('README.rst').read(),
     zip_safe=False,
     include_package_data=True,
     package_data={'': ['README.rst']},
     classifiers=[
-        'Development Status :: 3 - Alpha',
+        "Development Status :: 5 - Production/Stable",
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Topic :: Multimedia :: Graphics'
     ]
 )
```

### Comparing `da-vinci-0.3.0/da_vinci.egg-info/PKG-INFO` & `da-vinci-0.4.0/da_vinci.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,73 +1,81 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: da-vinci
-Version: 0.3.0
+Version: 0.4.0
 Summary: A simple image manipulation library aiming to make common image tasks easy.
 Home-page: https://github.com/ui/da-vinci
 Author: Selwin Ong
 Author-email: selwin.ong@gmail.com
 License: MIT
-Description: A simple image manipulation library aiming to make common image/photo
-        manipulation tasks easy. This library is still under development,
-        API may also change at any time.
-        
-        Requires PIL/Pillow.
-        
-        Example usage::
-        
-            from da_vinci import Image
-        
-            image = Image('lena.jpg')
-            image.flip('horizontal')
-            image.resize(width=10, height=10)
-            image.save()
-        
-            # Opening an image from URL, rotating and change it's format
-            image = Image('http://stamps.co.id/static/merchants/img/logo.png')
-            image.rotate(degrees=90)
-            image.set(format='jpg', quality=85)
-            image.save() # Creates a file logo.jpg
-        
-            # Manipulating saturation, brightness, contrast and sharpness
-            # Accepts values range from -100 (decrease) to 100 (increase)
-            image.adjust(saturation=-100)
-            image.adjust(brightness=-75, contrast=50, sharpness=-20)
-        
-        
-        If you need more extensive manipulation, an escape hatch to PIL
-        is also available::
-        
-            image = image.from_file('a.jpg')
-            pil_image = image.get_pil_image()
-            # Do whatever you need to do with the pil image
-            # And if you want to convert this back to a da_vinci image
-            image.set_pil_image(pil_image)
-        
-        Tests
-        
-        To run tests::
-        
-            python -m unittest tests
-        
-        Changelog
-        ---------
-        
-        Version 0.3.0
-        =============
-        * Added webp extension support
-        
-        Version 0.2.2
-        =============
-        * Added bmp extension support
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Multimedia :: Graphics
+
+A simple image manipulation library aiming to make common image/photo
+manipulation tasks easy. This library is still under development,
+API may also change at any time.
+
+Requires PIL/Pillow.
+
+Example usage::
+
+    from da_vinci import Image
+
+    image = Image('lena.jpg')
+    image.flip('horizontal')
+    image.resize(width=10, height=10)
+    image.save()
+
+    # Opening an image from URL, rotating and change it's format
+    image = Image('http://stamps.co.id/static/merchants/img/logo.png')
+    image.rotate(degrees=90)
+    image.set(format='jpg', quality=85)
+    image.save() # Creates a file logo.jpg
+
+    # Manipulating saturation, brightness, contrast and sharpness
+    # Accepts values range from -100 (decrease) to 100 (increase)
+    image.adjust(saturation=-100)
+    image.adjust(brightness=-75, contrast=50, sharpness=-20)
+
+
+If you need more extensive manipulation, an escape hatch to PIL
+is also available::
+
+    image = image.from_file('a.jpg')
+    pil_image = image.get_pil_image()
+    # Do whatever you need to do with the pil image
+    # And if you want to convert this back to a da_vinci image
+    image.set_pil_image(pil_image)
+
+Tests
+
+To run tests::
+
+    python -m unittest tests
+
+Changelog
+---------
+
+Version 0.4.0
+=============
+* Support Pillow 10
+* Preserve EXIF data when image is rotated
+
+Version 0.3.0
+=============
+* Added webp extension support
+
+Version 0.2.2
+=============
+* Added bmp extension support
```

### Comparing `da-vinci-0.3.0/README.rst` & `da-vinci-0.4.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,19 @@
 To run tests::
 
     python -m unittest tests
 
 Changelog
 ---------
 
+Version 0.4.0
+=============
+* Support Pillow 10
+* Preserve EXIF data when image is rotated
+
 Version 0.3.0
 =============
 * Added webp extension support
 
 Version 0.2.2
 =============
 * Added bmp extension support
```

