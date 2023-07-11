# Comparing `tmp/geventmp-0.0.8.dev20230711180100.tar.gz` & `tmp/geventmp-0.0.8.dev20230711180108.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geventmp-0.0.8.dev20230711180100.tar", last modified: Tue Jul 11 18:02:38 2023, max compression
+gzip compressed data, was "geventmp-0.0.8.dev20230711180108.tar", last modified: Tue Jul 11 18:02:47 2023, max compression
```

## Comparing `geventmp-0.0.8.dev20230711180100.tar` & `geventmp-0.0.8.dev20230711180108.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:02:38.212385 geventmp-0.0.8.dev20230711180100/
--rw-rw-r--   0 runner    (1001) docker     (123)       25 2023-07-11 18:01:11.000000 geventmp-0.0.8.dev20230711180100/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-07-11 18:02:38.212385 geventmp-0.0.8.dev20230711180100/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:02:38.212385 geventmp-0.0.8.dev20230711180100/geventmp/
--rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-07-11 18:01:11.000000 geventmp-0.0.8.dev20230711180100/geventmp/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-11 18:00:55.000000 geventmp-0.0.8.dev20230711180100/geventmp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:02:38.212385 geventmp-0.0.8.dev20230711180100/geventmp/_mp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:02:38.212385 geventmp-0.0.8.dev20230711180100/geventmp/_mp/3/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-11 18:00:55.000000 geventmp-0.0.8.dev20230711180100/geventmp/_mp/3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-11 18:00:55.000000 geventmp-0.0.8.dev20230711180100/geventmp/_mp/3/_mp_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-07-11 18:00:55.000000 geventmp-0.0.8.dev20230711180100/geventmp/_mp/3/_mp_forkserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-11 18:00:55.000000 geventmp-0.0.8.dev20230711180100/geventmp/_mp/3/_mp_popen_fork.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-11 18:00:55.000000 geventmp-0.0.8.dev20230711180100/geventmp/_mp/3/_mp_popen_spawn_posix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-11 18:00:55.000000 geventmp-0.0.8.dev20230711180100/geventmp/_mp/3/_mp_resource_tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-11 18:00:55.000000 geventmp-0.0.8.dev20230711180100/geventmp/_mp/3/_mp_sem_tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-11 18:00:55.000000 geventmp-0.0.8.dev20230711180100/geventmp/_mp/3/_mp_spawn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-07-11 18:00:55.000000 geventmp-0.0.8.dev20230711180100/geventmp/_mp/3/_mp_synchronize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-11 18:00:55.000000 geventmp-0.0.8.dev20230711180100/geventmp/_mp/3/_mp_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-11 18:00:55.000000 geventmp-0.0.8.dev20230711180100/geventmp/_mp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-07-11 18:00:55.000000 geventmp-0.0.8.dev20230711180100/geventmp/monkey.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:02:38.212385 geventmp-0.0.8.dev20230711180100/geventmp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-07-11 18:02:38.000000 geventmp-0.0.8.dev20230711180100/geventmp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-11 18:02:38.000000 geventmp-0.0.8.dev20230711180100/geventmp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 18:02:38.000000 geventmp-0.0.8.dev20230711180100/geventmp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-11 18:02:38.000000 geventmp-0.0.8.dev20230711180100/geventmp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 18:02:38.000000 geventmp-0.0.8.dev20230711180100/geventmp.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-11 18:02:38.000000 geventmp-0.0.8.dev20230711180100/geventmp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 18:02:38.000000 geventmp-0.0.8.dev20230711180100/geventmp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 18:01:15.000000 geventmp-0.0.8.dev20230711180100/geventmp.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 18:02:38.212385 geventmp-0.0.8.dev20230711180100/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     8159 2023-07-11 18:01:11.000000 geventmp-0.0.8.dev20230711180100/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:02:47.778115 geventmp-0.0.8.dev20230711180108/
+-rw-rw-r--   0 runner    (1001) docker     (123)       25 2023-07-11 18:01:26.000000 geventmp-0.0.8.dev20230711180108/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-07-11 18:02:47.778115 geventmp-0.0.8.dev20230711180108/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:02:47.778115 geventmp-0.0.8.dev20230711180108/geventmp/
+-rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-07-11 18:01:26.000000 geventmp-0.0.8.dev20230711180108/geventmp/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-11 18:00:58.000000 geventmp-0.0.8.dev20230711180108/geventmp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:02:47.778115 geventmp-0.0.8.dev20230711180108/geventmp/_mp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:02:47.778115 geventmp-0.0.8.dev20230711180108/geventmp/_mp/3/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-11 18:00:58.000000 geventmp-0.0.8.dev20230711180108/geventmp/_mp/3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-11 18:00:58.000000 geventmp-0.0.8.dev20230711180108/geventmp/_mp/3/_mp_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-07-11 18:00:58.000000 geventmp-0.0.8.dev20230711180108/geventmp/_mp/3/_mp_forkserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-11 18:00:58.000000 geventmp-0.0.8.dev20230711180108/geventmp/_mp/3/_mp_popen_fork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-11 18:00:58.000000 geventmp-0.0.8.dev20230711180108/geventmp/_mp/3/_mp_popen_spawn_posix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-11 18:00:58.000000 geventmp-0.0.8.dev20230711180108/geventmp/_mp/3/_mp_resource_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-11 18:00:58.000000 geventmp-0.0.8.dev20230711180108/geventmp/_mp/3/_mp_sem_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-11 18:00:58.000000 geventmp-0.0.8.dev20230711180108/geventmp/_mp/3/_mp_spawn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-07-11 18:00:58.000000 geventmp-0.0.8.dev20230711180108/geventmp/_mp/3/_mp_synchronize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-11 18:00:58.000000 geventmp-0.0.8.dev20230711180108/geventmp/_mp/3/_mp_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-07-11 18:00:58.000000 geventmp-0.0.8.dev20230711180108/geventmp/_mp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-07-11 18:00:58.000000 geventmp-0.0.8.dev20230711180108/geventmp/monkey.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 18:02:47.778115 geventmp-0.0.8.dev20230711180108/geventmp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-07-11 18:02:47.000000 geventmp-0.0.8.dev20230711180108/geventmp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-11 18:02:47.000000 geventmp-0.0.8.dev20230711180108/geventmp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 18:02:47.000000 geventmp-0.0.8.dev20230711180108/geventmp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-11 18:02:47.000000 geventmp-0.0.8.dev20230711180108/geventmp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 18:02:47.000000 geventmp-0.0.8.dev20230711180108/geventmp.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-11 18:02:47.000000 geventmp-0.0.8.dev20230711180108/geventmp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 18:02:47.000000 geventmp-0.0.8.dev20230711180108/geventmp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 18:01:27.000000 geventmp-0.0.8.dev20230711180108/geventmp.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 18:02:47.778115 geventmp-0.0.8.dev20230711180108/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8159 2023-07-11 18:01:26.000000 geventmp-0.0.8.dev20230711180108/setup.py
```

### Comparing `geventmp-0.0.8.dev20230711180100/PKG-INFO` & `geventmp-0.0.8.dev20230711180108/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geventmp
-Version: 0.0.8.dev20230711180100
+Version: 0.0.8.dev20230711180108
 Summary: Multiprocessing Gevent Extension
 Home-page: https://github.com/karellen/geventmp
 Author: Karellen, Inc.
 Author-email: supervisor@karellen.co
 Maintainer: Arcadiy Ivanov
 Maintainer-email: arcadiy@ivanov.biz
 License: Apache License, Version 2.0
```

### Comparing `geventmp-0.0.8.dev20230711180100/geventmp/LICENSE` & `geventmp-0.0.8.dev20230711180108/geventmp/LICENSE`

 * *Files identical despite different names*

### Comparing `geventmp-0.0.8.dev20230711180100/geventmp/__init__.py` & `geventmp-0.0.8.dev20230711180108/geventmp/__init__.py`

 * *Files identical despite different names*

### Comparing `geventmp-0.0.8.dev20230711180100/geventmp/_mp/3/__init__.py` & `geventmp-0.0.8.dev20230711180108/geventmp/_mp/3/__init__.py`

 * *Files identical despite different names*

### Comparing `geventmp-0.0.8.dev20230711180100/geventmp/_mp/3/_mp_connection.py` & `geventmp-0.0.8.dev20230711180108/geventmp/_mp/3/_mp_connection.py`

 * *Files identical despite different names*

### Comparing `geventmp-0.0.8.dev20230711180100/geventmp/_mp/3/_mp_forkserver.py` & `geventmp-0.0.8.dev20230711180108/geventmp/_mp/3/_mp_forkserver.py`

 * *Files identical despite different names*

### Comparing `geventmp-0.0.8.dev20230711180100/geventmp/_mp/3/_mp_popen_fork.py` & `geventmp-0.0.8.dev20230711180108/geventmp/_mp/3/_mp_popen_fork.py`

 * *Files identical despite different names*

### Comparing `geventmp-0.0.8.dev20230711180100/geventmp/_mp/3/_mp_popen_spawn_posix.py` & `geventmp-0.0.8.dev20230711180108/geventmp/_mp/3/_mp_popen_spawn_posix.py`

 * *Files identical despite different names*

### Comparing `geventmp-0.0.8.dev20230711180100/geventmp/_mp/3/_mp_resource_tracker.py` & `geventmp-0.0.8.dev20230711180108/geventmp/_mp/3/_mp_resource_tracker.py`

 * *Files identical despite different names*

### Comparing `geventmp-0.0.8.dev20230711180100/geventmp/_mp/3/_mp_sem_tracker.py` & `geventmp-0.0.8.dev20230711180108/geventmp/_mp/3/_mp_sem_tracker.py`

 * *Files identical despite different names*

### Comparing `geventmp-0.0.8.dev20230711180100/geventmp/_mp/3/_mp_spawn.py` & `geventmp-0.0.8.dev20230711180108/geventmp/_mp/3/_mp_spawn.py`

 * *Files identical despite different names*

### Comparing `geventmp-0.0.8.dev20230711180100/geventmp/_mp/3/_mp_synchronize.py` & `geventmp-0.0.8.dev20230711180108/geventmp/_mp/3/_mp_synchronize.py`

 * *Files identical despite different names*

### Comparing `geventmp-0.0.8.dev20230711180100/geventmp/_mp/3/_mp_util.py` & `geventmp-0.0.8.dev20230711180108/geventmp/_mp/3/_mp_util.py`

 * *Files identical despite different names*

### Comparing `geventmp-0.0.8.dev20230711180100/geventmp/_mp/__init__.py` & `geventmp-0.0.8.dev20230711180108/geventmp/_mp/__init__.py`

 * *Files identical despite different names*

### Comparing `geventmp-0.0.8.dev20230711180100/geventmp/monkey.py` & `geventmp-0.0.8.dev20230711180108/geventmp/monkey.py`

 * *Files identical despite different names*

### Comparing `geventmp-0.0.8.dev20230711180100/geventmp.egg-info/PKG-INFO` & `geventmp-0.0.8.dev20230711180108/geventmp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geventmp
-Version: 0.0.8.dev20230711180100
+Version: 0.0.8.dev20230711180108
 Summary: Multiprocessing Gevent Extension
 Home-page: https://github.com/karellen/geventmp
 Author: Karellen, Inc.
 Author-email: supervisor@karellen.co
 Maintainer: Arcadiy Ivanov
 Maintainer-email: arcadiy@ivanov.biz
 License: Apache License, Version 2.0
```

### Comparing `geventmp-0.0.8.dev20230711180100/geventmp.egg-info/SOURCES.txt` & `geventmp-0.0.8.dev20230711180108/geventmp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geventmp-0.0.8.dev20230711180100/setup.py` & `geventmp-0.0.8.dev20230711180108/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         _install.run(self)
 
         self.post_install_script()
 
 if __name__ == '__main__':
     setup(
         name = 'geventmp',
-        version = '0.0.8.dev20230711180100',
+        version = '0.0.8.dev20230711180108',
         description = 'Multiprocessing Gevent Extension',
         long_description = "===============================================\n GeventMP_ - Gevent_ Multiprocessing Extension\n===============================================\n\n.. image:: https://img.shields.io/gitter/room/karellen/Lobby?logo=gitter\n   :target: https://app.gitter.im/#/room/#karellen_Lobby:gitter.im\n   :alt: Gitter\n.. image:: https://img.shields.io/github/actions/workflow/status/karellen/geventmp/build.yml?branch=master\n   :target: https://github.com/karellen/geventmp/actions/workflows/build.yml\n   :alt: Build Status\n.. image:: https://img.shields.io/coveralls/github/karellen/geventmp/master?logo=coveralls\n   :target: https://coveralls.io/r/karellen/geventmp?branch=master\n   :alt: Coverage Status\n\n|\n\n.. image:: https://img.shields.io/pypi/v/geventmp?logo=pypi\n   :target: https://pypi.org/project/geventmp/\n   :alt: GeventMP Version\n.. image:: https://img.shields.io/pypi/pyversions/geventmp?logo=pypi\n   :target: https://pypi.org/project/geventmp/\n   :alt: GeventMP Python Versions\n.. image:: https://img.shields.io/pypi/dd/geventmp?logo=pypi\n   :target: https://pypi.org/project/geventmp/\n   :alt: GeventMP Downloads Per Day\n.. image:: https://img.shields.io/pypi/dw/geventmp?logo=pypi\n   :target: https://pypi.org/project/geventmp/\n   :alt: GeventMP Downloads Per Week\n.. image:: https://img.shields.io/pypi/dm/geventmp?logo=pypi\n   :target: https://pypi.org/project/geventmp/\n   :alt: GeventMP Downloads Per Month\n\n|\n\n.. warning::\n    HIC SUNT DRACONES!!!\n\n    This code is experimental (beta). There is some testing, but a lots of things are in flux, and\n    some platforms don't work at all.\n\n    You MAY try to use this in production with the understanding that this is a beta-quality software.\n\n    That said, this code may crash your server, bankrupt your company, burn your house down and be mean\n    to your puppy.\n\n    You've been warned.\n\nProblem\n=======\n\nDue to internal implementation, `multiprocessing` (`MP`) is unsafe to use with Gevent_ even when `monkey-patched`__.\nNamely, the use of OS semaphore primitives and inter-process IO in `MP` will cause the main\nloop to stall/deadlock/block (specific issue depends on the version of CPython).\n\n__ monkey_\n\nSolution\n========\nGeventMP_ (`Gee-vent Em-Pee`) is a gevent_ multiprocessing extension plugin for the `monkey-patching`__ subsystem.\nAs with the rest of the monkey patch subsystem the process is fairly clear:\n\n__ monkey_\n\n1. Identify all places where blocking occurs and where it may stall the loop.\n2. If blocking occurs on a file descriptor (`FD`), try to convert the file descriptor from blocking to non-blocking\n   (sockets/pipes/fifos, sometimes even files where, rarely, appropriate) and replace blocking IO functions with their\n   gevent_ non-blocking equivalents.\n3. If blocking occurs in a Python/OS primitive that does not support non-blocking access and thus cannot be geventized,\n   wrap all blocking access to that primitive with native thread-pool-based wrappers and call it a day (while fully\n   understanding that primitive access latency will increase and raw performance may suffer as a result).\n4. If you are really brave and have lots of free time on your hands, completely replace a standard blocking Python\n   non-`FD`-based primitive with implementation based on an `FD`-based OS primitive (e.g. POSIX semaphore =>\n   Linux `eventfd-based semaphore for kernels > 2.6.30`__).\n5. Due to launching of separate processes in `MP`, figure out how, when, and whether to `monkey-patch`__ spawned/forked\n   children and grandchildren.\n\n__ eventfd_\n\n__ monkey_\n\nInstallation\n============\nThe package is hosted on PyPi_.\n\nFor stable version:\n\n.. code-block:: bash\n\n  pip install geventmp\n\nFor unstable version:\n\n.. code-block:: bash\n\n  pip install --pre geventmp\n\n\nOnce installed, `GeventMP`_ will activate by default in the below stanza.\n\n.. code-block:: python\n\n   from gevent.monkey import patch_all\n   patch_all()\n\nIf you would like `GeventMP`_ to not activate by default, either do not install it or explicitly disable it:\n\n.. code-block:: python\n\n   from gevent.monkey import patch_all\n   patch_all(geventmp=False)\n\nThat's it - there are no other flags, settings, properties or config values so far.\n\nSupported Platforms\n===================\n\n.. note::\n    All claims of support may not be real at all. You're welcome to experiment. See warnings on top.\n\n* Linux and Darwin.\n* CPython 3.7, 3.8, 3.9, 3.10, 3.11, 3.12\n* PyPy 3.8, 3.9\n\nKnown Issues\n============\n\n* Multiprocessing `forkserver` works in GeventMP_, but the spawned child isn't green.\n\nTODO\n====\n1. Monkey patch Windows to the extent possible.\n2. Lots of applications use `Billiard <https://github.com/celery/billiard>`_ for multiprocessing instead of stock Python\n   package. Consider monkey patching Billiard if detected.\n\nContact Us\n==========\n\nPost feedback and issues on the `Bug Tracker`_, `Gitter`_,\nand `Twitter (@karelleninc)`_.\n\n.. _Gevent: https://github.com/gevent/gevent/\n.. _geventmp: https://github.com/karellen/geventmp\n.. _bug tracker: https://github.com/karellen/geventmp/issues\n.. _gitter: https://gitter.im/karellen/Lobby\n.. _twitter (@karelleninc): https://twitter.com/karelleninc\n.. _monkey: https://en.wikipedia.org/wiki/Monkey_patch\n.. _eventfd: https://linux.die.net/man/2/eventfd\n.. _pypi: https://pypi.org/project/geventmp/\n",
         long_description_content_type = 'text/x-rst; charset=UTF-8',
         classifiers = [
             'License :: OSI Approved :: Apache Software License',
             'Programming Language :: Python :: 3.7',
             'Programming Language :: Python :: 3.8',
```

