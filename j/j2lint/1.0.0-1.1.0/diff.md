# Comparing `tmp/j2lint-1.0.0.tar.gz` & `tmp/j2lint-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "j2lint-1.0.0.tar", last modified: Fri Jul 29 14:29:19 2022, max compression
+gzip compressed data, was "j2lint-1.1.0.tar", last modified: Tue Jul 11 09:18:31 2023, max compression
```

## Comparing `j2lint-1.0.0.tar` & `j2lint-1.1.0.tar`

### file list

```diff
@@ -1,41 +1,45 @@
-drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2022-07-29 14:29:19.201206 j2lint-1.0.0/
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     1072 2022-05-31 13:51:10.000000 j2lint-1.0.0/LICENSE
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     8207 2022-07-29 14:29:19.201365 j2lint-1.0.0/PKG-INFO
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     6056 2022-07-29 14:19:10.000000 j2lint-1.0.0/README.md
-drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2022-07-29 14:29:19.182366 j2lint-1.0.0/j2lint/
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)      217 2022-07-29 14:19:43.000000 j2lint-1.0.0/j2lint/__init__.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)      325 2022-06-30 14:57:06.000000 j2lint-1.0.0/j2lint/__main__.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     8155 2022-07-29 14:00:29.000000 j2lint-1.0.0/j2lint/cli.py
-drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2022-07-29 14:29:19.191054 j2lint-1.0.0/j2lint/linter/
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)        0 2022-05-31 13:51:10.000000 j2lint-1.0.0/j2lint/linter/__init__.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     3372 2022-07-29 14:19:10.000000 j2lint-1.0.0/j2lint/linter/collection.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     1538 2022-07-28 15:27:55.000000 j2lint-1.0.0/j2lint/linter/error.py
-drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2022-07-29 14:29:19.194522 j2lint-1.0.0/j2lint/linter/indenter/
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)        0 2022-05-31 13:51:10.000000 j2lint-1.0.0/j2lint/linter/indenter/__init__.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     7178 2022-07-29 14:19:10.000000 j2lint-1.0.0/j2lint/linter/indenter/node.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)      824 2022-06-30 14:57:06.000000 j2lint-1.0.0/j2lint/linter/indenter/statement.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     3047 2022-07-28 15:27:55.000000 j2lint-1.0.0/j2lint/linter/rule.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     2304 2022-07-28 15:27:55.000000 j2lint-1.0.0/j2lint/linter/runner.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)      773 2022-07-29 14:01:28.000000 j2lint-1.0.0/j2lint/logger.py
-drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2022-07-29 14:29:19.200934 j2lint-1.0.0/j2lint/rules/
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)        0 2022-05-31 13:51:10.000000 j2lint-1.0.0/j2lint/rules/__init__.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     2305 2022-06-30 14:57:06.000000 j2lint-1.0.0/j2lint/rules/jinja_operator_has_spaces_rule.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)      953 2022-07-29 14:19:10.000000 j2lint-1.0.0/j2lint/rules/jinja_statement_delimiter_rule.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)      977 2022-06-30 14:57:06.000000 j2lint-1.0.0/j2lint/rules/jinja_statement_has_spaces_rule.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     1897 2022-07-07 14:55:37.000000 j2lint-1.0.0/j2lint/rules/jinja_template_indentation_rule.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)      770 2022-06-30 14:57:06.000000 j2lint-1.0.0/j2lint/rules/jinja_template_no_tabs_rule.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)      938 2022-06-30 14:57:06.000000 j2lint-1.0.0/j2lint/rules/jinja_template_single_statement_rule.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     1278 2022-06-30 14:57:06.000000 j2lint-1.0.0/j2lint/rules/jinja_template_syntax_error_rule.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     1071 2022-06-30 14:57:06.000000 j2lint-1.0.0/j2lint/rules/jinja_variable_has_space_rule.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     1151 2022-06-30 14:57:06.000000 j2lint-1.0.0/j2lint/rules/jinja_variable_name_case_rule.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     1205 2022-06-30 14:57:06.000000 j2lint-1.0.0/j2lint/rules/jinja_variable_name_format_rule.py
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     7654 2022-07-29 14:19:10.000000 j2lint-1.0.0/j2lint/utils.py
-drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2022-07-29 14:29:19.185496 j2lint-1.0.0/j2lint.egg-info/
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     8207 2022-07-29 14:29:19.000000 j2lint-1.0.0/j2lint.egg-info/PKG-INFO
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     1035 2022-07-29 14:29:19.000000 j2lint-1.0.0/j2lint.egg-info/SOURCES.txt
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)        1 2022-07-29 14:29:19.000000 j2lint-1.0.0/j2lint.egg-info/dependency_links.txt
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)       42 2022-07-29 14:29:19.000000 j2lint-1.0.0/j2lint.egg-info/entry_points.txt
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)       40 2022-07-29 14:29:19.000000 j2lint-1.0.0/j2lint.egg-info/requires.txt
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)        7 2022-07-29 14:29:19.000000 j2lint-1.0.0/j2lint.egg-info/top_level.txt
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)     2260 2022-07-29 14:19:25.000000 j2lint-1.0.0/pyproject.toml
--rw-r--r--   0 guillaumemulocher   (501) staff       (20)       38 2022-07-29 14:29:19.201763 j2lint-1.0.0/setup.cfg
+drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2023-07-11 09:18:31.824769 j2lint-1.1.0/
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     1072 2022-05-31 13:51:10.000000 j2lint-1.1.0/LICENSE
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     8798 2023-07-11 09:18:31.824923 j2lint-1.1.0/PKG-INFO
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     6584 2023-07-11 08:46:14.000000 j2lint-1.1.0/README.md
+drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2023-07-11 09:18:31.723482 j2lint-1.1.0/j2lint/
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)      217 2023-07-11 09:16:14.000000 j2lint-1.1.0/j2lint/__init__.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)      325 2023-01-04 15:41:25.000000 j2lint-1.1.0/j2lint/__main__.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     9202 2023-07-11 08:36:57.000000 j2lint-1.1.0/j2lint/cli.py
+drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2023-07-11 09:18:31.763541 j2lint-1.1.0/j2lint/linter/
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)        0 2022-05-31 13:51:10.000000 j2lint-1.1.0/j2lint/linter/__init__.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     5475 2023-07-11 08:36:57.000000 j2lint-1.1.0/j2lint/linter/collection.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     2133 2023-07-11 08:36:57.000000 j2lint-1.1.0/j2lint/linter/error.py
+drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2023-07-11 09:18:31.766007 j2lint-1.1.0/j2lint/linter/indenter/
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)        0 2022-05-31 13:51:10.000000 j2lint-1.1.0/j2lint/linter/indenter/__init__.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     9797 2023-04-12 15:07:04.000000 j2lint-1.1.0/j2lint/linter/indenter/node.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)      940 2023-04-12 14:40:27.000000 j2lint-1.1.0/j2lint/linter/indenter/statement.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     4806 2023-07-11 08:36:57.000000 j2lint-1.1.0/j2lint/linter/rule.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     2902 2023-04-12 14:40:27.000000 j2lint-1.1.0/j2lint/linter/runner.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)      828 2023-04-12 15:03:47.000000 j2lint-1.1.0/j2lint/logger.py
+drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2023-07-11 09:18:31.817107 j2lint-1.1.0/j2lint/rules/
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)        0 2022-05-31 13:51:10.000000 j2lint-1.1.0/j2lint/rules/__init__.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     2861 2023-07-11 08:36:57.000000 j2lint-1.1.0/j2lint/rules/jinja_operator_has_spaces_rule.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     1502 2023-07-11 08:36:57.000000 j2lint-1.1.0/j2lint/rules/jinja_statement_delimiter_rule.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     1477 2023-07-11 08:36:57.000000 j2lint-1.1.0/j2lint/rules/jinja_statement_has_spaces_rule.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     2277 2023-07-11 08:36:57.000000 j2lint-1.1.0/j2lint/rules/jinja_template_indentation_rule.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     1260 2023-07-11 08:36:57.000000 j2lint-1.1.0/j2lint/rules/jinja_template_no_tabs_rule.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     1401 2023-07-11 08:36:57.000000 j2lint-1.1.0/j2lint/rules/jinja_template_single_statement_rule.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     1632 2023-07-11 08:36:57.000000 j2lint-1.1.0/j2lint/rules/jinja_template_syntax_error_rule.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     1591 2023-07-11 08:36:57.000000 j2lint-1.1.0/j2lint/rules/jinja_variable_has_space_rule.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     1833 2023-07-11 08:36:57.000000 j2lint-1.1.0/j2lint/rules/jinja_variable_name_case_rule.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     1821 2023-07-11 08:36:57.000000 j2lint-1.1.0/j2lint/rules/jinja_variable_name_format_rule.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     8343 2023-07-11 08:36:57.000000 j2lint-1.1.0/j2lint/utils.py
+drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2023-07-11 09:18:31.747899 j2lint-1.1.0/j2lint.egg-info/
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     8798 2023-07-11 09:18:31.000000 j2lint-1.1.0/j2lint.egg-info/PKG-INFO
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     1094 2023-07-11 09:18:31.000000 j2lint-1.1.0/j2lint.egg-info/SOURCES.txt
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)        1 2023-07-11 09:18:31.000000 j2lint-1.1.0/j2lint.egg-info/dependency_links.txt
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)       42 2023-07-11 09:18:31.000000 j2lint-1.1.0/j2lint.egg-info/entry_points.txt
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)      170 2023-07-11 09:18:31.000000 j2lint-1.1.0/j2lint.egg-info/requires.txt
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)        7 2023-07-11 09:18:31.000000 j2lint-1.1.0/j2lint.egg-info/top_level.txt
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     3358 2023-07-11 09:16:14.000000 j2lint-1.1.0/pyproject.toml
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)       38 2023-07-11 09:18:31.826055 j2lint-1.1.0/setup.cfg
+drwxr-xr-x   0 guillaumemulocher   (501) staff       (20)        0 2023-07-11 09:18:31.824188 j2lint-1.1.0/tests/
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)    11832 2023-07-11 09:16:14.000000 j2lint-1.1.0/tests/test_cli.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)      999 2023-04-12 15:03:47.000000 j2lint-1.1.0/tests/test_logger.py
+-rw-r--r--   0 guillaumemulocher   (501) staff       (20)     5925 2023-03-16 09:26:14.000000 j2lint-1.1.0/tests/test_utils.py
```

### Comparing `j2lint-1.0.0/LICENSE` & `j2lint-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `j2lint-1.0.0/PKG-INFO` & `j2lint-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: j2lint
-Version: 1.0.0
+Version: 1.1.0
 Summary: Command-line utility that validates jinja2 syntax according to Arista's AVD style guide.
 Author-email: Arista Ansible Team <ansible@arista.com>
 License: MIT License
         
         Copyright (c) 2021 Arista Networks
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -35,14 +35,17 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: test
+Provides-Extra: lint
+Provides-Extra: type
 License-File: LICENSE
 
 [![GitHub license](https://badgen.net/github/license/aristanetworks/j2lint)](https://github.com/aristanetworks/j2lint/blob/devel/LICENSE)
 [![PyPI version fury.io](https://badge.fury.io/py/j2lint.svg)](https://pypi.python.org/pypi/j2lint/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/j2lint.svg)](https://pypi.python.org/pypi/j2lint/)
 [![PyPI status](https://img.shields.io/pypi/status/j2lint.svg)](https://pypi.python.org/pypi/j2lint/)
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/aristanetworks/j2lint/graphs/commit-activity)
@@ -60,23 +63,23 @@
 - Develop an extension that works with VSCode and potentially other IDEs i.e PyCharm.
 
 ## Syntax and code style issues
 
 | Code | Short Description | Description |
 |------|-------------------|-------------|
 | S0   | `jinja-syntax-error`            | Jinja2 syntax should be correct |
-| S1   | `single-space-decorator`        | A single space shall be added between Jinja2 curly brackets and a variable's name |
+| S1   | `single-space-decorator`        | A single space should be added between Jinja2 curly brackets and a variable's name |
 | S2   | `operator-enclosed-by-spaces`   | When variables are used in combination with an operator, the operator shall be enclosed by space |
-| S3   | `jinja-statements-indentation`  | Nested jinja code block shall follow next rules:<br>- All J2 statements must be enclosed by 1 space<br>- All J2 statements must be indented by 4 more spaces within jinja delimiter<br>- To close a control, end tag must have same indentation level |
-| S4   | `jinja-statements-single-space` | Jinja statement should have a single space before and after |
-| S5   | `jinja-statements-no-tabs`      | Indentation are 4 spaces and NOT tabulation |
+| S3   | `jinja-statements-indentation`  | Nested jinja code block should follow next rules:<br>- All J2 statements must be enclosed by 1 space<br>- All J2 statements must be indented by 4 more spaces within jinja delimiter<br>- To close a control, end tag must have same indentation level |
+| S4   | `jinja-statements-single-space` | Jinja statement should have at least a single space after '{%' and a single space before '%}' |
+| S5   | `jinja-statements-no-tabs`      | Indentation should not use tabulation but 4 spaces |
 | S6   | `jinja-statements-delimiter`    | Jinja statements should not have {%- or {%+ or -%} as delimiters |
 | S7   | `single-statement-per-line`     | Jinja statements should be on separate lines |
-| V1   | `jinja-variable-lower-case`     | All variables shall use lower case |
-| V2   | `jinja-variable-format`         | If variable is multi-words, underscore _ shall be used as a separator |
+| V1   | `jinja-variable-lower-case`     | All variables should use lower case |
+| V2   | `jinja-variable-format`         | If variable is multi-words, underscore `_` should be used as a separator |
 
 ## Getting Started
 
 ### Requirements
 
 Python version 3.8+
 
@@ -92,33 +95,14 @@
 
 **Install the latest development version:**
 
 ```bash
 pip3 install git+https://github.com/aristanetworks/j2lint.git
 ```
 
-### Install with Git approach
-
-1. Create a virtual environment and activate it
-
-    ```bash
-    python3 -m venv myenv
-    source myenv/bin/activate
-    ```
-
-2. Install pip, jinja2 and jinja2-linter
-
-    ```bash
-    sudo apt-get install python3-pip
-    pip3 install jinja2
-    git clone https://github.com/aristanetworks/j2lint
-    cd j2lint
-    python setup.py install
-    ```
-
 ## Running the linter
 
 ```bash
 j2lint <path-to-directory-of-templates>
 ```
 
 ### Running the linter on a specific file
@@ -163,14 +147,24 @@
 
 2. If multiple rules are to be ignored, use the --ignore option along with rule descriptions separated by space.
 
     ```bash
     j2lint <path-to-directory-of-templates> --ignore <rule_description1> <rule_desc>
     ```
 
+> **Note**
+> This runs the custom linting rules in addition to the default linting rules.
+> When using the `-i/--ignore` or `-w/--warn` options, the arguments MUST either:
+> * Be entered at the end of the CLI as in the example above
+> * Be entered as the last options before the `<path-to-directory-of-templates>`
+>   with `--` separator.  e.g.
+>   ```bash
+>   j2lint --ignore <rule_description1> <rule_desc> -- <path-to-directory-of-templates>
+>   ```
+
 3. If one or more linting rules are to be ignored only for a specific jinja template file, add a Jinja comment at the top of the file. The rule can be disabled using the short description of the rule or the id of the rule.
 
     ```jinja2
     {# j2lint: disable=S6}
 
     # OR
     {# j2lint: disable=jinja-delimiter #}
@@ -189,15 +183,15 @@
     The file name of rules should be in snake_case and the class name should be the PascalCase version of the file name. For example:
     - File name: `jinja_operator_has_spaces_rule.py`
     - Class name: `JinjaOperatorHasSpacesRule`
 
 3. Run the jinja2 linter using --rules-dir option
 
     ```bash
-    j2lint <path-to-directory-of-templates> --rules_dir <custom-rules-directory>
+    j2lint <path-to-directory-of-templates> --rules-dir <custom-rules-directory>
     ```
 
 > **Note**
 > This runs the custom linting rules in addition to the default linting rules.
 
 ### Running jinja2 linter help command
 
@@ -220,10 +214,24 @@
         rev: <release_tag/sha>
         hooks:
         - id: j2lint
     ```
 
 2. Run pre-commit -> `pre-commit run --all-files`
 
+> **Note**
+> When using `-i/--ignore` or `-w/--warn` argument in pre-commit, use the
+> following syntax
+>
+> ```bash
+> - repo: https://github.com/aristanetworks/j2lint.git
+>     rev: <release_tag/sha>
+>     hooks:
+>     - id: j2lint
+>     # Using -- to separate the end of ignore from the positional arguments
+>     # passed to j2lint
+>       args: [--ignore, S3, jinja-statements-single-space, --]
+> ```
+
 ## Acknowledgments
 
 This project is based on [salt-lint](https://github.com/warpnet/salt-lint) and [jinjalint](https://github.com/motet-a/jinjalint)
```

### Comparing `j2lint-1.0.0/README.md` & `j2lint-1.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -17,23 +17,23 @@
 - Develop an extension that works with VSCode and potentially other IDEs i.e PyCharm.
 
 ## Syntax and code style issues
 
 | Code | Short Description | Description |
 |------|-------------------|-------------|
 | S0   | `jinja-syntax-error`            | Jinja2 syntax should be correct |
-| S1   | `single-space-decorator`        | A single space shall be added between Jinja2 curly brackets and a variable's name |
+| S1   | `single-space-decorator`        | A single space should be added between Jinja2 curly brackets and a variable's name |
 | S2   | `operator-enclosed-by-spaces`   | When variables are used in combination with an operator, the operator shall be enclosed by space |
-| S3   | `jinja-statements-indentation`  | Nested jinja code block shall follow next rules:<br>- All J2 statements must be enclosed by 1 space<br>- All J2 statements must be indented by 4 more spaces within jinja delimiter<br>- To close a control, end tag must have same indentation level |
-| S4   | `jinja-statements-single-space` | Jinja statement should have a single space before and after |
-| S5   | `jinja-statements-no-tabs`      | Indentation are 4 spaces and NOT tabulation |
+| S3   | `jinja-statements-indentation`  | Nested jinja code block should follow next rules:<br>- All J2 statements must be enclosed by 1 space<br>- All J2 statements must be indented by 4 more spaces within jinja delimiter<br>- To close a control, end tag must have same indentation level |
+| S4   | `jinja-statements-single-space` | Jinja statement should have at least a single space after '{%' and a single space before '%}' |
+| S5   | `jinja-statements-no-tabs`      | Indentation should not use tabulation but 4 spaces |
 | S6   | `jinja-statements-delimiter`    | Jinja statements should not have {%- or {%+ or -%} as delimiters |
 | S7   | `single-statement-per-line`     | Jinja statements should be on separate lines |
-| V1   | `jinja-variable-lower-case`     | All variables shall use lower case |
-| V2   | `jinja-variable-format`         | If variable is multi-words, underscore _ shall be used as a separator |
+| V1   | `jinja-variable-lower-case`     | All variables should use lower case |
+| V2   | `jinja-variable-format`         | If variable is multi-words, underscore `_` should be used as a separator |
 
 ## Getting Started
 
 ### Requirements
 
 Python version 3.8+
 
@@ -49,33 +49,14 @@
 
 **Install the latest development version:**
 
 ```bash
 pip3 install git+https://github.com/aristanetworks/j2lint.git
 ```
 
-### Install with Git approach
-
-1. Create a virtual environment and activate it
-
-    ```bash
-    python3 -m venv myenv
-    source myenv/bin/activate
-    ```
-
-2. Install pip, jinja2 and jinja2-linter
-
-    ```bash
-    sudo apt-get install python3-pip
-    pip3 install jinja2
-    git clone https://github.com/aristanetworks/j2lint
-    cd j2lint
-    python setup.py install
-    ```
-
 ## Running the linter
 
 ```bash
 j2lint <path-to-directory-of-templates>
 ```
 
 ### Running the linter on a specific file
@@ -120,14 +101,24 @@
 
 2. If multiple rules are to be ignored, use the --ignore option along with rule descriptions separated by space.
 
     ```bash
     j2lint <path-to-directory-of-templates> --ignore <rule_description1> <rule_desc>
     ```
 
+> **Note**
+> This runs the custom linting rules in addition to the default linting rules.
+> When using the `-i/--ignore` or `-w/--warn` options, the arguments MUST either:
+> * Be entered at the end of the CLI as in the example above
+> * Be entered as the last options before the `<path-to-directory-of-templates>`
+>   with `--` separator.  e.g.
+>   ```bash
+>   j2lint --ignore <rule_description1> <rule_desc> -- <path-to-directory-of-templates>
+>   ```
+
 3. If one or more linting rules are to be ignored only for a specific jinja template file, add a Jinja comment at the top of the file. The rule can be disabled using the short description of the rule or the id of the rule.
 
     ```jinja2
     {# j2lint: disable=S6}
 
     # OR
     {# j2lint: disable=jinja-delimiter #}
@@ -146,15 +137,15 @@
     The file name of rules should be in snake_case and the class name should be the PascalCase version of the file name. For example:
     - File name: `jinja_operator_has_spaces_rule.py`
     - Class name: `JinjaOperatorHasSpacesRule`
 
 3. Run the jinja2 linter using --rules-dir option
 
     ```bash
-    j2lint <path-to-directory-of-templates> --rules_dir <custom-rules-directory>
+    j2lint <path-to-directory-of-templates> --rules-dir <custom-rules-directory>
     ```
 
 > **Note**
 > This runs the custom linting rules in addition to the default linting rules.
 
 ### Running jinja2 linter help command
 
@@ -177,10 +168,24 @@
         rev: <release_tag/sha>
         hooks:
         - id: j2lint
     ```
 
 2. Run pre-commit -> `pre-commit run --all-files`
 
+> **Note**
+> When using `-i/--ignore` or `-w/--warn` argument in pre-commit, use the
+> following syntax
+>
+> ```bash
+> - repo: https://github.com/aristanetworks/j2lint.git
+>     rev: <release_tag/sha>
+>     hooks:
+>     - id: j2lint
+>     # Using -- to separate the end of ignore from the positional arguments
+>     # passed to j2lint
+>       args: [--ignore, S3, jinja-statements-single-space, --]
+> ```
+
 ## Acknowledgments
 
 This project is based on [salt-lint](https://github.com/warpnet/salt-lint) and [jinjalint](https://github.com/motet-a/jinjalint)
```

### Comparing `j2lint-1.0.0/j2lint/cli.py` & `j2lint-1.1.0/j2lint/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,96 +1,150 @@
 """cli.py - Command line argument parser.
 """
-import sys
-import os
+from __future__ import annotations
+
 import argparse
+import json
 import logging
+import os
+import sys
 import tempfile
-import json
-from j2lint import NAME, VERSION, DESCRIPTION
-from j2lint.linter.collection import RulesCollection
-from j2lint.linter.runner import Runner
-from j2lint.utils import get_files
-from j2lint.logger import logger, add_handler
-
-RULES_DIR = os.path.dirname(os.path.realpath(__file__)) + "/rules"
-IGNORE_RULES = WARN_RULES = ['jinja-syntax-error',
-                             'single-space-decorator',
-                             'operator-enclosed-by-spaces',
-                             'jinja-statements-single-space',
-                             'jinja-statements-indentation',
-                             'jinja-statements-no-tabs',
-                             'single-statement-per-line',
-                             'jinja-statements-delimiter',
-                             'jinja-variable-lower-case',
-                             'jinja-variable-format',
-                             'S0', 'S1', 'S2', 'S3', 'S4',
-                             'S5', 'S6', 'S7', 'V1', 'V2'
-                             ]
 
+from rich.console import Console
+from rich.tree import Tree
+
+from . import DESCRIPTION, NAME, VERSION
+from .linter.collection import DEFAULT_RULE_DIR, RulesCollection
+from .linter.error import LinterError
+from .linter.runner import Runner
+from .logger import add_handler, logger
+from .utils import get_files
+
+IGNORE_RULES = WARN_RULES = [
+    "jinja-syntax-error",
+    "single-space-decorator",
+    "operator-enclosed-by-spaces",
+    "jinja-statements-single-space",
+    "jinja-statements-indentation",
+    "jinja-statements-no-tabs",
+    "single-statement-per-line",
+    "jinja-statements-delimiter",
+    "jinja-variable-lower-case",
+    "jinja-variable-format",
+    "S0",
+    "S1",
+    "S2",
+    "S3",
+    "S4",
+    "S5",
+    "S6",
+    "S7",
+    "V1",
+    "V2",
+]
+
+CONSOLE = Console()
 
-def create_parser():
+
+def create_parser() -> argparse.ArgumentParser:
     """Initializes a new argument parser object
 
     Returns:
-        Object: Argument parser object
+        ArgumentParser: Argument parser object
     """
     parser = argparse.ArgumentParser(prog=NAME, description=DESCRIPTION)
 
-    parser.add_argument(dest='files', metavar='FILE', nargs='*', default=[],
-                        help='files or directories to lint')
-    parser.add_argument('-i', '--ignore', nargs='*',
-                        choices=IGNORE_RULES, default=[], help='rules to ignore')
-    parser.add_argument('-w', '--warn', nargs='*',
-                        choices=WARN_RULES, default=[], help='rules to warn')
-    parser.add_argument('-l', '--list', default=False,
-                        action='store_true', help='list of lint rules')
-    parser.add_argument('-r', '--rules_dir', dest='rules_dir', action='append',
-                        default=[RULES_DIR], help='rules directory')
-    parser.add_argument('-v', '--verbose', default=False,
-                        action='store_true', help='verbose output for lint issues')
-    parser.add_argument('-d', '--debug', default=False,
-                        action='store_true', help='enable debug logs')
-    parser.add_argument('-j', '--json', default=False,
-                        action='store_true', help='enable JSON output')
-    parser.add_argument('-s', '--stdin', default=False,
-                        action='store_true', help='accept template from STDIN')
-    parser.add_argument('--log', default=False,
-                        action='store_true', help='enable logging')
-    parser.add_argument('--version', default=False,
-                        action='store_true', help='Version of j2lint')
-    parser.add_argument('-o', '--stdout', default=False,
-                        action='store_true', help='stdout logging')
+    parser.add_argument(
+        dest="files",
+        metavar="FILE",
+        nargs="*",
+        default=[],
+        help="files or directories to lint",
+    )
+    parser.add_argument(
+        "-l", "--list", default=False, action="store_true", help="list of lint rules"
+    )
+    parser.add_argument(
+        "-r",
+        "--rules_dir",
+        dest="rules_dir",
+        action="append",
+        default=[DEFAULT_RULE_DIR],
+        help="rules directory",
+    )
+    parser.add_argument(
+        "-v",
+        "--verbose",
+        default=False,
+        action="store_true",
+        help="verbose output for lint issues",
+    )
+    parser.add_argument(
+        "-d", "--debug", default=False, action="store_true", help="enable debug logs"
+    )
+    parser.add_argument(
+        "-j", "--json", default=False, action="store_true", help="enable JSON output"
+    )
+    parser.add_argument(
+        "-s",
+        "--stdin",
+        default=False,
+        action="store_true",
+        help="accept template from STDIN",
+    )
+    parser.add_argument(
+        "--log", default=False, action="store_true", help="enable logging"
+    )
+    parser.add_argument(
+        "--version", default=False, action="store_true", help="Version of j2lint"
+    )
+    parser.add_argument(
+        "-o", "--stdout", default=False, action="store_true", help="stdout logging"
+    )
+    parser.add_argument(
+        "-i",
+        "--ignore",
+        nargs="*",
+        choices=IGNORE_RULES,
+        default=[],
+        help="rules to ignore, use `--` after this option to enter FILES",
+    )
+    parser.add_argument(
+        "-w",
+        "--warn",
+        nargs="*",
+        choices=WARN_RULES,
+        default=[],
+        help="rules to warn, use `--` after this option to enter FILES",
+    )
 
     return parser
 
 
-def sort_issues(issues):
+def sort_issues(issues: list[LinterError]) -> list[LinterError]:
     """Sorted list of issues
 
     Args:
         issues (list): list of issue dictionaries
 
     Returns:
         list: list of sorted issue dictionaries
     """
     issues.sort(
-        key=lambda issue: (
-            issue.filename,
-            issue.line_number,
-            issue.rule.id
-        )
+        key=lambda issue: (issue.filename, issue.line_number, issue.rule.rule_id)
     )
     return issues
 
 
-def get_linting_issues(file_or_dir_names, collection, checked_files):
-    """ checking errors and warnings """
-    lint_errors = {}
-    lint_warnings = {}
+def get_linting_issues(
+    file_or_dir_names: list[str], collection: RulesCollection, checked_files: list[str]
+) -> tuple[dict[str, list[LinterError]], dict[str, list[LinterError]]]:
+    """checking errors and warnings"""
+    lint_errors: dict[str, list[LinterError]] = {}
+    lint_warnings: dict[str, list[LinterError]] = {}
     files = get_files(file_or_dir_names)
 
     # Get linting issues
     for file_name in files:
         runner = Runner(collection, file_name, checked_files)
         if file_name not in lint_errors:
             lint_errors[file_name] = []
@@ -98,65 +152,89 @@
             lint_warnings[file_name] = []
         j2_errors, j2_warnings = runner.run()
         lint_errors[file_name].extend(sort_issues(j2_errors))
         lint_warnings[file_name].extend(sort_issues(j2_warnings))
     return lint_errors, lint_warnings
 
 
-def print_json_output(lint_errors, lint_warnings):
-    """ printing json output """
-    json_output = {'ERRORS': [], 'WARNINGS': []}
+def print_json_output(
+    lint_errors: dict[str, list[LinterError]],
+    lint_warnings: dict[str, list[LinterError]],
+) -> tuple[int, int]:
+    """printing json output"""
+    json_output: dict[str, list[str]] = {"ERRORS": [], "WARNINGS": []}
     for _, errors in lint_errors.items():
         for error in errors:
-            json_output['ERRORS'].append(json.loads(str(error.to_json())))
+            json_output["ERRORS"].append(json.loads(str(error.to_json())))
     for _, warnings in lint_warnings.items():
         for warning in warnings:
-            json_output['WARNINGS'].append(json.loads(str(warning.to_json())))
-    print(f"\n{json.dumps(json_output)}")
+            json_output["WARNINGS"].append(json.loads(str(warning.to_json())))
+    CONSOLE.print_json(f"\n{json.dumps(json_output)}")
 
-    return len(json_output['ERRORS']), len(json_output['WARNINGS'])
+    return len(json_output["ERRORS"]), len(json_output["WARNINGS"])
 
 
-def print_string_output(lint_errors, lint_warnings, verbose):
-    """ print non-json output """
-
-    def print_issues(lint_issues, issue_type):
-        print(f"\nJINJA2 LINT {issue_type}")
+def print_string_output(
+    lint_errors: dict[str, list[LinterError]],
+    lint_warnings: dict[str, list[LinterError]],
+    verbose: bool,
+) -> tuple[int, int]:
+    """print non-json output"""
+
+    def print_issues(
+        lint_issues: dict[str, list[LinterError]], issue_type: str
+    ) -> None:
+        CONSOLE.rule(f"[bold red]JINJA2 LINT {issue_type}")
         for key, issues in lint_issues.items():
             if not issues:
                 continue
-            print(f"************ File {key}")
+            tree = Tree(f"{key}")
+
             for j2_issue in issues:
-                print(f"{j2_issue.to_string(verbose)}")
+                tree.add(j2_issue.to_rich(verbose))
+            CONSOLE.print(tree)
 
     total_lint_errors = sum(len(issues) for _, issues in lint_errors.items())
-    total_lint_warnings = sum(len(issues)
-                              for _, issues in lint_warnings.items())
+    total_lint_warnings = sum(len(issues) for _, issues in lint_warnings.items())
 
     if total_lint_errors:
         print_issues(lint_errors, "ERRORS")
     if total_lint_warnings:
         print_issues(lint_warnings, "WARNINGS")
 
     if not total_lint_errors and not total_lint_warnings:
-        print("\nLinting complete. No problems found.")
+        if verbose:
+            CONSOLE.print("Linting complete. No problems found!", style="green")
     else:
-        print(f"\nJinja2 linting finished with "
-              f"{total_lint_errors} error(s) and {total_lint_warnings} warning(s)")
+        CONSOLE.print(
+            f"\nJinja2 linting finished with "
+            f"{total_lint_errors} error(s) and {total_lint_warnings} warning(s)"
+        )
 
     return total_lint_errors, total_lint_warnings
 
 
-def remove_temporary_file(stdin_filename):
-    """ Remove temporary file """
+def remove_temporary_file(stdin_filename: str) -> None:
+    """Remove temporary file"""
     if stdin_filename:
         os.unlink(stdin_filename)
 
 
-def run(args=None):
+def print_string_rules(collection: RulesCollection) -> None:
+    """Print active rules as string"""
+    CONSOLE.rule("[bold red]Rules in the Collection")
+    CONSOLE.print(collection.to_rich())
+
+
+def print_json_rules(collection: RulesCollection) -> None:
+    """Print active rules as json"""
+    CONSOLE.print_json(collection.to_json())
+
+
+def run(args: list[str] | None = None) -> int:
     """Runs jinja2 linter
 
     Args:
         args ([string], optional): Command line arguments. Defaults to None.
 
     Returns:
         int: 0 on success
@@ -169,67 +247,71 @@
 
     # Enable logs
 
     if not options.log and not options.stdout:
         logging.disable(sys.maxsize)
 
     else:
-        log_level = logging.INFO
-        if options.debug:
-            log_level = logging.DEBUG
+        log_level = logging.DEBUG if options.debug else logging.INFO
         if options.log:
             add_handler(logger, False, log_level)
         if options.stdout:
             add_handler(logger, True, log_level)
 
     logger.debug("Lint options selected %s", options)
 
     stdin_filename = None
-    file_or_dir_names = set(options.files)
-    checked_files = set()
+    file_or_dir_names: list[str] = list(set(options.files))
+    checked_files: list[str] = []
 
     if options.stdin and not sys.stdin.isatty():
-        with tempfile.NamedTemporaryFile('w', suffix='.j2', delete=False) as stdin_tmpfile:
+        with tempfile.NamedTemporaryFile(
+            "w", suffix=".j2", delete=False
+        ) as stdin_tmpfile:
             stdin_tmpfile.write(sys.stdin.read())
             stdin_filename = stdin_tmpfile.name
-            file_or_dir_names.add(stdin_filename)
+            file_or_dir_names.append(stdin_filename)
 
     # Collect the rules from the configuration
     collection = RulesCollection(options.verbose)
     for rules_dir in options.rules_dir:
-        collection.extend(RulesCollection.create_from_directory(
-            rules_dir, options.ignore, options.warn))
+        collection.extend(
+            RulesCollection.create_from_directory(
+                rules_dir, options.ignore, options.warn
+            ).rules
+        )
 
     # List lint rules
     if options.list:
-        rules = f"Jinja2 lint rules\n{collection}\n"
-        print(rules)
-        logger.debug(rules)
+        if options.json:
+            print_json_rules(collection)
+        else:
+            print_string_rules(collection)
         return 0
 
     # Version of j2lint
     if options.version:
-        print(f"Jinja2-Linter Version {VERSION}")
+        CONSOLE.print(f"Jinja2-Linter Version [bold red]{VERSION}")
         return 0
 
     # Print help message
     if not file_or_dir_names:
         parser.print_help(file=sys.stderr)
         return 1
 
-    lint_errors, lint_warnings = (
-        get_linting_issues(file_or_dir_names, collection, checked_files))
+    lint_errors, lint_warnings = get_linting_issues(
+        file_or_dir_names, collection, checked_files
+    )
 
     if options.json:
         logger.debug("JSON output enabled")
         total_lint_errors, _ = print_json_output(lint_errors, lint_warnings)
     else:
-        total_lint_errors, _ = print_string_output(lint_errors,
-                                                   lint_warnings, options.verbose)
+        total_lint_errors, _ = print_string_output(
+            lint_errors, lint_warnings, options.verbose
+        )
 
     # Remove temporary file
-    remove_temporary_file(stdin_filename)
-
-    if total_lint_errors:
-        return 2
+    if stdin_filename is not None:
+        remove_temporary_file(stdin_filename)
 
-    return 0
+    return 2 if total_lint_errors else 0
```

### Comparing `j2lint-1.0.0/j2lint/logger.py` & `j2lint-1.1.0/j2lint/logger.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 """logger.py - Creates logger object.
 """
 import logging
 from logging import handlers
-import sys
+
+from rich.logging import RichHandler
+
 JINJA2_LOG_FILE = "jinja2-linter.log"
 
-logger = logging.getLogger('')
+logger = logging.getLogger("")
 
 
-def add_handler(log, stream_handler, log_level):
-    """ defined logging handlers """
+def add_handler(log: logging.Logger, stream_handler: bool, log_level: int) -> None:
+    """defined logging handlers"""
     log_format = logging.Formatter(
-        "%(asctime)s - %(name)s - %(levelname)s - %(message)s")
+        "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
+    )
     log.setLevel(log_level)
     if not stream_handler:
         file_handler = handlers.RotatingFileHandler(
-            JINJA2_LOG_FILE, maxBytes=(1048576 * 5), backupCount=4)
+            JINJA2_LOG_FILE, maxBytes=(1048576 * 5), backupCount=4
+        )
         file_handler.setFormatter(log_format)
         log.addHandler(file_handler)
     else:
-        console_handler = logging.StreamHandler(sys.stdout)
+        console_handler = RichHandler()
         console_handler.setFormatter(log_format)
         log.addHandler(console_handler)
```

### Comparing `j2lint-1.0.0/j2lint/rules/jinja_statement_delimiter_rule.py` & `j2lint-1.1.0/j2lint/rules/jinja_statement_delimiter_rule.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,44 @@
 """jinja_statement_delimiter_rule.py - Rule class to check if jinja delimiters
                                     are wrong.
 """
 
+from __future__ import annotations
+
+from typing import Any
+
+from j2lint.linter.error import LinterError
 from j2lint.linter.rule import Rule
 from j2lint.utils import get_jinja_statements
 
 
 class JinjaStatementDelimiterRule(Rule):
     """Rule class to check if jinja delimiters are wrong."""
 
-    id = "S6"
-    short_description = "jinja-statements-delimiter"
+    rule_id = "S6"
     description = "Jinja statements should not have {%- or {%+ or -%} as delimiters"
+    short_description = "jinja-statements-delimiter"
     severity = "LOW"
 
-    def check(self, line):
+    def __init__(self, ignore: bool = False, warn: list[Any] | None = None) -> None:
+        super().__init__()
+
+    def checktext(self, filename: str, text: str) -> list[LinterError]:
+        raise NotImplementedError
+
+    def checkline(self, filename: str, line: str, line_no: int) -> list[LinterError]:
         """Checks if the given line matches the wrong delimiters
 
         Args:
             line (string): a single line from the file
 
         Returns:
-            Object: Returns True if error is found else False
+            list[LinterError]: the list of LinterError generated by this rule
         """
+        # pylint: disable=fixme
+        # TODO think about a better error message that can identify characters
         statements = get_jinja_statements(line)
-        for statement in statements:
-            if statement[3] in ["{%-", "{%+"] or statement[4] == "-%}":
-                return True
-
-        return False
+        return [
+            LinterError(line_no, line, filename, self)
+            for statement in statements
+            if statement[3] in ["{%-", "{%+"] or statement[4] == "-%}"
+        ]
```

### Comparing `j2lint-1.0.0/j2lint/rules/jinja_template_indentation_rule.py` & `j2lint-1.1.0/j2lint/rules/jinja_template_indentation_rule.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,65 @@
 """jinja_template_indentation_rule.py - Rule class to check the jinja statement
                                      indentation is correct.
 """
-from j2lint.linter.error import JinjaLinterError
+from __future__ import annotations
+
+from typing import Any
+
+from j2lint.linter.error import JinjaLinterError, LinterError
+from j2lint.linter.indenter.node import Node, NodeIndentationError
 from j2lint.linter.rule import Rule
-from j2lint.linter.indenter.node import Node
-from j2lint.utils import get_jinja_statements
 from j2lint.logger import logger
+from j2lint.utils import get_jinja_statements
 
 
 class JinjaTemplateIndentationRule(Rule):
-    """Rule class to check the jinja statement indentation is correct.
-    """
+    """Rule class to check the jinja statement indentation is correct."""
+
+    short_description = "jinja-statements-indentation"
+    rule_id = "S3"
+    description = (
+        "All J2 statements must be indented by 4 more spaces within jinja delimiter. "
+        "To close a control, end tag must have same indentation level."
+    )
+    severity = "HIGH"
 
-    id = 'S3'
-    short_description = 'jinja-statements-indentation'
-    description = ("All J2 statements must be indented by 4 more spaces within jinja delimiter. "
-                   "To close a control, end tag must have same indentation level.")
-    severity = 'HIGH'
+    def __init__(self, ignore: bool = False, warn: list[Any] | None = None) -> None:
+        super().__init__()
 
-    def checktext(self, file, text):
+    def checktext(self, filename: str, text: str) -> list[LinterError]:
         """Checks if the given text has the error
 
         Args:
             file (string): file path
             text (string): entire text content of the file
 
         Returns:
             list: Returns list of error objects
         """
-        result = []
-        errors = []
-
-        with open(file['path'], encoding="utf-8") as template:
-            text = template.read()
-            # Collect only Jinja Statements within delimiters {% and %}
-            # and ignore the other statements
-            lines = get_jinja_statements(text, indentation=True)
-
-            # Build a tree out of Jinja Statements to get the expected
-            # indentation level for each statement
-            root = Node()
-            try:
-                root.check_indentation(errors, lines, 0)
-            except (JinjaLinterError, TypeError, IndexError) as error:
-                logger.error("Indentation check failed for file %s: Error: %s",
-                             file['path'], str(error))
-            for error in errors:
-                result.append((error[0], error[1], error[2]))
+        # Collect only Jinja Statements within delimiters {% and %}
+        # and ignore the other statements
+        lines = get_jinja_statements(text, indentation=True)
+
+        # Build a tree out of Jinja Statements to get the expected
+        # indentation level for each statement
+        root = Node()
+        node_errors: list[NodeIndentationError] = []
+        try:
+            root.check_indentation(node_errors, lines, 0)
+
+        # pylint: disable=fixme
+        # TODO need to fix this index error in Node
+        except (JinjaLinterError, IndexError) as exc:
+            logger.error(
+                "Indentation check failed for file %s: Error: %s",
+                filename,
+                str(exc),
+            )
+
+        return [
+            LinterError(line_no, section, filename, self, message)
+            for line_no, section, message in node_errors
+        ]
 
-        return result
+    def checkline(self, filename: str, line: str, line_no: int) -> list[LinterError]:
+        raise NotImplementedError
```

### Comparing `j2lint-1.0.0/j2lint/rules/jinja_template_single_statement_rule.py` & `j2lint-1.1.0/j2lint/rules/jinja_template_single_statement_rule.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,43 @@
 """jinja_template_single_statement_rule.py - Rule class to check if only a single
                                          jinja statement is present on each
                                          line.
 """
+from __future__ import annotations
+
+from typing import Any
+
+from j2lint.linter.error import LinterError
 from j2lint.linter.rule import Rule
 from j2lint.utils import get_jinja_statements
 
 
 class JinjaTemplateSingleStatementRule(Rule):
     """Rule class to check if only a single jinja statement is present on each
-       line.
+    line.
     """
-    id = 'S7'
-    short_description = 'single-statement-per-line'
+
+    rule_id = "S7"
     description = "Jinja statements should be on separate lines"
-    severity = 'MEDIUM'
+    short_description = "single-statement-per-line"
+    severity = "MEDIUM"
 
-    def check(self, line):
+    def __init__(self, ignore: bool = False, warn: list[Any] | None = None) -> None:
+        super().__init__()
+
+    def checktext(self, filename: str, text: str) -> list[LinterError]:
+        raise NotImplementedError
+
+    def checkline(self, filename: str, line: str, line_no: int) -> list[LinterError]:
         """Checks if the given line matches the error regex
 
         Args:
             line (string): a single line from the file
 
         Returns:
-            Object: Returns True if error is found else False
+            list[LinterError]: the list of LinterError generated by this rule
         """
-        if len(get_jinja_statements(line)) > 1:
-            return True
-
-        return False
+        return (
+            [LinterError(line_no, line, filename, self)]
+            if len(get_jinja_statements(line)) > 1
+            else []
+        )
```

### Comparing `j2lint-1.0.0/j2lint/utils.py` & `j2lint-1.1.0/j2lint/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,152 +1,156 @@
 """utils.py - Utility functions for jinja2 linter.
 """
+from __future__ import annotations
+
 import glob
 import importlib.util
 import os
 import re
-
-from collections.abc import Iterable
+from collections.abc import Generator, Iterable
+from typing import TYPE_CHECKING, Any, Tuple
 
 from j2lint.logger import logger
 
+if TYPE_CHECKING:
+    from .linter.rule import Rule
+
 LANGUAGE_JINJA = "jinja"
 
+# Using Tuple from typing for 3.8 support
+# Statement type is a tuple
+# (line_without_delimiter, start_line, end_line, start_delimiter, end_delimiter)
+Statement = Tuple[str, int, int, str, str]
 
-def load_plugins(directory):
+
+def load_plugins(directory: str) -> list[Rule]:
     """Loads and executes all the Rule modules from the specified directory
 
     Args:
         directory (string): Loads the modules a directory
 
     Returns:
         list: List of rule classes
     """
     result = []
     file_handle = None
     for plugin_file in glob.glob(os.path.join(directory, "[A-Za-z_]*.py")):
         plugin_name = os.path.basename(plugin_file.replace(".py", ""))
         try:
             logger.debug("Loading plugin %s", plugin_name)
-            spec = importlib.util.spec_from_file_location(
-                plugin_name, plugin_file)
-            if plugin_name != "__init__":
+            spec = importlib.util.spec_from_file_location(plugin_name, plugin_file)
+            if plugin_name != "__init__" and spec is not None:
                 class_name = "".join(
                     str(name).capitalize() for name in plugin_name.split("_")
                 )
                 module = importlib.util.module_from_spec(spec)
-                spec.loader.exec_module(module)
-                obj = getattr(module, class_name)()
-                result.append(obj)
+                if spec.loader is not None:
+                    spec.loader.exec_module(module)
+                    obj = getattr(module, class_name)()
+                    result.append(obj)
         except AttributeError:
             logger.warning("Failed to load plugin %s", plugin_name)
         finally:
             if file_handle:
                 file_handle.close()
     return result
 
 
-def is_valid_file_type(file_name):
+def is_valid_file_type(file_name: str) -> bool:
     """Checks if the file is a valid Jinja file
 
     Args:
         file_name (string): file path with extension
 
     Returns:
         boolean: True if file type is correct
     """
     extension = os.path.splitext(file_name)[1].lower()
-    if extension in [".jinja", ".jinja2", ".j2"]:
-        return True
-    return False
+    return extension in [".jinja", ".jinja2", ".j2"]
 
 
-def get_file_type(file_name):
+def get_file_type(file_name: str) -> str | None:
     """Returns file type as Jinja or None
 
     Args:
         file_name (string): file path with extension
 
     Returns:
         string: jinja or None
 
     TODO: this method and the previous one are redundant
     """
-    if is_valid_file_type(file_name):
-        return LANGUAGE_JINJA
-    return None
+    return LANGUAGE_JINJA if is_valid_file_type(file_name) else None
 
 
-def get_files(file_or_dir_names):
+def get_files(file_or_dir_names: list[str]) -> list[str]:
     """Get files from a directory recursively
 
     Args:
         file_or_dir_names (list): list of directories and files
 
     Returns:
         list: list of file paths
     """
-    file_paths = []
+    file_paths: list[str] = []
 
     if not isinstance(file_or_dir_names, (list, set)):
         raise TypeError(
             f"get_files expects a list or a set and got {file_or_dir_names}"
         )
 
     for file_or_dir in file_or_dir_names:
         if os.path.isdir(file_or_dir):
             for root, _, files in os.walk(file_or_dir):
                 for file in files:
                     file_path = os.path.join(root, file)
                     if get_file_type(file_path) == LANGUAGE_JINJA:
                         file_paths.append(file_path)
-        else:
-            if get_file_type(file_or_dir) == LANGUAGE_JINJA:
-                file_paths.append(file_or_dir)
-    logger.debug("Linting directory %s: files %s",
-                 file_or_dir_names, file_paths)
+        elif get_file_type(file_or_dir) == LANGUAGE_JINJA:
+            file_paths.append(file_or_dir)
+    logger.debug("Linting directory %s: files %s", file_or_dir_names, file_paths)
     return file_paths
 
 
-def flatten(nested_list):
+def flatten(nested_list: Iterable[Any]) -> Generator[Any, Any, Any]:
     """Flattens an iterable
 
     Args:
         nested_list (list): Nested list
 
-    Yields:
-        list: flattened list
+    Returns:
+        a generator that yields the elements of each object in the nested_list
     """
     if not isinstance(nested_list, (list, tuple)):
         raise TypeError(
-            f"flatten is expecting a list or tuple and received {nested_list}")
+            f"flatten is expecting a list or tuple and received {nested_list}"
+        )
     for element in nested_list:
         if isinstance(element, Iterable) and not isinstance(element, (str, bytes)):
             yield from flatten(element)
         else:
             yield element
 
 
-def get_tuple(list_of_tuples, item):
+def get_tuple(
+    list_of_tuples: list[tuple[Any, ...]], item: Any
+) -> tuple[Any, ...] | None:
     """Checks if an item is present in any of the tuples
 
     Args:
         list_of_tuples (list): list of tuples
         item (object): single object which can be in a tuple
 
     Returns:
         [tuple]: tuple if the item exists in any of the tuples
     """
-    for entry in list_of_tuples:
-        if item in entry:
-            return entry
-    return None
+    return next((entry for entry in list_of_tuples if item in entry), None)
 
 
-def get_jinja_statements(text, indentation=False):
+def get_jinja_statements(text: str, indentation: bool = False) -> list[Statement]:
     """Gets jinja statements with {%[-/+] [-]%} delimiters
 
     The regex `regex_pattern` will return multiple groups when it matches
     Note that this is a multiline regex
 
     Args:
         text (string): multiline text to search the jinja statements in
@@ -175,91 +179,93 @@
         Found jinja statements []
         Found jinja statements []
         Found jinja statements [(' endif ', 1, 1, '{%', '%}')]
         Found jinja statements []
 
     Returns:
         [list]: list of jinja statements
+
+    # TODO - should probably return a JinjaStatement object..
     """
-    statements = []
+    statements: list[Statement] = []
     count = 0
-    regex_pattern = re.compile(
-        "(\\{%[-|+]?)((.|\n)*?)([-]?\\%})", re.MULTILINE)
+    regex_pattern = re.compile("(\\{%[-|+]?)((.|\n)*?)([-]?\\%})", re.MULTILINE)
     newline_pattern = re.compile(r"\n")
     lines = text.split("\n")
     for match in regex_pattern.finditer(text):
         count += 1
         start_line = len(newline_pattern.findall(text, 0, match.start(2))) + 1
         end_line = len(newline_pattern.findall(text, 0, match.end(2))) + 1
         if indentation and lines[start_line - 1].split()[0] not in ["{%", "{%-", "{%+"]:
             continue
+
         statements.append(
-            (match.group(2), start_line, end_line, match.group(1), match.group(4))
+            (
+                str(match.group(2)),
+                start_line,
+                end_line,
+                str(match.group(1)),
+                str(match.group(4)),
+            )
         )
     logger.debug("Found jinja statements %s", statements)
     return statements
 
 
-def delimit_jinja_statement(line, start="{%", end="%}"):
+def delimit_jinja_statement(line: str, start: str = "{%", end: str = "%}") -> str:
     """Adds end delimiters for a jinja statement
 
     Args:
         line (string): text line
 
     Returns:
         [string]: jinja statement with jinja start and end delimiters
     """
     return start + line + end
 
 
-def get_jinja_comments(text):
+def get_jinja_comments(text: str) -> list[str]:
     """Gets jinja comments
 
     Args:
         line (string): text to get jinja comments
 
     Returns:
         [list]: returns list of jinja comments
     """
-    comments = []
     regex_pattern = re.compile("(\\{#)((.|\n)*?)(\\#})", re.MULTILINE)
-    for line in regex_pattern.finditer(text):
-        comments.append(line.group(2))
-    return comments
+
+    return [line.group(2) for line in regex_pattern.finditer(text)]
 
 
-def get_jinja_variables(text):
+def get_jinja_variables(text: str) -> list[str]:
     """Gets jinja variables
 
     Args:
         line (string): text to get jinja variables
 
     Returns:
         [list]: returns list of jinja variables
     """
-    variables = []
-    regex_pattern = regex_pattern = re.compile(
-        "(\\{{)((.|\n)*?)(\\}})", re.MULTILINE)
-    for line in regex_pattern.finditer(text):
-        variables.append(line.group(2))
-    return variables
+    regex_pattern = regex_pattern = re.compile("(\\{{)((.|\n)*?)(\\}})", re.MULTILINE)
+    return [line.group(2) for line in regex_pattern.finditer(text)]
 
 
-def is_rule_disabled(text, rule):
+def is_rule_disabled(text: str, rule: Rule) -> bool:
     """Check if rule is disabled
 
     Args:
-        text (string): text to check jinja comments
-        rule (string): rule id or description
+        text (string): text to check
+        rule (Rule): Rule object
 
     Returns:
         [boolean]: True if rule is disabled
     """
     comments = get_jinja_comments(text)
     regex = re.compile(r"j2lint\s*:\s*disable\s*=\s*([\w-]+)")
     for comment in comments:
         for line in regex.finditer(comment):
             if rule.short_description == line.group(1):
                 return True
-            if rule.id == line.group(1):
+            if rule.rule_id == line.group(1):
                 return True
     return False
```

### Comparing `j2lint-1.0.0/j2lint.egg-info/PKG-INFO` & `j2lint-1.1.0/j2lint.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: j2lint
-Version: 1.0.0
+Version: 1.1.0
 Summary: Command-line utility that validates jinja2 syntax according to Arista's AVD style guide.
 Author-email: Arista Ansible Team <ansible@arista.com>
 License: MIT License
         
         Copyright (c) 2021 Arista Networks
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -35,14 +35,17 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: test
+Provides-Extra: lint
+Provides-Extra: type
 License-File: LICENSE
 
 [![GitHub license](https://badgen.net/github/license/aristanetworks/j2lint)](https://github.com/aristanetworks/j2lint/blob/devel/LICENSE)
 [![PyPI version fury.io](https://badge.fury.io/py/j2lint.svg)](https://pypi.python.org/pypi/j2lint/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/j2lint.svg)](https://pypi.python.org/pypi/j2lint/)
 [![PyPI status](https://img.shields.io/pypi/status/j2lint.svg)](https://pypi.python.org/pypi/j2lint/)
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/aristanetworks/j2lint/graphs/commit-activity)
@@ -60,23 +63,23 @@
 - Develop an extension that works with VSCode and potentially other IDEs i.e PyCharm.
 
 ## Syntax and code style issues
 
 | Code | Short Description | Description |
 |------|-------------------|-------------|
 | S0   | `jinja-syntax-error`            | Jinja2 syntax should be correct |
-| S1   | `single-space-decorator`        | A single space shall be added between Jinja2 curly brackets and a variable's name |
+| S1   | `single-space-decorator`        | A single space should be added between Jinja2 curly brackets and a variable's name |
 | S2   | `operator-enclosed-by-spaces`   | When variables are used in combination with an operator, the operator shall be enclosed by space |
-| S3   | `jinja-statements-indentation`  | Nested jinja code block shall follow next rules:<br>- All J2 statements must be enclosed by 1 space<br>- All J2 statements must be indented by 4 more spaces within jinja delimiter<br>- To close a control, end tag must have same indentation level |
-| S4   | `jinja-statements-single-space` | Jinja statement should have a single space before and after |
-| S5   | `jinja-statements-no-tabs`      | Indentation are 4 spaces and NOT tabulation |
+| S3   | `jinja-statements-indentation`  | Nested jinja code block should follow next rules:<br>- All J2 statements must be enclosed by 1 space<br>- All J2 statements must be indented by 4 more spaces within jinja delimiter<br>- To close a control, end tag must have same indentation level |
+| S4   | `jinja-statements-single-space` | Jinja statement should have at least a single space after '{%' and a single space before '%}' |
+| S5   | `jinja-statements-no-tabs`      | Indentation should not use tabulation but 4 spaces |
 | S6   | `jinja-statements-delimiter`    | Jinja statements should not have {%- or {%+ or -%} as delimiters |
 | S7   | `single-statement-per-line`     | Jinja statements should be on separate lines |
-| V1   | `jinja-variable-lower-case`     | All variables shall use lower case |
-| V2   | `jinja-variable-format`         | If variable is multi-words, underscore _ shall be used as a separator |
+| V1   | `jinja-variable-lower-case`     | All variables should use lower case |
+| V2   | `jinja-variable-format`         | If variable is multi-words, underscore `_` should be used as a separator |
 
 ## Getting Started
 
 ### Requirements
 
 Python version 3.8+
 
@@ -92,33 +95,14 @@
 
 **Install the latest development version:**
 
 ```bash
 pip3 install git+https://github.com/aristanetworks/j2lint.git
 ```
 
-### Install with Git approach
-
-1. Create a virtual environment and activate it
-
-    ```bash
-    python3 -m venv myenv
-    source myenv/bin/activate
-    ```
-
-2. Install pip, jinja2 and jinja2-linter
-
-    ```bash
-    sudo apt-get install python3-pip
-    pip3 install jinja2
-    git clone https://github.com/aristanetworks/j2lint
-    cd j2lint
-    python setup.py install
-    ```
-
 ## Running the linter
 
 ```bash
 j2lint <path-to-directory-of-templates>
 ```
 
 ### Running the linter on a specific file
@@ -163,14 +147,24 @@
 
 2. If multiple rules are to be ignored, use the --ignore option along with rule descriptions separated by space.
 
     ```bash
     j2lint <path-to-directory-of-templates> --ignore <rule_description1> <rule_desc>
     ```
 
+> **Note**
+> This runs the custom linting rules in addition to the default linting rules.
+> When using the `-i/--ignore` or `-w/--warn` options, the arguments MUST either:
+> * Be entered at the end of the CLI as in the example above
+> * Be entered as the last options before the `<path-to-directory-of-templates>`
+>   with `--` separator.  e.g.
+>   ```bash
+>   j2lint --ignore <rule_description1> <rule_desc> -- <path-to-directory-of-templates>
+>   ```
+
 3. If one or more linting rules are to be ignored only for a specific jinja template file, add a Jinja comment at the top of the file. The rule can be disabled using the short description of the rule or the id of the rule.
 
     ```jinja2
     {# j2lint: disable=S6}
 
     # OR
     {# j2lint: disable=jinja-delimiter #}
@@ -189,15 +183,15 @@
     The file name of rules should be in snake_case and the class name should be the PascalCase version of the file name. For example:
     - File name: `jinja_operator_has_spaces_rule.py`
     - Class name: `JinjaOperatorHasSpacesRule`
 
 3. Run the jinja2 linter using --rules-dir option
 
     ```bash
-    j2lint <path-to-directory-of-templates> --rules_dir <custom-rules-directory>
+    j2lint <path-to-directory-of-templates> --rules-dir <custom-rules-directory>
     ```
 
 > **Note**
 > This runs the custom linting rules in addition to the default linting rules.
 
 ### Running jinja2 linter help command
 
@@ -220,10 +214,24 @@
         rev: <release_tag/sha>
         hooks:
         - id: j2lint
     ```
 
 2. Run pre-commit -> `pre-commit run --all-files`
 
+> **Note**
+> When using `-i/--ignore` or `-w/--warn` argument in pre-commit, use the
+> following syntax
+>
+> ```bash
+> - repo: https://github.com/aristanetworks/j2lint.git
+>     rev: <release_tag/sha>
+>     hooks:
+>     - id: j2lint
+>     # Using -- to separate the end of ignore from the positional arguments
+>     # passed to j2lint
+>       args: [--ignore, S3, jinja-statements-single-space, --]
+> ```
+
 ## Acknowledgments
 
 This project is based on [salt-lint](https://github.com/warpnet/salt-lint) and [jinjalint](https://github.com/motet-a/jinjalint)
```

### Comparing `j2lint-1.0.0/j2lint.egg-info/SOURCES.txt` & `j2lint-1.1.0/j2lint.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -27,8 +27,11 @@
 j2lint/rules/jinja_statement_has_spaces_rule.py
 j2lint/rules/jinja_template_indentation_rule.py
 j2lint/rules/jinja_template_no_tabs_rule.py
 j2lint/rules/jinja_template_single_statement_rule.py
 j2lint/rules/jinja_template_syntax_error_rule.py
 j2lint/rules/jinja_variable_has_space_rule.py
 j2lint/rules/jinja_variable_name_case_rule.py
-j2lint/rules/jinja_variable_name_format_rule.py
+j2lint/rules/jinja_variable_name_format_rule.py
+tests/test_cli.py
+tests/test_logger.py
+tests/test_utils.py
```

