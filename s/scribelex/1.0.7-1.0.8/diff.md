# Comparing `tmp/scribelex-1.0.7.tar.gz` & `tmp/scribelex-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scribelex-1.0.7.tar", last modified: Tue Jul 11 20:41:21 2023, max compression
+gzip compressed data, was "scribelex-1.0.8.tar", last modified: Tue Jul 11 20:55:45 2023, max compression
```

## Comparing `scribelex-1.0.7.tar` & `scribelex-1.0.8.tar`

### file list

```diff
@@ -1,11 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:41:21.418811 scribelex-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-11 20:41:17.000000 scribelex-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-11 20:41:21.418811 scribelex-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-11 20:41:17.000000 scribelex-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 20:41:21.418811 scribelex-1.0.7/scribelex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-11 20:41:21.000000 scribelex-1.0.7/scribelex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-11 20:41:21.000000 scribelex-1.0.7/scribelex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 20:41:21.000000 scribelex-1.0.7/scribelex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 20:41:21.000000 scribelex-1.0.7/scribelex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 20:41:21.418811 scribelex-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-11 20:41:17.000000 scribelex-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 20:55:45.170624 scribelex-1.0.8/
+-rw-rw-rw-   0        0        0     1086 2023-07-08 20:43:01.000000 scribelex-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0     1596 2023-07-11 20:55:45.169618 scribelex-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      608 2023-07-08 21:29:07.000000 scribelex-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 20:55:45.158306 scribelex-1.0.8/scribelex/
+-rw-rw-rw-   0        0        0       44 2023-07-11 20:35:48.000000 scribelex-1.0.8/scribelex/__init__.py
+-rw-rw-rw-   0        0        0     2768 2023-07-11 19:12:33.000000 scribelex-1.0.8/scribelex/base.py
+-rw-rw-rw-   0        0        0     1486 2023-07-11 20:35:12.000000 scribelex-1.0.8/scribelex/common.py
+drwxrwxrwx   0        0        0        0 2023-07-11 20:55:45.169618 scribelex-1.0.8/scribelex.egg-info/
+-rw-rw-rw-   0        0        0     1596 2023-07-11 20:55:45.000000 scribelex-1.0.8/scribelex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-07-11 20:55:45.000000 scribelex-1.0.8/scribelex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 20:55:45.000000 scribelex-1.0.8/scribelex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-11 20:55:45.000000 scribelex-1.0.8/scribelex.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 20:55:45.170624 scribelex-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1252 2023-07-11 20:55:40.000000 scribelex-1.0.8/setup.py
```

### Comparing `scribelex-1.0.7/PKG-INFO` & `scribelex-1.0.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-Metadata-Version: 2.1
-Name: scribelex
-Version: 1.0.7
-Summary: Scribelex is a lightweight Python library for building parser combinators.
-Home-page: https://github.com/UncleDrema/scribelex
-Author: UncleDrema
-Author-email: missl.wipiece@gmail.com
-License: MIT
-Keywords: parser,parsing,combinator,library,Python,structured data,grammar,syntax,parsing toolkit
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# scribelex
-scribelex - это легковесная библиотека на языке Python для реализации комбинаторов парсеров, позволяющая гибко преобразовывать данные между различными форматами.
-
-## Установка
-
-Вы можете установить scribelex с помощью pip:
-
-```bash
-pip install scribelex
-```
-
-## Лицензия
-
-Этот проект лицензирован под лицензией MIT.
-Подробнее смотрите файл [LICENSE](LICENSE).
+Metadata-Version: 2.1
+Name: scribelex
+Version: 1.0.8
+Summary: Scribelex is a lightweight Python library for building parser combinators.
+Home-page: https://github.com/UncleDrema/scribelex
+Author: UncleDrema
+Author-email: missl.wipiece@gmail.com
+License: MIT
+Keywords: parser,parsing,combinator,library,Python,structured data,grammar,syntax,parsing toolkit
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# scribelex
+scribelex - это легковесная библиотека на языке Python для реализации комбинаторов парсеров, позволяющая гибко преобразовывать данные между различными форматами.
+
+## Установка
+
+Вы можете установить scribelex с помощью pip:
+
+```bash
+pip install scribelex
+```
+
+## Лицензия
+
+Этот проект лицензирован под лицензией MIT.
+Подробнее смотрите файл [LICENSE](LICENSE).
```

### Comparing `scribelex-1.0.7/README.md` & `scribelex-1.0.8/README.md`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# scribelex
-scribelex - это легковесная библиотека на языке Python для реализации комбинаторов парсеров, позволяющая гибко преобразовывать данные между различными форматами.
-
-## Установка
-
-Вы можете установить scribelex с помощью pip:
-
-```bash
-pip install scribelex
-```
-
-## Лицензия
-
-Этот проект лицензирован под лицензией MIT.
+# scribelex
+scribelex - это легковесная библиотека на языке Python для реализации комбинаторов парсеров, позволяющая гибко преобразовывать данные между различными форматами.
+
+## Установка
+
+Вы можете установить scribelex с помощью pip:
+
+```bash
+pip install scribelex
+```
+
+## Лицензия
+
+Этот проект лицензирован под лицензией MIT.
 Подробнее смотрите файл [LICENSE](LICENSE).
```

### Comparing `scribelex-1.0.7/scribelex.egg-info/PKG-INFO` & `scribelex-1.0.8/scribelex.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-Metadata-Version: 2.1
-Name: scribelex
-Version: 1.0.7
-Summary: Scribelex is a lightweight Python library for building parser combinators.
-Home-page: https://github.com/UncleDrema/scribelex
-Author: UncleDrema
-Author-email: missl.wipiece@gmail.com
-License: MIT
-Keywords: parser,parsing,combinator,library,Python,structured data,grammar,syntax,parsing toolkit
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# scribelex
-scribelex - это легковесная библиотека на языке Python для реализации комбинаторов парсеров, позволяющая гибко преобразовывать данные между различными форматами.
-
-## Установка
-
-Вы можете установить scribelex с помощью pip:
-
-```bash
-pip install scribelex
-```
-
-## Лицензия
-
-Этот проект лицензирован под лицензией MIT.
-Подробнее смотрите файл [LICENSE](LICENSE).
+Metadata-Version: 2.1
+Name: scribelex
+Version: 1.0.8
+Summary: Scribelex is a lightweight Python library for building parser combinators.
+Home-page: https://github.com/UncleDrema/scribelex
+Author: UncleDrema
+Author-email: missl.wipiece@gmail.com
+License: MIT
+Keywords: parser,parsing,combinator,library,Python,structured data,grammar,syntax,parsing toolkit
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# scribelex
+scribelex - это легковесная библиотека на языке Python для реализации комбинаторов парсеров, позволяющая гибко преобразовывать данные между различными форматами.
+
+## Установка
+
+Вы можете установить scribelex с помощью pip:
+
+```bash
+pip install scribelex
+```
+
+## Лицензия
+
+Этот проект лицензирован под лицензией MIT.
+Подробнее смотрите файл [LICENSE](LICENSE).
```

### Comparing `scribelex-1.0.7/setup.py` & `scribelex-1.0.8/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-from setuptools import setup, find_packages
-
-with open("README.md", "r", encoding="utf-8") as fh:
-    long_description = fh.read()
-
-setup(
-    name="scribelex",
-    version="1.0.7",
-    author="UncleDrema",
-    author_email="missl.wipiece@gmail.com",
-    description="Scribelex is a lightweight Python library for building parser combinators.",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    keywords=["parser", "parsing", "combinator", "library", "Python", "structured data", "grammar", "syntax", "parsing toolkit"],
-    url="https://github.com/UncleDrema/scribelex",
-    packages=find_packages("scribelex"),
-    package_dir={"scribelex": "scribelex"},
-    license="MIT",
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-    ],
+from setuptools import setup, find_packages
+
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
+setup(
+    name="scribelex",
+    version="1.0.8",
+    author="UncleDrema",
+    author_email="missl.wipiece@gmail.com",
+    description="Scribelex is a lightweight Python library for building parser combinators.",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    keywords=["parser", "parsing", "combinator", "library", "Python", "structured data", "grammar", "syntax", "parsing toolkit"],
+    url="https://github.com/UncleDrema/scribelex",
+    packages=["scribelex"],
+    license="MIT",
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+    ],
 )
```

