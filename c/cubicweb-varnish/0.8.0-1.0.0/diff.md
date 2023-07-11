# Comparing `tmp/cubicweb-varnish-0.8.0.tar.gz` & `tmp/cubicweb-varnish-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-varnish-0.8.0.tar", last modified: Wed Jan  4 10:37:54 2023, max compression
+gzip compressed data, was "cubicweb-varnish-1.0.0.tar", last modified: Tue Jul 11 08:02:07 2023, max compression
```

## Comparing `cubicweb-varnish-0.8.0.tar` & `cubicweb-varnish-1.0.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 10:37:54.621428 cubicweb-varnish-0.8.0/
--rw-rw-rw-   0 root         (0) root         (0)      425 2023-01-04 10:37:39.000000 cubicweb-varnish-0.8.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2013 2023-01-04 10:37:54.621428 cubicweb-varnish-0.8.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1562 2023-01-04 10:37:39.000000 cubicweb-varnish-0.8.0/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      674 2023-01-04 10:37:39.000000 cubicweb-varnish-0.8.0/__pkginfo__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 10:37:54.621428 cubicweb-varnish-0.8.0/cubicweb_varnish/
--rw-rw-rw-   0 root         (0) root         (0)       43 2023-01-04 10:37:39.000000 cubicweb-varnish-0.8.0/cubicweb_varnish/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      674 2023-01-04 10:37:39.000000 cubicweb-varnish-0.8.0/cubicweb_varnish/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1014 2023-01-04 10:37:39.000000 cubicweb-varnish-0.8.0/cubicweb_varnish/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     2467 2023-01-04 10:37:39.000000 cubicweb-varnish-0.8.0/cubicweb_varnish/hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 10:37:54.621428 cubicweb-varnish-0.8.0/cubicweb_varnish/i18n/
--rw-rw-rw-   0 root         (0) root         (0)      203 2023-01-04 10:37:39.000000 cubicweb-varnish-0.8.0/cubicweb_varnish/i18n/en.po
--rw-rw-rw-   0 root         (0) root         (0)      203 2023-01-04 10:37:39.000000 cubicweb-varnish-0.8.0/cubicweb_varnish/i18n/es.po
--rw-rw-rw-   0 root         (0) root         (0)      203 2023-01-04 10:37:39.000000 cubicweb-varnish-0.8.0/cubicweb_varnish/i18n/fr.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 10:37:54.621428 cubicweb-varnish-0.8.0/cubicweb_varnish/migration/
--rw-rw-rw-   0 root         (0) root         (0)     1067 2023-01-04 10:37:39.000000 cubicweb-varnish-0.8.0/cubicweb_varnish/migration/postcreate.py
--rw-rw-rw-   0 root         (0) root         (0)     1115 2023-01-04 10:37:39.000000 cubicweb-varnish-0.8.0/cubicweb_varnish/site_cubicweb.py
--rw-rw-rw-   0 root         (0) root         (0)     4491 2023-01-04 10:37:39.000000 cubicweb-varnish-0.8.0/cubicweb_varnish/varnishadm.py
--rw-rw-rw-   0 root         (0) root         (0)      857 2023-01-04 10:37:39.000000 cubicweb-varnish-0.8.0/cubicweb_varnish/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 10:37:54.621428 cubicweb-varnish-0.8.0/cubicweb_varnish.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2013 2023-01-04 10:37:53.000000 cubicweb-varnish-0.8.0/cubicweb_varnish.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      733 2023-01-04 10:37:54.000000 cubicweb-varnish-0.8.0/cubicweb_varnish.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-04 10:37:53.000000 cubicweb-varnish-0.8.0/cubicweb_varnish.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-01-04 10:37:54.000000 cubicweb-varnish-0.8.0/cubicweb_varnish.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-04 10:37:53.000000 cubicweb-varnish-0.8.0/cubicweb_varnish.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       25 2023-01-04 10:37:54.000000 cubicweb-varnish-0.8.0/cubicweb_varnish.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-01-04 10:37:54.000000 cubicweb-varnish-0.8.0/cubicweb_varnish.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-04 10:37:54.625428 cubicweb-varnish-0.8.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2612 2023-01-04 10:37:39.000000 cubicweb-varnish-0.8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 10:37:54.621428 cubicweb-varnish-0.8.0/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-04 10:37:54.621428 cubicweb-varnish-0.8.0/test/data/
--rw-rw-rw-   0 root         (0) root         (0)        8 2023-01-04 10:37:39.000000 cubicweb-varnish-0.8.0/test/data/bootstrap_cubes
--rw-rw-rw-   0 root         (0) root         (0)     2395 2023-01-04 10:37:39.000000 cubicweb-varnish-0.8.0/test/pytestconf.py
--rw-rw-rw-   0 root         (0) root         (0)     1737 2023-01-04 10:37:39.000000 cubicweb-varnish-0.8.0/test/test_varnish.py
--rw-rw-rw-   0 root         (0) root         (0)      851 2023-01-04 10:37:39.000000 cubicweb-varnish-0.8.0/tox.ini
+drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-07-11 08:02:07.324325 cubicweb-varnish-1.0.0/
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      425 2023-07-03 14:02:20.000000 cubicweb-varnish-1.0.0/MANIFEST.in
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     1993 2023-07-11 08:02:07.324325 cubicweb-varnish-1.0.0/PKG-INFO
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     1562 2023-07-03 14:02:20.000000 cubicweb-varnish-1.0.0/README.rst
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      671 2023-07-07 12:19:50.000000 cubicweb-varnish-1.0.0/__pkginfo__.py
+drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-07-11 08:02:07.320325 cubicweb-varnish-1.0.0/cubicweb_varnish/
+-rw-r--r--   0 fferry    (1000) fferry    (1000)       43 2023-07-03 14:02:20.000000 cubicweb-varnish-1.0.0/cubicweb_varnish/__init__.py
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      671 2023-07-07 12:19:50.000000 cubicweb-varnish-1.0.0/cubicweb_varnish/__pkginfo__.py
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     1014 2023-07-03 14:02:20.000000 cubicweb-varnish-1.0.0/cubicweb_varnish/entities.py
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     2463 2023-07-07 12:18:41.000000 cubicweb-varnish-1.0.0/cubicweb_varnish/hooks.py
+drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-07-11 08:02:07.320325 cubicweb-varnish-1.0.0/cubicweb_varnish/i18n/
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      203 2023-07-03 14:02:20.000000 cubicweb-varnish-1.0.0/cubicweb_varnish/i18n/en.po
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      203 2023-07-03 14:02:20.000000 cubicweb-varnish-1.0.0/cubicweb_varnish/i18n/es.po
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      203 2023-07-03 14:02:20.000000 cubicweb-varnish-1.0.0/cubicweb_varnish/i18n/fr.po
+drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-07-11 08:02:07.324325 cubicweb-varnish-1.0.0/cubicweb_varnish/migration/
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     1067 2023-07-03 14:02:20.000000 cubicweb-varnish-1.0.0/cubicweb_varnish/migration/postcreate.py
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     1115 2023-07-03 14:02:20.000000 cubicweb-varnish-1.0.0/cubicweb_varnish/site_cubicweb.py
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     4489 2023-07-07 12:18:41.000000 cubicweb-varnish-1.0.0/cubicweb_varnish/varnishadm.py
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      857 2023-07-03 14:02:20.000000 cubicweb-varnish-1.0.0/cubicweb_varnish/views.py
+drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-07-11 08:02:07.320325 cubicweb-varnish-1.0.0/cubicweb_varnish.egg-info/
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     1993 2023-07-11 08:02:07.000000 cubicweb-varnish-1.0.0/cubicweb_varnish.egg-info/PKG-INFO
+-rw-r--r--   0 fferry    (1000) fferry    (1000)      733 2023-07-11 08:02:07.000000 cubicweb-varnish-1.0.0/cubicweb_varnish.egg-info/SOURCES.txt
+-rw-r--r--   0 fferry    (1000) fferry    (1000)        1 2023-07-11 08:02:07.000000 cubicweb-varnish-1.0.0/cubicweb_varnish.egg-info/dependency_links.txt
+-rw-r--r--   0 fferry    (1000) fferry    (1000)       44 2023-07-11 08:02:07.000000 cubicweb-varnish-1.0.0/cubicweb_varnish.egg-info/entry_points.txt
+-rw-r--r--   0 fferry    (1000) fferry    (1000)        1 2023-07-03 14:05:12.000000 cubicweb-varnish-1.0.0/cubicweb_varnish.egg-info/not-zip-safe
+-rw-r--r--   0 fferry    (1000) fferry    (1000)       24 2023-07-11 08:02:07.000000 cubicweb-varnish-1.0.0/cubicweb_varnish.egg-info/requires.txt
+-rw-r--r--   0 fferry    (1000) fferry    (1000)       17 2023-07-11 08:02:07.000000 cubicweb-varnish-1.0.0/cubicweb_varnish.egg-info/top_level.txt
+-rw-r--r--   0 fferry    (1000) fferry    (1000)       38 2023-07-11 08:02:07.324325 cubicweb-varnish-1.0.0/setup.cfg
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     2596 2023-07-07 12:18:41.000000 cubicweb-varnish-1.0.0/setup.py
+drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-07-11 08:02:07.324325 cubicweb-varnish-1.0.0/test/
+drwxr-xr-x   0 fferry    (1000) fferry    (1000)        0 2023-07-11 08:02:07.324325 cubicweb-varnish-1.0.0/test/data/
+-rw-r--r--   0 fferry    (1000) fferry    (1000)        8 2023-07-03 14:02:20.000000 cubicweb-varnish-1.0.0/test/data/bootstrap_cubes
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     2395 2023-07-03 14:02:20.000000 cubicweb-varnish-1.0.0/test/pytestconf.py
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     1737 2023-07-03 14:02:20.000000 cubicweb-varnish-1.0.0/test/test_varnish.py
+-rw-r--r--   0 fferry    (1000) fferry    (1000)     1071 2023-07-11 08:01:22.000000 cubicweb-varnish-1.0.0/tox.ini
```

### Comparing `cubicweb-varnish-0.8.0/PKG-INFO` & `cubicweb-varnish-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: cubicweb-varnish
-Version: 0.8.0
+Version: 1.0.0
 Summary: cubicweb varnish helper
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/cubicweb-varnish
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL-2.1
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: JavaScript
 
 Summary
 -------
@@ -60,9 +59,7 @@
 
 Dependencies
 ------------
 
 http://www.varnish-cache.org/
 
 or apt-get install varnish (for debian derived distributions)
-
-
```

### Comparing `cubicweb-varnish-0.8.0/README.rst` & `cubicweb-varnish-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-varnish-0.8.0/__pkginfo__.py` & `cubicweb-varnish-1.0.0/__pkginfo__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # pylint: disable=W0622
 """cubicweb-varnish application packaging information"""
 
 modname = "cubicweb_varnish"
 distname = "cubicweb-varnish"
 
-numversion = (0, 8, 0)
+numversion = (1, 0, 0)
 version = ".".join(str(num) for num in numversion)
 
 license = "LGPL-2.1"
 author = "LOGILAB S.A. (Paris, FRANCE)"
 author_email = "contact@logilab.fr"
 description = "cubicweb varnish helper"
-web = "https://forge.extranet.logilab.fr/cubicweb/cubes/%s" % distname
+web = f"https://forge.extranet.logilab.fr/cubicweb/cubes/{distname}"
 
 __depends__ = {
-    "cubicweb": ">= 3.31.0, < 3.39.0",
+    "cubicweb": ">= 3.31.0, < 5.0.0",
 }
 __recommends__ = {}
 
 classifiers = [
     "Environment :: Web Environment",
     "Framework :: CubicWeb",
     "Programming Language :: Python :: 3",
```

### Comparing `cubicweb-varnish-0.8.0/cubicweb_varnish/__pkginfo__.py` & `cubicweb-varnish-1.0.0/cubicweb_varnish/__pkginfo__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # pylint: disable=W0622
 """cubicweb-varnish application packaging information"""
 
 modname = "cubicweb_varnish"
 distname = "cubicweb-varnish"
 
-numversion = (0, 8, 0)
+numversion = (1, 0, 0)
 version = ".".join(str(num) for num in numversion)
 
 license = "LGPL-2.1"
 author = "LOGILAB S.A. (Paris, FRANCE)"
 author_email = "contact@logilab.fr"
 description = "cubicweb varnish helper"
-web = "https://forge.extranet.logilab.fr/cubicweb/cubes/%s" % distname
+web = f"https://forge.extranet.logilab.fr/cubicweb/cubes/{distname}"
 
 __depends__ = {
-    "cubicweb": ">= 3.31.0, < 3.39.0",
+    "cubicweb": ">= 3.31.0, < 5.0.0",
 }
 __recommends__ = {}
 
 classifiers = [
     "Environment :: Web Environment",
     "Framework :: CubicWeb",
     "Programming Language :: Python :: 3",
```

### Comparing `cubicweb-varnish-0.8.0/cubicweb_varnish/entities.py` & `cubicweb-varnish-1.0.0/cubicweb_varnish/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-varnish-0.8.0/cubicweb_varnish/hooks.py` & `cubicweb-varnish-1.0.0/cubicweb_varnish/hooks.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,14 +51,14 @@
         if varnish_version == 2:
             purge_cmd = "purge.url"
         elif varnish_version == 3:
             purge_cmd = "ban.url"
         elif varnish_version >= 4:
             purge_cmd = "ban req.url ~"
         else:
-            raise ValueError("Unsupported varnish version %s" % varnish_version)
+            raise ValueError(f"Unsupported varnish version {varnish_version}")
         cnxs = varnish_cli_connect_from_config(config)
         for url in self.get_data():
             for varnish_cli in cnxs:
-                varnish_cli.execute(purge_cmd, "^%s$" % urlparse(url).path)
+                varnish_cli.execute(purge_cmd, f"^{urlparse(url).path}$")
         for varnish_cli in cnxs:
             varnish_cli.close()
```

### Comparing `cubicweb-varnish-0.8.0/cubicweb_varnish/migration/postcreate.py` & `cubicweb-varnish-1.0.0/cubicweb_varnish/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-varnish-0.8.0/cubicweb_varnish/site_cubicweb.py` & `cubicweb-varnish-1.0.0/cubicweb_varnish/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-varnish-0.8.0/cubicweb_varnish/varnishadm.py` & `cubicweb-varnish-1.0.0/cubicweb_varnish/varnishadm.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 
     def _receive(self):
         code, length = self._rfile.readline().split()
         msg = self._rfile.read(int(length) + 1).strip()
         return int(code), msg
 
     def _send(self, instruction):
-        self._wfile.write("%s\n" % instruction)
+        self._wfile.write(f"{instruction}\n")
         self._wfile.flush()
         return self._receive()
 
     # contextmanager interface ###############################################
     def __enter__(self):
         return self
```

### Comparing `cubicweb-varnish-0.8.0/cubicweb_varnish/views.py` & `cubicweb-varnish-1.0.0/cubicweb_varnish/views.py`

 * *Files identical despite different names*

### Comparing `cubicweb-varnish-0.8.0/cubicweb_varnish.egg-info/PKG-INFO` & `cubicweb-varnish-1.0.0/cubicweb_varnish.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: cubicweb-varnish
-Version: 0.8.0
+Version: 1.0.0
 Summary: cubicweb varnish helper
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/cubicweb-varnish
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL-2.1
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: JavaScript
 
 Summary
 -------
@@ -60,9 +59,7 @@
 
 Dependencies
 ------------
 
 http://www.varnish-cache.org/
 
 or apt-get install varnish (for debian derived distributions)
-
-
```

### Comparing `cubicweb-varnish-0.8.0/cubicweb_varnish.egg-info/SOURCES.txt` & `cubicweb-varnish-1.0.0/cubicweb_varnish.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-varnish-0.8.0/setup.py` & `cubicweb-varnish-1.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -52,17 +52,15 @@
 # get optional metadatas
 data_files = __pkginfo__.get("data_files", None)
 dependency_links = __pkginfo__.get("dependency_links", ())
 
 requires = {}
 for entry in ("__depends__",):  # "__recommends__"):
     requires.update(__pkginfo__.get(entry, {}))
-install_requires = [
-    "{} {}".format(d, v and v or "").strip() for d, v in requires.items()
-]
+install_requires = [f"{d} {v and v or ''}".strip() for d, v in requires.items()]
 
 
 setup(
     name=distname,
     version=version,
     license=license,
     description=description,
```

### Comparing `cubicweb-varnish-0.8.0/test/pytestconf.py` & `cubicweb-varnish-1.0.0/test/pytestconf.py`

 * *Files identical despite different names*

### Comparing `cubicweb-varnish-0.8.0/test/test_varnish.py` & `cubicweb-varnish-1.0.0/test/test_varnish.py`

 * *Files identical despite different names*

### Comparing `cubicweb-varnish-0.8.0/tox.ini` & `cubicweb-varnish-1.0.0/tox.ini`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tox]
-envlist = py3,flake8,yamllint
+envlist = py3,flake8,yamllint,black
 
 [testenv]
 deps =
   pytest
   webtest
   git+https://github.com/psycojoker/pytest-capture-deprecatedwarnings
 commands =
@@ -25,15 +25,15 @@
   check-manifest
 commands =
   {envpython} -m check_manifest {toxinidir}
 
 [testenv:pypi-publish]
 basepython = python3
 skip_install = true
-whitelist_externals = rm
+allowlist_externals = rm
 deps =
   twine
 passenv =
   TWINE_USERNAME
   TWINE_PASSWORD
 commands =
   rm -rf build dist .egg .egg-info
@@ -42,7 +42,21 @@
   twine upload --skip-existing dist/*
 
 [testenv:yamllint]
 skip_install = true
 deps = yamllint
 commands =
   yamllint .
+
+[testenv:black]
+basepython = python3
+skip_install = true
+deps =
+  black >= 22.12
+commands = black --check .
+
+[testenv:black-run]
+basepython = python3
+skip_install = true
+deps =
+  black >= 22.12
+commands = black .
```

