# Comparing `tmp/YYYTools-0.1.6.tar.gz` & `tmp/YYYTools-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\YYYTools-0.1.6.tar", last modified: Wed Jul  5 20:01:08 2023, max compression
+gzip compressed data, was "YYYTools-0.1.7.tar", last modified: Tue Jul 11 08:34:01 2023, max compression
```

## Comparing `YYYTools-0.1.6.tar` & `YYYTools-0.1.7.tar`

### file list

```diff
@@ -1,71 +1,78 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 20:01:08.089201 YYYTools-0.1.6/
--rw-rw-rw-   0        0        0     1059 2021-12-18 16:09:22.000000 YYYTools-0.1.6/LICENSE
--rw-rw-rw-   0        0        0       41 2021-12-18 16:09:22.000000 YYYTools-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0      265 2023-07-05 20:01:08.089201 YYYTools-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0        8 2021-12-18 16:09:22.000000 YYYTools-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-05 20:01:07.995222 YYYTools-0.1.6/YTools/
--rw-rw-rw-   0        0        0       57 2021-12-18 16:09:23.000000 YYYTools-0.1.6/YTools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-05 20:01:07.998224 YYYTools-0.1.6/YTools/cg/
--rw-rw-rw-   0        0        0        0 2021-12-18 16:09:52.000000 YYYTools-0.1.6/YTools/cg/__init__.py
--rw-rw-rw-   0        0        0     5297 2021-12-18 16:09:52.000000 YYYTools-0.1.6/YTools/cg/glsl_use.py
-drwxrwxrwx   0        0        0        0 2023-07-05 20:01:08.002223 YYYTools-0.1.6/YTools/client/
--rw-rw-rw-   0        0        0        0 2021-12-18 16:09:46.000000 YYYTools-0.1.6/YTools/client/__init__.py
--rw-rw-rw-   0        0        0     3104 2021-12-18 16:09:46.000000 YYYTools-0.1.6/YTools/client/cui.py
-drwxrwxrwx   0        0        0        0 2023-07-05 20:01:08.006224 YYYTools-0.1.6/YTools/debug/
--rw-rw-rw-   0        0        0        0 2021-12-18 16:09:45.000000 YYYTools-0.1.6/YTools/debug/__init__.py
--rw-rw-rw-   0        0        0     6855 2021-12-18 16:09:45.000000 YYYTools-0.1.6/YTools/debug/debug_recursion.py
-drwxrwxrwx   0        0        0        0 2023-07-05 20:01:08.010225 YYYTools-0.1.6/YTools/deeplearning/
--rw-rw-rw-   0        0        0       41 2021-12-18 16:09:49.000000 YYYTools-0.1.6/YTools/deeplearning/__init__.py
--rw-rw-rw-   0        0        0     1655 2021-12-18 16:09:49.000000 YYYTools-0.1.6/YTools/deeplearning/composed_model.py
-drwxrwxrwx   0        0        0        0 2023-07-05 20:01:08.018226 YYYTools-0.1.6/YTools/experiment_helper/
--rw-rw-rw-   0        0        0      104 2021-12-18 16:09:24.000000 YYYTools-0.1.6/YTools/experiment_helper/__init__.py
--rw-rw-rw-   0        0        0     1822 2021-12-18 16:09:24.000000 YYYTools-0.1.6/YTools/experiment_helper/logger.py
--rw-rw-rw-   0        0        0      646 2021-12-18 16:09:24.000000 YYYTools-0.1.6/YTools/experiment_helper/random_seeder.py
--rw-rw-rw-   0        0        0      194 2021-12-18 16:09:24.000000 YYYTools-0.1.6/YTools/experiment_helper/watch_time.py
-drwxrwxrwx   0        0        0        0 2023-07-05 20:01:08.023228 YYYTools-0.1.6/YTools/network/
--rw-rw-rw-   0        0        0        0 2021-12-18 16:09:47.000000 YYYTools-0.1.6/YTools/network/__init__.py
--rw-rw-rw-   0        0        0     3379 2021-12-18 16:09:47.000000 YYYTools-0.1.6/YTools/network/communicate.py
--rw-rw-rw-   0        0        0     4059 2021-12-18 16:09:47.000000 YYYTools-0.1.6/YTools/network/protocol.py
-drwxrwxrwx   0        0        0        0 2023-07-05 20:01:08.030229 YYYTools-0.1.6/YTools/network/server/
--rw-rw-rw-   0        0        0        0 2021-12-18 16:09:48.000000 YYYTools-0.1.6/YTools/network/server/__init__.py
--rw-rw-rw-   0        0        0      445 2021-12-18 16:09:48.000000 YYYTools-0.1.6/YTools/network/server/client.py
--rw-rw-rw-   0        0        0      751 2023-07-05 19:59:18.000000 YYYTools-0.1.6/YTools/network/server/server.py
--rw-rw-rw-   0        0        0      816 2021-12-18 16:09:48.000000 YYYTools-0.1.6/YTools/network/server/urlconf.py
-drwxrwxrwx   0        0        0        0 2023-07-05 20:01:08.043233 YYYTools-0.1.6/YTools/system/
--rw-rw-rw-   0        0        0       77 2021-12-18 16:09:25.000000 YYYTools-0.1.6/YTools/system/__init__.py
--rw-rw-rw-   0        0        0     2355 2021-12-18 16:09:25.000000 YYYTools-0.1.6/YTools/system/cmd_control.py
-drwxrwxrwx   0        0        0        0 2023-07-05 20:01:08.047233 YYYTools-0.1.6/YTools/system/fakepath/
--rw-rw-rw-   0        0        0       51 2021-12-18 16:09:25.000000 YYYTools-0.1.6/YTools/system/fakepath/__init__.py
--rw-rw-rw-   0        0        0      631 2021-12-18 16:09:25.000000 YYYTools-0.1.6/YTools/system/fakepath/fakepath.py
--rw-rw-rw-   0        0        0      376 2021-12-18 16:09:25.000000 YYYTools-0.1.6/YTools/system/fileintercept.py
--rw-rw-rw-   0        0        0      447 2021-12-18 16:09:25.000000 YYYTools-0.1.6/YTools/system/filewrite.py
-drwxrwxrwx   0        0        0        0 2023-07-05 20:01:08.052193 YYYTools-0.1.6/YTools/system/locker/
--rw-rw-rw-   0        0        0       42 2021-12-18 16:09:44.000000 YYYTools-0.1.6/YTools/system/locker/__init__.py
--rw-rw-rw-   0        0        0     2150 2021-12-18 16:09:44.000000 YYYTools-0.1.6/YTools/system/locker/filelock.py
--rw-rw-rw-   0        0        0     3783 2021-12-18 16:09:44.000000 YYYTools-0.1.6/YTools/system/locker/lock.py
--rw-rw-rw-   0        0        0    10592 2021-12-18 16:09:25.000000 YYYTools-0.1.6/YTools/system/static_hash.py
-drwxrwxrwx   0        0        0        0 2023-07-05 20:01:08.076198 YYYTools-0.1.6/YTools/universe/
--rw-rw-rw-   0        0        0      188 2021-12-18 16:09:50.000000 YYYTools-0.1.6/YTools/universe/__init__.py
--rw-rw-rw-   0        0        0     2275 2022-03-16 19:19:59.000000 YYYTools-0.1.6/YTools/universe/beautiful_str.py
--rw-rw-rw-   0        0        0     1779 2021-12-18 16:09:49.000000 YYYTools-0.1.6/YTools/universe/exceptions.py
--rw-rw-rw-   0        0        0     2159 2021-12-18 16:09:50.000000 YYYTools-0.1.6/YTools/universe/extra_type.py
--rw-rw-rw-   0        0        0     1169 2021-12-18 16:09:49.000000 YYYTools-0.1.6/YTools/universe/filename.py
--rw-rw-rw-   0        0        0      186 2021-12-18 16:09:50.000000 YYYTools-0.1.6/YTools/universe/myrandom.py
--rw-rw-rw-   0        0        0      478 2021-12-18 16:09:49.000000 YYYTools-0.1.6/YTools/universe/onexit.py
--rw-rw-rw-   0        0        0      112 2021-12-18 16:09:50.000000 YYYTools-0.1.6/YTools/universe/pather.py
--rw-rw-rw-   0        0        0      480 2021-12-18 16:09:50.000000 YYYTools-0.1.6/YTools/universe/save_load.py
--rw-rw-rw-   0        0        0      509 2022-03-16 19:15:25.000000 YYYTools-0.1.6/YTools/universe/strlen.py
--rw-rw-rw-   0        0        0      431 2021-12-18 16:09:49.000000 YYYTools-0.1.6/YTools/universe/temp_cwd.py
--rw-rw-rw-   0        0        0     1884 2021-12-18 16:09:50.000000 YYYTools-0.1.6/YTools/universe/timer.py
-drwxrwxrwx   0        0        0        0 2023-07-05 20:01:08.084200 YYYTools-0.1.6/YYYTools.egg-info/
-drwxrwxrwx   0        0        0        0 2023-07-05 20:01:08.086201 YYYTools-0.1.6/YYYTools.egg-info/._DAV/
--rw-rw-rw-   0        0        0        0 2021-12-18 18:41:26.000000 YYYTools-0.1.6/YYYTools.egg-info/._DAV/.state_for_dir.dir
--rw-rw-rw-   0        0        0     1024 2021-12-18 18:41:26.000000 YYYTools-0.1.6/YYYTools.egg-info/._DAV/.state_for_dir.pag
--rw-rw-rw-   0        0        0      265 2023-07-05 20:01:07.000000 YYYTools-0.1.6/YYYTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1549 2023-07-05 20:01:07.000000 YYYTools-0.1.6/YYYTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 20:01:07.000000 YYYTools-0.1.6/YYYTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-07-05 20:01:07.000000 YYYTools-0.1.6/YYYTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-05 20:01:07.000000 YYYTools-0.1.6/YYYTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        5 2022-11-13 21:08:17.000000 YYYTools-0.1.6/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-05 20:01:08.090201 YYYTools-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      776 2023-07-05 19:59:30.000000 YYYTools-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 08:34:01.849804 YYYTools-0.1.7/
+-rw-rw-rw-   0        0        0     1059 2021-12-18 16:09:22.000000 YYYTools-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0       41 2021-12-18 16:09:22.000000 YYYTools-0.1.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      265 2023-07-11 08:34:01.849804 YYYTools-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0        8 2021-12-18 16:09:22.000000 YYYTools-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 08:34:01.769792 YYYTools-0.1.7/YTools/
+-rw-rw-rw-   0        0        0      249 2023-07-11 08:33:57.000000 YYYTools-0.1.7/YTools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 08:34:01.772792 YYYTools-0.1.7/YTools/application/
+-rw-rw-rw-   0        0        0       28 2023-07-11 08:33:56.000000 YYYTools-0.1.7/YTools/application/__init__.py
+-rw-rw-rw-   0        0        0     4735 2023-07-11 08:29:10.000000 YYYTools-0.1.7/YTools/application/chord_analyze.py
+drwxrwxrwx   0        0        0        0 2023-07-11 08:34:01.774793 YYYTools-0.1.7/YTools/cg/
+-rw-rw-rw-   0        0        0       23 2023-07-11 08:29:28.000000 YYYTools-0.1.7/YTools/cg/__init__.py
+-rw-rw-rw-   0        0        0     5297 2021-12-18 16:09:52.000000 YYYTools-0.1.7/YTools/cg/glsl_use.py
+drwxrwxrwx   0        0        0        0 2023-07-11 08:34:01.777796 YYYTools-0.1.7/YTools/client/
+-rw-rw-rw-   0        0        0       18 2023-07-11 08:29:33.000000 YYYTools-0.1.7/YTools/client/__init__.py
+-rw-rw-rw-   0        0        0     3104 2021-12-18 16:09:46.000000 YYYTools-0.1.7/YTools/client/cui.py
+drwxrwxrwx   0        0        0        0 2023-07-11 08:34:01.781799 YYYTools-0.1.7/YTools/debug/
+-rw-rw-rw-   0        0        0       30 2023-07-11 08:29:39.000000 YYYTools-0.1.7/YTools/debug/__init__.py
+-rw-rw-rw-   0        0        0     6855 2021-12-18 16:09:45.000000 YYYTools-0.1.7/YTools/debug/debug_recursion.py
+drwxrwxrwx   0        0        0        0 2023-07-11 08:34:01.783798 YYYTools-0.1.7/YTools/deeplearning/
+-rw-rw-rw-   0        0        0       41 2021-12-18 16:09:49.000000 YYYTools-0.1.7/YTools/deeplearning/__init__.py
+-rw-rw-rw-   0        0        0     1655 2021-12-18 16:09:49.000000 YYYTools-0.1.7/YTools/deeplearning/composed_model.py
+drwxrwxrwx   0        0        0        0 2023-07-11 08:34:01.789792 YYYTools-0.1.7/YTools/experiment_helper/
+-rw-rw-rw-   0        0        0      104 2021-12-18 16:09:24.000000 YYYTools-0.1.7/YTools/experiment_helper/__init__.py
+-rw-rw-rw-   0        0        0     1822 2021-12-18 16:09:24.000000 YYYTools-0.1.7/YTools/experiment_helper/logger.py
+-rw-rw-rw-   0        0        0      646 2021-12-18 16:09:24.000000 YYYTools-0.1.7/YTools/experiment_helper/random_seeder.py
+-rw-rw-rw-   0        0        0      194 2021-12-18 16:09:24.000000 YYYTools-0.1.7/YTools/experiment_helper/watch_time.py
+drwxrwxrwx   0        0        0        0 2023-07-11 08:34:01.793795 YYYTools-0.1.7/YTools/magic/
+-rw-rw-rw-   0        0        0       51 2023-07-11 08:30:17.000000 YYYTools-0.1.7/YTools/magic/__init__.py
+-rw-rw-rw-   0        0        0     2468 2023-07-06 04:59:41.000000 YYYTools-0.1.7/YTools/magic/awss3.py
+-rw-rw-rw-   0        0        0      710 2023-07-06 04:57:10.000000 YYYTools-0.1.7/YTools/magic/egorov_awss3.py
+drwxrwxrwx   0        0        0        0 2023-07-11 08:34:01.797793 YYYTools-0.1.7/YTools/network/
+-rw-rw-rw-   0        0        0       76 2023-07-11 08:30:33.000000 YYYTools-0.1.7/YTools/network/__init__.py
+-rw-rw-rw-   0        0        0     3379 2021-12-18 16:09:47.000000 YYYTools-0.1.7/YTools/network/communicate.py
+-rw-rw-rw-   0        0        0     4059 2021-12-18 16:09:47.000000 YYYTools-0.1.7/YTools/network/protocol.py
+drwxrwxrwx   0        0        0        0 2023-07-11 08:34:01.803792 YYYTools-0.1.7/YTools/network/server/
+-rw-rw-rw-   0        0        0       46 2023-07-11 08:31:16.000000 YYYTools-0.1.7/YTools/network/server/__init__.py
+-rw-rw-rw-   0        0        0      445 2021-12-18 16:09:48.000000 YYYTools-0.1.7/YTools/network/server/client.py
+-rw-rw-rw-   0        0        0      751 2023-07-05 19:59:18.000000 YYYTools-0.1.7/YTools/network/server/server.py
+-rw-rw-rw-   0        0        0      816 2021-12-18 16:09:48.000000 YYYTools-0.1.7/YTools/network/server/urlconf.py
+drwxrwxrwx   0        0        0        0 2023-07-11 08:34:01.811795 YYYTools-0.1.7/YTools/system/
+-rw-rw-rw-   0        0        0      165 2023-07-11 08:31:45.000000 YYYTools-0.1.7/YTools/system/__init__.py
+-rw-rw-rw-   0        0        0     2355 2021-12-18 16:09:25.000000 YYYTools-0.1.7/YTools/system/cmd_control.py
+drwxrwxrwx   0        0        0        0 2023-07-11 08:34:01.814796 YYYTools-0.1.7/YTools/system/fakepath/
+-rw-rw-rw-   0        0        0       51 2021-12-18 16:09:25.000000 YYYTools-0.1.7/YTools/system/fakepath/__init__.py
+-rw-rw-rw-   0        0        0      631 2021-12-18 16:09:25.000000 YYYTools-0.1.7/YTools/system/fakepath/fakepath.py
+-rw-rw-rw-   0        0        0      376 2021-12-18 16:09:25.000000 YYYTools-0.1.7/YTools/system/fileintercept.py
+-rw-rw-rw-   0        0        0      447 2021-12-18 16:09:25.000000 YYYTools-0.1.7/YTools/system/filewrite.py
+drwxrwxrwx   0        0        0        0 2023-07-11 08:34:01.818797 YYYTools-0.1.7/YTools/system/locker/
+-rw-rw-rw-   0        0        0       42 2021-12-18 16:09:44.000000 YYYTools-0.1.7/YTools/system/locker/__init__.py
+-rw-rw-rw-   0        0        0     2150 2021-12-18 16:09:44.000000 YYYTools-0.1.7/YTools/system/locker/filelock.py
+-rw-rw-rw-   0        0        0     3783 2021-12-18 16:09:44.000000 YYYTools-0.1.7/YTools/system/locker/lock.py
+-rw-rw-rw-   0        0        0    10592 2021-12-18 16:09:25.000000 YYYTools-0.1.7/YTools/system/static_hash.py
+drwxrwxrwx   0        0        0        0 2023-07-11 08:34:01.835797 YYYTools-0.1.7/YTools/universe/
+-rw-rw-rw-   0        0        0      366 2023-07-11 08:32:40.000000 YYYTools-0.1.7/YTools/universe/__init__.py
+-rw-rw-rw-   0        0        0     2275 2022-03-16 19:19:59.000000 YYYTools-0.1.7/YTools/universe/beautiful_str.py
+-rw-rw-rw-   0        0        0     1779 2021-12-18 16:09:49.000000 YYYTools-0.1.7/YTools/universe/exceptions.py
+-rw-rw-rw-   0        0        0     2159 2021-12-18 16:09:50.000000 YYYTools-0.1.7/YTools/universe/extra_type.py
+-rw-rw-rw-   0        0        0     1169 2021-12-18 16:09:49.000000 YYYTools-0.1.7/YTools/universe/filename.py
+-rw-rw-rw-   0        0        0      186 2021-12-18 16:09:50.000000 YYYTools-0.1.7/YTools/universe/myrandom.py
+-rw-rw-rw-   0        0        0      478 2021-12-18 16:09:49.000000 YYYTools-0.1.7/YTools/universe/onexit.py
+-rw-rw-rw-   0        0        0      112 2021-12-18 16:09:50.000000 YYYTools-0.1.7/YTools/universe/pather.py
+-rw-rw-rw-   0        0        0      480 2021-12-18 16:09:50.000000 YYYTools-0.1.7/YTools/universe/save_load.py
+-rw-rw-rw-   0        0        0      509 2022-03-16 19:15:25.000000 YYYTools-0.1.7/YTools/universe/strlen.py
+-rw-rw-rw-   0        0        0      431 2021-12-18 16:09:49.000000 YYYTools-0.1.7/YTools/universe/temp_cwd.py
+-rw-rw-rw-   0        0        0     1884 2021-12-18 16:09:50.000000 YYYTools-0.1.7/YTools/universe/timer.py
+drwxrwxrwx   0        0        0        0 2023-07-11 08:34:01.845795 YYYTools-0.1.7/YYYTools.egg-info/
+drwxrwxrwx   0        0        0        0 2023-07-11 08:34:01.847793 YYYTools-0.1.7/YYYTools.egg-info/._DAV/
+-rw-rw-rw-   0        0        0        0 2021-12-18 18:41:26.000000 YYYTools-0.1.7/YYYTools.egg-info/._DAV/.state_for_dir.dir
+-rw-rw-rw-   0        0        0     1024 2021-12-18 18:41:26.000000 YYYTools-0.1.7/YYYTools.egg-info/._DAV/.state_for_dir.pag
+-rw-rw-rw-   0        0        0      265 2023-07-11 08:34:01.000000 YYYTools-0.1.7/YYYTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1692 2023-07-11 08:34:01.000000 YYYTools-0.1.7/YYYTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 08:34:01.000000 YYYTools-0.1.7/YYYTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-07-11 08:34:01.000000 YYYTools-0.1.7/YYYTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-11 08:34:01.000000 YYYTools-0.1.7/YYYTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       21 2023-07-06 04:27:09.000000 YYYTools-0.1.7/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 08:34:01.850806 YYYTools-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      776 2023-07-11 08:33:03.000000 YYYTools-0.1.7/setup.py
```

### Comparing `YYYTools-0.1.6/LICENSE` & `YYYTools-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.6/YTools/cg/glsl_use.py` & `YYYTools-0.1.7/YTools/cg/glsl_use.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.6/YTools/client/cui.py` & `YYYTools-0.1.7/YTools/client/cui.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.6/YTools/debug/debug_recursion.py` & `YYYTools-0.1.7/YTools/debug/debug_recursion.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.6/YTools/deeplearning/composed_model.py` & `YYYTools-0.1.7/YTools/deeplearning/composed_model.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.6/YTools/experiment_helper/logger.py` & `YYYTools-0.1.7/YTools/experiment_helper/logger.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.6/YTools/experiment_helper/random_seeder.py` & `YYYTools-0.1.7/YTools/experiment_helper/random_seeder.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.6/YTools/network/communicate.py` & `YYYTools-0.1.7/YTools/network/communicate.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.6/YTools/network/protocol.py` & `YYYTools-0.1.7/YTools/network/protocol.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.6/YTools/network/server/server.py` & `YYYTools-0.1.7/YTools/network/server/server.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.6/YTools/network/server/urlconf.py` & `YYYTools-0.1.7/YTools/network/server/urlconf.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.6/YTools/system/cmd_control.py` & `YYYTools-0.1.7/YTools/system/cmd_control.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.6/YTools/system/fakepath/fakepath.py` & `YYYTools-0.1.7/YTools/system/fakepath/fakepath.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.6/YTools/system/locker/filelock.py` & `YYYTools-0.1.7/YTools/system/locker/filelock.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.6/YTools/system/locker/lock.py` & `YYYTools-0.1.7/YTools/system/locker/lock.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.6/YTools/system/static_hash.py` & `YYYTools-0.1.7/YTools/system/static_hash.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.6/YTools/universe/beautiful_str.py` & `YYYTools-0.1.7/YTools/universe/beautiful_str.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.6/YTools/universe/exceptions.py` & `YYYTools-0.1.7/YTools/universe/exceptions.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.6/YTools/universe/extra_type.py` & `YYYTools-0.1.7/YTools/universe/extra_type.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.6/YTools/universe/filename.py` & `YYYTools-0.1.7/YTools/universe/filename.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.6/YTools/universe/timer.py` & `YYYTools-0.1.7/YTools/universe/timer.py`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.6/YYYTools.egg-info/._DAV/.state_for_dir.pag` & `YYYTools-0.1.7/YYYTools.egg-info/._DAV/.state_for_dir.pag`

 * *Files identical despite different names*

### Comparing `YYYTools-0.1.6/setup.py` & `YYYTools-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     reqs = f.read()
 
 pkgs = [p for p in find_packages() if p.startswith('YTools')]
 print(pkgs)
 
 setup(
     name='YYYTools',
-    version='0.1.6',
+    version='0.1.7',
     url='http://github.com/FFTYYY/YTools',
     description='',
     long_description=readme,
     long_description_content_type='text/markdown',
     license='MIT',
     author = 'Yongyi Yang',
 	author_email = 'yongyi@umich.edu',
```

