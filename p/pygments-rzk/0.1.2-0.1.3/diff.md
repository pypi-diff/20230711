# Comparing `tmp/pygments-rzk-0.1.2.tar.gz` & `tmp/pygments-rzk-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygments-rzk-0.1.2.tar", last modified: Fri Jun 30 22:11:47 2023, max compression
+gzip compressed data, was "pygments-rzk-0.1.3.tar", last modified: Mon Jul 10 21:57:17 2023, max compression
```

## Comparing `pygments-rzk-0.1.2.tar` & `pygments-rzk-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:11:47.753845 pygments-rzk-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-30 22:11:36.000000 pygments-rzk-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-30 22:11:36.000000 pygments-rzk-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-30 22:11:47.753845 pygments-rzk-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-30 22:11:36.000000 pygments-rzk-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:11:47.749844 pygments-rzk-0.1.2/images/
--rw-r--r--   0 runner    (1001) docker     (123)   449381 2023-06-30 22:11:36.000000 pygments-rzk-0.1.2/images/latex-highlighting-demo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:11:47.753845 pygments-rzk-0.1.2/pygments_rzk/
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-06-30 22:11:36.000000 pygments-rzk-0.1.2/pygments_rzk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 22:11:47.753845 pygments-rzk-0.1.2/pygments_rzk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-30 22:11:47.000000 pygments-rzk-0.1.2/pygments_rzk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-30 22:11:47.000000 pygments-rzk-0.1.2/pygments_rzk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 22:11:47.000000 pygments-rzk-0.1.2/pygments_rzk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-30 22:11:47.000000 pygments-rzk-0.1.2/pygments_rzk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-30 22:11:47.000000 pygments-rzk-0.1.2/pygments_rzk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-30 22:11:47.000000 pygments-rzk-0.1.2/pygments_rzk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 22:11:47.753845 pygments-rzk-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-30 22:11:36.000000 pygments-rzk-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:57:17.939104 pygments-rzk-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-10 21:57:02.000000 pygments-rzk-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-10 21:57:02.000000 pygments-rzk-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-10 21:57:17.939104 pygments-rzk-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-10 21:57:02.000000 pygments-rzk-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:57:17.939104 pygments-rzk-0.1.3/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   449381 2023-07-10 21:57:02.000000 pygments-rzk-0.1.3/images/latex-highlighting-demo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:57:17.939104 pygments-rzk-0.1.3/pygments_rzk/
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-10 21:57:02.000000 pygments-rzk-0.1.3/pygments_rzk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:57:17.939104 pygments-rzk-0.1.3/pygments_rzk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-10 21:57:17.000000 pygments-rzk-0.1.3/pygments_rzk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-10 21:57:17.000000 pygments-rzk-0.1.3/pygments_rzk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 21:57:17.000000 pygments-rzk-0.1.3/pygments_rzk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-10 21:57:17.000000 pygments-rzk-0.1.3/pygments_rzk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 21:57:17.000000 pygments-rzk-0.1.3/pygments_rzk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-10 21:57:17.000000 pygments-rzk-0.1.3/pygments_rzk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 21:57:17.939104 pygments-rzk-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-07-10 21:57:02.000000 pygments-rzk-0.1.3/setup.py
```

### Comparing `pygments-rzk-0.1.2/LICENSE` & `pygments-rzk-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pygments-rzk-0.1.2/PKG-INFO` & `pygments-rzk-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pygments-rzk
-Version: 0.1.2
+Version: 0.1.3
 Summary: Pygments lexer for Rzk language (of proof assistant for synthetic ∞-categories).
-Home-page: https://github.com/fizruk/pygments-rzk
+Home-page: https://github.com/rzk-lang/pygments-rzk
 Author: Nikolai Kudasov
 Author-email: nickolay.kudasov@gmail.com
 License: BSD 3
 Keywords: pygments rzk lexer
 Classifier: Environment :: Plugins
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -14,24 +14,24 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Pygments higlighter for Rzk
 
-This is a simple [Pygments](https://pygments.org) higlighter for [Rzk](https://github.com/fizruk/rzk), which can be used with [`minted` package](https://www.ctan.org/pkg/minted) when writing rzk code in LaTeX or with [MkDocs](https://www.mkdocs.org) to highlight code in blocks when rendering literate Rzk Markdown files.
+This is a simple [Pygments](https://pygments.org) higlighter for [Rzk](https://github.com/rzk-lang/rzk), which can be used with [`minted` package](https://www.ctan.org/pkg/minted) when writing rzk code in LaTeX or with [MkDocs](https://www.mkdocs.org) to highlight code in blocks when rendering literate Rzk Markdown files.
 
 ## How to use
 
 ### Install
 
 Clone this repository, and install the highlighter using [`pip` installer](https://pip.pypa.io/en/stable/):
 
 ```sh
-git clone https://github.com/fizruk/pygments-rzk.git
+git clone https://github.com/rzk-lang/pygments-rzk.git
 cd pygments-rzk   # enter repository root
 pip install .     # install using pip
 ```
 
 ### Use in MkDocs
 
 To be done.
@@ -66,15 +66,15 @@
 -- path reversal
 #define rev uses (A x y)
   (p : x = y)       -- A path from x to y in A.
   : y = x           -- The reversal will be defined by path induction on p.
   := idJ(A, x, \y' p' -> y' = x, refl, y, p)
 
 -- path composition by induction on the second path
-#define concat 
+#define concat
   (p : x = y)       -- A path from x to y in A.
   (q : y = z)       -- A path from y to z in A.
   : (x = z)
   := idJ(A, y, \z' q' -> (x = z'), p, z, q)
 
 #end path-algebra
 \end{minted}
```

### Comparing `pygments-rzk-0.1.2/README.md` & `pygments-rzk-0.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Pygments higlighter for Rzk
 
-This is a simple [Pygments](https://pygments.org) higlighter for [Rzk](https://github.com/fizruk/rzk), which can be used with [`minted` package](https://www.ctan.org/pkg/minted) when writing rzk code in LaTeX or with [MkDocs](https://www.mkdocs.org) to highlight code in blocks when rendering literate Rzk Markdown files.
+This is a simple [Pygments](https://pygments.org) higlighter for [Rzk](https://github.com/rzk-lang/rzk), which can be used with [`minted` package](https://www.ctan.org/pkg/minted) when writing rzk code in LaTeX or with [MkDocs](https://www.mkdocs.org) to highlight code in blocks when rendering literate Rzk Markdown files.
 
 ## How to use
 
 ### Install
 
 Clone this repository, and install the highlighter using [`pip` installer](https://pip.pypa.io/en/stable/):
 
 ```sh
-git clone https://github.com/fizruk/pygments-rzk.git
+git clone https://github.com/rzk-lang/pygments-rzk.git
 cd pygments-rzk   # enter repository root
 pip install .     # install using pip
 ```
 
 ### Use in MkDocs
 
 To be done.
@@ -48,15 +48,15 @@
 -- path reversal
 #define rev uses (A x y)
   (p : x = y)       -- A path from x to y in A.
   : y = x           -- The reversal will be defined by path induction on p.
   := idJ(A, x, \y' p' -> y' = x, refl, y, p)
 
 -- path composition by induction on the second path
-#define concat 
+#define concat
   (p : x = y)       -- A path from x to y in A.
   (q : y = z)       -- A path from y to z in A.
   : (x = z)
   := idJ(A, y, \z' q' -> (x = z'), p, z, q)
 
 #end path-algebra
 \end{minted}
```

### Comparing `pygments-rzk-0.1.2/images/latex-highlighting-demo.png` & `pygments-rzk-0.1.3/images/latex-highlighting-demo.png`

 * *Files identical despite different names*

### Comparing `pygments-rzk-0.1.2/pygments_rzk/__init__.py` & `pygments-rzk-0.1.3/pygments_rzk/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 __all__ = ["RzkLexer"]
 
 class RzkLexer(pygments.lexer.RegexLexer):
     name = 'Rzk'
     aliases = ['rzk']
     filenames = ['*.rzk']
-    url = 'https://github.com/fizruk/rzk'
+    url = 'https://github.com/rzk-lang/rzk'
     KEYWORDS = [] # ['as', 'uses']
     def get_tokens_unprocessed(self, text):
         for index, token, value in super(RzkLexer,self).get_tokens_unprocessed(text):
             if token is Name and value in self.KEYWORDS:
                 yield index, Keyword, value
             else:
                 yield index, token, value
@@ -31,41 +31,41 @@
         'root': [
             (r'--.*\n', Comment),
             (r'^(#lang)(\s+)((?![-?!.])[^.\\;,#"\]\[)(}{><|\s]*)(?=$|[.\\;,#"\]\[)(}{><|\s])\s*$',
              bygroups(Name.Decorator, Punctuation, String)),
             (r'^(#check|#compute(-whnf|-nf)?|#set-option|#unset-option)(?=$|[.\\;,#"\]\[)(}{><|\s-])',
              bygroups(Name.Decorator)),
             (r'^(#section|#end)(\s+(?![-?!.])[^.\\;,#"\]\[)(}{><|\s]*)?(?=$|[.\\;,#"\]\[)(}{><|\s])',
-             bygroups(Name.Decorator, Name.Entity)),
+             bygroups(Name.Decorator, Name)),
             (r'^(#assume|#variable|#variables)(\s+)((?![-?!.])[^.\\;,#"\]\[)(}{><|:]*)(?=$|[.\\;,#"\]\[)(}{><|\s])',
-             bygroups(Keyword.Declaration, Punctuation, Name.Variable)),
+             bygroups(Keyword.Reserved, Punctuation, Text)),
             (r'^(#def|#define|#postulate)(\s+)((?![-?!.])[^.\\;,#"\]\[)(}{><|\s]*)(?=$|[.\\;,#"\]\[)(}{><|\s])((\s+)(uses)(\s+\()((?![-?!.])[^.\\;,#"\]\[)(}{><|]*)(\)))?',
-             bygroups(Keyword.Declaration, Punctuation, Name.Function, None, Punctuation, Keyword, Punctuation, Name.Variable, Punctuation)),
+             bygroups(Keyword.Reserved, Punctuation, Name.Function, None, Punctuation, Keyword, Punctuation, Text, Punctuation)),
 
             # bultins
-            (r'(?<=[.\\;,#"\]\[)(}{><|\s])(CUBE|TOPE|U(nit)?|𝒰)(?=$|[.\\;,#"\]\[)(}{><|\s])',
+            (r'(?<=[.\\;,#"\]\[)(}{><|\s])(CUBE|TOPE|U(nit)?)(?=$|[.\\;,#"\]\[)(}{><|\s])',
              Keyword.Type),
-            (r'(?<=[.\\;,#"\]\[)(}{><|\s])(1|2|𝟙|𝟚|Sigma|∑|Σ)(?=$|[.\\;,#"\]\[)(}{><|\s])',
+            (r'(?<=[.\\;,#"\]\[)(}{><|\s])(1|2|Sigma|∑|Σ)(?=$|[.\\;,#"\]\[)(}{><|\s])',
              Keyword.Type),
-            (r'(===|<=|\\/|/\\)',
-             Operator),
-            (r'(⊤|⊥|\*_1|⋆)|(?<=[.\\;,#"\]\[)(}{><|\s])(0_2|1_2|TOP|BOT)(?=$|[.\\;,#"\]\[)(}{><|\s])',
-             Name.Constant),
-            (r'(?<=[.\\;,#"\]\[)(}{><|\s])(recOR|rec∨|recBOT|rec⊥|idJ|refl|first|second|π₁|π₂|unit)((?=$|[.\\;,#"\]\[)(}{><|\s])|(?=_{))',
-             Name.Constant),
+            (r'(===|≡|<=|≤|\\/|∨|/\\|∧)',
+             String.Other),
+            (r'(⊤|⊥|\*_1|\*₁)|(?<=[.\\;,#"\]\[)(}{><|\s])(0_2|0₂|1_2|1₂|TOP|BOT)(?=$|[.\\;,#"\]\[)(}{><|\s])',
+             Number),
+            (r'(?<=[.\\;,#"\]\[)(}{><|\s])(recOR|recBOT|idJ|refl|first|second|π₁|π₂|unit)((?=$|[.\\;,#"\]\[)(}{><|\s])|(?=_{))',
+             String),
             (r'(?<=[.\\;,#"\]\[)(}{><|\s])as(?=$|[.\\;,#"\]\[)(}{><|\s])',
-             Keyword),
+             Keyword.Reserved),
 
             # parameters
             (r'(\(\s*)([^{:\)]+\s*)(:)(?=$|[.\\;,#"\]\[)(}{><|\s])',
-             bygroups(Punctuation, Name.Variable, Punctuation)),
+             bygroups(Punctuation, Text, Punctuation)),
 
             (r'"', String, 'string'),
 
-            (r'(\\\s*)((([^\t\n\r !"#\(\),-\.;:\\\/=<>\?\[\\\]\{\|\}][^\t\n\r !"#\(\),\.;:<>\?\[\\\]\{\|\}]*)\s*)+)',
-                bygroups(Punctuation, Name.Variable)),
+            (r'(\\\s*)((([^→\t\n\r !"#\(\),-\.;:\\\/=<>\?\[\\\]\{\|\}][^\t\n\r !"#\(\),\.;:<>\?\[\\\]\{\|\}]*)\s*)+)',
+                bygroups(Punctuation, Text)),
         ],
         'string': [
             (r'[^"]+', String),
             (r'"', String, '#pop'),
         ],
     }
```

### Comparing `pygments-rzk-0.1.2/pygments_rzk.egg-info/PKG-INFO` & `pygments-rzk-0.1.3/pygments_rzk.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pygments-rzk
-Version: 0.1.2
+Version: 0.1.3
 Summary: Pygments lexer for Rzk language (of proof assistant for synthetic ∞-categories).
-Home-page: https://github.com/fizruk/pygments-rzk
+Home-page: https://github.com/rzk-lang/pygments-rzk
 Author: Nikolai Kudasov
 Author-email: nickolay.kudasov@gmail.com
 License: BSD 3
 Keywords: pygments rzk lexer
 Classifier: Environment :: Plugins
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -14,24 +14,24 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Pygments higlighter for Rzk
 
-This is a simple [Pygments](https://pygments.org) higlighter for [Rzk](https://github.com/fizruk/rzk), which can be used with [`minted` package](https://www.ctan.org/pkg/minted) when writing rzk code in LaTeX or with [MkDocs](https://www.mkdocs.org) to highlight code in blocks when rendering literate Rzk Markdown files.
+This is a simple [Pygments](https://pygments.org) higlighter for [Rzk](https://github.com/rzk-lang/rzk), which can be used with [`minted` package](https://www.ctan.org/pkg/minted) when writing rzk code in LaTeX or with [MkDocs](https://www.mkdocs.org) to highlight code in blocks when rendering literate Rzk Markdown files.
 
 ## How to use
 
 ### Install
 
 Clone this repository, and install the highlighter using [`pip` installer](https://pip.pypa.io/en/stable/):
 
 ```sh
-git clone https://github.com/fizruk/pygments-rzk.git
+git clone https://github.com/rzk-lang/pygments-rzk.git
 cd pygments-rzk   # enter repository root
 pip install .     # install using pip
 ```
 
 ### Use in MkDocs
 
 To be done.
@@ -66,15 +66,15 @@
 -- path reversal
 #define rev uses (A x y)
   (p : x = y)       -- A path from x to y in A.
   : y = x           -- The reversal will be defined by path induction on p.
   := idJ(A, x, \y' p' -> y' = x, refl, y, p)
 
 -- path composition by induction on the second path
-#define concat 
+#define concat
   (p : x = y)       -- A path from x to y in A.
   (q : y = z)       -- A path from y to z in A.
   : (x = z)
   := idJ(A, y, \z' q' -> (x = z'), p, z, q)
 
 #end path-algebra
 \end{minted}
```

### Comparing `pygments-rzk-0.1.2/setup.py` & `pygments-rzk-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #!/usr/bin/python
 
 from setuptools import setup, find_packages
 
 setup(
     name='pygments-rzk',
-    version='0.1.2',
+    version='0.1.3',
     description='Pygments lexer for Rzk language (of proof assistant for synthetic ∞-categories).',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     keywords='pygments rzk lexer',
     license='BSD 3',
 
     author='Nikolai Kudasov',
     author_email='nickolay.kudasov@gmail.com',
 
-    url='https://github.com/fizruk/pygments-rzk',
+    url='https://github.com/rzk-lang/pygments-rzk',
 
     packages=find_packages(),
     install_requires=['pygments >= 1.4'],
 
     entry_points='''[pygments.lexers]
                     rzklexer=pygments_rzk:RzkLexer''',
```

