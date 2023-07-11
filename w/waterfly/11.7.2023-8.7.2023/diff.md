# Comparing `tmp/waterfly-11.7.2023.tar.gz` & `tmp/waterfly-8.7.2023.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waterfly-11.7.2023.tar", last modified: Tue Jul 11 18:00:59 2023, max compression
+gzip compressed data, was "waterfly-8.7.2023.tar", last modified: Sat Jul  8 18:40:09 2023, max compression
```

## Comparing `waterfly-11.7.2023.tar` & `waterfly-8.7.2023.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 18:00:59.329835 waterfly-11.7.2023/
--rw-rw-rw-   0        0        0     2902 2023-07-11 18:00:59.329835 waterfly-11.7.2023/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-11 18:00:59.329835 waterfly-11.7.2023/setup.cfg
--rw-rw-rw-   0        0        0     3166 2023-07-11 17:53:05.000000 waterfly-11.7.2023/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 18:00:59.282974 waterfly-11.7.2023/waterfly/
--rw-rw-rw-   0        0        0    29541 2023-07-11 17:54:49.000000 waterfly-11.7.2023/waterfly/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 18:00:59.314215 waterfly-11.7.2023/waterfly.egg-info/
--rw-rw-rw-   0        0        0     2902 2023-07-11 18:00:59.000000 waterfly-11.7.2023/waterfly.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-07-11 18:00:59.000000 waterfly-11.7.2023/waterfly.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 18:00:59.000000 waterfly-11.7.2023/waterfly.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-07-11 18:00:59.000000 waterfly-11.7.2023/waterfly.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-11 18:00:59.000000 waterfly-11.7.2023/waterfly.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 18:40:09.640290 waterfly-8.7.2023/
+-rw-rw-rw-   0        0        0     1822 2023-07-08 18:40:09.640290 waterfly-8.7.2023/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-08 18:40:09.640290 waterfly-8.7.2023/setup.cfg
+-rw-rw-rw-   0        0        0     2173 2023-07-08 18:34:35.000000 waterfly-8.7.2023/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 18:40:09.593429 waterfly-8.7.2023/waterfly/
+-rw-rw-rw-   0        0        0     7887 2023-07-08 17:40:07.000000 waterfly-8.7.2023/waterfly/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 18:40:09.640290 waterfly-8.7.2023/waterfly.egg-info/
+-rw-rw-rw-   0        0        0     1822 2023-07-08 18:40:09.000000 waterfly-8.7.2023/waterfly.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-07-08 18:40:09.000000 waterfly-8.7.2023/waterfly.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 18:40:09.000000 waterfly-8.7.2023/waterfly.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-07-08 18:40:09.000000 waterfly-8.7.2023/waterfly.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-08 18:40:09.000000 waterfly-8.7.2023/waterfly.egg-info/top_level.txt
```

### Comparing `waterfly-11.7.2023/PKG-INFO` & `waterfly-8.7.2023/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,18 @@
 Metadata-Version: 2.1
 Name: waterfly
-Version: 11.7.2023
-Summary: Waterfly is a powerful new AI tool to create Firefly URLs, process images, and draw on images.
+Version: 8.7.2023
+Summary: Waterfly is a powerful new AI tool
 Author: Igor_Shapovalov_Andrejovich
 Author-email: igor.shapovalov.andrejovich@gmail.com
 
 
 
 Hi here!
 
-–––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––
-
-                                              ABOUT NEW
-
-— The code was rewritten from scratch to make it easier to read
-
-— A vulnerability has been discovered in Adobe Firefly, you can upload images without a watermark!
-  Check the element code and find the img tag with alt="Variation n of 4",
-  follow the link in the src and upload the image with the PNG or JPG extension
-
-–––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––
-
 Create URLs for images and text styles, for example:
 create.image('Chocolate tree', ['hyper_realistic', 'cool_colors', 'studio_light'], 'portrait')
 Create a great photo of a chocolate tree for your Instagram stories with very realistic graphics,
 beautiful colors, and studio lighting.
 Not interested in stories? Create something else! Example:
 create.image('Sakura tree', ['cartoon', 'beautiful', 'pastel_colors', dramatic_light'], 'widescreen')
 Creates a beautifully drawn picture of a sakura tree, in cartoon style, beautiful,
@@ -32,15 +20,15 @@
 with an aspect ratio that is ideal for desktop backgrounds
 
 –––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––
 
 Already have the image you need? Edit it!
 
 The code that will remove the background:
-edit.backdrop('image.img', 'backdrop.img')
+edit.backdrop('image.img')
 You can add a vignette like this:
 edit.vignette('image.img', level)
 Turn the image into a cartoon:
 edit.cartoon('image.img')
 
 –––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––
```

### Comparing `waterfly-11.7.2023/setup.py` & `waterfly-8.7.2023/waterfly.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,17 @@
-from setuptools import setup
+Metadata-Version: 2.1
+Name: waterfly
+Version: 8.7.2023
+Summary: Waterfly is a powerful new AI tool
+Author: Igor_Shapovalov_Andrejovich
+Author-email: igor.shapovalov.andrejovich@gmail.com
 
-setup(
-    name='waterfly',
-    version='11.7.2023',
-    install_requires=[
-        'googletrans>=3.1.0a0',
-        'opencv-python',
-        'rembg',
-        'requests',
-        'pyautogui'
-    ],
-    description='Waterfly is a powerful new AI tool to create Firefly URLs, process images, and draw on images.',
-    long_description='''
 
-Hi here!
-
-–––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––
-
-                                              ABOUT NEW
 
-— The code was rewritten from scratch to make it easier to read
-
-— A vulnerability has been discovered in Adobe Firefly, you can upload images without a watermark!
-  Check the element code and find the img tag with alt="Variation n of 4",
-  follow the link in the src and upload the image with the PNG or JPG extension
-
-–––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––
+Hi here!
 
 Create URLs for images and text styles, for example:
 create.image('Chocolate tree', ['hyper_realistic', 'cool_colors', 'studio_light'], 'portrait')
 Create a great photo of a chocolate tree for your Instagram stories with very realistic graphics,
 beautiful colors, and studio lighting.
 Not interested in stories? Create something else! Example:
 create.image('Sakura tree', ['cartoon', 'beautiful', 'pastel_colors', dramatic_light'], 'widescreen')
@@ -38,25 +20,20 @@
 with an aspect ratio that is ideal for desktop backgrounds
 
 –––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––
 
 Already have the image you need? Edit it!
 
 The code that will remove the background:
-edit.backdrop('image.img', 'backdrop.img')
+edit.backdrop('image.img')
 You can add a vignette like this:
 edit.vignette('image.img', level)
 Turn the image into a cartoon:
 edit.cartoon('image.img')
 
 –––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––
 
 Want to point out something in an image?
 Build any shape with lines and ellipses!
 
 And much more...
 
-''',
-    author = 'Igor_Shapovalov_Andrejovich',
-    packages = ['waterfly'],
-    author_email = 'igor.shapovalov.andrejovich@gmail.com'
-)
```

### Comparing `waterfly-11.7.2023/waterfly.egg-info/PKG-INFO` & `waterfly-8.7.2023/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,24 @@
-Metadata-Version: 2.1
-Name: waterfly
-Version: 11.7.2023
-Summary: Waterfly is a powerful new AI tool to create Firefly URLs, process images, and draw on images.
-Author: Igor_Shapovalov_Andrejovich
-Author-email: igor.shapovalov.andrejovich@gmail.com
-
+from setuptools import setup
 
+setup(
+    name='waterfly',
+    version='8.7.2023',
+    install_requires=[
+        'googletrans>=3.1.0a0',
+        'opencv-python',
+        'rembg'
+    ],
+    description='''Waterfly is a powerful new AI tool
+that reserves as partly an unofficial client for Adobe Firefly,
+to create Firefly URLs, process images, and draw on images.''',
+    long_description='''
 
 Hi here!
 
-–––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––
-
-                                              ABOUT NEW
-
-— The code was rewritten from scratch to make it easier to read
-
-— A vulnerability has been discovered in Adobe Firefly, you can upload images without a watermark!
-  Check the element code and find the img tag with alt="Variation n of 4",
-  follow the link in the src and upload the image with the PNG or JPG extension
-
-–––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––
-
 Create URLs for images and text styles, for example:
 create.image('Chocolate tree', ['hyper_realistic', 'cool_colors', 'studio_light'], 'portrait')
 Create a great photo of a chocolate tree for your Instagram stories with very realistic graphics,
 beautiful colors, and studio lighting.
 Not interested in stories? Create something else! Example:
 create.image('Sakura tree', ['cartoon', 'beautiful', 'pastel_colors', dramatic_light'], 'widescreen')
 Creates a beautifully drawn picture of a sakura tree, in cartoon style, beautiful,
@@ -32,20 +26,25 @@
 with an aspect ratio that is ideal for desktop backgrounds
 
 –––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––
 
 Already have the image you need? Edit it!
 
 The code that will remove the background:
-edit.backdrop('image.img', 'backdrop.img')
+edit.backdrop('image.img')
 You can add a vignette like this:
 edit.vignette('image.img', level)
 Turn the image into a cartoon:
 edit.cartoon('image.img')
 
 –––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––––
 
 Want to point out something in an image?
 Build any shape with lines and ellipses!
 
 And much more...
 
+''',
+    author = 'Igor_Shapovalov_Andrejovich',
+    packages = ['waterfly'],
+    author_email = 'igor.shapovalov.andrejovich@gmail.com'
+)
```

