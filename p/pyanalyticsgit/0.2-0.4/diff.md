# Comparing `tmp/pyanalyticsgit-0.2.tar.gz` & `tmp/pyanalyticsgit-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyanalyticsgit-0.2.tar", last modified: Tue Jul 11 00:11:08 2023, max compression
+gzip compressed data, was "pyanalyticsgit-0.4.tar", last modified: Tue Jul 11 05:12:21 2023, max compression
```

## Comparing `pyanalyticsgit-0.2.tar` & `pyanalyticsgit-0.4.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-11 00:11:08.770599 pyanalyticsgit-0.2/
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1064 2023-07-10 20:09:22.000000 pyanalyticsgit-0.2/LICENSE
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     2670 2023-07-11 00:11:08.770599 pyanalyticsgit-0.2/PKG-INFO
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     2335 2023-07-10 20:09:46.000000 pyanalyticsgit-0.2/README.md
-drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-11 00:11:08.766598 pyanalyticsgit-0.2/analyticsgit/
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)        0 2023-07-10 20:01:33.000000 pyanalyticsgit-0.2/analyticsgit/__init__.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     3889 2023-07-10 19:25:20.000000 pyanalyticsgit-0.2/analyticsgit/automatizar.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     4362 2023-07-10 20:34:01.000000 pyanalyticsgit-0.2/analyticsgit/commit.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     2509 2023-07-10 19:21:15.000000 pyanalyticsgit-0.2/analyticsgit/connect.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     4136 2023-07-10 20:34:01.000000 pyanalyticsgit-0.2/analyticsgit/issue.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       82 2023-07-10 17:59:42.000000 pyanalyticsgit-0.2/analyticsgit/main.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     3042 2023-07-10 20:34:01.000000 pyanalyticsgit-0.2/analyticsgit/milestone.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      267 2023-07-10 20:34:01.000000 pyanalyticsgit-0.2/analyticsgit/monitoramento.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     3457 2023-07-10 20:34:01.000000 pyanalyticsgit-0.2/analyticsgit/relatorio.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1132 2023-07-10 19:56:48.000000 pyanalyticsgit-0.2/analyticsgit/test_linux.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1134 2023-07-10 19:56:40.000000 pyanalyticsgit-0.2/analyticsgit/test_macos.py
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      838 2023-07-10 19:09:46.000000 pyanalyticsgit-0.2/analyticsgit/test_windows.py
-drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-11 00:11:08.766598 pyanalyticsgit-0.2/pyanalyticsgit.egg-info/
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     2670 2023-07-11 00:11:08.000000 pyanalyticsgit-0.2/pyanalyticsgit.egg-info/PKG-INFO
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      523 2023-07-11 00:11:08.000000 pyanalyticsgit-0.2/pyanalyticsgit.egg-info/SOURCES.txt
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)        1 2023-07-11 00:11:08.000000 pyanalyticsgit-0.2/pyanalyticsgit.egg-info/dependency_links.txt
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)        9 2023-07-11 00:11:08.000000 pyanalyticsgit-0.2/pyanalyticsgit.egg-info/requires.txt
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       13 2023-07-11 00:11:08.000000 pyanalyticsgit-0.2/pyanalyticsgit.egg-info/top_level.txt
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       38 2023-07-11 00:11:08.770599 pyanalyticsgit-0.2/setup.cfg
--rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      538 2023-07-11 00:10:59.000000 pyanalyticsgit-0.2/setup.py
+drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-11 05:12:21.295520 pyanalyticsgit-0.4/
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1064 2023-07-10 20:09:22.000000 pyanalyticsgit-0.4/LICENSE
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     2670 2023-07-11 05:12:21.295520 pyanalyticsgit-0.4/PKG-INFO
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     2335 2023-07-10 20:09:46.000000 pyanalyticsgit-0.4/README.md
+drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-11 05:12:21.291522 pyanalyticsgit-0.4/analyticsgit/
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)        0 2023-07-11 04:53:20.000000 pyanalyticsgit-0.4/analyticsgit/__init__.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     3887 2023-07-11 05:04:23.000000 pyanalyticsgit-0.4/analyticsgit/automatizar.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     4477 2023-07-11 04:43:02.000000 pyanalyticsgit-0.4/analyticsgit/commit.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     2509 2023-07-11 04:35:53.000000 pyanalyticsgit-0.4/analyticsgit/connect.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     4140 2023-07-11 04:20:34.000000 pyanalyticsgit-0.4/analyticsgit/issue.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     3045 2023-07-11 04:20:58.000000 pyanalyticsgit-0.4/analyticsgit/milestone.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      188 2023-07-11 04:30:58.000000 pyanalyticsgit-0.4/analyticsgit/monitoramento.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     3404 2023-07-11 04:38:23.000000 pyanalyticsgit-0.4/analyticsgit/relatorio.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1132 2023-07-10 19:56:48.000000 pyanalyticsgit-0.4/analyticsgit/test_linux.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     1134 2023-07-10 19:56:40.000000 pyanalyticsgit-0.4/analyticsgit/test_macos.py
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      838 2023-07-10 19:09:46.000000 pyanalyticsgit-0.4/analyticsgit/test_windows.py
+drwxrwxr-x   0 jefferson  (1000) jefferson  (1000)        0 2023-07-11 05:12:21.295520 pyanalyticsgit-0.4/pyanalyticsgit.egg-info/
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)     2670 2023-07-11 05:12:21.000000 pyanalyticsgit-0.4/pyanalyticsgit.egg-info/PKG-INFO
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      502 2023-07-11 05:12:21.000000 pyanalyticsgit-0.4/pyanalyticsgit.egg-info/SOURCES.txt
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)        1 2023-07-11 05:12:21.000000 pyanalyticsgit-0.4/pyanalyticsgit.egg-info/dependency_links.txt
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       92 2023-07-11 05:12:21.000000 pyanalyticsgit-0.4/pyanalyticsgit.egg-info/requires.txt
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       13 2023-07-11 05:12:21.000000 pyanalyticsgit-0.4/pyanalyticsgit.egg-info/top_level.txt
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)       38 2023-07-11 05:12:21.295520 pyanalyticsgit-0.4/setup.cfg
+-rw-rw-r--   0 jefferson  (1000) jefferson  (1000)      722 2023-07-11 05:11:46.000000 pyanalyticsgit-0.4/setup.py
```

### Comparing `pyanalyticsgit-0.2/LICENSE` & `pyanalyticsgit-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.2/PKG-INFO` & `pyanalyticsgit-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyanalyticsgit
-Version: 0.2
+Version: 0.4
 Summary: Biblioteca PyAnalyticsGit para gerar relatórios Git.
 Home-page: UNKNOWN
 Author: Jefferson Sena
 Author-email: jeffersonsena12144@gmail.com
 License: MIT License
 Keywords: Py Analytics Git
 Platform: UNKNOWN
```

### Comparing `pyanalyticsgit-0.2/README.md` & `pyanalyticsgit-0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.2/analyticsgit/automatizar.py` & `pyanalyticsgit-0.4/analyticsgit/automatizar.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import platform
 import sys
 
 class Automatizar:
     caminho_repositorio = str
     path_biblioteca = str
     localizacao_monitoramento = str
-    nome_biblioteca = "pyAnalyticsGit" 
+    nome_biblioteca = "analyticsgit" 
     path_post_commit = str
     path_python = ""
     comando_post_commit = str
 
     def __init(self):
         pass
```

### Comparing `pyanalyticsgit-0.2/analyticsgit/commit.py` & `pyanalyticsgit-0.4/analyticsgit/commit.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,108 +1,109 @@
-from collections import defaultdict
-import matplotlib.pyplot as plt
-from wordcloud import STOPWORDS, WordCloud
-import os
-from pyAnalyticsGit.analyticsgit.connect import Connect,api_name,api_user
-
-diretorio_raiz = os.path.abspath(os.path.dirname(__file__))
-
-nome_pasta = "docs"
-grafico = 'grafico.png'
-grafico_nuvem = 'grafico_nuvem.png'
-
-caminho_pasta = os.path.join(diretorio_raiz, nome_pasta)
-
-
-class Commits:
-    def __init__(self, user = api_user, repo=api_name):
-        connect = Connect()
-        self.commits = connect.connect_commit(user,repo)
-        self.palavras_ignoradas = ["o","a","e","i","u","de","des","da","das","do","dos","md","para","que"]
-
-    def listar_nomes_commits(self):
-        nomes_commits = []
-        for commit in self.commits:
-            nome_commit = commit["commit"]["message"]
-            nomes_commits.append(nome_commit)
-        return nomes_commits    
-
-    def gerar_nuvem_commits(self):
-        nomes_commits = self.listar_nomes_commits()
-        texto = " ".join(nomes_commits)
-
-        stopwords = set(STOPWORDS)
-        stopwords.update(self.palavras_ignoradas) 
-
-        wordcloud = WordCloud(width=800, height=400, background_color='white', stopwords=stopwords,
-                              colormap='viridis', max_words=300).generate(texto)
-
-        plt.figure(figsize=(10, 5))
-        plt.imshow(wordcloud, interpolation='bilinear') 
-        plt.axis('off')
-        plt.title('Nuvem de palavras com nomes dos Commits')
-
-        if os.path.exists(os.path.join(caminho_pasta,grafico_nuvem)):
-            os.remove(os.path.join(caminho_pasta,grafico_nuvem))
-
-        plt.savefig(os.path.join(caminho_pasta,grafico_nuvem))
-        plt.close()    
-
-    def criar_grafico_commit(self):
-        commit_authors = defaultdict(int)
-        for commit in self.commits:
-            author = commit["commit"]["author"]["name"]
-            commit_authors[author] += 1
-
-        authors = list(commit_authors.keys())
-        commit_numbers = list(commit_authors.values())
-
-        plt.bar(authors, commit_numbers, color='darkred')
-        plt.xlabel('Autores')
-        plt.ylabel('Número de Commits', color='darkred')
-        plt.title('Gráfico de Commits por Autor', fontsize=16, color='black')
-        plt.xticks(rotation=45)
-        plt.gca().set_facecolor('black')
-        if os.path.exists(os.path.join(caminho_pasta,grafico)):
-            os.remove(os.path.join(caminho_pasta,grafico))
-
-        plt.savefig(os.path.join(caminho_pasta,grafico))
-        plt.close()
-
-    def criar_tabela_commit(self, relatorio_file):
-        # Tabela de quantidade de commits por membro
-        commit_count = {}
-        commit_datas = {}
-        for commit in self.commits:
-            author = commit["commit"]["author"]["name"]
-            if author in commit_count:
-                commit_count[author] += 1
-                commit_datas[author].append(commit["commit"]["author"]["date"])
-            else:
-                commit_count[author] = 1
-                commit_datas[author] = [commit["commit"]["author"]["date"]]    
-
-        with open(relatorio_file, "a+", encoding="utf-8") as file:
-            file.write("# Tabela - Quantidade de Commits por Membro\n\n")
-            file.write("| Membro | Quantidade de Commits |\n")
-            file.write("| --- | ---: |\n")
-            for author, count in commit_count.items():
-                file.write(f"| {author} | {count} |\n")
-            file.write("\n")
-
-        with open(relatorio_file, "a+", encoding="utf-8") as file:
-            file.write("# Tabela de Commits por Autor\n\n")
-
-            for author in commit_count.keys():
-                file.write(f"## {author}\n\n")
-                file.write("| Commit | Data |\n")
-                file.write("| --- | --- |\n")
-        
-                author_commits = [commit for commit in self.commits if commit["commit"]["author"]["name"] == author]
-        
-                for commit in author_commits:
-                    commit_message = commit["commit"]["message"]
-                    commit_date = commit["commit"]["author"]["date"].split("T")[0]
-                    commit_resume = " ".join(commit_message.split()[:7]) + "..." if len(commit_message.split()) > 7 else commit_message
-                    file.write(f"| {commit_resume} | {commit_date} |\n")
-                file.write("\n")
-            file.write("\n")
+from collections import defaultdict
+import matplotlib.pyplot as plt
+from wordcloud import STOPWORDS, WordCloud
+import os
+from connect import  Connect, api_name, api_user
+
+# diretorio_raiz = os.path.abspath(os.path.dirname(__file__))
+diretorio_raiz = os.getcwd()
+
+nome_pasta = "docs"
+grafico = 'grafico.png'
+grafico_nuvem = 'grafico_nuvem.png'
+
+caminho_pasta = os.path.join(diretorio_raiz, nome_pasta)
+
+
+class Commits:
+    def __init__(self, user = api_user, repo=api_name):
+        connect = Connect()
+        self.commits = connect.connect_commit(user,repo)
+        self.palavras_ignoradas = ["o","a","e","i","u","de","des","da","das","do","dos","md","para","que"]
+
+    def listar_nomes_commits(self):
+        nomes_commits = []
+        for commit in self.commits:
+            nome_commit = commit["commit"]["message"]
+            nomes_commits.append(nome_commit)
+        return nomes_commits    
+
+    def gerar_nuvem_commits(self):
+        nomes_commits = self.listar_nomes_commits()
+        texto = " ".join(nomes_commits)
+
+        stopwords = set(STOPWORDS)
+        stopwords.update(self.palavras_ignoradas) 
+
+        wordcloud = WordCloud(width=800, height=400, background_color='white', stopwords=stopwords,
+                              colormap='viridis', max_words=300).generate(texto)
+
+        plt.figure(figsize=(10, 5))
+        plt.imshow(wordcloud, interpolation='bilinear') 
+        plt.axis('off')
+        plt.title('Nuvem de palavras com nomes dos Commits')
+
+        if os.path.exists(os.path.join(caminho_pasta,grafico_nuvem)):
+            os.remove(os.path.join(caminho_pasta,grafico_nuvem))
+
+        plt.savefig(os.path.join(caminho_pasta,grafico_nuvem))
+        plt.close()    
+
+    def criar_grafico_commit(self):
+        commit_authors = defaultdict(int)
+        for commit in self.commits:
+            author = commit["commit"]["author"]["name"]
+            commit_authors[author] += 1
+
+        authors = list(commit_authors.keys())
+        commit_numbers = list(commit_authors.values())
+
+        plt.bar(authors, commit_numbers, color='darkred')
+        plt.xlabel('Autores')
+        plt.ylabel('Número de Commits', color='darkred')
+        plt.title('Gráfico de Commits por Autor', fontsize=16, color='black')
+        plt.xticks(rotation=45)
+        plt.gca().set_facecolor('black')
+        if os.path.exists(os.path.join(caminho_pasta,grafico)):
+            os.remove(os.path.join(caminho_pasta,grafico))
+
+        plt.savefig(os.path.join(caminho_pasta,grafico))
+        plt.close()
+
+    def criar_tabela_commit(self, relatorio_file):
+        # Tabela de quantidade de commits por membro
+        commit_count = {}
+        commit_datas = {}
+        for commit in self.commits:
+            author = commit["commit"]["author"]["name"]
+            if author in commit_count:
+                commit_count[author] += 1
+                commit_datas[author].append(commit["commit"]["author"]["date"])
+            else:
+                commit_count[author] = 1
+                commit_datas[author] = [commit["commit"]["author"]["date"]]    
+
+        with open(relatorio_file, "a+", encoding="utf-8") as file:
+            file.write("# Tabela - Quantidade de Commits por Membro\n\n")
+            file.write("| Membro | Quantidade de Commits |\n")
+            file.write("| --- | ---: |\n")
+            for author, count in commit_count.items():
+                file.write(f"| {author} | {count} |\n")
+            file.write("\n")
+
+        with open(relatorio_file, "a+", encoding="utf-8") as file:
+            file.write("# Tabela de Commits por Autor\n\n")
+
+            for author in commit_count.keys():
+                file.write(f"## {author}\n\n")
+                file.write("| Commit | Data |\n")
+                file.write("| --- | --- |\n")
+        
+                author_commits = [commit for commit in self.commits if commit["commit"]["author"]["name"] == author]
+        
+                for commit in author_commits:
+                    commit_message = commit["commit"]["message"]
+                    commit_date = commit["commit"]["author"]["date"].split("T")[0]
+                    commit_resume = " ".join(commit_message.split()[:7]) + "..." if len(commit_message.split()) > 7 else commit_message
+                    file.write(f"| {commit_resume} | {commit_date} |\n")
+                file.write("\n")
+            file.write("\n")
```

### Comparing `pyanalyticsgit-0.2/analyticsgit/connect.py` & `pyanalyticsgit-0.4/analyticsgit/connect.py`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.2/analyticsgit/issue.py` & `pyanalyticsgit-0.4/analyticsgit/issue.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from collections import defaultdict
 import matplotlib.pyplot as plt
 import os
-from pyAnalyticsGit.analyticsgit.connect import Connect,api_name,api_user
+from connect import Connect,api_name,api_user
+
+# diretorio_raiz = os.path.abspath(os.path.dirname(__file__))
+diretorio_raiz = os.getcwd()
 
-diretorio_raiz = os.path.abspath(os.path.dirname(__file__))
 
 nome_pasta = "docs"
 grafico_issue = 'grafico_issue.png'
 grafico_pizza = 'grafico_pizza.png'
 
 caminho_pasta = os.path.join(diretorio_raiz, nome_pasta)
```

### Comparing `pyanalyticsgit-0.2/analyticsgit/milestone.py` & `pyanalyticsgit-0.4/analyticsgit/milestone.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from collections import defaultdict
 import matplotlib.pyplot as plt
 import os
 from datetime import datetime
-from pyAnalyticsGit.analyticsgit.connect import Connect,api_user,api_name
+from connect import Connect,api_user,api_name
 
-diretorio_raiz = os.path.abspath(os.path.dirname(__file__))
+# diretorio_raiz = os.path.abspath(os.path.dirname(__file__))
+diretorio_raiz = os.getcwd()
 
 nome_pasta = "docs"
 grafico_milestone = 'grafico_milestone.png'
 
 caminho_pasta = os.path.join(diretorio_raiz, nome_pasta)
 
 class Milestone:
```

### Comparing `pyanalyticsgit-0.2/analyticsgit/relatorio.py` & `pyanalyticsgit-0.4/analyticsgit/relatorio.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 from commit import Commits
-from pyAnalyticsGit.analyticsgit.connect import api_user,api_name
+from connect import api_name, api_user
 from issue import Issue
 from milestone import Milestone
 
-diretorio_raiz = os.path.abspath(os.path.dirname(__file__))
+# diretorio_raiz = os.path.abspath(os.path.dirname(__file__))
+diretorio_raiz = os.getcwd()
 
 nome_pasta = "docs"
 
-
 caminho_pasta = os.path.join(diretorio_raiz, nome_pasta)
 
 class Relatorio:
     def __init__(self):
         self.nome_arquivo = "relatorio_padrao.md"
         self.titulo = "# PyAnalyticsGit - Relatório automatizado"
         if not os.path.exists(caminho_pasta):
@@ -79,14 +79,10 @@
             arq.write("# Milestones\n\n")
             arq.write("## Gráfico de Milestones\n\n")
             arq.write("<div align='center'>\n\n")
             arq.write("![Gráfico de Milestones](grafico_milestone.png)\n\n")
             arq.write("</div>\n\n")
 
         grafico_tabela_milestone.criar_tabela_milestone(self.caminho_arquivo)
-
-
-relatorio = Relatorio()
-relatorio.gerar_relatorio()
```

### Comparing `pyanalyticsgit-0.2/analyticsgit/test_linux.py` & `pyanalyticsgit-0.4/analyticsgit/test_linux.py`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.2/analyticsgit/test_macos.py` & `pyanalyticsgit-0.4/analyticsgit/test_macos.py`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.2/analyticsgit/test_windows.py` & `pyanalyticsgit-0.4/analyticsgit/test_windows.py`

 * *Files identical despite different names*

### Comparing `pyanalyticsgit-0.2/pyanalyticsgit.egg-info/PKG-INFO` & `pyanalyticsgit-0.4/pyanalyticsgit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyanalyticsgit
-Version: 0.2
+Version: 0.4
 Summary: Biblioteca PyAnalyticsGit para gerar relatórios Git.
 Home-page: UNKNOWN
 Author: Jefferson Sena
 Author-email: jeffersonsena12144@gmail.com
 License: MIT License
 Keywords: Py Analytics Git
 Platform: UNKNOWN
```

### Comparing `pyanalyticsgit-0.2/setup.py` & `pyanalyticsgit-0.4/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from setuptools import setup
 from setuptools.dist import Distribution
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 setup(name='pyanalyticsgit',
-    version='0.2',
+    version='0.4',
     license='MIT License',
     author='Jefferson Sena',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='jeffersonsena12144@gmail.com',
     keywords='Py Analytics Git',
     description=u'Biblioteca PyAnalyticsGit para gerar relatórios Git.',
     packages=['analyticsgit'],
-    install_requires=['requests'],)
+    install_requires=['matplotlib==3.7.1', 
+                      'python-dotenv==1.0.0',
+                      'Requests==2.31.0',
+                      'setuptools==59.6.0',
+                      'wordcloud==1.9.2'],)
```

