# Comparing `tmp/to_tmx-1.0.1.tar.gz` & `tmp/to_tmx-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\to_tmx-1.0.1.tar", last modified: Wed Aug  5 13:32:01 2020, max compression
+gzip compressed data, was "/Users/alexskrn/Documents/NLP/to_tmx/dist/tmp8tsv29ex/to_tmx-1.0.2.tar", last modified: Tue Jul 11 17:42:26 2023, max compression
```

## Comparing `to_tmx-1.0.1.tar` & `to_tmx-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2020-08-05 13:32:01.000000 to_tmx-1.0.1/
--rw-rw-rw-   0        0        0     1086 2020-08-04 15:35:16.000000 to_tmx-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      142 2020-08-04 15:39:34.000000 to_tmx-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4650 2020-08-05 13:32:01.000000 to_tmx-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       69 2020-06-21 22:04:14.000000 to_tmx-1.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2020-08-05 13:32:01.000000 to_tmx-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1694 2020-08-05 13:30:28.000000 to_tmx-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2020-08-05 13:32:01.000000 to_tmx-1.0.1/to_tmx/
--rw-rw-rw-   0        0        0     1550 2020-08-04 18:02:01.000000 to_tmx-1.0.1/to_tmx/sent_tok.py
--rw-rw-rw-   0        0        0     2598 2020-08-04 18:01:18.000000 to_tmx-1.0.1/to_tmx/tmx_batch_tradosizer.py
--rw-rw-rw-   0        0        0     4022 2020-08-04 17:58:46.000000 to_tmx-1.0.1/to_tmx/tmx_tradosizer.py
--rw-rw-rw-   0        0        0     4772 2020-08-04 17:54:26.000000 to_tmx-1.0.1/to_tmx/to_tmx.py
--rw-rw-rw-   0        0        0        0 2020-06-21 20:06:37.000000 to_tmx-1.0.1/to_tmx/__init__.py
-drwxrwxrwx   0        0        0        0 2020-08-05 13:32:01.000000 to_tmx-1.0.1/to_tmx.egg-info/
--rw-rw-rw-   0        0        0        1 2020-08-05 13:32:00.000000 to_tmx-1.0.1/to_tmx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      183 2020-08-05 13:32:00.000000 to_tmx-1.0.1/to_tmx.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0     4650 2020-08-05 13:32:00.000000 to_tmx-1.0.1/to_tmx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       64 2020-08-05 13:32:00.000000 to_tmx-1.0.1/to_tmx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      342 2020-08-05 13:32:01.000000 to_tmx-1.0.1/to_tmx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2020-08-05 13:32:00.000000 to_tmx-1.0.1/to_tmx.egg-info/top_level.txt
+drwxr-xr-x   0 alexskrn   (502) staff       (20)        0 2023-07-11 17:42:26.000000 to_tmx-1.0.2/
+-rw-r--r--   0 alexskrn   (502) staff       (20)     4066 2023-07-11 17:42:26.000000 to_tmx-1.0.2/PKG-INFO
+-rw-r--r--   0 alexskrn   (502) staff       (20)       65 2020-07-10 16:28:04.000000 to_tmx-1.0.2/requirements.txt
+-rw-r--r--   0 alexskrn   (502) staff       (20)      135 2023-07-11 17:13:12.000000 to_tmx-1.0.2/MANIFEST.in
+drwxr-xr-x   0 alexskrn   (502) staff       (20)        0 2023-07-11 17:42:26.000000 to_tmx-1.0.2/to_tmx.egg-info/
+-rw-r--r--   0 alexskrn   (502) staff       (20)     4066 2023-07-11 17:42:26.000000 to_tmx-1.0.2/to_tmx.egg-info/PKG-INFO
+-rw-r--r--   0 alexskrn   (502) staff       (20)      342 2023-07-11 17:42:26.000000 to_tmx-1.0.2/to_tmx.egg-info/SOURCES.txt
+-rw-r--r--   0 alexskrn   (502) staff       (20)      183 2023-07-11 17:42:26.000000 to_tmx-1.0.2/to_tmx.egg-info/entry_points.txt
+-rw-r--r--   0 alexskrn   (502) staff       (20)       64 2023-07-11 17:42:26.000000 to_tmx-1.0.2/to_tmx.egg-info/requires.txt
+-rw-r--r--   0 alexskrn   (502) staff       (20)        7 2023-07-11 17:42:26.000000 to_tmx-1.0.2/to_tmx.egg-info/top_level.txt
+-rw-r--r--   0 alexskrn   (502) staff       (20)        1 2023-07-11 17:42:26.000000 to_tmx-1.0.2/to_tmx.egg-info/dependency_links.txt
+-rw-r--r--   0 alexskrn   (502) staff       (20)     1625 2023-07-11 17:23:08.000000 to_tmx-1.0.2/setup.py
+drwxr-xr-x   0 alexskrn   (502) staff       (20)        0 2023-07-11 17:42:26.000000 to_tmx-1.0.2/to_tmx/
+-rw-r--r--   0 alexskrn   (502) staff       (20)     2524 2023-07-11 17:13:12.000000 to_tmx-1.0.2/to_tmx/tmx_batch_tradosizer.py
+-rw-r--r--   0 alexskrn   (502) staff       (20)     4638 2023-07-11 17:13:12.000000 to_tmx-1.0.2/to_tmx/to_tmx.py
+-rw-r--r--   0 alexskrn   (502) staff       (20)     3890 2023-07-11 17:13:12.000000 to_tmx-1.0.2/to_tmx/tmx_tradosizer.py
+-rw-r--r--   0 alexskrn   (502) staff       (20)        0 2020-07-10 16:28:04.000000 to_tmx-1.0.2/to_tmx/__init__.py
+-rw-r--r--   0 alexskrn   (502) staff       (20)     1499 2020-07-10 16:28:04.000000 to_tmx-1.0.2/to_tmx/sent_tok.py
+-rw-r--r--   0 alexskrn   (502) staff       (20)       38 2023-07-11 17:42:26.000000 to_tmx-1.0.2/setup.cfg
+-rw-r--r--   0 alexskrn   (502) staff       (20)     1065 2023-07-11 17:13:12.000000 to_tmx-1.0.2/LICENSE.txt
```

### Comparing `to_tmx-1.0.1/PKG-INFO` & `to_tmx-1.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,80 +1,83 @@
-Metadata-Version: 2.1
-Name: to_tmx
-Version: 1.0.1
-Summary: Txt-to-tmx file converter.
-Home-page: https://github.com/AlexSkrn/to_tmx
-Author: AlexSkrn
-Author-email: alex.g.skrn@gmail.com
-License: MIT
-Description: 
-        # Пакет с несколькими скриптами для конвертации txt-файлов в tmx-файлы
-        
-        Эти скрипты позволяют токенизировать текстовые файлы на предложения, а затем
-        конвертировать получившиеся файлы в формат tmx (translation memory exchange,
-        по сути -- xml-файлы), в том числе в формат, понимаемый программой SDL Trados Studio 2017.
-        
-        ## Установка в Windows в терминале Anaconda Prompt
-        
-        ```
-        $ python -m venv .venv
-        $ .venv\Scripts\activate.bat  # в терминале Git Bash: source .venv/Scripts/activate
-        $ python -m pip install --upgrade pip
-        $ pip install to-tmx
-        $ python -m nltk.downloader punkt  # для токенизации на русском языке
-        ```
-        ## Внешние зависимости
-        
-        Пакет устанавливает NLTK. Кроме того, последняя строчка в разделе про установку
-        скачивает модели для токенизации на предложения из NLTK Corpora. Эта команда может
-        выдывать предупреждение при исполнении, но все равно работает.
-        
-        ## Использование
-        
-        Примеры исходных, промежуточных и финальных файлов лежат в репозитории проекта
-        на Гитхабе в папке ```data/```.
-        
-        ### Токенизация файлов на предложения
-        ```
-        $ sent-tok "path\file name.txt" language  # английский по умолчанию
-        ```
-        Например:
-        ```
-        $ sent-tok "data\Madrid System_eng.txt" english
-        $ sent-tok "data\Madrid System_rus.txt" russian
-        ```
-        На выходе получаем два токенизированных на предложения файла, ```Madrid System_eng.txt_sent_tok``` и ```Madrid System_rus.txt_sent_tok```.
-        
-        Их следует открыть в текстовом редакторе (Notepad++) и проверить, что все токенизировалось
-        правильно. Обычно ошибок хватает. Нужно, чтобы количество строк в обоих файлов стало одинаковым.
-        
-        ### Конвертация в tmx
-        ```
-        $ to-tmx "path\file name_eng.txt_sent_tok" "path\file name_rus.txt_sent_tok"
-        ```
-        Например:
-        ```
-        $ to-tmx "data\Madrid System_eng.txt_sent_tok" "data\Madrid System_rus.txt_sent_tok"
-        ```
-        Скрипт создаст файл ```"data\Madrid System_eng-Madrid System_rus.tmx"```.
-        
-        ### Конвертация в tmx, понимаемый программой SDL Trados Studio 2017
-        ```
-        $ tmx-tradosize "path\file name_eng-file name_rus.tmx "path\file_name_trados_style.tmx"
-        ```
-        Первый аргумент -- исходный tmx-файл (полученный на предыдущем этапе), второй аргумент -- путь и желаемое название выходящего файла. Например:
-        ```
-        $ tmx-tradosize "data\Madrid System_eng-Madrid System_rus.tmx" "data\madrid_system_trados_style.tmx"
-        ```
-        
-        ### Конвертация многих файлов в tmx-файлы, понимаемые программой SDL Trados Studio 2017
-        
-        Команда ```tmx-batch-tradosize``` попросит выбрать папку с несколькими tmx-файлами,
-        а результат сохранит в папку ```tmx-trados-style\```
-        
-Keywords: tmx converter
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6.0,<3.8.0
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: to_tmx
+Version: 1.0.2
+Summary: Txt-to-tmx file converter.
+Home-page: https://github.com/AlexSkrn/to_tmx
+Author: AlexSkrn
+Author-email: alex.g.skrn@gmail.com
+License: MIT
+Keywords: tmx converter
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6.0
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+
+# Пакет с несколькими скриптами для конвертации txt-файлов в tmx-файлы
+
+Эти скрипты позволяют токенизировать текстовые файлы на предложения, а затем
+конвертировать получившиеся файлы в формат tmx (translation memory exchange,
+по сути -- xml-файлы), в том числе в формат, понимаемый программой SDL Trados Studio 2017.
+
+## Установка в Windows в терминале Anaconda Prompt
+
+```
+$ python -m venv .venv
+$ .venv\Scripts\activate.bat  # в терминале Git Bash: source .venv/Scripts/activate
+$ python -m pip install --upgrade pip
+$ pip install to-tmx
+$ python -m nltk.downloader punkt  # для токенизации на русском языке
+```
+## Внешние зависимости
+
+Пакет устанавливает NLTK. Кроме того, последняя строчка в разделе про установку
+скачивает модели для токенизации на предложения из NLTK Corpora. Эта команда может
+выдывать предупреждение при исполнении, но все равно работает.
+
+## Использование
+
+Примеры исходных, промежуточных и финальных файлов лежат в репозитории проекта
+на Гитхабе в папке ```data/```.
+
+### Токенизация файлов на предложения
+```
+$ sent-tok "path\file name.txt" language  # английский по умолчанию
+```
+Например:
+```
+$ sent-tok "data\Madrid System_eng.txt" english
+$ sent-tok "data\Madrid System_rus.txt" russian
+```
+На выходе получаем два токенизированных на предложения файла, ```Madrid System_eng.txt_sent_tok``` и ```Madrid System_rus.txt_sent_tok```.
+
+Их следует открыть в текстовом редакторе (Notepad++) и проверить, что все токенизировалось
+правильно. Обычно ошибок хватает. Нужно, чтобы количество строк в обоих файлов стало одинаковым.
+
+### Конвертация в tmx
+```
+$ to-tmx "path\file name_eng.txt_sent_tok" "path\file name_rus.txt_sent_tok"
+```
+Например:
+```
+$ to-tmx "data\Madrid System_eng.txt_sent_tok" "data\Madrid System_rus.txt_sent_tok"
+```
+Скрипт создаст файл ```"data\Madrid System_eng-Madrid System_rus.tmx"```.
+
+### Конвертация в tmx, понимаемый программой SDL Trados Studio 2017
+```
+$ tmx-tradosize "path\file name_eng-file name_rus.tmx "path\file_name_trados_style.tmx"
+```
+Первый аргумент -- исходный tmx-файл (полученный на предыдущем этапе), второй аргумент -- путь и желаемое название выходящего файла. Например:
+```
+$ tmx-tradosize "data\Madrid System_eng-Madrid System_rus.tmx" "data\madrid_system_trados_style.tmx"
+```
+
+### Конвертация многих файлов в tmx-файлы, понимаемые программой SDL Trados Studio 2017
+
+Команда ```tmx-batch-tradosize``` попросит выбрать папку с несколькими tmx-файлами,
+а результат сохранит в папку ```tmx-trados-style\```
+
+
```

### Comparing `to_tmx-1.0.1/setup.py` & `to_tmx-1.0.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-import io
-import os
-
-import setuptools
-
-
-# Package meta-data.
-NAME = 'to_tmx'
-DESCRIPTION = 'Txt-to-tmx file converter.'
-URL = 'https://github.com/AlexSkrn/to_tmx'
-EMAIL = 'alex.g.skrn@gmail.com'
-AUTHOR = 'AlexSkrn'
-REQUIRES_PYTHON = '>=3.6.0,<3.8.0'
-
-
-def list_reqs(fname='requirements.txt'):
-    """Return a list of packages required for this module to be executed."""
-    with open(fname) as fd:
-        return fd.read().splitlines()
-
-
-here = os.path.abspath(os.path.dirname(__file__))
-
-# Import the README and use it as the long-description.
-try:
-    with io.open(os.path.join(here, 'readme.md'), encoding='utf-8') as f:
-        long_description = '\n' + f.read()
-except FileNotFoundError:
-    long_description = DESCRIPTION
-
-
-setuptools.setup(
-    name=NAME,
-    version='1.0.1',
-    description=DESCRIPTION,
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    author=AUTHOR,
-    author_email=EMAIL,
-    python_requires=REQUIRES_PYTHON,
-    url=URL,
-    packages=setuptools.find_packages(exclude=('tests',)),
-    install_requires=list_reqs(),
-    license='MIT',
-    classifiers=[
-        'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3'
-    ],
-    keywords='tmx converter',
-    entry_points={
-        'console_scripts': [
-            'sent-tok=to_tmx.sent_tok:main',
-            'to-tmx=to_tmx.to_tmx:main',
-            'tmx-tradosize=to_tmx.tmx_tradosizer:main',
-            'tmx-batch-tradosize=to_tmx.tmx_batch_tradosizer:ProcessTMX'
-        ],
-    },
-)
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+import io
+import os
+
+import setuptools
+
+
+# Package meta-data.
+NAME = 'to_tmx'
+DESCRIPTION = 'Txt-to-tmx file converter.'
+URL = 'https://github.com/AlexSkrn/to_tmx'
+EMAIL = 'alex.g.skrn@gmail.com'
+AUTHOR = 'AlexSkrn'
+REQUIRES_PYTHON = '>=3.6.0'
+
+
+def list_reqs(fname='requirements.txt'):
+    """Return a list of packages required for this module to be executed."""
+    with open(fname) as fd:
+        return fd.read().splitlines()
+
+
+here = os.path.abspath(os.path.dirname(__file__))
+
+# Import the README and use it as the long-description.
+try:
+    with io.open(os.path.join(here, 'readme.md'), encoding='utf-8') as f:
+        long_description = '\n' + f.read()
+except FileNotFoundError:
+    long_description = DESCRIPTION
+
+
+setuptools.setup(
+    name=NAME,
+    version='1.0.2',
+    description=DESCRIPTION,
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    author=AUTHOR,
+    author_email=EMAIL,
+    python_requires=REQUIRES_PYTHON,
+    url=URL,
+    packages=setuptools.find_packages(exclude=('tests',)),
+    install_requires=list_reqs(),
+    license='MIT',
+    classifiers=[
+        'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 3'
+    ],
+    keywords='tmx converter',
+    entry_points={
+        'console_scripts': [
+            'sent-tok=to_tmx.sent_tok:main',
+            'to-tmx=to_tmx.to_tmx:main',
+            'tmx-tradosize=to_tmx.tmx_tradosizer:main',
+            'tmx-batch-tradosize=to_tmx.tmx_batch_tradosizer:ProcessTMX'
+        ],
+    },
+)
```

### Comparing `to_tmx-1.0.1/to_tmx/sent_tok.py` & `to_tmx-1.0.2/to_tmx/sent_tok.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-#!/usr/bin/env python3
-"""This script tokenizes an input file into sentences.
-
-The sentences are written one sentence per line to file name <orig>_sent_tok.
-"""
-
-# import os
-import argparse
-import re
-from nltk.tokenize import sent_tokenize
-
-
-def sent_tok(filename, language):
-    """Return a list of sentencies."""
-    with open(filename, 'r', encoding='utf8') as fromF:
-        text = fromF.read()
-        sentences = []
-        # Split into paragraphs and tokenize
-        for para in re.split('\ufeff|\n|\r', text):
-            if para:
-                sentences.extend(sent_tokenize(para, language=language))
-    return sentences
-
-
-def write_to_file(sentences, filename):
-    """Write sentences to filename and return None."""
-    with open(filename + '_sent_tok', 'w', encoding='utf8') as toF:
-        for sent in sentences:
-            toF.write('{}\n'.format(sent))
-    return None
-
-
-def main():
-    """Run the script."""
-    parser = argparse.ArgumentParser()
-    parser.add_argument('path',
-                        help='Provide file name to tokenize into sentences')
-    parser.add_argument('lang', nargs='?', default='english',
-                        help='Specify language if not English')
-    args = parser.parse_args()
-
-    filename = args.path  # file name to process
-    # head, tail = os.path.split(filename)
-    lang = args.lang  # Tokenizer language
-
-    sentence_list = sent_tok(filename, lang)
-    write_to_file(sentence_list, filename)
-
-
-if __name__ == '__main__':
-    main()
+#!/usr/bin/env python3
+"""This script tokenizes an input file into sentences.
+
+The sentences are written one sentence per line to file name <orig>_sent_tok.
+"""
+
+# import os
+import argparse
+import re
+from nltk.tokenize import sent_tokenize
+
+
+def sent_tok(filename, language):
+    """Return a list of sentencies."""
+    with open(filename, 'r', encoding='utf8') as fromF:
+        text = fromF.read()
+        sentences = []
+        # Split into paragraphs and tokenize
+        for para in re.split('\ufeff|\n|\r', text):
+            if para:
+                sentences.extend(sent_tokenize(para, language=language))
+    return sentences
+
+
+def write_to_file(sentences, filename):
+    """Write sentences to filename and return None."""
+    with open(filename + '_sent_tok', 'w', encoding='utf8') as toF:
+        for sent in sentences:
+            toF.write('{}\n'.format(sent))
+    return None
+
+
+def main():
+    """Run the script."""
+    parser = argparse.ArgumentParser()
+    parser.add_argument('path',
+                        help='Provide file name to tokenize into sentences')
+    parser.add_argument('lang', nargs='?', default='english',
+                        help='Specify language if not English')
+    args = parser.parse_args()
+
+    filename = args.path  # file name to process
+    # head, tail = os.path.split(filename)
+    lang = args.lang  # Tokenizer language
+
+    sentence_list = sent_tok(filename, lang)
+    write_to_file(sentence_list, filename)
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `to_tmx-1.0.1/to_tmx/tmx_batch_tradosizer.py` & `to_tmx-1.0.2/to_tmx/tmx_batch_tradosizer.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,74 +1,74 @@
-#!/usr/bin/env python3
-"""This script applies tmx_tradosizer.py to a folder with several tmx files.
-
-It saves results in folder tmx-trados-style/.
-
-The effect of running this script on a directory containing tmx files is that
-the name of each tmx files becomes an attribute of each <tu> element so that
-when I import such tmx files into Trados Studio's TM, each imported segment
-has a property whose value is the name of the tmx file from which that
-segment originated.
-"""
-
-import os
-import sys
-import tkinter as tk
-from tkinter import filedialog
-
-from to_tmx import tmx_tradosizer
-
-
-class ProcessTMX:
-
-    def __init__(self):
-        """
-            self.inputdir: path returned by dialog window
-                        (and where TMX files to be processed are)
-            self.outputpath: where output files will be written
-            self.tmx_files: list of tmx files to be processes
-        """
-        self.inputdir = ''
-        self.outputpath = ''
-        self.tmx_files = []
-
-        self.select_directory()
-        if self.inputdir:
-            print('Reading files in:', self.inputdir)
-            self.make_output_dir()
-        if self.tmx_files:
-            print('# of tmx files identified:', len(self.tmx_files))
-            self.process_tmx_files()
-
-    def select_directory(self):
-        """Select the directory where the TMX files to be processed are."""
-        root = tk.Tk()
-        root.withdraw()
-        result = filedialog.askdirectory()
-        if result:
-            self.inputdir = result
-
-    def make_output_dir(self):
-        """Create a dir for output files."""
-        file_names = os.listdir(self.inputdir)
-        self.tmx_files = [f for f in file_names if f.endswith('.tmx')]
-        if self.tmx_files:
-            self.outputpath = os.path.join(self.inputdir, 'tmx-trados-style/')
-            print('Created output dir:', self.outputpath)
-            if not os.path.exists(self.outputpath):
-                try:
-                    os.mkdir(self.outputpath)
-                except Exception as e:
-                    print("The program can't create the directory")
-                    print(e)
-                    sys.exit()
-
-    def process_tmx_files(self):
-        """Process tmx files by applying Trados style fields."""
-        for f in self.tmx_files:
-            tmx_tradosizer.create_tmx(os.path.join(self.inputdir, f),
-                                      os.path.join(self.outputpath, f)
-                                      )
-
-
-if __name__ == '__main__':
-    ProcessTMX()
+#!/usr/bin/env python3
+"""This script applies tmx_tradosizer.py to a folder with several tmx files.
+
+It saves results in folder tmx-trados-style/.
+
+The effect of running this script on a directory containing tmx files is that
+the name of each tmx files becomes an attribute of each <tu> element so that
+when I import such tmx files into Trados Studio's TM, each imported segment
+has a property whose value is the name of the tmx file from which that
+segment originated.
+"""
+
+import os
+import sys
+import tkinter as tk
+from tkinter import filedialog
+
+from to_tmx import tmx_tradosizer
+
+
+class ProcessTMX:
+
+    def __init__(self):
+        """
+            self.inputdir: path returned by dialog window
+                        (and where TMX files to be processed are)
+            self.outputpath: where output files will be written
+            self.tmx_files: list of tmx files to be processes
+        """
+        self.inputdir = ''
+        self.outputpath = ''
+        self.tmx_files = []
+
+        self.select_directory()
+        if self.inputdir:
+            print('Reading files in:', self.inputdir)
+            self.make_output_dir()
+        if self.tmx_files:
+            print('# of tmx files identified:', len(self.tmx_files))
+            self.process_tmx_files()
+
+    def select_directory(self):
+        """Select the directory where the TMX files to be processed are."""
+        root = tk.Tk()
+        root.withdraw()
+        result = filedialog.askdirectory()
+        if result:
+            self.inputdir = result
+
+    def make_output_dir(self):
+        """Create a dir for output files."""
+        file_names = os.listdir(self.inputdir)
+        self.tmx_files = [f for f in file_names if f.endswith('.tmx')]
+        if self.tmx_files:
+            self.outputpath = os.path.join(self.inputdir, 'tmx-trados-style/')
+            print('Created output dir:', self.outputpath)
+            if not os.path.exists(self.outputpath):
+                try:
+                    os.mkdir(self.outputpath)
+                except Exception as e:
+                    print("The program can't create the directory")
+                    print(e)
+                    sys.exit()
+
+    def process_tmx_files(self):
+        """Process tmx files by applying Trados style fields."""
+        for f in self.tmx_files:
+            tmx_tradosizer.create_tmx(os.path.join(self.inputdir, f),
+                                      os.path.join(self.outputpath, f)
+                                      )
+
+
+if __name__ == '__main__':
+    ProcessTMX()
```

### Comparing `to_tmx-1.0.1/to_tmx/to_tmx.py` & `to_tmx-1.0.2/to_tmx/to_tmx.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,134 +1,134 @@
-#!/usr/bin/env python3
-"""This script converts two text files into one tmx file, with
-EN-US and RU-RU language codes.
-
-The files must have equal number of lines, with one sentence per line.
-
-The resulting tmx files have been checked for compatibility with Heartsome
-and Olifant tmx editors.
-"""
-
-import os
-import argparse
-import xml.etree.ElementTree as ET
-
-
-def build_tree(root, *args):
-    """Build a tree structure."""
-    body = ET.SubElement(root, "body")
-    if len(args) == 2:
-        file1, file2 = args
-        with open(file1, 'r', encoding='utf8') as f1, open(file2, 'r', encoding='utf8') as f2:
-            for src, trg in zip(f1, f2):
-                src = src.strip()
-                trg = trg.strip()
-                if src != trg:
-                    tu = ET.SubElement(body, "tu")
-
-                    tuv = ET.SubElement(tu,
-                                        "tuv",
-                                        attrib={'xml:lang': 'EN-US'}
-                                        )
-                    seg = ET.SubElement(tuv, "seg")
-                    seg.text = src
-
-                    tuv = ET.SubElement(tu,
-                                        "tuv",
-                                        attrib={'xml:lang': 'RU-RU'}
-                                        )
-                    seg = ET.SubElement(tuv, "seg")
-                    seg.text = trg
-    elif len(args) == 1:
-        file1 = args[0]
-        with open(file1, 'r', encoding='utf8') as f1:
-            for line in f1:
-                src, trg = line.split('\t')
-                src = src.strip()
-                trg = trg.strip()
-                if src != trg:
-                    tu = ET.SubElement(body, "tu")
-
-                    tuv = ET.SubElement(tu,
-                                        "tuv",
-                                        attrib={'xml:lang': 'EN-US'}
-                                        )
-                    seg = ET.SubElement(tuv, "seg")
-                    seg.text = src
-
-                    tuv = ET.SubElement(tu,
-                                        "tuv",
-                                        attrib={'xml:lang': 'RU-RU'}
-                                        )
-                    seg = ET.SubElement(tuv, "seg")
-                    seg.text = trg
-
-    # wrap it in an ElementTree instance
-    tree = ET.ElementTree(root)
-    return tree
-
-
-def indent(elem, level=0):
-    """Create indentation for tree elements."""
-    i = "\n" + level*"  "
-    if len(elem):
-        if not elem.text or not elem.text.strip():
-            elem.text = i + "  "
-        if not elem.tail or not elem.tail.strip():
-            elem.tail = i
-        for elem in elem:
-            indent(elem, level+1)
-        if not elem.tail or not elem.tail.strip():
-            elem.tail = i
-    else:
-        if level and (not elem.tail or not elem.tail.strip()):
-            elem.tail = i
-
-
-def build_trg_file_name(*args):
-    """Return the target file name."""
-    if len(args) == 2:
-        file1, file2 = args
-        head, tail1 = os.path.split(file1)
-        _, tail2 = os.path.split(file2)
-        target_file_name = '{}-{}.tmx'.format(os.path.splitext(tail1)[0],
-                                              os.path.splitext(tail2)[0])
-    elif len(args) == 1:
-        file_name = args[0]  # You get a tuple without [0]
-        head, tail = os.path.split(file_name)
-        target_file_name = '{}.tmx'.format(os.path.splitext(tail)[0])
-
-    return head, target_file_name
-
-
-def create_tmx(*args):
-    """Create the tmx file."""
-    root = ET.Element('tmx', attrib={'version': '1.4'})
-    ET.SubElement(root, 'header', attrib={'srclang': 'EN-US'})
-    tree = build_tree(root, *args)
-    indent(root)
-    # Save as tmx
-    head, target_file_name = build_trg_file_name(*args)
-    dsn = os.path.join(head, target_file_name)
-    tree.write(dsn, encoding='UTF-8', xml_declaration=True)
-
-
-def main():
-    """Run the script."""
-    description = """Text-to-tmx converter. Accepts one tab-delim source file
-    (format: 'english text \\t russian text')
-    or two source files: English.txt, Russian.txt. Texts must be
-    sentence tokenized before passing them to this script."""
-    parser = argparse.ArgumentParser(description=description)
-    parser.add_argument('source', nargs='*',
-                        help='Provide one or two file names, english first')
-    args = parser.parse_args()
-    if len(args.source) == 2:
-        create_tmx(*args.source)
-    elif len(args.source) == 1:
-        create_tmx(*args.source)
-    else:
-        print('Wrong number of arguments, use -h flag for help')
-
-
-if __name__ == '__main__':
-    main()
+#!/usr/bin/env python3
+"""This script converts two text files into one tmx file, with
+EN-US and RU-RU language codes.
+
+The files must have equal number of lines, with one sentence per line.
+
+The resulting tmx files have been checked for compatibility with Heartsome
+and Olifant tmx editors.
+"""
+
+import os
+import argparse
+import xml.etree.ElementTree as ET
+
+
+def build_tree(root, *args):
+    """Build a tree structure."""
+    body = ET.SubElement(root, "body")
+    if len(args) == 2:
+        file1, file2 = args
+        with open(file1, 'r', encoding='utf8') as f1, open(file2, 'r', encoding='utf8') as f2:
+            for src, trg in zip(f1, f2):
+                src = src.strip()
+                trg = trg.strip()
+                if src != trg:
+                    tu = ET.SubElement(body, "tu")
+
+                    tuv = ET.SubElement(tu,
+                                        "tuv",
+                                        attrib={'xml:lang': 'EN-US'}
+                                        )
+                    seg = ET.SubElement(tuv, "seg")
+                    seg.text = src
+
+                    tuv = ET.SubElement(tu,
+                                        "tuv",
+                                        attrib={'xml:lang': 'RU-RU'}
+                                        )
+                    seg = ET.SubElement(tuv, "seg")
+                    seg.text = trg
+    elif len(args) == 1:
+        file1 = args[0]
+        with open(file1, 'r', encoding='utf8') as f1:
+            for line in f1:
+                src, trg = line.split('\t')
+                src = src.strip()
+                trg = trg.strip()
+                if src != trg:
+                    tu = ET.SubElement(body, "tu")
+
+                    tuv = ET.SubElement(tu,
+                                        "tuv",
+                                        attrib={'xml:lang': 'EN-US'}
+                                        )
+                    seg = ET.SubElement(tuv, "seg")
+                    seg.text = src
+
+                    tuv = ET.SubElement(tu,
+                                        "tuv",
+                                        attrib={'xml:lang': 'RU-RU'}
+                                        )
+                    seg = ET.SubElement(tuv, "seg")
+                    seg.text = trg
+
+    # wrap it in an ElementTree instance
+    tree = ET.ElementTree(root)
+    return tree
+
+
+def indent(elem, level=0):
+    """Create indentation for tree elements."""
+    i = "\n" + level*"  "
+    if len(elem):
+        if not elem.text or not elem.text.strip():
+            elem.text = i + "  "
+        if not elem.tail or not elem.tail.strip():
+            elem.tail = i
+        for elem in elem:
+            indent(elem, level+1)
+        if not elem.tail or not elem.tail.strip():
+            elem.tail = i
+    else:
+        if level and (not elem.tail or not elem.tail.strip()):
+            elem.tail = i
+
+
+def build_trg_file_name(*args):
+    """Return the target file name."""
+    if len(args) == 2:
+        file1, file2 = args
+        head, tail1 = os.path.split(file1)
+        _, tail2 = os.path.split(file2)
+        target_file_name = '{}-{}.tmx'.format(os.path.splitext(tail1)[0],
+                                              os.path.splitext(tail2)[0])
+    elif len(args) == 1:
+        file_name = args[0]  # You get a tuple without [0]
+        head, tail = os.path.split(file_name)
+        target_file_name = '{}.tmx'.format(os.path.splitext(tail)[0])
+
+    return head, target_file_name
+
+
+def create_tmx(*args):
+    """Create the tmx file."""
+    root = ET.Element('tmx', attrib={'version': '1.4'})
+    ET.SubElement(root, 'header', attrib={'srclang': 'EN-US'})
+    tree = build_tree(root, *args)
+    indent(root)
+    # Save as tmx
+    head, target_file_name = build_trg_file_name(*args)
+    dsn = os.path.join(head, target_file_name)
+    tree.write(dsn, encoding='UTF-8', xml_declaration=True)
+
+
+def main():
+    """Run the script."""
+    description = """Text-to-tmx converter. Accepts one tab-delim source file
+    (format: 'english text \\t russian text')
+    or two source files: English.txt, Russian.txt. Texts must be
+    sentence tokenized before passing them to this script."""
+    parser = argparse.ArgumentParser(description=description)
+    parser.add_argument('source', nargs='*',
+                        help='Provide one or two file names, english first')
+    args = parser.parse_args()
+    if len(args.source) == 2:
+        create_tmx(*args.source)
+    elif len(args.source) == 1:
+        create_tmx(*args.source)
+    else:
+        print('Wrong number of arguments, use -h flag for help')
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `to_tmx-1.0.1/to_tmx.egg-info/PKG-INFO` & `to_tmx-1.0.2/to_tmx.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,80 +1,83 @@
-Metadata-Version: 2.1
-Name: to-tmx
-Version: 1.0.1
-Summary: Txt-to-tmx file converter.
-Home-page: https://github.com/AlexSkrn/to_tmx
-Author: AlexSkrn
-Author-email: alex.g.skrn@gmail.com
-License: MIT
-Description: 
-        # Пакет с несколькими скриптами для конвертации txt-файлов в tmx-файлы
-        
-        Эти скрипты позволяют токенизировать текстовые файлы на предложения, а затем
-        конвертировать получившиеся файлы в формат tmx (translation memory exchange,
-        по сути -- xml-файлы), в том числе в формат, понимаемый программой SDL Trados Studio 2017.
-        
-        ## Установка в Windows в терминале Anaconda Prompt
-        
-        ```
-        $ python -m venv .venv
-        $ .venv\Scripts\activate.bat  # в терминале Git Bash: source .venv/Scripts/activate
-        $ python -m pip install --upgrade pip
-        $ pip install to-tmx
-        $ python -m nltk.downloader punkt  # для токенизации на русском языке
-        ```
-        ## Внешние зависимости
-        
-        Пакет устанавливает NLTK. Кроме того, последняя строчка в разделе про установку
-        скачивает модели для токенизации на предложения из NLTK Corpora. Эта команда может
-        выдывать предупреждение при исполнении, но все равно работает.
-        
-        ## Использование
-        
-        Примеры исходных, промежуточных и финальных файлов лежат в репозитории проекта
-        на Гитхабе в папке ```data/```.
-        
-        ### Токенизация файлов на предложения
-        ```
-        $ sent-tok "path\file name.txt" language  # английский по умолчанию
-        ```
-        Например:
-        ```
-        $ sent-tok "data\Madrid System_eng.txt" english
-        $ sent-tok "data\Madrid System_rus.txt" russian
-        ```
-        На выходе получаем два токенизированных на предложения файла, ```Madrid System_eng.txt_sent_tok``` и ```Madrid System_rus.txt_sent_tok```.
-        
-        Их следует открыть в текстовом редакторе (Notepad++) и проверить, что все токенизировалось
-        правильно. Обычно ошибок хватает. Нужно, чтобы количество строк в обоих файлов стало одинаковым.
-        
-        ### Конвертация в tmx
-        ```
-        $ to-tmx "path\file name_eng.txt_sent_tok" "path\file name_rus.txt_sent_tok"
-        ```
-        Например:
-        ```
-        $ to-tmx "data\Madrid System_eng.txt_sent_tok" "data\Madrid System_rus.txt_sent_tok"
-        ```
-        Скрипт создаст файл ```"data\Madrid System_eng-Madrid System_rus.tmx"```.
-        
-        ### Конвертация в tmx, понимаемый программой SDL Trados Studio 2017
-        ```
-        $ tmx-tradosize "path\file name_eng-file name_rus.tmx "path\file_name_trados_style.tmx"
-        ```
-        Первый аргумент -- исходный tmx-файл (полученный на предыдущем этапе), второй аргумент -- путь и желаемое название выходящего файла. Например:
-        ```
-        $ tmx-tradosize "data\Madrid System_eng-Madrid System_rus.tmx" "data\madrid_system_trados_style.tmx"
-        ```
-        
-        ### Конвертация многих файлов в tmx-файлы, понимаемые программой SDL Trados Studio 2017
-        
-        Команда ```tmx-batch-tradosize``` попросит выбрать папку с несколькими tmx-файлами,
-        а результат сохранит в папку ```tmx-trados-style\```
-        
-Keywords: tmx converter
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6.0,<3.8.0
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: to-tmx
+Version: 1.0.2
+Summary: Txt-to-tmx file converter.
+Home-page: https://github.com/AlexSkrn/to_tmx
+Author: AlexSkrn
+Author-email: alex.g.skrn@gmail.com
+License: MIT
+Keywords: tmx converter
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6.0
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+
+# Пакет с несколькими скриптами для конвертации txt-файлов в tmx-файлы
+
+Эти скрипты позволяют токенизировать текстовые файлы на предложения, а затем
+конвертировать получившиеся файлы в формат tmx (translation memory exchange,
+по сути -- xml-файлы), в том числе в формат, понимаемый программой SDL Trados Studio 2017.
+
+## Установка в Windows в терминале Anaconda Prompt
+
+```
+$ python -m venv .venv
+$ .venv\Scripts\activate.bat  # в терминале Git Bash: source .venv/Scripts/activate
+$ python -m pip install --upgrade pip
+$ pip install to-tmx
+$ python -m nltk.downloader punkt  # для токенизации на русском языке
+```
+## Внешние зависимости
+
+Пакет устанавливает NLTK. Кроме того, последняя строчка в разделе про установку
+скачивает модели для токенизации на предложения из NLTK Corpora. Эта команда может
+выдывать предупреждение при исполнении, но все равно работает.
+
+## Использование
+
+Примеры исходных, промежуточных и финальных файлов лежат в репозитории проекта
+на Гитхабе в папке ```data/```.
+
+### Токенизация файлов на предложения
+```
+$ sent-tok "path\file name.txt" language  # английский по умолчанию
+```
+Например:
+```
+$ sent-tok "data\Madrid System_eng.txt" english
+$ sent-tok "data\Madrid System_rus.txt" russian
+```
+На выходе получаем два токенизированных на предложения файла, ```Madrid System_eng.txt_sent_tok``` и ```Madrid System_rus.txt_sent_tok```.
+
+Их следует открыть в текстовом редакторе (Notepad++) и проверить, что все токенизировалось
+правильно. Обычно ошибок хватает. Нужно, чтобы количество строк в обоих файлов стало одинаковым.
+
+### Конвертация в tmx
+```
+$ to-tmx "path\file name_eng.txt_sent_tok" "path\file name_rus.txt_sent_tok"
+```
+Например:
+```
+$ to-tmx "data\Madrid System_eng.txt_sent_tok" "data\Madrid System_rus.txt_sent_tok"
+```
+Скрипт создаст файл ```"data\Madrid System_eng-Madrid System_rus.tmx"```.
+
+### Конвертация в tmx, понимаемый программой SDL Trados Studio 2017
+```
+$ tmx-tradosize "path\file name_eng-file name_rus.tmx "path\file_name_trados_style.tmx"
+```
+Первый аргумент -- исходный tmx-файл (полученный на предыдущем этапе), второй аргумент -- путь и желаемое название выходящего файла. Например:
+```
+$ tmx-tradosize "data\Madrid System_eng-Madrid System_rus.tmx" "data\madrid_system_trados_style.tmx"
+```
+
+### Конвертация многих файлов в tmx-файлы, понимаемые программой SDL Trados Studio 2017
+
+Команда ```tmx-batch-tradosize``` попросит выбрать папку с несколькими tmx-файлами,
+а результат сохранит в папку ```tmx-trados-style\```
+
+
```

