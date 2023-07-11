# Comparing `tmp/django-lazy-srcset-0.2.2.tar.gz` & `tmp/django-lazy-srcset-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-lazy-srcset-0.2.2.tar", last modified: Thu Jul  6 22:44:29 2023, max compression
+gzip compressed data, was "django-lazy-srcset-1.0.0.tar", last modified: Tue Jul 11 16:16:16 2023, max compression
```

## Comparing `django-lazy-srcset-0.2.2.tar` & `django-lazy-srcset-1.0.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-06 22:44:29.530314 django-lazy-srcset-0.2.2/
--rw-r--r--   0 quantra    (501) staff       (20)     1076 2023-05-02 22:05:05.000000 django-lazy-srcset-0.2.2/LICENSE
--rw-r--r--   0 quantra    (501) staff       (20)       73 2023-06-29 00:05:50.000000 django-lazy-srcset-0.2.2/MANIFEST.in
--rw-r--r--   0 quantra    (501) staff       (20)     6969 2023-07-06 22:44:29.530437 django-lazy-srcset-0.2.2/PKG-INFO
--rw-r--r--   0 quantra    (501) staff       (20)     5492 2023-06-27 20:50:37.000000 django-lazy-srcset-0.2.2/README.rst
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-06 22:44:29.524296 django-lazy-srcset-0.2.2/django_lazy_srcset.egg-info/
--rw-r--r--   0 quantra    (501) staff       (20)     6969 2023-07-06 22:44:29.000000 django-lazy-srcset-0.2.2/django_lazy_srcset.egg-info/PKG-INFO
--rw-r--r--   0 quantra    (501) staff       (20)      576 2023-07-06 22:44:29.000000 django-lazy-srcset-0.2.2/django_lazy_srcset.egg-info/SOURCES.txt
--rw-r--r--   0 quantra    (501) staff       (20)       40 2023-07-06 22:44:29.000000 django-lazy-srcset-0.2.2/django_lazy_srcset.egg-info/dependency_links.txt
--rw-r--r--   0 quantra    (501) staff       (20)       35 2023-07-06 22:44:29.000000 django-lazy-srcset-0.2.2/django_lazy_srcset.egg-info/requires.txt
--rw-r--r--   0 quantra    (501) staff       (20)       20 2023-07-06 22:44:29.000000 django-lazy-srcset-0.2.2/django_lazy_srcset.egg-info/top_level.txt
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-06 22:44:29.526626 django-lazy-srcset-0.2.2/lazy_srcset/
--rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-26 14:12:57.000000 django-lazy-srcset-0.2.2/lazy_srcset/__init__.py
--rw-r--r--   0 quantra    (501) staff       (20)       96 2023-06-26 17:31:28.000000 django-lazy-srcset-0.2.2/lazy_srcset/apps.py
--rw-r--r--   0 quantra    (501) staff       (20)     1237 2023-06-26 19:06:25.000000 django-lazy-srcset-0.2.2/lazy_srcset/conf.py
--rw-r--r--   0 quantra    (501) staff       (20)      679 2023-06-26 19:06:25.000000 django-lazy-srcset-0.2.2/lazy_srcset/imagegenerators.py
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-06 22:44:29.527402 django-lazy-srcset-0.2.2/lazy_srcset/management/
--rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-27 22:41:58.000000 django-lazy-srcset-0.2.2/lazy_srcset/management/__init__.py
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-06 22:44:29.528478 django-lazy-srcset-0.2.2/lazy_srcset/management/commands/
--rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-27 22:41:50.000000 django-lazy-srcset-0.2.2/lazy_srcset/management/commands/__init__.py
--rw-r--r--   0 quantra    (501) staff       (20)     3299 2023-06-29 00:03:00.000000 django-lazy-srcset-0.2.2/lazy_srcset/management/commands/imagekit_cleanup.py
-drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-06 22:44:29.530098 django-lazy-srcset-0.2.2/lazy_srcset/templatetags/
--rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-26 14:12:57.000000 django-lazy-srcset-0.2.2/lazy_srcset/templatetags/__init__.py
--rw-r--r--   0 quantra    (501) staff       (20)     8925 2023-07-06 19:45:37.000000 django-lazy-srcset-0.2.2/lazy_srcset/templatetags/lazy_srcset.py
--rw-r--r--   0 quantra    (501) staff       (20)       89 2023-06-26 19:06:22.000000 django-lazy-srcset-0.2.2/pyproject.toml
--rw-r--r--   0 quantra    (501) staff       (20)     1917 2023-07-06 22:44:29.537313 django-lazy-srcset-0.2.2/setup.cfg
--rw-r--r--   0 quantra    (501) staff       (20)       38 2023-06-26 17:04:23.000000 django-lazy-srcset-0.2.2/setup.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-11 16:16:16.816509 django-lazy-srcset-1.0.0/
+-rw-r--r--   0 quantra    (501) staff       (20)     1076 2023-05-02 22:05:05.000000 django-lazy-srcset-1.0.0/LICENSE
+-rw-r--r--   0 quantra    (501) staff       (20)       73 2023-06-29 00:05:50.000000 django-lazy-srcset-1.0.0/MANIFEST.in
+-rw-r--r--   0 quantra    (501) staff       (20)     8616 2023-07-11 16:16:16.816647 django-lazy-srcset-1.0.0/PKG-INFO
+-rw-r--r--   0 quantra    (501) staff       (20)     7072 2023-07-11 15:48:24.000000 django-lazy-srcset-1.0.0/README.rst
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-11 16:16:16.805156 django-lazy-srcset-1.0.0/django_lazy_srcset.egg-info/
+-rw-r--r--   0 quantra    (501) staff       (20)     8616 2023-07-11 16:16:16.000000 django-lazy-srcset-1.0.0/django_lazy_srcset.egg-info/PKG-INFO
+-rw-r--r--   0 quantra    (501) staff       (20)      576 2023-07-11 16:16:16.000000 django-lazy-srcset-1.0.0/django_lazy_srcset.egg-info/SOURCES.txt
+-rw-r--r--   0 quantra    (501) staff       (20)       40 2023-07-11 16:16:16.000000 django-lazy-srcset-1.0.0/django_lazy_srcset.egg-info/dependency_links.txt
+-rw-r--r--   0 quantra    (501) staff       (20)       35 2023-07-11 16:16:16.000000 django-lazy-srcset-1.0.0/django_lazy_srcset.egg-info/requires.txt
+-rw-r--r--   0 quantra    (501) staff       (20)       20 2023-07-11 16:16:16.000000 django-lazy-srcset-1.0.0/django_lazy_srcset.egg-info/top_level.txt
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-11 16:16:16.807438 django-lazy-srcset-1.0.0/lazy_srcset/
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-26 14:12:57.000000 django-lazy-srcset-1.0.0/lazy_srcset/__init__.py
+-rw-r--r--   0 quantra    (501) staff       (20)       96 2023-06-26 17:31:28.000000 django-lazy-srcset-1.0.0/lazy_srcset/apps.py
+-rw-r--r--   0 quantra    (501) staff       (20)     1947 2023-07-10 23:00:44.000000 django-lazy-srcset-1.0.0/lazy_srcset/conf.py
+-rw-r--r--   0 quantra    (501) staff       (20)      679 2023-06-26 19:06:25.000000 django-lazy-srcset-1.0.0/lazy_srcset/imagegenerators.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-11 16:16:16.808194 django-lazy-srcset-1.0.0/lazy_srcset/management/
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-27 22:41:58.000000 django-lazy-srcset-1.0.0/lazy_srcset/management/__init__.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-11 16:16:16.813844 django-lazy-srcset-1.0.0/lazy_srcset/management/commands/
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-27 22:41:50.000000 django-lazy-srcset-1.0.0/lazy_srcset/management/commands/__init__.py
+-rw-r--r--   0 quantra    (501) staff       (20)     3299 2023-06-29 00:03:00.000000 django-lazy-srcset-1.0.0/lazy_srcset/management/commands/imagekit_cleanup.py
+drwxr-xr-x   0 quantra    (501) staff       (20)        0 2023-07-11 16:16:16.816315 django-lazy-srcset-1.0.0/lazy_srcset/templatetags/
+-rw-r--r--   0 quantra    (501) staff       (20)        0 2023-06-26 14:12:57.000000 django-lazy-srcset-1.0.0/lazy_srcset/templatetags/__init__.py
+-rw-r--r--   0 quantra    (501) staff       (20)    11435 2023-07-11 12:35:35.000000 django-lazy-srcset-1.0.0/lazy_srcset/templatetags/lazy_srcset.py
+-rw-r--r--   0 quantra    (501) staff       (20)       89 2023-06-26 19:06:22.000000 django-lazy-srcset-1.0.0/pyproject.toml
+-rw-r--r--   0 quantra    (501) staff       (20)     1979 2023-07-11 16:16:16.820050 django-lazy-srcset-1.0.0/setup.cfg
+-rw-r--r--   0 quantra    (501) staff       (20)       38 2023-06-26 17:04:23.000000 django-lazy-srcset-1.0.0/setup.py
```

### Comparing `django-lazy-srcset-0.2.2/LICENSE` & `django-lazy-srcset-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-lazy-srcset-0.2.2/PKG-INFO` & `django-lazy-srcset-1.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: django-lazy-srcset
-Version: 0.2.2
-Summary: Lazy srcset and image generation for Django. Minimum effort required. No database required.
+Version: 1.0.0
+Summary: Lazy srcset and responsive image generation for Django. Minimum effort required. No database required.
+Home-page: https://github.com/Quantra/django-lazy-srcset
 Author: Vince Coleman
 Author-email: vince@shystudios.co.uk
 License: MIT
 Project-URL: Source, https://github.com/Quantra/django-lazy-srcset
 Keywords: django,django-lazy-srcset,django lazy srcset,django srcset,django responsive images,django responsive
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -44,17 +45,17 @@
 |pypi downloads|
 |github stars|
 
 ==================
 Django Lazy srcset
 ==================
 
-Lazy srcset and image generation for Django. Minimum effort required. No database required.
+Lazy srcset and responsive image generation for Django. Minimum effort required. No database required.
 
-Django Lazy srcset will create all the markup and images you need to provide responsive images via the srcset attribute.  All you need to do is install it, configure your breakpoints and use the ``{% srcset %}`` template tag.
+Django Lazy srcset will create the markup and generate the images you need to provide responsive images via the `srcset and sizes attributes for the img tag <https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images#resolution_switching_different_sizes>`_.  All you need to do is install it, configure your breakpoints and use the ``{% srcset %}`` template tag.
 
 All of the hard work (image generation and cacheing) is done by django-imagekit, by default this means images are generated just in time - lazily. Please see the `django-imagekit docs <https://django-imagekit.readthedocs.io>`_ for more info and configuration options.
 
 SVG images are supported, they will not be converted or resized but width and height attributes are still added as well as the ``role="img"`` attribute.
 
 You will also need Django and Pillow.
 
@@ -74,28 +75,43 @@
     INSTALLED_APPS = [
         # ...
         "imagekit",
         "lazy_srcset",
         # ...
     ]
 
-Configure your breakpoints and stuff:
+Configure your breakpoints and stuff (most/all of this is optional):
 
 .. code-block:: python
 
+    # When disabled src, width and height attributes are returned so images still work but no srcset or image
+    # generation will happen. By default, lazy-srcset is disabled when debug is True.
+    LAZY_SRCSET_ENABLED = not django_settings.DEBUG
+
+    # The default threshold to use when not specified in the config.
+    LAZY_SRCSET_THRESHOLD = 69
+
+    # The default generator to use when not specified in the config.
+    LAZY_SRCSET_GENERATOR_ID = "lazy_srcset:srcset_image"
+
     LAZY_SRCSET = {
         "default": {
             # breakpoints is the only setting you must define
             "breakpoints": [1920, 1580, 1280, 1024, 640],
             # If max_width is not provided the source image width is used, it's a good idea to set this
             "max_width": 2560,
             # If quality is not provided PIL will choose a default
             "quality": 91,
             # If format is not provided the source image format is used
             "format": "WEBP",
+            # The difference in width (px) required to generate a new image
+            # This prevents images being created which are too similar in size
+            "threshold": LAZY_SRCSET_THRESHOLD,
+            # If generator_id is not provided LAZY_SRCSET_GENERATOR_ID is used
+            "generator_id": LAZY_SRCSET_GENERATOR_ID,
         }
     }
 
 Use the ``{% srcset %}`` template tag:
 
 .. code-block:: django
 
@@ -108,21 +124,39 @@
     <img {% srcset image 25 33 50 %}  />
 
     {# You can provide a path to a static file #}
     <img {% srcset 'path/to/my/image.png' %} />
 
 Whilst not required it is advisable to take a nap at this stage.
 
-For further documentation and usage examples please read the docstrings in the source code for  `lazy_srcset/templatetags/lazy_srcset.py <https://github.com/Quantra/django-lazy-srcset/blob/master/lazy_srcset/templatetags/lazy_srcset.py>`_.
+For further documentation and examples of all the options please see the huge and obvious docstring in the source code for `lazy_srcset/templatetags/lazy_srcset.py <https://github.com/Quantra/django-lazy-srcset/blob/master/lazy_srcset/templatetags/lazy_srcset.py>`_.
 
-Due to the awesomeness of imagekit it's possible to configure django-lazy-srcset to use any image generator you have registered on a per config basis. Take a look at `lazy_srcset/conf.py <https://github.com/Quantra/django-lazy-srcset/blob/master/lazy_srcset/conf.py>`_ to see how to change the ``generator_id`` setting. For an example image generator look at `lazy_srcset/imagegenerators.py <https://github.com/Quantra/django-lazy-srcset/blob/master/lazy_srcset/imagegenerators.py>`_. This is completely optional.
+Advanced
+--------
+
+Due to the awesomeness of django-imagekit it's possible to configure django-lazy-srcset to use any image generator you have registered on a per config basis. Take a look at `lazy_srcset/conf.py <https://github.com/Quantra/django-lazy-srcset/blob/master/lazy_srcset/conf.py>`_ to see how to change the ``generator_id`` setting. For an example image generator look at `lazy_srcset/imagegenerators.py <https://github.com/Quantra/django-lazy-srcset/blob/master/lazy_srcset/imagegenerators.py>`_. This is completely optional but I thought I'd mention it as there are potential artistic uses here; for example you could use a generator to add filters to some images.
 
 Currently imagekit ``SourceGroup`` has not been implemented therefore the imagekit ``generateimages`` management command will not generate images for django-lazy-srcset. If you want to pre-generate images you can ``render_to_string()`` your templates in an appropriate save method or signal.  If you are using `django-content-blocks <https://github.com/Quantra/django-content-blocks>`_ this happens on publish anyway.
 
-Clean up of unused files created by django-lazy-srcset is down to you, if you require it at all.
+Clean up of old, unused files created by django-lazy-srcset is down to you, if you require it at all.
+
+Development Status & Roadmap
+----------------------------
+
+Django lazy srcset is in beta. There are currently no plans for further development.
+
+Dependencies & Thank You
+------------------------
+
+* https://github.com/matthewwithanm/django-imagekit/
+
+Other Packages to Consider
+--------------------------
+
+* https://github.com/codingjoe/django-pictures
 
 .. shields.io badges
 
 .. |package version| image:: https://img.shields.io/pypi/v/django-lazy-srcset
     :alt: PyPI Package Version
     :target: https://pypi.python.org/pypi/django-lazy-srcset/
```

### Comparing `django-lazy-srcset-0.2.2/README.rst` & `django-lazy-srcset-1.0.0/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 |pypi downloads|
 |github stars|
 
 ==================
 Django Lazy srcset
 ==================
 
-Lazy srcset and image generation for Django. Minimum effort required. No database required.
+Lazy srcset and responsive image generation for Django. Minimum effort required. No database required.
 
-Django Lazy srcset will create all the markup and images you need to provide responsive images via the srcset attribute.  All you need to do is install it, configure your breakpoints and use the ``{% srcset %}`` template tag.
+Django Lazy srcset will create the markup and generate the images you need to provide responsive images via the `srcset and sizes attributes for the img tag <https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images#resolution_switching_different_sizes>`_.  All you need to do is install it, configure your breakpoints and use the ``{% srcset %}`` template tag.
 
 All of the hard work (image generation and cacheing) is done by django-imagekit, by default this means images are generated just in time - lazily. Please see the `django-imagekit docs <https://django-imagekit.readthedocs.io>`_ for more info and configuration options.
 
 SVG images are supported, they will not be converted or resized but width and height attributes are still added as well as the ``role="img"`` attribute.
 
 You will also need Django and Pillow.
 
@@ -40,28 +40,43 @@
     INSTALLED_APPS = [
         # ...
         "imagekit",
         "lazy_srcset",
         # ...
     ]
 
-Configure your breakpoints and stuff:
+Configure your breakpoints and stuff (most/all of this is optional):
 
 .. code-block:: python
 
+    # When disabled src, width and height attributes are returned so images still work but no srcset or image
+    # generation will happen. By default, lazy-srcset is disabled when debug is True.
+    LAZY_SRCSET_ENABLED = not django_settings.DEBUG
+
+    # The default threshold to use when not specified in the config.
+    LAZY_SRCSET_THRESHOLD = 69
+
+    # The default generator to use when not specified in the config.
+    LAZY_SRCSET_GENERATOR_ID = "lazy_srcset:srcset_image"
+
     LAZY_SRCSET = {
         "default": {
             # breakpoints is the only setting you must define
             "breakpoints": [1920, 1580, 1280, 1024, 640],
             # If max_width is not provided the source image width is used, it's a good idea to set this
             "max_width": 2560,
             # If quality is not provided PIL will choose a default
             "quality": 91,
             # If format is not provided the source image format is used
             "format": "WEBP",
+            # The difference in width (px) required to generate a new image
+            # This prevents images being created which are too similar in size
+            "threshold": LAZY_SRCSET_THRESHOLD,
+            # If generator_id is not provided LAZY_SRCSET_GENERATOR_ID is used
+            "generator_id": LAZY_SRCSET_GENERATOR_ID,
         }
     }
 
 Use the ``{% srcset %}`` template tag:
 
 .. code-block:: django
 
@@ -74,21 +89,39 @@
     <img {% srcset image 25 33 50 %}  />
 
     {# You can provide a path to a static file #}
     <img {% srcset 'path/to/my/image.png' %} />
 
 Whilst not required it is advisable to take a nap at this stage.
 
-For further documentation and usage examples please read the docstrings in the source code for  `lazy_srcset/templatetags/lazy_srcset.py <https://github.com/Quantra/django-lazy-srcset/blob/master/lazy_srcset/templatetags/lazy_srcset.py>`_.
+For further documentation and examples of all the options please see the huge and obvious docstring in the source code for `lazy_srcset/templatetags/lazy_srcset.py <https://github.com/Quantra/django-lazy-srcset/blob/master/lazy_srcset/templatetags/lazy_srcset.py>`_.
 
-Due to the awesomeness of imagekit it's possible to configure django-lazy-srcset to use any image generator you have registered on a per config basis. Take a look at `lazy_srcset/conf.py <https://github.com/Quantra/django-lazy-srcset/blob/master/lazy_srcset/conf.py>`_ to see how to change the ``generator_id`` setting. For an example image generator look at `lazy_srcset/imagegenerators.py <https://github.com/Quantra/django-lazy-srcset/blob/master/lazy_srcset/imagegenerators.py>`_. This is completely optional.
+Advanced
+--------
+
+Due to the awesomeness of django-imagekit it's possible to configure django-lazy-srcset to use any image generator you have registered on a per config basis. Take a look at `lazy_srcset/conf.py <https://github.com/Quantra/django-lazy-srcset/blob/master/lazy_srcset/conf.py>`_ to see how to change the ``generator_id`` setting. For an example image generator look at `lazy_srcset/imagegenerators.py <https://github.com/Quantra/django-lazy-srcset/blob/master/lazy_srcset/imagegenerators.py>`_. This is completely optional but I thought I'd mention it as there are potential artistic uses here; for example you could use a generator to add filters to some images.
 
 Currently imagekit ``SourceGroup`` has not been implemented therefore the imagekit ``generateimages`` management command will not generate images for django-lazy-srcset. If you want to pre-generate images you can ``render_to_string()`` your templates in an appropriate save method or signal.  If you are using `django-content-blocks <https://github.com/Quantra/django-content-blocks>`_ this happens on publish anyway.
 
-Clean up of unused files created by django-lazy-srcset is down to you, if you require it at all.
+Clean up of old, unused files created by django-lazy-srcset is down to you, if you require it at all.
+
+Development Status & Roadmap
+----------------------------
+
+Django lazy srcset is in beta. There are currently no plans for further development.
+
+Dependencies & Thank You
+------------------------
+
+* https://github.com/matthewwithanm/django-imagekit/
+
+Other Packages to Consider
+--------------------------
+
+* https://github.com/codingjoe/django-pictures
 
 .. shields.io badges
 
 .. |package version| image:: https://img.shields.io/pypi/v/django-lazy-srcset
     :alt: PyPI Package Version
     :target: https://pypi.python.org/pypi/django-lazy-srcset/
```

### Comparing `django-lazy-srcset-0.2.2/django_lazy_srcset.egg-info/PKG-INFO` & `django-lazy-srcset-1.0.0/django_lazy_srcset.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: django-lazy-srcset
-Version: 0.2.2
-Summary: Lazy srcset and image generation for Django. Minimum effort required. No database required.
+Version: 1.0.0
+Summary: Lazy srcset and responsive image generation for Django. Minimum effort required. No database required.
+Home-page: https://github.com/Quantra/django-lazy-srcset
 Author: Vince Coleman
 Author-email: vince@shystudios.co.uk
 License: MIT
 Project-URL: Source, https://github.com/Quantra/django-lazy-srcset
 Keywords: django,django-lazy-srcset,django lazy srcset,django srcset,django responsive images,django responsive
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -44,17 +45,17 @@
 |pypi downloads|
 |github stars|
 
 ==================
 Django Lazy srcset
 ==================
 
-Lazy srcset and image generation for Django. Minimum effort required. No database required.
+Lazy srcset and responsive image generation for Django. Minimum effort required. No database required.
 
-Django Lazy srcset will create all the markup and images you need to provide responsive images via the srcset attribute.  All you need to do is install it, configure your breakpoints and use the ``{% srcset %}`` template tag.
+Django Lazy srcset will create the markup and generate the images you need to provide responsive images via the `srcset and sizes attributes for the img tag <https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images#resolution_switching_different_sizes>`_.  All you need to do is install it, configure your breakpoints and use the ``{% srcset %}`` template tag.
 
 All of the hard work (image generation and cacheing) is done by django-imagekit, by default this means images are generated just in time - lazily. Please see the `django-imagekit docs <https://django-imagekit.readthedocs.io>`_ for more info and configuration options.
 
 SVG images are supported, they will not be converted or resized but width and height attributes are still added as well as the ``role="img"`` attribute.
 
 You will also need Django and Pillow.
 
@@ -74,28 +75,43 @@
     INSTALLED_APPS = [
         # ...
         "imagekit",
         "lazy_srcset",
         # ...
     ]
 
-Configure your breakpoints and stuff:
+Configure your breakpoints and stuff (most/all of this is optional):
 
 .. code-block:: python
 
+    # When disabled src, width and height attributes are returned so images still work but no srcset or image
+    # generation will happen. By default, lazy-srcset is disabled when debug is True.
+    LAZY_SRCSET_ENABLED = not django_settings.DEBUG
+
+    # The default threshold to use when not specified in the config.
+    LAZY_SRCSET_THRESHOLD = 69
+
+    # The default generator to use when not specified in the config.
+    LAZY_SRCSET_GENERATOR_ID = "lazy_srcset:srcset_image"
+
     LAZY_SRCSET = {
         "default": {
             # breakpoints is the only setting you must define
             "breakpoints": [1920, 1580, 1280, 1024, 640],
             # If max_width is not provided the source image width is used, it's a good idea to set this
             "max_width": 2560,
             # If quality is not provided PIL will choose a default
             "quality": 91,
             # If format is not provided the source image format is used
             "format": "WEBP",
+            # The difference in width (px) required to generate a new image
+            # This prevents images being created which are too similar in size
+            "threshold": LAZY_SRCSET_THRESHOLD,
+            # If generator_id is not provided LAZY_SRCSET_GENERATOR_ID is used
+            "generator_id": LAZY_SRCSET_GENERATOR_ID,
         }
     }
 
 Use the ``{% srcset %}`` template tag:
 
 .. code-block:: django
 
@@ -108,21 +124,39 @@
     <img {% srcset image 25 33 50 %}  />
 
     {# You can provide a path to a static file #}
     <img {% srcset 'path/to/my/image.png' %} />
 
 Whilst not required it is advisable to take a nap at this stage.
 
-For further documentation and usage examples please read the docstrings in the source code for  `lazy_srcset/templatetags/lazy_srcset.py <https://github.com/Quantra/django-lazy-srcset/blob/master/lazy_srcset/templatetags/lazy_srcset.py>`_.
+For further documentation and examples of all the options please see the huge and obvious docstring in the source code for `lazy_srcset/templatetags/lazy_srcset.py <https://github.com/Quantra/django-lazy-srcset/blob/master/lazy_srcset/templatetags/lazy_srcset.py>`_.
 
-Due to the awesomeness of imagekit it's possible to configure django-lazy-srcset to use any image generator you have registered on a per config basis. Take a look at `lazy_srcset/conf.py <https://github.com/Quantra/django-lazy-srcset/blob/master/lazy_srcset/conf.py>`_ to see how to change the ``generator_id`` setting. For an example image generator look at `lazy_srcset/imagegenerators.py <https://github.com/Quantra/django-lazy-srcset/blob/master/lazy_srcset/imagegenerators.py>`_. This is completely optional.
+Advanced
+--------
+
+Due to the awesomeness of django-imagekit it's possible to configure django-lazy-srcset to use any image generator you have registered on a per config basis. Take a look at `lazy_srcset/conf.py <https://github.com/Quantra/django-lazy-srcset/blob/master/lazy_srcset/conf.py>`_ to see how to change the ``generator_id`` setting. For an example image generator look at `lazy_srcset/imagegenerators.py <https://github.com/Quantra/django-lazy-srcset/blob/master/lazy_srcset/imagegenerators.py>`_. This is completely optional but I thought I'd mention it as there are potential artistic uses here; for example you could use a generator to add filters to some images.
 
 Currently imagekit ``SourceGroup`` has not been implemented therefore the imagekit ``generateimages`` management command will not generate images for django-lazy-srcset. If you want to pre-generate images you can ``render_to_string()`` your templates in an appropriate save method or signal.  If you are using `django-content-blocks <https://github.com/Quantra/django-content-blocks>`_ this happens on publish anyway.
 
-Clean up of unused files created by django-lazy-srcset is down to you, if you require it at all.
+Clean up of old, unused files created by django-lazy-srcset is down to you, if you require it at all.
+
+Development Status & Roadmap
+----------------------------
+
+Django lazy srcset is in beta. There are currently no plans for further development.
+
+Dependencies & Thank You
+------------------------
+
+* https://github.com/matthewwithanm/django-imagekit/
+
+Other Packages to Consider
+--------------------------
+
+* https://github.com/codingjoe/django-pictures
 
 .. shields.io badges
 
 .. |package version| image:: https://img.shields.io/pypi/v/django-lazy-srcset
     :alt: PyPI Package Version
     :target: https://pypi.python.org/pypi/django-lazy-srcset/
```

### Comparing `django-lazy-srcset-0.2.2/django_lazy_srcset.egg-info/SOURCES.txt` & `django-lazy-srcset-1.0.0/django_lazy_srcset.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-lazy-srcset-0.2.2/lazy_srcset/imagegenerators.py` & `django-lazy-srcset-1.0.0/lazy_srcset/imagegenerators.py`

 * *Files identical despite different names*

### Comparing `django-lazy-srcset-0.2.2/lazy_srcset/management/commands/imagekit_cleanup.py` & `django-lazy-srcset-1.0.0/lazy_srcset/management/commands/imagekit_cleanup.py`

 * *Files identical despite different names*

### Comparing `django-lazy-srcset-0.2.2/lazy_srcset/templatetags/lazy_srcset.py` & `django-lazy-srcset-1.0.0/lazy_srcset/templatetags/lazy_srcset.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,30 +3,23 @@
 from pathlib import Path
 from xml.etree import ElementTree
 
 from django import template
 from django.contrib.staticfiles import finders
 from django.contrib.staticfiles.storage import staticfiles_storage
 from django.core.files.images import ImageFile
-from django.utils.safestring import mark_safe
+from django.template.exceptions import TemplateSyntaxError
+from django.utils.html import format_html
 from imagekit.cachefiles import ImageCacheFile
 from imagekit.registry import generator_registry
 
 from lazy_srcset.conf import settings
 
 register = template.Library()
 
-# Format strings for attrs and parts of attrs.
-FORMAT_STRINGS = {
-    attr: f'{attr}="%s"' for attr in ["src", "width", "height", "srcset", "sizes"]
-}
-FORMAT_STRINGS["srcset_entry"] = "%s %iw"
-FORMAT_STRINGS["sizes_entry"] = "(max-width: %ipx) %ivw"
-FORMAT_STRINGS["size"] = "%ivw"
-
 
 def lists_to_dict(keys, values, default_value=100):
     """
     Combine uneven lists into a dictionary padding values with default_value if the values list is shorter than the
     keys list.  If the values list is longer it will ignore any extra values.
     """
     combined_dict = {}
@@ -62,178 +55,264 @@
         if width is None or height is None:
             viewbox = root.get("viewBox")
             try:
                 _, _, width, height = viewbox.split(" ")
             except (AttributeError, ValueError):
                 pass
 
-        # These could include units eg px or pt so strip them out.
+        # These could include units E.g. px or pt so strip them out.
         width = re.sub("\\D", "", width) if width is not None else None
         height = re.sub("\\D", "", height) if height is not None else None
 
     return width, height
 
 
-def svg_srcset(svg_file):
+def sanitize_breakpoint(breakpoint):
     """
-    Returns attrs string containing src and width and height if possible. Will also add role="img" attr.
+    Breakpoints must be integers.
+    """
+    try:
+        return int(breakpoint)
+    except ValueError:
+        raise TemplateSyntaxError(
+            "Invalid breakpoint: %s\nBreakpoints must be integers." % breakpoint
+        )
+
+
+def sanitize_size(size):
     """
-    # SVG only needs a src attribute, role="img" help screen readers to correctly announce the SVG as an image.
-    attrs = [FORMAT_STRINGS["src"] % svg_file.url, 'role="img"']
+    Sizes need to be either an integer or a string with px or vw units.
+    """
+    try:
+        return int(size), "vw"
+    except ValueError:
+        pass
+
+    try:
+        size, units = int(size[:-2]), size[-2:]
+    except (IndexError, ValueError):
+        raise TemplateSyntaxError(
+            "Invalid size: %s\nBreakpoints must be integers.\nSizes must specify vw or px units or be integers."
+            % size
+        )
+
+    if units not in ["px", "vw"]:
+        raise TemplateSyntaxError("Invalid size: %s\nUnits must be px or vw." % size)
+
+    return size, units
 
+
+def svg_srcset(svg):
+    """
+    Returns attrs string containing src and width and height if possible. Will also add role="img" attr.
+    """
     # Try getting width and height from attrs.
     try:
-        width = svg_file.width
-        height = svg_file.height
+        width = svg.width
+        height = svg.height
     except AttributeError:
         width, height = None, None
 
     # If we don't have the width and height try getting it from the SVG file.
     if width is None or height is None:
-        width, height = get_svg_dimensions(svg_file)
+        width, height = get_svg_dimensions(svg)
 
-    # Add width and height to our attrs if we have them.
+    # Return with width and height if we have them.
     if width is not None and height is not None:
-        attrs += [FORMAT_STRINGS["width"] % width, FORMAT_STRINGS["height"] % height]
+        return format_html(
+            'src="{}" width="{}" height="{}" role="img"', svg.url, width, height
+        )
 
-    # Stringification!
-    return mark_safe(" ".join(attrs))
+    # Return with src only if we don't have width and height
+    return format_html('src="{}" role="img"', svg.url)
 
 
 @register.simple_tag
 def srcset(*args, **kwargs):
     """
     The srcset template tag will create srcset, sizes, src, width and height attributes for an <img> tag.
 
     The first arg must be an ImageField or subclass or a path to an image discoverable by static files.
 
-    args can provide relative image sizes in vw for each breakpoint, if not provided 100vw is assumed.  These are
-    integers which are used to calculate generated image sizes.  They must be in vw.  Sorry no calc() etc. allowed.
-    Don't try too hard here! Close is good enough.
+    args can provide relative image sizes in vw for each break point, if not provided 100vw is assumed.  These are
+    integers which are used to calculate generated image sizes.  They must have units of vw or px only. If no units
+    are supplied then vw is assumed.
 
-    kwargs can be used to provide breakpoints and the relative width for each breakpoint directly (ignoring the
-    config breakpoints and args if you set them for some reason).
+    kwargs can be used to provide break points and the relative size for each break point directly (ignoring the
+    config break points and args if you set them for some reason).
 
     The config with the key ``default`` is used unless you provide the config kwarg to specify another config to use.
 
-    You can use the ``max_width`` and ``qualtiy`` kwargs to override the config on a per-use basis.
+    You can use the ``max_width``, ``threshold`` and ``quality`` kwargs to override the config on a per-use basis.
+
+    The default size (for any resolution above the biggest break point) is set to the same as the biggest break point
+    by default. If you want to set the default size to something else use the ``default_size`` kwarg.
 
     Example usage (where image is a file-like e.g. ImageField or a string representing a path to a static file):
 
+    <!-- All sizes assumed to be 100vw -->
     <img {% srcset image %} />
 
+    <!-- First break point 25vw second break point 50vw all others 100vw -->
     <img {% srcset image 25 50 %} />
 
-    <img {% srcset image 25 50 quality=50 %} />
+    <!-- These are all the valid ways to specify sizes as args -->
+    <img {% srcset image 25 '50vw' '300px' %}
+
+    <!-- Define break points and sizes as kwargs -->
+    <!-- Any sizes set as args are ignored + config break points are ignored -->
+    <img {% srcset image 1920=25 1024=50 %} />
 
-    <img {% srcset image config="custom_breakpoints" %} />
+    <!-- These are all the valid ways to specify break points and sizes as kwargs -->
+    <img {% srcset image 1920=25 1024='50vw' 640='300px' %} />
 
-    <img {% srcset image 25 50 config="custom_breakpoints" %} />
+    <!-- Use the config "custom_breakpoints" instead of "default" -->
+    <img {% srcset image config='custom_breakpoints' %} />
 
-    <img {% srcset image 25 50 config="custom_breakpoints" quality=50 %} />
+    <!-- Specify max_width as a kwarg -->
+    <img {% srcset image max_width=1920 %} />
 
-    <img {% srcset image 25 50 config="custom_breakpoints" max_width=1920 quality=50 %} />
+    <!-- Specify image quality as a kwarg -->
+    <img {% srcset image quality=50 %} />
 
-    <img {% srcset image 1920=25 1024=50 %} />
+    <!-- Specify threshold as a kwarg -->
+    <img {% srcset image threshold=100 %} />
 
-    <img {% srcset image 1920=25 1024=50 max_width=1920 quality=50 %} />
+    <!-- Specify default size as a kwarg (otherwise it is assumed to be the same as the biggest breakpoint) -->
+    <img {% srcset image default_size=50 %} />
 
+    <!-- You can set the default size with units in the same way as the sizes args -->
+    <img {% srcset image default_size='300px' %} />
 
+    <!-- You can mix and match all of the above E.g. -->
+    <img {% srcset image 25 33 50 config='custom_breakpoints' max_width=1920 image_quality=50 threshold=100 %} />
+    <img {% srcset image 1920=25 1024=50 default_size=50 image_quality=50 %} />
     """
+    # INIT
     args = list(args)
 
     # If the image has an open method we should be good to go.  If not assume it's a string and get it from
     # staticfiles wrapped up in ImageFile. Set the url attribute, so we can use it later.
     image = args.pop(0)
     if not hasattr(image, "open"):
         url = staticfiles_storage.url(image)
         image = ImageFile(open(finders.find(image), "rb"))
         image.url = url
 
-    # If the image is an SVG return now with src="whatever.svg" and width and height if possible. SVG is lazy king!
+    # If the image is an SVG return now with src, width and height if possible. SVG is lazy king!
     if Path(image.name).suffix.lower() == ".svg":
         return svg_srcset(image)
 
+    # If LAZY_SRCSET_ENABLED = False return src, width and height
+    if not settings.LAZY_SRCSET_ENABLED:
+        return format_html(
+            'src="{}" width="{}" height="{}"', image.url, image.width, image.height
+        )
+
     # Get the conf from the config kwarg or default
     try:
         conf = settings.LAZY_SRCSET[kwargs.pop("config")]
     except KeyError:
         conf = settings.LAZY_SRCSET["default"]
 
+    # Get the default size from kwargs
+    try:
+        default_size = kwargs.pop("default_size")
+    except KeyError:
+        default_size = None
+
     # Get the max_width from kwargs or conf.
     max_width = get_from_kwargs_or_conf("max_width", kwargs, conf)
 
+    # Get the kwargs for the image generator
+    output_format = conf.get("format")
+    quality = get_from_kwargs_or_conf("quality", kwargs, conf)
+    generator_id = conf.get("generator_id", settings.LAZY_SRCSET_GENERATOR_ID)
+    threshold = int(
+        get_from_kwargs_or_conf("threshold", kwargs, conf)
+        or settings.LAZY_SRCSET_THRESHOLD
+    )
+
+    # All kwargs except breakpoint kwargs must be popped by now!
+
+    # If we have kwargs we can set the sizes otherwise try and get them from args.
+    sizes_dict = kwargs or lists_to_dict(conf["breakpoints"], args)
+
+    # The sizes in our dict are strings and might contain px|vw
+    # After this our dict will be like: {1920: (50, "vw")}
+    sizes_dict = {
+        sanitize_breakpoint(k): sanitize_size(v) for k, v in sizes_dict.items()
+    }
+
+    # Create the sizes for the sizes attr
+    sizes = [
+        format_html("(max-width: {}px) {}{}", size, *sizes_dict[size])
+        for size in sorted(sizes_dict.keys())
+    ]
+
+    # Add the default size
+    if default_size is not None:
+        default_size = sanitize_size(default_size)
+    else:
+        default_size = sizes_dict[max(sizes_dict.keys())]
+    sizes.append(format_html("{}{}", *default_size))
+
     # Set the maximum width image in our srcset.
     if max_width is None or max_width > image.width:
         # Limit max_width to image.width or use image.width if max_width is None.
         max_width = image.width
 
-    # Get the format and quality from kwargs or conf and wrap up together with source in generator_kwargs.
-    # These will be used for every image generation.
-    generator_kwargs = {
-        "source": image,
-        "output_format": conf.get("format"),
-        "quality": get_from_kwargs_or_conf("quality", kwargs, conf),
-    }
+    # widths_dict will be a dict with the image width as key and a boolean if the image must be created E.g.
+    # {960: True}
+    widths_dict = {max_width: True}
 
     # Make sure the image file is closed as soon as we can.
     image.close()
 
-    # Big generator!  https://youtu.be/8W_VC_BgMjo
-    generator_id = conf.get("generator_id", settings.LAZY_SRCSET_GENERATOR_ID)
-
-    # Generate the max_width image via imagekit.
-    generator = generator_registry.get(
-        generator_id, width=max_width, **generator_kwargs
-    )
-    generator_image = ImageCacheFile(generator)
-
-    # Set the max_width image as our src and include it in the srcset.
-    src_value = generator_image.url
-    srcset_values = [FORMAT_STRINGS["srcset_entry"] % (generator_image.url, max_width)]
-
-    # Set the width and height from the max_width image.
-    width, height = generator_image.width, generator_image.height
-
-    # If we have kwargs we can set the sizes otherwise try and get them from args.
-    sizes_dict = (
-        {int(k): int(v) for k, v in kwargs.items()}
-        if kwargs
-        else lists_to_dict(conf["breakpoints"], args)
-    )
-
-    # Set the default size to match our relative width for the biggest breakpoint.
-    sizes = [FORMAT_STRINGS["size"] % sizes_dict[max(sizes_dict.keys())]]
+    # GO!
 
-    # Loop through the sizes_dict to create the sizes and srcset attrs and generate the scaled images.
-    for breakpoint_width, relative_width in sizes_dict.items():
-        # Add an entry for this breakpoint to sizes.
-        sizes.append(FORMAT_STRINGS["sizes_entry"] % (breakpoint_width, relative_width))
+    # Loop through the sizes_dict to create the widths_dict used for image generation.
+    for breakpoint_width, (width, units) in sizes_dict.items():
+        if units == "px":
+            # When px units are defined always generate an image with that width
+            widths_dict[width] = True
+            continue
 
         # Calculate the target width for this breakpoint with some quick maths.
-        target_width = math.ceil(breakpoint_width * relative_width / 100)
-        if target_width >= max_width:
+        target_width = math.ceil(breakpoint_width * width / 100)
+        if target_width < max_width:
             # Don't upscale images, that would require extra effort.
+            widths_dict[target_width] = False
+
+    # Loop through the widths of images and generate what is needed
+    current_width = max_width
+    images = []
+    for width in reversed(sorted(widths_dict.keys())):
+        if not widths_dict[width] and (current_width - width) < threshold:
+            # Only generate required images and images outside our threshold
             continue
 
+        current_width = width
+
         # Generate the image via imagekit.
         generator = generator_registry.get(
-            generator_id, width=target_width, **generator_kwargs
+            generator_id,
+            width=width,
+            source=image,
+            output_format=output_format,
+            quality=quality,
         )
         generator_image = ImageCacheFile(generator)
+        images.append(generator_image)
 
-        # Add an entry for this image to the srcset.
-        srcset_values.append(
-            FORMAT_STRINGS["srcset_entry"] % (generator_image.url, target_width)
-        )
-
-    # Create the attrs list for imminent stringification.
-    attrs = [
-        FORMAT_STRINGS["src"] % src_value,
-        FORMAT_STRINGS["srcset"] % ", ".join(srcset_values),
-        FORMAT_STRINGS["sizes"] % ", ".join(reversed(sizes)),
-        FORMAT_STRINGS["width"] % width,
-        FORMAT_STRINGS["height"] % height,
-    ]
+    # Create the srcsets
+    srcsets = [format_html("{} {}w", image.url, image.width) for image in images]
 
     # Stringify!
-    return mark_safe(" ".join(attrs))
+    return format_html(
+        'src="{}" srcset="{}" sizes="{}" width="{}" height="{}"',
+        images[0].url,
+        ", ".join(srcsets),
+        ", ".join(sizes),
+        images[0].width,
+        images[0].height,
+    )
```

### Comparing `django-lazy-srcset-0.2.2/setup.cfg` & `django-lazy-srcset-1.0.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 [metadata]
 name = django-lazy-srcset
-version = 0.2.2
-description = Lazy srcset and image generation for Django. Minimum effort required. No database required.
+version = 1.0.0
+description = Lazy srcset and responsive image generation for Django. Minimum effort required. No database required.
 long_description = file:README.rst
 long_description_content_type = text/x-rst
+url = https://github.com/Quantra/django-lazy-srcset
 author = Vince Coleman
 author_email = vince@shystudios.co.uk
 license = MIT
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
 	Framework :: Django :: 4.2
 	Intended Audience :: Developers
-	Development Status :: 3 - Alpha
+	Development Status :: 4 - Beta
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
```

