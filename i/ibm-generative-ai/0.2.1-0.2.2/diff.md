# Comparing `tmp/ibm-generative-ai-0.2.1.tar.gz` & `tmp/ibm-generative-ai-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibm-generative-ai-0.2.1.tar", last modified: Mon Jul 10 21:53:12 2023, max compression
+gzip compressed data, was "ibm-generative-ai-0.2.2.tar", last modified: Tue Jul 11 17:19:45 2023, max compression
```

## Comparing `ibm-generative-ai-0.2.1.tar` & `ibm-generative-ai-0.2.2.tar`

### file list

```diff
@@ -1,270 +1,272 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:53:12.194332 ibm-generative-ai-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:53:12.158332 ibm-generative-ai-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:53:12.158332 ibm-generative-ai-0.2.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/.github/ISSUE_TEMPLATE/01_bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/.github/ISSUE_TEMPLATE/02_feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/.github/ISSUE_TEMPLATE/03_documentation_update.md
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/.github/ISSUE_TEMPLATE/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:53:12.158332 ibm-generative-ai-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/.github/workflows/documentation.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/.github/workflows/integration-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/EXTENSIONS.md
--rw-r--r--   0 runner    (1001) docker     (123)     9706 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/GETTING_STARTED.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-10 21:53:12.194332 ibm-generative-ai-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/STARTER_TEAM.md
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/SUPPORT.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:53:12.158332 ibm-generative-ai-0.2.1/documentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/documentation/.nojekyll
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:53:12.162332 ibm-generative-ai-0.2.1/documentation/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    39195 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/documentation/assets/pull_request_from_fork_to_base.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:53:12.162332 ibm-generative-ai-0.2.1/documentation/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/documentation/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:53:12.162332 ibm-generative-ai-0.2.1/documentation/docs/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/documentation/docs/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/documentation/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:53:12.162332 ibm-generative-ai-0.2.1/documentation/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:53:12.162332 ibm-generative-ai-0.2.1/documentation/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/documentation/docs/source/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:53:12.162332 ibm-generative-ai-0.2.1/documentation/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/documentation/docs/source/_templates/custom_landing_page.html
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/documentation/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/documentation/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:53:12.166332 ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:53:12.166332 ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/examples/async.examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/examples/async.examples.user.rst
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/examples/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/examples/examples.user.rst
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/examples/extensions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/examples/extensions.user.rst
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/examples/prompts.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/examples/prompts.user.rst
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/genai.credentials.rst
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/genai.exceptions.genai_exception.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/genai.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/genai.metadata.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/genai.model.rst
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/genai.prompt.prompt_pattern.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/genai.prompt.quickstart.annexe.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9306 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/genai.prompt.quickstart.basics.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/genai.prompt.quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/genai.prompt.rst
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/genai.rst
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/genai.schemas.descriptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/genai.schemas.generate_params.rst
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/genai.schemas.history_params.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/genai.schemas.models.rst
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/genai.schemas.responses.rst
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/genai.schemas.rst
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/genai.schemas.token_params.rst
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/genai.services.request_handler.rst
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/genai.services.rst
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/genai.services.service_interface.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/local_server.rst
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:53:12.154332 ibm-generative-ai-0.2.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:53:12.170332 ibm-generative-ai-0.2.1/examples/dev/
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/dev/async-flaky-request-handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/dev/async-flaky-responses-ordered.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/dev/generate-all-models.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/dev/history-async.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/dev/load_token_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/dev/logging_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:53:12.174332 ibm-generative-ai-0.2.1/examples/user/
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/alice_bob_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/alice_bob_talk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:53:12.174332 ibm-generative-ai-0.2.1/examples/user/assets/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/assets/country-capital.csv
--rw-r--r--   0 runner    (1001) docker     (123)    19258 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/assets/penguins.csv
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/assets/penguins2.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/assets/seed_tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)   110931 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/assets/seed_tasks.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/async_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/async_greetings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/async_ordered.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/async_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/complete_my_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/country-capital-qa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/explain_my_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/generate_with_input_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/gpt_chat_bash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/grid_search_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/grid_search_params_greeating.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/history.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/jsonprompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/jsonprompt_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/langchain_qa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:53:12.174332 ibm-generative-ai-0.2.1/examples/user/localserver/
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/localserver/localserver.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/localserver/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/logprob_returns.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/many_greetings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/model_as_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/prompt-raw-string.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/prompt_csv_random_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/prompt_from_all_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/prompt_from_all_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/prompt_from_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/prompt_reuse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:53:12.174332 ibm-generative-ai-0.2.1/examples/user/prompt_templating/
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/prompt_templating/watsonx-prompt-output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/prompt_templating/watsonx-prompt-pattern-ux-async.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/prompt_templating/watsonx-prompt-pattern-ux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/prompt_templating/watsonx-prompt-templating.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:53:12.178332 ibm-generative-ai-0.2.1/examples/user/prompt_tuning/
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/prompt_tuning/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/prompt_tuning/file_to_tune.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/prompt_tuning/files_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/prompt_tuning/summarization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:53:12.178332 ibm-generative-ai-0.2.1/examples/user/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/prompts/Country-Capital-Factual-QA
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:53:12.178332 ibm-generative-ai-0.2.1/examples/user/prompts_adult_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/prompts_adult_dataset/prompt_generation_with_column_idx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/prompts_adult_dataset/prompt_generation_with_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/saving_prompts_as_hf_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/self-reflection.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/self_instruct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/streaming.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:53:12.178332 ibm-generative-ai-0.2.1/examples/user/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/templates/capital-qa.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/templates/instruction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/templates/qa.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/templates/self-reflection.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/templates/synth-animal.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/tokenize-sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/examples/user/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/innersource.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 21:53:12.194332 ibm-generative-ai-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:53:12.154332 ibm-generative-ai-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:53:12.178332 ibm-generative-ai-0.2.1/src/genai/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-10 21:53:11.000000 ibm-generative-ai-0.2.1/src/genai/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:53:12.178332 ibm-generative-ai-0.2.1/src/genai/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/exceptions/genai_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:53:12.154332 ibm-generative-ai-0.2.1/src/genai/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:53:12.178332 ibm-generative-ai-0.2.1/src/genai/extensions/huggingface/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/extensions/huggingface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/extensions/huggingface/save_huggingface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:53:12.182332 ibm-generative-ai-0.2.1/src/genai/extensions/langchain/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/extensions/langchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/extensions/langchain/llm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/extensions/langchain/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:53:12.182332 ibm-generative-ai-0.2.1/src/genai/extensions/localserver/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/extensions/localserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/extensions/localserver/custom_model_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/extensions/localserver/local_api_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/extensions/localserver/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:53:12.182332 ibm-generative-ai-0.2.1/src/genai/extensions/pandas/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/extensions/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/extensions/pandas/prompt_sub.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    15441 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    24219 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/prompt_pattern.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:53:12.182332 ibm-generative-ai-0.2.1/src/genai/routers/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/routers/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/routers/prompt_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/routers/tunes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:53:12.182332 ibm-generative-ai-0.2.1/src/genai/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7887 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/schemas/descriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/schemas/files_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/schemas/generate_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/schemas/history_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/schemas/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/schemas/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/schemas/token_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/schemas/tunes_params.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:53:12.186332 ibm-generative-ai-0.2.1/src/genai/services/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/services/async_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/services/connection_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/services/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/services/prompt_template_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    12951 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/services/request_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/services/service_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/services/tune_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:53:12.186332 ibm-generative-ai-0.2.1/src/genai/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/utils/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/utils/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/utils/request_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/utils/search_space_params.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/utils/service_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/src/genai/utils/watsonx_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:53:12.186332 ibm-generative-ai-0.2.1/src/ibm_generative_ai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-10 21:53:12.000000 ibm-generative-ai-0.2.1/src/ibm_generative_ai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8716 2023-07-10 21:53:12.000000 ibm-generative-ai-0.2.1/src/ibm_generative_ai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 21:53:12.000000 ibm-generative-ai-0.2.1/src/ibm_generative_ai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-10 21:53:12.000000 ibm-generative-ai-0.2.1/src/ibm_generative_ai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 21:53:12.000000 ibm-generative-ai-0.2.1/src/ibm_generative_ai.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:53:12.190332 ibm-generative-ai-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:53:12.194332 ibm-generative-ai-0.2.1/tests/assets/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/assets/age-gender.csv
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/assets/capital-qa-content.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/assets/capital-qa-multivar.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/assets/capital-qa-sub-noheader.csv
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/assets/capital-qa-sub.csv
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/assets/capital-qa-sub.json
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/assets/capital-qa-sub.txt
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/assets/capital-qa.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/assets/csv_file.csv
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/assets/csv_file.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/assets/file_to_tune.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/assets/file_to_tune.json
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/assets/file_to_tune.jsonl
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/assets/invalid-content-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/assets/invalid-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/assets/penguins.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/assets/prompt_contents.csv
--rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/assets/response_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/assets/story.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/assets/story_sub.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:53:12.194332 ibm-generative-ai-0.2.1/tests/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/extensions/test_langchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/extensions/test_localserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/extensions/test_save_huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/extensions/test_sub_from_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 21:53:12.194332 ibm-generative-ai-0.2.1/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/integration/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/integration/test_terms_of_use.py
--rw-r--r--   0 runner    (1001) docker     (123)    19430 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/test_concurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     9487 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)    10753 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/test_generate_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/test_generate_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/test_history.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/test_json_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/test_model_async.py
--rw-r--r--   0 runner    (1001) docker     (123)    14265 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/test_prompt_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/test_prompt_pattern_watsonx.py
--rw-r--r--   0 runner    (1001) docker     (123)    12442 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/test_prompt_template_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/test_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/test_schema_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/test_service_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/test_service_interface_async.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/test_service_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/test_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/test_tunes.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-10 21:52:35.000000 ibm-generative-ai-0.2.1/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.983202 ibm-generative-ai-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.935201 ibm-generative-ai-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.939201 ibm-generative-ai-0.2.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/.github/ISSUE_TEMPLATE/01_bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/.github/ISSUE_TEMPLATE/02_feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/.github/ISSUE_TEMPLATE/03_documentation_update.md
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/.github/ISSUE_TEMPLATE/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.939201 ibm-generative-ai-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/.github/workflows/documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/.github/workflows/integration-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5879 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/EXTENSIONS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9706 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/GETTING_STARTED.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-11 17:19:45.983202 ibm-generative-ai-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/STARTER_TEAM.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/SUPPORT.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.939201 ibm-generative-ai-0.2.2/documentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/.nojekyll
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.939201 ibm-generative-ai-0.2.2/documentation/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    39195 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/assets/pull_request_from_fork_to_base.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.939201 ibm-generative-ai-0.2.2/documentation/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.939201 ibm-generative-ai-0.2.2/documentation/docs/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.939201 ibm-generative-ai-0.2.2/documentation/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.939201 ibm-generative-ai-0.2.2/documentation/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.939201 ibm-generative-ai-0.2.2/documentation/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/_templates/custom_landing_page.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.947201 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.947201 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/examples/async.examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/examples/async.examples.user.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/examples/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/examples/examples.user.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/examples/extensions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/examples/extensions.user.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/examples/prompts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/examples/prompts.user.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.credentials.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.exceptions.genai_exception.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.prompt.prompt_pattern.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.prompt.quickstart.annexe.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9306 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.prompt.quickstart.basics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.prompt.quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.prompt.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.schemas.descriptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.schemas.files_params.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.schemas.generate_params.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.schemas.history_params.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.schemas.models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.schemas.responses.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.schemas.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.schemas.token_params.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.schemas.tunes_params.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.services.request_handler.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.services.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.services.service_interface.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/local_server.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.927201 ibm-generative-ai-0.2.2/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.947201 ibm-generative-ai-0.2.2/examples/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/dev/async-flaky-request-handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/dev/async-flaky-responses-ordered.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/dev/generate-all-models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/dev/history-async.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/dev/load_token_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/dev/logging_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.955201 ibm-generative-ai-0.2.2/examples/user/
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/alice_bob_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/alice_bob_talk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.955201 ibm-generative-ai-0.2.2/examples/user/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/assets/country-capital.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    19258 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/assets/penguins.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/assets/penguins2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/assets/seed_tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)   110931 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/assets/seed_tasks.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/async_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/async_greetings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/async_ordered.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/async_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/complete_my_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/country-capital-qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/explain_my_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/generate_with_input_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/gpt_chat_bash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/grid_search_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/grid_search_params_greeating.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/jsonprompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/jsonprompt_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/langchain_qa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.959201 ibm-generative-ai-0.2.2/examples/user/localserver/
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/localserver/localserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/localserver/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/logprob_returns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/many_greetings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/model_as_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/prompt-raw-string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/prompt_csv_random_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/prompt_from_all_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/prompt_from_all_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/prompt_from_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/prompt_reuse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.959201 ibm-generative-ai-0.2.2/examples/user/prompt_templating/
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/prompt_templating/watsonx-prompt-output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/prompt_templating/watsonx-prompt-pattern-ux-async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/prompt_templating/watsonx-prompt-pattern-ux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/prompt_templating/watsonx-prompt-templating.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.959201 ibm-generative-ai-0.2.2/examples/user/prompt_tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/prompt_tuning/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/prompt_tuning/file_to_tune.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/prompt_tuning/files_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/prompt_tuning/summarization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.959201 ibm-generative-ai-0.2.2/examples/user/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/prompts/Country-Capital-Factual-QA
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.963202 ibm-generative-ai-0.2.2/examples/user/prompts_adult_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/prompts_adult_dataset/prompt_generation_with_column_idx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/prompts_adult_dataset/prompt_generation_with_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/saving_prompts_as_hf_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/self-reflection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/self_instruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/streaming.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.963202 ibm-generative-ai-0.2.2/examples/user/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/templates/capital-qa.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/templates/instruction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/templates/qa.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/templates/self-reflection.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/templates/synth-animal.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/tokenize-sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/examples/user/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/innersource.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 17:19:45.983202 ibm-generative-ai-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.931201 ibm-generative-ai-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.963202 ibm-generative-ai-0.2.2/src/genai/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-11 17:19:45.000000 ibm-generative-ai-0.2.2/src/genai/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.963202 ibm-generative-ai-0.2.2/src/genai/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/exceptions/genai_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.931201 ibm-generative-ai-0.2.2/src/genai/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.963202 ibm-generative-ai-0.2.2/src/genai/extensions/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/extensions/huggingface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/extensions/huggingface/save_huggingface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.963202 ibm-generative-ai-0.2.2/src/genai/extensions/langchain/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/extensions/langchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/extensions/langchain/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/extensions/langchain/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.967202 ibm-generative-ai-0.2.2/src/genai/extensions/localserver/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/extensions/localserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/extensions/localserver/custom_model_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/extensions/localserver/local_api_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/extensions/localserver/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.967202 ibm-generative-ai-0.2.2/src/genai/extensions/pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/extensions/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/extensions/pandas/prompt_sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15441 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24219 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/prompt_pattern.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.967202 ibm-generative-ai-0.2.2/src/genai/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/routers/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/routers/prompt_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/routers/tunes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.967202 ibm-generative-ai-0.2.2/src/genai/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7887 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/schemas/descriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/schemas/files_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/schemas/generate_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/schemas/history_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/schemas/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/schemas/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/schemas/token_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/schemas/tunes_params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.971202 ibm-generative-ai-0.2.2/src/genai/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/services/async_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/services/connection_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/services/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/services/prompt_template_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12951 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/services/request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/services/service_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/services/tune_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.971202 ibm-generative-ai-0.2.2/src/genai/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/utils/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/utils/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/utils/request_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/utils/search_space_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/utils/service_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/src/genai/utils/watsonx_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.971202 ibm-generative-ai-0.2.2/src/ibm_generative_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-07-11 17:19:45.000000 ibm-generative-ai-0.2.2/src/ibm_generative_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8852 2023-07-11 17:19:45.000000 ibm-generative-ai-0.2.2/src/ibm_generative_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 17:19:45.000000 ibm-generative-ai-0.2.2/src/ibm_generative_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-11 17:19:45.000000 ibm-generative-ai-0.2.2/src/ibm_generative_ai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 17:19:45.000000 ibm-generative-ai-0.2.2/src/ibm_generative_ai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.975202 ibm-generative-ai-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.979202 ibm-generative-ai-0.2.2/tests/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/assets/age-gender.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/assets/capital-qa-content.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/assets/capital-qa-multivar.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/assets/capital-qa-sub-noheader.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/assets/capital-qa-sub.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/assets/capital-qa-sub.json
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/assets/capital-qa-sub.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/assets/capital-qa.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/assets/csv_file.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/assets/csv_file.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/assets/file_to_tune.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/assets/file_to_tune.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/assets/file_to_tune.jsonl
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/assets/invalid-content-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/assets/invalid-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/assets/penguins.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/assets/prompt_contents.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/assets/response_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/assets/story.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/assets/story_sub.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.983202 ibm-generative-ai-0.2.2/tests/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/extensions/test_langchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/extensions/test_localserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/extensions/test_save_huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/extensions/test_sub_from_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:19:45.983202 ibm-generative-ai-0.2.2/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/integration/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/integration/test_terms_of_use.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19430 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9487 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10753 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_generate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_generate_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_model_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14265 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_prompt_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_prompt_pattern_watsonx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12442 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_prompt_template_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_schema_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_service_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_service_interface_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_service_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_tunes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-11 17:19:19.000000 ibm-generative-ai-0.2.2/tests/test_version.py
```

### Comparing `ibm-generative-ai-0.2.1/.github/ISSUE_TEMPLATE/01_bug_report.md` & `ibm-generative-ai-0.2.2/.github/ISSUE_TEMPLATE/01_bug_report.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/.github/ISSUE_TEMPLATE/02_feature_request.md` & `ibm-generative-ai-0.2.2/.github/ISSUE_TEMPLATE/02_feature_request.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/.github/ISSUE_TEMPLATE/03_documentation_update.md` & `ibm-generative-ai-0.2.2/.github/ISSUE_TEMPLATE/03_documentation_update.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/.github/PULL_REQUEST_TEMPLATE.md` & `ibm-generative-ai-0.2.2/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/.github/workflows/documentation.yml` & `ibm-generative-ai-0.2.2/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/.github/workflows/integration-test.yml` & `ibm-generative-ai-0.2.2/.github/workflows/integration-test.yml`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/.github/workflows/main.yml` & `ibm-generative-ai-0.2.2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/.github/workflows/python-publish.yml` & `ibm-generative-ai-0.2.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/.gitignore` & `ibm-generative-ai-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/.pre-commit-config.yaml` & `ibm-generative-ai-0.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/CODE_OF_CONDUCT.md` & `ibm-generative-ai-0.2.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/CONTRIBUTING.md` & `ibm-generative-ai-0.2.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/EXTENSIONS.md` & `ibm-generative-ai-0.2.2/EXTENSIONS.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/GETTING_STARTED.md` & `ibm-generative-ai-0.2.2/GETTING_STARTED.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/LICENSE` & `ibm-generative-ai-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/PKG-INFO` & `ibm-generative-ai-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibm-generative-ai
-Version: 0.2.1
+Version: 0.2.2
 Summary: IBM Generative AI is a Python library built on IBM's large language model REST interface.
 Author-email: Lee Martie <lee.martie@ibm.com>, Ana Fucs <ana.fucs@ibm.com>, Veronique Demers <vdemers@ibm.com>, Mairead O'Neill <moneill@ibm.com>, Mirian Silva <mirianfrsilva@ibm.com>, Onkar Bhardwaj <onkarbhardwaj@ibm.com>, James Sutton <james.sutton@uk.ibm.com>, Ja Young Lee <younglee@ibm.com>, Adriana Meza Soria <adriana.meza.soria@ibm.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: langchain
 Provides-Extra: huggingface
```

### Comparing `ibm-generative-ai-0.2.1/README.md` & `ibm-generative-ai-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/STARTER_TEAM.md` & `ibm-generative-ai-0.2.2/STARTER_TEAM.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/SUPPORT.md` & `ibm-generative-ai-0.2.2/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/documentation/assets/pull_request_from_fork_to_base.png` & `ibm-generative-ai-0.2.2/documentation/assets/pull_request_from_fork_to_base.png`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/documentation/docs/Makefile` & `ibm-generative-ai-0.2.2/documentation/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/documentation/docs/make.bat` & `ibm-generative-ai-0.2.2/documentation/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/documentation/docs/source/_templates/custom_landing_page.html` & `ibm-generative-ai-0.2.2/documentation/docs/source/_templates/custom_landing_page.html`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/documentation/docs/source/conf.py` & `ibm-generative-ai-0.2.2/documentation/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/documentation/docs/source/index.rst` & `ibm-generative-ai-0.2.2/documentation/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/examples/async.examples.user.rst` & `ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/examples/async.examples.user.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/examples/examples.user.rst` & `ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/examples/examples.user.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/examples/extensions.user.rst` & `ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/examples/extensions.user.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/examples/prompts.user.rst` & `ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/examples/prompts.user.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/genai.prompt.quickstart.annexe.rst` & `ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.prompt.quickstart.annexe.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/genai.prompt.quickstart.basics.rst` & `ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.prompt.quickstart.basics.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/genai.prompt.quickstart.rst` & `ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/genai.prompt.quickstart.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/documentation/docs/source/rst_source/local_server.rst` & `ibm-generative-ai-0.2.2/documentation/docs/source/rst_source/local_server.rst`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/dev/async-flaky-request-handler.py` & `ibm-generative-ai-0.2.2/examples/dev/async-flaky-request-handler.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/dev/async-flaky-responses-ordered.py` & `ibm-generative-ai-0.2.2/examples/dev/async-flaky-responses-ordered.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/dev/generate-all-models.py` & `ibm-generative-ai-0.2.2/examples/dev/generate-all-models.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/dev/history-async.py` & `ibm-generative-ai-0.2.2/examples/dev/history-async.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/dev/logging_example.py` & `ibm-generative-ai-0.2.2/examples/dev/logging_example.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/alice_bob_qa.py` & `ibm-generative-ai-0.2.2/examples/user/alice_bob_qa.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/alice_bob_talk.py` & `ibm-generative-ai-0.2.2/examples/user/alice_bob_talk.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/assets/penguins.csv` & `ibm-generative-ai-0.2.2/examples/user/assets/penguins.csv`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/assets/penguins2.csv` & `ibm-generative-ai-0.2.2/examples/user/assets/penguins2.csv`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/assets/seed_tasks.json` & `ibm-generative-ai-0.2.2/examples/user/assets/seed_tasks.json`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/assets/seed_tasks.jsonl` & `ibm-generative-ai-0.2.2/examples/user/assets/seed_tasks.jsonl`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/async_callback.py` & `ibm-generative-ai-0.2.2/examples/user/async_callback.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/async_greetings.py` & `ibm-generative-ai-0.2.2/examples/user/async_greetings.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/async_ordered.py` & `ibm-generative-ai-0.2.2/examples/user/async_ordered.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/async_tokenize.py` & `ibm-generative-ai-0.2.2/examples/user/async_tokenize.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/complete_my_code.py` & `ibm-generative-ai-0.2.2/examples/user/complete_my_code.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/country-capital-qa.py` & `ibm-generative-ai-0.2.2/examples/user/country-capital-qa.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/explain_my_code.py` & `ibm-generative-ai-0.2.2/examples/user/explain_my_code.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/generate_with_input_text.py` & `ibm-generative-ai-0.2.2/examples/user/generate_with_input_text.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/gpt_chat_bash.py` & `ibm-generative-ai-0.2.2/examples/user/gpt_chat_bash.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/grid_search_params.py` & `ibm-generative-ai-0.2.2/examples/user/grid_search_params.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/grid_search_params_greeating.py` & `ibm-generative-ai-0.2.2/examples/user/grid_search_params_greeating.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/history.py` & `ibm-generative-ai-0.2.2/examples/user/history.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/jsonprompt.py` & `ibm-generative-ai-0.2.2/examples/user/jsonprompt.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/jsonprompt_multi.py` & `ibm-generative-ai-0.2.2/examples/user/jsonprompt_multi.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/langchain_qa.py` & `ibm-generative-ai-0.2.2/examples/user/langchain_qa.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/localserver/localserver.py` & `ibm-generative-ai-0.2.2/examples/user/localserver/localserver.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/logprob_returns.py` & `ibm-generative-ai-0.2.2/examples/user/logprob_returns.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/many_greetings.py` & `ibm-generative-ai-0.2.2/examples/user/many_greetings.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/model_as_string.py` & `ibm-generative-ai-0.2.2/examples/user/model_as_string.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/prompt-raw-string.py` & `ibm-generative-ai-0.2.2/examples/user/prompt-raw-string.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/prompt_csv_random_rows.py` & `ibm-generative-ai-0.2.2/examples/user/prompt_csv_random_rows.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/prompt_from_all_csv.py` & `ibm-generative-ai-0.2.2/examples/user/prompt_from_all_csv.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/prompt_from_all_dataframe.py` & `ibm-generative-ai-0.2.2/examples/user/prompt_from_all_dataframe.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/prompt_from_dataframe.py` & `ibm-generative-ai-0.2.2/examples/user/prompt_from_dataframe.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/prompt_reuse.py` & `ibm-generative-ai-0.2.2/examples/user/prompt_reuse.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/prompt_templating/watsonx-prompt-output.py` & `ibm-generative-ai-0.2.2/examples/user/prompt_templating/watsonx-prompt-output.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/prompt_templating/watsonx-prompt-pattern-ux-async.py` & `ibm-generative-ai-0.2.2/examples/user/prompt_templating/watsonx-prompt-pattern-ux-async.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/prompt_templating/watsonx-prompt-pattern-ux.py` & `ibm-generative-ai-0.2.2/examples/user/prompt_templating/watsonx-prompt-pattern-ux.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/prompt_templating/watsonx-prompt-templating.py` & `ibm-generative-ai-0.2.2/examples/user/prompt_templating/watsonx-prompt-templating.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/prompt_tuning/classification.py` & `ibm-generative-ai-0.2.2/examples/user/prompt_tuning/classification.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/prompt_tuning/file_to_tune.jsonl` & `ibm-generative-ai-0.2.2/examples/user/prompt_tuning/file_to_tune.jsonl`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/prompt_tuning/files_manager.py` & `ibm-generative-ai-0.2.2/examples/user/prompt_tuning/files_manager.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/prompt_tuning/summarization.py` & `ibm-generative-ai-0.2.2/examples/user/prompt_tuning/summarization.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/prompts_adult_dataset/prompt_generation_with_column_idx.py` & `ibm-generative-ai-0.2.2/examples/user/prompts_adult_dataset/prompt_generation_with_column_idx.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/prompts_adult_dataset/prompt_generation_with_headers.py` & `ibm-generative-ai-0.2.2/examples/user/prompts_adult_dataset/prompt_generation_with_headers.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/saving_prompts_as_hf_dataset.py` & `ibm-generative-ai-0.2.2/examples/user/saving_prompts_as_hf_dataset.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/self-reflection.py` & `ibm-generative-ai-0.2.2/examples/user/self-reflection.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/self_instruct.py` & `ibm-generative-ai-0.2.2/examples/user/self_instruct.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/streaming.py` & `ibm-generative-ai-0.2.2/examples/user/streaming.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/tokenize-sync.py` & `ibm-generative-ai-0.2.2/examples/user/tokenize-sync.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/examples/user/tokens.py` & `ibm-generative-ai-0.2.2/examples/user/tokens.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/pyproject.toml` & `ibm-generative-ai-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/src/genai/credentials.py` & `ibm-generative-ai-0.2.2/src/genai/credentials.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/src/genai/exceptions/genai_exception.py` & `ibm-generative-ai-0.2.2/src/genai/exceptions/genai_exception.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/src/genai/extensions/huggingface/save_huggingface.py` & `ibm-generative-ai-0.2.2/src/genai/extensions/huggingface/save_huggingface.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/src/genai/extensions/langchain/llm.py` & `ibm-generative-ai-0.2.2/src/genai/extensions/langchain/llm.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/src/genai/extensions/langchain/prompt.py` & `ibm-generative-ai-0.2.2/src/genai/extensions/langchain/prompt.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/src/genai/extensions/localserver/custom_model_interface.py` & `ibm-generative-ai-0.2.2/src/genai/extensions/localserver/custom_model_interface.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/src/genai/extensions/localserver/local_api_server.py` & `ibm-generative-ai-0.2.2/src/genai/extensions/localserver/local_api_server.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/src/genai/extensions/pandas/prompt_sub.py` & `ibm-generative-ai-0.2.2/src/genai/extensions/pandas/prompt_sub.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/src/genai/metadata.py` & `ibm-generative-ai-0.2.2/src/genai/metadata.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/src/genai/model.py` & `ibm-generative-ai-0.2.2/src/genai/model.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/src/genai/prompt_pattern.py` & `ibm-generative-ai-0.2.2/src/genai/prompt_pattern.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/src/genai/routers/files.py` & `ibm-generative-ai-0.2.2/src/genai/routers/files.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/src/genai/routers/prompt_template.py` & `ibm-generative-ai-0.2.2/src/genai/routers/prompt_template.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/src/genai/routers/tunes.py` & `ibm-generative-ai-0.2.2/src/genai/routers/tunes.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/src/genai/schemas/__init__.py` & `ibm-generative-ai-0.2.2/src/genai/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/src/genai/schemas/descriptions.py` & `ibm-generative-ai-0.2.2/src/genai/schemas/descriptions.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/src/genai/schemas/files_params.py` & `ibm-generative-ai-0.2.2/src/genai/schemas/files_params.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/src/genai/schemas/generate_params.py` & `ibm-generative-ai-0.2.2/src/genai/schemas/generate_params.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/src/genai/schemas/history_params.py` & `ibm-generative-ai-0.2.2/src/genai/schemas/history_params.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/src/genai/schemas/models.py` & `ibm-generative-ai-0.2.2/src/genai/schemas/models.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/src/genai/schemas/responses.py` & `ibm-generative-ai-0.2.2/src/genai/schemas/responses.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/src/genai/schemas/tunes_params.py` & `ibm-generative-ai-0.2.2/src/genai/schemas/tunes_params.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/src/genai/services/__init__.py` & `ibm-generative-ai-0.2.2/src/genai/services/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/src/genai/services/async_generator.py` & `ibm-generative-ai-0.2.2/src/genai/services/async_generator.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/src/genai/services/connection_manager.py` & `ibm-generative-ai-0.2.2/src/genai/services/connection_manager.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/src/genai/services/file_manager.py` & `ibm-generative-ai-0.2.2/src/genai/services/file_manager.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/src/genai/services/prompt_template_manager.py` & `ibm-generative-ai-0.2.2/src/genai/services/prompt_template_manager.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/src/genai/services/request_handler.py` & `ibm-generative-ai-0.2.2/src/genai/services/request_handler.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/src/genai/services/service_interface.py` & `ibm-generative-ai-0.2.2/src/genai/services/service_interface.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/src/genai/services/tune_manager.py` & `ibm-generative-ai-0.2.2/src/genai/services/tune_manager.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/src/genai/utils/extensions.py` & `ibm-generative-ai-0.2.2/src/genai/utils/extensions.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/src/genai/utils/json_utils.py` & `ibm-generative-ai-0.2.2/src/genai/utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/src/genai/utils/search_space_params.py` & `ibm-generative-ai-0.2.2/src/genai/utils/search_space_params.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/src/genai/utils/service_utils.py` & `ibm-generative-ai-0.2.2/src/genai/utils/service_utils.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/src/ibm_generative_ai.egg-info/PKG-INFO` & `ibm-generative-ai-0.2.2/src/ibm_generative_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibm-generative-ai
-Version: 0.2.1
+Version: 0.2.2
 Summary: IBM Generative AI is a Python library built on IBM's large language model REST interface.
 Author-email: Lee Martie <lee.martie@ibm.com>, Ana Fucs <ana.fucs@ibm.com>, Veronique Demers <vdemers@ibm.com>, Mairead O'Neill <moneill@ibm.com>, Mirian Silva <mirianfrsilva@ibm.com>, Onkar Bhardwaj <onkarbhardwaj@ibm.com>, James Sutton <james.sutton@uk.ibm.com>, Ja Young Lee <younglee@ibm.com>, Adriana Meza Soria <adriana.meza.soria@ibm.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: langchain
 Provides-Extra: huggingface
```

### Comparing `ibm-generative-ai-0.2.1/src/ibm_generative_ai.egg-info/SOURCES.txt` & `ibm-generative-ai-0.2.2/src/ibm_generative_ai.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -38,20 +38,22 @@
 documentation/docs/source/rst_source/genai.prompt.prompt_pattern.rst
 documentation/docs/source/rst_source/genai.prompt.quickstart.annexe.rst
 documentation/docs/source/rst_source/genai.prompt.quickstart.basics.rst
 documentation/docs/source/rst_source/genai.prompt.quickstart.rst
 documentation/docs/source/rst_source/genai.prompt.rst
 documentation/docs/source/rst_source/genai.rst
 documentation/docs/source/rst_source/genai.schemas.descriptions.rst
+documentation/docs/source/rst_source/genai.schemas.files_params.rst
 documentation/docs/source/rst_source/genai.schemas.generate_params.rst
 documentation/docs/source/rst_source/genai.schemas.history_params.rst
 documentation/docs/source/rst_source/genai.schemas.models.rst
 documentation/docs/source/rst_source/genai.schemas.responses.rst
 documentation/docs/source/rst_source/genai.schemas.rst
 documentation/docs/source/rst_source/genai.schemas.token_params.rst
+documentation/docs/source/rst_source/genai.schemas.tunes_params.rst
 documentation/docs/source/rst_source/genai.services.request_handler.rst
 documentation/docs/source/rst_source/genai.services.rst
 documentation/docs/source/rst_source/genai.services.service_interface.rst
 documentation/docs/source/rst_source/local_server.rst
 documentation/docs/source/rst_source/modules.rst
 documentation/docs/source/rst_source/examples/async.examples.rst
 documentation/docs/source/rst_source/examples/async.examples.user.rst
```

### Comparing `ibm-generative-ai-0.2.1/src/ibm_generative_ai.egg-info/requires.txt` & `ibm-generative-ai-0.2.2/src/ibm_generative_ai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/tests/assets/file_to_tune.json` & `ibm-generative-ai-0.2.2/tests/assets/file_to_tune.json`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/tests/assets/file_to_tune.jsonl` & `ibm-generative-ai-0.2.2/tests/assets/file_to_tune.jsonl`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/tests/assets/response_helper.py` & `ibm-generative-ai-0.2.2/tests/assets/response_helper.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/tests/extensions/test_langchain.py` & `ibm-generative-ai-0.2.2/tests/extensions/test_langchain.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/tests/extensions/test_localserver.py` & `ibm-generative-ai-0.2.2/tests/extensions/test_localserver.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/tests/extensions/test_save_huggingface.py` & `ibm-generative-ai-0.2.2/tests/extensions/test_save_huggingface.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/tests/extensions/test_sub_from_pandas.py` & `ibm-generative-ai-0.2.2/tests/extensions/test_sub_from_pandas.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/tests/integration/conftest.py` & `ibm-generative-ai-0.2.2/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/tests/integration/test_examples.py` & `ibm-generative-ai-0.2.2/tests/integration/test_examples.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/tests/test_concurrent.py` & `ibm-generative-ai-0.2.2/tests/test_concurrent.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/tests/test_files.py` & `ibm-generative-ai-0.2.2/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/tests/test_generate_schema.py` & `ibm-generative-ai-0.2.2/tests/test_generate_schema.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/tests/test_generate_service.py` & `ibm-generative-ai-0.2.2/tests/test_generate_service.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/tests/test_history.py` & `ibm-generative-ai-0.2.2/tests/test_history.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/tests/test_json_utils.py` & `ibm-generative-ai-0.2.2/tests/test_json_utils.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/tests/test_logging.py` & `ibm-generative-ai-0.2.2/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/tests/test_metadata.py` & `ibm-generative-ai-0.2.2/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/tests/test_model.py` & `ibm-generative-ai-0.2.2/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/tests/test_model_async.py` & `ibm-generative-ai-0.2.2/tests/test_model_async.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/tests/test_prompt_pattern.py` & `ibm-generative-ai-0.2.2/tests/test_prompt_pattern.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/tests/test_prompt_pattern_watsonx.py` & `ibm-generative-ai-0.2.2/tests/test_prompt_pattern_watsonx.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/tests/test_prompt_template_manager.py` & `ibm-generative-ai-0.2.2/tests/test_prompt_template_manager.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/tests/test_request_handler.py` & `ibm-generative-ai-0.2.2/tests/test_request_handler.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/tests/test_schema_validation.py` & `ibm-generative-ai-0.2.2/tests/test_schema_validation.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/tests/test_service_interface.py` & `ibm-generative-ai-0.2.2/tests/test_service_interface.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/tests/test_service_interface_async.py` & `ibm-generative-ai-0.2.2/tests/test_service_interface_async.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/tests/test_service_utils.py` & `ibm-generative-ai-0.2.2/tests/test_service_utils.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/tests/test_token.py` & `ibm-generative-ai-0.2.2/tests/test_token.py`

 * *Files identical despite different names*

### Comparing `ibm-generative-ai-0.2.1/tests/test_tunes.py` & `ibm-generative-ai-0.2.2/tests/test_tunes.py`

 * *Files identical despite different names*

