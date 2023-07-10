# Comparing `tmp/f5project-0.0.1.tar.gz` & `tmp/f5project-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f5project-0.0.1.tar", last modified: Wed Jun 28 09:20:34 2023, max compression
+gzip compressed data, was "f5project-0.0.3.tar", last modified: Mon Jul 10 23:54:07 2023, max compression
```

## Comparing `f5project-0.0.1.tar` & `f5project-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-06-28 09:20:34.272441 f5project-0.0.1/
--rw-r--r--   0 j3ymac     (501) staff       (20)     1066 2023-06-28 09:15:27.000000 f5project-0.0.1/LICENSE
--rw-r--r--   0 j3ymac     (501) staff       (20)      512 2023-06-28 09:20:34.272268 f5project-0.0.1/PKG-INFO
--rw-r--r--   0 j3ymac     (501) staff       (20)     1060 2023-06-28 09:17:04.000000 f5project-0.0.1/README.md
-drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-06-28 09:20:34.270943 f5project-0.0.1/f5project/
--rw-r--r--   0 j3ymac     (501) staff       (20)       72 2023-06-28 09:17:52.000000 f5project-0.0.1/f5project/__init__.py
-drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-06-28 09:20:34.271964 f5project-0.0.1/f5project.egg-info/
--rw-r--r--   0 j3ymac     (501) staff       (20)      512 2023-06-28 09:20:34.000000 f5project-0.0.1/f5project.egg-info/PKG-INFO
--rw-r--r--   0 j3ymac     (501) staff       (20)      180 2023-06-28 09:20:34.000000 f5project-0.0.1/f5project.egg-info/SOURCES.txt
--rw-r--r--   0 j3ymac     (501) staff       (20)        1 2023-06-28 09:20:34.000000 f5project-0.0.1/f5project.egg-info/dependency_links.txt
--rw-r--r--   0 j3ymac     (501) staff       (20)       10 2023-06-28 09:20:34.000000 f5project-0.0.1/f5project.egg-info/top_level.txt
--rw-r--r--   0 j3ymac     (501) staff       (20)       38 2023-06-28 09:20:34.272486 f5project-0.0.1/setup.cfg
--rw-r--r--   0 j3ymac     (501) staff       (20)      650 2023-06-28 09:18:42.000000 f5project-0.0.1/setup.py
+drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-10 23:54:07.786023 f5project-0.0.3/
+-rw-r--r--   0 j3ymac     (501) staff       (20)     1066 2023-06-28 09:15:27.000000 f5project-0.0.3/LICENSE
+-rw-r--r--   0 j3ymac     (501) staff       (20)     5176 2023-07-10 23:54:07.785899 f5project-0.0.3/PKG-INFO
+-rw-r--r--   0 j3ymac     (501) staff       (20)     4727 2023-07-10 23:53:10.000000 f5project-0.0.3/README.md
+drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-10 23:54:07.785191 f5project-0.0.3/f5project/
+-rw-r--r--   0 j3ymac     (501) staff       (20)    11747 2023-07-10 23:27:29.000000 f5project-0.0.3/f5project/__init__.py
+drwxr-xr-x   0 j3ymac     (501) staff       (20)        0 2023-07-10 23:54:07.785745 f5project-0.0.3/f5project.egg-info/
+-rw-r--r--   0 j3ymac     (501) staff       (20)     5176 2023-07-10 23:54:07.000000 f5project-0.0.3/f5project.egg-info/PKG-INFO
+-rw-r--r--   0 j3ymac     (501) staff       (20)      180 2023-07-10 23:54:07.000000 f5project-0.0.3/f5project.egg-info/SOURCES.txt
+-rw-r--r--   0 j3ymac     (501) staff       (20)        1 2023-07-10 23:54:07.000000 f5project-0.0.3/f5project.egg-info/dependency_links.txt
+-rw-r--r--   0 j3ymac     (501) staff       (20)       10 2023-07-10 23:54:07.000000 f5project-0.0.3/f5project.egg-info/top_level.txt
+-rw-r--r--   0 j3ymac     (501) staff       (20)       38 2023-07-10 23:54:07.786062 f5project-0.0.3/setup.cfg
+-rw-r--r--   0 j3ymac     (501) staff       (20)      701 2023-07-10 23:51:11.000000 f5project-0.0.3/setup.py
```

### Comparing `f5project-0.0.1/LICENSE` & `f5project-0.0.3/LICENSE`

 * *Files identical despite different names*

