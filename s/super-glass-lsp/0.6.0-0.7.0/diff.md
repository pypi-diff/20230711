# Comparing `tmp/super_glass_lsp-0.6.0.tar.gz` & `tmp/super_glass_lsp-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "super_glass_lsp-0.6.0.tar", max compression
+gzip compressed data, was "super_glass_lsp-0.7.0.tar", max compression
```

## Comparing `super_glass_lsp-0.6.0.tar` & `super_glass_lsp-0.7.0.tar`

### file list

```diff
@@ -1,51 +1,55 @@
--rw-r--r--   0        0        0     7467 2022-12-06 21:05:51.138398 super_glass_lsp-0.6.0/README.md
--rw-r--r--   0        0        0     1016 2022-12-06 21:05:51.355398 super_glass_lsp-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      175 2022-12-06 20:59:46.513272 super_glass_lsp-0.6.0/super_glass_lsp/__init__.py
--rw-r--r--   0        0        0     1993 2022-12-06 21:05:49.765397 super_glass_lsp-0.6.0/super_glass_lsp/config.default.yaml
--rw-r--r--   0        0        0      594 2022-12-06 20:59:46.514272 super_glass_lsp-0.6.0/super_glass_lsp/lsp/__init__.py
--rw-r--r--   0        0        0      122 2022-12-06 20:59:46.514272 super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/__init__.py
--rw-r--r--   0        0        0     7227 2022-12-06 21:05:51.139397 super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/apps/email_client.yaml
--rw-r--r--   0        0        0     5070 2022-12-06 21:05:50.704397 super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/config_definitions.py
--rw-r--r--   0        0        0        0 2022-12-06 20:59:46.514272 super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/features/__init__.py
--rw-r--r--   0        0        0     2988 2022-12-06 20:59:46.514272 super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/features/_debounce.py
--rw-r--r--   0        0        0     7799 2022-12-06 21:05:51.139397 super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/features/_feature.py
--rw-r--r--   0        0        0     2927 2022-12-06 21:05:50.704397 super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/features/_subprocess.py
--rw-r--r--   0        0        0     2675 2022-12-06 21:05:51.139397 super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/features/completer.py
--rw-r--r--   0        0        0     6315 2022-12-06 21:05:51.139397 super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/features/diagnoser.py
--rw-r--r--   0        0        0     2015 2022-12-06 21:05:51.140398 super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/features/formatter.py
--rw-r--r--   0        0        0     2884 2022-12-06 21:05:51.140398 super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/features/goto_definition.py
--rw-r--r--   0        0        0     5582 2022-12-06 21:05:51.140398 super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/features/workspace_edit.py
--rw-r--r--   0        0        0     6002 2022-12-06 21:05:51.140398 super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/hub.py
--rw-r--r--   0        0        0        0 2022-12-06 20:59:46.514272 super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/__init__.py
--rw-r--r--   0        0        0        0 2022-12-06 21:05:49.766397 super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/e2e/__init__.py
--rwxr-xr-x   0        0        0      455 2022-12-06 21:05:50.704397 super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/e2e/_bin/himalaya
--rw-r--r--   0        0        0        0 2022-12-06 21:05:49.766397 super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/e2e/apps/__init__.py
--rw-r--r--   0        0        0     2899 2022-12-06 21:05:50.463397 super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/e2e/apps/_utils.py
--rw-r--r--   0        0        0      933 2022-12-06 21:05:50.705397 super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/e2e/apps/email_client/main_test.py
--rw-r--r--   0        0        0       71 2022-12-06 21:05:49.766397 super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/e2e/apps/email_client/workspace/.gitignore
--rw-r--r--   0        0        0     3619 2022-12-06 21:05:49.766397 super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/e2e/configs/__init__.py
--rw-r--r--   0        0        0     1173 2022-12-06 20:59:46.514272 super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/e2e/configs/black_test.py
--rw-r--r--   0        0        0     1450 2022-12-06 21:05:50.463397 super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/e2e/configs/flake8_test.py
--rw-r--r--   0        0        0      764 2022-12-06 20:59:46.514272 super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/e2e/configs/fzf_buffer_test.py
--rw-r--r--   0        0        0     1434 2022-12-06 21:05:50.463397 super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/e2e/configs/jq_test.py
--rw-r--r--   0        0        0     1482 2022-12-06 21:05:49.924397 super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/e2e/configs/markdownlint_test.py
--rw-r--r--   0        0        0     1585 2022-12-06 21:05:49.924397 super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/e2e/configs/mypy_test.py
--rw-r--r--   0        0        0       71 2022-12-06 20:59:46.515272 super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/e2e/configs/workspace/.gitignore
--rw-r--r--   0        0        0      304 2022-12-06 20:59:46.515272 super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/e2e/test_debounce_e2e.py
--rw-r--r--   0        0        0     1501 2022-12-06 20:59:46.515272 super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/e2e/test_init_config.py
--rw-r--r--   0        0        0        0 2022-12-06 20:59:46.515272 super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/units/__init__.py
--rw-r--r--   0        0        0     1154 2022-12-06 21:05:51.140398 super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/units/_utils.py
--rw-r--r--   0        0        0     1681 2022-12-06 20:59:46.515272 super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/units/test_completer.py
--rw-r--r--   0        0        0     2102 2022-12-06 21:05:50.463397 super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/units/test_config.py
--rw-r--r--   0        0        0     2854 2022-12-06 20:59:46.515272 super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/units/test_debounce.py
--rw-r--r--   0        0        0     2228 2022-12-06 20:59:46.515272 super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/units/test_diagnostics.py
--rw-r--r--   0        0        0     1490 2022-12-06 21:05:51.141398 super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/units/test_feature.py
--rw-r--r--   0        0        0     1395 2022-12-06 20:59:46.515272 super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/units/test_formatter.py
--rw-r--r--   0        0        0     1678 2022-12-06 21:05:50.274397 super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/units/test_workspace_edit.py
--rw-r--r--   0        0        0      460 2022-12-06 20:59:46.515272 super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/utils.py
--rw-r--r--   0        0        0     5029 2022-12-06 21:05:49.767397 super_glass_lsp-0.6.0/super_glass_lsp/lsp/server.py
--rw-r--r--   0        0        0     9573 2022-12-06 21:05:51.141398 super_glass_lsp-0.6.0/super_glass_lsp/lsp/setup.py
--rw-r--r--   0        0        0     1019 2022-12-06 21:05:49.924397 super_glass_lsp-0.6.0/super_glass_lsp/main.py
--rw-r--r--   0        0        0        0 2022-12-06 20:59:46.515272 super_glass_lsp-0.6.0/super_glass_lsp/py.typed
--rw-r--r--   0        0        0     9277 1970-01-01 00:00:00.000000 super_glass_lsp-0.6.0/setup.py
--rw-r--r--   0        0        0     8193 1970-01-01 00:00:00.000000 super_glass_lsp-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     7663 2023-07-10 22:44:47.368278 super_glass_lsp-0.7.0/README.md
+-rw-r--r--   0        0        0     1163 2023-07-10 22:44:47.368278 super_glass_lsp-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      175 2023-07-10 22:44:47.368278 super_glass_lsp-0.7.0/super_glass_lsp/__init__.py
+-rw-r--r--   0        0        0     2020 2023-07-10 22:44:47.368278 super_glass_lsp-0.7.0/super_glass_lsp/config.default.yaml
+-rw-r--r--   0        0        0      593 2023-07-10 22:44:47.368278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/__init__.py
+-rw-r--r--   0        0        0      122 2023-07-10 22:44:47.368278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/__init__.py
+-rw-r--r--   0        0        0     6902 2023-07-10 22:44:47.368278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/apps/email_client.yaml
+-rw-r--r--   0        0        0     5571 2023-07-10 22:44:47.368278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/config_definitions.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:44:47.368278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/features/__init__.py
+-rw-r--r--   0        0        0      995 2023-07-10 22:44:47.368278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/features/_base.py
+-rw-r--r--   0        0        0     5239 2023-07-10 22:44:47.368278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/features/_commands.py
+-rw-r--r--   0        0        0     2988 2023-07-10 22:44:47.368278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/features/_debounce.py
+-rw-r--r--   0        0        0     2582 2023-07-10 22:44:47.368278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/features/_document.py
+-rw-r--r--   0        0        0     2071 2023-07-10 22:44:47.368278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/features/_feature.py
+-rw-r--r--   0        0        0     2976 2023-07-10 22:44:47.368278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/features/_subprocess.py
+-rw-r--r--   0        0        0     2648 2023-07-10 22:44:47.368278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/features/completer.py
+-rw-r--r--   0        0        0     6061 2023-07-10 22:44:47.368278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/features/diagnoser.py
+-rw-r--r--   0        0        0     2036 2023-07-10 22:44:47.368278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/features/formatter.py
+-rw-r--r--   0        0        0     2876 2023-07-10 22:44:47.368278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/features/goto_definition.py
+-rw-r--r--   0        0        0     2438 2023-07-10 22:44:47.368278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/features/work_done_progress.py
+-rw-r--r--   0        0        0     4934 2023-07-10 22:44:47.368278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/features/workspace_edit.py
+-rw-r--r--   0        0        0     6002 2023-07-10 22:44:47.368278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/hub.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:44:47.368278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:44:47.368278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/e2e/__init__.py
+-rwxr-xr-x   0        0        0      455 2023-07-10 22:44:47.368278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/e2e/_bin/himalaya
+-rw-r--r--   0        0        0        0 2023-07-10 22:44:47.368278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/e2e/apps/__init__.py
+-rw-r--r--   0        0        0     2899 2023-07-10 22:44:47.368278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/e2e/apps/_utils.py
+-rw-r--r--   0        0        0      908 2023-07-10 22:44:47.368278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/e2e/apps/email_client/main_test.py
+-rw-r--r--   0        0        0       71 2023-07-10 22:44:47.372278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/e2e/apps/email_client/workspace/.gitignore
+-rw-r--r--   0        0        0     3619 2023-07-10 22:44:47.372278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/e2e/configs/__init__.py
+-rw-r--r--   0        0        0     1173 2023-07-10 22:44:47.372278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/e2e/configs/black_test.py
+-rw-r--r--   0        0        0     1450 2023-07-10 22:44:47.372278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/e2e/configs/flake8_test.py
+-rw-r--r--   0        0        0      766 2023-07-10 22:44:47.372278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/e2e/configs/fzf_buffer_test.py
+-rw-r--r--   0        0        0     1434 2023-07-10 22:44:47.372278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/e2e/configs/jq_test.py
+-rw-r--r--   0        0        0     1482 2023-07-10 22:44:47.372278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/e2e/configs/markdownlint_test.py
+-rw-r--r--   0        0        0     1585 2023-07-10 22:44:47.372278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/e2e/configs/mypy_test.py
+-rw-r--r--   0        0        0       71 2023-07-10 22:44:47.372278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/e2e/configs/workspace/.gitignore
+-rw-r--r--   0        0        0      304 2023-07-10 22:44:47.372278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/e2e/test_debounce_e2e.py
+-rw-r--r--   0        0        0     1501 2023-07-10 22:44:47.372278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/e2e/test_init_config.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:44:47.372278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/units/__init__.py
+-rw-r--r--   0        0        0     1239 2023-07-10 22:44:47.372278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/units/_utils.py
+-rw-r--r--   0        0        0     1690 2023-07-10 22:44:47.372278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/units/test_completer.py
+-rw-r--r--   0        0        0     2102 2023-07-10 22:44:47.372278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/units/test_config.py
+-rw-r--r--   0        0        0     3113 2023-07-10 22:44:47.372278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/units/test_debounce.py
+-rw-r--r--   0        0        0     2372 2023-07-10 22:44:47.372278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/units/test_diagnostics.py
+-rw-r--r--   0        0        0     3665 2023-07-10 22:44:47.372278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/units/test_feature.py
+-rw-r--r--   0        0        0     1402 2023-07-10 22:44:47.372278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/units/test_formatter.py
+-rw-r--r--   0        0        0     4587 2023-07-10 22:44:47.372278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/units/test_work_done_progress.py
+-rw-r--r--   0        0        0     1681 2023-07-10 22:44:47.372278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/units/test_workspace_edit.py
+-rw-r--r--   0        0        0      460 2023-07-10 22:44:47.372278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/utils.py
+-rw-r--r--   0        0        0     5078 2023-07-10 22:44:47.372278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/server.py
+-rw-r--r--   0        0        0     9573 2023-07-10 22:44:47.372278 super_glass_lsp-0.7.0/super_glass_lsp/lsp/setup.py
+-rw-r--r--   0        0        0     1019 2023-07-10 22:44:47.372278 super_glass_lsp-0.7.0/super_glass_lsp/main.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:44:47.372278 super_glass_lsp-0.7.0/super_glass_lsp/py.typed
+-rw-r--r--   0        0        0     8574 1970-01-01 00:00:00.000000 super_glass_lsp-0.7.0/PKG-INFO
```

### Comparing `super_glass_lsp-0.6.0/README.md` & `super_glass_lsp-0.7.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -63,16 +63,19 @@
       enabled: true
 ```
 
 TODO:
 * [ ] Explain all the fields and tokens for each LSP feature
 * [ ] Remember to describe the format array lines priorities
 * [ ] How to set up the debug logs. But also maybe a LSP option to get all the debug in your editor
+  * [ ] Mention the test logs too. Because the E2E tests run in a subprocess
 * [ ] Remember to advise that some diagnostic tools output on STDERR, not STDOUT
 
+* [ ] Can you have both a Super Glass app _and_ default configs?? I think at the moment you can't? (I don't think so)
+
 ## Editor Setups
 
 Because this is a generic language server, the filetype/language that the server applies to varies depending on the config you've setup. It would be a bad idea for a generic language server to tell an editor that it wants to connect with every possible filetype/language (although this can be enabled on a per tool basis with the `language_ids: ["*"]` setting). Instead, it is better that you manually inform your editor which filetypes/languages this generic server should be enabled for. How that is done is unique to each editor's config, I've tried to include examples for each one.
 
 <details>
 <summary>Neovim Lua (vanilla Neovim without `lspconfig`)</summary>
```

### Comparing `super_glass_lsp-0.6.0/pyproject.toml` & `super_glass_lsp-0.7.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 [tool.poetry]
 name = "super-glass-lsp"
-version = "0.6.0"
+version = "0.7.0"
 description = "Generic LSP to parse the output of CLI tools, linters, formatters, etc"
 authors = ["Thomas Buckley-Houston <tom@tombh.co.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "super_glass_lsp"}]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = ">=3.7,<3.12" # TODO: Is Python 3.8 ok?
 parse = "^1.19.0"
-pygls = "^0.12.2"
+pygls = "^0.13.1" # TODO: upgrade to v1
 pyyaml = "^6.0"
+pydantic = "1.10.7" # TODO: Remove when upgrading to Pygls v1
 mergedeep = "^1.3.4"
 single-source = "^0.3.0"
 psutil = "^5.9.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.3"
 flake8 = "^5.0.4"
 mypy = "^0.982"
 black = "^22.8.0"
 pytest-mock = "^3.10.0"
 pytest-lsp = "^0.1.2"
 types-pyyaml = "^6.0.12"
 pytest-timeout = "^2.1.0"
 pytest-xdist = "^3.0.2"
+pytest-rerunfailures = "^12.0"
 
 [tool.poetry.scripts]
 super-glass-lsp   = "super_glass_lsp.main:main"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `super_glass_lsp-0.6.0/super_glass_lsp/config.default.yaml` & `super_glass_lsp-0.7.0/super_glass_lsp/config.default.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     # That will allow buffer updates rather than just on-disk changes to trigger diagnostics
     command: |
       mypy \
         --no-color-output \
         --no-error-summary \
         --follow-imports=silent \
         {file}
+    use_lsp_progress: true
     piped: false
     stdout: true
     timeout: 15
     parsing:
       formats:
         - "{}:{line:d}: {severity}: {msg}"
         - "{}: {severity}: {msg}"
```

### Comparing `super_glass_lsp-0.6.0/super_glass_lsp/lsp/__init__.py` & `super_glass_lsp-0.7.0/super_glass_lsp/lsp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
     def default(o):
         if isinstance(o, enum.Enum):
             return o.value
 
         fields = {}
         for k, v in o.__dict__.items():
-
             if v is None:
                 continue
 
             # Truncate long strings - but not uris!
             if isinstance(v, str) and not k.lower().endswith("uri"):
                 v = textwrap.shorten(v, width=25)
```

### Comparing `super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/config_definitions.py` & `super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/config_definitions.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 from enum import Enum, auto
 import os
 
 from pydantic import BaseModel, Field
 
 ShellCommand = Union[str, List[str]]
 
+DEFAULT_FORMATTERS = ["{msg}"]
+
 
 class AutoName(Enum):
     def _generate_next_value_(name, start, count, last_values):
         return name
 
 
 # TODO: Rename? Because it's specific to diagnostics?
 class OutputParsingConfig(BaseModel):
     """Config for the output of `command`s run in the sub shell"""
 
     @classmethod
     def default(cls):
-        return cls(formats=["{msg}"])
+        return cls(formats=DEFAULT_FORMATTERS)
 
     formats: List[str] = Field()
     """
     Token definitions for parsing the output of the commands.
     This a Python token string that defines the components of a parsable line.
     `{msg}`, `{line:d}` and `{col:d}` are required.
     Eg; "{msg} at line {line:d}, column {col:d}"
@@ -41,26 +43,28 @@
     """All the possible features that a config block can configure"""
 
     diagnostic = auto()
     completion = auto()
     formatter = auto()
     workspace_edit = auto()
     goto_definition = auto()
+    work_done_progress = auto()
 
 
 class ConfigBasic(BaseModel):
     """Absolute minimum config that the LSP server can recieve from the client"""
 
     # TODO: I do not like this repetition. But we're going to be replacing Pydantic in
     # Pygls v1 anyway, so punting this for another day.
     enabled: bool = Field()
     lsp_feature: Optional[LSPFeature] = Field()
     language_id: Optional[str] = Field()
     root_markers: Optional[List[str]] = Field()
     command: Optional[ShellCommand] = Field()
+    use_lsp_progress: Optional[bool] = Field()
     env: Optional[Dict] = Field()
     piped: Optional[bool] = Field()
     stdout: Optional[bool] = Field()
     stderr: Optional[bool] = Field()
     timeout: Optional[int] = Field()
     debounce: Optional[int] = Field()
     parsing: Optional[OutputParsingConfig] = Field()
@@ -105,14 +109,26 @@
     """
 
     command: ShellCommand = Field("true")
     """
     The command to run, eg; `"jsonlint --strict"`
     """
 
+    use_lsp_progress: bool = Field(False)
+    """
+    Use default LSP progress notifications
+    """
+
+    # TODO: Custom progress reporting behaviour
+    # progress_config: Optional[str] = Field()
+    # """
+    # Name of config block that provides custom progress reporting behaviour.
+    # For example, the ability to use WorkspaceEdit to show a spinner in the editor.
+    # """
+
     env: Dict = Field({})
     """
     Extra environment variables to pass to the shell
     """
 
     piped: bool = Field(True)
     """
```

### Comparing `super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/features/_debounce.py` & `super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/features/_debounce.py`

 * *Files identical despite different names*

### Comparing `super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/features/_subprocess.py` & `super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/features/_subprocess.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,28 +10,32 @@
 from super_glass_lsp.lsp.custom.config_definitions import Config
 
 
 SubprocessArgs = Dict[str, Any]
 
 
 class SubprocessOutput:
-    def __init__(self, stdout: str, stderr: str):
+    def __init__(self, stdout: str, stderr: str, returncode: Optional[int]):
         self.stdout = stdout
         self.stderr = stderr
+        self.returncode = returncode
+
+    def is_non_zero_exit(self) -> bool:
+        return self.returncode is None or self.returncode > 0
 
 
 class Subprocess:
     @classmethod
     async def run(
         cls,
         server: "CustomLanguageServer",
         config: Config,
         command: str,
         input: Optional[str],
-        check: bool = False,
+        check: bool = True,
     ) -> SubprocessOutput:
         new_env = cls.update_env(config)
         try:
             server.logger.debug(f"Subprocess command: {command}")
             process = await asyncio.create_subprocess_shell(
                 command,
                 stdin=asyncio.subprocess.PIPE if input is not None else None,
@@ -40,36 +44,35 @@
                 env=new_env,
             )
             stdout, stderr = await asyncio.wait_for(
                 # TODO: Figure out the typing problem here. Is it a false negative?
                 process.communicate(input.encode() if input is not None else None),  # type: ignore
                 timeout=config.timeout,
             )
-            output = SubprocessOutput(stdout.decode(), stderr.decode())
-            server.logger.debug(f"Subprocess STDOUT: {output.stdout}")
-            server.logger.debug(f"Subprocess STDERR: {output.stderr}")
+            result = SubprocessOutput(
+                stdout.decode().strip(), stderr.decode().strip(), process.returncode
+            )
+            server.logger.debug(f"Subprocess STDOUT: {result.stdout}")
+            server.logger.debug(f"Subprocess STDERR: {result.stderr}")
         except asyncio.TimeoutError:
             message = f"Timeout: `{command}` took longer than {config.timeout} seconds"
             server.logger.warning(message)
             server.show_message(message)
             if process.returncode is None:
                 server.logger.warning(
                     f"Terminating subprocess: `{command}` (timed out)"
                 )
                 parent = psutil.Process(process.pid)
                 for child in parent.children(recursive=True):
                     child.terminate()
                 parent.terminate()
+            return result
         if process.returncode is None:
             raise Exception("Completed subprocess exited without return code")
-        if check and process.returncode > 0:
-            message = f"Subprocess error for `{config.command}`: {output.stderr}"
-            server.logger.error(message)
-            server.show_message(message)
-        return output
+        return result
 
     @classmethod
     def update_env(cls, config: Config) -> Dict:
         new_env = os.environ.copy() | config.env
         if "PYTEST_CURRENT_TEST" in os.environ:
             dir_path = os.path.dirname(os.path.realpath(__file__))
             test_binaries_path = os.path.join(dir_path, "../", "tests", "e2e", "_bin")
```

### Comparing `super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/features/completer.py` & `super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/features/completer.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 
 from pygls.lsp import (
     CompletionItem,
     CompletionList,
 )
 
 from super_glass_lsp.lsp.custom.config_definitions import LSPFeature
-from super_glass_lsp.lsp.custom.features._feature import Feature
-from super_glass_lsp.lsp.custom.features._debounce import Debounce
+from ._feature import Feature
+from ._commands import Commands
+from ._debounce import Debounce
 
 
-class Completer(Feature):
+class Completer(Feature, Commands):
     @classmethod
     async def run_all(
         cls,
         server: "CustomLanguageServer",
         text_doc_uri: str,
         cursor_position: Position,
     ) -> Optional[CompletionList]:
@@ -70,16 +71,18 @@
         self,
         word: str,
         cursor_position: Position,
     ) -> str:
         if isinstance(self.command, list):
             raise Exception("Completions do not support multiple commands")
 
-        command = self.command
-
-        # TODO: probably refactor into a list of Tuple pairs?
-        command = command.replace("{word}", word)
-        command = command.replace("{cursor_line}", str(cursor_position.line))
-        command = command.replace("{cursor_char}", str(cursor_position.character))
+        replacements = [
+            ("{word}", word),
+            ("{cursor_line}", str(cursor_position.line)),
+            ("{cursor_char}", str(cursor_position.character)),
+        ]
+        command = self.resolve_commands(replacements)
+        if isinstance(command, list):
+            raise Exception
 
         result = await self.shell(command)
         return result.stdout
```

### Comparing `super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/features/diagnoser.py` & `super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/features/diagnoser.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import typing
-from typing import TYPE_CHECKING, List, Optional, Dict
+from typing import TYPE_CHECKING, List, Optional
 
 if TYPE_CHECKING:
     from super_glass_lsp.lsp.server import CustomLanguageServer
 
 from parse import parse  # type: ignore
 
-from pygls.lsp.types import Diagnostic, Position, Range, DiagnosticSeverity, MessageType
+from pygls.lsp.types import Diagnostic, Position, Range, DiagnosticSeverity
 
 from super_glass_lsp.lsp.custom.config_definitions import (
     OutputParsingConfig,
     LSPFeature,
 )
-from super_glass_lsp.lsp.custom.features._feature import Feature
-from super_glass_lsp.lsp.custom.features._debounce import Debounce
+from ._feature import Feature
+from ._debounce import Debounce
+from ._commands import Commands
 
 
-class Diagnoser(Feature):
+class Diagnoser(Feature, Commands):
     @classmethod
     async def run_all(cls, server: "CustomLanguageServer", text_doc_uri: str) -> None:
         configs = Feature.get_configs(server, text_doc_uri, LSPFeature.diagnostic)
         for id, config in configs.items():
             diagnoser = cls(server, id, text_doc_uri)
             if not diagnoser.debouncer.is_debounced():
                 await diagnoser.run_one()
@@ -80,35 +80,25 @@
             return DiagnosticSeverity.Error
         if severity_string.startswith("w"):
             return DiagnosticSeverity.Warning
         if severity_string.startswith("i"):
             return DiagnosticSeverity.Information
         return DiagnosticSeverity.Error
 
-    def parse_line(self, line: str) -> Diagnostic:
-        if self.config.parsing is not None:
-            config = self.config.parsing
-        else:
-            # TODO: I think we're using 2 different defaults for emptpy format now?
-            config = OutputParsingConfig(**typing.cast(Dict, {"formats": ["{line}"]}))
-
+    def parse_line(self, line: str) -> Optional[Diagnostic]:
+        config = self.get_parsing_config()
         for format_string in config.formats:
             maybe_diagnostic = self.parse_line_maybe(
                 config, format_string, line
             )  # type: ignore
             if maybe_diagnostic is not None:
                 return maybe_diagnostic
 
-        summary = "Super Glass failed to parse shell output"
-        command = f"Command: `{self.config.command}`"
-        debug = f"{summary}\n{command}\nOutput: {line}"
-        self.server.logger.warning(debug)
-        self.server.show_message(debug, msg_type=MessageType.Warning)
-        # TODO: Maybe not send a diagnostic if there was an error?
-        return self.build_diagnostic_object(summary)
+        self.parsing_failed(line)
+        return None
 
     def parse_line_maybe(
         self, parsing: OutputParsingConfig, format_string: str, line: str
     ) -> Optional[Diagnostic]:
         # Most diagnostic tools seem to be 1-indexed. But the LSP spec is zero-indexed
         ZERO_INDEXING = -1
 
@@ -147,15 +137,22 @@
         return self.build_diagnostic_object(message, line_number, col_number, severity)
 
     async def run_cli_tool(self) -> str:
         if isinstance(self.command, list):
             raise Exception("Diagnostics do not support multiple commands")
 
         output = ""
-        result = await self.shell(self.command, check=False)
+        result = await self.shell(
+            self.command,
+            # By default shell output is allowed to exit with non-zero code.
+            # This seems to be the more common behaviour of formatters. Namely that
+            # they fail if formatting is needed, but nevertheless successfully output
+            # the formatted version of the file.
+            check=False,
+        )
 
         if self.config.stdout and result.stdout is not None:
             output = result.stdout
 
         if not self.config.stdout and result.stderr is not None:
             output = result.stderr
 
@@ -166,9 +163,10 @@
 
         output = await self.run_cli_tool()
         if not output:
             return diagnostics
 
         for line in output.splitlines():
             diagnostic = self.parse_line(line)
-            diagnostics.append(diagnostic)
+            if diagnostic is not None:
+                diagnostics.append(diagnostic)
         return diagnostics
```

### Comparing `super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/features/formatter.py` & `super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/features/formatter.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,21 +4,22 @@
     from super_glass_lsp.lsp.server import CustomLanguageServer
 
 from pygls.lsp.types import (
     TextEdit,
 )
 
 from super_glass_lsp.lsp.custom.config_definitions import LSPFeature
-from super_glass_lsp.lsp.custom.features._feature import Feature
-from super_glass_lsp.lsp.custom.features._debounce import Debounce
+from ._feature import Feature
+from ._debounce import Debounce
+from ._commands import Commands
 
 SuperGlassFormatResult = Optional[List[TextEdit]]
 
 
-class Formatter(Feature):
+class Formatter(Feature, Commands):
     @classmethod
     async def run_all(
         cls, server: "CustomLanguageServer", text_doc_uri: str
     ) -> SuperGlassFormatResult:
         configs = Feature.get_configs(server, text_doc_uri, LSPFeature.formatter)
 
         edit: SuperGlassFormatResult = None
@@ -41,16 +42,18 @@
             self.cache_key(),
         )
 
     async def run_one(self) -> SuperGlassFormatResult:
         if isinstance(self.command, list):
             raise Exception("Formatters do not support multiple commands")
 
-        result = await self.shell(self.command, check=False)
+        result = await self.shell(self.command)
         new_text = result.stdout
+        if result.is_non_zero_exit():
+            return None
         # TODO: update the document with the new text so that each tool
         # incrementaly applies its changes on top of the previous
         edit = self.new_text_to_textedit(new_text)
         return edit
 
     def new_text_to_textedit(self, new_text: str) -> SuperGlassFormatResult:
         return [
```

### Comparing `super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/features/goto_definition.py` & `super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/features/goto_definition.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,18 +4,23 @@
     from super_glass_lsp.lsp.server import CustomLanguageServer
 
 from parse import parse  # type: ignore
 
 from pygls.lsp.types import Position, Location
 
 from super_glass_lsp.lsp.custom.config_definitions import LSPFeature
-from super_glass_lsp.lsp.custom.features._feature import Feature
+from ._feature import Feature
+from ._commands import Commands
 
+# `uri`: File where definition is.
+# `range`: Exact character range where definition is.
+DEFAULT_FORMAT = "{uri} {start_line}:{start_char},{end_line}:{end_char}"
 
-class GotoDefinition(Feature):
+
+class GotoDefinition(Feature, Commands):
     @classmethod
     async def run_all(
         cls,
         server: "CustomLanguageServer",
         text_doc_uri: str,
         cursor_position: Position,
     ) -> Optional[List[Location]]:
@@ -29,22 +34,21 @@
             server.logger.debug(f"Running Goto Definition request for: {id}: {config}")
             location = await definer.get_location(cursor_position)
             definitions.extend(location)
 
         return definitions
 
     async def get_location(self, cursor_position: Position) -> List[Location]:
-        default_format = "{uri} {start_line}:{start_char},{end_line}:{end_char}"
         word = self.get_wordish_under_cursor(cursor_position)
         line = self.get_line_under_cursor(cursor_position)
         output = await self.run_cli_tool(line, word, cursor_position)
 
         locations = []
         for line in output.splitlines():
-            parsed = parse(default_format, output)
+            parsed = parse(DEFAULT_FORMAT, output)
             if parsed is None:
                 continue
             location = Location(
                 uri=f'file://{parsed["uri"]}',  # TODO: formalise workspace_root/file:/// usage
                 range=self.parse_range(
                     parsed["start_line"],
                     parsed["start_char"],
@@ -58,25 +62,24 @@
 
     async def run_cli_tool(
         self,
         line: str,
         word: str,
         cursor_position: Position,
     ) -> str:
-        self.server.logger.debug("!!!!!!!!!!!!!!!!!!!!!!!")
-        self.server.logger.debug(line)
-        self.server.logger.debug("!!!!!!!!!!!!!!!!!!!!!!!")
         replacements = [
             ("{line}", line),
             ("{word}", word),
             ("{cursor_line}", str(cursor_position.line)),
             ("{cursor_char}", str(cursor_position.character)),
         ]
         commands = self.resolve_commands(replacements)
 
-        await self.run_pre_commands(commands)
+        is_success = await self.run_pre_commands(commands)
+        if not is_success:
+            return ""
         if isinstance(commands, list):
             final_command = commands[-1]
         else:
             final_command = commands
         result = await self.shell(final_command)
         return result.stdout
```

### Comparing `super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/features/workspace_edit.py` & `super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/features/workspace_edit.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,44 @@
-import typing
-from typing import Optional, Dict, TYPE_CHECKING, Union
+from typing import Optional, TYPE_CHECKING, Union
 
 if TYPE_CHECKING:
     from super_glass_lsp.lsp.server import CustomLanguageServer
 
 import os
 import asyncio
 
 from parse import parse  # type: ignore
 
 from pygls.lsp.types import (
     WorkspaceEdit as WorkspaceEditRequest,
     TextDocumentEdit,
     DeleteFile,
     TextDocumentIdentifier,
-    MessageType,
     TextEdit,
 )
 
-from super_glass_lsp.lsp.custom.features._feature import Feature
+from ._feature import Feature
+from ._commands import Commands
 from super_glass_lsp.lsp.custom.config_definitions import (
     LSPFeature,
     OutputParsingConfig,
 )
 
+# `kind`: TextDocumentEdit | CreateFile | RenameFile | DeleteFile
+# `uri`: Text document URI
+# `range` (only for TextDocumentEdit): start_line,start_char,end_line,end_char
+# `text_edit`: All remaining lines
+DEFAULT_FORMATTERS = [
+    "{kind} {uri} {start_line}:{start_char},{end_line}:{end_char}\n{text_edit}",
+    "{kind} {uri} {start_line}:{start_char},{end_line}:{end_char}",
+    "{kind} {uri}",
+]
 
-class WorkspaceEdit(Feature):
+
+class WorkspaceEdit(Feature, Commands):
     @classmethod
     def start_all_daemons(
         cls,
         server: "CustomLanguageServer",
     ):
         # TODO: think about how language IDs fit into Workspace Edits
         language_id = "*"
@@ -49,80 +58,60 @@
         while True:
             await self.run_once()
             if "PYTEST_CURRENT_TEST" in os.environ:
                 break
             await asyncio.sleep(float(self.config.period))
 
     def __init__(self, server: "CustomLanguageServer", config_id: str):
-        text_doc_uri = None  # TODO: think about what text_doc_uri means in this feature
-        super().__init__(server, config_id, text_doc_uri)
+        super().__init__(server, config_id, None)
 
-    async def run_once(self, args: Optional[str] = None):
+    async def run_once(self, args: Optional[str] = None) -> bool:
         if not self.config.has_root_marker(self.server.custom.get_workspace_root()):
-            return
+            return True
 
         replacements = []
         if args:
             replacements = [
                 ("{args}", args),
             ]
         commands = self.resolve_commands(replacements)
-        await self.run_pre_commands(commands)
+        is_success = await self.run_pre_commands(commands)
+        if not is_success:
+            return False
 
         if isinstance(commands, list):
             final_command = commands[-1]
         else:
             final_command = commands
         result = await self.shell(final_command)
+        if result.is_non_zero_exit():
+            return False
 
         workspace_edit = self.build_workspace_edit(result.stdout)
         if workspace_edit is not None:
             self.send_workspace_edit(workspace_edit)
 
+        return True
+
     def send_workspace_edit(self, workspace_edit: WorkspaceEditRequest):
         self.server.logger.debug("Sending Workspace Edit")
         self.server.lsp.apply_edit(workspace_edit, f"{self.config_id} document update")
 
-    # TODO: Refactor with what Diagnoser is also doing
     def build_workspace_edit(self, output: str) -> Optional[WorkspaceEditRequest]:
-        default_formats = [
-            "{kind} {uri} {start_line}:{start_char},{end_line}:{end_char}\n{text_edit}",
-            "{kind} {uri} {start_line}:{start_char},{end_line}:{end_char}",
-            "{kind} {uri}",
-        ]
-
-        if (
-            self.config.parsing is not None
-            and self.config.parsing != OutputParsingConfig.default()
-        ):
-            config = self.config.parsing
-        else:
-            config = OutputParsingConfig(
-                **typing.cast(Dict, {"formats": default_formats})
-            )
-
+        config = self.get_parsing_config(DEFAULT_FORMATTERS)
         for format_string in config.formats:
             maybe_workspace_edit = self.parse_output(
                 config, format_string, output
             )  # type: ignore
             if maybe_workspace_edit is not None:
                 return maybe_workspace_edit
 
-        summary = "Super Glass failed to parse shell output"
-        command = f"Command: `{self.config.command}`"
-        debug = f"{summary}\n{command}\nOutput: {output}"
-        self.server.logger.warning(debug)
-        self.server.show_message(debug, msg_type=MessageType.Warning)
+        self.parsing_failed(output)
         return None
 
-    # `kind`: TextDocumentEdit | CreateFile | RenameFile | DeleteFile
-    # `uri`: Text document URI
-    # `range` (only for TextDocumentEdit): start_line,start_char,end_line,end_char
-    # `text_edit`: All remaining lines
-    # TODO: perhaps this could be made a default formatter?
     def parse_output(
         self, parsing: OutputParsingConfig, format_string: str, output: str
     ) -> Optional[WorkspaceEditRequest]:
         self.server.logger.debug(msg=f"Parsing: '{output}' with '{format_string}'")
         parsed = parse(format_string, output)
         if parsed is None:
             return None
@@ -152,9 +141,10 @@
             )
 
         if parsed["kind"] == "DeleteFile":
             edit = DeleteFile(
                 uri=uri,
             )
 
-        # Also CreateFile, RenameFile can go in the list
+        # TODO: Also CreateFile, RenameFile
+
         return WorkspaceEditRequest(document_changes=[edit])
```

### Comparing `super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/hub.py` & `super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/hub.py`

 * *Files identical despite different names*

### Comparing `super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/e2e/apps/_utils.py` & `super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/e2e/apps/_utils.py`

 * *Files identical despite different names*

### Comparing `super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/e2e/apps/email_client/main_test.py` & `super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/e2e/apps/email_client/main_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,16 +20,15 @@
     waited = 0.0
     max_wait = 8
     while True:
         waited = waited + pause
         if waited > max_wait:
             assert False, "Timeout waiting for LSP server to send applyEdit request"
         calls = patched.call_args_list
-        if len(calls) == 2:
+        if len(calls) == 4:
             break
         await asyncio.sleep(pause)
 
-    args, _kwargs = calls[1]
+    args, _kwargs = calls[3]
     data = args[0]
     body = data["params"]["edit"]["documentChanges"][0]["edits"][0]["newText"]
-    assert "# Inbox" in body
-    assert "| Google" in body
+    assert "1   | Google" in body
```

### Comparing `super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/e2e/configs/__init__.py` & `super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/e2e/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/e2e/configs/black_test.py` & `super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/e2e/configs/black_test.py`

 * *Files identical despite different names*

### Comparing `super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/e2e/configs/flake8_test.py` & `super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/e2e/configs/flake8_test.py`

 * *Files identical despite different names*

### Comparing `super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/e2e/configs/jq_test.py` & `super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/e2e/configs/jq_test.py`

 * *Files identical despite different names*

### Comparing `super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/e2e/configs/markdownlint_test.py` & `super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/e2e/configs/markdownlint_test.py`

 * *Files identical despite different names*

### Comparing `super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/e2e/configs/mypy_test.py` & `super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/e2e/configs/mypy_test.py`

 * *Files identical despite different names*

### Comparing `super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/e2e/test_init_config.py` & `super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/e2e/test_init_config.py`

 * *Files identical despite different names*

### Comparing `super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/units/_utils.py` & `super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/units/_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,18 +24,21 @@
 
     mocker.patch(
         "pygls.workspace.Document.source",
         new_callable=PropertyMock,
         return_value=source,
     )
 
-    subprocess_mock = mocker.patch(
-        "super_glass_lsp.lsp.custom.features._subprocess.Subprocess.run",
-        side_effect=outputs,
-    )
+    if outputs is not None:
+        subprocess_mock = mocker.patch(
+            "super_glass_lsp.lsp.custom.features._subprocess.Subprocess.run",
+            side_effect=outputs,
+        )
+    else:
+        subprocess_mock = None
 
     mocker.patch(
         "super_glass_lsp.lsp.custom.hub.Hub.get_workspace_root",
         return_value="",
     )
 
     server = CustomLanguageServer()
```

### Comparing `super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/units/test_completer.py` & `super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/units/test_completer.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from ._utils import create_server
 
 
 @pytest.mark.asyncio
 async def test_completer(mocker):
     outputs = [
-        SubprocessOutput("foo\nbar", ""),
+        SubprocessOutput("foo\nbar", "", 0),
     ]
     config = {
         "config1": {
             "lsp_feature": "completion",
             "language_id": "testing",
         },
     }
@@ -30,16 +30,16 @@
     assert completions.items[0].label == "foo"
     assert completions.items[1].label == "bar"
 
 
 @pytest.mark.asyncio
 async def test_completer_debounce_cache(mocker):
     outputs = [
-        SubprocessOutput("foo1\nbar1", ""),
-        SubprocessOutput("foo2\nba2", ""),
+        SubprocessOutput("foo1\nbar1", "", 0),
+        SubprocessOutput("foo2\nba2", "", 0),
     ]
     config = {
         "config1": {
             "lsp_feature": "completion",
             "language_id": "testing",
         },
     }
```

### Comparing `super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/units/test_config.py` & `super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/units/test_config.py`

 * *Files identical despite different names*

### Comparing `super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/units/test_debounce.py` & `super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/units/test_debounce.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,16 +9,19 @@
 from super_glass_lsp.lsp.custom.tests.utils import make_diagnostic
 
 from ._utils import create_server
 
 
 @pytest.mark.asyncio
 async def test_debounce_restricts(mocker):
+    mocker.patch("pygls.protocol.JsonRPCProtocol.send_request")
+    mocker.patch("pygls.protocol.JsonRPCProtocol.notify")
+
     outputs = [
-        SubprocessOutput("", "1"),
+        SubprocessOutput("", "1", 0),
     ]
     config = {
         "config1": {
             "lsp_feature": "diagnostic",
             "language_id": "testing",
         },
     }
@@ -32,18 +35,20 @@
         await Diagnoser.run_all(server, uri)
 
     assert subprocess_mock.call_count == 1
 
 
 @pytest.mark.asyncio
 async def test_debounce_releases(mocker):
+    mocker.patch("pygls.protocol.JsonRPCProtocol.notify")
+
     outputs = [
-        SubprocessOutput("", "all"),
-        SubprocessOutput("", "all different"),
-        SubprocessOutput("", "all moore"),
+        SubprocessOutput("", "all", 0),
+        SubprocessOutput("", "all different", 0),
+        SubprocessOutput("", "all moore", 0),
     ]
     config = {
         "config1": {
             "lsp_feature": "diagnostic",
             "language_id": "testing",
             "debounce": 50,
         },
@@ -71,17 +76,19 @@
     assert diagnostics[0] == make_diagnostic([0, 0, 0, 1], "all different", "config1")
 
     assert subprocess_mock.call_count == 2
 
 
 @pytest.mark.asyncio
 async def test_debounce_defers(mocker):
+    mocker.patch("pygls.protocol.JsonRPCProtocol.notify")
+
     outputs = [
-        SubprocessOutput("", "all"),
-        SubprocessOutput("", "all different"),
+        SubprocessOutput("", "all", 0),
+        SubprocessOutput("", "all different", 0),
     ]
     config = {
         "config1": {
             "lsp_feature": "diagnostic",
             "language_id": "testing",
             "debounce": 50,
         },
```

### Comparing `super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/units/test_diagnostics.py` & `super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/units/test_diagnostics.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 @pytest.mark.asyncio
 async def test_supplying_multiple_output_formatters(mocker):
     outputs = [
         SubprocessOutput(
             "",
             "\n".join(["stdin:1:2 all", "stdin:11 no col", "stdin just the message"]),
+            0,
         ),
     ]
     config = {
         "config1": {
             "lsp_feature": "diagnostic",
             "language_id": "testing",
             "command": "",
@@ -45,17 +46,20 @@
     assert diagnostics[2] == make_diagnostic(
         [0, 0, 0, 1], "just the message", "config1"
     )
 
 
 @pytest.mark.asyncio
 async def test_concurrent_diagnosers_dont_clobber(mocker):
+    mocker.patch("pygls.protocol.JsonRPCProtocol.send_request")
+    mocker.patch("pygls.protocol.JsonRPCProtocol.notify")
+
     outputs = [
-        SubprocessOutput("", "1"),
-        SubprocessOutput("", "2"),
+        SubprocessOutput("", "1", 0),
+        SubprocessOutput("", "2", 0),
     ]
     config = {
         "config1": {
             "lsp_feature": "diagnostic",
             "language_id": "testing",
             "piped": False,
         },
```

### Comparing `super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/units/test_formatter.py` & `super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/units/test_formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 
 from ._utils import create_server
 
 
 @pytest.mark.asyncio
 async def test_formatter_debounce(mocker):
     outputs = [
-        SubprocessOutput("\n".join(["foo1", "bar1"]), ""),
-        SubprocessOutput("\n".join(["foo2", "bar2"]), ""),
+        SubprocessOutput("\n".join(["foo1", "bar1"]), "", 0),
+        SubprocessOutput("\n".join(["foo2", "bar2"]), "", 0),
     ]
     server, uri, _ = create_server(
         mocker,
         {
             "config1": {
                 "lsp_feature": "formatter",
                 "language_id": "testing",
                 "debounce": 50,
             }
         },
         outputs,
-        ""
+        "",
     )
 
     expected = TextEdit(
         range=Range(
             start=Position(line=0, character=0),
             end=Position(line=0, character=0),
         ),
```

### Comparing `super_glass_lsp-0.6.0/super_glass_lsp/lsp/custom/tests/units/test_workspace_edit.py` & `super_glass_lsp-0.7.0/super_glass_lsp/lsp/custom/tests/units/test_workspace_edit.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 @pytest.mark.asyncio
 async def test_workspace_edit_textedit(mocker):
     send_request = mocker.patch("pygls.protocol.JsonRPCProtocol.send_request")
 
     new_text = "😊"
     outputs = [
         SubprocessOutput(
-            "\n".join(["TextDocumentEdit /text.txt 0:0,0:0", new_text]), ""
+            "\n".join(["TextDocumentEdit /text.txt 0:0,0:0", new_text]), "", 0
         ),
     ]
     server, _, _ = create_server(
         mocker,
         {
             "config": {
                 "lsp_feature": "workspace_edit",
```

### Comparing `super_glass_lsp-0.6.0/super_glass_lsp/lsp/server.py` & `super_glass_lsp-0.7.0/super_glass_lsp/lsp/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import Dict, Optional, Union, Any, List
 
 from argparse import Namespace
 import logging
 
 from pygls.lsp.types import InitializeParams, Diagnostic
 from pygls import server as pygls_server
+from pygls.workspace import Document
 
 from .custom.hub import Hub as CustomFeatures
 from .custom.config_definitions import (
     Configs as CustomConfig,
 )
 from .custom.config_definitions import (
     InitializationOptions as CustomInitializationOptions,
@@ -129,9 +130,9 @@
     @property
     def configuration(
         self,
     ) -> Optional[Config]:
         """Return the server's actual configuration."""
         return self.config
 
-    def get_document_from_uri(self, uri: str):
+    def get_document_from_uri(self, uri: str) -> Document:
         return self.workspace.get_document(uri)
```

### Comparing `super_glass_lsp-0.6.0/super_glass_lsp/lsp/setup.py` & `super_glass_lsp-0.7.0/super_glass_lsp/lsp/setup.py`

 * *Files identical despite different names*

### Comparing `super_glass_lsp-0.6.0/super_glass_lsp/main.py` & `super_glass_lsp-0.7.0/super_glass_lsp/main.py`

 * *Files identical despite different names*

### Comparing `super_glass_lsp-0.6.0/setup.py` & `super_glass_lsp-0.7.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,203 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: super-glass-lsp
+Version: 0.7.0
+Summary: Generic LSP to parse the output of CLI tools, linters, formatters, etc
+License: MIT
+Author: Thomas Buckley-Houston
+Author-email: tom@tombh.co.uk
+Requires-Python: >=3.7,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: mergedeep (>=1.3.4,<2.0.0)
+Requires-Dist: parse (>=1.19.0,<2.0.0)
+Requires-Dist: psutil (>=5.9.3,<6.0.0)
+Requires-Dist: pydantic (==1.10.7)
+Requires-Dist: pygls (>=0.13.1,<0.14.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: single-source (>=0.3.0,<0.4.0)
+Description-Content-Type: text/markdown
+
+_🚧 WIP: you're very welcome to try this, but I'm breaking a lot at the moment (October 16th)_
+
+# Super Glass
+## Generic LSP Server and/or Pygls Starting Template
+
+> Hackable LSP
+> — @cathalogrady
+
+<img src="logo.png" align="left" />
+
+This project has 2 goals.
+
+  1. A generic LSP server that parses CLI tools, or indeed any program that outputs to STDOUT, such as  linters, formatters, style checkers, etc and converts their output to LSP-compatible behaviour.
+  2. An easily-forkable template to start your own custom LSP server using [Pygls](https://github.com/openlawlibrary/pygls).
+
+Because the heavy-lifting of this language server is done by external tooling (think `pylint`, `jq`, `markdownlint`, etc), there is minimal implementation-specific code in this repo. That is to say that the majority of the code here is applicable to any language server built with [Pygls](https://github.com/openlawlibrary/pygls). Or at the very least, it demonstrates a reasonable starting point. Deleting the `super_glass_lsp/lsp/custom` folder should leave the codebase as close as possible to the minimum starting point for your own custom language server. Then you will also want to rename occurrences of `[C|c]ustom` to your own language server's name.
+
+## Installation
+
+`pip install super-glass-lsp`
+
+## Usage
+
+### Quickstart
+Once you've installed the language server and [set it up in your editor](https://github.com/tombh/super-glass#editor-setups), it should be as easy as this to add new features (this is YAML, but your editor likely has its own config format):
+```yaml
+# This is jsut an ID, so can be anything. Internally it's important so that you can
+# override existing configs (either the bundled defaults, or configs you have
+# created elsewhere): all configs with the same ID are automaticallly merged. 
+fuzzy_similar_words_completion:
+
+  # This is the part of the language server to which the `command` will apply.
+  # The other currently supported features are: `diagnostic`.
+  lsp_feature: completion
+  
+  # This is the external command which will be triggered and parsed for every
+  # invocation of the feature. In the case of completions, editors will generally
+  # trigger it for _every_ character change, or even every key press. So be
+  # careful not to make this too expensive.
+  #
+  # Default behaviour is to pipe the entire contents of the file into the command.
+  # This can be overriden with `piped: false`. In which case you will likely want
+  # to manually do something with the file. You can access its path with the `{file}`
+  # token. Eg; `command: "cat {file} | tr ..."`.
+  #
+  # This particular command first breaks up the file into a list of words, which are
+  # then piped into a fuzzy finder, which then queries the list with the particular
+  # word currently under your cursor in the editor. Finally the results of the fuzzy
+  # search are deduplicated (with `uniq`).
+  #
+  # The command is run in a shell, so all the tools from your own machine are available.
+  command: "tr -cs '[:alnum:]' '\n' | fzf --filter='{word}' | uniq"
+```
+
+### Configuration
+
+The server comes with a lot of [defaults](super_glass_lsp/config.default.yaml). To enable a particular tool simple provide the `enabled: true` field for that tool. For example:
+```yaml
+# This is YAML, but should be whatever format your editor's config is
+initialization_options:
+  configs:
+    jqlint:
+      enabled: true
+```
+
+TODO:
+* [ ] Explain all the fields and tokens for each LSP feature
+* [ ] Remember to describe the format array lines priorities
+* [ ] How to set up the debug logs. But also maybe a LSP option to get all the debug in your editor
+  * [ ] Mention the test logs too. Because the E2E tests run in a subprocess
+* [ ] Remember to advise that some diagnostic tools output on STDERR, not STDOUT
+
+* [ ] Can you have both a Super Glass app _and_ default configs?? I think at the moment you can't? (I don't think so)
+
+## Editor Setups
+
+Because this is a generic language server, the filetype/language that the server applies to varies depending on the config you've setup. It would be a bad idea for a generic language server to tell an editor that it wants to connect with every possible filetype/language (although this can be enabled on a per tool basis with the `language_ids: ["*"]` setting). Instead, it is better that you manually inform your editor which filetypes/languages this generic server should be enabled for. How that is done is unique to each editor's config, I've tried to include examples for each one.
+
+<details>
+<summary>Neovim Lua (vanilla Neovim without `lspconfig`)</summary>
+
+  Since this project is very beta, we're not yet submitting this language server to the LSP Config plugin (the defacto way to add new language servers). Therefore, for now, we have to use Neovim's vanilla LSP setup (which has actually simplified a lot recently).
+
+  ```lua
+  vim.api.nvim_create_autocmd({ "BufEnter" }, {
+    -- NB: You must remember to manually put the file extension pattern matchers for each LSP filetype
+    pattern = { "*" },
+    callback = function()
+      vim.lsp.start({
+        name = "super-glass",
+        cmd = { "super-glass-lsp" },
+        root_dir = vim.fs.dirname(vim.fs.find({ ".git" }, { upward = true })[1]),
+        init_options = {
+          configs = {
+            fuzzy_buffer_tokens = {
+              lsp_feature = "completion",
+              command = "tr -cs '[:alnum:]' '\n' | fzf --filter='{word}' | uniq",
+            },
+          }
+        },
+      })
+    end,
+  })
+  ```
+</details>
+
+<details>
+<summary>Vim (`vim-lsp`)</summary>
+
+  ```vim
+  augroup LspSuperGlass
+  au!
+  autocmd User lsp_setup call lsp#register_server({
+      \ 'name': 'super-glass',
+      \ 'cmd': {server_info->['super-glass-lsp', '--logfile', 'path/to-logfile']},
+      \ 'allowlist': ['vim', 'eruby', 'markdown', 'yaml'],
+      \ 'initialization_options': { "configs":
+      \   { "fuzzy_buffer_tokens": {
+      \       "lsp_feature": "completion",
+      \       "command": "tr -cs '[:alnum:]' '\n' | fzf --filter='{word}' | uniq",
+      \     }
+      \   }
+      \ }})
+  augroup END
+  ```
+</details>
+
+<details>
+<summary>Neovim (`lspconfig`) TBC</summary>
+
+  Once we're stable, we'll submit ourselves for inclusion.
+</details>
+
+<details>
+<summary>Emacs (`lsp-mode`)</summary>
+
+
+  ```
+  (make-lsp-client :new-connection
+  (lsp-stdio-connection
+    `(,(executable-find "super-glass-lsp") "--logfile" "path/to/logs"))
+    :activation-fn (lsp-activate-on "json")
+    :initialization-options ; TODO: I'm not an Emacs user, how do we provide these options?
+    :server-id 'super-glass-lsp')))
+  ```
+</details>
+
+<details>
+<summary>Emacs (`eglot`) TBC</summary>
+  
+  Once we're stable, we'll submit ourselves for inclusion.
+</details>
+
+<details>
+<summary>VSCode TBC</summary>
+  
+  Can we copy EFM's VSCode extension?
+  https://github.com/Matts966/efm-langserver-vscode
+</details>
+
+
+## Testing
+
+Uses [@alcarney](https://github.com/alcarney)'s [pytest-lsp module](https://github.com/alcarney/lsp-devtools/tree/develop/lib/pytest-lsp) for end-to-end testing.
+
+`poetry run python -m pytest`
+
+## Acknowledgements
+
+This projects takes a lot of inspiration from [@alcarney](https://github.com/alcarney)'s fantastic Sphinx/RST LSP server [Esbonio](https://github.com/swyddfa/esbonio). 
+
+Logo is from [a sticker I found on Amazon](https://www.amazon.com/-/es/Superman-S-Adhesivo-reflectante-plateado/dp/B00PEZKHV8), obviously want a proper logo before I publish.
+
+## Other generic LSP servers
+
+* https://github.com/iamcco/diagnostic-languageserver
+* https://github.com/mattn/efm-langserver
+* https://github.com/jose-elias-alvarez/null-ls.nvim (Neovim only)
 
-packages = \
-['super_glass_lsp',
- 'super_glass_lsp.lsp',
- 'super_glass_lsp.lsp.custom',
- 'super_glass_lsp.lsp.custom.features',
- 'super_glass_lsp.lsp.custom.tests',
- 'super_glass_lsp.lsp.custom.tests.e2e',
- 'super_glass_lsp.lsp.custom.tests.e2e.apps',
- 'super_glass_lsp.lsp.custom.tests.e2e.apps.email_client',
- 'super_glass_lsp.lsp.custom.tests.e2e.configs',
- 'super_glass_lsp.lsp.custom.tests.units']
-
-package_data = \
-{'': ['*'],
- 'super_glass_lsp.lsp.custom': ['apps/*'],
- 'super_glass_lsp.lsp.custom.tests.e2e': ['_bin/*'],
- 'super_glass_lsp.lsp.custom.tests.e2e.apps.email_client': ['workspace/.gitignore'],
- 'super_glass_lsp.lsp.custom.tests.e2e.configs': ['workspace/.gitignore']}
-
-install_requires = \
-['mergedeep>=1.3.4,<2.0.0',
- 'parse>=1.19.0,<2.0.0',
- 'psutil>=5.9.3,<6.0.0',
- 'pygls>=0.12.2,<0.13.0',
- 'pyyaml>=6.0,<7.0',
- 'single-source>=0.3.0,<0.4.0']
-
-entry_points = \
-{'console_scripts': ['super-glass-lsp = super_glass_lsp.main:main']}
-
-setup_kwargs = {
-    'name': 'super-glass-lsp',
-    'version': '0.6.0',
-    'description': 'Generic LSP to parse the output of CLI tools, linters, formatters, etc',
-    'long_description': '_🚧 WIP: you\'re very welcome to try this, but I\'m breaking a lot at the moment (October 16th)_\n\n# Super Glass\n## Generic LSP Server and/or Pygls Starting Template\n\n> Hackable LSP\n> — @cathalogrady\n\n<img src="logo.png" align="left" />\n\nThis project has 2 goals.\n\n  1. A generic LSP server that parses CLI tools, or indeed any program that outputs to STDOUT, such as  linters, formatters, style checkers, etc and converts their output to LSP-compatible behaviour.\n  2. An easily-forkable template to start your own custom LSP server using [Pygls](https://github.com/openlawlibrary/pygls).\n\nBecause the heavy-lifting of this language server is done by external tooling (think `pylint`, `jq`, `markdownlint`, etc), there is minimal implementation-specific code in this repo. That is to say that the majority of the code here is applicable to any language server built with [Pygls](https://github.com/openlawlibrary/pygls). Or at the very least, it demonstrates a reasonable starting point. Deleting the `super_glass_lsp/lsp/custom` folder should leave the codebase as close as possible to the minimum starting point for your own custom language server. Then you will also want to rename occurrences of `[C|c]ustom` to your own language server\'s name.\n\n## Installation\n\n`pip install super-glass-lsp`\n\n## Usage\n\n### Quickstart\nOnce you\'ve installed the language server and [set it up in your editor](https://github.com/tombh/super-glass#editor-setups), it should be as easy as this to add new features (this is YAML, but your editor likely has its own config format):\n```yaml\n# This is jsut an ID, so can be anything. Internally it\'s important so that you can\n# override existing configs (either the bundled defaults, or configs you have\n# created elsewhere): all configs with the same ID are automaticallly merged. \nfuzzy_similar_words_completion:\n\n  # This is the part of the language server to which the `command` will apply.\n  # The other currently supported features are: `diagnostic`.\n  lsp_feature: completion\n  \n  # This is the external command which will be triggered and parsed for every\n  # invocation of the feature. In the case of completions, editors will generally\n  # trigger it for _every_ character change, or even every key press. So be\n  # careful not to make this too expensive.\n  #\n  # Default behaviour is to pipe the entire contents of the file into the command.\n  # This can be overriden with `piped: false`. In which case you will likely want\n  # to manually do something with the file. You can access its path with the `{file}`\n  # token. Eg; `command: "cat {file} | tr ..."`.\n  #\n  # This particular command first breaks up the file into a list of words, which are\n  # then piped into a fuzzy finder, which then queries the list with the particular\n  # word currently under your cursor in the editor. Finally the results of the fuzzy\n  # search are deduplicated (with `uniq`).\n  #\n  # The command is run in a shell, so all the tools from your own machine are available.\n  command: "tr -cs \'[:alnum:]\' \'\\n\' | fzf --filter=\'{word}\' | uniq"\n```\n\n### Configuration\n\nThe server comes with a lot of [defaults](super_glass_lsp/config.default.yaml). To enable a particular tool simple provide the `enabled: true` field for that tool. For example:\n```yaml\n# This is YAML, but should be whatever format your editor\'s config is\ninitialization_options:\n  configs:\n    jqlint:\n      enabled: true\n```\n\nTODO:\n* [ ] Explain all the fields and tokens for each LSP feature\n* [ ] Remember to describe the format array lines priorities\n* [ ] How to set up the debug logs. But also maybe a LSP option to get all the debug in your editor\n* [ ] Remember to advise that some diagnostic tools output on STDERR, not STDOUT\n\n## Editor Setups\n\nBecause this is a generic language server, the filetype/language that the server applies to varies depending on the config you\'ve setup. It would be a bad idea for a generic language server to tell an editor that it wants to connect with every possible filetype/language (although this can be enabled on a per tool basis with the `language_ids: ["*"]` setting). Instead, it is better that you manually inform your editor which filetypes/languages this generic server should be enabled for. How that is done is unique to each editor\'s config, I\'ve tried to include examples for each one.\n\n<details>\n<summary>Neovim Lua (vanilla Neovim without `lspconfig`)</summary>\n\n  Since this project is very beta, we\'re not yet submitting this language server to the LSP Config plugin (the defacto way to add new language servers). Therefore, for now, we have to use Neovim\'s vanilla LSP setup (which has actually simplified a lot recently).\n\n  ```lua\n  vim.api.nvim_create_autocmd({ "BufEnter" }, {\n    -- NB: You must remember to manually put the file extension pattern matchers for each LSP filetype\n    pattern = { "*" },\n    callback = function()\n      vim.lsp.start({\n        name = "super-glass",\n        cmd = { "super-glass-lsp" },\n        root_dir = vim.fs.dirname(vim.fs.find({ ".git" }, { upward = true })[1]),\n        init_options = {\n          configs = {\n            fuzzy_buffer_tokens = {\n              lsp_feature = "completion",\n              command = "tr -cs \'[:alnum:]\' \'\\n\' | fzf --filter=\'{word}\' | uniq",\n            },\n          }\n        },\n      })\n    end,\n  })\n  ```\n</details>\n\n<details>\n<summary>Vim (`vim-lsp`)</summary>\n\n  ```vim\n  augroup LspSuperGlass\n  au!\n  autocmd User lsp_setup call lsp#register_server({\n      \\ \'name\': \'super-glass\',\n      \\ \'cmd\': {server_info->[\'super-glass-lsp\', \'--logfile\', \'path/to-logfile\']},\n      \\ \'allowlist\': [\'vim\', \'eruby\', \'markdown\', \'yaml\'],\n      \\ \'initialization_options\': { "configs":\n      \\   { "fuzzy_buffer_tokens": {\n      \\       "lsp_feature": "completion",\n      \\       "command": "tr -cs \'[:alnum:]\' \'\\n\' | fzf --filter=\'{word}\' | uniq",\n      \\     }\n      \\   }\n      \\ }})\n  augroup END\n  ```\n</details>\n\n<details>\n<summary>Neovim (`lspconfig`) TBC</summary>\n\n  Once we\'re stable, we\'ll submit ourselves for inclusion.\n</details>\n\n<details>\n<summary>Emacs (`lsp-mode`)</summary>\n\n\n  ```\n  (make-lsp-client :new-connection\n  (lsp-stdio-connection\n    `(,(executable-find "super-glass-lsp") "--logfile" "path/to/logs"))\n    :activation-fn (lsp-activate-on "json")\n    :initialization-options ; TODO: I\'m not an Emacs user, how do we provide these options?\n    :server-id \'super-glass-lsp\')))\n  ```\n</details>\n\n<details>\n<summary>Emacs (`eglot`) TBC</summary>\n  \n  Once we\'re stable, we\'ll submit ourselves for inclusion.\n</details>\n\n<details>\n<summary>VSCode TBC</summary>\n  \n  Can we copy EFM\'s VSCode extension?\n  https://github.com/Matts966/efm-langserver-vscode\n</details>\n\n\n## Testing\n\nUses [@alcarney](https://github.com/alcarney)\'s [pytest-lsp module](https://github.com/alcarney/lsp-devtools/tree/develop/lib/pytest-lsp) for end-to-end testing.\n\n`poetry run python -m pytest`\n\n## Acknowledgements\n\nThis projects takes a lot of inspiration from [@alcarney](https://github.com/alcarney)\'s fantastic Sphinx/RST LSP server [Esbonio](https://github.com/swyddfa/esbonio). \n\nLogo is from [a sticker I found on Amazon](https://www.amazon.com/-/es/Superman-S-Adhesivo-reflectante-plateado/dp/B00PEZKHV8), obviously want a proper logo before I publish.\n\n## Other generic LSP servers\n\n* https://github.com/iamcco/diagnostic-languageserver\n* https://github.com/mattn/efm-langserver\n* https://github.com/jose-elias-alvarez/null-ls.nvim (Neovim only)\n',
-    'author': 'Thomas Buckley-Houston',
-    'author_email': 'tom@tombh.co.uk',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.10,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

