# Comparing `tmp/pylinefinder-0.1.4.tar.gz` & `tmp/pylinefinder-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylinefinder-0.1.4.tar", max compression
+gzip compressed data, was "pylinefinder-0.1.5.tar", max compression
```

## Comparing `pylinefinder-0.1.4.tar` & `pylinefinder-0.1.5.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-07-09 18:25:21.168640 pylinefinder-0.1.4/README.md
--rw-r--r--   0        0        0     1994 2023-07-11 02:41:32.140111 pylinefinder-0.1.4/pylinefinder/__main__.py
--rw-r--r--   0        0        0      294 2023-07-11 02:42:49.881617 pylinefinder-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      385 1970-01-01 00:00:00.000000 pylinefinder-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-09 18:25:21.168640 pylinefinder-0.1.5/README.md
+-rw-r--r--   0        0        0     1994 2023-07-11 02:43:40.830583 pylinefinder-0.1.5/pylinefinder/__main__.py
+-rw-r--r--   0        0        0      294 2023-07-11 02:44:05.075038 pylinefinder-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      385 1970-01-01 00:00:00.000000 pylinefinder-0.1.5/PKG-INFO
```

### Comparing `pylinefinder-0.1.4/pylinefinder/__main__.py` & `pylinefinder-0.1.5/pylinefinder/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
 )
 def parse(arquivo, trecho, extrair):
     if extrair:
         linhas = []
         resultados = []
         try:
-            with open(arquivo) as f1, open('resultado.txt', 'w') as f2:
+            with open(arquivo) as f1, open('resultado.txt', 'a') as f2:
                 for line in f1:
                     if trecho.lower() in line.lower():
                         resultados.append(line)
                     else:
                         linhas.append(line)
                         
                 conteudo = ''.join(resultados)
```

