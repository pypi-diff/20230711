# Comparing `tmp/db-gpt-0.2.7.tar.gz` & `tmp/db-gpt-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "db-gpt-0.2.7.tar", last modified: Tue Jul 11 02:52:08 2023, max compression
+gzip compressed data, was "db-gpt-0.2.8.tar", last modified: Tue Jul 11 07:35:39 2023, max compression
```

## Comparing `db-gpt-0.2.7.tar` & `db-gpt-0.2.8.tar`

### file list

```diff
@@ -1,248 +1,248 @@
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:08.176336 db-gpt-0.2.7/
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:07.984824 db-gpt-0.2.7/DB_GPT.egg-info/
--rw-r--r--   0 chenketing   (502) staff       (20)     8144 2023-07-11 02:52:07.000000 db-gpt-0.2.7/DB_GPT.egg-info/PKG-INFO
--rw-r--r--   0 chenketing   (502) staff       (20)     6845 2023-07-11 02:52:07.000000 db-gpt-0.2.7/DB_GPT.egg-info/SOURCES.txt
--rw-r--r--   0 chenketing   (502) staff       (20)        1 2023-07-11 02:52:07.000000 db-gpt-0.2.7/DB_GPT.egg-info/dependency_links.txt
--rw-r--r--   0 chenketing   (502) staff       (20)       56 2023-07-11 02:52:07.000000 db-gpt-0.2.7/DB_GPT.egg-info/entry_points.txt
--rw-r--r--   0 chenketing   (502) staff       (20)     1155 2023-07-11 02:52:07.000000 db-gpt-0.2.7/DB_GPT.egg-info/requires.txt
--rw-r--r--   0 chenketing   (502) staff       (20)       12 2023-07-11 02:52:07.000000 db-gpt-0.2.7/DB_GPT.egg-info/top_level.txt
--rw-r--r--   0 chenketing   (502) staff       (20)     1067 2023-06-20 09:57:25.000000 db-gpt-0.2.7/LICENSE
--rw-r--r--   0 chenketing   (502) staff       (20)     8144 2023-07-11 02:52:08.175968 db-gpt-0.2.7/PKG-INFO
--rw-r--r--   0 chenketing   (502) staff       (20)     7613 2023-07-10 06:54:41.000000 db-gpt-0.2.7/README.md
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:07.988499 db-gpt-0.2.7/pilot/
--rw-r--r--   0 chenketing   (502) staff       (20)      206 2023-07-10 08:01:44.000000 db-gpt-0.2.7/pilot/__init__.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:07.991144 db-gpt-0.2.7/pilot/agent/
--rw-r--r--   0 chenketing   (502) staff       (20)       46 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/agent/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)      179 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/agent/agent.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2266 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/agent/agent_manager.py
--rw-r--r--   0 chenketing   (502) staff       (20)     4025 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/agent/json_fix_llm.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:07.992464 db-gpt-0.2.7/pilot/chain/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/chain/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)       46 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/chain/audio.py
--rw-r--r--   0 chenketing   (502) staff       (20)       47 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/chain/visual.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:07.994552 db-gpt-0.2.7/pilot/commands/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/commands/__init__.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:07.995661 db-gpt-0.2.7/pilot/commands/built_in/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/commands/built_in/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1430 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/commands/built_in/audio_text.py
--rw-r--r--   0 chenketing   (502) staff       (20)     3509 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/commands/built_in/image_gen.py
--rw-r--r--   0 chenketing   (502) staff       (20)     4602 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/commands/command.py
--rw-r--r--   0 chenketing   (502) staff       (20)     5168 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/commands/command_mange.py
--rw-r--r--   0 chenketing   (502) staff       (20)      128 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/commands/exception_not_commands.py
--rw-r--r--   0 chenketing   (502) staff       (20)      244 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/commands/times.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:07.999289 db-gpt-0.2.7/pilot/common/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/common/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)      803 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/common/custom_data_structure.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1516 2023-07-05 08:29:49.000000 db-gpt-0.2.7/pilot/common/formatting.py
--rw-r--r--   0 chenketing   (502) staff       (20)     3044 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/common/markdown_text.py
--rw-r--r--   0 chenketing   (502) staff       (20)     6545 2023-06-27 11:35:59.000000 db-gpt-0.2.7/pilot/common/plugins.py
--rw-r--r--   0 chenketing   (502) staff       (20)      239 2023-07-05 08:29:49.000000 db-gpt-0.2.7/pilot/common/schema.py
--rw-r--r--   0 chenketing   (502) staff       (20)    17355 2023-07-10 06:54:41.000000 db-gpt-0.2.7/pilot/common/sql_database.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:08.001081 db-gpt-0.2.7/pilot/configs/
--rw-r--r--   0 chenketing   (502) staff       (20)      452 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/configs/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     7429 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/configs/config.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2219 2023-07-05 08:29:49.000000 db-gpt-0.2.7/pilot/configs/model_config.py
--rw-r--r--   0 chenketing   (502) staff       (20)    13673 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/conversation.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:08.010612 db-gpt-0.2.7/pilot/embedding_engine/
--rw-r--r--   0 chenketing   (502) staff       (20)      877 2023-07-05 08:29:49.000000 db-gpt-0.2.7/pilot/embedding_engine/EncodeTextLoader.py
--rw-r--r--   0 chenketing   (502) staff       (20)      289 2023-07-10 08:01:44.000000 db-gpt-0.2.7/pilot/embedding_engine/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2486 2023-07-05 08:29:49.000000 db-gpt-0.2.7/pilot/embedding_engine/chn_document_splitter.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1023 2023-07-05 08:29:49.000000 db-gpt-0.2.7/pilot/embedding_engine/csv_embedding.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2515 2023-07-10 12:58:18.000000 db-gpt-0.2.7/pilot/embedding_engine/embedding_engine.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:08.011170 db-gpt-0.2.7/pilot/embedding_engine/external/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-05 08:29:49.000000 db-gpt-0.2.7/pilot/embedding_engine/external/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     3649 2023-07-11 02:16:19.000000 db-gpt-0.2.7/pilot/embedding_engine/knowledge_type.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2200 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/embedding_engine/markdown_embedding.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2052 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/embedding_engine/pdf_embedding.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2102 2023-07-05 08:29:49.000000 db-gpt-0.2.7/pilot/embedding_engine/pdf_loader.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1965 2023-07-10 07:29:21.000000 db-gpt-0.2.7/pilot/embedding_engine/ppt_embedding.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1729 2023-07-05 08:29:49.000000 db-gpt-0.2.7/pilot/embedding_engine/search_milvus.py
--rw-r--r--   0 chenketing   (502) staff       (20)     3077 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/embedding_engine/source_embedding.py
--rw-r--r--   0 chenketing   (502) staff       (20)      883 2023-07-10 07:28:43.000000 db-gpt-0.2.7/pilot/embedding_engine/string_embedding.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1922 2023-07-10 07:28:43.000000 db-gpt-0.2.7/pilot/embedding_engine/url_embedding.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1793 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/embedding_engine/word_embedding.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:08.011692 db-gpt-0.2.7/pilot/inference_parsers/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/inference_parsers/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2234 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/inference_parsers/base.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:08.013285 db-gpt-0.2.7/pilot/json_utils/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/json_utils/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     3609 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/json_utils/json_fix_general.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2270 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/json_utils/utilities.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:08.014146 db-gpt-0.2.7/pilot/log/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/log/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)      531 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/log/json_handler.py
--rw-r--r--   0 chenketing   (502) staff       (20)     9846 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/logs.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:08.015125 db-gpt-0.2.7/pilot/memory/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/memory/__init__.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:08.018665 db-gpt-0.2.7/pilot/memory/chat_history/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/memory/chat_history/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1079 2023-07-05 08:29:49.000000 db-gpt-0.2.7/pilot/memory/chat_history/base.py
--rw-r--r--   0 chenketing   (502) staff       (20)     5319 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/memory/chat_history/duckdb_history.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1496 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/memory/chat_history/file_history.py
--rw-r--r--   0 chenketing   (502) staff       (20)      968 2023-07-05 08:29:49.000000 db-gpt-0.2.7/pilot/memory/chat_history/mem_history.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:08.070362 db-gpt-0.2.7/pilot/model/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/model/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     6541 2023-07-05 08:29:49.000000 db-gpt-0.2.7/pilot/model/adapter.py
--rw-r--r--   0 chenketing   (502) staff       (20)      206 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/model/base.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:08.073386 db-gpt-0.2.7/pilot/model/cache/
--rw-r--r--   0 chenketing   (502) staff       (20)      130 2023-07-05 08:29:49.000000 db-gpt-0.2.7/pilot/model/cache/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)      617 2023-07-05 08:29:49.000000 db-gpt-0.2.7/pilot/model/cache/base.py
--rw-r--r--   0 chenketing   (502) staff       (20)      718 2023-07-05 08:29:49.000000 db-gpt-0.2.7/pilot/model/cache/disk_cache.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1060 2023-07-05 08:29:49.000000 db-gpt-0.2.7/pilot/model/cache/gpt_cache.py
--rw-r--r--   0 chenketing   (502) staff       (20)      599 2023-07-05 08:29:49.000000 db-gpt-0.2.7/pilot/model/cache/memory_cache.py
--rw-r--r--   0 chenketing   (502) staff       (20)     3955 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/model/compression.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:08.079215 db-gpt-0.2.7/pilot/model/llm_out/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/model/llm_out/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2251 2023-07-05 08:29:49.000000 db-gpt-0.2.7/pilot/model/llm_out/chatglm_llm.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1546 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/model/llm_out/falcon_llm.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2001 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/model/llm_out/gorilla_llm.py
--rw-r--r--   0 chenketing   (502) staff       (20)      568 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/model/llm_out/gpt4all_llm.py
--rw-r--r--   0 chenketing   (502) staff       (20)     3276 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/model/llm_out/guanaco_llm.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2679 2023-07-10 06:54:41.000000 db-gpt-0.2.7/pilot/model/llm_out/proxy_llm.py
--rw-r--r--   0 chenketing   (502) staff       (20)     7674 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/model/llm_out/vicuna_base_llm.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2606 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/model/llm_out/vicuna_llm.py
--rw-r--r--   0 chenketing   (502) staff       (20)     3113 2023-07-05 08:29:49.000000 db-gpt-0.2.7/pilot/model/llm_utils.py
--rw-r--r--   0 chenketing   (502) staff       (20)     3949 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/model/loader.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:08.079837 db-gpt-0.2.7/pilot/model/proxy/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-05 08:29:49.000000 db-gpt-0.2.7/pilot/model/proxy/__init__.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:08.080170 db-gpt-0.2.7/pilot/openapi/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-05 08:29:49.000000 db-gpt-0.2.7/pilot/openapi/__init__.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:08.081788 db-gpt-0.2.7/pilot/openapi/api_v1/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-26 11:33:41.000000 db-gpt-0.2.7/pilot/openapi/api_v1/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     9550 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/openapi/api_v1/api_v1.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1559 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/openapi/api_v1/api_view_model.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:08.082833 db-gpt-0.2.7/pilot/out_parser/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/out_parser/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     8144 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/out_parser/base.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:08.085763 db-gpt-0.2.7/pilot/prompts/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/prompts/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1453 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/prompts/base.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1063 2023-07-05 08:29:49.000000 db-gpt-0.2.7/pilot/prompts/example_base.py
--rw-r--r--   0 chenketing   (502) staff       (20)     5623 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/prompts/generator.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2596 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/prompts/prompt_new.py
--rw-r--r--   0 chenketing   (502) staff       (20)    11978 2023-07-05 08:29:49.000000 db-gpt-0.2.7/pilot/prompts/prompt_template.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:08.089041 db-gpt-0.2.7/pilot/scene/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/scene/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2437 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/scene/base.py
--rw-r--r--   0 chenketing   (502) staff       (20)    12576 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/scene/base_chat.py
--rw-r--r--   0 chenketing   (502) staff       (20)     3683 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/scene/base_message.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:08.091432 db-gpt-0.2.7/pilot/scene/chat_dashboard/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-05 08:29:49.000000 db-gpt-0.2.7/pilot/scene/chat_dashboard/__init__.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:08.092163 db-gpt-0.2.7/pilot/scene/chat_dashboard/business_cockpit/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-05 08:29:49.000000 db-gpt-0.2.7/pilot/scene/chat_dashboard/business_cockpit/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     4957 2023-07-10 06:54:41.000000 db-gpt-0.2.7/pilot/scene/chat_dashboard/chat.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:08.092891 db-gpt-0.2.7/pilot/scene/chat_dashboard/data_preparation/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-05 08:29:49.000000 db-gpt-0.2.7/pilot/scene/chat_dashboard/data_preparation/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1383 2023-07-10 06:54:41.000000 db-gpt-0.2.7/pilot/scene/chat_dashboard/data_preparation/report_schma.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1359 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/scene/chat_dashboard/out_parser.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2432 2023-07-10 06:54:41.000000 db-gpt-0.2.7/pilot/scene/chat_dashboard/prompt.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:08.093843 db-gpt-0.2.7/pilot/scene/chat_db/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/scene/chat_db/__init__.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:08.096064 db-gpt-0.2.7/pilot/scene/chat_db/auto_execute/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/scene/chat_db/auto_execute/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1969 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/scene/chat_db/auto_execute/chat.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1218 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/scene/chat_db/auto_execute/example.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2285 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/scene/chat_db/auto_execute/out_parser.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2257 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/scene/chat_db/auto_execute/prompt.py
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/scene/chat_db/example.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:08.098095 db-gpt-0.2.7/pilot/scene/chat_db/professional_qa/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/scene/chat_db/professional_qa/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2047 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/scene/chat_db/professional_qa/chat.py
--rw-r--r--   0 chenketing   (502) staff       (20)      521 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/scene/chat_db/professional_qa/out_parser.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2634 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/scene/chat_db/professional_qa/prompt.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:08.101280 db-gpt-0.2.7/pilot/scene/chat_execution/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/scene/chat_execution/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2830 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/scene/chat_execution/chat.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1182 2023-07-06 05:46:38.000000 db-gpt-0.2.7/pilot/scene/chat_execution/example.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1510 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/scene/chat_execution/out_parser.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1732 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/scene/chat_execution/prompt.py
--rw-r--r--   0 chenketing   (502) staff       (20)        1 2023-07-05 08:29:49.000000 db-gpt-0.2.7/pilot/scene/chat_execution/prompt_v2.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1216 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/scene/chat_factory.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:08.101942 db-gpt-0.2.7/pilot/scene/chat_knowledge/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/scene/chat_knowledge/__init__.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:08.103957 db-gpt-0.2.7/pilot/scene/chat_knowledge/custom/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/scene/chat_knowledge/custom/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1882 2023-07-11 02:36:56.000000 db-gpt-0.2.7/pilot/scene/chat_knowledge/custom/chat.py
--rw-r--r--   0 chenketing   (502) staff       (20)      521 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/scene/chat_knowledge/custom/out_parser.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1881 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/scene/chat_knowledge/custom/prompt.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:08.105816 db-gpt-0.2.7/pilot/scene/chat_knowledge/default/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/scene/chat_knowledge/default/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2088 2023-07-11 02:46:32.000000 db-gpt-0.2.7/pilot/scene/chat_knowledge/default/chat.py
--rw-r--r--   0 chenketing   (502) staff       (20)      521 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/scene/chat_knowledge/default/out_parser.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1979 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/scene/chat_knowledge/default/prompt.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:08.108071 db-gpt-0.2.7/pilot/scene/chat_knowledge/inner_db_summary/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/scene/chat_knowledge/inner_db_summary/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1036 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/scene/chat_knowledge/inner_db_summary/chat.py
--rw-r--r--   0 chenketing   (502) staff       (20)      709 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/scene/chat_knowledge/inner_db_summary/out_parser.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1507 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/scene/chat_knowledge/inner_db_summary/prompt.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:08.110313 db-gpt-0.2.7/pilot/scene/chat_knowledge/url/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/scene/chat_knowledge/url/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2217 2023-07-11 02:46:32.000000 db-gpt-0.2.7/pilot/scene/chat_knowledge/url/chat.py
--rw-r--r--   0 chenketing   (502) staff       (20)      521 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/scene/chat_knowledge/url/out_parser.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1975 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/scene/chat_knowledge/url/prompt.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:08.112259 db-gpt-0.2.7/pilot/scene/chat_knowledge/v1/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-05 08:29:49.000000 db-gpt-0.2.7/pilot/scene/chat_knowledge/v1/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2073 2023-07-11 02:46:32.000000 db-gpt-0.2.7/pilot/scene/chat_knowledge/v1/chat.py
--rw-r--r--   0 chenketing   (502) staff       (20)      521 2023-07-05 08:29:49.000000 db-gpt-0.2.7/pilot/scene/chat_knowledge/v1/out_parser.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1972 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/scene/chat_knowledge/v1/prompt.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:08.114621 db-gpt-0.2.7/pilot/scene/chat_normal/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/scene/chat_normal/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1034 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/scene/chat_normal/chat.py
--rw-r--r--   0 chenketing   (502) staff       (20)      521 2023-06-30 02:43:35.000000 db-gpt-0.2.7/pilot/scene/chat_normal/out_parser.py
--rw-r--r--   0 chenketing   (502) staff       (20)      820 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/scene/chat_normal/prompt.py
--rw-r--r--   0 chenketing   (502) staff       (20)     4091 2023-07-05 08:29:49.000000 db-gpt-0.2.7/pilot/scene/message.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:08.121757 db-gpt-0.2.7/pilot/server/
--rw-r--r--   0 chenketing   (502) staff       (20)      312 2023-06-27 11:36:00.000000 db-gpt-0.2.7/pilot/server/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     3874 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/server/chat_adapter.py
--rw-r--r--   0 chenketing   (502) staff       (20)     3299 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/server/dbgpt_server.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2761 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/server/gradio_css.py
--rw-r--r--   0 chenketing   (502) staff       (20)     7338 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/server/gradio_patch.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:08.125651 db-gpt-0.2.7/pilot/server/knowledge/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/server/knowledge/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     5529 2023-07-10 07:05:37.000000 db-gpt-0.2.7/pilot/server/knowledge/api.py
--rw-r--r--   0 chenketing   (502) staff       (20)     4680 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/server/knowledge/chunk_db.py
--rw-r--r--   0 chenketing   (502) staff       (20)     5141 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/server/knowledge/document_db.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:08.131843 db-gpt-0.2.7/pilot/server/knowledge/request/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/server/knowledge/request/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1747 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/server/knowledge/request/request.py
--rw-r--r--   0 chenketing   (502) staff       (20)      721 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/server/knowledge/request/response.py
--rw-r--r--   0 chenketing   (502) staff       (20)     7435 2023-07-11 02:33:25.000000 db-gpt-0.2.7/pilot/server/knowledge/service.py
--rw-r--r--   0 chenketing   (502) staff       (20)     3902 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/server/knowledge/space_db.py
--rw-r--r--   0 chenketing   (502) staff       (20)     5841 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/server/llmserver.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2545 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/server/vectordb_qa.py
--rw-r--r--   0 chenketing   (502) staff       (20)    23645 2023-07-10 12:58:18.000000 db-gpt-0.2.7/pilot/server/webserver.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1622 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/server/webserver_base.py
--rw-r--r--   0 chenketing   (502) staff       (20)      697 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/singleton.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:08.136826 db-gpt-0.2.7/pilot/speech/
--rw-r--r--   0 chenketing   (502) staff       (20)       62 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/speech/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1114 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/speech/base.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1166 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/speech/brian.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2956 2023-07-05 08:29:49.000000 db-gpt-0.2.7/pilot/speech/eleven_labs.py
--rw-r--r--   0 chenketing   (502) staff       (20)      453 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/speech/gtts.py
--rw-r--r--   0 chenketing   (502) staff       (20)      518 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/speech/macos_tts.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1425 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/speech/say.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:08.138964 db-gpt-0.2.7/pilot/summary/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/summary/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)      635 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/summary/db_summary.py
--rw-r--r--   0 chenketing   (502) staff       (20)     6906 2023-07-11 02:46:32.000000 db-gpt-0.2.7/pilot/summary/db_summary_client.py
--rw-r--r--   0 chenketing   (502) staff       (20)     8382 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/summary/mysql_db_summary.py
--rw-r--r--   0 chenketing   (502) staff       (20)     4148 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/utils.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:08.172652 db-gpt-0.2.7/pilot/vector_store/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/vector_store/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1382 2023-07-11 02:25:57.000000 db-gpt-0.2.7/pilot/vector_store/chroma_store.py
--rw-r--r--   0 chenketing   (502) staff       (20)     1042 2023-07-05 08:29:49.000000 db-gpt-0.2.7/pilot/vector_store/connector.py
--rw-r--r--   0 chenketing   (502) staff       (20)     2594 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/vector_store/extract_tovec.py
--rw-r--r--   0 chenketing   (502) staff       (20)     3587 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/vector_store/file_loader.py
--rw-r--r--   0 chenketing   (502) staff       (20)    12126 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/vector_store/milvus_store.py
--rw-r--r--   0 chenketing   (502) staff       (20)      506 2023-06-20 09:57:25.000000 db-gpt-0.2.7/pilot/vector_store/vector_store_base.py
--rw-r--r--   0 chenketing   (502) staff       (20)     5312 2023-07-06 07:40:51.000000 db-gpt-0.2.7/pilot/vector_store/weaviate_store.py
--rw-r--r--   0 chenketing   (502) staff       (20)       38 2023-07-11 02:52:08.176444 db-gpt-0.2.7/setup.cfg
--rw-r--r--   0 chenketing   (502) staff       (20)     1201 2023-07-11 02:51:38.000000 db-gpt-0.2.7/setup.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:08.173380 db-gpt-0.2.7/tests/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.7/tests/__init__.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:08.174015 db-gpt-0.2.7/tests/unit/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-10 07:52:37.000000 db-gpt-0.2.7/tests/unit/__init__.py
-drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 02:52:08.175066 db-gpt-0.2.7/tests/unit/embedding_engine/
--rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-10 07:53:06.000000 db-gpt-0.2.7/tests/unit/embedding_engine/__init__.py
--rw-r--r--   0 chenketing   (502) staff       (20)      678 2023-07-11 02:33:25.000000 db-gpt-0.2.7/tests/unit/embedding_engine/test_url_embedding.py
--rw-r--r--   0 chenketing   (502) staff       (20)     4480 2023-06-20 09:57:25.000000 db-gpt-0.2.7/tests/unit/test_plugins.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.614894 db-gpt-0.2.8/
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.469304 db-gpt-0.2.8/DB_GPT.egg-info/
+-rw-r--r--   0 chenketing   (502) staff       (20)     8144 2023-07-11 07:35:39.000000 db-gpt-0.2.8/DB_GPT.egg-info/PKG-INFO
+-rw-r--r--   0 chenketing   (502) staff       (20)     6845 2023-07-11 07:35:39.000000 db-gpt-0.2.8/DB_GPT.egg-info/SOURCES.txt
+-rw-r--r--   0 chenketing   (502) staff       (20)        1 2023-07-11 07:35:39.000000 db-gpt-0.2.8/DB_GPT.egg-info/dependency_links.txt
+-rw-r--r--   0 chenketing   (502) staff       (20)       56 2023-07-11 07:35:39.000000 db-gpt-0.2.8/DB_GPT.egg-info/entry_points.txt
+-rw-r--r--   0 chenketing   (502) staff       (20)     1155 2023-07-11 07:35:39.000000 db-gpt-0.2.8/DB_GPT.egg-info/requires.txt
+-rw-r--r--   0 chenketing   (502) staff       (20)       12 2023-07-11 07:35:39.000000 db-gpt-0.2.8/DB_GPT.egg-info/top_level.txt
+-rw-r--r--   0 chenketing   (502) staff       (20)     1067 2023-06-20 09:57:25.000000 db-gpt-0.2.8/LICENSE
+-rw-r--r--   0 chenketing   (502) staff       (20)     8144 2023-07-11 07:35:39.614493 db-gpt-0.2.8/PKG-INFO
+-rw-r--r--   0 chenketing   (502) staff       (20)     7613 2023-07-10 06:54:41.000000 db-gpt-0.2.8/README.md
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.472997 db-gpt-0.2.8/pilot/
+-rw-r--r--   0 chenketing   (502) staff       (20)      206 2023-07-10 08:01:44.000000 db-gpt-0.2.8/pilot/__init__.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.475656 db-gpt-0.2.8/pilot/agent/
+-rw-r--r--   0 chenketing   (502) staff       (20)       46 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/agent/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      179 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/agent/agent.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2266 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/agent/agent_manager.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     4025 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/agent/json_fix_llm.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.477034 db-gpt-0.2.8/pilot/chain/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/chain/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)       46 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/chain/audio.py
+-rw-r--r--   0 chenketing   (502) staff       (20)       47 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/chain/visual.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.479255 db-gpt-0.2.8/pilot/commands/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/commands/__init__.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.480535 db-gpt-0.2.8/pilot/commands/built_in/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/commands/built_in/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1430 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/commands/built_in/audio_text.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     3509 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/commands/built_in/image_gen.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     4602 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/commands/command.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     5168 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/commands/command_mange.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      128 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/commands/exception_not_commands.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      244 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/commands/times.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.484603 db-gpt-0.2.8/pilot/common/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/common/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      803 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/common/custom_data_structure.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1516 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/common/formatting.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     3044 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/common/markdown_text.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     6545 2023-06-27 11:35:59.000000 db-gpt-0.2.8/pilot/common/plugins.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      239 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/common/schema.py
+-rw-r--r--   0 chenketing   (502) staff       (20)    17355 2023-07-10 06:54:41.000000 db-gpt-0.2.8/pilot/common/sql_database.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.486621 db-gpt-0.2.8/pilot/configs/
+-rw-r--r--   0 chenketing   (502) staff       (20)      452 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/configs/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     7429 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/configs/config.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2219 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/configs/model_config.py
+-rw-r--r--   0 chenketing   (502) staff       (20)    13673 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/conversation.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.496369 db-gpt-0.2.8/pilot/embedding_engine/
+-rw-r--r--   0 chenketing   (502) staff       (20)      877 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/embedding_engine/EncodeTextLoader.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      289 2023-07-10 08:01:44.000000 db-gpt-0.2.8/pilot/embedding_engine/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2486 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/embedding_engine/chn_document_splitter.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1023 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/embedding_engine/csv_embedding.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2459 2023-07-11 07:28:43.000000 db-gpt-0.2.8/pilot/embedding_engine/embedding_engine.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.497094 db-gpt-0.2.8/pilot/embedding_engine/external/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/embedding_engine/external/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     3649 2023-07-11 02:16:19.000000 db-gpt-0.2.8/pilot/embedding_engine/knowledge_type.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2200 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/embedding_engine/markdown_embedding.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2052 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/embedding_engine/pdf_embedding.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2102 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/embedding_engine/pdf_loader.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1965 2023-07-10 07:29:21.000000 db-gpt-0.2.8/pilot/embedding_engine/ppt_embedding.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1729 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/embedding_engine/search_milvus.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     3094 2023-07-11 07:34:47.000000 db-gpt-0.2.8/pilot/embedding_engine/source_embedding.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      883 2023-07-10 07:28:43.000000 db-gpt-0.2.8/pilot/embedding_engine/string_embedding.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1922 2023-07-10 07:28:43.000000 db-gpt-0.2.8/pilot/embedding_engine/url_embedding.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1793 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/embedding_engine/word_embedding.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.497690 db-gpt-0.2.8/pilot/inference_parsers/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/inference_parsers/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2234 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/inference_parsers/base.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.499344 db-gpt-0.2.8/pilot/json_utils/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/json_utils/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     3609 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/json_utils/json_fix_general.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2270 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/json_utils/utilities.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.500359 db-gpt-0.2.8/pilot/log/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/log/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      531 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/log/json_handler.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     9846 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/logs.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.501033 db-gpt-0.2.8/pilot/memory/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/memory/__init__.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.503823 db-gpt-0.2.8/pilot/memory/chat_history/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/memory/chat_history/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1079 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/memory/chat_history/base.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     5319 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/memory/chat_history/duckdb_history.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1496 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/memory/chat_history/file_history.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      968 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/memory/chat_history/mem_history.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.507772 db-gpt-0.2.8/pilot/model/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/model/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     6541 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/model/adapter.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      206 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/model/base.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.510962 db-gpt-0.2.8/pilot/model/cache/
+-rw-r--r--   0 chenketing   (502) staff       (20)      130 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/model/cache/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      617 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/model/cache/base.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      718 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/model/cache/disk_cache.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1060 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/model/cache/gpt_cache.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      599 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/model/cache/memory_cache.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     3955 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/model/compression.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.516836 db-gpt-0.2.8/pilot/model/llm_out/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/model/llm_out/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2251 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/model/llm_out/chatglm_llm.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1546 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/model/llm_out/falcon_llm.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2001 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/model/llm_out/gorilla_llm.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      568 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/model/llm_out/gpt4all_llm.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     3276 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/model/llm_out/guanaco_llm.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2679 2023-07-10 06:54:41.000000 db-gpt-0.2.8/pilot/model/llm_out/proxy_llm.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     7674 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/model/llm_out/vicuna_base_llm.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2606 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/model/llm_out/vicuna_llm.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     3113 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/model/llm_utils.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     3949 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/model/loader.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.517493 db-gpt-0.2.8/pilot/model/proxy/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/model/proxy/__init__.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.517795 db-gpt-0.2.8/pilot/openapi/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/openapi/__init__.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.519038 db-gpt-0.2.8/pilot/openapi/api_v1/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-26 11:33:41.000000 db-gpt-0.2.8/pilot/openapi/api_v1/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     9550 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/openapi/api_v1/api_v1.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1559 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/openapi/api_v1/api_view_model.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.520091 db-gpt-0.2.8/pilot/out_parser/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/out_parser/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     8144 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/out_parser/base.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.523707 db-gpt-0.2.8/pilot/prompts/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/prompts/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1453 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/prompts/base.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1063 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/prompts/example_base.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     5623 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/prompts/generator.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2596 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/prompts/prompt_new.py
+-rw-r--r--   0 chenketing   (502) staff       (20)    11978 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/prompts/prompt_template.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.527233 db-gpt-0.2.8/pilot/scene/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/scene/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2437 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/base.py
+-rw-r--r--   0 chenketing   (502) staff       (20)    12576 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/base_chat.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     3683 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/scene/base_message.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.529295 db-gpt-0.2.8/pilot/scene/chat_dashboard/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/scene/chat_dashboard/__init__.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.530151 db-gpt-0.2.8/pilot/scene/chat_dashboard/business_cockpit/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/scene/chat_dashboard/business_cockpit/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     4957 2023-07-10 06:54:41.000000 db-gpt-0.2.8/pilot/scene/chat_dashboard/chat.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.530858 db-gpt-0.2.8/pilot/scene/chat_dashboard/data_preparation/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/scene/chat_dashboard/data_preparation/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1383 2023-07-10 06:54:41.000000 db-gpt-0.2.8/pilot/scene/chat_dashboard/data_preparation/report_schma.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1359 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/chat_dashboard/out_parser.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2432 2023-07-10 06:54:41.000000 db-gpt-0.2.8/pilot/scene/chat_dashboard/prompt.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.531803 db-gpt-0.2.8/pilot/scene/chat_db/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/scene/chat_db/__init__.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.533876 db-gpt-0.2.8/pilot/scene/chat_db/auto_execute/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/scene/chat_db/auto_execute/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1969 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/chat_db/auto_execute/chat.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1218 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/chat_db/auto_execute/example.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2285 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/chat_db/auto_execute/out_parser.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2257 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/chat_db/auto_execute/prompt.py
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/scene/chat_db/example.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.535848 db-gpt-0.2.8/pilot/scene/chat_db/professional_qa/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/scene/chat_db/professional_qa/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2047 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/chat_db/professional_qa/chat.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      521 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/scene/chat_db/professional_qa/out_parser.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2634 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/chat_db/professional_qa/prompt.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.538569 db-gpt-0.2.8/pilot/scene/chat_execution/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/scene/chat_execution/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2830 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/chat_execution/chat.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1182 2023-07-06 05:46:38.000000 db-gpt-0.2.8/pilot/scene/chat_execution/example.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1510 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/chat_execution/out_parser.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1732 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/chat_execution/prompt.py
+-rw-r--r--   0 chenketing   (502) staff       (20)        1 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/scene/chat_execution/prompt_v2.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1216 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/chat_factory.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.539125 db-gpt-0.2.8/pilot/scene/chat_knowledge/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/__init__.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.540987 db-gpt-0.2.8/pilot/scene/chat_knowledge/custom/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/custom/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1882 2023-07-11 02:36:56.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/custom/chat.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      521 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/custom/out_parser.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1881 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/custom/prompt.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.542880 db-gpt-0.2.8/pilot/scene/chat_knowledge/default/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/default/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2088 2023-07-11 02:46:32.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/default/chat.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      521 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/default/out_parser.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1979 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/default/prompt.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.544808 db-gpt-0.2.8/pilot/scene/chat_knowledge/inner_db_summary/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/inner_db_summary/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1036 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/inner_db_summary/chat.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      709 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/inner_db_summary/out_parser.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1507 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/inner_db_summary/prompt.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.546787 db-gpt-0.2.8/pilot/scene/chat_knowledge/url/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/url/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2217 2023-07-11 02:46:32.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/url/chat.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      521 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/url/out_parser.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1975 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/url/prompt.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.548805 db-gpt-0.2.8/pilot/scene/chat_knowledge/v1/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/v1/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2073 2023-07-11 02:46:32.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/v1/chat.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      521 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/v1/out_parser.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1972 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/chat_knowledge/v1/prompt.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.551115 db-gpt-0.2.8/pilot/scene/chat_normal/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/scene/chat_normal/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1034 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/chat_normal/chat.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      521 2023-06-30 02:43:35.000000 db-gpt-0.2.8/pilot/scene/chat_normal/out_parser.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      820 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/scene/chat_normal/prompt.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     4091 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/scene/message.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.557182 db-gpt-0.2.8/pilot/server/
+-rw-r--r--   0 chenketing   (502) staff       (20)      312 2023-06-27 11:36:00.000000 db-gpt-0.2.8/pilot/server/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     3874 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/server/chat_adapter.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     3299 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/server/dbgpt_server.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2761 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/server/gradio_css.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     7338 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/server/gradio_patch.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.590366 db-gpt-0.2.8/pilot/server/knowledge/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/server/knowledge/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     5529 2023-07-10 07:05:37.000000 db-gpt-0.2.8/pilot/server/knowledge/api.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     4680 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/server/knowledge/chunk_db.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     5141 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/server/knowledge/document_db.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.592923 db-gpt-0.2.8/pilot/server/knowledge/request/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/server/knowledge/request/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1747 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/server/knowledge/request/request.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      721 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/server/knowledge/request/response.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     7435 2023-07-11 02:33:25.000000 db-gpt-0.2.8/pilot/server/knowledge/service.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     3902 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/server/knowledge/space_db.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     5841 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/server/llmserver.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2545 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/server/vectordb_qa.py
+-rw-r--r--   0 chenketing   (502) staff       (20)    23645 2023-07-10 12:58:18.000000 db-gpt-0.2.8/pilot/server/webserver.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1622 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/server/webserver_base.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      697 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/singleton.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.598541 db-gpt-0.2.8/pilot/speech/
+-rw-r--r--   0 chenketing   (502) staff       (20)       62 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/speech/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1114 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/speech/base.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1166 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/speech/brian.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2956 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/speech/eleven_labs.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      453 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/speech/gtts.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      518 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/speech/macos_tts.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1425 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/speech/say.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.601706 db-gpt-0.2.8/pilot/summary/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/summary/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      635 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/summary/db_summary.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     6906 2023-07-11 02:46:32.000000 db-gpt-0.2.8/pilot/summary/db_summary_client.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     8382 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/summary/mysql_db_summary.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     4148 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/utils.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.609608 db-gpt-0.2.8/pilot/vector_store/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/vector_store/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1382 2023-07-11 02:25:57.000000 db-gpt-0.2.8/pilot/vector_store/chroma_store.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     1042 2023-07-05 08:29:49.000000 db-gpt-0.2.8/pilot/vector_store/connector.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     2594 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/vector_store/extract_tovec.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     3587 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/vector_store/file_loader.py
+-rw-r--r--   0 chenketing   (502) staff       (20)    12126 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/vector_store/milvus_store.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      506 2023-06-20 09:57:25.000000 db-gpt-0.2.8/pilot/vector_store/vector_store_base.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     5312 2023-07-06 07:40:51.000000 db-gpt-0.2.8/pilot/vector_store/weaviate_store.py
+-rw-r--r--   0 chenketing   (502) staff       (20)       38 2023-07-11 07:35:39.615054 db-gpt-0.2.8/setup.cfg
+-rw-r--r--   0 chenketing   (502) staff       (20)     1201 2023-07-11 07:35:28.000000 db-gpt-0.2.8/setup.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.610825 db-gpt-0.2.8/tests/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-06-20 09:57:25.000000 db-gpt-0.2.8/tests/__init__.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.611998 db-gpt-0.2.8/tests/unit/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-10 07:52:37.000000 db-gpt-0.2.8/tests/unit/__init__.py
+drwxr-xr-x   0 chenketing   (502) staff       (20)        0 2023-07-11 07:35:39.613502 db-gpt-0.2.8/tests/unit/embedding_engine/
+-rw-r--r--   0 chenketing   (502) staff       (20)        0 2023-07-10 07:53:06.000000 db-gpt-0.2.8/tests/unit/embedding_engine/__init__.py
+-rw-r--r--   0 chenketing   (502) staff       (20)      678 2023-07-11 02:33:25.000000 db-gpt-0.2.8/tests/unit/embedding_engine/test_url_embedding.py
+-rw-r--r--   0 chenketing   (502) staff       (20)     4480 2023-06-20 09:57:25.000000 db-gpt-0.2.8/tests/unit/test_plugins.py
```

### Comparing `db-gpt-0.2.7/DB_GPT.egg-info/PKG-INFO` & `db-gpt-0.2.8/DB_GPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: db-gpt
-Version: 0.2.7
+Version: 0.2.8
 Summary: DB-GPT is an experimental open-source project that uses localized GPT large models to interact with your data and environment. With this solution, you can be assured that there is no risk of data leakage, and your data is 100% private and secure.
 Home-page: https://github.com/csunny/DB-GPT
 Author: csunny
 Author-email: cfqcsunny@gmail.com
 License: https://opensource.org/license/mit/
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: db-gpt Version: 0.2.7 Summary: DB-GPT is an
+Metadata-Version: 2.1 Name: db-gpt Version: 0.2.8 Summary: DB-GPT is an
 experimental open-source project that uses localized GPT large models to
 interact with your data and environment. With this solution, you can be assured
 that there is no risk of data leakage, and your data is 100% private and
 secure. Home-page: https://github.com/csunny/DB-GPT Author: csunny Author-
 email: cfqcsunny@gmail.com License: https://opensource.org/license/mit/
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
 LICENSE # DB-GPT: Revolutionizing Database Interactions with Private LLM
```

### Comparing `db-gpt-0.2.7/DB_GPT.egg-info/SOURCES.txt` & `db-gpt-0.2.8/DB_GPT.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/DB_GPT.egg-info/requires.txt` & `db-gpt-0.2.8/DB_GPT.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/LICENSE` & `db-gpt-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/PKG-INFO` & `db-gpt-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: db-gpt
-Version: 0.2.7
+Version: 0.2.8
 Summary: DB-GPT is an experimental open-source project that uses localized GPT large models to interact with your data and environment. With this solution, you can be assured that there is no risk of data leakage, and your data is 100% private and secure.
 Home-page: https://github.com/csunny/DB-GPT
 Author: csunny
 Author-email: cfqcsunny@gmail.com
 License: https://opensource.org/license/mit/
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: db-gpt Version: 0.2.7 Summary: DB-GPT is an
+Metadata-Version: 2.1 Name: db-gpt Version: 0.2.8 Summary: DB-GPT is an
 experimental open-source project that uses localized GPT large models to
 interact with your data and environment. With this solution, you can be assured
 that there is no risk of data leakage, and your data is 100% private and
 secure. Home-page: https://github.com/csunny/DB-GPT Author: csunny Author-
 email: cfqcsunny@gmail.com License: https://opensource.org/license/mit/
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
 LICENSE # DB-GPT: Revolutionizing Database Interactions with Private LLM
```

### Comparing `db-gpt-0.2.7/README.md` & `db-gpt-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/agent/agent_manager.py` & `db-gpt-0.2.8/pilot/agent/agent_manager.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/agent/json_fix_llm.py` & `db-gpt-0.2.8/pilot/agent/json_fix_llm.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/commands/built_in/audio_text.py` & `db-gpt-0.2.8/pilot/commands/built_in/audio_text.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/commands/built_in/image_gen.py` & `db-gpt-0.2.8/pilot/commands/built_in/image_gen.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/commands/command.py` & `db-gpt-0.2.8/pilot/commands/command.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/commands/command_mange.py` & `db-gpt-0.2.8/pilot/commands/command_mange.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/common/custom_data_structure.py` & `db-gpt-0.2.8/pilot/common/custom_data_structure.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/common/formatting.py` & `db-gpt-0.2.8/pilot/common/formatting.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/common/markdown_text.py` & `db-gpt-0.2.8/pilot/common/markdown_text.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/common/plugins.py` & `db-gpt-0.2.8/pilot/common/plugins.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/common/sql_database.py` & `db-gpt-0.2.8/pilot/common/sql_database.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/configs/config.py` & `db-gpt-0.2.8/pilot/configs/config.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/configs/model_config.py` & `db-gpt-0.2.8/pilot/configs/model_config.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/conversation.py` & `db-gpt-0.2.8/pilot/conversation.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/embedding_engine/EncodeTextLoader.py` & `db-gpt-0.2.8/pilot/embedding_engine/EncodeTextLoader.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/embedding_engine/chn_document_splitter.py` & `db-gpt-0.2.8/pilot/embedding_engine/chn_document_splitter.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/embedding_engine/csv_embedding.py` & `db-gpt-0.2.8/pilot/embedding_engine/csv_embedding.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/embedding_engine/embedding_engine.py` & `db-gpt-0.2.8/pilot/embedding_engine/embedding_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 from typing import Optional
 
 from chromadb.errors import NotEnoughElementsException
 from langchain.embeddings import HuggingFaceEmbeddings
 
-from pilot.configs.config import Config
 from pilot.embedding_engine.knowledge_type import get_knowledge_embedding, KnowledgeType
 from pilot.vector_store.connector import VectorStoreConnector
 
-CFG = Config()
-
 
 class EmbeddingEngine:
     def __init__(
         self,
         model_name,
         vector_store_config,
         knowledge_type: Optional[str] = KnowledgeType.DOCUMENT.value,
```

### Comparing `db-gpt-0.2.7/pilot/embedding_engine/knowledge_type.py` & `db-gpt-0.2.8/pilot/embedding_engine/knowledge_type.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/embedding_engine/markdown_embedding.py` & `db-gpt-0.2.8/pilot/embedding_engine/markdown_embedding.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/embedding_engine/pdf_embedding.py` & `db-gpt-0.2.8/pilot/embedding_engine/pdf_embedding.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/embedding_engine/pdf_loader.py` & `db-gpt-0.2.8/pilot/embedding_engine/pdf_loader.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/embedding_engine/ppt_embedding.py` & `db-gpt-0.2.8/pilot/embedding_engine/ppt_embedding.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/embedding_engine/search_milvus.py` & `db-gpt-0.2.8/pilot/embedding_engine/search_milvus.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/embedding_engine/source_embedding.py` & `db-gpt-0.2.8/pilot/embedding_engine/source_embedding.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 from abc import ABC, abstractmethod
 from typing import Dict, List, Optional
 
 from chromadb.errors import NotEnoughElementsException
-from pilot.configs.config import Config
 from pilot.vector_store.connector import VectorStoreConnector
 
 registered_methods = []
-CFG = Config()
 
 
 def register(method):
     registered_methods.append(method.__name__)
     return method
 
 
@@ -53,33 +51,33 @@
         """transform vector"""
         pass
 
     @register
     def index_to_store(self, docs):
         """index to vector store"""
         self.vector_client = VectorStoreConnector(
-            CFG.VECTOR_STORE_TYPE, self.vector_store_config
+            self.vector_store_config["vector_store_type"], self.vector_store_config
         )
         return self.vector_client.load_document(docs)
 
     @register
     def similar_search(self, doc, topk):
         """vector store similarity_search"""
         self.vector_client = VectorStoreConnector(
-            CFG.VECTOR_STORE_TYPE, self.vector_store_config
+            self.vector_store_config["vector_store_type"], self.vector_store_config
         )
         try:
             ans = self.vector_client.similar_search(doc, topk)
         except NotEnoughElementsException:
             ans = self.vector_client.similar_search(doc, 1)
         return ans
 
     def vector_name_exist(self):
         self.vector_client = VectorStoreConnector(
-            CFG.VECTOR_STORE_TYPE, self.vector_store_config
+            self.vector_store_config["vector_store_type"], self.vector_store_config
         )
         return self.vector_client.vector_name_exists()
 
     def source_embedding(self):
         if "read" in registered_methods:
             text = self.read()
         if "data_process" in registered_methods:
```

### Comparing `db-gpt-0.2.7/pilot/embedding_engine/string_embedding.py` & `db-gpt-0.2.8/pilot/embedding_engine/string_embedding.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/embedding_engine/url_embedding.py` & `db-gpt-0.2.8/pilot/embedding_engine/url_embedding.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/embedding_engine/word_embedding.py` & `db-gpt-0.2.8/pilot/embedding_engine/word_embedding.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/inference_parsers/base.py` & `db-gpt-0.2.8/pilot/inference_parsers/base.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/json_utils/json_fix_general.py` & `db-gpt-0.2.8/pilot/json_utils/json_fix_general.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/json_utils/utilities.py` & `db-gpt-0.2.8/pilot/json_utils/utilities.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/log/json_handler.py` & `db-gpt-0.2.8/pilot/log/json_handler.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/logs.py` & `db-gpt-0.2.8/pilot/logs.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/memory/chat_history/base.py` & `db-gpt-0.2.8/pilot/memory/chat_history/base.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/memory/chat_history/duckdb_history.py` & `db-gpt-0.2.8/pilot/memory/chat_history/duckdb_history.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/memory/chat_history/file_history.py` & `db-gpt-0.2.8/pilot/memory/chat_history/file_history.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/memory/chat_history/mem_history.py` & `db-gpt-0.2.8/pilot/memory/chat_history/mem_history.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/model/adapter.py` & `db-gpt-0.2.8/pilot/model/adapter.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/model/cache/base.py` & `db-gpt-0.2.8/pilot/model/cache/base.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/model/cache/disk_cache.py` & `db-gpt-0.2.8/pilot/model/cache/disk_cache.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/model/cache/gpt_cache.py` & `db-gpt-0.2.8/pilot/model/cache/gpt_cache.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/model/cache/memory_cache.py` & `db-gpt-0.2.8/pilot/model/cache/memory_cache.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/model/compression.py` & `db-gpt-0.2.8/pilot/model/compression.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/model/llm_out/chatglm_llm.py` & `db-gpt-0.2.8/pilot/model/llm_out/chatglm_llm.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/model/llm_out/falcon_llm.py` & `db-gpt-0.2.8/pilot/model/llm_out/falcon_llm.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/model/llm_out/gorilla_llm.py` & `db-gpt-0.2.8/pilot/model/llm_out/gorilla_llm.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/model/llm_out/gpt4all_llm.py` & `db-gpt-0.2.8/pilot/model/llm_out/gpt4all_llm.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/model/llm_out/guanaco_llm.py` & `db-gpt-0.2.8/pilot/model/llm_out/guanaco_llm.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/model/llm_out/proxy_llm.py` & `db-gpt-0.2.8/pilot/model/llm_out/proxy_llm.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/model/llm_out/vicuna_base_llm.py` & `db-gpt-0.2.8/pilot/model/llm_out/vicuna_base_llm.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/model/llm_out/vicuna_llm.py` & `db-gpt-0.2.8/pilot/model/llm_out/vicuna_llm.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/model/llm_utils.py` & `db-gpt-0.2.8/pilot/model/llm_utils.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/model/loader.py` & `db-gpt-0.2.8/pilot/model/loader.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/openapi/api_v1/api_v1.py` & `db-gpt-0.2.8/pilot/openapi/api_v1/api_v1.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/openapi/api_v1/api_view_model.py` & `db-gpt-0.2.8/pilot/openapi/api_v1/api_view_model.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/out_parser/base.py` & `db-gpt-0.2.8/pilot/out_parser/base.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/prompts/base.py` & `db-gpt-0.2.8/pilot/prompts/base.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/prompts/example_base.py` & `db-gpt-0.2.8/pilot/prompts/example_base.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/prompts/generator.py` & `db-gpt-0.2.8/pilot/prompts/generator.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/prompts/prompt_new.py` & `db-gpt-0.2.8/pilot/prompts/prompt_new.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/prompts/prompt_template.py` & `db-gpt-0.2.8/pilot/prompts/prompt_template.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/scene/base.py` & `db-gpt-0.2.8/pilot/scene/base.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/scene/base_chat.py` & `db-gpt-0.2.8/pilot/scene/base_chat.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/scene/base_message.py` & `db-gpt-0.2.8/pilot/scene/base_message.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/scene/chat_dashboard/chat.py` & `db-gpt-0.2.8/pilot/scene/chat_dashboard/chat.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/scene/chat_dashboard/data_preparation/report_schma.py` & `db-gpt-0.2.8/pilot/scene/chat_dashboard/data_preparation/report_schma.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/scene/chat_dashboard/out_parser.py` & `db-gpt-0.2.8/pilot/scene/chat_dashboard/out_parser.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/scene/chat_dashboard/prompt.py` & `db-gpt-0.2.8/pilot/scene/chat_dashboard/prompt.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/scene/chat_db/auto_execute/chat.py` & `db-gpt-0.2.8/pilot/scene/chat_db/auto_execute/chat.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/scene/chat_db/auto_execute/example.py` & `db-gpt-0.2.8/pilot/scene/chat_db/auto_execute/example.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/scene/chat_db/auto_execute/out_parser.py` & `db-gpt-0.2.8/pilot/scene/chat_db/auto_execute/out_parser.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/scene/chat_db/auto_execute/prompt.py` & `db-gpt-0.2.8/pilot/scene/chat_db/auto_execute/prompt.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/scene/chat_db/professional_qa/chat.py` & `db-gpt-0.2.8/pilot/scene/chat_db/professional_qa/chat.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/scene/chat_db/professional_qa/out_parser.py` & `db-gpt-0.2.8/pilot/scene/chat_db/professional_qa/out_parser.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/scene/chat_db/professional_qa/prompt.py` & `db-gpt-0.2.8/pilot/scene/chat_db/professional_qa/prompt.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/scene/chat_execution/chat.py` & `db-gpt-0.2.8/pilot/scene/chat_execution/chat.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/scene/chat_execution/example.py` & `db-gpt-0.2.8/pilot/scene/chat_execution/example.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/scene/chat_execution/out_parser.py` & `db-gpt-0.2.8/pilot/scene/chat_execution/out_parser.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/scene/chat_execution/prompt.py` & `db-gpt-0.2.8/pilot/scene/chat_execution/prompt.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/scene/chat_factory.py` & `db-gpt-0.2.8/pilot/scene/chat_factory.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/scene/chat_knowledge/custom/chat.py` & `db-gpt-0.2.8/pilot/scene/chat_knowledge/custom/chat.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/scene/chat_knowledge/custom/out_parser.py` & `db-gpt-0.2.8/pilot/scene/chat_knowledge/custom/out_parser.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/scene/chat_knowledge/custom/prompt.py` & `db-gpt-0.2.8/pilot/scene/chat_knowledge/custom/prompt.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/scene/chat_knowledge/default/chat.py` & `db-gpt-0.2.8/pilot/scene/chat_knowledge/default/chat.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/scene/chat_knowledge/default/out_parser.py` & `db-gpt-0.2.8/pilot/scene/chat_knowledge/default/out_parser.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/scene/chat_knowledge/default/prompt.py` & `db-gpt-0.2.8/pilot/scene/chat_knowledge/default/prompt.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/scene/chat_knowledge/inner_db_summary/chat.py` & `db-gpt-0.2.8/pilot/scene/chat_knowledge/inner_db_summary/chat.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/scene/chat_knowledge/inner_db_summary/out_parser.py` & `db-gpt-0.2.8/pilot/scene/chat_knowledge/inner_db_summary/out_parser.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/scene/chat_knowledge/inner_db_summary/prompt.py` & `db-gpt-0.2.8/pilot/scene/chat_knowledge/inner_db_summary/prompt.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/scene/chat_knowledge/url/chat.py` & `db-gpt-0.2.8/pilot/scene/chat_knowledge/url/chat.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/scene/chat_knowledge/url/out_parser.py` & `db-gpt-0.2.8/pilot/scene/chat_knowledge/url/out_parser.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/scene/chat_knowledge/url/prompt.py` & `db-gpt-0.2.8/pilot/scene/chat_knowledge/url/prompt.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/scene/chat_knowledge/v1/chat.py` & `db-gpt-0.2.8/pilot/scene/chat_knowledge/v1/chat.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/scene/chat_knowledge/v1/out_parser.py` & `db-gpt-0.2.8/pilot/scene/chat_knowledge/v1/out_parser.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/scene/chat_knowledge/v1/prompt.py` & `db-gpt-0.2.8/pilot/scene/chat_knowledge/v1/prompt.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/scene/chat_normal/chat.py` & `db-gpt-0.2.8/pilot/scene/chat_normal/chat.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/scene/chat_normal/out_parser.py` & `db-gpt-0.2.8/pilot/scene/chat_normal/out_parser.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/scene/chat_normal/prompt.py` & `db-gpt-0.2.8/pilot/scene/chat_normal/prompt.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/scene/message.py` & `db-gpt-0.2.8/pilot/scene/message.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/server/chat_adapter.py` & `db-gpt-0.2.8/pilot/server/chat_adapter.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/server/dbgpt_server.py` & `db-gpt-0.2.8/pilot/server/dbgpt_server.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/server/gradio_css.py` & `db-gpt-0.2.8/pilot/server/gradio_css.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/server/gradio_patch.py` & `db-gpt-0.2.8/pilot/server/gradio_patch.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/server/knowledge/api.py` & `db-gpt-0.2.8/pilot/server/knowledge/api.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/server/knowledge/chunk_db.py` & `db-gpt-0.2.8/pilot/server/knowledge/chunk_db.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/server/knowledge/document_db.py` & `db-gpt-0.2.8/pilot/server/knowledge/document_db.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/server/knowledge/request/request.py` & `db-gpt-0.2.8/pilot/server/knowledge/request/request.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/server/knowledge/request/response.py` & `db-gpt-0.2.8/pilot/server/knowledge/request/response.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/server/knowledge/service.py` & `db-gpt-0.2.8/pilot/server/knowledge/service.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/server/knowledge/space_db.py` & `db-gpt-0.2.8/pilot/server/knowledge/space_db.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/server/llmserver.py` & `db-gpt-0.2.8/pilot/server/llmserver.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/server/vectordb_qa.py` & `db-gpt-0.2.8/pilot/server/vectordb_qa.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/server/webserver.py` & `db-gpt-0.2.8/pilot/server/webserver.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/server/webserver_base.py` & `db-gpt-0.2.8/pilot/server/webserver_base.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/singleton.py` & `db-gpt-0.2.8/pilot/singleton.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/speech/base.py` & `db-gpt-0.2.8/pilot/speech/base.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/speech/brian.py` & `db-gpt-0.2.8/pilot/speech/brian.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/speech/eleven_labs.py` & `db-gpt-0.2.8/pilot/speech/eleven_labs.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/speech/macos_tts.py` & `db-gpt-0.2.8/pilot/speech/macos_tts.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/speech/say.py` & `db-gpt-0.2.8/pilot/speech/say.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/summary/db_summary.py` & `db-gpt-0.2.8/pilot/summary/db_summary.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/summary/db_summary_client.py` & `db-gpt-0.2.8/pilot/summary/db_summary_client.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/summary/mysql_db_summary.py` & `db-gpt-0.2.8/pilot/summary/mysql_db_summary.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/utils.py` & `db-gpt-0.2.8/pilot/utils.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/vector_store/chroma_store.py` & `db-gpt-0.2.8/pilot/vector_store/chroma_store.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/vector_store/connector.py` & `db-gpt-0.2.8/pilot/vector_store/connector.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/vector_store/extract_tovec.py` & `db-gpt-0.2.8/pilot/vector_store/extract_tovec.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/vector_store/file_loader.py` & `db-gpt-0.2.8/pilot/vector_store/file_loader.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/vector_store/milvus_store.py` & `db-gpt-0.2.8/pilot/vector_store/milvus_store.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/pilot/vector_store/weaviate_store.py` & `db-gpt-0.2.8/pilot/vector_store/weaviate_store.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/setup.py` & `db-gpt-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             if require.strip() and not require.startswith("#")
         ]
 
 
 setuptools.setup(
     name="db-gpt",
     packages=find_packages(),
-    version="0.2.7",
+    version="0.2.8",
     author="csunny",
     author_email="cfqcsunny@gmail.com",
     description="DB-GPT is an experimental open-source project that uses localized GPT large models to interact with your data and environment."
     " With this solution, you can be assured that there is no risk of data leakage, and your data is 100% private and secure.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=parse_requirements("requirements.txt"),
```

### Comparing `db-gpt-0.2.7/tests/unit/embedding_engine/test_url_embedding.py` & `db-gpt-0.2.8/tests/unit/embedding_engine/test_url_embedding.py`

 * *Files identical despite different names*

### Comparing `db-gpt-0.2.7/tests/unit/test_plugins.py` & `db-gpt-0.2.8/tests/unit/test_plugins.py`

 * *Files identical despite different names*

