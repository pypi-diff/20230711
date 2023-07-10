# Comparing `tmp/problem_bank_scripts-0.7.0.tar.gz` & `tmp/problem_bank_scripts-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "problem_bank_scripts-0.7.0.tar", max compression
+gzip compressed data, was "problem_bank_scripts-0.7.1.tar", max compression
```

## Comparing `problem_bank_scripts-0.7.0.tar` & `problem_bank_scripts-0.7.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rwxr-xr-x   0        0        0        1 2021-05-16 14:07:02.985176 problem_bank_scripts-0.7.0/LICENSE
--rw-r--r--   0        0        0     1605 2023-06-15 01:42:11.784217 problem_bank_scripts-0.7.0/README.md
--rw-r--r--   0        0        0     1051 2023-07-07 00:05:52.988895 problem_bank_scripts-0.7.0/pyproject.toml
--rw-r--r--   0        0        0       59 2023-07-07 00:06:02.994431 problem_bank_scripts-0.7.0/src/problem_bank_scripts/__init__.py
--rw-r--r--   0        0        0     1757 2023-06-15 17:31:34.807559 problem_bank_scripts-0.7.0/src/problem_bank_scripts/attributions.json
--rw-r--r--   0        0        0    13614 2023-07-07 00:02:47.412321 problem_bank_scripts-0.7.0/src/problem_bank_scripts/prairielearn.py
--rw-r--r--   0        0        0    46545 2023-07-07 00:05:32.880433 problem_bank_scripts-0.7.0/src/problem_bank_scripts/problem_bank_scripts.py
--rw-r--r--   0        0        0      129 2022-06-24 05:48:29.289246 problem_bank_scripts-0.7.0/src/problem_bank_scripts/qti_export.py
--rw-r--r--   0        0        0    19225 2022-06-24 07:32:56.504377 problem_bank_scripts-0.7.0/src/problem_bank_scripts/webwork_to_md.py
--rw-r--r--   0        0        0     2643 2023-07-07 00:07:06.814077 problem_bank_scripts-0.7.0/setup.py
--rw-r--r--   0        0        0     2625 2023-07-07 00:07:06.814296 problem_bank_scripts-0.7.0/PKG-INFO
+-rwxr-xr-x   0        0        0        1 2021-05-16 14:07:02.985176 problem_bank_scripts-0.7.1/LICENSE
+-rw-r--r--   0        0        0     1605 2023-06-15 01:42:11.784217 problem_bank_scripts-0.7.1/README.md
+-rw-r--r--   0        0        0     1052 2023-07-10 22:54:12.853113 problem_bank_scripts-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0       59 2023-07-10 22:46:01.404559 problem_bank_scripts-0.7.1/src/problem_bank_scripts/__init__.py
+-rw-r--r--   0        0        0     1757 2023-06-15 17:31:34.807559 problem_bank_scripts-0.7.1/src/problem_bank_scripts/attributions.json
+-rw-r--r--   0        0        0    13614 2023-07-07 00:02:47.412321 problem_bank_scripts-0.7.1/src/problem_bank_scripts/prairielearn.py
+-rw-r--r--   0        0        0    47476 2023-07-10 22:57:58.740430 problem_bank_scripts-0.7.1/src/problem_bank_scripts/problem_bank_scripts.py
+-rw-r--r--   0        0        0      129 2022-06-24 05:48:29.289246 problem_bank_scripts-0.7.1/src/problem_bank_scripts/qti_export.py
+-rw-r--r--   0        0        0    19225 2022-06-24 07:32:56.504377 problem_bank_scripts-0.7.1/src/problem_bank_scripts/webwork_to_md.py
+-rw-r--r--   0        0        0     2644 2023-07-10 22:58:44.071882 problem_bank_scripts-0.7.1/setup.py
+-rw-r--r--   0        0        0     2576 2023-07-10 22:58:44.072101 problem_bank_scripts-0.7.1/PKG-INFO
```

### Comparing `problem_bank_scripts-0.7.0/README.md` & `problem_bank_scripts-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `problem_bank_scripts-0.7.0/pyproject.toml` & `problem_bank_scripts-0.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "problem_bank_scripts"
-version = "0.7.0"
+version = "0.7.1"
 description = "A package with useful functions to convert between different problem bank formats."
 authors = ["Open Problem Bank Team"]
 license = "MIT"
 readme = "README.md"
 documentation = "https://problem_bank_scripts.readthedocs.io/en/latest/"
 homepage = "https://github.com/open-resources/problem_bank_scripts"
 repository = "https://github.com/open-resources/problem_bank_scripts"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.10"
 pandas = "^2.0"
 PyYAML = "^6.0"
 docopt = "^0.6.2"
 numpy = "^1.22"
 markdown-it-py = "^2.1.0"
 mdformat = "^0.7.14"
 sympy = "^1.8"
```

### Comparing `problem_bank_scripts-0.7.0/src/problem_bank_scripts/attributions.json` & `problem_bank_scripts-0.7.1/src/problem_bank_scripts/attributions.json`

 * *Files identical despite different names*

### Comparing `problem_bank_scripts-0.7.0/src/problem_bank_scripts/prairielearn.py` & `problem_bank_scripts-0.7.1/src/problem_bank_scripts/prairielearn.py`

 * *Files identical despite different names*

### Comparing `problem_bank_scripts-0.7.0/src/problem_bank_scripts/problem_bank_scripts.py` & `problem_bank_scripts-0.7.1/src/problem_bank_scripts/problem_bank_scripts.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,25 +15,40 @@
 from collections import defaultdict
 from shutil import copy2
 import re
 import codecs
 import importlib.util
 import problem_bank_helpers as pbh
 import pandas as pd
+import warnings
 
 ## Parse Markdown
 import markdown_it
 import mdformat
 
 ## Dealing with YAML
 import yaml
 
 ## Loading files : https://stackoverflow.com/a/60687710
 import importlib.resources
 
+## Topic Validation
+topic_list = set()
+path = pathlib.Path().resolve()
+try:
+    subjects = [path.split('instructor_')[1].split('_bank')[0]]
+except:
+    warnings.warn(f"\na subject could not be found from the path:\n'{path}'\ntopics from all subjects have been loaded.")
+    subjects = ["physics", "datascience", "stats"]
+
+for subject in subjects:
+    url = f"https://raw.githubusercontent.com/open-resources/learning_outcomes/main/outputs_csv/LO_{subject}.csv"
+    learning_outcomes = pd.read_csv(url)
+    topic_list |= set(learning_outcomes["Topic"])
+
 # Start of reading/parsing functions
 
 
 def defdict_to_dict(defdict, finaldict):
     """Convert a defaultdict (nested) to a regular dictionary.
         - Answer copied from: https://stackoverflow.com/a/61133504/2217577
     Args:
@@ -264,15 +279,15 @@
     """
 
     mdtext = pathlib.Path(filepath).read_text(encoding="utf8")
 
     # Deal with YAML header
     header_text = mdtext.rsplit("---\n")[1]
     header = yaml.safe_load("---\n" + header_text)
-
+    validate_header(header)
     # Deal with Markdown Body
     body = mdtext.rsplit("---\n")[2]
 
     # Set up the markdown parser
     # to be honest, not fully sure what's going on here, see this issue: https://github.com/executablebooks/markdown-it-py/issues/164
 
     mdit = markdown_it.MarkdownIt()
@@ -1226,7 +1241,12 @@
     html = html.replace(
         ' highlight-lines=""', ""
     )  # Remove empty highlight-lines attributes
     html = re.sub(r"(?<!\\)`(?P<Code>[^`]+)`", r"<code>\g<Code></code>", html)
     html = html.replace("\\`", "`")  # Replace escaped backticks
     return html
 
+def validate_header(header_dict):
+    # check if topic is valid (i.e. from the list of topics in the learning_outcomes repo for this subject)
+    if header_dict["topic"] not in topic_list and header_dict["topic"] != "Template":
+        raise ValueError(f"topic '{header_dict['topic']}' is not listed in the learning outcomes")
+
```

### Comparing `problem_bank_scripts-0.7.0/src/problem_bank_scripts/webwork_to_md.py` & `problem_bank_scripts-0.7.1/src/problem_bank_scripts/webwork_to_md.py`

 * *Files identical despite different names*

### Comparing `problem_bank_scripts-0.7.0/setup.py` & `problem_bank_scripts-0.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,24 +18,24 @@
  'numpy>=1.22,<2.0',
  'pandas>=2.0,<3.0',
  'problem-bank-helpers>=0.1.14,<0.2.0',
  'sympy>=1.8,<2.0']
 
 setup_kwargs = {
     'name': 'problem-bank-scripts',
-    'version': '0.7.0',
+    'version': '0.7.1',
     'description': 'A package with useful functions to convert between different problem bank formats.',
     'long_description': '# Problem Bank Scripts \n\n[![Python](https://img.shields.io/badge/python-3.9-blue)]()\n[![codecov](https://codecov.io/gh/open-resources/problem_bank_scripts/branch/main/graph/badge.svg)](https://codecov.io/gh/open-resources/problem_bank_scripts)\n[![Documentation Status](https://readthedocs.org/projects/problem_bank_scripts/badge/?version=latest)](https://problem_bank_scripts.readthedocs.io/en/latest/?badge=latest)\n\n\n## Installation\n\n```bash\n$ pip install -i https://test.pypi.org/simple/ problem_bank_scripts\n```\n\n## Update version\n\nHere are the steps to increment the version (replace patch with major/minor/patch)\n\n```\npoetry version patch\n\npico src/problem_bank_scripts/__init__.py\n\npico tests/test_problem_bank_scripts.py\n\npoetry run pytest\n\ncd docs; poetry run make html; cd ..\n\ngit add .; git commit -m "increment version"; git push\n\npoetry build\n\npoetry publish\n```\n\n\n## Features\n\n- TODO\n\n## Dependencies\n\n- TODO\n\n## Usage\n\n- TODO\n\n## Documentation\n\nThe official documentation is hosted on Read the Docs: https://problem_bank_scripts.readthedocs.io/en/latest/\n\n## Contributors\n\nWe welcome and recognize all contributions. You can see a list of current contributors in the [contributors tab](https://github.com/open-resources/problem_bank_scripts/graphs/contributors).\n\n### Credits\n\nThis package was created with Cookiecutter and the UBC-MDS/cookiecutter-ubc-mds project template, modified from the [pyOpenSci/cookiecutter-pyopensci](https://github.com/pyOpenSci/cookiecutter-pyopensci) project template and the [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage).\n',
     'author': 'Open Problem Bank Team',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/open-resources/problem_bank_scripts',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
+    'python_requires': '>=3.10,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `problem_bank_scripts-0.7.0/PKG-INFO` & `problem_bank_scripts-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: problem-bank-scripts
-Version: 0.7.0
+Version: 0.7.1
 Summary: A package with useful functions to convert between different problem bank formats.
 Home-page: https://github.com/open-resources/problem_bank_scripts
 License: MIT
 Author: Open Problem Bank Team
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: docopt (>=0.6.2,<0.7.0)
 Requires-Dist: markdown-it-py (>=2.1.0,<3.0.0)
 Requires-Dist: mdformat (>=0.7.14,<0.8.0)
 Requires-Dist: numpy (>=1.22,<2.0)
 Requires-Dist: pandas (>=2.0,<3.0)
 Requires-Dist: problem-bank-helpers (>=0.1.14,<0.2.0)
```

