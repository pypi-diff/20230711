# Comparing `tmp/pyanalyticsgit-0.4.tar.gz` & `tmp/pyanalyticsgit-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyanalyticsgit-0.4.tar", last modified: Tue Jul 11 05:12:21 2023, max compression
+gzip compressed data, was "pyanalyticsgit-0.5.tar", last modified: Tue Jul 11 16:02:49 2023, max compression
```

## Comparing `pyanalyticsgit-0.4.tar` & `pyanalyticsgit-0.5.tar`

### file list

```diff
@@ -1,24 +1,18 @@
-drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-11 05:12:21.295520 pyanalyticsgit-0.4/
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1064 2023-07-10 20:09:22.000000 pyanalyticsgit-0.4/LICENSE
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     2670 2023-07-11 05:12:21.295520 pyanalyticsgit-0.4/PKG-INFO
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     2335 2023-07-10 20:09:46.000000 pyanalyticsgit-0.4/README.md
-drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-11 05:12:21.291522 pyanalyticsgit-0.4/analyticsgit/
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)        0 2023-07-11 04:53:20.000000 pyanalyticsgit-0.4/analyticsgit/__init__.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     3887 2023-07-11 05:04:23.000000 pyanalyticsgit-0.4/analyticsgit/automatizar.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     4477 2023-07-11 04:43:02.000000 pyanalyticsgit-0.4/analyticsgit/commit.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     2509 2023-07-11 04:35:53.000000 pyanalyticsgit-0.4/analyticsgit/connect.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     4140 2023-07-11 04:20:34.000000 pyanalyticsgit-0.4/analyticsgit/issue.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     3045 2023-07-11 04:20:58.000000 pyanalyticsgit-0.4/analyticsgit/milestone.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      188 2023-07-11 04:30:58.000000 pyanalyticsgit-0.4/analyticsgit/monitoramento.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     3404 2023-07-11 04:38:23.000000 pyanalyticsgit-0.4/analyticsgit/relatorio.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1132 2023-07-10 19:56:48.000000 pyanalyticsgit-0.4/analyticsgit/test_linux.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1134 2023-07-10 19:56:40.000000 pyanalyticsgit-0.4/analyticsgit/test_macos.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      838 2023-07-10 19:09:46.000000 pyanalyticsgit-0.4/analyticsgit/test_windows.py
-drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-11 05:12:21.295520 pyanalyticsgit-0.4/pyanalyticsgit.egg-info/
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     2670 2023-07-11 05:12:21.000000 pyanalyticsgit-0.4/pyanalyticsgit.egg-info/PKG-INFO
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      502 2023-07-11 05:12:21.000000 pyanalyticsgit-0.4/pyanalyticsgit.egg-info/SOURCES.txt
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)        1 2023-07-11 05:12:21.000000 pyanalyticsgit-0.4/pyanalyticsgit.egg-info/dependency_links.txt
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       92 2023-07-11 05:12:21.000000 pyanalyticsgit-0.4/pyanalyticsgit.egg-info/requires.txt
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       13 2023-07-11 05:12:21.000000 pyanalyticsgit-0.4/pyanalyticsgit.egg-info/top_level.txt
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       38 2023-07-11 05:12:21.295520 pyanalyticsgit-0.4/setup.cfg
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      722 2023-07-11 05:11:46.000000 pyanalyticsgit-0.4/setup.py
+drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-11 16:02:49.287697 pyanalyticsgit-0.5/
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1064 2023-07-10 20:09:22.000000 pyanalyticsgit-0.5/LICENSE
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     2668 2023-07-11 16:02:49.283697 pyanalyticsgit-0.5/PKG-INFO
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     2335 2023-07-10 20:09:46.000000 pyanalyticsgit-0.5/README.md
+drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-11 16:02:49.283697 pyanalyticsgit-0.5/pyanalyticsgit/
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       19 2023-07-11 15:56:19.000000 pyanalyticsgit-0.5/pyanalyticsgit/__init__.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      227 2023-07-11 16:00:17.000000 pyanalyticsgit-0.5/pyanalyticsgit/monitoramento.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1137 2023-07-11 16:01:40.000000 pyanalyticsgit-0.5/pyanalyticsgit/test_linux.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1139 2023-07-11 16:01:51.000000 pyanalyticsgit-0.5/pyanalyticsgit/test_macos.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      843 2023-07-11 16:02:01.000000 pyanalyticsgit-0.5/pyanalyticsgit/test_windows.py
+drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-11 16:02:49.283697 pyanalyticsgit-0.5/pyanalyticsgit.egg-info/
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     2668 2023-07-11 16:02:49.000000 pyanalyticsgit-0.5/pyanalyticsgit.egg-info/PKG-INFO
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      363 2023-07-11 16:02:49.000000 pyanalyticsgit-0.5/pyanalyticsgit.egg-info/SOURCES.txt
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)        1 2023-07-11 16:02:49.000000 pyanalyticsgit-0.5/pyanalyticsgit.egg-info/dependency_links.txt
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       92 2023-07-11 16:02:49.000000 pyanalyticsgit-0.5/pyanalyticsgit.egg-info/requires.txt
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       15 2023-07-11 16:02:49.000000 pyanalyticsgit-0.5/pyanalyticsgit.egg-info/top_level.txt
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       38 2023-07-11 16:02:49.287697 pyanalyticsgit-0.5/setup.cfg
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      723 2023-07-11 16:00:37.000000 pyanalyticsgit-0.5/setup.py
```

### Comparing `pyanalyticsgit-0.4/LICENSE` & `pyanalyticsgit-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.4/PKG-INFO` & `pyanalyticsgit-0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pyanalyticsgit
-Version: 0.4
+Version: 0.5
 Summary: Biblioteca PyAnalyticsGit para gerar relatórios Git.
 Home-page: UNKNOWN
 Author: Jefferson Sena
 Author-email: jeffersonsena12144@gmail.com
 License: MIT License
-Keywords: Py Analytics Git
+Keywords: pyAnalyticsGit
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 📝 Descrição
 O PyAnalyticsGit é um projeto em Python criado por estudantes de Engenharia de Software que tem como funcionalidades, a biblioteca do PyAnalyticsGit possibilita que o usuário consiga gerar relatórios automatizados com base em dados de repositórios do GitHub, tais quais, histórico de commits, nome do commit, branch, tamanho do log, etc...
```

### Comparing `pyanalyticsgit-0.4/README.md` & `pyanalyticsgit-0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.4/analyticsgit/test_linux.py` & `pyanalyticsgit-0.5/pyanalyticsgit/test_linux.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .automatizar import Automatizar
+from .repo.automatizar import Automatizar
 from pathlib import Path
 
 def test_encontra_path_biblioteca(monkeypatch):
     teste_path = "/home/runner/work/2023.1-PyAnalyticsGit/2023.1-PyAnalyticsGit/pyAnalyticsGit/monitoramento.py"
     def mock_home():
         return Path(teste_path)
     monkeypatch.setattr(Path, "home", mock_home)
```

### Comparing `pyanalyticsgit-0.4/analyticsgit/test_macos.py` & `pyanalyticsgit-0.5/pyanalyticsgit/test_macos.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .automatizar import Automatizar
+from .repo.automatizar import Automatizar
 from pathlib import Path
 
 def test_encontra_path_biblioteca(monkeypatch):
     teste_path = "/Users/runner/work/2023.1-PyAnalyticsGit/2023.1-PyAnalyticsGit/pyAnalyticsGit/monitoramento.py"
     def mock_home():
         return Path(teste_path)
     monkeypatch.setattr(Path, "home", mock_home)
```

### Comparing `pyanalyticsgit-0.4/analyticsgit/test_windows.py` & `pyanalyticsgit-0.5/pyanalyticsgit/test_windows.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .automatizar import Automatizar
+from .repo.automatizar import Automatizar
 from pathlib import Path
 
 def test_encontra_path_biblioteca_windows(monkeypatch):
     teste_path = Automatizar.encontra_path_biblioteca()
     resultado = Automatizar.encontra_path_biblioteca()
     assert resultado == teste_path
```

### Comparing `pyanalyticsgit-0.4/pyanalyticsgit.egg-info/PKG-INFO` & `pyanalyticsgit-0.5/pyanalyticsgit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pyanalyticsgit
-Version: 0.4
+Version: 0.5
 Summary: Biblioteca PyAnalyticsGit para gerar relatórios Git.
 Home-page: UNKNOWN
 Author: Jefferson Sena
 Author-email: jeffersonsena12144@gmail.com
 License: MIT License
-Keywords: Py Analytics Git
+Keywords: pyAnalyticsGit
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 📝 Descrição
 O PyAnalyticsGit é um projeto em Python criado por estudantes de Engenharia de Software que tem como funcionalidades, a biblioteca do PyAnalyticsGit possibilita que o usuário consiga gerar relatórios automatizados com base em dados de repositórios do GitHub, tais quais, histórico de commits, nome do commit, branch, tamanho do log, etc...
```

### Comparing `pyanalyticsgit-0.4/setup.py` & `pyanalyticsgit-0.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 from setuptools.dist import Distribution
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 setup(name='pyanalyticsgit',
-    version='0.4',
+    version='0.5',
     license='MIT License',
     author='Jefferson Sena',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='jeffersonsena12144@gmail.com',
-    keywords='Py Analytics Git',
+    keywords='pyAnalyticsGit',
     description=u'Biblioteca PyAnalyticsGit para gerar relatórios Git.',
-    packages=['analyticsgit'],
+    packages=['pyanalyticsgit'],
     install_requires=['matplotlib==3.7.1', 
                       'python-dotenv==1.0.0',
                       'Requests==2.31.0',
                       'setuptools==59.6.0',
-                      'wordcloud==1.9.2'],)
+                      'wordcloud==1.9.2'],)
```

