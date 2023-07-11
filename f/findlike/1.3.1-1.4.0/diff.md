# Comparing `tmp/findlike-1.3.1.tar.gz` & `tmp/findlike-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findlike-1.3.1.tar", last modified: Sat Jul  1 01:05:21 2023, max compression
+gzip compressed data, was "findlike-1.4.0.tar", last modified: Tue Jul 11 01:56:20 2023, max compression
```

## Comparing `findlike-1.3.1.tar` & `findlike-1.4.0.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 soldeace  (1000) soldeace  (1000)        0 2023-07-01 01:05:21.616878 findlike-1.3.1/
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     1067 2023-06-27 14:06:31.000000 findlike-1.3.1/LICENSE
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)    11535 2023-07-01 01:05:21.616878 findlike-1.3.1/PKG-INFO
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)    10911 2023-06-29 21:00:15.000000 findlike-1.3.1/README.md
-drwxr-xr-x   0 soldeace  (1000) soldeace  (1000)        0 2023-07-01 01:05:21.616878 findlike-1.3.1/findlike/
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)        0 2022-12-31 23:26:30.000000 findlike-1.3.1/findlike/__init__.py
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)       59 2023-06-23 20:53:39.000000 findlike-1.3.1/findlike/__main__.py
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     5151 2023-07-01 00:35:57.000000 findlike-1.3.1/findlike/cli.py
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     3952 2023-07-01 00:02:10.000000 findlike-1.3.1/findlike/constants.py
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     4330 2023-06-28 17:12:04.000000 findlike-1.3.1/findlike/format.py
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     3586 2023-07-01 01:01:42.000000 findlike-1.3.1/findlike/preprocessing.py
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     1211 2023-07-01 00:00:21.000000 findlike-1.3.1/findlike/utils.py
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     2111 2023-07-01 00:49:44.000000 findlike-1.3.1/findlike/wrappers.py
-drwxr-xr-x   0 soldeace  (1000) soldeace  (1000)        0 2023-07-01 01:05:21.616878 findlike-1.3.1/findlike.egg-info/
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)    11535 2023-07-01 01:05:21.000000 findlike-1.3.1/findlike.egg-info/PKG-INFO
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)      474 2023-07-01 01:05:21.000000 findlike-1.3.1/findlike.egg-info/SOURCES.txt
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)        1 2023-07-01 01:05:21.000000 findlike-1.3.1/findlike.egg-info/dependency_links.txt
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)       46 2023-07-01 01:05:21.000000 findlike-1.3.1/findlike.egg-info/entry_points.txt
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)      186 2023-07-01 01:05:21.000000 findlike-1.3.1/findlike.egg-info/requires.txt
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)        9 2023-07-01 01:05:21.000000 findlike-1.3.1/findlike.egg-info/top_level.txt
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     1095 2023-07-01 01:04:44.000000 findlike-1.3.1/pyproject.toml
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)       38 2023-07-01 01:05:21.616878 findlike-1.3.1/setup.cfg
-drwxr-xr-x   0 soldeace  (1000) soldeace  (1000)        0 2023-07-01 01:05:21.616878 findlike-1.3.1/tests/
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     8759 2023-07-01 00:11:26.000000 findlike-1.3.1/tests/test_cli.py
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     1897 2023-07-01 00:24:14.000000 findlike-1.3.1/tests/test_corpus.py
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     2937 2023-06-27 19:22:45.000000 findlike-1.3.1/tests/test_format.py
--rw-r--r--   0 soldeace  (1000) soldeace  (1000)     1967 2023-06-28 17:48:50.000000 findlike-1.3.1/tests/test_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:56:20.771449 findlike-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-11 01:56:07.000000 findlike-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11647 2023-07-11 01:56:20.771449 findlike-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-07-11 01:56:07.000000 findlike-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:56:20.771449 findlike-1.4.0/findlike/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 01:56:07.000000 findlike-1.4.0/findlike/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-11 01:56:07.000000 findlike-1.4.0/findlike/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-07-11 01:56:07.000000 findlike-1.4.0/findlike/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-07-11 01:56:07.000000 findlike-1.4.0/findlike/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-07-11 01:56:07.000000 findlike-1.4.0/findlike/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-11 01:56:07.000000 findlike-1.4.0/findlike/markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-07-11 01:56:07.000000 findlike-1.4.0/findlike/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-11 01:56:07.000000 findlike-1.4.0/findlike/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-11 01:56:07.000000 findlike-1.4.0/findlike/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:56:20.771449 findlike-1.4.0/findlike.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11647 2023-07-11 01:56:20.000000 findlike-1.4.0/findlike.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-11 01:56:20.000000 findlike-1.4.0/findlike.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 01:56:20.000000 findlike-1.4.0/findlike.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-11 01:56:20.000000 findlike-1.4.0/findlike.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-11 01:56:20.000000 findlike-1.4.0/findlike.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 01:56:20.000000 findlike-1.4.0/findlike.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-11 01:56:07.000000 findlike-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 01:56:20.771449 findlike-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:56:20.771449 findlike-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-07-11 01:56:07.000000 findlike-1.4.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-07-11 01:56:07.000000 findlike-1.4.0/tests/test_corpus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-11 01:56:07.000000 findlike-1.4.0/tests/test_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-11 01:56:07.000000 findlike-1.4.0/tests/test_markup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-11 01:56:07.000000 findlike-1.4.0/tests/test_processor.py
```

### Comparing `findlike-1.3.1/LICENSE` & `findlike-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `findlike-1.3.1/PKG-INFO` & `findlike-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findlike
-Version: 1.3.1
+Version: 1.4.0
 Summary: findlike is a package to retrieve similar documents
 Author-email: Bruno Arine <bruno.arine@runbox.com>
 Project-URL: Homepage, http://www.github.com/brunoarine/findlike
 Project-URL: Repository, https://github.com/brunoarine/findlike.git
 Project-URL: Bug Tracker, http://www.github.com/brunoarine/findlike/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -128,14 +128,15 @@
 | `-A, --absolute-paths`      | Show the absolute path of each result instead of relative paths. Example: `findlike reference_file.txt -A`                                                                                                                                                                                                                            |
 | `-m, --max-results INTEGER` | Number of items to show in the final results. Default is 10. Example: `findlike reference_file.txt -m 5`                                                                                                                                                                                                                              |
 | `-p, --prefix TEXT`         | String to prepend each entry in the final results. Default is "". Example: `findlike reference_file.txt -p "- "`                                                                                                                                                                                                                      |
 | `-h, --hide-reference`      | Remove the first result from the scores list. This option has no effect if the `--query` option is used. Example: `findlike reference_file.txt -h`                                                                                                                                                                                    |
 | `-H, --heading TEXT`        | Text to show as the list heading. Default is "". Example: `findlike reference_file.txt -H "## Similar files"`                                                                                                                                                                                                                         |
 | `-F, --format [plain, json]` | This option sets the output format. Default is "plain". Example: `findlike reference_file.txt -F json`                                                       |
 | `-t, --threshold FLOAT`     | Similarity score threshold. All results whose score are below the determined threshold will be omitted. Default is 0.05. Example: `findlike reference_file.txt -t 0`                                                                                                                                                                  |
+| `-i, --ignore-front-matter` | Tries to strip the front-matter from markup files like Markdown and Org-mode. |
 
 ## Examples
 
 To find similar documents in a directory (recursively) against a reference text file:
 
 ```sh
 findlike -R -d /path/to/directory reference_file.md
```

### Comparing `findlike-1.3.1/README.md` & `findlike-1.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -112,14 +112,15 @@
 | `-A, --absolute-paths`      | Show the absolute path of each result instead of relative paths. Example: `findlike reference_file.txt -A`                                                                                                                                                                                                                            |
 | `-m, --max-results INTEGER` | Number of items to show in the final results. Default is 10. Example: `findlike reference_file.txt -m 5`                                                                                                                                                                                                                              |
 | `-p, --prefix TEXT`         | String to prepend each entry in the final results. Default is "". Example: `findlike reference_file.txt -p "- "`                                                                                                                                                                                                                      |
 | `-h, --hide-reference`      | Remove the first result from the scores list. This option has no effect if the `--query` option is used. Example: `findlike reference_file.txt -h`                                                                                                                                                                                    |
 | `-H, --heading TEXT`        | Text to show as the list heading. Default is "". Example: `findlike reference_file.txt -H "## Similar files"`                                                                                                                                                                                                                         |
 | `-F, --format [plain, json]` | This option sets the output format. Default is "plain". Example: `findlike reference_file.txt -F json`                                                       |
 | `-t, --threshold FLOAT`     | Similarity score threshold. All results whose score are below the determined threshold will be omitted. Default is 0.05. Example: `findlike reference_file.txt -t 0`                                                                                                                                                                  |
+| `-i, --ignore-front-matter` | Tries to strip the front-matter from markup files like Markdown and Org-mode. |
 
 ## Examples
 
 To find similar documents in a directory (recursively) against a reference text file:
 
 ```sh
 findlike -R -d /path/to/directory reference_file.md
```

### Comparing `findlike-1.3.1/findlike/cli.py` & `findlike-1.4.0/findlike/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 from pathlib import Path
 
 import click
 from nltk.stem import SnowballStemmer
 from stop_words import get_stop_words
 
+from .constants import ALGORITHM_CLASSES, FORMATTER_CLASSES, TEXT_FILE_EXT
 from .preprocessing import (
     Corpus,
     Processor,
 )
-from .utils import try_read_file, collect_paths
-from .constants import FORMATTER_CLASSES, ALGORITHM_CLASSES, TEXT_FILE_EXT
+from .utils import collect_paths
 
 
 @click.command()
 @click.version_option()
 @click.argument("reference-file", type=click.Path(), nargs=1, required=False)
 @click.option(
     "-q",
@@ -112,14 +112,21 @@
     "--hide-reference",
     "-h",
     is_flag=True,
     help="remove REFERENCE_FILE from results",
     required=False,
 )
 @click.option(
+    "--ignore-front-matter",
+    "-i",
+    is_flag=True,
+    help="ignore front-matter from supported markup languages",
+    required=False,
+)
+@click.option(
     "--heading",
     "-H",
     type=str,
     default="",
     show_default=True,
     help="results list heading",
     required=False,
@@ -155,59 +162,63 @@
     show_scores,
     recursive,
     hide_reference,
     query,
     format,
     threshold,
     absolute_paths,
+    ignore_front_matter,
 ):
     """'findlike' is a program that scans a given directory and returns the most
     similar documents in relation to REFERENCE_FILE or --query QUERY.
 
     Example using a reference file:
 
     $ findlike -d /path/to/my/notes my_recipe.md
 
     Example using a query:
 
     $ findlike -q "There is only one good, knowledge, and one evil, ignorance"
     """
 
-    # Set up the reference text.
-    if reference_file:
-        reference_content = try_read_file(Path(reference_file))
-    elif query:
-        reference_content = query
-    else:
-        raise click.UsageError(
-            "Neither REFERENCE_FILE nor --query QUERY was provided."
-        )
-
     # Put together the list of documents to be analyzed.
     directory_path = Path(directory)
-    extensions: list[str] = [filename_pattern] if filename_pattern else TEXT_FILE_EXT
+    extensions: list[str] = (
+        [filename_pattern] if filename_pattern else TEXT_FILE_EXT
+    )
     document_paths = collect_paths(
         directory=directory_path, extensions=extensions, recursive=recursive
     )
 
     # Create a corpus with the collected documents.
-    corpus = Corpus(paths=document_paths, min_chars=min_chars)
-    corpus.add_document(document=reference_content)
+    corpus = Corpus(
+        paths=document_paths,
+        min_chars=min_chars,
+        ignore_front_matter=ignore_front_matter,
+    )
+    if reference_file:
+        corpus.add_from_file(path=Path(reference_file), is_reference=True)
+    elif query:
+        corpus.add_from_query(query=query)
+    else:
+        raise click.UsageError(
+            "Neither REFERENCE_FILE nor --query QUERY was provided."
+        )
 
     # Set up the documents pre-processor.
     stemmer = SnowballStemmer(language).stem
     processor = Processor(
         stopwords=get_stop_words(language=language),
         stemmer=stemmer,
     )
-    
+
     # Set up the similarity model.
     model = ALGORITHM_CLASSES[algorithm](processor=processor)
     model.fit(corpus.documents_)  # Add reference to avoid zero division
-    scores = model.get_scores(source=reference_content)
+    scores = model.get_scores(source=corpus.reference_)
 
     # Format and print results.
     formatter = FORMATTER_CLASSES[format](
         targets=corpus.paths_,
         scores=scores,
         max_results=max_results,
         show_scores=show_scores,
```

### Comparing `findlike-1.3.1/findlike/constants.py` & `findlike-1.4.0/findlike/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
 	"*.nfo",
 	"*.noon",
 	"*.npmignore",
 	"*.npmrc",
 	"*.nuspec",
 	"*.nvmrc",
 	"*.ops",
-    "org",
+    "*.org",
 	"*.pas",
 	"*.pasm",
 	"*.patch",
 	"*.pbxproj",
 	"*.pch",
 	"*.pem",
 	"*.pg",
```

### Comparing `findlike-1.3.1/findlike/format.py` & `findlike-1.4.0/findlike/format.py`

 * *Files identical despite different names*

### Comparing `findlike-1.3.1/findlike/utils.py` & `findlike-1.4.0/findlike/utils.py`

 * *Files identical despite different names*

### Comparing `findlike-1.3.1/findlike/wrappers.py` & `findlike-1.4.0/findlike/wrappers.py`

 * *Files identical despite different names*

### Comparing `findlike-1.3.1/findlike.egg-info/PKG-INFO` & `findlike-1.4.0/findlike.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findlike
-Version: 1.3.1
+Version: 1.4.0
 Summary: findlike is a package to retrieve similar documents
 Author-email: Bruno Arine <bruno.arine@runbox.com>
 Project-URL: Homepage, http://www.github.com/brunoarine/findlike
 Project-URL: Repository, https://github.com/brunoarine/findlike.git
 Project-URL: Bug Tracker, http://www.github.com/brunoarine/findlike/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -128,14 +128,15 @@
 | `-A, --absolute-paths`      | Show the absolute path of each result instead of relative paths. Example: `findlike reference_file.txt -A`                                                                                                                                                                                                                            |
 | `-m, --max-results INTEGER` | Number of items to show in the final results. Default is 10. Example: `findlike reference_file.txt -m 5`                                                                                                                                                                                                                              |
 | `-p, --prefix TEXT`         | String to prepend each entry in the final results. Default is "". Example: `findlike reference_file.txt -p "- "`                                                                                                                                                                                                                      |
 | `-h, --hide-reference`      | Remove the first result from the scores list. This option has no effect if the `--query` option is used. Example: `findlike reference_file.txt -h`                                                                                                                                                                                    |
 | `-H, --heading TEXT`        | Text to show as the list heading. Default is "". Example: `findlike reference_file.txt -H "## Similar files"`                                                                                                                                                                                                                         |
 | `-F, --format [plain, json]` | This option sets the output format. Default is "plain". Example: `findlike reference_file.txt -F json`                                                       |
 | `-t, --threshold FLOAT`     | Similarity score threshold. All results whose score are below the determined threshold will be omitted. Default is 0.05. Example: `findlike reference_file.txt -t 0`                                                                                                                                                                  |
+| `-i, --ignore-front-matter` | Tries to strip the front-matter from markup files like Markdown and Org-mode. |
 
 ## Examples
 
 To find similar documents in a directory (recursively) against a reference text file:
 
 ```sh
 findlike -R -d /path/to/directory reference_file.md
```

### Comparing `findlike-1.3.1/pyproject.toml` & `findlike-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "findlike"
-version = "1.3.1"
+version = "1.4.0"
 authors = [{ name = "Bruno Arine", email = "bruno.arine@runbox.com" }]
 description = "findlike is a package to retrieve similar documents"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `findlike-1.3.1/tests/test_cli.py` & `findlike-1.4.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `findlike-1.3.1/tests/test_format.py` & `findlike-1.4.0/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `findlike-1.3.1/tests/test_processor.py` & `findlike-1.4.0/tests/test_processor.py`

 * *Files identical despite different names*

