# Comparing `tmp/spacy-llm-0.4.0.tar.gz` & `tmp/spacy-llm-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacy-llm-0.4.0.tar", last modified: Thu Jul  6 12:07:58 2023, max compression
+gzip compressed data, was "spacy-llm-0.4.1.tar", last modified: Tue Jul 11 11:30:17 2023, max compression
```

## Comparing `spacy-llm-0.4.0.tar` & `spacy-llm-0.4.1.tar`

### file list

```diff
@@ -1,170 +1,170 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.961167 spacy-llm-0.4.0/
--rw-r--r--   0 vsts      (1001) docker     (122)     1066 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      147 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)   103207 2023-07-06 12:07:58.961167 spacy-llm-0.4.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)   101989 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)      884 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)     1799 2023-07-06 12:07:58.965167 spacy-llm-0.4.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      153 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.949167 spacy-llm-0.4.0/spacy_llm/
--rw-r--r--   0 vsts      (1001) docker     (122)      232 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10379 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/cache.py
--rw-r--r--   0 vsts      (1001) docker     (122)      895 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/compat.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.949167 spacy-llm-0.4.0/spacy_llm/models/
--rw-r--r--   0 vsts      (1001) docker     (122)      291 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.949167 spacy-llm-0.4.0/spacy_llm/models/hf/
--rw-r--r--   0 vsts      (1001) docker     (122)      264 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/hf/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4886 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/hf/base.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2439 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/hf/dolly.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2814 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/hf/falcon.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3384 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/hf/openllama.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4816 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/hf/stablelm.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.949167 spacy-llm-0.4.0/spacy_llm/models/langchain/
--rw-r--r--   0 vsts      (1001) docker     (122)      227 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/langchain/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4540 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/langchain/model.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.949167 spacy-llm-0.4.0/spacy_llm/models/rest/
--rw-r--r--   0 vsts      (1001) docker     (122)      136 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/rest/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.949167 spacy-llm-0.4.0/spacy_llm/models/rest/anthropic/
--rw-r--r--   0 vsts      (1001) docker     (122)      476 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/rest/anthropic/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3964 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/rest/anthropic/model.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10902 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/rest/anthropic/registry.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5808 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/rest/base.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.949167 spacy-llm-0.4.0/spacy_llm/models/rest/cohere/
--rw-r--r--   0 vsts      (1001) docker     (122)      127 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/rest/cohere/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3369 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/rest/cohere/model.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2016 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/rest/cohere/registry.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.949167 spacy-llm-0.4.0/spacy_llm/models/rest/noop/
--rw-r--r--   0 vsts      (1001) docker     (122)      123 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/rest/noop/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      815 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/rest/noop/model.py
--rw-r--r--   0 vsts      (1001) docker     (122)      351 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/rest/noop/registry.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.949167 spacy-llm-0.4.0/spacy_llm/models/rest/openai/
--rw-r--r--   0 vsts      (1001) docker     (122)      538 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/rest/openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5801 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/rest/openai/model.py
--rw-r--r--   0 vsts      (1001) docker     (122)    19421 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/models/rest/openai/registry.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.953167 spacy-llm-0.4.0/spacy_llm/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (122)       54 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11251 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/pipeline/llm.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.953167 spacy-llm-0.4.0/spacy_llm/registry/
--rw-r--r--   0 vsts      (1001) docker     (122)      262 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/registry/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      606 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/registry/normalizer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2940 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/registry/reader.py
--rw-r--r--   0 vsts      (1001) docker     (122)      450 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/registry/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.953167 spacy-llm-0.4.0/spacy_llm/tasks/
--rw-r--r--   0 vsts      (1001) docker     (122)      850 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4725 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/lemma.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8738 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/ner.py
--rw-r--r--   0 vsts      (1001) docker     (122)      645 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/noop.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8998 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/rel.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4807 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/sentiment.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6944 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/span.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9497 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/spancat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5720 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/summarization.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.953167 spacy-llm-0.4.0/spacy_llm/tasks/templates/
--rw-r--r--   0 vsts      (1001) docker     (122)      288 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/templates/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1003 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/templates/lemma.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)      732 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/templates/ner.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     1396 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/templates/ner.v2.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     1571 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/templates/rel.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)      526 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/templates/sentiment.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)      755 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/templates/spancat.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     1465 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/templates/spancat.v2.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)      661 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/templates/summarization.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     1237 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/templates/textcat.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     1703 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/templates/textcat.v2.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)     2148 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/templates/textcat.v3.jinja
--rw-r--r--   0 vsts      (1001) docker     (122)    16409 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/textcat.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.953167 spacy-llm-0.4.0/spacy_llm/tasks/util/
--rw-r--r--   0 vsts      (1001) docker     (122)      132 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1319 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/util/parsing.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4042 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tasks/util/serialization.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.957167 spacy-llm-0.4.0/spacy_llm/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      315 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/compat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1107 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/conftest.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.957167 spacy-llm-0.4.0/spacy_llm/tests/models/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2481 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/models/test_anthropic.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3094 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/models/test_cohere.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1567 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/models/test_dolly.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1457 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/models/test_falcon.py
--rw-r--r--   0 vsts      (1001) docker     (122)      597 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/models/test_langchain.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1825 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/models/test_openllama.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3299 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/models/test_rest.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2017 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/models/test_stablelm.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.957167 spacy-llm-0.4.0/spacy_llm/tests/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8914 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/pipeline/test_llm.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.957167 spacy-llm-0.4.0/spacy_llm/tests/tasks/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.961167 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/
--rw-r--r--   0 vsts      (1001) docker     (122)     1115 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/lemma.json
--rw-r--r--   0 vsts      (1001) docker     (122)      841 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/lemma.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      930 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/lemma.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      409 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/ner.json
--rw-r--r--   0 vsts      (1001) docker     (122)      233 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/ner.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      255 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/ner.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      349 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/ner_inconsistent.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      579 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/rel.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      249 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/sentiment.json
--rw-r--r--   0 vsts      (1001) docker     (122)      186 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/sentiment.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      174 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/sentiment.yml
--rw-r--r--   0 vsts      (1001) docker     (122)     3126 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/summarization.json
--rw-r--r--   0 vsts      (1001) docker     (122)     3093 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/summarization.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)     3089 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/summarization.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      411 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/textcat_binary.json
--rw-r--r--   0 vsts      (1001) docker     (122)      355 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/textcat_binary.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      359 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/textcat_binary.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      417 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/textcat_multi_excl.json
--rw-r--r--   0 vsts      (1001) docker     (122)      367 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/textcat_multi_excl.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      379 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/textcat_multi_excl.yml
--rw-r--r--   0 vsts      (1001) docker     (122)      433 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl.json
--rw-r--r--   0 vsts      (1001) docker     (122)      383 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl.jsonl
--rw-r--r--   0 vsts      (1001) docker     (122)      395 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl.yml
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.961167 spacy-llm-0.4.0/spacy_llm/tests/tasks/templates/
--rw-r--r--   0 vsts      (1001) docker     (122)       59 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/templates/lemma.jinja2
--rw-r--r--   0 vsts      (1001) docker     (122)      183 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/templates/ner.jinja2
--rw-r--r--   0 vsts      (1001) docker     (122)       27 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/templates/sentiment.jinja2
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/templates/summarization.jinja2
--rw-r--r--   0 vsts      (1001) docker     (122)      191 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/templates/textcat.jinja2
--rw-r--r--   0 vsts      (1001) docker     (122)     9678 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/test_lemma.py
--rw-r--r--   0 vsts      (1001) docker     (122)    24355 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/test_ner.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6093 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/test_rel.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6983 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/test_sentiment.py
--rw-r--r--   0 vsts      (1001) docker     (122)    17549 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/test_spancat.py
--rw-r--r--   0 vsts      (1001) docker     (122)    13777 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/test_summarization.py
--rw-r--r--   0 vsts      (1001) docker     (122)    23930 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/tasks/test_textcat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9200 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/test_cache.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1694 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/test_combinations.py
--rw-r--r--   0 vsts      (1001) docker     (122)      325 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/tests/test_registry.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9252 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/ty.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1764 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/spacy_llm/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.949167 spacy-llm-0.4.0/spacy_llm.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)   103207 2023-07-06 12:07:58.000000 spacy-llm-0.4.0/spacy_llm.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     5129 2023-07-06 12:07:58.000000 spacy-llm-0.4.0/spacy_llm.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-06 12:07:58.000000 spacy-llm-0.4.0/spacy_llm.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      182 2023-07-06 12:07:58.000000 spacy-llm-0.4.0/spacy_llm.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-06 12:07:58.000000 spacy-llm-0.4.0/spacy_llm.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      137 2023-07-06 12:07:58.000000 spacy-llm-0.4.0/spacy_llm.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       25 2023-07-06 12:07:58.000000 spacy-llm-0.4.0/spacy_llm.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.961167 spacy-llm-0.4.0/usage_examples/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/usage_examples/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.961167 spacy-llm-0.4.0/usage_examples/multitask_openai/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/usage_examples/multitask_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1244 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/usage_examples/multitask_openai/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.961167 spacy-llm-0.4.0/usage_examples/ner_dolly/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/usage_examples/ner_dolly/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      972 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/usage_examples/ner_dolly/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.961167 spacy-llm-0.4.0/usage_examples/ner_langchain_openai/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/usage_examples/ner_langchain_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      900 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/usage_examples/ner_langchain_openai/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.961167 spacy-llm-0.4.0/usage_examples/rel_openai/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/usage_examples/rel_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1337 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/usage_examples/rel_openai/run_pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.961167 spacy-llm-0.4.0/usage_examples/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/usage_examples/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      166 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/usage_examples/tests/conftest.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3344 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/usage_examples/tests/test_readme_examples.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2591 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/usage_examples/tests/test_usage_examples.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-06 12:07:58.961167 spacy-llm-0.4.0/usage_examples/textcat_openai/
--rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/usage_examples/textcat_openai/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1173 2023-07-06 12:07:43.000000 spacy-llm-0.4.0/usage_examples/textcat_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.310685 spacy-llm-0.4.1/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1066 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      147 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)   102951 2023-07-11 11:30:17.314685 spacy-llm-0.4.1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)   101733 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      918 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     1827 2023-07-11 11:30:17.314685 spacy-llm-0.4.1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      153 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.294685 spacy-llm-0.4.1/spacy_llm/
+-rw-r--r--   0 vsts      (1001) docker     (122)      232 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10379 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/cache.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      895 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/compat.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.294685 spacy-llm-0.4.1/spacy_llm/models/
+-rw-r--r--   0 vsts      (1001) docker     (122)      291 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.298685 spacy-llm-0.4.1/spacy_llm/models/hf/
+-rw-r--r--   0 vsts      (1001) docker     (122)      264 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/hf/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4886 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/hf/base.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2439 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/hf/dolly.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2814 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/hf/falcon.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3332 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/hf/openllama.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4816 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/hf/stablelm.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.298685 spacy-llm-0.4.1/spacy_llm/models/langchain/
+-rw-r--r--   0 vsts      (1001) docker     (122)      227 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/langchain/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4540 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/langchain/model.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.298685 spacy-llm-0.4.1/spacy_llm/models/rest/
+-rw-r--r--   0 vsts      (1001) docker     (122)      136 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/rest/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.298685 spacy-llm-0.4.1/spacy_llm/models/rest/anthropic/
+-rw-r--r--   0 vsts      (1001) docker     (122)      476 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/rest/anthropic/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4252 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/rest/anthropic/model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10902 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/rest/anthropic/registry.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5971 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/rest/base.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.298685 spacy-llm-0.4.1/spacy_llm/models/rest/cohere/
+-rw-r--r--   0 vsts      (1001) docker     (122)      127 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/rest/cohere/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3369 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/rest/cohere/model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2016 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/rest/cohere/registry.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.298685 spacy-llm-0.4.1/spacy_llm/models/rest/noop/
+-rw-r--r--   0 vsts      (1001) docker     (122)      123 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/rest/noop/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      865 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/rest/noop/model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      351 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/rest/noop/registry.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.298685 spacy-llm-0.4.1/spacy_llm/models/rest/openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)      538 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/rest/openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5813 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/rest/openai/model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    19421 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/models/rest/openai/registry.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.298685 spacy-llm-0.4.1/spacy_llm/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (122)       54 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11251 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/pipeline/llm.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.298685 spacy-llm-0.4.1/spacy_llm/registry/
+-rw-r--r--   0 vsts      (1001) docker     (122)      262 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/registry/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      606 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/registry/normalizer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2940 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/registry/reader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      450 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/registry/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.302685 spacy-llm-0.4.1/spacy_llm/tasks/
+-rw-r--r--   0 vsts      (1001) docker     (122)      850 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4725 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/lemma.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8738 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/ner.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      645 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/noop.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8998 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/rel.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4807 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/sentiment.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6944 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/span.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9497 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/spancat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5720 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/summarization.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.302685 spacy-llm-0.4.1/spacy_llm/tasks/templates/
+-rw-r--r--   0 vsts      (1001) docker     (122)      288 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/templates/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1003 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/templates/lemma.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)      732 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/templates/ner.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1396 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/templates/ner.v2.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1571 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/templates/rel.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)      526 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/templates/sentiment.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)      755 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/templates/spancat.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1465 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/templates/spancat.v2.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)      661 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/templates/summarization.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1237 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/templates/textcat.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     1703 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/templates/textcat.v2.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)     2148 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/templates/textcat.v3.jinja
+-rw-r--r--   0 vsts      (1001) docker     (122)    16409 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/textcat.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.302685 spacy-llm-0.4.1/spacy_llm/tasks/util/
+-rw-r--r--   0 vsts      (1001) docker     (122)      132 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1319 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/util/parsing.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4042 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tasks/util/serialization.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.302685 spacy-llm-0.4.1/spacy_llm/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      315 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/compat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1350 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/conftest.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.306685 spacy-llm-0.4.1/spacy_llm/tests/models/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2323 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/models/test_anthropic.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3068 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/models/test_cohere.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1618 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/models/test_dolly.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1508 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/models/test_falcon.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      597 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/models/test_langchain.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1865 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/models/test_openllama.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3299 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/models/test_rest.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2085 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/models/test_stablelm.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.306685 spacy-llm-0.4.1/spacy_llm/tests/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8914 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/pipeline/test_llm.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.306685 spacy-llm-0.4.1/spacy_llm/tests/tasks/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.310685 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1115 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/lemma.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      841 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/lemma.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      930 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/lemma.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      409 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/ner.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      233 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/ner.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      255 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/ner.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      349 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/ner_inconsistent.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      579 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/rel.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      249 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/sentiment.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      186 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/sentiment.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      174 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/sentiment.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)     3126 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/summarization.json
+-rw-r--r--   0 vsts      (1001) docker     (122)     3093 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/summarization.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)     3089 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/summarization.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      411 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/textcat_binary.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      355 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/textcat_binary.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      359 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/textcat_binary.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      417 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/textcat_multi_excl.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      367 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/textcat_multi_excl.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      379 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/textcat_multi_excl.yml
+-rw-r--r--   0 vsts      (1001) docker     (122)      433 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl.json
+-rw-r--r--   0 vsts      (1001) docker     (122)      383 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl.jsonl
+-rw-r--r--   0 vsts      (1001) docker     (122)      395 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/textcat_multi_nonexcl.yml
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.310685 spacy-llm-0.4.1/spacy_llm/tests/tasks/templates/
+-rw-r--r--   0 vsts      (1001) docker     (122)       59 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/templates/lemma.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (122)      183 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/templates/ner.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (122)       27 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/templates/sentiment.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/templates/summarization.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (122)      191 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/templates/textcat.jinja2
+-rw-r--r--   0 vsts      (1001) docker     (122)     9678 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/test_lemma.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    24355 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/test_ner.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6093 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/test_rel.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6983 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/test_sentiment.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    17549 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/test_spancat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13777 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/test_summarization.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    23930 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/tasks/test_textcat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9200 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/test_cache.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1694 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/test_combinations.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      325 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/tests/test_registry.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9252 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/ty.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1764 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/spacy_llm/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.294685 spacy-llm-0.4.1/spacy_llm.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)   102951 2023-07-11 11:30:17.000000 spacy-llm-0.4.1/spacy_llm.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     5129 2023-07-11 11:30:17.000000 spacy-llm-0.4.1/spacy_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-11 11:30:17.000000 spacy-llm-0.4.1/spacy_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      182 2023-07-11 11:30:17.000000 spacy-llm-0.4.1/spacy_llm.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-11 11:30:17.000000 spacy-llm-0.4.1/spacy_llm.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      137 2023-07-11 11:30:17.000000 spacy-llm-0.4.1/spacy_llm.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       25 2023-07-11 11:30:17.000000 spacy-llm-0.4.1/spacy_llm.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.310685 spacy-llm-0.4.1/usage_examples/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/usage_examples/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.310685 spacy-llm-0.4.1/usage_examples/multitask_openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/usage_examples/multitask_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1244 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/usage_examples/multitask_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.310685 spacy-llm-0.4.1/usage_examples/ner_dolly/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/usage_examples/ner_dolly/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      972 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/usage_examples/ner_dolly/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.310685 spacy-llm-0.4.1/usage_examples/ner_langchain_openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/usage_examples/ner_langchain_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      900 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/usage_examples/ner_langchain_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.310685 spacy-llm-0.4.1/usage_examples/rel_openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/usage_examples/rel_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1337 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/usage_examples/rel_openai/run_pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.310685 spacy-llm-0.4.1/usage_examples/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/usage_examples/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      166 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/usage_examples/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3361 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/usage_examples/tests/test_readme_examples.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2608 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/usage_examples/tests/test_usage_examples.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-11 11:30:17.310685 spacy-llm-0.4.1/usage_examples/textcat_openai/
+-rw-r--r--   0 vsts      (1001) docker     (122)       67 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/usage_examples/textcat_openai/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1173 2023-07-11 11:30:06.000000 spacy-llm-0.4.1/usage_examples/textcat_openai/run_pipeline.py
```

### Comparing `spacy-llm-0.4.0/LICENSE` & `spacy-llm-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/PKG-INFO` & `spacy-llm-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy-llm
-Version: 0.4.0
+Version: 0.4.1
 Summary: Integrating LLMs into structured NLP pipelines
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Project-URL: Release notes, https://github.com/explosion/spacy-llm/releases
 Project-URL: Source, https://github.com/explosion/spacy-llm
 Classifier: Development Status :: 4 - Beta
@@ -1502,22 +1502,22 @@
 ```
 
 Example config block:
 
 ```ini
 [components.llm.model]
 @llm_models = "spacy.OpenLLaMA.v1"
-name = "open_llama_3b_350bt_preview"
+name = "open_llama_3b"
 ```
 
-| Argument      | Type                                                                                                                                  | Default | Description                                                                                                                  |
-| ------------- | ------------------------------------------------------------------------------------------------------------------------------------- | ------- | ---------------------------------------------------------------------------------------------------------------------------- |
-| `name`        | `Literal["open_llama_3b_350bt_preview", "open_llama_3b_600bt_preview", "open_llama_7b_400bt_preview", "open_llama_7b_600bt_preview"]` |         | The name of a OpenLLaMA model that is supported (e. g. "open_llama_3b_350bt_preview").                                       |
-| `config_init` | `Dict[str, Any]`                                                                                                                      | `{}`    | Further configuration passed on to the construction of the model with `transformers.AutoModelForCausalLM.from_pretrained()`. |
-| `config_run`  | `Dict[str, Any]`                                                                                                                      | `{}`    | Further configuration used during model inference.                                                                           |
+| Argument      | Type                                                                                            | Default | Description                                                                                                                  |
+| ------------- |-------------------------------------------------------------------------------------------------| ------- | ---------------------------------------------------------------------------------------------------------------------------- |
+| `name`        | `Literal["open_llama_3b", "open_llama_7b", "open_llama_7b_v2", "open_llama_13b"]` |         | The name of a OpenLLaMA model that is supported.                                       |
+| `config_init` | `Dict[str, Any]`                                                                                | `{}`    | Further configuration passed on to the construction of the model with `transformers.AutoModelForCausalLM.from_pretrained()`. |
+| `config_run`  | `Dict[str, Any]`                                                                                | `{}`    | Further configuration used during model inference.                                                                           |
 
 See the [OpenLM Research OpenLLaMA GitHub repo](https://github.com/openlm-research/open_llama) for details.
 
 Note that Hugging Face will download this model the first time you use it - you can
 [define the cached directory](https://huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache)
 by setting the environmental variable `HF_HOME`.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spacy-llm Version: 0.4.0 Summary: Integrating LLMs
+Metadata-Version: 2.1 Name: spacy-llm Version: 0.4.1 Summary: Integrating LLMs
 into structured NLP pipelines Author: Explosion Author-email:
 contact@explosion.ai License: MIT Project-URL: Release notes, https://
 github.com/explosion/spacy-llm/releases Project-URL: Source, https://
 github.com/explosion/spacy-llm Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: POSIX :: Linux
@@ -927,22 +927,20 @@
 with ```shell python -m pip install "spacy-llm[transformers]" "transformers
 [sentencepiece]" ``` If you don't have access to a GPU, you can install
 `accelerate` and set`device_map=auto` instead, but be aware that this may
 result in some layers getting distributed to the CPU or even the hard drive,
 which may ultimately result in extremely slow queries. ```shell python -m pip
 install "accelerate>=0.16.0,<1.0" ``` Example config block: ```ini
 [components.llm.model] @llm_models = "spacy.OpenLLaMA.v1" name =
-"open_llama_3b_350bt_preview" ``` | Argument | Type | Default | Description | |
-------------- | ---------------------------------------------------------------
----------------------------------------------------------------------- | ------
-- | ---------------------------------------------------------------------------
-------------------------------------------------- | | `name` | `Literal
-["open_llama_3b_350bt_preview", "open_llama_3b_600bt_preview",
-"open_llama_7b_400bt_preview", "open_llama_7b_600bt_preview"]` | | The name of
-a OpenLLaMA model that is supported (e. g. "open_llama_3b_350bt_preview"). | |
+"open_llama_3b" ``` | Argument | Type | Default | Description | | ------------
+- |----------------------------------------------------------------------------
+---------------------| ------- | ----------------------------------------------
+-----------------------------------------------------------------------------
+- | | `name` | `Literal["open_llama_3b", "open_llama_7b", "open_llama_7b_v2",
+"open_llama_13b"]` | | The name of a OpenLLaMA model that is supported. | |
 `config_init` | `Dict[str, Any]` | `{}` | Further configuration passed on to
 the construction of the model with
 `transformers.AutoModelForCausalLM.from_pretrained()`. | | `config_run` | `Dict
 [str, Any]` | `{}` | Further configuration used during model inference. | See
 the [OpenLM Research OpenLLaMA GitHub repo](https://github.com/openlm-research/
 open_llama) for details. Note that Hugging Face will download this model the
 first time you use it - you can [define the cached directory](https://
```

### Comparing `spacy-llm-0.4.0/README.md` & `spacy-llm-0.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1471,22 +1471,22 @@
 ```
 
 Example config block:
 
 ```ini
 [components.llm.model]
 @llm_models = "spacy.OpenLLaMA.v1"
-name = "open_llama_3b_350bt_preview"
+name = "open_llama_3b"
 ```
 
-| Argument      | Type                                                                                                                                  | Default | Description                                                                                                                  |
-| ------------- | ------------------------------------------------------------------------------------------------------------------------------------- | ------- | ---------------------------------------------------------------------------------------------------------------------------- |
-| `name`        | `Literal["open_llama_3b_350bt_preview", "open_llama_3b_600bt_preview", "open_llama_7b_400bt_preview", "open_llama_7b_600bt_preview"]` |         | The name of a OpenLLaMA model that is supported (e. g. "open_llama_3b_350bt_preview").                                       |
-| `config_init` | `Dict[str, Any]`                                                                                                                      | `{}`    | Further configuration passed on to the construction of the model with `transformers.AutoModelForCausalLM.from_pretrained()`. |
-| `config_run`  | `Dict[str, Any]`                                                                                                                      | `{}`    | Further configuration used during model inference.                                                                           |
+| Argument      | Type                                                                                            | Default | Description                                                                                                                  |
+| ------------- |-------------------------------------------------------------------------------------------------| ------- | ---------------------------------------------------------------------------------------------------------------------------- |
+| `name`        | `Literal["open_llama_3b", "open_llama_7b", "open_llama_7b_v2", "open_llama_13b"]` |         | The name of a OpenLLaMA model that is supported.                                       |
+| `config_init` | `Dict[str, Any]`                                                                                | `{}`    | Further configuration passed on to the construction of the model with `transformers.AutoModelForCausalLM.from_pretrained()`. |
+| `config_run`  | `Dict[str, Any]`                                                                                | `{}`    | Further configuration used during model inference.                                                                           |
 
 See the [OpenLM Research OpenLLaMA GitHub repo](https://github.com/openlm-research/open_llama) for details.
 
 Note that Hugging Face will download this model the first time you use it - you can
 [define the cached directory](https://huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache)
 by setting the environmental variable `HF_HOME`.
```

#### html2text {}

```diff
@@ -911,22 +911,20 @@
 with ```shell python -m pip install "spacy-llm[transformers]" "transformers
 [sentencepiece]" ``` If you don't have access to a GPU, you can install
 `accelerate` and set`device_map=auto` instead, but be aware that this may
 result in some layers getting distributed to the CPU or even the hard drive,
 which may ultimately result in extremely slow queries. ```shell python -m pip
 install "accelerate>=0.16.0,<1.0" ``` Example config block: ```ini
 [components.llm.model] @llm_models = "spacy.OpenLLaMA.v1" name =
-"open_llama_3b_350bt_preview" ``` | Argument | Type | Default | Description | |
-------------- | ---------------------------------------------------------------
----------------------------------------------------------------------- | ------
-- | ---------------------------------------------------------------------------
-------------------------------------------------- | | `name` | `Literal
-["open_llama_3b_350bt_preview", "open_llama_3b_600bt_preview",
-"open_llama_7b_400bt_preview", "open_llama_7b_600bt_preview"]` | | The name of
-a OpenLLaMA model that is supported (e. g. "open_llama_3b_350bt_preview"). | |
+"open_llama_3b" ``` | Argument | Type | Default | Description | | ------------
+- |----------------------------------------------------------------------------
+---------------------| ------- | ----------------------------------------------
+-----------------------------------------------------------------------------
+- | | `name` | `Literal["open_llama_3b", "open_llama_7b", "open_llama_7b_v2",
+"open_llama_13b"]` | | The name of a OpenLLaMA model that is supported. | |
 `config_init` | `Dict[str, Any]` | `{}` | Further configuration passed on to
 the construction of the model with
 `transformers.AutoModelForCausalLM.from_pretrained()`. | | `config_run` | `Dict
 [str, Any]` | `{}` | Further configuration used during model inference. | See
 the [OpenLM Research OpenLLaMA GitHub repo](https://github.com/openlm-research/
 open_llama) for details. Note that Hugging Face will download this model the
 first time you use it - you can [define the cached directory](https://
```

### Comparing `spacy-llm-0.4.0/pyproject.toml` & `spacy-llm-0.4.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -18,13 +18,14 @@
     "ignore:^.*pkg_resources.*:DeprecationWarning",
     "ignore:.*function is now available as sqlalchemy.orm.declarative_base().*:",
     "ignore:^.*You are trying to use a chat model. This way of initializing it is no longer supported. Instead, please use.*:UserWarning",
     "ignore:^.*Xformers is not installed correctly.*:",
     "ignore:^.*The 'warn' method is deprecated, use 'warning' instead.*:DeprecationWarning"
 ]
 markers = [
-    "external: interacts with a (potentially cost-incurring) third-party API"
+    "external: interacts with a (potentially cost-incurring) third-party API",
+    "gpu: requires a GPU to run"
 ]
 
 [tool.isort]
 multi_line_output = 9
 profile = "black"
```

### Comparing `spacy-llm-0.4.0/setup.cfg` & `spacy-llm-0.4.1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 0.4.0
+version = 0.4.1
 description = Integrating LLMs into structured NLP pipelines
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
@@ -61,14 +61,15 @@
 ignore_missing_imports = true
 no_implicit_optional = true
 allow_redefinition = true
 
 [tool:pytest]
 markers = 
 	external: interacts with a (potentially cost-incurring) third-party API
+	gpu: requires a GPU to run
 filterwarnings = 
 	ignore:pkg_resources:DeprecationWarning
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `spacy-llm-0.4.0/spacy_llm/cache.py` & `spacy-llm-0.4.1/spacy_llm/cache.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/compat.py` & `spacy-llm-0.4.1/spacy_llm/compat.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/models/hf/base.py` & `spacy-llm-0.4.1/spacy_llm/models/hf/base.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/models/hf/dolly.py` & `spacy-llm-0.4.1/spacy_llm/models/hf/dolly.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/models/hf/falcon.py` & `spacy-llm-0.4.1/spacy_llm/models/hf/falcon.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/models/hf/openllama.py` & `spacy-llm-0.4.1/spacy_llm/models/hf/openllama.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 from ...compat import Literal, torch, transformers
 from ...registry.util import registry
 from .base import HuggingFace
 
 
 class OpenLLaMA(HuggingFace):
     MODEL_NAMES = Literal[
-        "open_llama_3b_350bt_preview",  # noqa: F722
-        "open_llama_3b_600bt_preview",  # noqa: F722
-        "open_llama_7b_400bt_preview",  # noqa: F722
-        "open_llama_7b_600bt_preview",  # noqa: F722
+        "open_llama_3b",  # noqa: F722
+        "open_llama_7b",  # noqa: F722
+        "open_llama_7b_v2",  # noqa: F722
+        "open_llama_13b",  # noqa: F722
     ]
 
     def __init__(
         self,
         name: str,
         config_init: Optional[Dict[str, Any]],
         config_run: Optional[Dict[str, Any]],
```

### Comparing `spacy-llm-0.4.0/spacy_llm/models/hf/stablelm.py` & `spacy-llm-0.4.1/spacy_llm/models/hf/stablelm.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/models/langchain/model.py` & `spacy-llm-0.4.1/spacy_llm/models/langchain/model.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/models/rest/anthropic/model.py` & `spacy-llm-0.4.1/spacy_llm/models/rest/anthropic/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,27 +26,28 @@
 class Anthropic(REST):
     MODEL_NAMES = {
         "claude-1": Literal["claude-1", "claude-1-100k"],
     }
 
     @property
     def credentials(self) -> Dict[str, str]:
-        # Fetch and check the key
+        # Fetch and check the key, set up headers
         api_key = os.getenv("ANTHROPIC_API_KEY")
         if api_key is None:
             raise ValueError(
                 "Could not find the API key to access the Anthropic Claude API. Ensure you have an API key "
                 "set up via the Anthropic console (https://console.anthropic.com/), then make it available as "
                 "an environment variable 'ANTHROPIC_API_KEY."
             )
 
-        # Set-up headers
-        headers = {"X-API-Key": api_key}
-        assert api_key is not None
-        return headers
+        return {"X-API-Key": api_key}
+
+    def _verify_auth(self) -> None:
+        # Execute a dummy prompt. If the API setup is incorrect, we should fail at initialization time.
+        self(["test"])
 
     def __call__(self, prompts: Iterable[str]) -> Iterable[str]:
         headers = {
             **self._credentials,
             "model": self._name,
             "Content-Type": "application/json",
         }
@@ -63,17 +64,19 @@
                 timeout=self._max_request_time,
             )
             try:
                 r.raise_for_status()
             except HTTPError as ex:
                 res_content = srsly.json_loads(r.content.decode("utf-8"))
                 # Include specific error message in exception.
-                raise ValueError(
-                    f"Request to Anthropic API failed: {res_content.get('error', {})}"
-                ) from ex
+                error = res_content.get("error", {})
+                error_msg = f"Request to Anthropic API failed: {error}"
+                if error["type"] == "not_found_error":
+                    error_msg += f". Ensure that the selected model ({self._name}) is supported by the API."
+                raise ValueError(error_msg) from ex
             response = r.json()
 
             # c.f. https://console.anthropic.com/docs/api/errors
             if "error" in response:
                 if self._strict:
                     raise ValueError(f"API call failed: {response}.")
                 else:
```

### Comparing `spacy-llm-0.4.0/spacy_llm/models/rest/anthropic/registry.py` & `spacy-llm-0.4.1/spacy_llm/models/rest/anthropic/registry.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/models/rest/base.py` & `spacy-llm-0.4.1/spacy_llm/models/rest/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,14 +58,15 @@
         self._credentials = self.credentials
 
         assert self._max_tries >= 1
         assert self._interval > 0
         assert self._max_request_time > 0
 
         self._check_model()
+        self._verify_auth()
 
     def _check_model(self) -> None:
         """Checks whether model is supported. Raises if it isn't."""
         if self._name not in self.get_model_names():
             raise ValueError(
                 f"Model '{self._name}' is not supported - select one of {self.get_model_names()} instead"
             )
@@ -87,14 +88,18 @@
     @property
     @abc.abstractmethod
     def credentials(self) -> Dict[str, str]:
         """Get credentials for the LLM API.
         RETURNS (Dict[str, str]): Credentials.
         """
 
+    @abc.abstractmethod
+    def _verify_auth(self) -> None:
+        """Verifiy API authentication (and model choice, if possible)."""
+
     def retry(
         self, call_method: Callable[..., requests.Response], url: str, **kwargs
     ) -> requests.Response:
         """Retry a call to an API if we get a non-ok status code.
         This function automatically retries a request if it catches a response with an error code in `error_codes`.
         The time interval also increases exponentially every time we retry.
         call_method (Callable[[str, ...], requests.Response]): Method to use to fetch request. Must accept URL as first
```

### Comparing `spacy-llm-0.4.0/spacy_llm/models/rest/cohere/model.py` & `spacy-llm-0.4.1/spacy_llm/models/rest/cohere/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,17 +19,19 @@
         api_key = os.getenv("CO_API_KEY")
         if api_key is None:
             raise ValueError(
                 "Could not find the API key to access the Cohere API. Ensure you have an API key "
                 "set up via https://dashboard.cohere.ai/api-keys, then make it available as "
                 "an environment variable 'CO_API_KEY'."
             )
-        headers = {"Authorization": f"Bearer {api_key}"}
-        assert api_key is not None
-        return headers
+
+        return {"Authorization": f"Bearer {api_key}"}
+
+    def _verify_auth(self) -> None:
+        self(["test"])
 
     def __call__(self, prompts: Iterable[str]) -> Iterable[str]:
         headers = {
             **self._credentials,
             "Content-Type": "application/json",
             "Accept": "application/json",
         }
```

### Comparing `spacy-llm-0.4.0/spacy_llm/models/rest/cohere/registry.py` & `spacy-llm-0.4.1/spacy_llm/models/rest/cohere/registry.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/models/rest/openai/__init__.py` & `spacy-llm-0.4.1/spacy_llm/models/rest/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/models/rest/openai/model.py` & `spacy-llm-0.4.1/spacy_llm/models/rest/openai/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,18 +30,28 @@
         # Check the access and get a list of available models to verify the model argument (if not None)
         # Even if the model is None, this call is used as a healthcheck to verify access.
         headers = {
             "Authorization": f"Bearer {api_key}",
         }
         if api_org:
             headers["OpenAI-Organization"] = api_org
+
+        # Ensure endpoint is supported.
+        if self._endpoint not in (Endpoints.NON_CHAT, Endpoints.CHAT):
+            raise ValueError(
+                f"Endpoint {self._endpoint} isn't supported. Please use one of: {Endpoints.CHAT}, {Endpoints.NON_CHAT}."
+            )
+
+        return headers
+
+    def _verify_auth(self) -> None:
         r = self.retry(
             call_method=requests.get,
             url="https://api.openai.com/v1/models",
-            headers=headers,
+            headers=self._credentials,
             timeout=self._max_request_time,
         )
         if r.status_code == 422:
             raise ValueError(
                 "Could not access api.openai.com -- 422 permission denied."
                 "Visit https://platform.openai.com/account/api-keys to check your API keys."
             )
@@ -53,23 +63,14 @@
         response = r.json()["data"]
         models = [response[i]["id"] for i in range(len(response))]
         if self._name not in models:
             raise ValueError(
                 f"The specified model '{self._name}' is not available. Choices are: {sorted(set(models))}"
             )
 
-        # Ensure endpoint is supported.
-        if self._endpoint not in (Endpoints.NON_CHAT, Endpoints.CHAT):
-            raise ValueError(
-                f"Endpoint {self._endpoint} isn't supported. Please use one of: {Endpoints.CHAT}, {Endpoints.NON_CHAT}."
-            )
-
-        assert api_key is not None
-        return headers
-
     def __call__(self, prompts: Iterable[str]) -> Iterable[str]:
         headers = {
             **self._credentials,
             "Content-Type": "application/json",
         }
         api_responses: List[str] = []
         prompts = list(prompts)
```

### Comparing `spacy-llm-0.4.0/spacy_llm/models/rest/openai/registry.py` & `spacy-llm-0.4.1/spacy_llm/models/rest/openai/registry.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/pipeline/llm.py` & `spacy-llm-0.4.1/spacy_llm/pipeline/llm.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/registry/normalizer.py` & `spacy-llm-0.4.1/spacy_llm/registry/normalizer.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/registry/reader.py` & `spacy-llm-0.4.1/spacy_llm/registry/reader.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tasks/__init__.py` & `spacy-llm-0.4.1/spacy_llm/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tasks/lemma.py` & `spacy-llm-0.4.1/spacy_llm/tasks/lemma.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tasks/ner.py` & `spacy-llm-0.4.1/spacy_llm/tasks/ner.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tasks/noop.py` & `spacy-llm-0.4.1/spacy_llm/tasks/noop.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tasks/rel.py` & `spacy-llm-0.4.1/spacy_llm/tasks/rel.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tasks/sentiment.py` & `spacy-llm-0.4.1/spacy_llm/tasks/sentiment.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tasks/span.py` & `spacy-llm-0.4.1/spacy_llm/tasks/span.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tasks/spancat.py` & `spacy-llm-0.4.1/spacy_llm/tasks/spancat.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tasks/summarization.py` & `spacy-llm-0.4.1/spacy_llm/tasks/summarization.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tasks/templates/lemma.jinja` & `spacy-llm-0.4.1/spacy_llm/tasks/templates/lemma.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tasks/templates/ner.jinja` & `spacy-llm-0.4.1/spacy_llm/tasks/templates/ner.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tasks/templates/ner.v2.jinja` & `spacy-llm-0.4.1/spacy_llm/tasks/templates/ner.v2.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tasks/templates/rel.jinja` & `spacy-llm-0.4.1/spacy_llm/tasks/templates/rel.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tasks/templates/sentiment.jinja` & `spacy-llm-0.4.1/spacy_llm/tasks/templates/sentiment.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tasks/templates/spancat.jinja` & `spacy-llm-0.4.1/spacy_llm/tasks/templates/spancat.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tasks/templates/spancat.v2.jinja` & `spacy-llm-0.4.1/spacy_llm/tasks/templates/spancat.v2.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tasks/templates/summarization.jinja` & `spacy-llm-0.4.1/spacy_llm/tasks/templates/summarization.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tasks/templates/textcat.jinja` & `spacy-llm-0.4.1/spacy_llm/tasks/templates/textcat.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tasks/templates/textcat.v2.jinja` & `spacy-llm-0.4.1/spacy_llm/tasks/templates/textcat.v2.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tasks/templates/textcat.v3.jinja` & `spacy-llm-0.4.1/spacy_llm/tasks/templates/textcat.v3.jinja`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tasks/textcat.py` & `spacy-llm-0.4.1/spacy_llm/tasks/textcat.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tasks/util/parsing.py` & `spacy-llm-0.4.1/spacy_llm/tasks/util/parsing.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tasks/util/serialization.py` & `spacy-llm-0.4.1/spacy_llm/tasks/util/serialization.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tests/conftest.py` & `spacy-llm-0.4.1/spacy_llm/tests/conftest.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,34 +9,39 @@
 def pytest_addoption(parser):
     parser.addoption(
         "--external",
         action="store_true",
         default=bool(int(os.environ.get("TEST_EXTERNAL", 0))),
         help="include tests that connects to third-party API",
     )
+    parser.addoption(
+        "--gpu",
+        action="store_true",
+        default=bool(int(os.environ.get("TEST_GPU", 0))),
+        help="include tests that use a GPU",
+    )
 
 
 def pytest_runtest_setup(item):
     def getopt(opt):
         return item.config.getoption(f"--{opt}", False)
 
     # Integration of boolean flags
-    for opt in ["external"]:
+    for opt in ["external", "gpu"]:
         if opt in item.keywords and not getopt(opt):
             pytest.skip(f"need --{opt} option to run")
 
 
 def pytest_collection_modifyitems(config, items):
-    if config.getoption("--external"):
-        return
-
-    skip_external = pytest.mark.skip(reason="need --external option to run")
+    types = ("external", "gpu")
+    skip_marks = [pytest.mark.skip(reason=f"need --{t} option to run") for t in types]
     for item in items:
-        if "external" in item.keywords:
-            item.add_marker(skip_external)
+        for t, sm in zip(types, skip_marks):
+            if (not config.getoption(f"--{t}")) and (t in item.keywords):
+                item.add_marker(sm)
 
 
 @registry.llm_models("test.NoOpModel.v1")
 def noop_factory(output: str = ""):
     def noop(prompts: Iterable[str]) -> Iterable[str]:
         return [output] * len(list(prompts))
```

### Comparing `spacy-llm-0.4.0/spacy_llm/tests/models/test_anthropic.py` & `spacy-llm-0.4.1/spacy_llm/tests/models/test_anthropic.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,32 +31,27 @@
 
 @pytest.mark.external
 @pytest.mark.skipif(has_anthropic_key is False, reason="Anthropic API key unavailable")
 def test_anthropic_api_response_when_error():
     """Check if error message shows up properly given incorrect config"""
     # Incorrect config c.f. https://console.anthropic.com/docs/api/reference
     incorrect_temperature = "one"  # should be an int
-    anthropic = Anthropic(
-        name="claude-instant-1",
-        endpoint=Endpoints.COMPLETIONS.value,
-        config={
-            "max_tokens_to_sample": 10,
-            "temperature": incorrect_temperature,
-        },
-        strict=False,
-        max_tries=10,
-        interval=5.0,
-        max_request_time=20,
-    )
-
-    prompt = "Count the number of characters in this string: hello"
-    with pytest.raises(ValueError) as err:
-        anthropic(prompts=[prompt])
-    assert "invalid_request_error" in str(err.value)
-    assert "temperature: value is not a valid float" in str(err.value)
+    with pytest.raises(ValueError, match="Request to Anthropic API failed:"):
+        Anthropic(
+            name="claude-instant-1",
+            endpoint=Endpoints.COMPLETIONS.value,
+            config={
+                "max_tokens_to_sample": 10,
+                "temperature": incorrect_temperature,
+            },
+            strict=False,
+            max_tries=10,
+            interval=5.0,
+            max_request_time=20,
+        )
 
 
 @pytest.mark.external
 @pytest.mark.skipif(has_anthropic_key is False, reason="Anthropic API key unavailable")
 def test_anthropic_error_unsupported_model():
     """Ensure graceful handling of error when model is not supported"""
     incorrect_model = "x-gpt-3.5-turbo"
```

### Comparing `spacy-llm-0.4.0/spacy_llm/tests/models/test_cohere.py` & `spacy-llm-0.4.1/spacy_llm/tests/models/test_cohere.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import pytest
 
 from spacy_llm.models.rest.cohere import Cohere, Endpoints
 
 from ..compat import has_cohere_key
 
 
+@pytest.mark.external
 @pytest.mark.skipif(has_cohere_key is False, reason="Cohere API key not available")
 def test_cohere_api_response_is_correct():
     """Check if we're getting the response from the correct structure"""
     cohere = Cohere(
         name="command",
         endpoint=Endpoints.COMPLETION.value,
         config={},
@@ -21,14 +22,15 @@
     prompt = "Count the number of characters in this string: hello"
     num_prompts = 3  # arbitrary number to check multiple inputs
     responses = cohere(prompts=[prompt] * num_prompts)
     for response in responses:
         assert isinstance(response, str)
 
 
+@pytest.mark.external
 @pytest.mark.skipif(has_cohere_key is False, reason="Cohere API key not available")
 def test_cohere_api_response_n_generations():
     """Test how the model handles more than 1 generation of output
 
     Users can configure Cohere to return more than 1 output for a single prompt
     The current model doesn't support that and the implementation only returns
     the very first output.
@@ -47,35 +49,34 @@
     prompt = "Count the number of characters in this string: hello"
     num_prompts = 3
     responses = cohere(prompts=[prompt] * num_prompts)
     for response in responses:
         assert isinstance(response, str)
 
 
+@pytest.mark.external
 @pytest.mark.skipif(has_cohere_key is False, reason="Cohere API key not available")
 def test_cohere_api_response_when_error():
     """Ensure graceful handling of error in the Cohere model"""
     # Incorrect config because temperature is in incorrect range [0, 5]
     # c.f. https://docs.cohere.com/reference/generate
     incorrect_temperature = 1000  # must be between 0 and 5
-    cohere = Cohere(
-        name="command",
-        endpoint=Endpoints.COMPLETION.value,
-        config={"temperature": incorrect_temperature},
-        strict=False,
-        max_tries=10,
-        interval=5.0,
-        max_request_time=20,
-    )
-    prompt = "Count the number of characters in this string: hello"
-    num_prompts = 3  # arbitrary number to check multiple inputs
-    with pytest.raises(ValueError):
-        cohere(prompts=[prompt] * num_prompts)
+    with pytest.raises(ValueError, match="Request to Cohere API failed:"):
+        Cohere(
+            name="command",
+            endpoint=Endpoints.COMPLETION.value,
+            config={"temperature": incorrect_temperature},
+            strict=False,
+            max_tries=10,
+            interval=5.0,
+            max_request_time=20,
+        )
 
 
+@pytest.mark.external
 @pytest.mark.skipif(has_cohere_key is False, reason="Cohere API key not available")
 def test_cohere_error_unsupported_model():
     """Ensure graceful handling of error when model is not supported"""
     incorrect_model = "x-gpt-3.5-turbo"
     with pytest.raises(ValueError, match="Model 'x-gpt-3.5-turbo' is not supported"):
         Cohere(
             name=incorrect_model,
```

### Comparing `spacy-llm-0.4.0/spacy_llm/tests/models/test_dolly.py` & `spacy-llm-0.4.1/spacy_llm/tests/models/test_dolly.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,32 +30,35 @@
 
 [components.llm.model]
 @llm_models = "spacy.Dolly.v1"
 name = "dolly-v2-3b"
 """
 
 
+@pytest.mark.gpu
 @pytest.mark.skipif(not has_torch_cuda_gpu, reason="needs GPU & CUDA")
 def test_init():
     """Test initialization and simple run."""
     nlp = spacy.blank("en")
     cfg = copy.deepcopy(_PIPE_CFG)
     cfg["model"]["@llm_models"] = "spacy.Dolly.v1"
     nlp.add_pipe("llm", config=cfg)
     nlp("This is a test.")
     nlp.get_pipe("llm")._model.get_model_names()
 
 
+@pytest.mark.gpu
 @pytest.mark.skipif(not has_torch_cuda_gpu, reason="needs GPU & CUDA")
 def test_init_from_config():
     orig_config = Config().from_str(_NLP_CONFIG)
     nlp = spacy.util.load_model_from_config(orig_config, auto_fill=True)
     assert nlp.pipe_names == ["llm"]
 
 
+@pytest.mark.gpu
 @pytest.mark.skipif(not has_torch_cuda_gpu, reason="needs GPU & CUDA")
 def test_invalid_model():
     orig_config = Config().from_str(_NLP_CONFIG)
     config = copy.deepcopy(orig_config)
     config["components"]["llm"]["model"]["name"] = "dolly-the-sheep"
     with pytest.raises(ValueError, match="unexpected value; permitted"):
         spacy.util.load_model_from_config(config, auto_fill=True)
```

### Comparing `spacy-llm-0.4.0/spacy_llm/tests/models/test_falcon.py` & `spacy-llm-0.4.1/spacy_llm/tests/models/test_falcon.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,30 +30,33 @@
 
 [components.llm.model]
 @llm_models = "spacy.Falcon.v1"
 name = "falcon-rw-1b"
 """
 
 
+@pytest.mark.gpu
 @pytest.mark.skipif(not has_torch_cuda_gpu, reason="needs GPU & CUDA")
 def test_init():
     """Test initialization and simple run."""
     nlp = spacy.blank("en")
     cfg = copy.deepcopy(_PIPE_CFG)
     nlp.add_pipe("llm", config=cfg)
     nlp("This is a test.")
 
 
+@pytest.mark.gpu
 @pytest.mark.skipif(not has_torch_cuda_gpu, reason="needs GPU & CUDA")
 def test_init_from_config():
     orig_config = Config().from_str(_NLP_CONFIG)
     nlp = spacy.util.load_model_from_config(orig_config, auto_fill=True)
     assert nlp.pipe_names == ["llm"]
 
 
+@pytest.mark.gpu
 @pytest.mark.skipif(not has_torch_cuda_gpu, reason="needs GPU & CUDA")
 def test_invalid_model():
     orig_config = Config().from_str(_NLP_CONFIG)
     config = copy.deepcopy(orig_config)
     config["components"]["llm"]["model"]["name"] = "x"
     with pytest.raises(ValueError, match="unexpected value; permitted"):
         spacy.util.load_model_from_config(config, auto_fill=True)
```

### Comparing `spacy-llm-0.4.0/spacy_llm/tests/models/test_langchain.py` & `spacy-llm-0.4.1/spacy_llm/tests/models/test_langchain.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tests/models/test_openllama.py` & `spacy-llm-0.4.1/spacy_llm/tests/models/test_openllama.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import spacy
 from confection import Config  # type: ignore[import]
 from thinc.compat import has_torch_cuda_gpu
 
 _PIPE_CFG = {
     "model": {
         "@llm_models": "spacy.OpenLLaMA.v1",
-        "name": "open_llama_3b_350bt_preview",
+        "name": "open_llama_3b",
     },
     "task": {"@llm_tasks": "spacy.NoOp.v1"},
 }
 
 _NLP_CONFIG = """
 [nlp]
 lang = "en"
@@ -25,43 +25,47 @@
 factory = "llm"
 
 [components.llm.task]
 @llm_tasks = "spacy.NoOp.v1"
 
 [components.llm.model]
 @llm_models = spacy.OpenLLaMA.v1
-name = open_llama_3b_350bt_preview
+name = open_llama_3b
 """
 
 
+@pytest.mark.gpu
 @pytest.mark.skipif(not has_torch_cuda_gpu, reason="needs GPU & CUDA")
 def test_init():
     """Test initialization and simple run."""
     nlp = spacy.blank("en")
     nlp.add_pipe("llm", config=_PIPE_CFG)
     nlp("This is a test.")
 
 
+@pytest.mark.gpu
 @pytest.mark.skipif(not has_torch_cuda_gpu, reason="needs GPU & CUDA")
 def test_init_with_set_config():
     """Test initialization and simple run with changed config."""
     nlp = spacy.blank("en")
     cfg = copy.deepcopy(_PIPE_CFG)
     cfg["model"]["config_run"] = {"max_new_tokens": 32}
     nlp.add_pipe("llm", config=cfg)
     nlp("This is a test.")
 
 
+@pytest.mark.gpu
 @pytest.mark.skipif(not has_torch_cuda_gpu, reason="needs GPU & CUDA")
 def test_init_from_config():
     orig_config = Config().from_str(_NLP_CONFIG)
     nlp = spacy.util.load_model_from_config(orig_config, auto_fill=True)
     assert nlp.pipe_names == ["llm"]
 
 
+@pytest.mark.gpu
 @pytest.mark.skipif(not has_torch_cuda_gpu, reason="needs GPU & CUDA")
 def test_invalid_model():
     orig_config = Config().from_str(_NLP_CONFIG)
     config = copy.deepcopy(orig_config)
     config["components"]["llm"]["model"]["name"] = "anything-else"
     with pytest.raises(ValueError, match="unexpected value; permitted"):
         spacy.util.load_model_from_config(config, auto_fill=True)
```

### Comparing `spacy-llm-0.4.0/spacy_llm/tests/models/test_rest.py` & `spacy-llm-0.4.1/spacy_llm/tests/models/test_rest.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tests/models/test_stablelm.py` & `spacy-llm-0.4.1/spacy_llm/tests/models/test_stablelm.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,44 +29,48 @@
 
 [components.llm.model]
 @llm_models = "spacy.StableLM.v1"
 name = "stablelm-base-alpha-3b"
 """
 
 
-@pytest.mark.parametrize("name", ("stablelm-base-alpha-3b", "stablelm-tuned-alpha-3b"))
+@pytest.mark.gpu
 @pytest.mark.skipif(not has_torch_cuda_gpu, reason="needs GPU & CUDA")
+@pytest.mark.parametrize("name", ("stablelm-base-alpha-3b", "stablelm-tuned-alpha-3b"))
 def test_init(name: str):
     """Test initialization and simple run.
     name (str): Name of model to run.
     """
     nlp = spacy.blank("en")
     cfg = copy.deepcopy(_PIPE_CFG)
     cfg["model"]["name"] = name
     nlp.add_pipe("llm", config=cfg)
     nlp("This is a test.")
 
 
+@pytest.mark.gpu
 @pytest.mark.skipif(not has_torch_cuda_gpu, reason="needs GPU & CUDA")
 def test_init_from_config():
     orig_config = Config().from_str(_NLP_CONFIG)
     nlp = spacy.util.load_model_from_config(orig_config, auto_fill=True)
     assert nlp.pipe_names == ["llm"]
 
 
+@pytest.mark.gpu
 @pytest.mark.skipif(not has_torch_cuda_gpu, reason="needs GPU & CUDA")
 def test_init_with_set_config():
     """Test initialization and simple run with changed config."""
     nlp = spacy.blank("en")
     cfg = copy.deepcopy(_PIPE_CFG)
     cfg["model"]["config_run"] = {"temperature": 0.3}
     nlp.add_pipe("llm", config=cfg)
     nlp("This is a test.")
 
 
+@pytest.mark.gpu
 @pytest.mark.skipif(not has_torch_cuda_gpu, reason="needs GPU & CUDA")
 def test_invalid_model():
     orig_config = Config().from_str(_NLP_CONFIG)
     config = copy.deepcopy(orig_config)
     config["components"]["llm"]["model"]["name"] = "anything-else"
     with pytest.raises(ValueError, match="unexpected value; permitted:"):
         spacy.util.load_model_from_config(config, auto_fill=True)
```

### Comparing `spacy-llm-0.4.0/spacy_llm/tests/pipeline/test_llm.py` & `spacy-llm-0.4.1/spacy_llm/tests/pipeline/test_llm.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/lemma.json` & `spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/lemma.json`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/lemma.jsonl` & `spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/lemma.jsonl`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/lemma.yml` & `spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/lemma.yml`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/rel.jsonl` & `spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/rel.jsonl`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/summarization.json` & `spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/summarization.json`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/summarization.jsonl` & `spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/summarization.jsonl`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tests/tasks/examples/summarization.yml` & `spacy-llm-0.4.1/spacy_llm/tests/tasks/examples/summarization.yml`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tests/tasks/test_lemma.py` & `spacy-llm-0.4.1/spacy_llm/tests/tasks/test_lemma.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tests/tasks/test_ner.py` & `spacy-llm-0.4.1/spacy_llm/tests/tasks/test_ner.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tests/tasks/test_rel.py` & `spacy-llm-0.4.1/spacy_llm/tests/tasks/test_rel.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tests/tasks/test_sentiment.py` & `spacy-llm-0.4.1/spacy_llm/tests/tasks/test_sentiment.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tests/tasks/test_spancat.py` & `spacy-llm-0.4.1/spacy_llm/tests/tasks/test_spancat.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tests/tasks/test_summarization.py` & `spacy-llm-0.4.1/spacy_llm/tests/tasks/test_summarization.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tests/tasks/test_textcat.py` & `spacy-llm-0.4.1/spacy_llm/tests/tasks/test_textcat.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tests/test_cache.py` & `spacy-llm-0.4.1/spacy_llm/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/tests/test_combinations.py` & `spacy-llm-0.4.1/spacy_llm/tests/test_combinations.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/ty.py` & `spacy-llm-0.4.1/spacy_llm/ty.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm/util.py` & `spacy-llm-0.4.1/spacy_llm/util.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/spacy_llm.egg-info/PKG-INFO` & `spacy-llm-0.4.1/spacy_llm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy-llm
-Version: 0.4.0
+Version: 0.4.1
 Summary: Integrating LLMs into structured NLP pipelines
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Project-URL: Release notes, https://github.com/explosion/spacy-llm/releases
 Project-URL: Source, https://github.com/explosion/spacy-llm
 Classifier: Development Status :: 4 - Beta
@@ -1502,22 +1502,22 @@
 ```
 
 Example config block:
 
 ```ini
 [components.llm.model]
 @llm_models = "spacy.OpenLLaMA.v1"
-name = "open_llama_3b_350bt_preview"
+name = "open_llama_3b"
 ```
 
-| Argument      | Type                                                                                                                                  | Default | Description                                                                                                                  |
-| ------------- | ------------------------------------------------------------------------------------------------------------------------------------- | ------- | ---------------------------------------------------------------------------------------------------------------------------- |
-| `name`        | `Literal["open_llama_3b_350bt_preview", "open_llama_3b_600bt_preview", "open_llama_7b_400bt_preview", "open_llama_7b_600bt_preview"]` |         | The name of a OpenLLaMA model that is supported (e. g. "open_llama_3b_350bt_preview").                                       |
-| `config_init` | `Dict[str, Any]`                                                                                                                      | `{}`    | Further configuration passed on to the construction of the model with `transformers.AutoModelForCausalLM.from_pretrained()`. |
-| `config_run`  | `Dict[str, Any]`                                                                                                                      | `{}`    | Further configuration used during model inference.                                                                           |
+| Argument      | Type                                                                                            | Default | Description                                                                                                                  |
+| ------------- |-------------------------------------------------------------------------------------------------| ------- | ---------------------------------------------------------------------------------------------------------------------------- |
+| `name`        | `Literal["open_llama_3b", "open_llama_7b", "open_llama_7b_v2", "open_llama_13b"]` |         | The name of a OpenLLaMA model that is supported.                                       |
+| `config_init` | `Dict[str, Any]`                                                                                | `{}`    | Further configuration passed on to the construction of the model with `transformers.AutoModelForCausalLM.from_pretrained()`. |
+| `config_run`  | `Dict[str, Any]`                                                                                | `{}`    | Further configuration used during model inference.                                                                           |
 
 See the [OpenLM Research OpenLLaMA GitHub repo](https://github.com/openlm-research/open_llama) for details.
 
 Note that Hugging Face will download this model the first time you use it - you can
 [define the cached directory](https://huggingface.co/docs/huggingface_hub/main/en/guides/manage-cache)
 by setting the environmental variable `HF_HOME`.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spacy-llm Version: 0.4.0 Summary: Integrating LLMs
+Metadata-Version: 2.1 Name: spacy-llm Version: 0.4.1 Summary: Integrating LLMs
 into structured NLP pipelines Author: Explosion Author-email:
 contact@explosion.ai License: MIT Project-URL: Release notes, https://
 github.com/explosion/spacy-llm/releases Project-URL: Source, https://
 github.com/explosion/spacy-llm Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: POSIX :: Linux
@@ -927,22 +927,20 @@
 with ```shell python -m pip install "spacy-llm[transformers]" "transformers
 [sentencepiece]" ``` If you don't have access to a GPU, you can install
 `accelerate` and set`device_map=auto` instead, but be aware that this may
 result in some layers getting distributed to the CPU or even the hard drive,
 which may ultimately result in extremely slow queries. ```shell python -m pip
 install "accelerate>=0.16.0,<1.0" ``` Example config block: ```ini
 [components.llm.model] @llm_models = "spacy.OpenLLaMA.v1" name =
-"open_llama_3b_350bt_preview" ``` | Argument | Type | Default | Description | |
-------------- | ---------------------------------------------------------------
----------------------------------------------------------------------- | ------
-- | ---------------------------------------------------------------------------
-------------------------------------------------- | | `name` | `Literal
-["open_llama_3b_350bt_preview", "open_llama_3b_600bt_preview",
-"open_llama_7b_400bt_preview", "open_llama_7b_600bt_preview"]` | | The name of
-a OpenLLaMA model that is supported (e. g. "open_llama_3b_350bt_preview"). | |
+"open_llama_3b" ``` | Argument | Type | Default | Description | | ------------
+- |----------------------------------------------------------------------------
+---------------------| ------- | ----------------------------------------------
+-----------------------------------------------------------------------------
+- | | `name` | `Literal["open_llama_3b", "open_llama_7b", "open_llama_7b_v2",
+"open_llama_13b"]` | | The name of a OpenLLaMA model that is supported. | |
 `config_init` | `Dict[str, Any]` | `{}` | Further configuration passed on to
 the construction of the model with
 `transformers.AutoModelForCausalLM.from_pretrained()`. | | `config_run` | `Dict
 [str, Any]` | `{}` | Further configuration used during model inference. | See
 the [OpenLM Research OpenLLaMA GitHub repo](https://github.com/openlm-research/
 open_llama) for details. Note that Hugging Face will download this model the
 first time you use it - you can [define the cached directory](https://
```

### Comparing `spacy-llm-0.4.0/spacy_llm.egg-info/SOURCES.txt` & `spacy-llm-0.4.1/spacy_llm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/usage_examples/multitask_openai/run_pipeline.py` & `spacy-llm-0.4.1/usage_examples/multitask_openai/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/usage_examples/ner_dolly/run_pipeline.py` & `spacy-llm-0.4.1/usage_examples/ner_dolly/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/usage_examples/ner_langchain_openai/run_pipeline.py` & `spacy-llm-0.4.1/usage_examples/ner_langchain_openai/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/usage_examples/rel_openai/run_pipeline.py` & `spacy-llm-0.4.1/usage_examples/rel_openai/run_pipeline.py`

 * *Files identical despite different names*

### Comparing `spacy-llm-0.4.0/usage_examples/tests/test_readme_examples.py` & `spacy-llm-0.4.1/usage_examples/tests/test_readme_examples.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,15 @@
             text_file.write(cfg_str)
 
         nlp = assemble(tmpdir / "cfg")
         doc = nlp("You look gorgeous!")
         print(doc.cats)  # noqa: T201
 
 
+@pytest.mark.gpu
 @pytest.mark.skipif(not has_torch_cuda_gpu, reason="needs GPU & CUDA")
 def test_example_2_ner_hf():
     with util.make_tempdir() as tmpdir:
         cfg_str = """
         [nlp]
         lang = "en"
         pipeline = ["llm"]
```

### Comparing `spacy-llm-0.4.0/usage_examples/tests/test_usage_examples.py` & `spacy-llm-0.4.1/usage_examples/tests/test_usage_examples.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from .. import multitask_openai, ner_dolly, ner_langchain_openai, rel_openai
 from .. import textcat_openai
 
 _USAGE_EXAMPLE_PATH = Path(__file__).parent.parent
 
 
+@pytest.mark.gpu
 @pytest.mark.skipif(not has_torch_cuda_gpu, reason="needs GPU & CUDA")
 @pytest.mark.parametrize("config_name", ("fewshot.cfg", "zeroshot.cfg"))
 def test_ner_dolly(config_name: str):
     """Test NER Dolly usage example.
     config_name (str): Name of config file to use.
     """
     path = _USAGE_EXAMPLE_PATH / "ner_dolly"
```

### Comparing `spacy-llm-0.4.0/usage_examples/textcat_openai/run_pipeline.py` & `spacy-llm-0.4.1/usage_examples/textcat_openai/run_pipeline.py`

 * *Files identical despite different names*

