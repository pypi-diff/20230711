# Comparing `tmp/pylinefinder-0.1.5.tar.gz` & `tmp/pylinefinder-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylinefinder-0.1.5.tar", max compression
+gzip compressed data, was "pylinefinder-0.1.6.tar", max compression
```

## Comparing `pylinefinder-0.1.5.tar` & `pylinefinder-0.1.6.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-07-09 18:25:21.168640 pylinefinder-0.1.5/README.md
--rw-r--r--   0        0        0     1994 2023-07-11 02:43:40.830583 pylinefinder-0.1.5/pylinefinder/__main__.py
--rw-r--r--   0        0        0      294 2023-07-11 02:44:05.075038 pylinefinder-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      385 1970-01-01 00:00:00.000000 pylinefinder-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-09 18:25:21.168640 pylinefinder-0.1.6/README.md
+-rw-r--r--   0        0        0     1994 2023-07-11 02:47:57.239281 pylinefinder-0.1.6/pylinefinder/__main__.py
+-rw-r--r--   0        0        0      294 2023-07-11 02:49:17.348716 pylinefinder-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      385 1970-01-01 00:00:00.000000 pylinefinder-0.1.6/PKG-INFO
```

### Comparing `pylinefinder-0.1.5/pylinefinder/__main__.py` & `pylinefinder-0.1.6/pylinefinder/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         results = []
         try:
             with open(arquivo) as f1:
                 for line in f1:
                     if trecho.lower() in line.lower():
                         results.append(line)
                         
-            with open('resultado.txt', 'w') as f2:
+            with open('resultado.txt', 'a') as f2:
                 conteudo = ''.join(results)
                 f2.write(conteudo)
                 
                 click.echo('Arquivo raspado com sucesso!')
                 click.echo('Resultado:')
                 for line in results:
                     click.echo(line.strip())
```

