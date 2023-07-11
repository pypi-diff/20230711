# Comparing `tmp/cookiecutter-2.2.2.tar.gz` & `tmp/cookiecutter-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cookiecutter-2.2.2.tar", last modified: Mon Jul 10 13:27:00 2023, max compression
+gzip compressed data, was "cookiecutter-2.2.3.tar", last modified: Tue Jul 11 15:59:13 2023, max compression
```

## Comparing `cookiecutter-2.2.2.tar` & `cookiecutter-2.2.3.tar`

### file list

```diff
@@ -1,341 +1,342 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.938853 cookiecutter-2.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    72932 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12922 2023-07-10 13:27:00.938853 cookiecutter-2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.886849 cookiecutter-2.2.2/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/cookiecutter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/cookiecutter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/cookiecutter/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/cookiecutter/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/cookiecutter/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/cookiecutter/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/cookiecutter/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/cookiecutter/find.py
--rw-r--r--   0 runner    (1001) docker     (123)    15885 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/cookiecutter/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/cookiecutter/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/cookiecutter/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/cookiecutter/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/cookiecutter/prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/cookiecutter/replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/cookiecutter/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/cookiecutter/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/cookiecutter/vcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/cookiecutter/zipfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.886849 cookiecutter-2.2.2/cookiecutter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12922 2023-07-10 13:27:00.000000 cookiecutter-2.2.2/cookiecutter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11578 2023-07-10 13:27:00.000000 cookiecutter-2.2.2/cookiecutter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 13:27:00.000000 cookiecutter-2.2.2/cookiecutter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-10 13:27:00.000000 cookiecutter-2.2.2/cookiecutter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 13:27:00.000000 cookiecutter-2.2.2/cookiecutter.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-10 13:27:00.000000 cookiecutter-2.2.2/cookiecutter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-10 13:27:00.000000 cookiecutter-2.2.2/cookiecutter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-10 13:27:00.938853 cookiecutter-2.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.898850 cookiecutter-2.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.898850 cookiecutter-2.2.2/tests/fake-nested-templates/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/fake-nested-templates/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.898850 cookiecutter-2.2.2/tests/fake-nested-templates/fake-project/
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/fake-nested-templates/fake-project/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.898850 cookiecutter-2.2.2/tests/fake-repo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/fake-repo/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.902850 cookiecutter-2.2.2/tests/fake-repo/fake-project/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/fake-repo/fake-project/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.898850 cookiecutter-2.2.2/tests/fake-repo-bad/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/fake-repo-bad/no-project-in-here.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.898850 cookiecutter-2.2.2/tests/fake-repo-bad-json/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/fake-repo-bad-json/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.898850 cookiecutter-2.2.2/tests/fake-repo-bad-json/{{cookiecutter.repo_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/fake-repo-bad-json/{{cookiecutter.repo_name}}/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.898850 cookiecutter-2.2.2/tests/fake-repo-dict/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/fake-repo-dict/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.898850 cookiecutter-2.2.2/tests/fake-repo-dict/{{cookiecutter.project_slug}}/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/fake-repo-dict/{{cookiecutter.project_slug}}/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.858847 cookiecutter-2.2.2/tests/fake-repo-dir/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.898850 cookiecutter-2.2.2/tests/fake-repo-dir/my-dir/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/fake-repo-dir/my-dir/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.898850 cookiecutter-2.2.2/tests/fake-repo-dir/my-dir/{{cookiecutter.repo_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/fake-repo-dir/my-dir/{{cookiecutter.repo_name}}/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.898850 cookiecutter-2.2.2/tests/fake-repo-pre/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/fake-repo-pre/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.898850 cookiecutter-2.2.2/tests/fake-repo-pre/{{cookiecutter.repo_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/fake-repo-pre/{{cookiecutter.repo_name}}/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.898850 cookiecutter-2.2.2/tests/fake-repo-pre2/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/fake-repo-pre2/cookiecutter.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/fake-repo-pre2/whatever.some.thing
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.902850 cookiecutter-2.2.2/tests/fake-repo-pre2/{{cookiecutter.repo_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/fake-repo-pre2/{{cookiecutter.repo_name}}/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.902850 cookiecutter-2.2.2/tests/fake-repo-tmpl/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/fake-repo-tmpl/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.902850 cookiecutter-2.2.2/tests/fake-repo-tmpl/{{cookiecutter.repo_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/fake-repo-tmpl/{{cookiecutter.repo_name}}/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.902850 cookiecutter-2.2.2/tests/fake-repo-tmpl-_cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/fake-repo-tmpl-_cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.902850 cookiecutter-2.2.2/tests/fake-repo-tmpl-_cookiecutter/{{cookiecutter.repo_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/fake-repo-tmpl-_cookiecutter/{{cookiecutter.repo_name}}/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.906851 cookiecutter-2.2.2/tests/files/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/files/bad-zip-file.zip
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/files/empty.zip
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/files/fake-repo-tmpl.zip
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/files/not-a-repo.zip
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/files/protected-fake-repo-tmpl.zip
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/files/syntax_error.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/files/unicode.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/files/{% if cookiecutter.generate_file == 'y' %}cheese.txt{% endif %}
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/files/{{cookiecutter.generate_file}}.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/files/{{cookiecutter.generate_file}}_crlf_newlines.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/files/{{cookiecutter.generate_file}}_lf_newlines.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/files/{{cookiecutter.jsonify_file}}.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/files/{{cookiecutter.random_string_file}}.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.862847 cookiecutter-2.2.2/tests/hooks-abort-render/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.906851 cookiecutter-2.2.2/tests/hooks-abort-render/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/hooks-abort-render/hooks/post_gen_project.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/hooks-abort-render/hooks/pre_gen_project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.906851 cookiecutter-2.2.2/tests/hooks-abort-render/{{cookiecutter.repo_dir}}/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/hooks-abort-render/{{cookiecutter.repo_dir}}/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.906851 cookiecutter-2.2.2/tests/replay/
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/replay/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/replay/test_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/replay/test_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/replay/test_replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.910851 cookiecutter-2.2.2/tests/repository/
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/repository/test_abbreviation_expansion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/repository/test_determine_repo_dir_clones_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/repository/test_determine_repo_dir_finds_existing_cookiecutter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/repository/test_determine_repo_dir_finds_subdirectories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/repository/test_determine_repository_should_use_local_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/repository/test_is_repo_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/repository/test_repository_has_cookiecutter_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.910851 cookiecutter-2.2.2/tests/test-config/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-config/config-expand-user.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-config/config-expand-vars.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-config/invalid-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-config/valid-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-config/valid-partial-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.862847 cookiecutter-2.2.2/tests/test-extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.910851 cookiecutter-2.2.2/tests/test-extensions/custom-extension-post/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-extensions/custom-extension-post/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.910851 cookiecutter-2.2.2/tests/test-extensions/custom-extension-post/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-extensions/custom-extension-post/hooks/post_gen_project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.910851 cookiecutter-2.2.2/tests/test-extensions/custom-extension-post/{{cookiecutter.project_slug}}/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-extensions/custom-extension-post/{{cookiecutter.project_slug}}/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.910851 cookiecutter-2.2.2/tests/test-extensions/custom-extension-pre/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-extensions/custom-extension-pre/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.910851 cookiecutter-2.2.2/tests/test-extensions/custom-extension-pre/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-extensions/custom-extension-pre/hooks/pre_gen_project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.910851 cookiecutter-2.2.2/tests/test-extensions/custom-extension-pre/{{cookiecutter.project_slug}}/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-extensions/custom-extension-pre/{{cookiecutter.project_slug}}/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.910851 cookiecutter-2.2.2/tests/test-extensions/default/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-extensions/default/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.914851 cookiecutter-2.2.2/tests/test-extensions/default/{{cookiecutter.project_slug}}/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-extensions/default/{{cookiecutter.project_slug}}/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-extensions/default/{{cookiecutter.project_slug}}/id
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.914851 cookiecutter-2.2.2/tests/test-extensions/hello_extension/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-extensions/hello_extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-extensions/hello_extension/hello_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.914851 cookiecutter-2.2.2/tests/test-extensions/local_extension/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-extensions/local_extension/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.914851 cookiecutter-2.2.2/tests/test-extensions/local_extension/local_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-extensions/local_extension/local_extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-extensions/local_extension/local_extensions/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.914851 cookiecutter-2.2.2/tests/test-extensions/local_extension/{{cookiecutter.project_slug}}/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-extensions/local_extension/{{cookiecutter.project_slug}}/HISTORY.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.914851 cookiecutter-2.2.2/tests/test-extensions/unknown/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-extensions/unknown/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.914851 cookiecutter-2.2.2/tests/test-extensions/unknown/{{cookiecutter.project_slug}}/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-extensions/unknown/{{cookiecutter.project_slug}}/HISTORY.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.866847 cookiecutter-2.2.2/tests/test-generate-binaries/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.914851 cookiecutter-2.2.2/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/
--rw-r--r--   0 runner    (1001) docker     (123)    15364 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/readme.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    18116 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/some_font.otf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.918852 cookiecutter-2.2.2/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/
--rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/readme.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    18116 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/some_font.otf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.918852 cookiecutter-2.2.2/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.918852 cookiecutter-2.2.2/tests/test-generate-context/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-context/choices_template.json
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-context/invalid-syntax.json
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-context/nested_dict.json
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-context/non_ascii.json
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-context/test.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.866847 cookiecutter-2.2.2/tests/test-generate-copy-without-render/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.922852 cookiecutter-2.2.2/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.922852 cookiecutter-2.2.2/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/rendered/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/rendered/not_rendered.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.922852 cookiecutter-2.2.2/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-not-rendered/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-not-rendered/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.922852 cookiecutter-2.2.2/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.866847 cookiecutter-2.2.2/tests/test-generate-copy-without-render-override/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.918852 cookiecutter-2.2.2/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.918852 cookiecutter-2.2.2/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/rendered/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/rendered/not_rendered.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.918852 cookiecutter-2.2.2/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-not-rendered/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-not-rendered/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.922852 cookiecutter-2.2.2/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/README.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.870848 cookiecutter-2.2.2/tests/test-generate-files/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.926852 cookiecutter-2.2.2/tests/test-generate-files/input{{cookiecutter.food}}/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-files/input{{cookiecutter.food}}/simple-with-conditions.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-files/input{{cookiecutter.food}}/simple-with-newline-crlf.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-files/input{{cookiecutter.food}}/simple-with-newline.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-files/input{{cookiecutter.food}}/simple.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.922852 cookiecutter-2.2.2/tests/test-generate-files-line-end/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-files-line-end/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.922852 cookiecutter-2.2.2/tests/test-generate-files-line-end/{{cookiecutter.test_name}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.922852 cookiecutter-2.2.2/tests/test-generate-files-line-end/{{cookiecutter.test_name}}/folder/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-files-line-end/{{cookiecutter.test_name}}/folder/in_folder.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-files-line-end/{{cookiecutter.test_name}}/something.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.922852 cookiecutter-2.2.2/tests/test-generate-files-line-end/{{cookiecutter.test_name}}/{{cookiecutter.folder_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-files-line-end/{{cookiecutter.test_name}}/{{cookiecutter.folder_name}}/{{cookiecutter.filename}}.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.866847 cookiecutter-2.2.2/tests/test-generate-files-nontemplated/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.922852 cookiecutter-2.2.2/tests/test-generate-files-nontemplated/input/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-files-nontemplated/input/simple.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.870848 cookiecutter-2.2.2/tests/test-generate-files-permissions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.922852 cookiecutter-2.2.2/tests/test-generate-files-permissions/input{{cookiecutter.permissions}}/
--rwxr-xr-x   0 runner    (1001) docker     (123)       32 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-files-permissions/input{{cookiecutter.permissions}}/script.sh
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-generate-files-permissions/input{{cookiecutter.permissions}}/simple.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.926852 cookiecutter-2.2.2/tests/test-output-folder/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-output-folder/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.926852 cookiecutter-2.2.2/tests/test-output-folder/{{cookiecutter.test_name}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.926852 cookiecutter-2.2.2/tests/test-output-folder/{{cookiecutter.test_name}}/folder/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-output-folder/{{cookiecutter.test_name}}/folder/in_folder.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-output-folder/{{cookiecutter.test_name}}/something.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.926852 cookiecutter-2.2.2/tests/test-output-folder/{{cookiecutter.test_name}}/{{cookiecutter.folder_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-output-folder/{{cookiecutter.test_name}}/{{cookiecutter.folder_name}}/{{cookiecutter.filename}}.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.870848 cookiecutter-2.2.2/tests/test-pyhooks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.926852 cookiecutter-2.2.2/tests/test-pyhooks/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-pyhooks/hooks/post_gen_project.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-pyhooks/hooks/pre_gen_project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.926852 cookiecutter-2.2.2/tests/test-pyhooks/input{{cookiecutter.pyhooks}}/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-pyhooks/input{{cookiecutter.pyhooks}}/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.870848 cookiecutter-2.2.2/tests/test-pyshellhooks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.930853 cookiecutter-2.2.2/tests/test-pyshellhooks/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-pyshellhooks/hooks/post_gen_project.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       65 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-pyshellhooks/hooks/post_gen_project.sh
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-pyshellhooks/hooks/pre_gen_project.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       64 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-pyshellhooks/hooks/pre_gen_project.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.930853 cookiecutter-2.2.2/tests/test-pyshellhooks/input{{pyshellhooks}}/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-pyshellhooks/input{{pyshellhooks}}/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.930853 cookiecutter-2.2.2/tests/test-replay/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-replay/cookiedozer_load.json
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-replay/invalid_replay.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.870848 cookiecutter-2.2.2/tests/test-shellhooks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.930853 cookiecutter-2.2.2/tests/test-shellhooks/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (123)       65 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-shellhooks/hooks/post_gen_project.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)       63 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-shellhooks/hooks/pre_gen_project.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.930853 cookiecutter-2.2.2/tests/test-shellhooks/input{{cookiecutter.shellhooks}}/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-shellhooks/input{{cookiecutter.shellhooks}}/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.870848 cookiecutter-2.2.2/tests/test-shellhooks-empty/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.930853 cookiecutter-2.2.2/tests/test-shellhooks-empty/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-shellhooks-empty/hooks/pre_gen_project.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.930853 cookiecutter-2.2.2/tests/test-shellhooks-empty/input{{cookiecutter.shellhooks}}/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-shellhooks-empty/input{{cookiecutter.shellhooks}}/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.870848 cookiecutter-2.2.2/tests/test-shellhooks-win/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.930853 cookiecutter-2.2.2/tests/test-shellhooks-win/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-shellhooks-win/hooks/post_gen_project.bat
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-shellhooks-win/hooks/pre_gen_project.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.930853 cookiecutter-2.2.2/tests/test-shellhooks-win/input{{cookiecutter.shellhooks}}/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-shellhooks-win/input{{cookiecutter.shellhooks}}/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.874848 cookiecutter-2.2.2/tests/test-templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.930853 cookiecutter-2.2.2/tests/test-templates/extends/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-templates/extends/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.930853 cookiecutter-2.2.2/tests/test-templates/extends/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-templates/extends/templates/base-requirements.jinja
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-templates/extends/templates/click-requirements.jinja
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-templates/extends/templates/pytest-requirements.jinja
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.934853 cookiecutter-2.2.2/tests/test-templates/extends/{{cookiecutter.project_slug}}/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-templates/extends/{{cookiecutter.project_slug}}/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.934853 cookiecutter-2.2.2/tests/test-templates/include/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-templates/include/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.934853 cookiecutter-2.2.2/tests/test-templates/include/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-templates/include/templates/click-requirements.jinja
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-templates/include/templates/pytest-requirements.jinja
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.934853 cookiecutter-2.2.2/tests/test-templates/include/{{cookiecutter.project_slug}}/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-templates/include/{{cookiecutter.project_slug}}/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.934853 cookiecutter-2.2.2/tests/test-templates/no-templates/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-templates/no-templates/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.934853 cookiecutter-2.2.2/tests/test-templates/no-templates/{{cookiecutter.project_slug}}/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-templates/no-templates/{{cookiecutter.project_slug}}/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.934853 cookiecutter-2.2.2/tests/test-templates/super/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-templates/super/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.934853 cookiecutter-2.2.2/tests/test-templates/super/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-templates/super/templates/base-requirements.jinja
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-templates/super/templates/click-requirements.jinja
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-templates/super/templates/pytest-requirements.jinja
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.934853 cookiecutter-2.2.2/tests/test-templates/super/{{cookiecutter.project_slug}}/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test-templates/super/{{cookiecutter.project_slug}}/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_abort_generate_on_hook_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    20303 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_cookiecutter_invocation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_cookiecutter_local_no_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_cookiecutter_local_with_input.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_cookiecutter_nested_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_custom_extensions_in_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_default_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_find.py
--rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_generate_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_generate_copy_without_render.py
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_generate_copy_without_render_override.py
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_generate_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    15950 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_generate_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     8141 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_generate_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_get_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_get_user_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10502 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_output_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_preferred_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_read_repo_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_read_user_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_read_user_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_read_user_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_read_user_yes_no.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_repo_not_found.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_specify_output_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_time_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.874848 cookiecutter-2.2.2/tests/undefined-variable/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.874848 cookiecutter-2.2.2/tests/undefined-variable/dir-name/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.934853 cookiecutter-2.2.2/tests/undefined-variable/dir-name/{{cookiecutter.project_slug}}/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/undefined-variable/dir-name/{{cookiecutter.project_slug}}/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.934853 cookiecutter-2.2.2/tests/undefined-variable/dir-name/{{cookiecutter.project_slug}}/{{cookiecutter.foobar}}/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/undefined-variable/dir-name/{{cookiecutter.project_slug}}/{{cookiecutter.foobar}}/helloworld.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.874848 cookiecutter-2.2.2/tests/undefined-variable/file-content/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.934853 cookiecutter-2.2.2/tests/undefined-variable/file-content/{{cookiecutter.project_slug}}/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/undefined-variable/file-content/{{cookiecutter.project_slug}}/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.934853 cookiecutter-2.2.2/tests/undefined-variable/file-name/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/undefined-variable/file-name/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.934853 cookiecutter-2.2.2/tests/undefined-variable/file-name/{{cookiecutter.project_slug}}/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/undefined-variable/file-name/{{cookiecutter.project_slug}}/{{cookiecutter.foobar}}
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.938853 cookiecutter-2.2.2/tests/vcs/
--rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/vcs/test_clone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/vcs/test_identify_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/vcs/test_is_vcs_installed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 13:27:00.938853 cookiecutter-2.2.2/tests/zipfile/
--rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-07-10 13:26:49.000000 cookiecutter-2.2.2/tests/zipfile/test_unzip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.387875 cookiecutter-2.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11796 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    73635 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13155 2023-07-11 15:59:13.387875 cookiecutter-2.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11589 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.359875 cookiecutter-2.2.3/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/cookiecutter/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/cookiecutter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/cookiecutter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/cookiecutter/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/cookiecutter/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/cookiecutter/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/cookiecutter/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/cookiecutter/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/cookiecutter/find.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15885 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/cookiecutter/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/cookiecutter/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/cookiecutter/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/cookiecutter/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9736 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/cookiecutter/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/cookiecutter/replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/cookiecutter/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/cookiecutter/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/cookiecutter/vcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/cookiecutter/zipfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.359875 cookiecutter-2.2.3/cookiecutter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13155 2023-07-11 15:59:13.000000 cookiecutter-2.2.3/cookiecutter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-07-11 15:59:13.000000 cookiecutter-2.2.3/cookiecutter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:59:13.000000 cookiecutter-2.2.3/cookiecutter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-11 15:59:13.000000 cookiecutter-2.2.3/cookiecutter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:59:13.000000 cookiecutter-2.2.3/cookiecutter.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-11 15:59:13.000000 cookiecutter-2.2.3/cookiecutter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-11 15:59:13.000000 cookiecutter-2.2.3/cookiecutter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-11 15:59:13.391875 cookiecutter-2.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.363875 cookiecutter-2.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.363875 cookiecutter-2.2.3/tests/fake-nested-templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/fake-nested-templates/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.363875 cookiecutter-2.2.3/tests/fake-nested-templates/fake-project/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/fake-nested-templates/fake-project/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.363875 cookiecutter-2.2.3/tests/fake-repo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/fake-repo/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.367875 cookiecutter-2.2.3/tests/fake-repo/fake-project/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/fake-repo/fake-project/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.363875 cookiecutter-2.2.3/tests/fake-repo-bad/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/fake-repo-bad/no-project-in-here.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.363875 cookiecutter-2.2.3/tests/fake-repo-bad-json/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/fake-repo-bad-json/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.363875 cookiecutter-2.2.3/tests/fake-repo-bad-json/{{cookiecutter.repo_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/fake-repo-bad-json/{{cookiecutter.repo_name}}/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.367875 cookiecutter-2.2.3/tests/fake-repo-dict/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/fake-repo-dict/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.367875 cookiecutter-2.2.3/tests/fake-repo-dict/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/fake-repo-dict/{{cookiecutter.project_slug}}/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.347874 cookiecutter-2.2.3/tests/fake-repo-dir/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.367875 cookiecutter-2.2.3/tests/fake-repo-dir/my-dir/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/fake-repo-dir/my-dir/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.367875 cookiecutter-2.2.3/tests/fake-repo-dir/my-dir/{{cookiecutter.repo_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/fake-repo-dir/my-dir/{{cookiecutter.repo_name}}/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.367875 cookiecutter-2.2.3/tests/fake-repo-pre/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/fake-repo-pre/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.367875 cookiecutter-2.2.3/tests/fake-repo-pre/{{cookiecutter.repo_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/fake-repo-pre/{{cookiecutter.repo_name}}/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.367875 cookiecutter-2.2.3/tests/fake-repo-pre2/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/fake-repo-pre2/cookiecutter.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/fake-repo-pre2/whatever.some.thing
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.367875 cookiecutter-2.2.3/tests/fake-repo-pre2/{{cookiecutter.repo_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/fake-repo-pre2/{{cookiecutter.repo_name}}/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.367875 cookiecutter-2.2.3/tests/fake-repo-tmpl/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/fake-repo-tmpl/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.367875 cookiecutter-2.2.3/tests/fake-repo-tmpl/{{cookiecutter.repo_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/fake-repo-tmpl/{{cookiecutter.repo_name}}/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.367875 cookiecutter-2.2.3/tests/fake-repo-tmpl-_cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/fake-repo-tmpl-_cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.367875 cookiecutter-2.2.3/tests/fake-repo-tmpl-_cookiecutter/{{cookiecutter.repo_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/fake-repo-tmpl-_cookiecutter/{{cookiecutter.repo_name}}/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.371875 cookiecutter-2.2.3/tests/files/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/files/bad-zip-file.zip
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/files/empty.zip
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/files/fake-repo-tmpl.zip
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/files/not-a-repo.zip
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/files/protected-fake-repo-tmpl.zip
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/files/syntax_error.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/files/unicode.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/files/{% if cookiecutter.generate_file == 'y' %}cheese.txt{% endif %}
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/files/{{cookiecutter.generate_file}}.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/files/{{cookiecutter.generate_file}}_crlf_newlines.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/files/{{cookiecutter.generate_file}}_lf_newlines.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/files/{{cookiecutter.jsonify_file}}.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/files/{{cookiecutter.random_string_file}}.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.347874 cookiecutter-2.2.3/tests/hooks-abort-render/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.371875 cookiecutter-2.2.3/tests/hooks-abort-render/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/hooks-abort-render/hooks/post_gen_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/hooks-abort-render/hooks/pre_gen_project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.371875 cookiecutter-2.2.3/tests/hooks-abort-render/{{cookiecutter.repo_dir}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/hooks-abort-render/{{cookiecutter.repo_dir}}/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.371875 cookiecutter-2.2.3/tests/replay/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/replay/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/replay/test_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/replay/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/replay/test_replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.371875 cookiecutter-2.2.3/tests/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/repository/test_abbreviation_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/repository/test_determine_repo_dir_clones_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/repository/test_determine_repo_dir_finds_existing_cookiecutter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/repository/test_determine_repo_dir_finds_subdirectories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/repository/test_determine_repository_should_use_local_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/repository/test_is_repo_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/repository/test_repository_has_cookiecutter_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.371875 cookiecutter-2.2.3/tests/test-config/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-config/config-expand-user.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-config/config-expand-vars.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-config/invalid-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-config/valid-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-config/valid-partial-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.351875 cookiecutter-2.2.3/tests/test-extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.371875 cookiecutter-2.2.3/tests/test-extensions/custom-extension-post/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-extensions/custom-extension-post/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.371875 cookiecutter-2.2.3/tests/test-extensions/custom-extension-post/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-extensions/custom-extension-post/hooks/post_gen_project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.371875 cookiecutter-2.2.3/tests/test-extensions/custom-extension-post/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-extensions/custom-extension-post/{{cookiecutter.project_slug}}/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.371875 cookiecutter-2.2.3/tests/test-extensions/custom-extension-pre/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-extensions/custom-extension-pre/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.371875 cookiecutter-2.2.3/tests/test-extensions/custom-extension-pre/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-extensions/custom-extension-pre/hooks/pre_gen_project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.375875 cookiecutter-2.2.3/tests/test-extensions/custom-extension-pre/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-extensions/custom-extension-pre/{{cookiecutter.project_slug}}/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.375875 cookiecutter-2.2.3/tests/test-extensions/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-extensions/default/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.375875 cookiecutter-2.2.3/tests/test-extensions/default/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-extensions/default/{{cookiecutter.project_slug}}/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-extensions/default/{{cookiecutter.project_slug}}/id
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.375875 cookiecutter-2.2.3/tests/test-extensions/hello_extension/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-extensions/hello_extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-extensions/hello_extension/hello_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.375875 cookiecutter-2.2.3/tests/test-extensions/local_extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-extensions/local_extension/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.375875 cookiecutter-2.2.3/tests/test-extensions/local_extension/local_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-extensions/local_extension/local_extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-extensions/local_extension/local_extensions/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.375875 cookiecutter-2.2.3/tests/test-extensions/local_extension/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-extensions/local_extension/{{cookiecutter.project_slug}}/HISTORY.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.375875 cookiecutter-2.2.3/tests/test-extensions/unknown/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-extensions/unknown/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.375875 cookiecutter-2.2.3/tests/test-extensions/unknown/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-extensions/unknown/{{cookiecutter.project_slug}}/HISTORY.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.351875 cookiecutter-2.2.3/tests/test-generate-binaries/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.375875 cookiecutter-2.2.3/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/
+-rw-r--r--   0 runner    (1001) docker     (123)    15364 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/readme.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18116 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/some_font.otf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.375875 cookiecutter-2.2.3/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/
+-rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/readme.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18116 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/some_font.otf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.375875 cookiecutter-2.2.3/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.375875 cookiecutter-2.2.3/tests/test-generate-context/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-generate-context/choices_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-generate-context/invalid-syntax.json
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-generate-context/nested_dict.json
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-generate-context/non_ascii.json
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-generate-context/test.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.351875 cookiecutter-2.2.3/tests/test-generate-copy-without-render/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.375875 cookiecutter-2.2.3/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.379875 cookiecutter-2.2.3/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/rendered/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/rendered/not_rendered.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.379875 cookiecutter-2.2.3/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-not-rendered/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-not-rendered/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.379875 cookiecutter-2.2.3/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-generate-copy-without-render/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.351875 cookiecutter-2.2.3/tests/test-generate-copy-without-render-override/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.375875 cookiecutter-2.2.3/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.375875 cookiecutter-2.2.3/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/rendered/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/rendered/not_rendered.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.375875 cookiecutter-2.2.3/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-not-rendered/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-not-rendered/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.375875 cookiecutter-2.2.3/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-generate-copy-without-render-override/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}-rendered/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.351875 cookiecutter-2.2.3/tests/test-generate-files/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.379875 cookiecutter-2.2.3/tests/test-generate-files/input{{cookiecutter.food}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-generate-files/input{{cookiecutter.food}}/simple-with-conditions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-generate-files/input{{cookiecutter.food}}/simple-with-newline-crlf.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-generate-files/input{{cookiecutter.food}}/simple-with-newline.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-generate-files/input{{cookiecutter.food}}/simple.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.379875 cookiecutter-2.2.3/tests/test-generate-files-line-end/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-generate-files-line-end/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.379875 cookiecutter-2.2.3/tests/test-generate-files-line-end/{{cookiecutter.test_name}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.379875 cookiecutter-2.2.3/tests/test-generate-files-line-end/{{cookiecutter.test_name}}/folder/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-generate-files-line-end/{{cookiecutter.test_name}}/folder/in_folder.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-generate-files-line-end/{{cookiecutter.test_name}}/something.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.379875 cookiecutter-2.2.3/tests/test-generate-files-line-end/{{cookiecutter.test_name}}/{{cookiecutter.folder_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-generate-files-line-end/{{cookiecutter.test_name}}/{{cookiecutter.folder_name}}/{{cookiecutter.filename}}.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.351875 cookiecutter-2.2.3/tests/test-generate-files-nontemplated/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.379875 cookiecutter-2.2.3/tests/test-generate-files-nontemplated/input/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-generate-files-nontemplated/input/simple.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.351875 cookiecutter-2.2.3/tests/test-generate-files-permissions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.379875 cookiecutter-2.2.3/tests/test-generate-files-permissions/input{{cookiecutter.permissions}}/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       32 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-generate-files-permissions/input{{cookiecutter.permissions}}/script.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-generate-files-permissions/input{{cookiecutter.permissions}}/simple.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.379875 cookiecutter-2.2.3/tests/test-output-folder/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-output-folder/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.379875 cookiecutter-2.2.3/tests/test-output-folder/{{cookiecutter.test_name}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.379875 cookiecutter-2.2.3/tests/test-output-folder/{{cookiecutter.test_name}}/folder/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-output-folder/{{cookiecutter.test_name}}/folder/in_folder.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-output-folder/{{cookiecutter.test_name}}/something.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.379875 cookiecutter-2.2.3/tests/test-output-folder/{{cookiecutter.test_name}}/{{cookiecutter.folder_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-output-folder/{{cookiecutter.test_name}}/{{cookiecutter.folder_name}}/{{cookiecutter.filename}}.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.351875 cookiecutter-2.2.3/tests/test-pyhooks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.379875 cookiecutter-2.2.3/tests/test-pyhooks/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-pyhooks/hooks/post_gen_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-pyhooks/hooks/pre_gen_project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.379875 cookiecutter-2.2.3/tests/test-pyhooks/input{{cookiecutter.pyhooks}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-pyhooks/input{{cookiecutter.pyhooks}}/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.351875 cookiecutter-2.2.3/tests/test-pyshellhooks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.383875 cookiecutter-2.2.3/tests/test-pyshellhooks/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-pyshellhooks/hooks/post_gen_project.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       65 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-pyshellhooks/hooks/post_gen_project.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-pyshellhooks/hooks/pre_gen_project.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       64 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-pyshellhooks/hooks/pre_gen_project.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.383875 cookiecutter-2.2.3/tests/test-pyshellhooks/input{{pyshellhooks}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-pyshellhooks/input{{pyshellhooks}}/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.383875 cookiecutter-2.2.3/tests/test-replay/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-replay/cookiedozer_load.json
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-replay/invalid_replay.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.355875 cookiecutter-2.2.3/tests/test-shellhooks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.383875 cookiecutter-2.2.3/tests/test-shellhooks/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       65 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-shellhooks/hooks/post_gen_project.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)       63 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-shellhooks/hooks/pre_gen_project.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.383875 cookiecutter-2.2.3/tests/test-shellhooks/input{{cookiecutter.shellhooks}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-shellhooks/input{{cookiecutter.shellhooks}}/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.351875 cookiecutter-2.2.3/tests/test-shellhooks-empty/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.383875 cookiecutter-2.2.3/tests/test-shellhooks-empty/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-shellhooks-empty/hooks/pre_gen_project.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.383875 cookiecutter-2.2.3/tests/test-shellhooks-empty/input{{cookiecutter.shellhooks}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-shellhooks-empty/input{{cookiecutter.shellhooks}}/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.351875 cookiecutter-2.2.3/tests/test-shellhooks-win/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.383875 cookiecutter-2.2.3/tests/test-shellhooks-win/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-shellhooks-win/hooks/post_gen_project.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-shellhooks-win/hooks/pre_gen_project.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.383875 cookiecutter-2.2.3/tests/test-shellhooks-win/input{{cookiecutter.shellhooks}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-shellhooks-win/input{{cookiecutter.shellhooks}}/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.355875 cookiecutter-2.2.3/tests/test-templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.383875 cookiecutter-2.2.3/tests/test-templates/extends/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-templates/extends/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.383875 cookiecutter-2.2.3/tests/test-templates/extends/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-templates/extends/templates/base-requirements.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-templates/extends/templates/click-requirements.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-templates/extends/templates/pytest-requirements.jinja
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.383875 cookiecutter-2.2.3/tests/test-templates/extends/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-templates/extends/{{cookiecutter.project_slug}}/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.383875 cookiecutter-2.2.3/tests/test-templates/include/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-templates/include/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.387875 cookiecutter-2.2.3/tests/test-templates/include/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-templates/include/templates/click-requirements.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-templates/include/templates/pytest-requirements.jinja
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.387875 cookiecutter-2.2.3/tests/test-templates/include/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-templates/include/{{cookiecutter.project_slug}}/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.387875 cookiecutter-2.2.3/tests/test-templates/no-templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-templates/no-templates/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.387875 cookiecutter-2.2.3/tests/test-templates/no-templates/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-templates/no-templates/{{cookiecutter.project_slug}}/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.387875 cookiecutter-2.2.3/tests/test-templates/super/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-templates/super/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.387875 cookiecutter-2.2.3/tests/test-templates/super/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-templates/super/templates/base-requirements.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-templates/super/templates/click-requirements.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-templates/super/templates/pytest-requirements.jinja
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.387875 cookiecutter-2.2.3/tests/test-templates/super/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test-templates/super/{{cookiecutter.project_slug}}/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test_abort_generate_on_hook_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20667 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test_cookiecutter_invocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test_cookiecutter_local_no_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test_cookiecutter_local_with_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test_cookiecutter_nested_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test_custom_extensions_in_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test_default_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test_find.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test_generate_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test_generate_copy_without_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test_generate_copy_without_render_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test_generate_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15950 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test_generate_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8141 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test_generate_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test_get_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test_get_user_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10502 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test_output_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test_preferred_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20908 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test_read_repo_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test_read_user_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test_read_user_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test_read_user_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test_read_user_yes_no.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test_repo_not_found.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test_specify_output_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test_time_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.355875 cookiecutter-2.2.3/tests/undefined-variable/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.355875 cookiecutter-2.2.3/tests/undefined-variable/dir-name/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.387875 cookiecutter-2.2.3/tests/undefined-variable/dir-name/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/undefined-variable/dir-name/{{cookiecutter.project_slug}}/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.387875 cookiecutter-2.2.3/tests/undefined-variable/dir-name/{{cookiecutter.project_slug}}/{{cookiecutter.foobar}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/undefined-variable/dir-name/{{cookiecutter.project_slug}}/{{cookiecutter.foobar}}/helloworld.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.355875 cookiecutter-2.2.3/tests/undefined-variable/file-content/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.387875 cookiecutter-2.2.3/tests/undefined-variable/file-content/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/undefined-variable/file-content/{{cookiecutter.project_slug}}/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.387875 cookiecutter-2.2.3/tests/undefined-variable/file-name/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/undefined-variable/file-name/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.387875 cookiecutter-2.2.3/tests/undefined-variable/file-name/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/undefined-variable/file-name/{{cookiecutter.project_slug}}/{{cookiecutter.foobar}}
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.387875 cookiecutter-2.2.3/tests/vcs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/vcs/test_clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/vcs/test_identify_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/vcs/test_is_vcs_installed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:59:13.387875 cookiecutter-2.2.3/tests/zipfile/
+-rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-07-11 15:59:04.000000 cookiecutter-2.2.3/tests/zipfile/test_unzip.py
```

### Comparing `cookiecutter-2.2.2/AUTHORS.md` & `cookiecutter-2.2.3/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/CONTRIBUTING.md` & `cookiecutter-2.2.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/HISTORY.md` & `cookiecutter-2.2.3/HISTORY.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,34 @@
 # History
 
 History is important, but our current roadmap can be found [here](https://github.com/cookiecutter/cookiecutter/projects)
 
+## 2.2.3 (2023-07-11)
+### Changes
+
+### Minor Changes
+
+* Add support for adding human-readable labels for choices when defining multiple choices questions (#1898) @vemonet
+
+* Prompt with replay file (#1758) @w1ndblow
+
+### CI/CD and QA changes
+
+* Set cookiecutter/VERSION.txt as source of truth for version number (#1896) @ericof
+* [pre-commit.ci] pre-commit autoupdate (#1897) @pre-commit-ci
+
+### Bugfixes
+
+* Fix issue where the prompts dict was not passed for yes_no questions (#1895) @vemonet
+* Set cookiecutter/VERSION.txt as source of truth for version number (#1896) @ericof
+
+### This release is made by wonderful contributors:
+
+@ericof, @pre-commit-ci, @pre-commit-ci[bot], @vemonet and @w1ndblow
+
 ## 2.2.2 (2023-07-10)
 
 ### CI/CD and QA changes
 
 * Improve gitignore (#1889) @audreyfeldroy
 * Add warning for jinja2_time (#1890) @henryiii
```

### Comparing `cookiecutter-2.2.2/LICENSE` & `cookiecutter-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/PKG-INFO` & `cookiecutter-2.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cookiecutter
-Version: 2.2.2
+Version: 2.2.3
 Summary: A command-line utility that creates projects from project templates, e.g. creating a Python package project from a Python package project template.
 Home-page: https://github.com/cookiecutter/cookiecutter
 Author: Audrey Feldroy
 Author-email: audreyr@gmail.com
 License: BSD
 Project-URL: Documentation, https://cookiecutter.readthedocs.io
 Project-URL: Issues, https://github.com/cookiecutter/cookiecutter/issues
@@ -142,30 +142,37 @@
 - 100% of templating is done with Jinja2.
 - Both, directory names and filenames can be templated.
   For example:
 
   ```py
   {{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}.py
   ```
-- Simply define your template variables in a `cookiecutter.json` file. You can also add human-readable questions that will be prompted to the user for each variable using the `__prompts__` key.
+- Simply define your template variables in a `cookiecutter.json` file. You can also add human-readable questions and choices that will be prompted to the user for each variable using the `__prompts__` key.
   For example:
 
   ```json
   {
     "full_name": "Audrey Roy Greenfeld",
     "email": "audreyr@gmail.com",
     "project_name": "Complexity",
     "repo_name": "complexity",
     "project_short_description": "Refreshingly simple static site generator.",
     "release_date": "2013-07-10",
     "year": "2013",
     "version": "0.1.1",
+    "linting": ["ruff", "flake8", "none"],
     "__prompts__": {
       "full_name": "Provide your full name",
-      "email": "Provide your email"
+      "email": "Provide your email",
+      "linting": {
+        "__prompt__": "Which linting tool do you want to use?",
+        "ruff": "Ruff",
+        "flake8": "Flake8",
+        "none": "No linting tool"
+      }
     }
   }
   ```
 - Pre- and post-generate hooks: Python or shell scripts to run before or after generating a project.
 
 ## Available Cookiecutters
```

### Comparing `cookiecutter-2.2.2/README.md` & `cookiecutter-2.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -109,30 +109,37 @@
 - 100% of templating is done with Jinja2.
 - Both, directory names and filenames can be templated.
   For example:
 
   ```py
   {{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}.py
   ```
-- Simply define your template variables in a `cookiecutter.json` file. You can also add human-readable questions that will be prompted to the user for each variable using the `__prompts__` key.
+- Simply define your template variables in a `cookiecutter.json` file. You can also add human-readable questions and choices that will be prompted to the user for each variable using the `__prompts__` key.
   For example:
 
   ```json
   {
     "full_name": "Audrey Roy Greenfeld",
     "email": "audreyr@gmail.com",
     "project_name": "Complexity",
     "repo_name": "complexity",
     "project_short_description": "Refreshingly simple static site generator.",
     "release_date": "2013-07-10",
     "year": "2013",
     "version": "0.1.1",
+    "linting": ["ruff", "flake8", "none"],
     "__prompts__": {
       "full_name": "Provide your full name",
-      "email": "Provide your email"
+      "email": "Provide your email",
+      "linting": {
+        "__prompt__": "Which linting tool do you want to use?",
+        "ruff": "Ruff",
+        "flake8": "Flake8",
+        "none": "No linting tool"
+      }
     }
   }
   ```
 - Pre- and post-generate hooks: Python or shell scripts to run before or after generating a project.
 
 ## Available Cookiecutters
```

### Comparing `cookiecutter-2.2.2/cookiecutter/cli.py` & `cookiecutter-2.2.3/cookiecutter/cli.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/cookiecutter/config.py` & `cookiecutter-2.2.3/cookiecutter/config.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/cookiecutter/environment.py` & `cookiecutter-2.2.3/cookiecutter/environment.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/cookiecutter/exceptions.py` & `cookiecutter-2.2.3/cookiecutter/exceptions.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/cookiecutter/extensions.py` & `cookiecutter-2.2.3/cookiecutter/extensions.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/cookiecutter/find.py` & `cookiecutter-2.2.3/cookiecutter/find.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/cookiecutter/generate.py` & `cookiecutter-2.2.3/cookiecutter/generate.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/cookiecutter/hooks.py` & `cookiecutter-2.2.3/cookiecutter/hooks.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/cookiecutter/log.py` & `cookiecutter-2.2.3/cookiecutter/log.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/cookiecutter/main.py` & `cookiecutter-2.2.3/cookiecutter/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -84,36 +84,58 @@
     import_patch = _patch_import_path_for_repo(repo_dir)
 
     template_name = os.path.basename(os.path.abspath(repo_dir))
 
     if replay:
         with import_patch:
             if isinstance(replay, bool):
-                context = load(config_dict['replay_dir'], template_name)
+                context_from_replayfile = load(config_dict['replay_dir'], template_name)
             else:
                 path, template_name = os.path.split(os.path.splitext(replay)[0])
-                context = load(path, template_name)
-    else:
-        context_file = os.path.join(repo_dir, 'cookiecutter.json')
-        logger.debug('context_file is %s', context_file)
+                context_from_replayfile = load(path, template_name)
+
+    context_file = os.path.join(repo_dir, 'cookiecutter.json')
+    logger.debug('context_file is %s', context_file)
 
+    if replay:
+        context = generate_context(
+            context_file=context_file,
+            default_context=config_dict['default_context'],
+            extra_context=None,
+        )
+        logger.debug('replayfile context: %s', context_from_replayfile)
+        items_for_prompting = {
+            k: v
+            for k, v in context['cookiecutter'].items()
+            if k not in context_from_replayfile['cookiecutter'].keys()
+        }
+        context_for_prompting = {}
+        context_for_prompting['cookiecutter'] = items_for_prompting
+        logger.debug('prompting context: %s', context_for_prompting)
+    else:
         context = generate_context(
             context_file=context_file,
             default_context=config_dict['default_context'],
             extra_context=extra_context,
         )
+        context_for_prompting = context
+    # preserve the original cookiecutter options
+    # print(context['cookiecutter'])
+    context['_cookiecutter'] = {
+        k: v for k, v in context['cookiecutter'].items() if not k.startswith("_")
+    }
 
-        # preserve the original cookiecutter options
-        context['_cookiecutter'] = context['cookiecutter']
-
-        # prompt the user to manually configure at the command line.
-        # except when 'no-input' flag is set
-        with import_patch:
-            context['cookiecutter'] = prompt_for_config(context, no_input)
+    # prompt the user to manually configure at the command line.
+    # except when 'no-input' flag is set
 
+    with import_patch:
+        if context_for_prompting['cookiecutter']:
+            context['cookiecutter'].update(
+                prompt_for_config(context_for_prompting, no_input)
+            )
         if "template" in context["cookiecutter"]:
             nested_template = re.search(
                 r'\((.*?)\)', context["cookiecutter"]["template"]
             ).group(1)
             return cookiecutter(
                 template=os.path.join(template, nested_template),
                 checkout=checkout,
@@ -127,24 +149,25 @@
                 password=password,
                 directory=directory,
                 skip_if_file_exists=skip_if_file_exists,
                 accept_hooks=accept_hooks,
                 keep_project_on_failure=keep_project_on_failure,
             )
 
-        # include template dir or url in the context dict
-        context['cookiecutter']['_template'] = template
+    logger.debug('contex is %s', context)
 
-        # include repo dir or url in the context dict
-        context['cookiecutter']['_repo_dir'] = repo_dir
+    # include template dir or url in the context dict
+    context['cookiecutter']['_template'] = template
 
-        # include output+dir in the context dict
-        context['cookiecutter']['_output_dir'] = os.path.abspath(output_dir)
+    # include output+dir in the context dict
+    context['cookiecutter']['_output_dir'] = os.path.abspath(output_dir)
+    # include repo dir or url in the context dict
+    context['cookiecutter']['_repo_dir'] = repo_dir
 
-        dump(config_dict['replay_dir'], template_name, context)
+    dump(config_dict['replay_dir'], template_name, context)
 
     # Create project from local context and project template.
     with import_patch:
         result = generate_files(
             repo_dir=repo_dir,
             context=context,
             overwrite_if_exists=overwrite_if_exists,
```

### Comparing `cookiecutter-2.2.2/cookiecutter/prompt.py` & `cookiecutter-2.2.3/cookiecutter/prompt.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,22 +68,31 @@
 
     if not options:
         raise ValueError
 
     choice_map = OrderedDict((f'{i}', value) for i, value in enumerate(options, 1))
     choices = choice_map.keys()
     default = '1'
+    question = f"Select {var_name}"
+    choice_lines = ['{} - {}'.format(*c) for c in choice_map.items()]
 
-    question = (
-        prompts[var_name]
-        if prompts and var_name in prompts.keys() and prompts[var_name]
-        else f"Select {var_name}"
-    )
+    # Handle if human-readable prompt is provided
+    if prompts and var_name in prompts.keys():
+        if isinstance(prompts[var_name], str):
+            question = prompts[var_name]
+        else:
+            if "__prompt__" in prompts[var_name]:
+                question = prompts[var_name]["__prompt__"]
+            choice_lines = [
+                f"{i} - {prompts[var_name][p]}"
+                if p in prompts[var_name]
+                else f"{i} - {p}"
+                for i, p in choice_map.items()
+            ]
 
-    choice_lines = ['{} - {}'.format(*c) for c in choice_map.items()]
     prompt = '\n'.join(
         (
             f"{question}:",
             "\n".join(choice_lines),
             f"Choose from {', '.join(choices)}",
         )
     )
@@ -231,15 +240,15 @@
             elif isinstance(raw, bool):
                 # We are dealing with a boolean variable
                 if no_input:
                     cookiecutter_dict[key] = render_variable(
                         env, raw, cookiecutter_dict
                     )
                 else:
-                    cookiecutter_dict[key] = read_user_yes_no(key, raw)
+                    cookiecutter_dict[key] = read_user_yes_no(key, raw, prompts)
             elif not isinstance(raw, dict):
                 # We are dealing with a regular variable
                 val = render_variable(env, raw, cookiecutter_dict)
 
                 if not no_input:
                     val = read_user_variable(key, val, prompts)
```

### Comparing `cookiecutter-2.2.2/cookiecutter/replay.py` & `cookiecutter-2.2.3/cookiecutter/replay.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/cookiecutter/repository.py` & `cookiecutter-2.2.3/cookiecutter/repository.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/cookiecutter/utils.py` & `cookiecutter-2.2.3/cookiecutter/utils.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/cookiecutter/vcs.py` & `cookiecutter-2.2.3/cookiecutter/vcs.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/cookiecutter/zipfile.py` & `cookiecutter-2.2.3/cookiecutter/zipfile.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/cookiecutter.egg-info/PKG-INFO` & `cookiecutter-2.2.3/cookiecutter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cookiecutter
-Version: 2.2.2
+Version: 2.2.3
 Summary: A command-line utility that creates projects from project templates, e.g. creating a Python package project from a Python package project template.
 Home-page: https://github.com/cookiecutter/cookiecutter
 Author: Audrey Feldroy
 Author-email: audreyr@gmail.com
 License: BSD
 Project-URL: Documentation, https://cookiecutter.readthedocs.io
 Project-URL: Issues, https://github.com/cookiecutter/cookiecutter/issues
@@ -142,30 +142,37 @@
 - 100% of templating is done with Jinja2.
 - Both, directory names and filenames can be templated.
   For example:
 
   ```py
   {{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}/{{cookiecutter.repo_name}}.py
   ```
-- Simply define your template variables in a `cookiecutter.json` file. You can also add human-readable questions that will be prompted to the user for each variable using the `__prompts__` key.
+- Simply define your template variables in a `cookiecutter.json` file. You can also add human-readable questions and choices that will be prompted to the user for each variable using the `__prompts__` key.
   For example:
 
   ```json
   {
     "full_name": "Audrey Roy Greenfeld",
     "email": "audreyr@gmail.com",
     "project_name": "Complexity",
     "repo_name": "complexity",
     "project_short_description": "Refreshingly simple static site generator.",
     "release_date": "2013-07-10",
     "year": "2013",
     "version": "0.1.1",
+    "linting": ["ruff", "flake8", "none"],
     "__prompts__": {
       "full_name": "Provide your full name",
-      "email": "Provide your email"
+      "email": "Provide your email",
+      "linting": {
+        "__prompt__": "Which linting tool do you want to use?",
+        "ruff": "Ruff",
+        "flake8": "Flake8",
+        "none": "No linting tool"
+      }
     }
   }
   ```
 - Pre- and post-generate hooks: Python or shell scripts to run before or after generating a project.
 
 ## Available Cookiecutters
```

### Comparing `cookiecutter-2.2.2/cookiecutter.egg-info/SOURCES.txt` & `cookiecutter-2.2.3/cookiecutter.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 HISTORY.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
+cookiecutter/VERSION.txt
 cookiecutter/__init__.py
 cookiecutter/__main__.py
 cookiecutter/cli.py
 cookiecutter/config.py
 cookiecutter/environment.py
 cookiecutter/exceptions.py
 cookiecutter/extensions.py
```

### Comparing `cookiecutter-2.2.2/setup.py` & `cookiecutter-2.2.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,26 @@
 """cookiecutter distutils configuration."""
+from pathlib import Path
 from setuptools import setup
 
-version = "2.2.2"
+
+def _get_version() -> str:
+    """Read cookiecutter/VERSION.txt and return its contents."""
+    path = Path("cookiecutter").resolve()
+    version_file = path / "VERSION.txt"
+    return version_file.read_text().strip()
+
+
+version = _get_version()
+
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
+
 requirements = [
     'binaryornot>=0.4.4',
     'Jinja2>=2.7,<4.0.0',
     'click>=7.0,<9.0.0',
     'pyyaml>=5.3.1',
     'python-slugify>=4.0.0',
     'requests>=2.23.0',
```

### Comparing `cookiecutter-2.2.2/tests/conftest.py` & `cookiecutter-2.2.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/files/fake-repo-tmpl.zip` & `cookiecutter-2.2.3/tests/files/fake-repo-tmpl.zip`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/files/protected-fake-repo-tmpl.zip` & `cookiecutter-2.2.3/tests/files/protected-fake-repo-tmpl.zip`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/replay/conftest.py` & `cookiecutter-2.2.3/tests/replay/conftest.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/replay/test_dump.py` & `cookiecutter-2.2.3/tests/replay/test_dump.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/replay/test_load.py` & `cookiecutter-2.2.3/tests/replay/test_load.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/replay/test_replay.py` & `cookiecutter-2.2.3/tests/replay/test_replay.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,16 +35,16 @@
     mock_gen_files = mocker.patch('cookiecutter.main.generate_files')
     mock_replay_dump = mocker.patch('cookiecutter.main.dump')
     mock_replay_load = mocker.patch('cookiecutter.main.load')
 
     main.cookiecutter('tests/fake-repo-tmpl/', replay=True)
 
     assert not mock_prompt.called
-    assert not mock_gen_context.called
-    assert not mock_replay_dump.called
+    assert mock_gen_context.called
+    assert mock_replay_dump.called
     assert mock_replay_load.called
     assert mock_gen_files.called
 
 
 def test_main_does_not_invoke_load_but_dump(mocker):
     """Test `cookiecutter` calling correct functions on non-replay launch."""
     mock_prompt = mocker.patch('cookiecutter.main.prompt_for_config')
```

### Comparing `cookiecutter-2.2.2/tests/repository/test_abbreviation_expansion.py` & `cookiecutter-2.2.3/tests/repository/test_abbreviation_expansion.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/repository/test_determine_repo_dir_clones_repo.py` & `cookiecutter-2.2.3/tests/repository/test_determine_repo_dir_clones_repo.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/repository/test_determine_repo_dir_finds_existing_cookiecutter.py` & `cookiecutter-2.2.3/tests/repository/test_determine_repo_dir_finds_existing_cookiecutter.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/repository/test_determine_repo_dir_finds_subdirectories.py` & `cookiecutter-2.2.3/tests/repository/test_determine_repo_dir_finds_subdirectories.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/repository/test_determine_repository_should_use_local_repo.py` & `cookiecutter-2.2.3/tests/repository/test_determine_repository_should_use_local_repo.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/repository/test_is_repo_url.py` & `cookiecutter-2.2.3/tests/repository/test_is_repo_url.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/repository/test_repository_has_cookiecutter_json.py` & `cookiecutter-2.2.3/tests/repository/test_repository_has_cookiecutter_json.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/test-extensions/hello_extension/hello_extension.py` & `cookiecutter-2.2.3/tests/test-extensions/hello_extension/hello_extension.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/test-extensions/local_extension/local_extensions/main.py` & `cookiecutter-2.2.3/tests/test-extensions/local_extension/local_extensions/main.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/.DS_Store` & `cookiecutter-2.2.3/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/.DS_Store`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/logo.png` & `cookiecutter-2.2.3/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/logo.png`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/some_font.otf` & `cookiecutter-2.2.3/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/some_font.otf`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/.DS_Store` & `cookiecutter-2.2.3/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/.DS_Store`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/logo.png` & `cookiecutter-2.2.3/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/logo.png`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/some_font.otf` & `cookiecutter-2.2.3/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/some_font.otf`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/logo.png` & `cookiecutter-2.2.3/tests/test-generate-binaries/input{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/{{cookiecutter.binary_test}}/logo.png`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/test_abort_generate_on_hook_error.py` & `cookiecutter-2.2.3/tests/test_abort_generate_on_hook_error.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/test_cli.py` & `cookiecutter-2.2.3/tests/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -652,7 +652,17 @@
     assert re.search(pattern, result.output)
     # File name should be included too...for testing purposes, just test the
     # last part of the file. If we wanted to test the absolute path, we'd have
     # to do some additional work in the test which doesn't seem that needed at
     # this point.
     path = os.path.sep.join(['tests', 'fake-repo-bad-json', 'cookiecutter.json'])
     assert path in result.output
+
+
+@pytest.mark.usefixtures('remove_fake_project_dir')
+def test_prompt_when_replyfile_not_full(mocker):
+    """Test execute prompt when replayfile not full."""
+    mock_prompt = mocker.patch('cookiecutter.main.prompt_for_config')
+    cookiecutter(
+        'tests/fake-repo-pre/', replay='tests/test-replay/cookiedozer_load.json'
+    )
+    assert mock_prompt.called
```

### Comparing `cookiecutter-2.2.2/tests/test_cookiecutter_invocation.py` & `cookiecutter-2.2.3/tests/test_cookiecutter_invocation.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/test_cookiecutter_local_no_input.py` & `cookiecutter-2.2.3/tests/test_cookiecutter_local_no_input.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/test_cookiecutter_local_with_input.py` & `cookiecutter-2.2.3/tests/test_cookiecutter_local_with_input.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/test_cookiecutter_nested_templates.py` & `cookiecutter-2.2.3/tests/test_cookiecutter_nested_templates.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/test_custom_extensions_in_hooks.py` & `cookiecutter-2.2.3/tests/test_custom_extensions_in_hooks.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/test_default_extensions.py` & `cookiecutter-2.2.3/tests/test_default_extensions.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/test_environment.py` & `cookiecutter-2.2.3/tests/test_environment.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/test_exceptions.py` & `cookiecutter-2.2.3/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/test_find.py` & `cookiecutter-2.2.3/tests/test_find.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/test_generate_context.py` & `cookiecutter-2.2.3/tests/test_generate_context.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/test_generate_copy_without_render.py` & `cookiecutter-2.2.3/tests/test_generate_copy_without_render.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/test_generate_copy_without_render_override.py` & `cookiecutter-2.2.3/tests/test_generate_copy_without_render_override.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/test_generate_file.py` & `cookiecutter-2.2.3/tests/test_generate_file.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/test_generate_files.py` & `cookiecutter-2.2.3/tests/test_generate_files.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/test_generate_hooks.py` & `cookiecutter-2.2.3/tests/test_generate_hooks.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/test_get_config.py` & `cookiecutter-2.2.3/tests/test_get_config.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/test_get_user_config.py` & `cookiecutter-2.2.3/tests/test_get_user_config.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/test_hooks.py` & `cookiecutter-2.2.3/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/test_log.py` & `cookiecutter-2.2.3/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/test_main.py` & `cookiecutter-2.2.3/tests/test_main.py`

 * *Files 9% similar despite different names*

```diff
@@ -70,14 +70,17 @@
 
     Change the current working directory temporarily to 'tests/fake-repo-tmpl'
     for this test and call cookiecutter with '.' for the target template.
     """
     monkeypatch.chdir('tests/fake-repo-tmpl')
 
     mock_replay_load = mocker.patch('cookiecutter.main.load')
+    mocker.patch('cookiecutter.main.generate_context').return_value = {
+        'cookiecutter': {}
+    }
     mocker.patch('cookiecutter.main.generate_files')
 
     cookiecutter(
         '.',
         replay=True,
         config_file=user_config_file,
     )
@@ -89,14 +92,17 @@
 
 
 def test_custom_replay_file(monkeypatch, mocker, user_config_file):
     """Check that reply.load is called with the custom replay_file."""
     monkeypatch.chdir('tests/fake-repo-tmpl')
 
     mock_replay_load = mocker.patch('cookiecutter.main.load')
+    mocker.patch('cookiecutter.main.generate_context').return_value = {
+        'cookiecutter': {}
+    }
     mocker.patch('cookiecutter.main.generate_files')
 
     cookiecutter(
         '.',
         replay='./custom-replay-file',
         config_file=user_config_file,
     )
```

### Comparing `cookiecutter-2.2.2/tests/test_output_folder.py` & `cookiecutter-2.2.3/tests/test_output_folder.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/test_preferred_encoding.py` & `cookiecutter-2.2.3/tests/test_preferred_encoding.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/test_prompt.py` & `cookiecutter-2.2.3/tests/test_prompt.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Tests for `cookiecutter.prompt` module."""
 import platform
 from collections import OrderedDict
 
+import click
 import pytest
 
 from cookiecutter import prompt, exceptions, environment
 
 
 @pytest.fixture(autouse=True)
 def patch_readline_on_win(monkeypatch):
@@ -118,14 +119,56 @@
             'cookiecutter.prompt.read_user_choice',
             lambda var, default, prompts: default,
         )
 
         cookiecutter_dict = prompt.prompt_for_config(context)
         assert cookiecutter_dict == context['cookiecutter']
 
+    @pytest.mark.parametrize(
+        'context',
+        [
+            {
+                'cookiecutter': {
+                    'full_name': 'Your Name',
+                    'check': ['yes', 'no'],
+                    '__prompts__': {
+                        'check': 'Checking',
+                    },
+                }
+            },
+            {
+                'cookiecutter': {
+                    'full_name': 'Your Name',
+                    'check': ['yes', 'no'],
+                    '__prompts__': {
+                        'full_name': 'Name please',
+                        'check': {'__prompt__': 'Checking', 'yes': 'Yes', 'no': 'No'},
+                    },
+                }
+            },
+            {
+                'cookiecutter': {
+                    'full_name': 'Your Name',
+                    'check': ['yes', 'no'],
+                    '__prompts__': {
+                        'full_name': 'Name please',
+                        'check': {'no': 'No'},
+                    },
+                }
+            },
+        ],
+    )
+    def test_prompt_for_config_with_human_choices(self, monkeypatch, context):
+        """Test prompts when human-readable labels for user choices."""
+        runner = click.testing.CliRunner()
+        with runner.isolation(input="\n\n\n"):
+            cookiecutter_dict = prompt.prompt_for_config(context)
+
+        assert dict(cookiecutter_dict) == {'full_name': 'Your Name', 'check': 'yes'}
+
     def test_prompt_for_config_dict(self, monkeypatch):
         """Verify `prompt_for_config` call `read_user_variable` on dict request."""
         monkeypatch.setattr(
             'cookiecutter.prompt.read_user_dict',
             lambda var, default, prompts: {"key": "value", "integer": 37},
         )
         context = {'cookiecutter': {'details': {}}}
@@ -476,15 +519,15 @@
         read_user_variable = mocker.patch('cookiecutter.prompt.read_user_variable')
 
         context = {'cookiecutter': {'run_as_docker': run_as_docker}}
 
         cookiecutter_dict = prompt.prompt_for_config(context)
 
         assert not read_user_variable.called
-        read_user_yes_no.assert_called_once_with('run_as_docker', run_as_docker)
+        read_user_yes_no.assert_called_once_with('run_as_docker', run_as_docker, {})
         assert cookiecutter_dict == {'run_as_docker': run_as_docker}
 
     def test_boolean_parameter_no_input(self):
         """Verify boolean parameter sent to prompt for config with no input."""
         context = {
             'cookiecutter': {
                 'run_as_docker': True,
```

### Comparing `cookiecutter-2.2.2/tests/test_read_user_choice.py` & `cookiecutter-2.2.3/tests/test_read_user_choice.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/test_read_user_dict.py` & `cookiecutter-2.2.3/tests/test_read_user_dict.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/test_read_user_yes_no.py` & `cookiecutter-2.2.3/tests/test_read_user_yes_no.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/test_specify_output_dir.py` & `cookiecutter-2.2.3/tests/test_specify_output_dir.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/test_templates.py` & `cookiecutter-2.2.3/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/test_time_extension.py` & `cookiecutter-2.2.3/tests/test_time_extension.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/test_utils.py` & `cookiecutter-2.2.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/vcs/test_clone.py` & `cookiecutter-2.2.3/tests/vcs/test_clone.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/vcs/test_identify_repo.py` & `cookiecutter-2.2.3/tests/vcs/test_identify_repo.py`

 * *Files identical despite different names*

### Comparing `cookiecutter-2.2.2/tests/zipfile/test_unzip.py` & `cookiecutter-2.2.3/tests/zipfile/test_unzip.py`

 * *Files identical despite different names*

