# Comparing `tmp/kevlar-system-inspector-1.0.1.tar.gz` & `tmp/kevlar-system-inspector-1.1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/builds/wrlx-octane/kevlar-inspector/dist/.tmp-y4s_az4f/kevlar-system-inspector-1.0.1.tar", last modified: Tue Apr 18 21:22:58 2023, max compression
+gzip compressed data, was "/builds/wrlx-octane/kevlar-inspector/dist/.tmp-s4dsz_p2/kevlar-system-inspector-1.1.0a1.tar", last modified: Mon Jul 10 21:23:19 2023, max compression
```

## Comparing `kevlar-system-inspector-1.0.1.tar` & `kevlar-system-inspector-1.1.0a1.tar`

### file list

```diff
@@ -1,49 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 21:22:58.000000 kevlar-system-inspector-1.0.1/
--rw-rw-rw-   0 root         (0) root         (0)     1078 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5085 2023-04-18 21:22:58.000000 kevlar-system-inspector-1.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4056 2023-04-18 21:00:38.000000 kevlar-system-inspector-1.0.1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)       82 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 21:22:58.000000 kevlar-system-inspector-1.0.1/scripts/
--rwxrwxrwx   0 root         (0) root         (0)       71 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/scripts/kevlar-system-inspector
--rw-rw-rw-   0 root         (0) root         (0)     1351 2023-04-18 21:22:58.000000 kevlar-system-inspector-1.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      124 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 21:22:58.000000 kevlar-system-inspector-1.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 21:22:58.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/
--rw-rw-rw-   0 root         (0) root         (0)     6110 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     6310 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)    16848 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/console.py
--rw-rw-rw-   0 root         (0) root         (0)     3713 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     6470 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/output.py
--rw-rw-rw-   0 root         (0) root         (0)     8240 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 21:22:58.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/resources/
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/resources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1272 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/sysinfo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 21:22:58.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/templates/
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1004 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/templates/failures.rst
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/templates/html5-template.txt
--rw-rw-rw-   0 root         (0) root         (0)     3215 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/templates/report.rst
--rw-rw-rw-   0 root         (0) root         (0)    11687 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/templates/starlab.css
--rw-rw-rw-   0 root         (0) root         (0)      330 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/templates/warnings.rst
--rw-rw-rw-   0 root         (0) root         (0)     9266 2023-04-18 21:00:38.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/test_allowlisting.py
--rw-rw-rw-   0 root         (0) root         (0)    12847 2023-04-18 21:00:38.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/test_kernel_config.py
--rw-rw-rw-   0 root         (0) root         (0)     5870 2023-04-18 21:00:38.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/test_kernel_modules.py
--rw-rw-rw-   0 root         (0) root         (0)     2978 2023-04-18 21:00:38.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/test_offline_integrity.py
--rw-rw-rw-   0 root         (0) root         (0)     4631 2023-04-18 21:00:38.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/test_secure_dns.py
--rw-rw-rw-   0 root         (0) root         (0)     2714 2023-04-18 21:00:38.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/test_systemd_syscall_filtering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 21:22:58.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/utils/
--rw-rw-rw-   0 root         (0) root         (0)      565 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1271 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/utils/elf.py
--rw-rw-rw-   0 root         (0) root         (0)     4226 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/utils/kconfig.py
--rw-rw-rw-   0 root         (0) root         (0)      884 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/utils/modules.py
--rw-rw-rw-   0 root         (0) root         (0)     3943 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/utils/mount.py
--rw-rw-rw-   0 root         (0) root         (0)     4631 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/utils/systemd.py
--rw-rw-rw-   0 root         (0) root         (0)     2289 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/utils/workdir.py
--rw-rw-rw-   0 root         (0) root         (0)      294 2023-04-18 21:00:38.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 21:22:58.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5085 2023-04-18 21:22:58.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1674 2023-04-18 21:22:58.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 21:22:58.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2023-04-18 21:22:58.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-04-18 21:22:58.000000 kevlar-system-inspector-1.0.1/src/kevlar_system_inspector.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:23:19.000000 kevlar-system-inspector-1.1.0a1/
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.1.0a1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5089 2023-07-10 21:23:19.000000 kevlar-system-inspector-1.1.0a1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4058 2023-05-16 13:17:40.000000 kevlar-system-inspector-1.1.0a1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)       82 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.1.0a1/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:23:19.000000 kevlar-system-inspector-1.1.0a1/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)       71 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.1.0a1/scripts/kevlar-system-inspector
+-rw-rw-rw-   0 root         (0) root         (0)     1353 2023-07-10 21:23:19.000000 kevlar-system-inspector-1.1.0a1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.1.0a1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:23:19.000000 kevlar-system-inspector-1.1.0a1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:23:19.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/
+-rw-rw-rw-   0 root         (0) root         (0)     6827 2023-06-16 17:53:59.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6310 2023-05-23 12:08:31.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)    16780 2023-06-16 18:06:26.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/console.py
+-rw-rw-rw-   0 root         (0) root         (0)     4161 2023-06-13 18:38:19.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     6821 2023-06-16 14:27:46.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/output.py
+-rw-rw-rw-   0 root         (0) root         (0)    11579 2023-06-16 21:44:19.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:23:19.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/resources/
+-rw-rw-rw-   0 root         (0) root         (0)       49 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1272 2023-05-23 12:08:31.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/sysinfo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:23:19.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/templates/
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/templates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1158 2023-06-16 21:44:19.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/templates/failures.rst
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/templates/html5-template.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3295 2023-06-16 17:50:38.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/templates/report.rst
+-rw-rw-rw-   0 root         (0) root         (0)    11687 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/templates/starlab.css
+-rw-rw-rw-   0 root         (0) root         (0)      354 2023-06-16 18:06:26.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/templates/successes.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-16 14:24:35.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/templates/summary.rst
+-rw-rw-rw-   0 root         (0) root         (0)      330 2023-04-14 16:14:11.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/templates/warnings.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5360 2023-06-16 21:44:19.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/test_allowlisting.py
+-rw-rw-rw-   0 root         (0) root         (0)     7875 2023-06-16 21:44:19.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/test_kernel_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      650 2023-06-16 19:17:04.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/test_kernel_sandboxing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2835 2023-06-16 17:50:38.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/test_offline_integrity.py
+-rw-rw-rw-   0 root         (0) root         (0)     6668 2023-06-16 21:44:19.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/test_secure_networking.py
+-rw-rw-rw-   0 root         (0) root         (0)     2000 2023-06-16 21:44:19.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/test_systemd_syscall_filtering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:23:19.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      565 2023-05-23 12:08:31.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      250 2023-07-06 18:45:08.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/utils/access.py
+-rw-rw-rw-   0 root         (0) root         (0)     1271 2023-05-23 12:08:31.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/utils/elf.py
+-rw-rw-rw-   0 root         (0) root         (0)     4226 2023-05-23 12:08:31.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/utils/kconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)     1590 2023-06-13 16:06:35.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/utils/modules.py
+-rw-rw-rw-   0 root         (0) root         (0)     3943 2023-05-23 12:08:31.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/utils/mount.py
+-rw-rw-rw-   0 root         (0) root         (0)     4631 2023-05-23 12:08:31.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/utils/systemd.py
+-rw-rw-rw-   0 root         (0) root         (0)     2825 2023-07-06 18:45:08.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/utils/workdir.py
+-rw-rw-rw-   0 root         (0) root         (0)      296 2023-05-16 13:17:40.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-10 21:23:19.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5089 2023-07-10 21:23:19.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1830 2023-07-10 21:23:19.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-10 21:23:19.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2023-07-10 21:23:19.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-07-10 21:23:19.000000 kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector.egg-info/top_level.txt
```

### Comparing `kevlar-system-inspector-1.0.1/LICENSE` & `kevlar-system-inspector-1.1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.1/PKG-INFO` & `kevlar-system-inspector-1.1.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kevlar-system-inspector
-Version: 1.0.1
+Version: 1.1.0a1
 Summary: A security scanner for Linux systems
 Home-page: https://www.starlab.io/explore-kevlar-system-inspector
 Author: Star Lab
 Author-email: info@starlab.io
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -96,15 +96,15 @@
 copied this tarball to your device, you can simply extract and run:
 
 .. code-block:: console
 
    $ tar xf ./kevlar-system-inspector-standalone.tar.gz
    $ sudo ./kevlar-system-inspector-standalone/kevlar-system-inspector
 
-.. _standalone tarball: https://inspector.starlab.io/kevlar-system-inspector-standalone-v1.0.1.tar.gz
+.. _standalone tarball: https://inspector.starlab.io/kevlar-system-inspector-standalone-v1.1.01a.tar.gz
 
 
 Running as Root
 ===============
 
 Although running as root is not necessary, Kevlar System Inspector is designed
 to be run as root in a embedded test environment for two reasons:
```

### Comparing `kevlar-system-inspector-1.0.1/README.rst` & `kevlar-system-inspector-1.1.0a1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 copied this tarball to your device, you can simply extract and run:
 
 .. code-block:: console
 
    $ tar xf ./kevlar-system-inspector-standalone.tar.gz
    $ sudo ./kevlar-system-inspector-standalone/kevlar-system-inspector
 
-.. _standalone tarball: https://inspector.starlab.io/kevlar-system-inspector-standalone-v1.0.1.tar.gz
+.. _standalone tarball: https://inspector.starlab.io/kevlar-system-inspector-standalone-v1.1.01a.tar.gz
 
 
 Running as Root
 ===============
 
 Although running as root is not necessary, Kevlar System Inspector is designed
 to be run as root in a embedded test environment for two reasons:
```

### Comparing `kevlar-system-inspector-1.0.1/setup.cfg` & `kevlar-system-inspector-1.1.0a1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = kevlar-system-inspector
-version = 1.0.1
+version = 1.1.0a1
 author = Star Lab
 author_email = info@starlab.io
 url = https://www.starlab.io/explore-kevlar-system-inspector
 license = MIT
 license_files = LICENSE
 description = A security scanner for Linux systems
 long_description = file: README.rst
```

### Comparing `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/__init__.py` & `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,19 +14,29 @@
 # imports
 _THIS_DIR = os.path.abspath(os.path.dirname(__file__))
 _VENDOR_ZIP = os.path.join(_THIS_DIR, "_vendor.zip")
 sys.path.insert(0, _VENDOR_ZIP)
 
 import pytest
 
-from .console import ConsoleProgress, ConsoleReporter
+from .console import ConsoleProgress
 from .report import KevlarReporter
-from .output import HtmlReporter, RstReporter, ConsoleTestLister, CsvTestLister
+from .output import (
+    HtmlReporter,
+    RstReporter,
+    ConsoleTestLister,
+    CsvTestLister,
+    ConsoleReporter,
+    TextReporter,
+    SummaryReporter,
+)
 from .version import get_version
 
+DEFAULT_OUTPUT_FILE = "kevlar-system-inspector-report.txt"
+
 
 class Tweaks:
     """Misc things to get around the fact that we are disabling default plugins"""
 
     def pytest_configure(self, config: "pytest.Config") -> None:
         # These are usually set by terminal plugin. Various bits of pytest expect them to
         # be set. Mostly an issue only when we want to break into pdb.
@@ -54,20 +64,27 @@
 
 
 def main() -> None:
     system_check()
     parser = argparse.ArgumentParser(description=__doc__)
     output = parser.add_argument_group("Output Options")
     output.add_argument(
+        "--output",
+        action="store",
+        help=f"""
+             Print plaint text report to a file. This is the default, unless
+             any of the other --ouput-* options are given. The default file
+             name is {DEFAULT_OUTPUT_FILE!r}.
+             """,
+    )
+    output.add_argument(
         "--output-console",
         action="store_true",
         help="""
-             Print formatted console output. This is the default, unless any of
-             the other --ouput-* options are given. This option exists to turn
-             console output back on.
+             Print formatted console output.
              """,
     )
     output.add_argument(
         "--output-html",
         action="store",
         help="Write an HTML output report to the given file.",
     )
@@ -119,41 +136,52 @@
     # Undocumented options:
     #   --debug: turn on regular pytest output
     #   --pytest: Pass arbitrary args to pytest
     #   --debug-coverate: Generate code coverage info
     parser.add_argument("--debug", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--pytest", action="store", help=argparse.SUPPRESS)
     parser.add_argument("--debug-coverage", action="store_true", help=argparse.SUPPRESS)
+    parser.add_argument("--force-fail-all", action="store_true", help=argparse.SUPPRESS)
 
     args = parser.parse_args()
 
-    terminal_color_options = {"auto": None, "always": True, "never": False}
-    terminal_color = terminal_color_options[args.terminal_color]
-
-    args.output_console = args.output_console or not (
-        args.output_html or args.output_rst
-    )
-
-    pytest_args = ["--pyargs", __name__]
+    if args.terminal_color == "always":
+        os.environ["FORCE_COLOR"] = "1"
+    elif args.terminal_color == "never":
+        os.environ["TERM"] = "unknown"
+
+    if not any([args.output, args.output_console, args.output_html, args.output_rst]):
+        # Default: text report only
+        args.output = DEFAULT_OUTPUT_FILE
+
+    # To isolate from any conftest.py or directories with test_*.py in them,
+    # use path rather than --pyargs, and explicitly set the root directory.
+    pytest_args = [_THIS_DIR, "--rootdir", _THIS_DIR]
     plugins: List[Any] = [Tweaks()]
 
     if args.list_tests:
         if isinstance(args.list_tests, str):
-            plugins.append(CsvTestLister(args.list_tests, terminal_color))
+            plugins.append(CsvTestLister(args.list_tests))
         else:
-            plugins.append(ConsoleTestLister(terminal_color))
+            plugins.append(ConsoleTestLister())
         pytest_args.append("--collect-only")
     else:
-        plugins.extend([KevlarReporter(), ConsoleProgress(terminal_color)])
-        if args.output_console:
-            plugins.append(ConsoleReporter(terminal_color))
+        plugins.extend(
+            [KevlarReporter(force_fail=args.force_fail_all), ConsoleProgress()]
+        )
+        if args.output:
+            plugins.append(TextReporter(args.output))
         if args.output_html:
-            plugins.append(HtmlReporter(args.output_html, terminal_color))
+            plugins.append(HtmlReporter(args.output_html))
         if args.output_rst:
-            plugins.append(RstReporter(args.output_rst, terminal_color))
+            plugins.append(RstReporter(args.output_rst))
+        if args.output_console:
+            plugins.append(ConsoleReporter())
+        else:
+            plugins.append(SummaryReporter())
 
     if args.debug_coverage:
         try:
             import pytest_cov  # type: ignore # noqa: 401
         except ImportError:
             parser.error("ptest-cov module not installed. Cannot generate coverage.")
         pytest_args.extend(
```

### Comparing `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/conftest.py` & `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/conftest.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/console.py` & `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/console.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Plugin to print progress as we go
 """
 
 import copy
 import re
-from typing import Set, Optional, List, Any, Generator, Union, Callable
+from typing import Set, Optional, List, Any, Generator, Union, Callable, TextIO
 
 from docutils.nodes import NodeVisitor, SkipNode
 import docutils.nodes
 import pytest
 from rich.console import Console, Group, ConsoleOptions
 from rich.errors import MissingStyle
 from rich.padding import Padding
@@ -18,16 +18,14 @@
 from rich.style import Style
 from rich.syntax import Syntax
 from rich.table import Table
 from rich.text import Text
 from rich.theme import Theme
 from pygments.lexers import LEXERS
 
-from .report import TestReport
-
 ALL_LEXERS: Set[str] = set()
 for lexers in LEXERS.values():
     ALL_LEXERS.update(lexers[1])
 
 THEME = Theme(
     {
         "h1": Style(bold=True),
@@ -48,18 +46,18 @@
         "admonition-issue.border": Style(bold=True),
         "term": Style(bold=True),
     }
 )
 
 
 class ConsoleProgress:
-    def __init__(self, terminal_color: Optional[bool]):
+    def __init__(self) -> None:
         self.total = 0
         self.curr_weight = 0
-        self.console = Console(force_terminal=terminal_color, theme=THEME)
+        self.console = Console(theme=THEME)
         self.progress = Progress(console=self.console)
         self.task: Any = None  # opaque value
 
     def pytest_itemcollected(self, item: "pytest.Function") -> None:
         self.total += getattr(item.function, "weight", 1)
 
     @pytest.hookimpl(hookwrapper=True)
@@ -319,14 +317,16 @@
     depart_emphasis = styled_text_depart
     visit_strong = container_visit
     depart_strong = styled_text_depart
     visit_inline = container_visit
     depart_inline = styled_text_depart
     visit_literal = container_visit
     depart_literal = styled_text_depart
+    visit_line_block = container_visit
+    depart_line_block = container_depart
 
     def visit_literal_block(self, node: docutils.nodes.literal_block) -> None:
         possible_lexers = [cls for cls in node["classes"] if cls in ALL_LEXERS]
         lexer = possible_lexers[0] if possible_lexers else None
         self.insert_line_break()
         self.elements.append(Syntax(node.astext(), theme="default", lexer=lexer))
         # self.elements.append("")
@@ -510,16 +510,14 @@
         else:
             self.context.table.add_row(*context.elements)
 
     visit_entry = container_visit
     depart_entry = container_depart
 
 
-class ConsoleReporter:
+def print_document(
+    document: docutils.nodes.document, file: Optional[TextIO] = None, **kwargs: Any
+) -> None:
     """Display the report on the console. Depends on KevlarReporter"""
-
-    def __init__(self, terminal_color: Optional[bool]):
-        self.console = Console(force_terminal=terminal_color, theme=THEME)
-
-    def pytest_kevlar_report(self, report: TestReport) -> None:
-        printer = ConsolePrinter(report.document)
-        self.console.print(printer)
+    printer = ConsolePrinter(document)
+    console = Console(file=file, theme=THEME, **kwargs)
+    console.print(printer)
```

### Comparing `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/decorators.py` & `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/decorators.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from typing import Any, Callable, TypeVar, cast, Union, List
+from typing import Any, Callable, TypeVar, cast, Union, List, overload
 import re
 import importlib
 import textwrap
 import inspect
+import warnings
 
 import pytest
 
 F = TypeVar("F", bound=Callable[..., Any])
 
 
 def weight(value: float) -> Callable[[F], F]:
@@ -17,14 +18,24 @@
     def decorator(func: F) -> F:
         cast(Any, func).weight = value
         return func
 
     return decorator
 
 
+@overload
+def full_version_only(__func: F) -> F:
+    ...
+
+
+@overload
+def full_version_only(__name: str) -> Callable[[F], F]:
+    ...
+
+
 def full_version_only(func_or_name: Union[F, str]) -> Union[F, Callable[[F], F]]:
     """
     Mark a test as implemented in the full version only.
 
     May be called in two forms:
 
         @full_version_only
@@ -32,30 +43,32 @@
             ...
 
         @full_version_only("module.name:function_name")
         def test_foo_bar():
             ...
     """
 
-    def mismatch_placeholder() -> None:
+    def mismatch_placeholder(*args: Any) -> None:
         pytest.fail("**Version mismatch!** Could not find function implementation")
 
-    def lite_version_placeholder() -> None:
-        pytest.fail(
+    def lite_version_placeholder(*args: Any) -> None:
+        warnings.warn(
             textwrap.dedent(
                 """\
-            **This test was skipped.**
+                **Some tests were skipped.**
 
-            This test is only available in the full version of Kevlar System
-            Inspector.  Please contact `Star Lab`__ for more information.
+                Some tests are only available in the full version of Kevlar
+                System Inspector.  Please contact `Star Lab`__ for more
+                information.
 
-            .. __: https://www.starlab.io/contact-us-kevlar-system-inspector-user
-            """
+                .. __: https://www.starlab.io/contact-us-kevlar-system-inspector-user
+                """
             )
         )
+        pytest.skip("not present")
 
     def get_params(func: Any) -> List[str]:
         return list(inspect.signature(func).parameters)
 
     def decorator(func: F) -> F:
         try:
             module = importlib.import_module(module_name)
@@ -85,16 +98,20 @@
                     fixture_names.extend(get_params(fixture))
 
         # Mark it for introspection
         full_func = pytest.mark.full_version_only(full_func)
 
         # Replace it wholesale so that pytest sees the fixtures of the the
         # implementation function, but copy over the documentation first so
-        # that we don't have to duplicate.
+        # that we don't have to duplicate. Other attributes are for unit
+        # testing.
         full_func.__doc__ = func.__doc__
+        full_func.__module__ = func.__module__
+        full_func.__name__ = func.__name__
+        full_func.__qualname__ = func.__qualname__
         return cast(F, full_func)
 
     if isinstance(func_or_name, str):
         assert ":" in func_or_name, "Expecting locator of the form 'module:function'"
         module_name, func_name = func_or_name.split(":", 1)
         return decorator
     else:
```

### Comparing `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/output.py` & `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/output.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,34 +2,34 @@
 Output of reports in various formats, as pytest plugins
 """
 
 import csv
 from dataclasses import dataclass
 import os
 from types import ModuleType, FunctionType
-from typing import Optional, Dict, Set, List, cast
+from typing import Dict, Set, List, cast
 from collections import defaultdict
 import xml.etree.ElementTree as ET
 
 import docutils.core
 from rich.console import Console
 from rich.table import Table
 from rich.panel import Panel
 from rich.text import Text
 
 from . import templates
 from .report import TestReport
+from .console import print_document
 
 import pytest
 
 
 class HtmlReporter:
-    def __init__(self, filename: str, terminal_color: Optional[bool]):
+    def __init__(self, filename: str):
         self.filename = filename
-        self.terminal_color = terminal_color
 
     def pytest_kevlar_report(self, report: TestReport) -> None:
         templates_dir = os.path.dirname(templates.__file__)
         template = os.path.join(templates_dir, "html5-template.txt")
         stylesheet = os.path.join(templates_dir, "starlab.css")
 
         with open(self.filename, "wb") as fp:
@@ -41,28 +41,55 @@
                     settings_overrides={
                         "stylesheet_path": stylesheet,
                         "template": template,
                     },
                 )
             )
 
-        console = Console(force_terminal=self.terminal_color)
-        console.print(f"Printed HTML output to '{self.filename}'")
+        console = Console()
+        console.print(f"Printed detailed report (HTML) to '{self.filename}'")
 
 
 class RstReporter:
-    def __init__(self, filename: str, terminal_color: Optional[bool]):
+    def __init__(self, filename: str):
         self.filename = filename
-        self.terminal_color = terminal_color
 
     def pytest_kevlar_report(self, report: TestReport) -> None:
-        console = Console(force_terminal=self.terminal_color)
+        console = Console()
         with open(self.filename, "w") as fp:
             fp.write(report.document_source)
-        console.print(f"Printed reStructuredText output to '{self.filename}'")
+        console.print(
+            f"Printed detailed report (reStructuredText) to '{self.filename}'"
+        )
+
+
+class ConsoleReporter:
+    def pytest_kevlar_report(self, report: TestReport) -> None:
+        print_document(report.document)
+
+
+class TextReporter:
+    def __init__(self, filename: str):
+        self.filename = filename
+
+    def pytest_kevlar_report(self, report: TestReport) -> None:
+        with open(self.filename, "w") as fp:
+            print_document(report.document, file=fp, width=80)
+        console = Console()
+        console.print(f"Printed detailed report (plain text) to '{self.filename}'")
+
+
+class SummaryReporter:
+    """
+    Stuff that gets printed in lieu of the full report, when we write to a file.
+    """
+
+    def pytest_kevlar_report(self, report: TestReport) -> None:
+        print_document(report.summary)
+        print()
 
 
 @dataclass
 class TestItem:
     title: str
     references: Set[str]
     full_version_only: bool
@@ -71,17 +98,14 @@
 @dataclass
 class TestCategory:
     title: str
     items: List[TestItem]
 
 
 class TestListerBase:
-    def __init__(self, terminal_color: Optional[bool]):
-        self.terminal_color = terminal_color
-
     def pytest_collection_finish(self, session: pytest.Session) -> None:
         # So that we don't have to tag all our tests with additional metadata,
         # we will create a report document with all tests, and then parse the
         # document structure for the info we need.  Any metadata that we do
         # need to tag can be inserted into the documentation along with
         # everything else.
 
@@ -137,15 +161,15 @@
         if title is None:
             return "<undocumented>"
         return "".join(title.itertext())
 
 
 class ConsoleTestLister(TestListerBase):
     def print_output(self, listing: List[TestCategory]) -> None:
-        console = Console(force_terminal=self.terminal_color)
+        console = Console()
         grid = Table.grid()
         grid.add_column()
         grid.add_row(
             Panel(
                 Text(
                     "Tests Included with Kevlar System Inspector",
                     justify="center",
@@ -168,23 +192,22 @@
                     "*" if test_item.full_version_only else "",
                 )
             grid.add_row(table)
         console.print(grid)
 
 
 class CsvTestLister(TestListerBase):
-    def __init__(self, filename: str, terminal_color: Optional[bool]):
-        self.terminal_color = terminal_color
+    def __init__(self, filename: str):
         self.filename = filename
 
     def print_output(self, listing: List[TestCategory]) -> None:
         with open(self.filename, "w") as csvfile:
             writer = csv.writer(csvfile)
             writer.writerow(["Title", "Category", "References", "Full Version"])
 
             for category in listing:
                 for test_item in category.items:
                     references = " ".join(sorted(test_item.references))
                     full = "*" if test_item.full_version_only else ""
                     writer.writerow([test_item.title, category.title, references, full])
-        console = Console(force_terminal=self.terminal_color)
+        console = Console()
         console.print(f"Printed CSV listing to '{self.filename}'")
```

### Comparing `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/report.py` & `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/report.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,30 +8,30 @@
 import warnings
 from dataclasses import dataclass
 
 import docutils.core
 import docutils.nodes
 import docutils.utils
 from docutils.parsers.rst import roles, states
-from jinja2 import Environment, PackageLoader, select_autoescape
+from jinja2 import Environment, PackageLoader
 
 # Below, we do type annotations for pytest things in quotes, because some of
 # them aren't publicly exposed until version 7.0. That only matters for mypy
 # checking, so putting them in quotes means Python won't care about them at
 # runtime.
 import pytest
 
 from .version import is_full_version
 from .sysinfo import get_system_info
 from .version import VERSION
 
 
 JINJA_ENV = Environment(
     loader=PackageLoader(__package__),
-    autoescape=select_autoescape(),
+    autoescape=False,
 )
 JINJA_ENV.filters["dedent"] = textwrap.dedent
 
 
 # Code to register a custom role for our test documentation:
 #
 #   :kevlar-code:`300` which generates a link to our webpage and inserts
@@ -105,52 +105,117 @@
                 message = message.split(":", 1)[1].strip()
             else:
                 is_internal = True
                 message = str(pytest_report.longrepr)  # full crash, if available
         return cls(message=message, is_internal=is_internal)
 
 
-class TestFailure:
+def find_title(documentation: str) -> Optional[str]:
+    # Some skipped tests with parametrized documentation will warn. Since
+    # we're not going to show them, just don't print out anything.
+    document = docutils.core.publish_doctree(
+        documentation, settings_overrides={"report_level": 5}
+    )
+    try:
+        title = next(document.findall(lambda n: n.tagname == "title"))
+        return str(title.rawsource)
+    except StopIteration:
+        return None
+
+
+class TestOutcome:
     def __init__(self, item: "pytest.Function"):
         self.item = item
         self.documentation = item.function.__doc__
+        self.title = None
+        if not self.documentation:
+            self.documentation = getattr(item.cls, "__doc__", None)
+
         self.tags = {mark.name for mark in item.iter_markers()}
         if self.documentation:
             vars = item.function.__globals__.copy()
             try:
                 vars["fixture_names"] = item.callspec.params
                 vars.update(item.callspec.params)
             except AttributeError:
                 pass
             vars.update(item.funcargs)
             template = JINJA_ENV.from_string(textwrap.dedent(self.documentation))
             self.documentation = template.render(vars)
-        self.causes: Dict[
+            self.title = find_title(self.documentation)
+
+        self.failures: Dict[
             FailureCause, int
         ] = {}  # set-like, to preserve insertion order
+        self.skipped = False
+
+    def add_failure(self, pytest_report: "pytest.TestReport") -> None:
+        self.failures[FailureCause.from_pytest(pytest_report)] = 1
 
-    def add_report(self, pytest_report: "pytest.TestReport") -> None:
-        self.causes[FailureCause.from_pytest(pytest_report)] = 1
+    @property
+    def failed(self) -> bool:
+        return bool(self.failures)
+
+    @property
+    def succeeded(self) -> bool:
+        return not self.failures and not self.skipped
 
 
 class TestModule:
     """
     Holds the module documentation, and lets us group in a dict by module.
     """
 
     def __init__(self, item: "pytest.Function"):
         self.module = item.module
         self.documentation = item.module.__doc__
+        self.title = None
         self.tags = {mark.name for mark in item.iter_markers()}
         if self.documentation:
             template = JINJA_ENV.from_string(textwrap.dedent(self.documentation))
             self.documentation = template.render(item.module.__dict__)
+            self.title = find_title(self.documentation)
+
+        # Individual tests, grouped by base (non-parametrized) nodeid
+        self.tests: Dict[str, TestOutcome] = {}
+
+    @property
+    def any_failures(self) -> bool:
+        return any(t.failed for t in self.tests.values())
+
+    @property
+    def any_successes(self) -> bool:
+        return any(not t.failed for t in self.tests.values())
+
+    @property
+    def failures(self) -> List[Tuple[str, TestOutcome]]:
+        return [(nodeid, t) for nodeid, t in self.tests.items() if t.failed]
+
+    @property
+    def successes(self) -> List[Tuple[str, TestOutcome]]:
+        return [(nodeid, t) for nodeid, t in self.tests.items() if t.succeeded]
+
+    @property
+    def failure_count(self) -> int:
+        return sum(1 for t in self.tests.values() if t.failed)
+
+    @property
+    def success_count(self) -> int:
+        return sum(1 for t in self.tests.values() if not t.failed)
+
 
-        # Failures, grouped by base (non-parametrized) nodeid
-        self.failures: Dict[str, TestFailure] = {}
+def get_base_nodeid(item: "pytest.Function") -> str:
+    if getattr(item.cls, "merge_tests", False):
+        # Merge by class
+        return item.nodeid.rsplit("::", 1)[0]
+    elif getattr(item.function, "merge_tests", False):
+        # Merge by parameter
+        return item.nodeid.rsplit("[", 1)[0]
+    else:
+        return item.nodeid
 
 
 class TestReport:
     """
     The final test report. Contains the human-readable document parsed from
     restructuredtext, suitable for display in any other format.
     """
@@ -164,33 +229,59 @@
         self._warnings: Dict[object, warnings.WarningMessage] = {}
 
         # Will be filled out at the end
         self.document = docutils.utils.new_document("<pending>")
 
     @property
     def any_failures(self) -> bool:
-        return any(m.failures for m in self.modules.values())
+        return any(m.any_failures for m in self.modules.values())
+
+    @property
+    def any_successes(self) -> bool:
+        return any(m.any_successes for m in self.modules.values())
 
     @property
     def failure_count(self) -> int:
-        return sum(len(m.failures) for m in self.modules.values())
+        return sum(m.failure_count for m in self.modules.values())
+
+    @property
+    def success_count(self) -> int:
+        return sum(m.success_count for m in self.modules.values())
+
+    @property
+    def failures(self) -> List[TestModule]:
+        return [m for m in self.modules.values() if m.any_failures]
+
+    @property
+    def successes(self) -> List[TestModule]:
+        return [m for m in self.modules.values() if m.any_successes]
 
     def add_item(
         self,
         item: "pytest.Function",
         pytest_report: Optional["pytest.TestReport"] = None,
     ) -> None:
-        if getattr(item.function, "merge_tests", False):
-            base_nodeid = item.nodeid.rsplit("[", 1)[0]
-        else:
-            base_nodeid = item.nodeid
-        module_failures = self.modules.setdefault(item.module, TestModule(item))
-        failure = module_failures.failures.setdefault(base_nodeid, TestFailure(item))
+        base_nodeid = get_base_nodeid(item)
+        module_items = self.modules.setdefault(item.module, TestModule(item))
+        outcome = module_items.tests.setdefault(base_nodeid, TestOutcome(item))
         if pytest_report is not None:
-            failure.add_report(pytest_report)
+            if pytest_report.failed:
+                outcome.add_failure(pytest_report)
+            elif pytest_report.skipped:
+                outcome.skipped = True
+
+    def remove_item(
+        self,
+        item: "pytest.Function",
+    ) -> None:
+        base_nodeid = get_base_nodeid(item)
+        try:
+            del self.modules[item.module].tests[base_nodeid]
+        except KeyError:
+            pass
 
     def add_warning(self, warning: warnings.WarningMessage) -> None:
         key = (str(warning.message), warning.category, warning.filename, warning.lineno)
         self._warnings.setdefault(key, warning)  # only keep the first
 
     @property
     def warnings(self) -> Iterable[warnings.WarningMessage]:
@@ -206,36 +297,49 @@
             is_full_version=is_full_version(),
             system_info=get_system_info(),
             inspector_version=VERSION,
         )
         self.document_source = src
         self.document = docutils.core.publish_doctree(src)
 
+        summary_template = JINJA_ENV.get_template("summary.rst")
+        src = summary_template.render(
+            report=self,
+            is_full_version=is_full_version(),
+            system_info=get_system_info(),
+            inspector_version=VERSION,
+        )
+        self.summary_source = src
+        self.summary = docutils.core.publish_doctree(src)
+
 
 class KevlarHooks:
     @pytest.hookspec()
     def pytest_kevlar_report(self, report: TestReport) -> None:
         pass
 
 
 class KevlarReporter:
     """Collect pytest output into a report object"""
 
-    def __init__(self) -> None:
+    def __init__(self, force_fail: bool = False) -> None:
         self.report = TestReport()
+        self.force_fail = force_fail
 
     @pytest.hookimpl(hookwrapper=True)
     def pytest_runtest_makereport(
         self, item: "pytest.Function", call: "pytest.CallInfo[None]"
     ) -> Generator[None, "pytest.TestReport", None]:
         outcome = yield
         pytest_report = outcome.get_result()
 
-        if not pytest_report.failed:
-            return
+        if pytest_report.passed:
+            # Where it will cause the least amount of trouble
+            if self.force_fail and pytest_report.when == "teardown":
+                pytest_report.outcome = "failed"
 
         self.report.add_item(item, pytest_report)
 
     def pytest_addhooks(self, pluginmanager: "pytest.PytestPluginManager") -> None:
         pluginmanager.add_hookspecs(KevlarHooks)
 
     def pytest_sessionfinish(self, session: "pytest.Session") -> None:
```

### Comparing `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/sysinfo.py` & `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/sysinfo.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/templates/report.rst` & `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/templates/report.rst`

 * *Files 12% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 is secure and capable of operating in hostile environments. Star Lab’s Kevlar
 System Inspector{{ lite }} is designed to help you identify many
 vulnerabilities often overlooked during the design of embedded systems, so you
 can protect your business and your customers. Below are the results of a
 comprehensive security test on your embedded operating environment.
 
 {% if not is_full_version %}
-The Lite version of Kevlar System Inspector does skip several tests, but you
-can request the full version of Kevlar System Inspector from Star Lab at no
+The Lite version of Kevlar System Inspector does not include several tests, but
+you can request the full version of Kevlar System Inspector from Star Lab at no
 cost when you `contact us`__. Kevlar System Inspector Lite is completely
 risk-free and there is no obligation to purchase anything after use. Star Lab
 wants every business to have access to the best possible security solutions,
 and our Kevlar System Inspector is just one of the ways we demonstrate our
 commitment to that belief.
 
 .. __: https://www.starlab.io/contact-us-kevlar-system-inspector-user
@@ -75,14 +75,18 @@
 {% include "warnings.rst" %}
 {% endif %}
 
 {% if report.any_failures %}
 {% include "failures.rst" %}
 {% endif %}
 
+{% if report.any_successes %}
+{% include "successes.rst" %}
+{% endif %}
+
 ==========
 Conclusion
 ==========
 
 Star Lab hopes the results from Kevlar System Inspector{{ lite }} will help you
 in identifying any vulnerabilities in your software and providing you with
 actionable recommendations to enhance your security. Cyber threats are
```

### Comparing `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/templates/starlab.css` & `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/templates/starlab.css`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/test_offline_integrity.py` & `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/test_offline_integrity.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """
 ---------------------
 Application Integrity
 ---------------------
 
-It is often a simple matter to alter files while the computer is turned off,
-allowing an attacker to alter data and executables without needing to bypass
-enforcement that happens while the system is live. It is critical to secure the
-system from offline tampering, or none of the data on the device can really be
-trusted. This is a prerequisite to secure boot.
+Attackers will often attempt to introduce malicious code on a system before the
+system runs. This approach means that the attacker does not have to contend
+with runtime protections. Application Integrity is a security layer for
+preventing this offline tampering.
 
 See :kevlar-code:`500`
 """
 
 from typing import Dict
 from dataclasses import dataclass
 import subprocess
@@ -63,15 +62,15 @@
             table = subprocess.run(
                 ["dmsetup", "table", name],
                 check=True,
                 text=True,
                 stdout=subprocess.PIPE,
             ).stdout
         except (OSError, subprocess.CalledProcessError):
-            pytest.fail(f"Cannot run dmsetup to inspect device {name}")
+            pytest.fail(f"Cannot run dmsetup to inspect device {name}.")
 
         _start, _end, kind, *fields = table.split()
         if kind in ("verity", "integrity"):
             has_integrity = True
         elif kind == "crypt":
             has_encryption = True
 
@@ -82,18 +81,19 @@
                 devices.append(field)
 
     return BlockDevInfo(has_encryption=has_encryption, has_integrity=has_integrity)
 
 
 def test_root_filesystem_has_integrity() -> None:
     """
-    The root filesystem should be protected at the block level from offline modification
-    ====================================================================================
+    The root filesystem should be protected at the block level from offline modification.
+    =====================================================================================
 
-    The root filesystem holds system binaries and configuration and should be
-    protected from offline modification. We recommend block-based schemes such
-    as dm-verity, because they are higher performance and present fewer
-    configuration challenges than file-based schemes.
+    The integrity of system binaries and configuration files in the root
+    filesystem should be evaluated using the stronger block-based scheme vs a
+    file-based scheme.
     """
 
     info = inspect_mountpoint("/")
-    assert info.has_integrity, "Root file system is unprotected."
+    assert (
+        info.has_integrity
+    ), "Root file system is unprotected from offline modification at the block level."
```

### Comparing `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/utils/__init__.py` & `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/utils/elf.py` & `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/utils/elf.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/utils/kconfig.py` & `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/utils/kconfig.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/utils/mount.py` & `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/utils/mount.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/utils/systemd.py` & `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/utils/systemd.py`

 * *Files identical despite different names*

### Comparing `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector/utils/workdir.py` & `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector/utils/workdir.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import Generator, List, ContextManager
 import warnings
 
 import pytest
 
 from . import PathLike
 from .mount import get_mountinfo, mount, umount, MNT_DETACH, MountEntry
+from .access import access
 
 
 @contextmanager
 def get_workdir(
     tmp_path_factory: "pytest.TempPathFactory",
 ) -> Generator[Path, None, None]:
     """Create a working directory:
@@ -58,17 +59,29 @@
 
     with workdir as dir_name:
         yield Path(dir_name)
 
 
 @contextmanager
 def mount_workdir() -> Generator[str, None, None]:
+    mounted = True
     try:
         tmpdir = tempfile.TemporaryDirectory()
-        mount("tmpfs", tmpdir.name, "tmpfs", 0, None)
+        try:
+            mount("tmpfs", tmpdir.name, "tmpfs", 0, None)
+        except OSError as e:
+            if access(tmpdir.name, os.W_OK):
+                # If we fail to mount but our tmpdir creation succeeded and we
+                # can write then continue. We might be under allowlisting
+                # so mount may not succeed.
+                mounted = False
+                pass
+            else:
+                # We will need to write to this temp dir so we should fail now
+                raise e
     except OSError:
         # Don't give them a clean bill of health: spit out a warning. Note that
         # even if we are run as a regular user or in a very locked down read-only
         # system, it would be still possible to enter into a user/mount namespace
         # to make a tmpfs. So we can still try harder if we need to.
         warnings.warn(
             textwrap.dedent(
@@ -79,8 +92,9 @@
         )
         pytest.skip("Could not set up workdir")
 
     with tmpdir:
         try:
             yield tmpdir.name
         finally:
-            umount(tmpdir.name, MNT_DETACH)
+            if mounted:
+                umount(tmpdir.name, MNT_DETACH)
```

### Comparing `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector.egg-info/PKG-INFO` & `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kevlar-system-inspector
-Version: 1.0.1
+Version: 1.1.0a1
 Summary: A security scanner for Linux systems
 Home-page: https://www.starlab.io/explore-kevlar-system-inspector
 Author: Star Lab
 Author-email: info@starlab.io
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -96,15 +96,15 @@
 copied this tarball to your device, you can simply extract and run:
 
 .. code-block:: console
 
    $ tar xf ./kevlar-system-inspector-standalone.tar.gz
    $ sudo ./kevlar-system-inspector-standalone/kevlar-system-inspector
 
-.. _standalone tarball: https://inspector.starlab.io/kevlar-system-inspector-standalone-v1.0.1.tar.gz
+.. _standalone tarball: https://inspector.starlab.io/kevlar-system-inspector-standalone-v1.1.01a.tar.gz
 
 
 Running as Root
 ===============
 
 Although running as root is not necessary, Kevlar System Inspector is designed
 to be run as root in a embedded test environment for two reasons:
```

### Comparing `kevlar-system-inspector-1.0.1/src/kevlar_system_inspector.egg-info/SOURCES.txt` & `kevlar-system-inspector-1.1.0a1/src/kevlar_system_inspector.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -10,31 +10,34 @@
 src/kevlar_system_inspector/console.py
 src/kevlar_system_inspector/decorators.py
 src/kevlar_system_inspector/output.py
 src/kevlar_system_inspector/report.py
 src/kevlar_system_inspector/sysinfo.py
 src/kevlar_system_inspector/test_allowlisting.py
 src/kevlar_system_inspector/test_kernel_config.py
-src/kevlar_system_inspector/test_kernel_modules.py
+src/kevlar_system_inspector/test_kernel_sandboxing.py
 src/kevlar_system_inspector/test_offline_integrity.py
-src/kevlar_system_inspector/test_secure_dns.py
+src/kevlar_system_inspector/test_secure_networking.py
 src/kevlar_system_inspector/test_systemd_syscall_filtering.py
 src/kevlar_system_inspector/version.py
 src/kevlar_system_inspector.egg-info/PKG-INFO
 src/kevlar_system_inspector.egg-info/SOURCES.txt
 src/kevlar_system_inspector.egg-info/dependency_links.txt
 src/kevlar_system_inspector.egg-info/requires.txt
 src/kevlar_system_inspector.egg-info/top_level.txt
 src/kevlar_system_inspector/resources/__init__.py
 src/kevlar_system_inspector/templates/__init__.py
 src/kevlar_system_inspector/templates/failures.rst
 src/kevlar_system_inspector/templates/html5-template.txt
 src/kevlar_system_inspector/templates/report.rst
 src/kevlar_system_inspector/templates/starlab.css
+src/kevlar_system_inspector/templates/successes.rst
+src/kevlar_system_inspector/templates/summary.rst
 src/kevlar_system_inspector/templates/warnings.rst
 src/kevlar_system_inspector/utils/__init__.py
+src/kevlar_system_inspector/utils/access.py
 src/kevlar_system_inspector/utils/elf.py
 src/kevlar_system_inspector/utils/kconfig.py
 src/kevlar_system_inspector/utils/modules.py
 src/kevlar_system_inspector/utils/mount.py
 src/kevlar_system_inspector/utils/systemd.py
 src/kevlar_system_inspector/utils/workdir.py
```

