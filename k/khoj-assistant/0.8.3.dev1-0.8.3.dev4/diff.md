# Comparing `tmp/khoj_assistant-0.8.3.dev1.tar.gz` & `tmp/khoj_assistant-0.8.3.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue Jul 11 04:16:19 2023, max compression
+gzip compressed data, last modified: Tue Jul 11 04:27:58 2023, max compression
```

## Comparing `khoj_assistant-0.8.3.dev1.tar` & `khoj_assistant-0.8.3.dev4.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0        0 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/__init__.py
--rw-r--r--   0        0        0    11624 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/configure.py
--rw-r--r--   0        0        0     5389 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/main.py
--rw-r--r--   0        0        0        0 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/interface/desktop/__init__.py
--rw-r--r--   0        0        0     2049 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/interface/desktop/main_window.py
--rw-r--r--   0        0        0     1395 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/interface/desktop/system_tray.py
--rw-r--r--   0        0        0      582 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/interface/web/404.html
--rw-r--r--   0        0        0     4897 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/interface/web/base_config.html
--rw-r--r--   0        0        0      657 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/interface/web/base_processor_integration.html
--rw-r--r--   0        0        0    18018 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/interface/web/chat.html
--rw-r--r--   0        0        0    16252 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/interface/web/config.html
--rw-r--r--   0        0        0     6930 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/interface/web/content_type_github_input.html
--rw-r--r--   0        0        0     7322 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/interface/web/content_type_input.html
--rw-r--r--   0        0        0     3401 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/interface/web/content_type_notion_input.html
--rw-r--r--   0        0        0    18924 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/interface/web/index.html
--rw-r--r--   0        0        0      402 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/interface/web/khoj.webmanifest
--rw-r--r--   0        0        0      418 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/interface/web/khoj_chat.webmanifest
--rw-r--r--   0        0        0     3660 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/interface/web/processor_conversation_input.html
--rw-r--r--   0        0        0     2433 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/interface/web/assets/khoj.css
--rw-r--r--   0        0        0   275822 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/interface/web/assets/markdown-it.min.js
--rw-r--r--   0        0        0    58643 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/interface/web/assets/org.min.js
--rw-r--r--   0        0        0    73572 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/interface/web/assets/pico.min.css
--rw-r--r--   0        0        0    51584 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/interface/web/assets/icons/chat.svg
--rw-r--r--   0        0        0      549 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/interface/web/assets/icons/confirm-icon.svg
--rw-r--r--   0        0        0   205167 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/interface/web/assets/icons/favicon-128x128.ico
--rw-r--r--   0        0        0    12518 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/interface/web/assets/icons/favicon-128x128.png
--rw-r--r--   0        0        0    31531 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/interface/web/assets/icons/favicon.icns
--rw-r--r--   0        0        0      964 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/interface/web/assets/icons/github.svg
--rw-r--r--   0        0        0    13011 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
--rw-r--r--   0        0        0  1301428 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
--rw-r--r--   0        0        0     4031 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/interface/web/assets/icons/logotype.svg
--rw-r--r--   0        0        0      283 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/interface/web/assets/icons/markdown.svg
--rw-r--r--   0        0        0     1578 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/interface/web/assets/icons/notion.svg
--rw-r--r--   0        0        0     7946 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/interface/web/assets/icons/org.svg
--rw-r--r--   0        0        0     2504 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/interface/web/assets/icons/pdf.svg
--rw-r--r--   0        0        0        0 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/processor/__init__.py
--rw-r--r--   0        0        0     4455 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/processor/text_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/processor/conversation/__init__.py
--rw-r--r--   0        0        0     4824 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/processor/conversation/gpt.py
--rw-r--r--   0        0        0     3991 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/processor/conversation/prompts.py
--rw-r--r--   0        0        0     8304 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/processor/conversation/utils.py
--rw-r--r--   0        0        0        0 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/processor/github/__init__.py
--rw-r--r--   0        0        0    13517 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/processor/github/github_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/processor/jsonl/__init__.py
--rw-r--r--   0        0        0     3937 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/processor/jsonl/jsonl_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/processor/markdown/__init__.py
--rw-r--r--   0        0        0     7454 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/processor/markdown/markdown_to_jsonl.py
--rw-r--r--   0        0        0     9295 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/processor/notion/notion_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/processor/org_mode/__init__.py
--rw-r--r--   0        0        0     7259 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/processor/org_mode/org_to_jsonl.py
--rw-r--r--   0        0        0    16881 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/processor/org_mode/orgnode.py
--rw-r--r--   0        0        0        0 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/processor/pdf/__init__.py
--rw-r--r--   0        0        0     5397 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/processor/pdf/pdf_to_jsonl.py
--rw-r--r--   0        0        0        0 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/routers/__init__.py
--rw-r--r--   0        0        0    20526 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/routers/api.py
--rw-r--r--   0        0        0      167 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/routers/api_beta.py
--rw-r--r--   0        0        0     2895 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/routers/helpers.py
--rw-r--r--   0        0        0     5524 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/routers/web_client.py
--rw-r--r--   0        0        0        0 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/search_filter/__init__.py
--rw-r--r--   0        0        0      539 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/search_filter/base_filter.py
--rw-r--r--   0        0        0     7566 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/search_filter/date_filter.py
--rw-r--r--   0        0        0     2844 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/search_filter/file_filter.py
--rw-r--r--   0        0        0     3770 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/search_filter/word_filter.py
--rw-r--r--   0        0        0        0 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/search_type/__init__.py
--rw-r--r--   0        0        0    11381 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/search_type/image_search.py
--rw-r--r--   0        0        0    11237 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/search_type/text_search.py
--rw-r--r--   0        0        0        0 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/utils/__init__.py
--rw-r--r--   0        0        0     2040 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/utils/cli.py
--rw-r--r--   0        0        0     2571 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/utils/config.py
--rw-r--r--   0        0        0     2710 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/utils/constants.py
--rw-r--r--   0        0        0     6889 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/utils/helpers.py
--rw-r--r--   0        0        0     1607 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/utils/jsonl.py
--rw-r--r--   0        0        0     2463 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/utils/models.py
--rw-r--r--   0        0        0     4338 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/utils/rawconfig.py
--rw-r--r--   0        0        0     1066 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/utils/state.py
--rw-r--r--   0        0        0     1486 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/src/khoj/utils/yaml.py
--rw-r--r--   0        0        0      523 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/.gitignore
--rw-r--r--   0        0        0    32472 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/LICENSE
--rw-r--r--   0        0        0    24888 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/README.md
--rw-r--r--   0        0        0     2792 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/pyproject.toml
--rw-r--r--   0        0        0    27252 2023-07-11 04:16:19.000000 khoj_assistant-0.8.3.dev1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/__init__.py
+-rw-r--r--   0        0        0    11626 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/configure.py
+-rw-r--r--   0        0        0     5389 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/main.py
+-rw-r--r--   0        0        0        0 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/desktop/__init__.py
+-rw-r--r--   0        0        0     2049 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/desktop/main_window.py
+-rw-r--r--   0        0        0     1395 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/desktop/system_tray.py
+-rw-r--r--   0        0        0      582 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/404.html
+-rw-r--r--   0        0        0     4897 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/base_config.html
+-rw-r--r--   0        0        0      657 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/base_processor_integration.html
+-rw-r--r--   0        0        0    18018 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/chat.html
+-rw-r--r--   0        0        0    16252 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/config.html
+-rw-r--r--   0        0        0     6930 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/content_type_github_input.html
+-rw-r--r--   0        0        0     7322 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/content_type_input.html
+-rw-r--r--   0        0        0     3401 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/content_type_notion_input.html
+-rw-r--r--   0        0        0    18924 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/index.html
+-rw-r--r--   0        0        0      402 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/khoj.webmanifest
+-rw-r--r--   0        0        0      418 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/khoj_chat.webmanifest
+-rw-r--r--   0        0        0     3660 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/processor_conversation_input.html
+-rw-r--r--   0        0        0     2433 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/khoj.css
+-rw-r--r--   0        0        0   275822 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/markdown-it.min.js
+-rw-r--r--   0        0        0    58643 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/org.min.js
+-rw-r--r--   0        0        0    73572 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/pico.min.css
+-rw-r--r--   0        0        0    51584 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/chat.svg
+-rw-r--r--   0        0        0      549 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/confirm-icon.svg
+-rw-r--r--   0        0        0   205167 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/favicon-128x128.ico
+-rw-r--r--   0        0        0    12518 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/favicon-128x128.png
+-rw-r--r--   0        0        0    31531 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/favicon.icns
+-rw-r--r--   0        0        0      964 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/github.svg
+-rw-r--r--   0        0        0    13011 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
+-rw-r--r--   0        0        0  1301428 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
+-rw-r--r--   0        0        0     4031 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/logotype.svg
+-rw-r--r--   0        0        0      283 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/markdown.svg
+-rw-r--r--   0        0        0     1578 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/notion.svg
+-rw-r--r--   0        0        0     7946 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/org.svg
+-rw-r--r--   0        0        0     2504 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/pdf.svg
+-rw-r--r--   0        0        0        0 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/processor/__init__.py
+-rw-r--r--   0        0        0     4455 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/processor/text_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/processor/conversation/__init__.py
+-rw-r--r--   0        0        0     4824 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/processor/conversation/gpt.py
+-rw-r--r--   0        0        0     3991 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/processor/conversation/prompts.py
+-rw-r--r--   0        0        0     8304 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/processor/conversation/utils.py
+-rw-r--r--   0        0        0        0 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/processor/github/__init__.py
+-rw-r--r--   0        0        0    13517 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/processor/github/github_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/processor/jsonl/__init__.py
+-rw-r--r--   0        0        0     3937 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/processor/jsonl/jsonl_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/processor/markdown/__init__.py
+-rw-r--r--   0        0        0     7454 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/processor/markdown/markdown_to_jsonl.py
+-rw-r--r--   0        0        0     9295 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/processor/notion/notion_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/processor/org_mode/__init__.py
+-rw-r--r--   0        0        0     7259 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/processor/org_mode/org_to_jsonl.py
+-rw-r--r--   0        0        0    16881 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/processor/org_mode/orgnode.py
+-rw-r--r--   0        0        0        0 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/processor/pdf/__init__.py
+-rw-r--r--   0        0        0     5397 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/processor/pdf/pdf_to_jsonl.py
+-rw-r--r--   0        0        0        0 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/routers/__init__.py
+-rw-r--r--   0        0        0    20526 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/routers/api.py
+-rw-r--r--   0        0        0      167 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/routers/api_beta.py
+-rw-r--r--   0        0        0     2895 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/routers/helpers.py
+-rw-r--r--   0        0        0     5524 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/routers/web_client.py
+-rw-r--r--   0        0        0        0 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/search_filter/__init__.py
+-rw-r--r--   0        0        0      539 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/search_filter/base_filter.py
+-rw-r--r--   0        0        0     7566 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/search_filter/date_filter.py
+-rw-r--r--   0        0        0     2844 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/search_filter/file_filter.py
+-rw-r--r--   0        0        0     3770 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/search_filter/word_filter.py
+-rw-r--r--   0        0        0        0 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/search_type/__init__.py
+-rw-r--r--   0        0        0    11381 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/search_type/image_search.py
+-rw-r--r--   0        0        0    11237 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/search_type/text_search.py
+-rw-r--r--   0        0        0        0 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/utils/__init__.py
+-rw-r--r--   0        0        0     2042 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/utils/cli.py
+-rw-r--r--   0        0        0     2571 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/utils/config.py
+-rw-r--r--   0        0        0     2710 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/utils/constants.py
+-rw-r--r--   0        0        0     6889 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/utils/helpers.py
+-rw-r--r--   0        0        0     1607 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/utils/jsonl.py
+-rw-r--r--   0        0        0     2463 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/utils/models.py
+-rw-r--r--   0        0        0     4338 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/utils/rawconfig.py
+-rw-r--r--   0        0        0     1066 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/utils/state.py
+-rw-r--r--   0        0        0     1486 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/src/khoj/utils/yaml.py
+-rw-r--r--   0        0        0      523 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/.gitignore
+-rw-r--r--   0        0        0    32472 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/LICENSE
+-rw-r--r--   0        0        0    24858 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/README.md
+-rw-r--r--   0        0        0     2792 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/pyproject.toml
+-rw-r--r--   0        0        0    27222 2023-07-11 04:27:58.000000 khoj_assistant-0.8.3.dev4/PKG-INFO
```

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/configure.py` & `khoj_assistant-0.8.3.dev4/src/khoj/configure.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,20 +31,20 @@
 logger = logging.getLogger(__name__)
 
 
 def configure_server(args, required=False):
     if args.config is None:
         if required:
             logger.error(
-                f"Exiting as Khoj is not configured.\nConfigure it via http://localhost:8000/config or by editing {state.config_file}."
+                f"Exiting as Khoj is not configured.\nConfigure it via http://localhost:42110/config or by editing {state.config_file}."
             )
             sys.exit(1)
         else:
             logger.warning(
-                f"Khoj is not configured.\nConfigure it via http://localhost:8000/config, plugins or by editing {state.config_file}."
+                f"Khoj is not configured.\nConfigure it via http://localhost:42110/config, plugins or by editing {state.config_file}."
             )
             return
     else:
         state.config = args.config
 
     # Initialize Processor from Config
     state.processor_config = configure_processor(args.config.processor)
```

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/main.py` & `khoj_assistant-0.8.3.dev4/src/khoj/main.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/interface/desktop/main_window.py` & `khoj_assistant-0.8.3.dev4/src/khoj/interface/desktop/main_window.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/interface/desktop/system_tray.py` & `khoj_assistant-0.8.3.dev4/src/khoj/interface/desktop/system_tray.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/interface/web/404.html` & `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/404.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/interface/web/base_config.html` & `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/base_config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/interface/web/base_processor_integration.html` & `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/base_processor_integration.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/interface/web/chat.html` & `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/chat.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/interface/web/config.html` & `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/interface/web/content_type_github_input.html` & `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/content_type_github_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/interface/web/content_type_input.html` & `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/content_type_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/interface/web/content_type_notion_input.html` & `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/content_type_notion_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/interface/web/index.html` & `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/index.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/interface/web/processor_conversation_input.html` & `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/processor_conversation_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/interface/web/assets/khoj.css` & `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/khoj.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/interface/web/assets/markdown-it.min.js` & `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/markdown-it.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/interface/web/assets/org.min.js` & `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/org.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/interface/web/assets/pico.min.css` & `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/pico.min.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/interface/web/assets/icons/chat.svg` & `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/chat.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/interface/web/assets/icons/confirm-icon.svg` & `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/confirm-icon.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/interface/web/assets/icons/favicon-128x128.ico` & `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/favicon-128x128.ico`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/interface/web/assets/icons/favicon-128x128.png` & `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/interface/web/assets/icons/favicon.icns` & `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/favicon.icns`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/interface/web/assets/icons/github.svg` & `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/github.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png` & `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg` & `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/interface/web/assets/icons/logotype.svg` & `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/logotype.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/interface/web/assets/icons/notion.svg` & `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/notion.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/interface/web/assets/icons/org.svg` & `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/org.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/interface/web/assets/icons/pdf.svg` & `khoj_assistant-0.8.3.dev4/src/khoj/interface/web/assets/icons/pdf.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/processor/text_to_jsonl.py` & `khoj_assistant-0.8.3.dev4/src/khoj/processor/text_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/processor/conversation/gpt.py` & `khoj_assistant-0.8.3.dev4/src/khoj/processor/conversation/gpt.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/processor/conversation/prompts.py` & `khoj_assistant-0.8.3.dev4/src/khoj/processor/conversation/prompts.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/processor/conversation/utils.py` & `khoj_assistant-0.8.3.dev4/src/khoj/processor/conversation/utils.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/processor/github/github_to_jsonl.py` & `khoj_assistant-0.8.3.dev4/src/khoj/processor/github/github_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/processor/jsonl/jsonl_to_jsonl.py` & `khoj_assistant-0.8.3.dev4/src/khoj/processor/jsonl/jsonl_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/processor/markdown/markdown_to_jsonl.py` & `khoj_assistant-0.8.3.dev4/src/khoj/processor/markdown/markdown_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/processor/notion/notion_to_jsonl.py` & `khoj_assistant-0.8.3.dev4/src/khoj/processor/notion/notion_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/processor/org_mode/org_to_jsonl.py` & `khoj_assistant-0.8.3.dev4/src/khoj/processor/org_mode/org_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/processor/org_mode/orgnode.py` & `khoj_assistant-0.8.3.dev4/src/khoj/processor/org_mode/orgnode.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/processor/pdf/pdf_to_jsonl.py` & `khoj_assistant-0.8.3.dev4/src/khoj/processor/pdf/pdf_to_jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/routers/api.py` & `khoj_assistant-0.8.3.dev4/src/khoj/routers/api.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/routers/helpers.py` & `khoj_assistant-0.8.3.dev4/src/khoj/routers/helpers.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/routers/web_client.py` & `khoj_assistant-0.8.3.dev4/src/khoj/routers/web_client.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/search_filter/base_filter.py` & `khoj_assistant-0.8.3.dev4/src/khoj/search_filter/base_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/search_filter/date_filter.py` & `khoj_assistant-0.8.3.dev4/src/khoj/search_filter/date_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/search_filter/file_filter.py` & `khoj_assistant-0.8.3.dev4/src/khoj/search_filter/file_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/search_filter/word_filter.py` & `khoj_assistant-0.8.3.dev4/src/khoj/search_filter/word_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/search_type/image_search.py` & `khoj_assistant-0.8.3.dev4/src/khoj/search_type/image_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/search_type/text_search.py` & `khoj_assistant-0.8.3.dev4/src/khoj/search_type/text_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/utils/cli.py` & `khoj_assistant-0.8.3.dev4/src/khoj/utils/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         "--regenerate",
         action="store_true",
         default=False,
         help="Regenerate model embeddings from source files. Default: false",
     )
     parser.add_argument("--verbose", "-v", action="count", default=0, help="Show verbose conversion logs. Default: 0")
     parser.add_argument("--host", type=str, default="127.0.0.1", help="Host address of the server. Default: 127.0.0.1")
-    parser.add_argument("--port", "-p", type=int, default=8000, help="Port of the server. Default: 8000")
+    parser.add_argument("--port", "-p", type=int, default=42110, help="Port of the server. Default: 42110")
     parser.add_argument(
         "--socket",
         type=pathlib.Path,
         help="Path to UNIX socket for server. Use to run server behind reverse proxy. Default: /tmp/uvicorn.sock",
     )
     parser.add_argument("--version", "-V", action="store_true", help="Print the installed Khoj version and exit")
     parser.add_argument("--demo", action="store_true", default=False, help="Run Khoj in demo mode")
```

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/utils/config.py` & `khoj_assistant-0.8.3.dev4/src/khoj/utils/config.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/utils/constants.py` & `khoj_assistant-0.8.3.dev4/src/khoj/utils/constants.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/utils/helpers.py` & `khoj_assistant-0.8.3.dev4/src/khoj/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/utils/jsonl.py` & `khoj_assistant-0.8.3.dev4/src/khoj/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/utils/models.py` & `khoj_assistant-0.8.3.dev4/src/khoj/utils/models.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/utils/rawconfig.py` & `khoj_assistant-0.8.3.dev4/src/khoj/utils/rawconfig.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/utils/state.py` & `khoj_assistant-0.8.3.dev4/src/khoj/utils/state.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/src/khoj/utils/yaml.py` & `khoj_assistant-0.8.3.dev4/src/khoj/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/.gitignore` & `khoj_assistant-0.8.3.dev4/.gitignore`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/LICENSE` & `khoj_assistant-0.8.3.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/README.md` & `khoj_assistant-0.8.3.dev4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -43,18 +43,18 @@
   - [GPT API](#gpt-api)
 - [Performance](#Performance)
   - [Query Performance](#Query-performance)
   - [Indexing Performance](#Indexing-performance)
   - [Miscellaneous](#Miscellaneous-1)
 - [Development](#Development)
   - [Visualize Codebase](#visualize-codebase)
+  - [Create Release](#create-khoj-release)
   - [Setup](#Setup)
     - [Using Pip](#Using-Pip)
     - [Using Docker](#Using-Docker)
-    - [Using Conda](#Using-Conda)
   - [Validate](#Validate)
 - [Credits](#Credits)
 
 ## Features
 - **Search**
   - **Local**: Your personal data stays local. All search and indexing is done on your machine. *Unlike chat which requires access to GPT.*
   - **Incremental**: Incremental search for a fast, search-as-you-type experience
@@ -165,17 +165,17 @@
 ## Use
 ### Khoj Search
 - **Khoj via Obsidian**
   - Click the *Khoj search* icon 🔎 on the [Ribbon](https://help.obsidian.md/User+interface/Workspace/Ribbon) or Search for *Khoj: Search* in the [Command Palette](https://help.obsidian.md/Plugins/Command+palette)
 - **Khoj via Emacs**
   - Run `M-x khoj <user-query>`
 - **Khoj via Web**
-  - Open <http://localhost:8000/> directly
+  - Open <http://localhost:42110/> directly
 - **Khoj via API**
-  - See the Khoj FastAPI [Swagger Docs](http://localhost:8000/docs), [ReDocs](http://localhost:8000/redocs)
+  - See the Khoj FastAPI [Swagger Docs](http://localhost:42110/docs), [ReDocs](http://localhost:42110/redocs)
 
 <details><summary>Query Filters</summary>
 
 Use structured query syntax to filter the natural language search results
 - **Word Filter**: Get entries that include/exclude a specified term
   - Entries that contain term_to_include: `+"term_to_include"`
   - Entries that contain term_to_exclude: `-"term_to_exclude"`
@@ -203,15 +203,15 @@
 - Shows reference notes used to generate a response
 - **Note**: *Your query and top notes from khoj search will be sent to OpenAI for processing*
 
 #### Setup
 - [Setup your OpenAI API key in Khoj](#set-your-openai-api-key-in-khoj)
 
 #### Use
-1. Open [/chat](http://localhost:8000/chat)[^2]
+1. Open [/chat](http://localhost:42110/chat)[^2]
 2. Type your queries and see response by Khoj from your notes
 
 #### Demo
 ![](https://github.com/khoj-ai/khoj/blob/master/docs/khoj_chat_web_interface.png?)
 
 ### Details
 1. Your query is used to retrieve the most relevant notes, if any, using Khoj search
@@ -252,29 +252,29 @@
     brew install rustup
     rustup-init
     source ~/.cargo/env
     ```
 - **Refer**: [Issue with Fix](https://github.com/khoj-ai/khoj/issues/82#issuecomment-1241890946) for more details
 
 #### Search starts giving wonky results
-- **Fix**: Open [/api/update?force=true](http://localhost:8000/api/update?force=true)[^2] in browser to regenerate index from scratch
+- **Fix**: Open [/api/update?force=true](http://localhost:42110/api/update?force=true)[^2] in browser to regenerate index from scratch
 - **Note**: *This is a fix for when you percieve the search results have degraded. Not if you think they've always given wonky results*
 
 #### Khoj in Docker errors out with \"Killed\" in error message
 - **Fix**: Increase RAM available to Docker Containers in Docker Settings
 - **Refer**: [StackOverflow Solution](https://stackoverflow.com/a/50770267), [Configure Resources on Docker for Mac](https://docs.docker.com/desktop/mac/#resources)
 
 #### Khoj errors out complaining about Tensors mismatch or null
 - **Mitigation**: Disable `image` search using the desktop GUI
 
 ## Advanced Usage
 ### Access Khoj on Mobile
 1. [Setup Khoj](#Setup) on your personal server. This can be any always-on machine, i.e an old computer, RaspberryPi(?) etc
 2. [Install](https://tailscale.com/kb/installation/) [Tailscale](tailscale.com/) on your personal server and phone
-3. Open the Khoj web interface of the server from your phone browser.<br /> It should be `http://tailscale-ip-of-server:8000` or `http://name-of-server:8000` if you've setup [MagicDNS](https://tailscale.com/kb/1081/magicdns/)
+3. Open the Khoj web interface of the server from your phone browser.<br /> It should be `http://tailscale-ip-of-server:42110` or `http://name-of-server:42110` if you've setup [MagicDNS](https://tailscale.com/kb/1081/magicdns/)
 4. Click the [Add to Homescreen](https://developer.mozilla.org/en-US/docs/Web/Progressive_web_apps/Add_to_home_screen) button
 5. Enjoy exploring your notes, documents and images from your phone!
 
 ![](https://github.com/khoj-ai/khoj/blob/master/docs/khoj_pwa_android.png?)
 
 ### Use OpenAI Models for Search
 #### Setup
@@ -307,15 +307,15 @@
    asymmetric:
 - encoder: "sentence-transformers/multi-qa-MiniLM-L6-cos-v1"
 + encoder: "paraphrase-multilingual-MiniLM-L12-v2"
      cross-encoder: "cross-encoder/ms-marco-MiniLM-L-6-v2"
      model_directory: "~/.khoj/search/asymmetric/"
   ```
 
-  2. Regenerate your content index. For example, by opening [\<khoj-url\>/api/update?t=force](http://localhost:8000/api/update?t=force)
+  2. Regenerate your content index. For example, by opening [\<khoj-url\>/api/update?t=force](http://localhost:42110/api/update?t=force)
 
 ### Bootstrap Khoj Search for Offline Usage later
 
   You can bootstrap Khoj pre-emptively to run on machines that do not have internet access. An example use-case would be to run Khoj on an air-gapped machine.
   Note: *Only search can currently run in fully offline mode, not chat.*
 
   - With Internet
@@ -326,33 +326,33 @@
     2. Copy the khoj virtual environment directory onto the air-gapped machine, activate the environment and start and khoj as normal. E.g `source .venv/bin/activate && khoj`
 
 
 ## Miscellaneous
 ### Set your OpenAI API key in Khoj
 If you want, Khoj can be configured to use OpenAI for search and chat.<br />
 Add your OpenAI API to Khoj by using either of the two options below:
- - Open your [Khoj settings](http://localhost:8000/config/processor/conversation), add your OpenAI API key, and click *Save*. Then go to your [Khoj settings](http://localhost:8000/config) and click `Configure`. This will refresh Khoj with your OpenAI API key.
+ - Open your [Khoj settings](http://localhost:42110/config/processor/conversation), add your OpenAI API key, and click *Save*. Then go to your [Khoj settings](http://localhost:42110/config) and click `Configure`. This will refresh Khoj with your OpenAI API key.
  - Set `openai-api-key` field under `processor.conversation` section in your `khoj.yml`[^1] to your [OpenAI API key](https://beta.openai.com/account/api-keys) and restart khoj:
     ```diff
     processor:
       conversation:
     -    openai-api-key: # "YOUR_OPENAI_API_KEY"
     +    openai-api-key: sk-aaaaaaaaaaaaaaaaaaaaaaaahhhhhhhhhhhhhhhhhhhhhhhh
         model: "text-davinci-003"
         conversation-logfile: "~/.khoj/processor/conversation/conversation_logs.json"
     ```
 
 **Warning**: *This will enable Khoj to send your query and note(s) to OpenAI for processing*
 
 ### GPT API
-- The [chat](http://localhost:8000/api/chat), [answer](http://localhost:8000/api/beta/answer) and [search](http://localhost:8000/api/beta/search) API endpoints use [OpenAI API](https://openai.com/api/)
+- The [chat](http://localhost:42110/api/chat), [answer](http://localhost:42110/api/beta/answer) and [search](http://localhost:42110/api/beta/search) API endpoints use [OpenAI API](https://openai.com/api/)
 - They are disabled by default
 - To use them:
   1. [Setup your OpenAI API key in Khoj](#set-your-openai-api-key-in-khoj)
-  2. Interact with them from the [Khoj Swagger docs](http://locahost:8000/docs)[^2]
+  2. Interact with them from the [Khoj Swagger docs](http://locahost:42110/docs)[^2]
 
 ### Index Github Repository for Search, Chat
 The Khoj Github plugin can index issues, commit messages and markdown, org-mode and PDF files from any repositories you have access to. This allows you to chat or search with these repositories. Get answers, resolve issues or just explore a repo with the help of your AI personal assistant.
 
 See the [Khoj FAQ](https://faq.khoj.dev) for a demo of Khoj search and chat. It makes the Khoj github repo available for exploring.
 
 Note: *Khoj will ignore code files in the repository for now as the default AI model used works best with natural language text, not code.*
@@ -384,14 +384,27 @@
 ## Development
 ### Visualize Codebase
 
 *[Interactive Visualization](https://mango-dune-07a8b7110.1.azurestaticapps.net/?repo=debanjum%2Fkhoj)*
 
 ![](https://github.com/khoj-ai/khoj/blob/master/docs/khoj_codebase_visualization_0.2.1.png?)
 
+### Create Khoj Release
+Follow the steps below to [release](https://github.com/debanjum/khoj/releases/) Khoj. This will create a stable release of Khoj on [Pypi](https://pypi.org/project/khoj-assistant/), [Melpa](https://stable.melpa.org/#%252Fkhoj) and [Obsidian](https://obsidian.md/plugins?id%253Dkhoj). It will also create desktop apps of Khoj and attach them to the latest release.
+
+1. Create and tag release commit by running the bump_version script. The release commit sets version number in required metadata files.
+  ```shell
+  ./scripts/bump_version.sh -c "<release_version>"
+  ```
+2. Push commit and then the tag to trigger the release workflow to create Release with auto generated release notes.
+  ```shell
+  git push origin master  # push release commit to khoj repository
+  git push origin <release_version>  # push release tag to khoj repository
+  ```
+3. [Optional] Update the Release Notes to highlight new features, fixes and updates
 ### Setup
 #### Using Pip
 ##### 1. Install
 
 ```shell
 # Get Khoj Code
 git clone https://github.com/khoj-ai/khoj && cd khoj
@@ -405,15 +418,15 @@
 
 ##### 2. Run
 1. Start Khoj
    ```shell
    khoj -vv
    ```
 2. Configure Khoj
-   - **Via the Settings UI**: Add files, directories to index the [Khoj settings](http://localhost:8000/config) UI once Khoj has started up. Once you've saved all your settings, click `Configure`.
+   - **Via the Settings UI**: Add files, directories to index the [Khoj settings](http://localhost:42110/config) UI once Khoj has started up. Once you've saved all your settings, click `Configure`.
    - **Manually**:
      - Copy the `config/khoj_sample.yml` to `~/.khoj/khoj.yml`
      - Set `input-files` or `input-filter` in each relevant `content-type` section of `~/.khoj/khoj.yml`
        - Set `input-directories` field in `image` `content-type` section
      - Delete `content-type` and `processor` sub-section(s) irrelevant for your use-case
      - Restart khoj
 
@@ -441,47 +454,14 @@
 
 ##### 4. Upgrade
 
 ```shell
 docker-compose build --pull
 ```
 
-#### Using Conda
-##### 1. Install Dependencies
-- [Install Conda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html)
-
-##### 2. Install Khoj
-```shell
-git clone https://github.com/khoj-ai/khoj && cd khoj
-conda env create -f config/environment.yml
-conda activate khoj
-python3 -m pip install pyqt6  # As conda does not support pyqt6 yet
-```
-
-##### 3. Configure
-- Copy the `config/khoj_sample.yml` to `~/.khoj/khoj.yml`
-- Set `input-files` or `input-filter` in each relevant `content-type` section of `~/.khoj/khoj.yml`
-  - Set `input-directories` field in `image` `content-type` section
-- Delete `content-type`, `processor` sub-sections irrelevant for your use-case
-
-##### 4. Run
-```shell
-python3 -m src.khoj.main -vv
-```
-  Load ML model, generate embeddings and expose API to query notes, images, documents etc specified in config YAML
-
-##### 5. Upgrade
-```shell
-cd khoj
-git pull origin master
-conda deactivate khoj
-conda env update -f config/environment.yml
-conda activate khoj
-```
-
 ### Validate
 #### Before Make Changes
 1. Install Git Hooks for Validation
    ```shell
    pre-commit install -t pre-push -t pre-commit
    ```
    - This ensures standard code formatting fixes and other checks run automatically on every commit and push
@@ -518,8 +498,8 @@
 - Charles Cave for [OrgNode Parser](http://members.optusnet.com.au/~charles57/GTD/orgnode.html)
 - [Org.js](https://mooz.github.io/org-js/) to render Org-mode results on the Web interface
 - [Markdown-it](https://github.com/markdown-it/markdown-it) to render Markdown results on the Web interface
 
 
 [^1]: Default Khoj config file @ `~/.khoj/khoj.yml`
 
-[^2]: Default Khoj url @ http://localhost:8000
+[^2]: Default Khoj url @ http://localhost:42110
```

### Comparing `khoj_assistant-0.8.3.dev1/pyproject.toml` & `khoj_assistant-0.8.3.dev4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `khoj_assistant-0.8.3.dev1/PKG-INFO` & `khoj_assistant-0.8.3.dev4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khoj-assistant
-Version: 0.8.3.dev1
+Version: 0.8.3.dev4
 Summary: An AI personal assistant for your Digital Brain
 Project-URL: Homepage, https://github.com/khoj-ai/khoj#readme
 Project-URL: Issues, https://github.com/khoj-ai/khoj/issues
 Project-URL: Discussions, https://github.com/khoj-ai/khoj/discussions
 Project-URL: Releases, https://github.com/khoj-ai/khoj/releases
 Author: Debanjum Singh Solanky, Saba Imran
 License-Expression: GPL-3.0-or-later
@@ -101,18 +101,18 @@
   - [GPT API](#gpt-api)
 - [Performance](#Performance)
   - [Query Performance](#Query-performance)
   - [Indexing Performance](#Indexing-performance)
   - [Miscellaneous](#Miscellaneous-1)
 - [Development](#Development)
   - [Visualize Codebase](#visualize-codebase)
+  - [Create Release](#create-khoj-release)
   - [Setup](#Setup)
     - [Using Pip](#Using-Pip)
     - [Using Docker](#Using-Docker)
-    - [Using Conda](#Using-Conda)
   - [Validate](#Validate)
 - [Credits](#Credits)
 
 ## Features
 - **Search**
   - **Local**: Your personal data stays local. All search and indexing is done on your machine. *Unlike chat which requires access to GPT.*
   - **Incremental**: Incremental search for a fast, search-as-you-type experience
@@ -223,17 +223,17 @@
 ## Use
 ### Khoj Search
 - **Khoj via Obsidian**
   - Click the *Khoj search* icon 🔎 on the [Ribbon](https://help.obsidian.md/User+interface/Workspace/Ribbon) or Search for *Khoj: Search* in the [Command Palette](https://help.obsidian.md/Plugins/Command+palette)
 - **Khoj via Emacs**
   - Run `M-x khoj <user-query>`
 - **Khoj via Web**
-  - Open <http://localhost:8000/> directly
+  - Open <http://localhost:42110/> directly
 - **Khoj via API**
-  - See the Khoj FastAPI [Swagger Docs](http://localhost:8000/docs), [ReDocs](http://localhost:8000/redocs)
+  - See the Khoj FastAPI [Swagger Docs](http://localhost:42110/docs), [ReDocs](http://localhost:42110/redocs)
 
 <details><summary>Query Filters</summary>
 
 Use structured query syntax to filter the natural language search results
 - **Word Filter**: Get entries that include/exclude a specified term
   - Entries that contain term_to_include: `+"term_to_include"`
   - Entries that contain term_to_exclude: `-"term_to_exclude"`
@@ -261,15 +261,15 @@
 - Shows reference notes used to generate a response
 - **Note**: *Your query and top notes from khoj search will be sent to OpenAI for processing*
 
 #### Setup
 - [Setup your OpenAI API key in Khoj](#set-your-openai-api-key-in-khoj)
 
 #### Use
-1. Open [/chat](http://localhost:8000/chat)[^2]
+1. Open [/chat](http://localhost:42110/chat)[^2]
 2. Type your queries and see response by Khoj from your notes
 
 #### Demo
 ![](https://github.com/khoj-ai/khoj/blob/master/docs/khoj_chat_web_interface.png?)
 
 ### Details
 1. Your query is used to retrieve the most relevant notes, if any, using Khoj search
@@ -310,29 +310,29 @@
     brew install rustup
     rustup-init
     source ~/.cargo/env
     ```
 - **Refer**: [Issue with Fix](https://github.com/khoj-ai/khoj/issues/82#issuecomment-1241890946) for more details
 
 #### Search starts giving wonky results
-- **Fix**: Open [/api/update?force=true](http://localhost:8000/api/update?force=true)[^2] in browser to regenerate index from scratch
+- **Fix**: Open [/api/update?force=true](http://localhost:42110/api/update?force=true)[^2] in browser to regenerate index from scratch
 - **Note**: *This is a fix for when you percieve the search results have degraded. Not if you think they've always given wonky results*
 
 #### Khoj in Docker errors out with \"Killed\" in error message
 - **Fix**: Increase RAM available to Docker Containers in Docker Settings
 - **Refer**: [StackOverflow Solution](https://stackoverflow.com/a/50770267), [Configure Resources on Docker for Mac](https://docs.docker.com/desktop/mac/#resources)
 
 #### Khoj errors out complaining about Tensors mismatch or null
 - **Mitigation**: Disable `image` search using the desktop GUI
 
 ## Advanced Usage
 ### Access Khoj on Mobile
 1. [Setup Khoj](#Setup) on your personal server. This can be any always-on machine, i.e an old computer, RaspberryPi(?) etc
 2. [Install](https://tailscale.com/kb/installation/) [Tailscale](tailscale.com/) on your personal server and phone
-3. Open the Khoj web interface of the server from your phone browser.<br /> It should be `http://tailscale-ip-of-server:8000` or `http://name-of-server:8000` if you've setup [MagicDNS](https://tailscale.com/kb/1081/magicdns/)
+3. Open the Khoj web interface of the server from your phone browser.<br /> It should be `http://tailscale-ip-of-server:42110` or `http://name-of-server:42110` if you've setup [MagicDNS](https://tailscale.com/kb/1081/magicdns/)
 4. Click the [Add to Homescreen](https://developer.mozilla.org/en-US/docs/Web/Progressive_web_apps/Add_to_home_screen) button
 5. Enjoy exploring your notes, documents and images from your phone!
 
 ![](https://github.com/khoj-ai/khoj/blob/master/docs/khoj_pwa_android.png?)
 
 ### Use OpenAI Models for Search
 #### Setup
@@ -365,15 +365,15 @@
    asymmetric:
 - encoder: "sentence-transformers/multi-qa-MiniLM-L6-cos-v1"
 + encoder: "paraphrase-multilingual-MiniLM-L12-v2"
      cross-encoder: "cross-encoder/ms-marco-MiniLM-L-6-v2"
      model_directory: "~/.khoj/search/asymmetric/"
   ```
 
-  2. Regenerate your content index. For example, by opening [\<khoj-url\>/api/update?t=force](http://localhost:8000/api/update?t=force)
+  2. Regenerate your content index. For example, by opening [\<khoj-url\>/api/update?t=force](http://localhost:42110/api/update?t=force)
 
 ### Bootstrap Khoj Search for Offline Usage later
 
   You can bootstrap Khoj pre-emptively to run on machines that do not have internet access. An example use-case would be to run Khoj on an air-gapped machine.
   Note: *Only search can currently run in fully offline mode, not chat.*
 
   - With Internet
@@ -384,33 +384,33 @@
     2. Copy the khoj virtual environment directory onto the air-gapped machine, activate the environment and start and khoj as normal. E.g `source .venv/bin/activate && khoj`
 
 
 ## Miscellaneous
 ### Set your OpenAI API key in Khoj
 If you want, Khoj can be configured to use OpenAI for search and chat.<br />
 Add your OpenAI API to Khoj by using either of the two options below:
- - Open your [Khoj settings](http://localhost:8000/config/processor/conversation), add your OpenAI API key, and click *Save*. Then go to your [Khoj settings](http://localhost:8000/config) and click `Configure`. This will refresh Khoj with your OpenAI API key.
+ - Open your [Khoj settings](http://localhost:42110/config/processor/conversation), add your OpenAI API key, and click *Save*. Then go to your [Khoj settings](http://localhost:42110/config) and click `Configure`. This will refresh Khoj with your OpenAI API key.
  - Set `openai-api-key` field under `processor.conversation` section in your `khoj.yml`[^1] to your [OpenAI API key](https://beta.openai.com/account/api-keys) and restart khoj:
     ```diff
     processor:
       conversation:
     -    openai-api-key: # "YOUR_OPENAI_API_KEY"
     +    openai-api-key: sk-aaaaaaaaaaaaaaaaaaaaaaaahhhhhhhhhhhhhhhhhhhhhhhh
         model: "text-davinci-003"
         conversation-logfile: "~/.khoj/processor/conversation/conversation_logs.json"
     ```
 
 **Warning**: *This will enable Khoj to send your query and note(s) to OpenAI for processing*
 
 ### GPT API
-- The [chat](http://localhost:8000/api/chat), [answer](http://localhost:8000/api/beta/answer) and [search](http://localhost:8000/api/beta/search) API endpoints use [OpenAI API](https://openai.com/api/)
+- The [chat](http://localhost:42110/api/chat), [answer](http://localhost:42110/api/beta/answer) and [search](http://localhost:42110/api/beta/search) API endpoints use [OpenAI API](https://openai.com/api/)
 - They are disabled by default
 - To use them:
   1. [Setup your OpenAI API key in Khoj](#set-your-openai-api-key-in-khoj)
-  2. Interact with them from the [Khoj Swagger docs](http://locahost:8000/docs)[^2]
+  2. Interact with them from the [Khoj Swagger docs](http://locahost:42110/docs)[^2]
 
 ### Index Github Repository for Search, Chat
 The Khoj Github plugin can index issues, commit messages and markdown, org-mode and PDF files from any repositories you have access to. This allows you to chat or search with these repositories. Get answers, resolve issues or just explore a repo with the help of your AI personal assistant.
 
 See the [Khoj FAQ](https://faq.khoj.dev) for a demo of Khoj search and chat. It makes the Khoj github repo available for exploring.
 
 Note: *Khoj will ignore code files in the repository for now as the default AI model used works best with natural language text, not code.*
@@ -442,14 +442,27 @@
 ## Development
 ### Visualize Codebase
 
 *[Interactive Visualization](https://mango-dune-07a8b7110.1.azurestaticapps.net/?repo=debanjum%2Fkhoj)*
 
 ![](https://github.com/khoj-ai/khoj/blob/master/docs/khoj_codebase_visualization_0.2.1.png?)
 
+### Create Khoj Release
+Follow the steps below to [release](https://github.com/debanjum/khoj/releases/) Khoj. This will create a stable release of Khoj on [Pypi](https://pypi.org/project/khoj-assistant/), [Melpa](https://stable.melpa.org/#%252Fkhoj) and [Obsidian](https://obsidian.md/plugins?id%253Dkhoj). It will also create desktop apps of Khoj and attach them to the latest release.
+
+1. Create and tag release commit by running the bump_version script. The release commit sets version number in required metadata files.
+  ```shell
+  ./scripts/bump_version.sh -c "<release_version>"
+  ```
+2. Push commit and then the tag to trigger the release workflow to create Release with auto generated release notes.
+  ```shell
+  git push origin master  # push release commit to khoj repository
+  git push origin <release_version>  # push release tag to khoj repository
+  ```
+3. [Optional] Update the Release Notes to highlight new features, fixes and updates
 ### Setup
 #### Using Pip
 ##### 1. Install
 
 ```shell
 # Get Khoj Code
 git clone https://github.com/khoj-ai/khoj && cd khoj
@@ -463,15 +476,15 @@
 
 ##### 2. Run
 1. Start Khoj
    ```shell
    khoj -vv
    ```
 2. Configure Khoj
-   - **Via the Settings UI**: Add files, directories to index the [Khoj settings](http://localhost:8000/config) UI once Khoj has started up. Once you've saved all your settings, click `Configure`.
+   - **Via the Settings UI**: Add files, directories to index the [Khoj settings](http://localhost:42110/config) UI once Khoj has started up. Once you've saved all your settings, click `Configure`.
    - **Manually**:
      - Copy the `config/khoj_sample.yml` to `~/.khoj/khoj.yml`
      - Set `input-files` or `input-filter` in each relevant `content-type` section of `~/.khoj/khoj.yml`
        - Set `input-directories` field in `image` `content-type` section
      - Delete `content-type` and `processor` sub-section(s) irrelevant for your use-case
      - Restart khoj
 
@@ -499,47 +512,14 @@
 
 ##### 4. Upgrade
 
 ```shell
 docker-compose build --pull
 ```
 
-#### Using Conda
-##### 1. Install Dependencies
-- [Install Conda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html)
-
-##### 2. Install Khoj
-```shell
-git clone https://github.com/khoj-ai/khoj && cd khoj
-conda env create -f config/environment.yml
-conda activate khoj
-python3 -m pip install pyqt6  # As conda does not support pyqt6 yet
-```
-
-##### 3. Configure
-- Copy the `config/khoj_sample.yml` to `~/.khoj/khoj.yml`
-- Set `input-files` or `input-filter` in each relevant `content-type` section of `~/.khoj/khoj.yml`
-  - Set `input-directories` field in `image` `content-type` section
-- Delete `content-type`, `processor` sub-sections irrelevant for your use-case
-
-##### 4. Run
-```shell
-python3 -m src.khoj.main -vv
-```
-  Load ML model, generate embeddings and expose API to query notes, images, documents etc specified in config YAML
-
-##### 5. Upgrade
-```shell
-cd khoj
-git pull origin master
-conda deactivate khoj
-conda env update -f config/environment.yml
-conda activate khoj
-```
-
 ### Validate
 #### Before Make Changes
 1. Install Git Hooks for Validation
    ```shell
    pre-commit install -t pre-push -t pre-commit
    ```
    - This ensures standard code formatting fixes and other checks run automatically on every commit and push
@@ -576,8 +556,8 @@
 - Charles Cave for [OrgNode Parser](http://members.optusnet.com.au/~charles57/GTD/orgnode.html)
 - [Org.js](https://mooz.github.io/org-js/) to render Org-mode results on the Web interface
 - [Markdown-it](https://github.com/markdown-it/markdown-it) to render Markdown results on the Web interface
 
 
 [^1]: Default Khoj config file @ `~/.khoj/khoj.yml`
 
-[^2]: Default Khoj url @ http://localhost:8000
+[^2]: Default Khoj url @ http://localhost:42110
```

