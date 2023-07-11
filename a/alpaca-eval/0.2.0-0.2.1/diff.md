# Comparing `tmp/alpaca_eval-0.2.0.tar.gz` & `tmp/alpaca_eval-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpaca_eval-0.2.0.tar", last modified: Sun Jul  9 00:13:54 2023, max compression
+gzip compressed data, was "alpaca_eval-0.2.1.tar", last modified: Tue Jul 11 01:19:06 2023, max compression
```

## Comparing `alpaca_eval-0.2.0.tar` & `alpaca_eval-0.2.1.tar`

### file list

```diff
@@ -1,200 +1,207 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.464719 alpaca_eval-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    66370 2023-07-09 00:13:54.464719 alpaca_eval-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    65548 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.432720 alpaca_eval-0.2.0/example/
--rw-r--r--   0 runner    (1001) docker     (123)   500735 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/example/outputs.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 00:13:54.464719 alpaca_eval-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.416720 alpaca_eval-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.436720 alpaca_eval-0.2.0/src/alpaca_eval/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-09 00:13:42.000000 alpaca_eval-0.2.0/src/alpaca_eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21377 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/analyze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.436720 alpaca_eval-0.2.0/src/alpaca_eval/annotators/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/annotators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33422 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/annotators/pairwise_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/completion_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.440720 alpaca_eval-0.2.0/src/alpaca_eval/decoders/
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/decoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/decoders/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/decoders/cohere.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/decoders/huggingface_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/decoders/huggingface_local.py
--rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/decoders/openai.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.440720 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.440720 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.440720 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.444720 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/alpaca_farm/
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.444720 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.448720 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/aviary_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/aviary_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.448720 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/chatgpt/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/chatgpt/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.448720 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/chatgpt_fn/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.448720 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/claude/
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/claude/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.448720 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/claude_ranking/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/claude_ranking/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.448720 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/cohere/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/cohere/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.448720 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.448720 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/guanaco_33b/
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/guanaco_33b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.452720 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.452720 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.452720 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/lmsys_gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/lmsys_gpt4/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.452720 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.452720 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/test/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/test/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.452720 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/text_davinci_003/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/text_davinci_003/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.420720 alpaca_eval-0.2.0/src/alpaca_eval/leaderboards/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.452720 alpaca_eval-0.2.0/src/alpaca_eval/leaderboards/data_AlpacaEval/
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/leaderboards/data_AlpacaEval/text_davinci_003_leaderboard.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.456719 alpaca_eval-0.2.0/src/alpaca_eval/leaderboards/evaluators/
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv
--rw-r--r--   0 runner    (1001) docker     (123)    21556 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.428720 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.456719 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/airoboros-33b/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/airoboros-33b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/airoboros-33b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.456719 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/airoboros-65b/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/airoboros-65b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.456719 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/alpaca-7b/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/alpaca-7b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/alpaca-7b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.456719 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.456719 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.456719 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/baize-v2-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/baize-v2-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/baize-v2-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.456719 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/baize-v2-7b/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/baize-v2-7b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.456719 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/chatgpt/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/chatgpt/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.456719 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/claude/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/claude/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/claude/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.456719 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/cohere/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/cohere/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/cohere/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.456719 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/cohere-chat/
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/cohere-chat/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.456719 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/falcon-40b-instruct/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/falcon-40b-instruct/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.456719 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/falcon-7b-instruct/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/falcon-7b-instruct/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.456719 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/gpt4/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/gpt4/chatml_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/gpt4/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.456719 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/guanaco-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/guanaco-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.456719 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/guanaco-33b/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/guanaco-33b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.456719 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/guanaco-65b/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/guanaco-65b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.456719 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/guanaco-7b/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/guanaco-7b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/guanaco-7b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.456719 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/minotaur-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/minotaur-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/minotaur-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.456719 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/nous-hermes-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/nous-hermes-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/nous-hermes-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.456719 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.456719 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/oasst-sft-llama-33b/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/oasst-sft-llama-33b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/oasst-sft-llama-33b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.460719 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.460719 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/openchat-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/openchat-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/openchat-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.460719 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/openchat-v2-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/openchat-v2-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.460719 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/openchat-v2-w-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/openchat-v2-w-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.460719 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/openchat8192-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/openchat8192-13b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.460719 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/opencoderplus-15b/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/opencoderplus-15b/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.460719 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/pythia-12b-mix-sft/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/pythia-12b-mix-sft/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.460719 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/text_davinci_001/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/text_davinci_001/configs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.460719 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/text_davinci_003/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/text_davinci_003/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/text_davinci_003/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.460719 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/ultralm-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/ultralm-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/ultralm-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.460719 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/vicuna-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/vicuna-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/vicuna-13b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.460719 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/vicuna-7b/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/vicuna-7b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/vicuna-7b/prompt.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.460719 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/wizardlm-13b/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/wizardlm-13b/configs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/models_configs/wizardlm-13b/prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20680 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/src/alpaca_eval/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.436720 alpaca_eval-0.2.0/src/alpaca_eval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    66370 2023-07-09 00:13:54.000000 alpaca_eval-0.2.0/src/alpaca_eval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-07-09 00:13:54.000000 alpaca_eval-0.2.0/src/alpaca_eval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 00:13:54.000000 alpaca_eval-0.2.0/src/alpaca_eval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-09 00:13:54.000000 alpaca_eval-0.2.0/src/alpaca_eval.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-09 00:13:54.000000 alpaca_eval-0.2.0/src/alpaca_eval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-09 00:13:54.000000 alpaca_eval-0.2.0/src/alpaca_eval.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 00:13:54.464719 alpaca_eval-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/tests/test_analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/tests/test_decoders_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-07-09 00:13:34.000000 alpaca_eval-0.2.0/tests/test_pairwise_evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.931748 alpaca_eval-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    66370 2023-07-11 01:19:06.931748 alpaca_eval-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    65548 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.911748 alpaca_eval-0.2.1/example/
+-rw-r--r--   0 runner    (1001) docker     (123)   500735 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/example/outputs.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 01:19:06.931748 alpaca_eval-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.907747 alpaca_eval-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.915748 alpaca_eval-0.2.1/src/alpaca_eval/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-11 01:18:53.000000 alpaca_eval-0.2.1/src/alpaca_eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21377 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/analyze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.915748 alpaca_eval-0.2.1/src/alpaca_eval/annotators/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/annotators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34017 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/annotators/pairwise_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/completion_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.915748 alpaca_eval-0.2.1/src/alpaca_eval/decoders/
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/decoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/decoders/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/decoders/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/decoders/huggingface_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/decoders/huggingface_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12959 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/decoders/openai.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.915748 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.915748 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.915748 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.919748 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.919748 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.919748 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/aviary_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/aviary_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.919748 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/chatgpt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/chatgpt/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.919748 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/chatgpt_fn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.919748 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/claude/
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/claude/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.919748 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/claude_ranking/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/claude_ranking/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.919748 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/cohere/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/cohere/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.919748 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.919748 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/guanaco_33b/
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/guanaco_33b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.919748 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/improved_aviary_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.919748 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/improved_lmsys_gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.923748 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/lmsys_gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/lmsys_gpt4/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.923748 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.923748 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/test/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.923748 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/text_davinci_003/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/text_davinci_003/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.907747 alpaca_eval-0.2.1/src/alpaca_eval/leaderboards/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.923748 alpaca_eval-0.2.1/src/alpaca_eval/leaderboards/data_AlpacaEval/
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/leaderboards/data_AlpacaEval/text_davinci_003_leaderboard.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.923748 alpaca_eval-0.2.1/src/alpaca_eval/leaderboards/evaluators/
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21739 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.911748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.923748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/airoboros-33b/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/airoboros-33b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/airoboros-33b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.923748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/airoboros-65b/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/airoboros-65b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.923748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/alpaca-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/alpaca-7b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/alpaca-7b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.923748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/alpaca-farm-ppo-human/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.923748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/alpaca-farm-ppo-sim-gpt4-20k/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.923748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/baize-v2-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/baize-v2-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/baize-v2-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.923748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/baize-v2-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/baize-v2-7b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.923748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/chatgpt/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/chatgpt/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.923748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/claude/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/claude/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/claude/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.923748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/cohere/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/cohere/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/cohere/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.923748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/cohere-chat/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/cohere-chat/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.923748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/falcon-40b-instruct/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/falcon-40b-instruct/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.923748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/falcon-7b-instruct/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/falcon-7b-instruct/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/gpt4/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/gpt4/chatml_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/gpt4/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/guanaco-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/guanaco-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/guanaco-33b/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/guanaco-33b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/guanaco-65b/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/guanaco-65b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/guanaco-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/guanaco-7b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/guanaco-7b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/minotaur-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/minotaur-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/minotaur-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/nous-hermes-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/nous-hermes-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/nous-hermes-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/oasst-rlhf-llama-33b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/oasst-sft-llama-33b/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/oasst-sft-llama-33b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/oasst-sft-llama-33b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/oasst-sft-pythia-12b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/openchat-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/openchat-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/openchat-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/openchat-v2-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/openchat-v2-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/openchat-v2-w-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/openchat-v2-w-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/openchat8192-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/openchat8192-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/opencoderplus-15b/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/opencoderplus-15b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/pythia-12b-mix-sft/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/pythia-12b-mix-sft/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/text_davinci_001/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/text_davinci_001/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/text_davinci_003/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/text_davinci_003/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/text_davinci_003/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/ultralm-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/ultralm-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/ultralm-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/vicuna-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/vicuna-13b/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/vicuna-13b-v1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/vicuna-13b-v1.3/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/vicuna-33b-v1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/vicuna-33b-v1.3/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/vicuna-7b/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/vicuna-7b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/vicuna-7b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.927748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/vicuna-7b-v1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/vicuna-7b-v1.3/configs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.931748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/wizardlm-13b/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/wizardlm-13b/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/wizardlm-13b/prompt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.931748 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/wizardlm-13b-v1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/models_configs/wizardlm-13b-v1.1/configs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20680 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/src/alpaca_eval/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.915748 alpaca_eval-0.2.1/src/alpaca_eval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    66370 2023-07-11 01:19:06.000000 alpaca_eval-0.2.1/src/alpaca_eval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-07-11 01:19:06.000000 alpaca_eval-0.2.1/src/alpaca_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 01:19:06.000000 alpaca_eval-0.2.1/src/alpaca_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-11 01:19:06.000000 alpaca_eval-0.2.1/src/alpaca_eval.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-11 01:19:06.000000 alpaca_eval-0.2.1/src/alpaca_eval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-11 01:19:06.000000 alpaca_eval-0.2.1/src/alpaca_eval.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 01:19:06.931748 alpaca_eval-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/tests/test_analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/tests/test_decoders_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-07-11 01:18:43.000000 alpaca_eval-0.2.1/tests/test_pairwise_evaluator.py
```

### Comparing `alpaca_eval-0.2.0/LICENSE` & `alpaca_eval-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/PKG-INFO` & `alpaca_eval-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaca_eval
-Version: 0.2.0
+Version: 0.2.1
 Summary: AlpacaEval : An Automatic Evaluator of Instruction-following Models
 Author: The Alpaca Team
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: alpaca_eval Version: 0.2.0 Summary: AlpacaEval : An
+Metadata-Version: 2.1 Name: alpaca_eval Version: 0.2.1 Summary: AlpacaEval : An
 Automatic Evaluator of Instruction-following Models Author: The Alpaca Team
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Education Classifier: Intended Audience :: Science/Research Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: Topic :: Scientific/Engineering :: Artificial
```

### Comparing `alpaca_eval-0.2.0/README.md` & `alpaca_eval-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/example/outputs.json` & `alpaca_eval-0.2.1/example/outputs.json`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/setup.py` & `alpaca_eval-0.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,18 +7,26 @@
 with open(os.path.join(here, "src", "alpaca_eval", "__init__.py")) as f:
     meta_match = re.search(r"^__version__ = ['\"]([^'\"]*)['\"]", f.read(), re.M)
     if meta_match:
         version = meta_match.group(1)
     else:
         raise RuntimeError("Unable to find `__version__`.")
 
-PACKAGES_DEV = ["pre-commit>=3.2.0", "black>=23.1.0", "isort", "pytest", "pytest-mock", "pytest-skip-slow"]
+PACKAGES_DEV = [
+    "pre-commit>=3.2.0",
+    "black>=23.1.0",
+    "isort",
+    "pytest",
+    "pytest-mock",
+    "pytest-skip-slow",
+    "python-dotenv",
+]
 PACKAGES_ANALYSIS = ["seaborn", "matplotlib", "jupyterlab"]
 PACKAGES_LOCAL = ["accelerate", "transformers", "bitsandbytes", "xformers", "peft", "optimum", "scipy", "einops"]
-PACKAGES_ALL_API = ["anthropic>=0.3.0", "huggingface_hub", "cohere"]
+PACKAGES_ALL_API = ["anthropic>=0.3.3", "huggingface_hub", "cohere"]
 PACKAGES_ALL = PACKAGES_LOCAL + PACKAGES_ALL_API + PACKAGES_ANALYSIS + PACKAGES_DEV
 
 setuptools.setup(
     name="alpaca_eval",
     version=version,
     description="AlpacaEval : An Automatic Evaluator of Instruction-following Models",
     package_dir={"": "src"},
```

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/analyze.py` & `alpaca_eval-0.2.1/src/alpaca_eval/analyze.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/annotators/pairwise_evaluator.py` & `alpaca_eval-0.2.1/src/alpaca_eval/annotators/pairwise_evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import os
 from functools import partial
 from pathlib import Path
-from typing import Any, Callable, Optional, Sequence, Union
+from typing import Any, Callable, Optional, Sequence, Type, Union
 
 import numpy as np
 import pandas as pd
 
 from .. import completion_parsers, constants, utils
 from ..decoders import get_fn_completions
 
@@ -128,23 +128,27 @@
         self.p_label_flip = p_label_flip
         self.is_store_missing_preferences = is_store_missing_preferences
         self.annotators_config = annotators_config
 
         self.annotators = self._initialize_annotators(annotators_config)
         self.caching_path = caching_path
         self.df_annotations = None
-        self.load_()
+        self.reinitialize_cache_()
 
     ### Helper properties to make it easier to inherit from this class ###
     @property
     def SingleAnnotator(self):
         return SinglePairwiseAnnotator
 
     #########################################
 
+    @property
+    def annotator_name(self) -> str:
+        return Path(self.annotators_config).parent.name
+
     def annotate_samples(
         self,
         all_outputs: utils.AnyData,
         keys_to_sample_output_2: Optional[Sequence] = None,
         is_unique_instructions: bool = True,
         p_label_flip: Optional[float] = None,
         is_multisample_list: bool = True,
@@ -379,16 +383,15 @@
                 seed="annotator" + x["instruction"] + str(self.seed),
                 choices=list(self.annotators.keys()),
             ),
             axis=1,
         )
 
         if self.is_avoid_reannotations:
-            # merge the old annotations
-            df_to_annotate = self._merge_annotations(df_to_annotate, self.df_annotations)
+            df_to_annotate = self.apply_cached_annotations(df_to_annotate)
 
         # adds random noise => avoids annotating examples that will be noised out.
         if self.p_label_flip:
             logging.info(f"Adding random noise to the labels p_label_flip={self.p_label_flip}.")
             # if you have 25% change of flipping the label, you have 50% chance of selecting random label
             p_noise = self.p_label_flip * 2
             noisy_preference = df_to_annotate.apply(
@@ -409,16 +412,21 @@
             )
 
         idcs_is_same_outputs = df_to_annotate["output_1"] == df_to_annotate["output_2"]
         df_to_annotate.loc[idcs_is_same_outputs, "preference"] = 0
 
         return df_to_annotate
 
+    def apply_cached_annotations(self, df_to_annotate: pd.DataFrame) -> pd.DataFrame:
+        """annotate examples with cached annotations"""
+        df_to_annotate = self._merge_annotations(df_to_annotate, self.df_annotations)
+        return df_to_annotate
+
     def _initialize_annotators(
-        self, annotators_config: Union[utils.AnyPath, dict[str, dict[str, Any]]]
+        self, annotators_config: Union[utils.AnyPath, dict[str, dict[str, Type["SinglePairwiseAnnotator"]]]]
     ) -> dict[str, Callable]:
         """Load all the configs and prompts if necessary."""
         annotators_config = utils.load_configs(annotators_config)
         return {
             name: self.SingleAnnotator(seed=self.seed, base_dir=self.base_dir, **annotator_config)
             for name, annotator_config in annotators_config.items()
         }
@@ -467,22 +475,15 @@
         else:
             df_annotated_to_store = df_annotated
 
         other_keys_to_keep = [c for c in self.other_keys_to_keep if c in df_annotated_to_store.columns]
         all_keys_to_keep = self.all_keys + ["preference"] + other_keys_to_keep
         df_annotated_to_store = df_annotated_to_store[all_keys_to_keep]
 
-        if self.df_annotations is None:
-            df_annotations = df_annotated_to_store
-        else:
-            df_annotations = pd.concat([self.df_annotations, df_annotated_to_store], axis=0, ignore_index=True)
-
-        self.df_annotations = df_annotations.drop_duplicates(subset=self.all_keys, keep="last")
-
-        self.save()
+        self.store_annotations_(df_annotated_to_store)
 
         if self.is_store_missing_preferences:
             # put back np.nan
             df_annotated["preference"] = df_annotated["preference"].replace(-1, np.nan)
 
         # need to merge with df_to_annotate in case you dropped duplicates
         on = list(self.input_keys + self.output_keys)
@@ -491,14 +492,25 @@
         # need to remove all other columns before merging if not you will
         df_annotated = df_to_annotate.merge(df_annotated, on=on, how="outer")
 
         annotated = df_annotated.to_dict(orient="records")
 
         return annotated
 
+    def store_annotations_(self, df_annotated_to_store: pd.DataFrame):
+        """Store annotation in memory and on disk"""
+        if self.df_annotations is None:
+            df_annotations = df_annotated_to_store
+        else:
+            df_annotations = pd.concat([self.df_annotations, df_annotated_to_store], axis=0, ignore_index=True)
+
+        self.df_annotations = df_annotations.drop_duplicates(subset=self.all_keys, keep="last")
+
+        self.save()
+
     def save(self, path: Optional[utils.AnyPath] = None):
         """Save the annotations to json."""
         path = path or self.caching_path
         if path is not None:
             logging.info(f"Saving all annotations to {path}.")
             # to make sure that we don't overwrite the annotations we load again from file (ideally would use a DB)
             self._refresh_annotations_()
@@ -510,44 +522,48 @@
         """Refresh the annotations in memory."""
         curr_df_annotations = self.df_annotations.copy()
         self.load_()
         self.df_annotations = pd.concat(
             [self.df_annotations, curr_df_annotations], axis=0, ignore_index=True
         ).drop_duplicates(subset=self.all_keys, keep="last")
 
+    def reinitialize_cache_(self):
+        self.load_()
+
     def load_(self, path: Optional[utils.AnyPath] = None):
         """Load all the annotations from json."""
         path = path or self.caching_path
         if path is not None:
             path = Path(path)
             if path.exists():
                 logging.info(f"Loading all annotations from {path}.")
                 self.df_annotations = pd.read_json(path, dtype={k: str for k in self.all_keys})
 
     def _merge_annotations(self, df_to_annotate: pd.DataFrame, df_partially_annotated: pd.DataFrame) -> pd.DataFrame:
         """Merge (partial) annotations with the original df to keep the same order and avoid duplicates annotations."""
+
         if df_partially_annotated is None or df_partially_annotated.empty:
             return df_to_annotate
 
         other_keys_to_keep = [c for c in self.other_keys_to_keep if c in df_partially_annotated.columns]
 
-        kwargrs = dict(
+        kwargs = dict(
             on=self.all_keys,
             how="left",
             suffixes=("_old", "_new"),
         )
         try:
             df_to_annotate = df_to_annotate.merge(
-                df_partially_annotated[self.all_keys + ["preference"] + other_keys_to_keep], **kwargrs
+                df_partially_annotated[self.all_keys + ["preference"] + other_keys_to_keep], **kwargs
             )
         except ValueError:
             # can have merging issues if columns have different dtypes
             df_partially_annotated = df_partially_annotated.astype({k: str for k in self.all_keys})
             df_to_annotate = df_to_annotate.astype({k: str for k in self.all_keys}).merge(
-                df_partially_annotated[self.all_keys + ["preference"] + other_keys_to_keep], **kwargrs
+                df_partially_annotated[self.all_keys + ["preference"] + other_keys_to_keep], **kwargs
             )
 
         # if columns were in both dataframes, try to merge them
         for c in other_keys_to_keep + ["preference"]:
             if f"{c}_old" in df_to_annotate.columns and f"{c}_new" in df_to_annotate.columns:
                 df_to_annotate[c] = df_to_annotate[c + "_old"].fillna(df_to_annotate[c + "_new"])
                 df_to_annotate = df_to_annotate.drop(columns=[c + "_old", c + "_new"])
```

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/completion_parsers.py` & `alpaca_eval-0.2.1/src/alpaca_eval/completion_parsers.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/constants.py` & `alpaca_eval-0.2.1/src/alpaca_eval/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,17 @@
     "guanaco-33b",
     "nous-hermes-13b",
     "oasst-sft-llama-33b",
     "oasst-sft-pythia-12b",
     "pythia-12b-mix-sft",
     "vicuna-7b",
     "wizardlm-13b",
+    "vicuna-7b-v1.3",
+    "vicuna-13b-v1.3",
+    "vicuna-33b-v1.3",
 )
 
 MINIMAL_EVALUATORS = (
     "alpaca_eval_gpt4",
     "aviary_gpt4",
     "gpt4",
     "claude",
```

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/decoders/__init__.py` & `alpaca_eval-0.2.1/src/alpaca_eval/decoders/__init__.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/decoders/anthropic.py` & `alpaca_eval-0.2.1/src/alpaca_eval/decoders/anthropic.py`

 * *Files 5% similar despite different names*

```diff
@@ -95,22 +95,25 @@
 
             if completion == "":
                 completion = " "  # annoying doesn't allow empty string
 
             break
 
         except anthropic.RateLimitError as e:
-            logging.warning(f"APIError: {e}.")
+            logging.warning(f"API RateLimitError: {e}.")
             if len(anthropic_api_keys) > 1:
                 anthropic_api_key = random.choice(anthropic_api_keys)
                 client = anthropic.Anthropic(api_key=anthropic_api_key, max_retries=n_retries)
                 logging.info(f"Switching anthropic API key.")
             logging.warning(f"Rate limit hit. Sleeping for {sleep_time} seconds.")
             time.sleep(sleep_time)
 
+        except anthropic.APITimeoutError as e:
+            logging.warning(f"API TimeoutError: {e}. Retrying request.")
+
     return completion
 
 
 def _get_price_per_token(model):
     """Returns the price per token for a given model"""
     # https://cdn2.assets-servd.host/anthropic-website/production/images/model_pricing_may2023.pdf
     if "claude-v1" in model:
```

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/decoders/cohere.py` & `alpaca_eval-0.2.1/src/alpaca_eval/decoders/cohere.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/decoders/huggingface_api.py` & `alpaca_eval-0.2.1/src/alpaca_eval/decoders/huggingface_api.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/decoders/huggingface_local.py` & `alpaca_eval-0.2.1/src/alpaca_eval/decoders/huggingface_local.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/decoders/openai.py` & `alpaca_eval-0.2.1/src/alpaca_eval/decoders/openai.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/README.md` & `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/README.md`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt` & `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4/alpaca_eval.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt` & `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/alpaca_eval_fn.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml` & `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_eval_gpt4_fn/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt` & `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_v0_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt` & `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_chat_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt` & `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_cot_json_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt` & `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b1_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt` & `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b4_cot_json_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt` & `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_diana_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt` & `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_joe_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt` & `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/chatml_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml` & `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt` & `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_v0_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt` & `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b1_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt` & `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b4_reasoning_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt` & `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm/text_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt` & `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/alpaca_farm_greedy_gpt4/chatml_b5_without_inputs.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt` & `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/aviary_gpt4/aviary_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt` & `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/chatgpt/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt` & `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/chatgpt_fn/basic_function_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml` & `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/chatgpt_fn/configs.yaml`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt` & `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/claude/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt` & `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/claude_ranking/ranking_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt` & `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/guanaco_33b/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt` & `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/lmsys_gpt4/lmsys_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt` & `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/oasst_pythia_12b/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt` & `alpaca_eval-0.2.1/src/alpaca_eval/evaluators_configs/text_davinci_003/basic_prompt.txt`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv` & `alpaca_eval-0.2.1/src/alpaca_eval/leaderboards/data_AlpacaEval/alpaca_eval_gpt4_leaderboard.csv`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 ,win_rate,standard_error,mode,n_draws,n_total,n_wins,n_wins_base
 gpt4,95.27950310559004,0.716281440286153,minimal,12,805,761,32
+vicuna-33b-v1.3,88.99253731343283,1.095692216068168,verified,5,804,713,86
 claude,88.38509316770187,1.1144875403283188,minimal,9,805,707,89
-openchat-v2-w-13b,87.1268656716418,1.1769197439396017,community,3,804,699,102
+openchat-v2-w-13b,87.1268656716418,1.1769197439396015,community,3,804,699,102
+wizardlm-13b-v1.1,86.31840796019901,1.2063217831272972,community,4,804,692,108
 chatgpt,86.08695652173914,1.2110077772660273,minimal,6,805,690,109
 openchat-v2-13b,84.96894409937889,1.2572979835605944,community,2,805,683,120
+vicuna-13b-v1.3,82.11180124223603,1.348769957803504,verified,2,805,660,143
 openchat-13b,80.8695652173913,1.3843738653129234,community,2,805,650,153
 ultralm-13b,80.63511830635119,1.3939556917204066,community,1,803,647,155
 openchat8192-13b,79.53980099502488,1.4222439886269744,community,1,804,639,164
 opencoderplus-15b,78.69565217391305,1.440029529188432,community,3,805,632,170
+vicuna-7b-v1.3,76.8414481897628,1.487520320531845,verified,3,801,614,184
 wizardlm-13b,75.31094527363184,1.5101858292160824,minimal,9,804,601,194
 airoboros-65b,73.91304347826086,1.5285333061227804,verified,16,805,587,202
 airoboros-33b,73.29192546583852,1.55290318216736,verified,6,805,587,212
 guanaco-65b,71.80124223602485,1.586912361158523,minimal,0,805,578,227
 vicuna-13b,70.43478260869566,1.6069688407799696,minimal,2,805,566,237
 baize-v2-13b,66.95652173913044,1.6565358231309506,community,2,805,538,265
 oasst-rlhf-llama-33b,66.52173913043478,1.6608288428292477,minimal,3,805,534,268
```

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv` & `alpaca_eval-0.2.1/src/alpaca_eval/leaderboards/data_AlpacaEval/chatgpt_fn_leaderboard.csv`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv` & `alpaca_eval-0.2.1/src/alpaca_eval/leaderboards/data_AlpacaEval/claude_leaderboard.csv`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 ,win_rate,standard_error,mode,n_draws,n_total,n_wins,n_wins_base
 gpt4,77.01863354037268,1.46803688292698,minimal,12,805,614,179
 claude,75.83850931677019,1.4981004247868313,minimal,9,805,606,190
+vicuna-33b-v1.3,72.36024844720497,1.5710737760483915,verified,5,805,580,220
 chatgpt,67.70186335403726,1.642111587090117,minimal,6,805,542,257
+vicuna-13b-v1.3,66.2111801242236,1.6657907370589309,verified,2,805,532,271
 wizardlm-13b,66.14906832298136,1.6584088766540706,minimal,9,805,528,268
 vicuna-13b,63.22981366459627,1.698243477332765,minimal,2,805,508,295
 guanaco-65b,62.60869565217392,1.7063755171155923,minimal,0,805,504,301
+vicuna-7b-v1.3,62.54658385093168,1.7035470981976453,verified,3,805,502,300
 nous-hermes-13b,60.86956521739131,1.7144465955143962,verified,6,805,487,312
 guanaco-33b,57.88819875776397,1.7412811662531051,verified,0,805,466,339
 vicuna-7b,57.329192546583855,1.7409917994657298,verified,3,805,460,342
 oasst-rlhf-llama-33b,57.329192546583855,1.7409917994657302,minimal,3,805,460,342
 guanaco-13b,53.36239103362392,1.7582560332920765,verified,3,803,427,373
 oasst-sft-llama-33b,51.24223602484472,1.748518981999294,verified,13,805,406,386
 text_davinci_003,50.0,0.0,minimal,805,805,0,0
```

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv` & `alpaca_eval-0.2.1/src/alpaca_eval/leaderboards/evaluators/evaluators_leaderboard.csv`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/main.py` & `alpaca_eval-0.2.1/src/alpaca_eval/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 from . import analyze, annotators, constants, decoders, metrics, utils
 from .types import AnyData, AnyPath
 
 CUR_DIR = Path(__file__).parent
 DEFAULT_CONFIGS = "alpaca_eval_gpt4"
 
+__all__ = ["evaluate", "evaluate_from_model", "analyze_evaluators", "make_leaderboard"]
+
 
 def evaluate(
     model_outputs: Optional[Union[AnyPath, AnyData, Callable]] = None,
     reference_outputs: Union[AnyPath, AnyData, Callable] = constants.ALPACAEVAL_REFERENCE_OUTPUTS,
     annotators_config: AnyPath = DEFAULT_CONFIGS,
     name: Optional[str] = None,
     output_path: Optional[Union[AnyPath, str]] = "auto",
@@ -25,14 +27,15 @@
     current_leaderboard_mode: str = "community",
     is_return_instead_of_print: bool = False,
     fn_metric: Union[str, callable] = "pairwise_to_winrate",
     sort_by: str = "win_rate",
     is_cache_leaderboard: Optional[bool] = None,
     max_instances: Optional[int] = None,
     annotation_kwargs: Optional[dict[str, Any]] = None,
+    Annotator=annotators.PairwiseAnnotator,
     **annotator_kwargs,
 ):
     """Evaluate a model based on its outputs. This is the default entrypoint if no command is specified.
 
     Parameters
     ----------
     model_outputs : path or data or dict
@@ -90,14 +93,17 @@
 
     max_instances : int, optional
         The maximum number of instances to annotate. Useful for testing.
 
     annotation_kwargs : dict, optional
         Additional arguments to pass to `PairwiseAnnotator.annotate_head2head`.
 
+    Annotator : class, optional
+        The annotator class to use.
+
     annotator_kwargs :
         Additional arguments to pass to `PairwiseAnnotator`.
     """
     if (
         isinstance(current_leaderboard_mode, str)
         and current_leaderboard_mode not in constants.ORDERED_LEADERBOARD_MODES
     ):
@@ -118,15 +124,15 @@
         if (name not in leaderboard) or is_overwrite_leaderboard:
             logging.info(f"Evaluating the {name} outputs.")
 
             if max_instances is not None:
                 model_outputs = model_outputs[:max_instances]
                 reference_outputs = reference_outputs[:max_instances]
 
-            annotator = annotators.PairwiseAnnotator(annotators_config=annotators_config, **annotator_kwargs)
+            annotator = Annotator(annotators_config=annotators_config, **annotator_kwargs)
             annotations = annotator.annotate_head2head(
                 outputs_1=reference_outputs, outputs_2=model_outputs, **annotation_kwargs
             )
 
             if isinstance(fn_metric, str):
                 fn_metric = getattr(metrics, fn_metric)
```

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/metrics.py` & `alpaca_eval-0.2.1/src/alpaca_eval/metrics.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/plotting.py` & `alpaca_eval-0.2.1/src/alpaca_eval/plotting.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval/utils.py` & `alpaca_eval-0.2.1/src/alpaca_eval/utils.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval.egg-info/PKG-INFO` & `alpaca_eval-0.2.1/src/alpaca_eval.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaca-eval
-Version: 0.2.0
+Version: 0.2.1
 Summary: AlpacaEval : An Automatic Evaluator of Instruction-following Models
 Author: The Alpaca Team
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: alpaca-eval Version: 0.2.0 Summary: AlpacaEval : An
+Metadata-Version: 2.1 Name: alpaca-eval Version: 0.2.1 Summary: AlpacaEval : An
 Automatic Evaluator of Instruction-following Models Author: The Alpaca Team
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Education Classifier: Intended Audience :: Science/Research Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: Topic :: Scientific/Engineering :: Artificial
```

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval.egg-info/SOURCES.txt` & `alpaca_eval-0.2.1/src/alpaca_eval.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -117,16 +117,19 @@
 src/alpaca_eval/models_configs/pythia-12b-mix-sft/configs.yaml
 src/alpaca_eval/models_configs/text_davinci_001/configs.yaml
 src/alpaca_eval/models_configs/text_davinci_003/configs.yaml
 src/alpaca_eval/models_configs/text_davinci_003/prompt.txt
 src/alpaca_eval/models_configs/ultralm-13b/configs.yaml
 src/alpaca_eval/models_configs/ultralm-13b/prompt.txt
 src/alpaca_eval/models_configs/vicuna-13b/configs.yaml
-src/alpaca_eval/models_configs/vicuna-13b/prompt.txt
+src/alpaca_eval/models_configs/vicuna-13b-v1.3/configs.yaml
+src/alpaca_eval/models_configs/vicuna-33b-v1.3/configs.yaml
 src/alpaca_eval/models_configs/vicuna-7b/configs.yaml
 src/alpaca_eval/models_configs/vicuna-7b/prompt.txt
+src/alpaca_eval/models_configs/vicuna-7b-v1.3/configs.yaml
 src/alpaca_eval/models_configs/wizardlm-13b/configs.yaml
 src/alpaca_eval/models_configs/wizardlm-13b/prompt.txt
+src/alpaca_eval/models_configs/wizardlm-13b-v1.1/configs.yaml
 tests/test_analyze.py
 tests/test_decoders_unit.py
 tests/test_main.py
 tests/test_pairwise_evaluator.py
```

### Comparing `alpaca_eval-0.2.0/src/alpaca_eval.egg-info/requires.txt` & `alpaca_eval-0.2.1/src/alpaca_eval.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -9,44 +9,46 @@
 transformers
 bitsandbytes
 xformers
 peft
 optimum
 scipy
 einops
-anthropic>=0.3.0
+anthropic>=0.3.3
 huggingface_hub
 cohere
 seaborn
 matplotlib
 jupyterlab
 pre-commit>=3.2.0
 black>=23.1.0
 isort
 pytest
 pytest-mock
 pytest-skip-slow
+python-dotenv
 
 [analysis]
 seaborn
 matplotlib
 jupyterlab
 
 [api]
-anthropic>=0.3.0
+anthropic>=0.3.3
 huggingface_hub
 cohere
 
 [dev]
 pre-commit>=3.2.0
 black>=23.1.0
 isort
 pytest
 pytest-mock
 pytest-skip-slow
+python-dotenv
 
 [local]
 accelerate
 transformers
 bitsandbytes
 xformers
 peft
```

### Comparing `alpaca_eval-0.2.0/tests/test_analyze.py` & `alpaca_eval-0.2.1/tests/test_analyze.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/tests/test_decoders_unit.py` & `alpaca_eval-0.2.1/tests/test_decoders_unit.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/tests/test_main.py` & `alpaca_eval-0.2.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `alpaca_eval-0.2.0/tests/test_pairwise_evaluator.py` & `alpaca_eval-0.2.1/tests/test_pairwise_evaluator.py`

 * *Files identical despite different names*

