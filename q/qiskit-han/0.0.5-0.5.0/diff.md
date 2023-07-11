# Comparing `tmp/qiskit_han-0.0.5.tar.gz` & `tmp/qiskit_han-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "qiskit_han-0.5.0.tar", last modified: Tue Jul 11 09:59:55 2023, max compression
```

## Comparing `qiskit_han-0.0.5.tar` & `qiskit_han-0.5.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     5001 2020-02-02 00:00:00.000000 qiskit_han-0.0.5/Untitled.ipynb
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 qiskit_han-0.0.5/qiskit.json
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 qiskit_han-0.0.5/result.json
--rw-r--r--   0        0        0     5040 2020-02-02 00:00:00.000000 qiskit_han-0.0.5/.ipynb_checkpoints/Untitled-checkpoint.ipynb
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 qiskit_han-0.0.5/qiskit_han/__init__.py
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 qiskit_han-0.0.5/qiskit_han/backend.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 qiskit_han-0.0.5/qiskit_han/job.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 qiskit_han-0.0.5/qiskit_han/provider.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 qiskit_han-0.0.5/qiskit_han/.ipynb_checkpoints/Untitled-checkpoint.ipynb
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 qiskit_han-0.0.5/LICENSE
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 qiskit_han-0.0.5/README.md
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 qiskit_han-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 qiskit_han-0.0.5/PKG-INFO
+drwxr-xr-x   0 hangyulson   (501) staff       (20)        0 2023-07-11 09:59:55.831164 qiskit_han-0.5.0/
+-rw-r--r--   0 hangyulson   (501) staff       (20)      330 2023-07-11 09:59:55.831238 qiskit_han-0.5.0/PKG-INFO
+-rw-r--r--   0 hangyulson   (501) staff       (20)       26 2023-04-08 21:37:34.000000 qiskit_han-0.5.0/README.md
+drwxr-xr-x   0 hangyulson   (501) staff       (20)        0 2023-07-11 09:59:55.830438 qiskit_han-0.5.0/qiskit_han.egg-info/
+-rw-r--r--   0 hangyulson   (501) staff       (20)      330 2023-07-11 09:59:55.000000 qiskit_han-0.5.0/qiskit_han.egg-info/PKG-INFO
+-rw-r--r--   0 hangyulson   (501) staff       (20)      239 2023-07-11 09:59:55.000000 qiskit_han-0.5.0/qiskit_han.egg-info/SOURCES.txt
+-rw-r--r--   0 hangyulson   (501) staff       (20)        1 2023-07-11 09:59:55.000000 qiskit_han-0.5.0/qiskit_han.egg-info/dependency_links.txt
+-rw-r--r--   0 hangyulson   (501) staff       (20)       40 2023-07-11 09:59:55.000000 qiskit_han-0.5.0/qiskit_han.egg-info/requires.txt
+-rw-r--r--   0 hangyulson   (501) staff       (20)        9 2023-07-11 09:59:55.000000 qiskit_han-0.5.0/qiskit_han.egg-info/top_level.txt
+drwxr-xr-x   0 hangyulson   (501) staff       (20)        0 2023-07-11 09:59:55.830894 qiskit_han-0.5.0/quantier/
+-rw-r--r--   0 hangyulson   (501) staff       (20)       55 2023-07-11 09:42:46.000000 qiskit_han-0.5.0/quantier/__init__.py
+-rw-r--r--   0 hangyulson   (501) staff       (20)     4181 2023-07-11 09:43:02.000000 qiskit_han-0.5.0/quantier/quantier.py
+-rw-r--r--   0 hangyulson   (501) staff       (20)       38 2023-07-11 09:59:55.831488 qiskit_han-0.5.0/setup.cfg
+-rw-r--r--   0 hangyulson   (501) staff       (20)      690 2023-07-11 09:59:48.000000 qiskit_han-0.5.0/setup.py
```

