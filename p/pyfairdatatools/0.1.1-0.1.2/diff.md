# Comparing `tmp/pyfairdatatools-0.1.1.tar.gz` & `tmp/pyfairdatatools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfairdatatools-0.1.1.tar", max compression
+gzip compressed data, was "pyfairdatatools-0.1.2.tar", max compression
```

## Comparing `pyfairdatatools-0.1.1.tar` & `pyfairdatatools-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1109 2023-05-04 17:42:12.820675 pyfairdatatools-0.1.1/LICENSE.md
--rw-r--r--   0        0        0      257 2023-07-11 20:14:43.501620 pyfairdatatools-0.1.1/pyfairdatatools/__init__.py
--rw-r--r--   0        0        0      199 2023-05-09 00:30:52.905419 pyfairdatatools-0.1.1/pyfairdatatools/__main__.py
--rw-r--r--   0        0        0    15683 2023-06-19 19:50:06.297393 pyfairdatatools-0.1.1/pyfairdatatools/assets/languages.json
--rw-r--r--   0        0        0   251950 2023-05-18 20:27:24.899227 pyfairdatatools-0.1.1/pyfairdatatools/assets/licenses.json
--rw-r--r--   0        0        0      636 2023-05-09 00:54:20.112753 pyfairdatatools-0.1.1/pyfairdatatools/cli.py
--rw-r--r--   0        0        0    12566 2023-07-11 00:10:10.930787 pyfairdatatools-0.1.1/pyfairdatatools/generate.py
--rw-r--r--   0        0        0     3005 2023-05-04 20:33:46.686345 pyfairdatatools-0.1.1/pyfairdatatools/gui.py
--rw-r--r--   0        0        0    71270 2023-07-06 18:02:25.758085 pyfairdatatools-0.1.1/pyfairdatatools/schemas/dataset_description.schema.json
--rw-r--r--   0        0        0     2854 2023-07-06 18:02:25.759069 pyfairdatatools-0.1.1/pyfairdatatools/schemas/folder_structure.schema.json
--rw-r--r--   0        0        0     2222 2023-07-06 18:02:25.759069 pyfairdatatools-0.1.1/pyfairdatatools/schemas/participants.schema.json
--rw-r--r--   0        0        0     3300 2023-07-06 18:02:25.760069 pyfairdatatools-0.1.1/pyfairdatatools/schemas/readme.schema.json
--rw-r--r--   0        0        0    68051 2023-07-10 23:27:33.272942 pyfairdatatools-0.1.1/pyfairdatatools/schemas/study_description.schema.json
--rw-r--r--   0        0        0        0 2023-07-06 18:02:25.762076 pyfairdatatools-0.1.1/pyfairdatatools/templates/high-level-dataset-structure/activity_monitor/README.md
--rw-r--r--   0        0        0        0 2023-07-06 18:02:25.763076 pyfairdatatools-0.1.1/pyfairdatatools/templates/high-level-dataset-structure/best_corrected_visual_acuity/README.md
--rw-r--r--   0        0        0        0 2023-07-06 18:02:25.761077 pyfairdatatools-0.1.1/pyfairdatatools/templates/high-level-dataset-structure/CHANGELOG.md
--rw-r--r--   0        0        0        0 2023-07-06 18:02:25.763076 pyfairdatatools-0.1.1/pyfairdatatools/templates/high-level-dataset-structure/dataset_description.json
--rw-r--r--   0        0        0        0 2023-07-06 18:02:25.761077 pyfairdatatools-0.1.1/pyfairdatatools/templates/high-level-dataset-structure/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-07-06 18:02:25.763076 pyfairdatatools-0.1.1/pyfairdatatools/templates/high-level-dataset-structure/participants.json
--rw-r--r--   0        0        0        0 2023-07-06 18:02:25.764075 pyfairdatatools-0.1.1/pyfairdatatools/templates/high-level-dataset-structure/participants.tsv
--rw-r--r--   0        0        0        0 2023-07-06 18:02:25.762076 pyfairdatatools-0.1.1/pyfairdatatools/templates/high-level-dataset-structure/README.md
--rw-r--r--   0        0        0      442 2023-05-22 21:03:22.914816 pyfairdatatools-0.1.1/pyfairdatatools/templates/readme.mdtxt.template
--rw-r--r--   0        0        0       35 2023-05-04 17:42:12.915909 pyfairdatatools-0.1.1/pyfairdatatools/tests/__init__.py
--rw-r--r--   0        0        0      278 2023-05-04 20:19:34.392045 pyfairdatatools-0.1.1/pyfairdatatools/tests/conftest.py
--rw-r--r--   0        0        0     1417 2023-05-30 22:36:52.736046 pyfairdatatools-0.1.1/pyfairdatatools/utils.py
--rw-r--r--   0        0        0    13715 2023-07-10 23:38:43.990162 pyfairdatatools-0.1.1/pyfairdatatools/validate.py
--rw-r--r--   0        0        0     3011 2023-07-11 20:14:51.486369 pyfairdatatools-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     8119 2023-07-11 20:12:21.296144 pyfairdatatools-0.1.1/README.md
--rw-r--r--   0        0        0     9483 1970-01-01 00:00:00.000000 pyfairdatatools-0.1.1/setup.py
--rw-r--r--   0        0        0     9303 1970-01-01 00:00:00.000000 pyfairdatatools-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1109 2023-05-04 17:42:12.820675 pyfairdatatools-0.1.2/LICENSE.md
+-rw-r--r--   0        0        0      257 2023-07-11 20:51:14.926401 pyfairdatatools-0.1.2/pyfairdatatools/__init__.py
+-rw-r--r--   0        0        0      199 2023-05-09 00:30:52.905419 pyfairdatatools-0.1.2/pyfairdatatools/__main__.py
+-rw-r--r--   0        0        0    15683 2023-06-19 19:50:06.297393 pyfairdatatools-0.1.2/pyfairdatatools/assets/languages.json
+-rw-r--r--   0        0        0   251950 2023-05-18 20:27:24.899227 pyfairdatatools-0.1.2/pyfairdatatools/assets/licenses.json
+-rw-r--r--   0        0        0      636 2023-05-09 00:54:20.112753 pyfairdatatools-0.1.2/pyfairdatatools/cli.py
+-rw-r--r--   0        0        0    12566 2023-07-11 00:10:10.930787 pyfairdatatools-0.1.2/pyfairdatatools/generate.py
+-rw-r--r--   0        0        0     3005 2023-05-04 20:33:46.686345 pyfairdatatools-0.1.2/pyfairdatatools/gui.py
+-rw-r--r--   0        0        0    71270 2023-07-06 18:02:25.758085 pyfairdatatools-0.1.2/pyfairdatatools/schemas/dataset_description.schema.json
+-rw-r--r--   0        0        0     2854 2023-07-06 18:02:25.759069 pyfairdatatools-0.1.2/pyfairdatatools/schemas/folder_structure.schema.json
+-rw-r--r--   0        0        0     2222 2023-07-06 18:02:25.759069 pyfairdatatools-0.1.2/pyfairdatatools/schemas/participants.schema.json
+-rw-r--r--   0        0        0     3300 2023-07-06 18:02:25.760069 pyfairdatatools-0.1.2/pyfairdatatools/schemas/readme.schema.json
+-rw-r--r--   0        0        0    68051 2023-07-10 23:27:33.272942 pyfairdatatools-0.1.2/pyfairdatatools/schemas/study_description.schema.json
+-rw-r--r--   0        0        0        0 2023-07-06 18:02:25.762076 pyfairdatatools-0.1.2/pyfairdatatools/templates/high-level-dataset-structure/activity_monitor/README.md
+-rw-r--r--   0        0        0        0 2023-07-06 18:02:25.763076 pyfairdatatools-0.1.2/pyfairdatatools/templates/high-level-dataset-structure/best_corrected_visual_acuity/README.md
+-rw-r--r--   0        0        0        0 2023-07-06 18:02:25.761077 pyfairdatatools-0.1.2/pyfairdatatools/templates/high-level-dataset-structure/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2023-07-06 18:02:25.763076 pyfairdatatools-0.1.2/pyfairdatatools/templates/high-level-dataset-structure/dataset_description.json
+-rw-r--r--   0        0        0        0 2023-07-06 18:02:25.761077 pyfairdatatools-0.1.2/pyfairdatatools/templates/high-level-dataset-structure/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-07-06 18:02:25.763076 pyfairdatatools-0.1.2/pyfairdatatools/templates/high-level-dataset-structure/participants.json
+-rw-r--r--   0        0        0        0 2023-07-06 18:02:25.764075 pyfairdatatools-0.1.2/pyfairdatatools/templates/high-level-dataset-structure/participants.tsv
+-rw-r--r--   0        0        0        0 2023-07-06 18:02:25.762076 pyfairdatatools-0.1.2/pyfairdatatools/templates/high-level-dataset-structure/README.md
+-rw-r--r--   0        0        0      442 2023-05-22 21:03:22.914816 pyfairdatatools-0.1.2/pyfairdatatools/templates/readme.mdtxt.template
+-rw-r--r--   0        0        0       35 2023-05-04 17:42:12.915909 pyfairdatatools-0.1.2/pyfairdatatools/tests/__init__.py
+-rw-r--r--   0        0        0      278 2023-05-04 20:19:34.392045 pyfairdatatools-0.1.2/pyfairdatatools/tests/conftest.py
+-rw-r--r--   0        0        0     1417 2023-05-30 22:36:52.736046 pyfairdatatools-0.1.2/pyfairdatatools/utils.py
+-rw-r--r--   0        0        0    13715 2023-07-10 23:38:43.990162 pyfairdatatools-0.1.2/pyfairdatatools/validate.py
+-rw-r--r--   0        0        0     2997 2023-07-11 20:51:06.840155 pyfairdatatools-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     8119 2023-07-11 20:12:21.296144 pyfairdatatools-0.1.2/README.md
+-rw-r--r--   0        0        0     9465 1970-01-01 00:00:00.000000 pyfairdatatools-0.1.2/setup.py
+-rw-r--r--   0        0        0     9271 1970-01-01 00:00:00.000000 pyfairdatatools-0.1.2/PKG-INFO
```

### Comparing `pyfairdatatools-0.1.1/LICENSE.md` & `pyfairdatatools-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyfairdatatools-0.1.1/pyfairdatatools/assets/languages.json` & `pyfairdatatools-0.1.2/pyfairdatatools/assets/languages.json`

 * *Files identical despite different names*

### Comparing `pyfairdatatools-0.1.1/pyfairdatatools/assets/licenses.json` & `pyfairdatatools-0.1.2/pyfairdatatools/assets/licenses.json`

 * *Files identical despite different names*

### Comparing `pyfairdatatools-0.1.1/pyfairdatatools/cli.py` & `pyfairdatatools-0.1.2/pyfairdatatools/cli.py`

 * *Files identical despite different names*

### Comparing `pyfairdatatools-0.1.1/pyfairdatatools/generate.py` & `pyfairdatatools-0.1.2/pyfairdatatools/generate.py`

 * *Files identical despite different names*

### Comparing `pyfairdatatools-0.1.1/pyfairdatatools/gui.py` & `pyfairdatatools-0.1.2/pyfairdatatools/gui.py`

 * *Files identical despite different names*

### Comparing `pyfairdatatools-0.1.1/pyfairdatatools/schemas/dataset_description.schema.json` & `pyfairdatatools-0.1.2/pyfairdatatools/schemas/dataset_description.schema.json`

 * *Files identical despite different names*

### Comparing `pyfairdatatools-0.1.1/pyfairdatatools/schemas/folder_structure.schema.json` & `pyfairdatatools-0.1.2/pyfairdatatools/schemas/folder_structure.schema.json`

 * *Files identical despite different names*

### Comparing `pyfairdatatools-0.1.1/pyfairdatatools/schemas/participants.schema.json` & `pyfairdatatools-0.1.2/pyfairdatatools/schemas/participants.schema.json`

 * *Files identical despite different names*

### Comparing `pyfairdatatools-0.1.1/pyfairdatatools/schemas/readme.schema.json` & `pyfairdatatools-0.1.2/pyfairdatatools/schemas/readme.schema.json`

 * *Files identical despite different names*

### Comparing `pyfairdatatools-0.1.1/pyfairdatatools/schemas/study_description.schema.json` & `pyfairdatatools-0.1.2/pyfairdatatools/schemas/study_description.schema.json`

 * *Files identical despite different names*

### Comparing `pyfairdatatools-0.1.1/pyfairdatatools/utils.py` & `pyfairdatatools-0.1.2/pyfairdatatools/utils.py`

 * *Files identical despite different names*

### Comparing `pyfairdatatools-0.1.1/pyfairdatatools/validate.py` & `pyfairdatatools-0.1.2/pyfairdatatools/validate.py`

 * *Files identical despite different names*

### Comparing `pyfairdatatools-0.1.1/pyproject.toml` & `pyfairdatatools-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 
 name = "pyfairdatatools"
-version = "0.1.1"
+version = "0.1.2"
 description = "Tools for AI-READI"
 
 packages = [{ include = "pyfairdatatools" }]
 
 license = "MIT"
 authors = ["FAIR Data Innovations Hub <contact@fairdataihub.org>"]
 
@@ -33,15 +33,14 @@
 
 python = "^3.8"
 urllib3="<2.0"
 
 # TODO: Remove these and add your library's requirements
 click = "*"
 minilog = "*"
-art = "^5.9"
 jsonschema = "^4.17.3"
 dicttoxml = "^1.7.16"
 types-requests = "^2.30.0.0"
 pymdown-extensions = "^10.0.1"
 validators = "^0.20.0"
```

### Comparing `pyfairdatatools-0.1.1/README.md` & `pyfairdatatools-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyfairdatatools-0.1.1/setup.py` & `pyfairdatatools-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,30 +10,29 @@
                      'schemas/*',
                      'templates/*',
                      'templates/high-level-dataset-structure/*',
                      'templates/high-level-dataset-structure/activity_monitor/*',
                      'templates/high-level-dataset-structure/best_corrected_visual_acuity/*']}
 
 install_requires = \
-['art>=5.9,<6.0',
- 'click',
+['click',
  'dicttoxml>=1.7.16,<2.0.0',
  'jsonschema>=4.17.3,<5.0.0',
  'minilog',
  'pymdown-extensions>=10.0.1,<11.0.0',
  'types-requests>=2.30.0.0,<3.0.0.0',
  'urllib3<2.0',
  'validators>=0.20.0,<0.21.0']
 
 entry_points = \
 {'console_scripts': ['pyfairdatatools = pyfairdatatools.cli:main']}
 
 setup_kwargs = {
     'name': 'pyfairdatatools',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Tools for AI-READI',
     'long_description': '<div align="center">\n\n<img src="https://freesvg.org/img/1653682897science-svgrepo-com.png" alt="logo" width="200" height="auto" />\n\n<br />\n\n<h1>pyfairdatatools</h1>\n\n<p>\nPython package for the FAIR tools of fairhub.io\n</p>\n\n<br />\n\n<p>\n  <a href="https://github.com/AI-READI/pyfairdatatools/graphs/contributors">\n    <img src="https://img.shields.io/github/contributors/AI-READI/pyfairdatatools.svg?style=flat-square" alt="contributors" />\n  </a>\n  <a href="https://github.com/AI-READI/pyfairdatatools/stargazers">\n    <img src="https://img.shields.io/github/stars/AI-READI/pyfairdatatools.svg?style=flat-square" alt="stars" />\n  </a>\n  <a href="https://github.com/AI-READI/pyfairdatatools/issues/">\n    <img src="https://img.shields.io/github/issues/AI-READI/pyfairdatatools.svg?style=flat-square" alt="open issues" />\n  </a>\n  <a href="https://github.com/AI-READI/pyfairdatatools/blob/main/LICENSE">\n    <img src="https://img.shields.io/github/license/AI-READI/pyfairdatatools.svg?style=flat-square" alt="license" />\n  </a>\n  <a href="https://fairdataihub.org/fairshare">\n    <img src="https://raw.githubusercontent.com/fairdataihub/FAIRshare/main/badge.svg" alt="Curated with FAIRshare" />\n  </a>\n</p>\n<p>\n  <a href="https://github.com/AI-READI/pyfairdatatools/actions">\n    <img src="https://img.shields.io/github/actions/workflow/status/AI-READI/pyfairdatatools/main.yml?branch=main&label=linux" alt="Unix Build Status" />\n  </a>\n  <a href="https://ci.appveyor.com/project/AI-READI/pyfairdatatools">\n    <img src="https://img.shields.io/appveyor/ci/AI-READI/pyfairdatatools.svg?label=windows" alt="Windows Build Status" />\n  </a>\n  <a href="https://codecov.io/gh/AI-READI/pyfairdatatools">\n    <img src="https://img.shields.io/codecov/c/gh/AI-READI/pyfairdatatools" alt="Coverage Status" />\n  </a>\n  <a href="https://scrutinizer-ci.com/g/AI-READI/pyfairdatatools">\n    <img src="https://img.shields.io/scrutinizer/g/AI-READI/pyfairdatatools.svg" alt="Scrutinizer Code Quality" />\n  </a>\n  <a href="https://pypi.org/project/pyfairdatatools">\n    <img src="https://img.shields.io/pypi/l/pyfairdatatools.svg" alt="PyPI License" />\n  </a>\n  <a href="https://pypi.org/project/pyfairdatatools">\n    <img src="https://img.shields.io/pypi/v/pyfairdatatools.svg" alt="PyPI Version" />\n  </a>\n  <a href="https://pypistats.org/packages/pyfairdatatools">\n    <img src="https://img.shields.io/pypi/dm/pyfairdatatools.svg?color=orange" alt="PyPI Downloads" />\n  </a>\n</p>\n\n<h4>\n    <a href="https://ai-readi.github.io/pyfairdatatools/">Documentation</a>\n  <span> · </span>\n    <a href="https://ai-readi.github.io/pyfairdatatools/about/changelog/">Changelog</a>\n  <span> · </span>\n    <a href="https://github.com/AI-READI/pyfairdatatools/issues/">Report Bug</a>\n  <span> · </span>\n    <a href="#">Request Feature</a>\n  </h4>\n</div>\n\n<br />\n\n---\n\n## Description\n\npyfairdatatools is a Python package that includes functions of fairhub.io for making data FAIR. This consists of a collection of helpful functions for extracting, transforming raw data, generating relevant metadata files and validating the data and metadata files against the FAIR guidelines adopted by the AI-READI project. Beside supporting fairhub.io, our aim is that the package can be used by anyone wanting to make their data FAIR according to the AI-READI FAIR guidelines.\n\n## Getting started\n\n### Prerequisites/Dependencies\n\nYou will need the following installed on your system:\n\n- Python 3.8+\n- [Pip](https://pip.pypa.io/en/stable/)\n- [Poetry](https://poetry.eustace.io/)\n\n### Installing\n\nInstall it directly into an activated virtual environment:\n\n```bash\npip install pyfairdatatools\n```\n\nor add it to your [Poetry](https://poetry.eustace.io/) project:\n\n```bash\npoetry add pyfairdatatools\n```\n\n### Usage\n\nAfter installation, the package can be imported:\n\n```bash\n$ python\n>>> import pyfairdatatools\n>>> pyfairdatatools.__version__\n```\n\n### Inputs and Outputs\n\nThe input of most functions will be a json format schema (see "Standards followed" sections) that contain data and metadata related information. The outputs of most functions will be standards metadata files, structured data, etc.\n\n## Standards followed\n\nThis software is being developed following the [Software Development Best Practices of the AI-READI Project](https://github.com/AI-READI/software-development-best-practices), which include following the [FAIR-BioRS guidelines](https://github.com/FAIR-BioRS/Guidelines). Amongs other, we are following closely the [PEP 8 Style Guide for Python Code](https://peps.python.org/pep-0008/).\n\nThe input structure of the function is currently being developed but anticipated to follow existing schemas such as schema.org and bioschemas.org.\n\n## Contributing\n\n<a href="https://github.com/AI-READI/pyfairdatatools/graphs/contributors">\n  <img src="https://contrib.rocks/image?repo=AI-READI/pyfairdatatools" />\n</a>\n\nContributions are always welcome!\n\nIf you are interested in reporting/fixing issues and contributing directly to the code base, please see [CONTRIBUTING.md](CONTRIBUTING.md) for more information on what we\'re looking for and how to get started.\n\n## Issues and Feedback\n\nTo report any issues with the software, suggest improvements, or request a new feature, please open a new issue via the [Issues](https://github.com/AI-READI/pyfairdatatools/issues) tab. Provide adequate information (operating system, steps leading to error, screenshots) so we can help you efficiently.\n\n### Setup\n\nIf you would like to update the package, please follow the instructions below.\n\n1. Create a local virtual environment and activate it:\n\n   ```bash\n   python -m venv .venv\n   source .venv/bin/activate\n   ```\n\n   If you are using Anaconda, you can create a virtual environment with:\n\n   ```bash\n   conda create -n pyfairdatatools-env python\n   conda activate pyfairdatatools-env\n   ```\n\n2. Install the dependencies for this package. We use [Poetry](https://poetry.eustace.io/) to manage the dependencies:\n\n   ```bash\n   pip install poetry==1.3.2\n   poetry install\n   ```\n\n   You can also use version 1.2.0 of Poetry, but you will need to run `poetry lock` after installing the dependencies.\n\n3. Add your modifications and run the tests:\n\n   ```bash\n   poetry run pytest\n   ```\n\n   If you need to add new python packages, you can use Poetry to add them:\n\n   ```bash\n    poetry add <package-name>\n   ```\n\n4. Format the code:\n\n   ```bash\n   poe format\n   ```\n\n5. Check the code quality:\n\n   ```bash\n   poetry run flake8 pyfairdatatools tests\n   ```\n\n6. Run the tests and check the code coverage:\n\n   ```bash\n   poe test\n   poe test --cov=pyfairdatatools\n   ```\n\n7. Build the package:\n\n   Update the version number in `pyproject.toml` and `pyfairdatatools/__init__.py` and then run:\n\n   ```text\n   poetry build\n   ```\n\n8. Publish the package:\n\n   ```bash\n   poetry publish\n   ```\n\n   Set your API token for PyPI in your environment variables:\n\n   ```bash\n   poetry config pypi-token.pypi your-api-token\n   ```\n\n## License\n\nThis work is licensed under\n[MIT](https://opensource.org/licenses/mit). See [LICENSE](https://github.com/AI-READI/pyfairdatatools/blob/main/LICENSE) for more information.\n\n<a href="https://aireadi.org" >\n  <img src="https://www.channelfutures.com/files/2017/04/3_0.png" height="30" />\n</a>\n\n## How to cite\n\nIf you are using this package or reusing the source code from this repository for any purpose, please cite:\n\n```text\n    Coming soon...\n```\n\n## Acknowledgements\n\nThis project is funded by the NIH under award number 1OT2OD032644. The content is solely the responsibility of the authors and does not necessarily represent the official views of the NIH.\n\nAdd any other acknowledgements here.\n\n<br />\n\n---\n\n<br />\n\n<div align="center">\n\n<a href="https://aireadi.org">\n  <img src="https://github.com/AI-READI/AI-READI-logo/raw/main/logo/png/option2.png" height="200" />\n</a>\n\n</div>\n',
     'author': 'FAIR Data Innovations Hub',
     'author_email': 'contact@fairdataihub.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://pypi.org/project/pyfairdatatools',
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['pyfairdatatools', 'pyfairdatatools.tests'] package_data = \ {'': ['*'],
 'pyfairdatatools': ['assets/*', 'schemas/*', 'templates/*', 'templates/high-
 level-dataset-structure/*', 'templates/high-level-dataset-structure/
 activity_monitor/*', 'templates/high-level-dataset-structure/
-best_corrected_visual_acuity/*']} install_requires = \ ['art>=5.9,<6.0',
-'click', 'dicttoxml>=1.7.16,<2.0.0', 'jsonschema>=4.17.3,<5.0.0', 'minilog',
-'pymdown-extensions>=10.0.1,<11.0.0', 'types-requests>=2.30.0.0,<3.0.0.0',
+best_corrected_visual_acuity/*']} install_requires = \ ['click',
+'dicttoxml>=1.7.16,<2.0.0', 'jsonschema>=4.17.3,<5.0.0', 'minilog', 'pymdown-
+extensions>=10.0.1,<11.0.0', 'types-requests>=2.30.0.0,<3.0.0.0',
 'urllib3<2.0', 'validators>=0.20.0,<0.21.0'] entry_points = \
 {'console_scripts': ['pyfairdatatools = pyfairdatatools.cli:main']}
-setup_kwargs = { 'name': 'pyfairdatatools', 'version': '0.1.1', 'description':
+setup_kwargs = { 'name': 'pyfairdatatools', 'version': '0.1.2', 'description':
 'Tools for AI-READI', 'long_description': '
                                 \n\n[logo]\n\n
                                      \n\n
                          ****** pyfairdatatools ******
                                      \n\n
               \nPython package for the FAIR tools of fairhub.io\n
                                      \n\n
```

### Comparing `pyfairdatatools-0.1.1/PKG-INFO` & `pyfairdatatools-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfairdatatools
-Version: 0.1.1
+Version: 0.1.2
 Summary: Tools for AI-READI
 Home-page: https://pypi.org/project/pyfairdatatools
 License: MIT
 Author: FAIR Data Innovations Hub
 Author-email: contact@fairdataihub.org
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 1 - Planning
@@ -17,15 +17,14 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
-Requires-Dist: art (>=5.9,<6.0)
 Requires-Dist: click
 Requires-Dist: dicttoxml (>=1.7.16,<2.0.0)
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
 Requires-Dist: minilog
 Requires-Dist: pymdown-extensions (>=10.0.1,<11.0.0)
 Requires-Dist: types-requests (>=2.30.0.0,<3.0.0.0)
 Requires-Dist: urllib3 (<2.0)
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: pyfairdatatools Version: 0.1.1 Summary: Tools for
+Metadata-Version: 2.1 Name: pyfairdatatools Version: 0.1.2 Summary: Tools for
 AI-READI Home-page: https://pypi.org/project/pyfairdatatools License: MIT
 Author: FAIR Data Innovations Hub Author-email: contact@fairdataihub.org
 Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: MIT License Classifier: Natural Language
 :: English Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
-Requires-Dist: art (>=5.9,<6.0) Requires-Dist: click Requires-Dist: dicttoxml
-(>=1.7.16,<2.0.0) Requires-Dist: jsonschema (>=4.17.3,<5.0.0) Requires-Dist:
-minilog Requires-Dist: pymdown-extensions (>=10.0.1,<11.0.0) Requires-Dist:
-types-requests (>=2.30.0.0,<3.0.0.0) Requires-Dist: urllib3 (<2.0) Requires-
-Dist: validators (>=0.20.0,<0.21.0) Project-URL: Documentation, https://
+Requires-Dist: click Requires-Dist: dicttoxml (>=1.7.16,<2.0.0) Requires-Dist:
+jsonschema (>=4.17.3,<5.0.0) Requires-Dist: minilog Requires-Dist: pymdown-
+extensions (>=10.0.1,<11.0.0) Requires-Dist: types-requests
+(>=2.30.0.0,<3.0.0.0) Requires-Dist: urllib3 (<2.0) Requires-Dist: validators
+(>=0.20.0,<0.21.0) Project-URL: Documentation, https://
 pyfairdatatools.readthedocs.io Project-URL: Repository, https://github.com/AI-
 READI/pyfairdatatools Description-Content-Type: text/markdown
                                     [logo]
                          ****** pyfairdatatools ******
                 Python package for the FAIR tools of fairhub.io
 
     [contributors] [stars] [open_issues] [license] [Curated_with_FAIRshare]
```

