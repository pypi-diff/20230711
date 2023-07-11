# Comparing `tmp/open-gpt-torch-0.0.9.dev1.tar.gz` & `tmp/open-gpt-torch-0.0.9.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-gpt-torch-0.0.9.dev1.tar", last modified: Mon Jul 10 10:16:39 2023, max compression
+gzip compressed data, was "open-gpt-torch-0.0.9.dev2.tar", last modified: Mon Jul 10 10:24:54 2023, max compression
```

## Comparing `open-gpt-torch-0.0.9.dev1.tar` & `open-gpt-torch-0.0.9.dev2.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:39.873473 open-gpt-torch-0.0.9.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)    10825 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-10 10:16:39.873473 open-gpt-torch-0.0.9.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:39.869473 open-gpt-torch-0.0.9.dev1/open_gpt/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:39.869473 open-gpt-torch-0.0.9.dev1/open_gpt/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/cli/application.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/cli/command_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:39.869473 open-gpt-torch-0.0.9.dev1/open_gpt/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/cli/commands/about.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/cli/commands/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/cli/commands/playground.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/cli/commands/quantize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/cli/commands/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/logs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:39.869473 open-gpt-torch-0.0.9.dev1/open_gpt/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/models/embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:39.873473 open-gpt-torch-0.0.9.dev1/open_gpt/models/flamingo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/models/flamingo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/models/flamingo/configuration_flamingo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/models/flamingo/flamingo_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9481 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/models/flamingo/flamingo_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/models/flamingo/loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/models/flamingo/modeling.py
--rw-r--r--   0 runner    (1001) docker     (123)    11873 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/models/generation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:39.873473 open-gpt-torch-0.0.9.dev1/open_gpt/models/llama/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/models/llama/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/models/llama/loading.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/models/llama/modeling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/models/loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/models/modeling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:39.873473 open-gpt-torch-0.0.9.dev1/open_gpt/models/moss/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/models/moss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/models/moss/modeling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:39.873473 open-gpt-torch-0.0.9.dev1/open_gpt/models/pythia/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/models/pythia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/models/pythia/modeling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:39.873473 open-gpt-torch-0.0.9.dev1/open_gpt/models/rwkv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/models/rwkv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/models/rwkv/modeling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/models/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:39.873473 open-gpt-torch-0.0.9.dev1/open_gpt/models/stablelm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/models/stablelm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/models/stablelm/modeling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:39.873473 open-gpt-torch-0.0.9.dev1/open_gpt/models/vicuna/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/models/vicuna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/models/vicuna/loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/models/vicuna/modeling.py
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:39.873473 open-gpt-torch-0.0.9.dev1/open_gpt/serve/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/serve/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:39.873473 open-gpt-torch-0.0.9.dev1/open_gpt/serve/executors/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/serve/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/serve/executors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/serve/executors/flamingo.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/serve/executors/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/serve/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/serve/gateway.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:39.873473 open-gpt-torch-0.0.9.dev1/open_gpt/serve/playground/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/serve/playground/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/serve/playground/gradio.py
--rw-r--r--   0 runner    (1001) docker     (123)     7396 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/serve/playground/gradio_chatbot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/open_gpt/serve/playground/gradio_css.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:16:39.873473 open-gpt-torch-0.0.9.dev1/open_gpt_torch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-10 10:16:39.000000 open-gpt-torch-0.0.9.dev1/open_gpt_torch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-10 10:16:39.000000 open-gpt-torch-0.0.9.dev1/open_gpt_torch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 10:16:39.000000 open-gpt-torch-0.0.9.dev1/open_gpt_torch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 10:16:39.000000 open-gpt-torch-0.0.9.dev1/open_gpt_torch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-10 10:16:39.000000 open-gpt-torch-0.0.9.dev1/open_gpt_torch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 10:16:39.000000 open-gpt-torch-0.0.9.dev1/open_gpt_torch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 10:16:39.877473 open-gpt-torch-0.0.9.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-07-10 10:16:31.000000 open-gpt-torch-0.0.9.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:24:54.840558 open-gpt-torch-0.0.9.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10825 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-10 10:24:54.840558 open-gpt-torch-0.0.9.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:24:54.836557 open-gpt-torch-0.0.9.dev2/open_gpt/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:24:54.836557 open-gpt-torch-0.0.9.dev2/open_gpt/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/cli/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/cli/command_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:24:54.836557 open-gpt-torch-0.0.9.dev2/open_gpt/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/cli/commands/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/cli/commands/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/cli/commands/playground.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/cli/commands/quantize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/cli/commands/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/logs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:24:54.836557 open-gpt-torch-0.0.9.dev2/open_gpt/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/models/embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:24:54.840558 open-gpt-torch-0.0.9.dev2/open_gpt/models/flamingo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/models/flamingo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/models/flamingo/configuration_flamingo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5954 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/models/flamingo/flamingo_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9481 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/models/flamingo/flamingo_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6484 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/models/flamingo/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/models/flamingo/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11873 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/models/generation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:24:54.840558 open-gpt-torch-0.0.9.dev2/open_gpt/models/llama/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/models/llama/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/models/llama/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/models/llama/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/models/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/models/modeling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:24:54.840558 open-gpt-torch-0.0.9.dev2/open_gpt/models/moss/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/models/moss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/models/moss/modeling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:24:54.840558 open-gpt-torch-0.0.9.dev2/open_gpt/models/pythia/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/models/pythia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/models/pythia/modeling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:24:54.840558 open-gpt-torch-0.0.9.dev2/open_gpt/models/rwkv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/models/rwkv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/models/rwkv/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/models/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:24:54.840558 open-gpt-torch-0.0.9.dev2/open_gpt/models/stablelm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/models/stablelm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/models/stablelm/modeling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:24:54.840558 open-gpt-torch-0.0.9.dev2/open_gpt/models/vicuna/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/models/vicuna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/models/vicuna/loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/models/vicuna/modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:24:54.840558 open-gpt-torch-0.0.9.dev2/open_gpt/serve/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/serve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:24:54.840558 open-gpt-torch-0.0.9.dev2/open_gpt/serve/executors/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/serve/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/serve/executors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/serve/executors/flamingo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/serve/executors/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/serve/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/serve/gateway.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:24:54.840558 open-gpt-torch-0.0.9.dev2/open_gpt/serve/playground/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/serve/playground/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/serve/playground/gradio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7396 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/serve/playground/gradio_chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/open_gpt/serve/playground/gradio_css.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:24:54.840558 open-gpt-torch-0.0.9.dev2/open_gpt_torch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-10 10:24:54.000000 open-gpt-torch-0.0.9.dev2/open_gpt_torch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-10 10:24:54.000000 open-gpt-torch-0.0.9.dev2/open_gpt_torch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 10:24:54.000000 open-gpt-torch-0.0.9.dev2/open_gpt_torch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 10:24:54.000000 open-gpt-torch-0.0.9.dev2/open_gpt_torch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-10 10:24:54.000000 open-gpt-torch-0.0.9.dev2/open_gpt_torch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 10:24:54.000000 open-gpt-torch-0.0.9.dev2/open_gpt_torch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 10:24:54.840558 open-gpt-torch-0.0.9.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-07-10 10:24:46.000000 open-gpt-torch-0.0.9.dev2/setup.py
```

### Comparing `open-gpt-torch-0.0.9.dev1/LICENSE` & `open-gpt-torch-0.0.9.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `open-gpt-torch-0.0.9.dev1/PKG-INFO` & `open-gpt-torch-0.0.9.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-gpt-torch
-Version: 0.0.9.dev1
+Version: 0.0.9.dev2
 Summary: An open-source cloud-native of large multi-modal models (LMMs) serving framework.
 Home-page: https://https://github.com/jina-ai/opengpt
 Download-URL: https://https://github.com/jina-ai/opengpt/tags
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Project-URL: Documentation, https://opengpt.jina.ai
```

### Comparing `open-gpt-torch-0.0.9.dev1/README.md` & `open-gpt-torch-0.0.9.dev2/README.md`

 * *Files identical despite different names*

### Comparing `open-gpt-torch-0.0.9.dev1/open_gpt/__init__.py` & `open-gpt-torch-0.0.9.dev2/open_gpt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging as _logging
 import os as _os
 import sys
 
-__version__ = '0.0.9.dev1'
+__version__ = '0.0.9.dev2'
 
 _logging.captureWarnings(True)
 
 
 # import importlib.metadata if available, otherwise importlib_metadata
 if sys.version_info >= (3, 8):
     import importlib.metadata as importlib_metadata
```

### Comparing `open-gpt-torch-0.0.9.dev1/open_gpt/cli/application.py` & `open-gpt-torch-0.0.9.dev2/open_gpt/cli/application.py`

 * *Files identical despite different names*

### Comparing `open-gpt-torch-0.0.9.dev1/open_gpt/cli/commands/about.py` & `open-gpt-torch-0.0.9.dev2/open_gpt/cli/commands/about.py`

 * *Files identical despite different names*

### Comparing `open-gpt-torch-0.0.9.dev1/open_gpt/cli/commands/deploy.py` & `open-gpt-torch-0.0.9.dev2/open_gpt/cli/commands/deploy.py`

 * *Files identical despite different names*

### Comparing `open-gpt-torch-0.0.9.dev1/open_gpt/cli/commands/playground.py` & `open-gpt-torch-0.0.9.dev2/open_gpt/cli/commands/playground.py`

 * *Files identical despite different names*

### Comparing `open-gpt-torch-0.0.9.dev1/open_gpt/cli/commands/quantize.py` & `open-gpt-torch-0.0.9.dev2/open_gpt/cli/commands/quantize.py`

 * *Files identical despite different names*

### Comparing `open-gpt-torch-0.0.9.dev1/open_gpt/cli/commands/serve.py` & `open-gpt-torch-0.0.9.dev2/open_gpt/cli/commands/serve.py`

 * *Files identical despite different names*

### Comparing `open-gpt-torch-0.0.9.dev1/open_gpt/factory.py` & `open-gpt-torch-0.0.9.dev2/open_gpt/factory.py`

 * *Files identical despite different names*

### Comparing `open-gpt-torch-0.0.9.dev1/open_gpt/helper.py` & `open-gpt-torch-0.0.9.dev2/open_gpt/helper.py`

 * *Files identical despite different names*

### Comparing `open-gpt-torch-0.0.9.dev1/open_gpt/models/embedding.py` & `open-gpt-torch-0.0.9.dev2/open_gpt/models/embedding.py`

 * *Files identical despite different names*

### Comparing `open-gpt-torch-0.0.9.dev1/open_gpt/models/flamingo/configuration_flamingo.py` & `open-gpt-torch-0.0.9.dev2/open_gpt/models/flamingo/configuration_flamingo.py`

 * *Files identical despite different names*

### Comparing `open-gpt-torch-0.0.9.dev1/open_gpt/models/flamingo/flamingo_lm.py` & `open-gpt-torch-0.0.9.dev2/open_gpt/models/flamingo/flamingo_lm.py`

 * *Files identical despite different names*

### Comparing `open-gpt-torch-0.0.9.dev1/open_gpt/models/flamingo/flamingo_model.py` & `open-gpt-torch-0.0.9.dev2/open_gpt/models/flamingo/flamingo_model.py`

 * *Files identical despite different names*

### Comparing `open-gpt-torch-0.0.9.dev1/open_gpt/models/flamingo/loading.py` & `open-gpt-torch-0.0.9.dev2/open_gpt/models/flamingo/loading.py`

 * *Files identical despite different names*

### Comparing `open-gpt-torch-0.0.9.dev1/open_gpt/models/flamingo/modeling.py` & `open-gpt-torch-0.0.9.dev2/open_gpt/models/flamingo/modeling.py`

 * *Files identical despite different names*

### Comparing `open-gpt-torch-0.0.9.dev1/open_gpt/models/generation.py` & `open-gpt-torch-0.0.9.dev2/open_gpt/models/generation.py`

 * *Files identical despite different names*

### Comparing `open-gpt-torch-0.0.9.dev1/open_gpt/models/llama/loading.py` & `open-gpt-torch-0.0.9.dev2/open_gpt/models/llama/loading.py`

 * *Files identical despite different names*

### Comparing `open-gpt-torch-0.0.9.dev1/open_gpt/models/llama/modeling.py` & `open-gpt-torch-0.0.9.dev2/open_gpt/models/llama/modeling.py`

 * *Files identical despite different names*

### Comparing `open-gpt-torch-0.0.9.dev1/open_gpt/models/loading.py` & `open-gpt-torch-0.0.9.dev2/open_gpt/models/loading.py`

 * *Files identical despite different names*

### Comparing `open-gpt-torch-0.0.9.dev1/open_gpt/models/modeling.py` & `open-gpt-torch-0.0.9.dev2/open_gpt/models/modeling.py`

 * *Files identical despite different names*

### Comparing `open-gpt-torch-0.0.9.dev1/open_gpt/models/moss/modeling.py` & `open-gpt-torch-0.0.9.dev2/open_gpt/models/moss/modeling.py`

 * *Files identical despite different names*

### Comparing `open-gpt-torch-0.0.9.dev1/open_gpt/models/pythia/modeling.py` & `open-gpt-torch-0.0.9.dev2/open_gpt/models/pythia/modeling.py`

 * *Files identical despite different names*

### Comparing `open-gpt-torch-0.0.9.dev1/open_gpt/models/rwkv/modeling.py` & `open-gpt-torch-0.0.9.dev2/open_gpt/models/rwkv/modeling.py`

 * *Files identical despite different names*

### Comparing `open-gpt-torch-0.0.9.dev1/open_gpt/models/session.py` & `open-gpt-torch-0.0.9.dev2/open_gpt/models/session.py`

 * *Files identical despite different names*

### Comparing `open-gpt-torch-0.0.9.dev1/open_gpt/models/stablelm/modeling.py` & `open-gpt-torch-0.0.9.dev2/open_gpt/models/stablelm/modeling.py`

 * *Files identical despite different names*

### Comparing `open-gpt-torch-0.0.9.dev1/open_gpt/models/vicuna/loading.py` & `open-gpt-torch-0.0.9.dev2/open_gpt/models/vicuna/loading.py`

 * *Files identical despite different names*

### Comparing `open-gpt-torch-0.0.9.dev1/open_gpt/models/vicuna/modeling.py` & `open-gpt-torch-0.0.9.dev2/open_gpt/models/vicuna/modeling.py`

 * *Files identical despite different names*

### Comparing `open-gpt-torch-0.0.9.dev1/open_gpt/profile.py` & `open-gpt-torch-0.0.9.dev2/open_gpt/profile.py`

 * *Files identical despite different names*

### Comparing `open-gpt-torch-0.0.9.dev1/open_gpt/serve/executors/base.py` & `open-gpt-torch-0.0.9.dev2/open_gpt/serve/executors/base.py`

 * *Files identical despite different names*

### Comparing `open-gpt-torch-0.0.9.dev1/open_gpt/serve/executors/flamingo.py` & `open-gpt-torch-0.0.9.dev2/open_gpt/serve/executors/flamingo.py`

 * *Files identical despite different names*

### Comparing `open-gpt-torch-0.0.9.dev1/open_gpt/serve/flow.py` & `open-gpt-torch-0.0.9.dev2/open_gpt/serve/flow.py`

 * *Files identical despite different names*

### Comparing `open-gpt-torch-0.0.9.dev1/open_gpt/serve/gateway.py` & `open-gpt-torch-0.0.9.dev2/open_gpt/serve/gateway.py`

 * *Files identical despite different names*

### Comparing `open-gpt-torch-0.0.9.dev1/open_gpt/serve/playground/gradio.py` & `open-gpt-torch-0.0.9.dev2/open_gpt/serve/playground/gradio.py`

 * *Files identical despite different names*

### Comparing `open-gpt-torch-0.0.9.dev1/open_gpt/serve/playground/gradio_chatbot.py` & `open-gpt-torch-0.0.9.dev2/open_gpt/serve/playground/gradio_chatbot.py`

 * *Files identical despite different names*

### Comparing `open-gpt-torch-0.0.9.dev1/open_gpt/serve/playground/gradio_css.py` & `open-gpt-torch-0.0.9.dev2/open_gpt/serve/playground/gradio_css.py`

 * *Files identical despite different names*

### Comparing `open-gpt-torch-0.0.9.dev1/open_gpt_torch.egg-info/PKG-INFO` & `open-gpt-torch-0.0.9.dev2/open_gpt_torch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-gpt-torch
-Version: 0.0.9.dev1
+Version: 0.0.9.dev2
 Summary: An open-source cloud-native of large multi-modal models (LMMs) serving framework.
 Home-page: https://https://github.com/jina-ai/opengpt
 Download-URL: https://https://github.com/jina-ai/opengpt/tags
 Author: Jina AI
 Author-email: hello@jina.ai
 License: Apache 2.0
 Project-URL: Documentation, https://opengpt.jina.ai
```

### Comparing `open-gpt-torch-0.0.9.dev1/open_gpt_torch.egg-info/SOURCES.txt` & `open-gpt-torch-0.0.9.dev2/open_gpt_torch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `open-gpt-torch-0.0.9.dev1/setup.py` & `open-gpt-torch-0.0.9.dev2/setup.py`

 * *Files identical despite different names*

