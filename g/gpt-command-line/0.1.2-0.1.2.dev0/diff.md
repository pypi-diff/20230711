# Comparing `tmp/gpt-command-line-0.1.2.tar.gz` & `tmp/gpt-command-line-0.1.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-command-line-0.1.2.tar", last modified: Tue Jul 11 03:11:53 2023, max compression
+gzip compressed data, was "gpt-command-line-0.1.2.dev0.tar", last modified: Sun Jul  9 20:41:39 2023, max compression
```

## Comparing `gpt-command-line-0.1.2.tar` & `gpt-command-line-0.1.2.dev0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:11:53.730771 gpt-command-line-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-11 03:11:42.000000 gpt-command-line-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10089 2023-07-11 03:11:53.730771 gpt-command-line-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8133 2023-07-11 03:11:42.000000 gpt-command-line-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:11:53.726771 gpt-command-line-0.1.2/gpt_command_line.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10089 2023-07-11 03:11:53.000000 gpt-command-line-0.1.2/gpt_command_line.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-11 03:11:53.000000 gpt-command-line-0.1.2/gpt_command_line.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 03:11:53.000000 gpt-command-line-0.1.2/gpt_command_line.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-11 03:11:53.000000 gpt-command-line-0.1.2/gpt_command_line.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-11 03:11:53.000000 gpt-command-line-0.1.2/gpt_command_line.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-11 03:11:53.000000 gpt-command-line-0.1.2/gpt_command_line.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:11:53.730771 gpt-command-line-0.1.2/gptcli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 03:11:42.000000 gpt-command-line-0.1.2/gptcli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-11 03:11:42.000000 gpt-command-line-0.1.2/gptcli/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-07-11 03:11:42.000000 gpt-command-line-0.1.2/gptcli/assistant.py
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-07-11 03:11:42.000000 gpt-command-line-0.1.2/gptcli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-11 03:11:42.000000 gpt-command-line-0.1.2/gptcli/completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-07-11 03:11:42.000000 gpt-command-line-0.1.2/gptcli/composite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-11 03:11:42.000000 gpt-command-line-0.1.2/gptcli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-07-11 03:11:42.000000 gpt-command-line-0.1.2/gptcli/cost.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-11 03:11:42.000000 gpt-command-line-0.1.2/gptcli/google.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7802 2023-07-11 03:11:42.000000 gpt-command-line-0.1.2/gptcli/gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-07-11 03:11:42.000000 gpt-command-line-0.1.2/gptcli/llama.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-11 03:11:42.000000 gpt-command-line-0.1.2/gptcli/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-11 03:11:42.000000 gpt-command-line-0.1.2/gptcli/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)     5642 2023-07-11 03:11:42.000000 gpt-command-line-0.1.2/gptcli/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-11 03:11:42.000000 gpt-command-line-0.1.2/gptcli/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-11 03:11:42.000000 gpt-command-line-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 03:11:53.730771 gpt-command-line-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 03:11:53.730771 gpt-command-line-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-11 03:11:42.000000 gpt-command-line-0.1.2/tests/test_assistant.py
--rw-r--r--   0 runner    (1001) docker     (123)     9112 2023-07-11 03:11:42.000000 gpt-command-line-0.1.2/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-11 03:11:42.000000 gpt-command-line-0.1.2/tests/test_term_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:41:39.726502 gpt-command-line-0.1.2.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10125 2023-07-09 20:41:39.726502 gpt-command-line-0.1.2.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:41:39.722502 gpt-command-line-0.1.2.dev0/gpt_command_line.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10125 2023-07-09 20:41:39.000000 gpt-command-line-0.1.2.dev0/gpt_command_line.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-09 20:41:39.000000 gpt-command-line-0.1.2.dev0/gpt_command_line.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 20:41:39.000000 gpt-command-line-0.1.2.dev0/gpt_command_line.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-09 20:41:39.000000 gpt-command-line-0.1.2.dev0/gpt_command_line.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-09 20:41:39.000000 gpt-command-line-0.1.2.dev0/gpt_command_line.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-09 20:41:39.000000 gpt-command-line-0.1.2.dev0/gpt_command_line.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:41:39.726502 gpt-command-line-0.1.2.dev0/gptcli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/gptcli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/gptcli/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/gptcli/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/gptcli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/gptcli/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/gptcli/composite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/gptcli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/gptcli/cost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/gptcli/google.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7802 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/gptcli/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/gptcli/llama.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/gptcli/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/gptcli/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/gptcli/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/gptcli/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 20:41:39.726502 gpt-command-line-0.1.2.dev0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 20:41:39.726502 gpt-command-line-0.1.2.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/tests/test_assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-09 20:41:26.000000 gpt-command-line-0.1.2.dev0/tests/test_term_utils.py
```

### Comparing `gpt-command-line-0.1.2/LICENSE` & `gpt-command-line-0.1.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.2/PKG-INFO` & `gpt-command-line-0.1.2.dev0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-command-line
-Version: 0.1.2
+Version: 0.1.2.dev0
 Summary: Command-line interface for ChatGPT, Claude and Bard
 Author-email: Val Kharitonov <val@kharvd.com>
 License: Copyright (c) 2023 by Val Kharitonov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -81,15 +81,15 @@
 You can also use a `gpt.yml` file for configuration. See the [Configuration](README.md#Configuration) section below.
 
 ## Usage
 
 Make sure to set the `OPENAI_API_KEY` environment variable to your OpenAI API key (or put it in the `~/.config/gpt-cli/gpt.yml` file as described below).
 
 ```
-usage: gpt [-h] [--no_markdown] [--model MODEL] [--temperature TEMPERATURE] [--top_p TOP_P]
+usage: gpt.py [-h] [--no_markdown] [--model MODEL] [--temperature TEMPERATURE] [--top_p TOP_P]
               [--log_file LOG_FILE] [--log_level {DEBUG,INFO,WARNING,ERROR,CRITICAL}]
               [--prompt PROMPT] [--execute EXECUTE] [--no_stream]
               [{dev,general,bash}]
 
 Run a chat session with ChatGPT. See https://github.com/kharvd/gpt-cli for more information.
 
 positional arguments:
@@ -123,34 +123,34 @@
                         Use `-` to read the prompt from standard input.
   --no_stream           If specified, will not stream the response to standard output. This is
                         useful if you want to use the response in a script. Ignored when the
                         --prompt option is not specified.
   --no_price            Disable price logging.
 ```
 
-Type `:q` or Ctrl-D to exit, `:c` or Ctrl-C to clear the conversation, `:r` or Ctrl-R to re-generate the last response.
+Type `q` or Ctrl-D to exit, `c` or Ctrl-C to clear the conversation, `r` or Ctrl-R to re-generate the last response.
 To enter multi-line mode, enter a backslash `\` followed by a new line. Exit the multi-line mode by pressing ESC and then Enter.
 
 You can override the model parameters using `--model`, `--temperature` and `--top_p` arguments at the end of your prompt. For example:
 
 ```
 > What is the meaning of life? --model gpt-4 --temperature 2.0
 The meaning of life is subjective and can be different for diverse human beings and unique-phil ethics.org/cultuties-/ it that reson/bdstals89im3_jrf334;mvs-bread99ef=g22me
 ```
 
 The `dev` assistant is instructed to be an expert in software development and provide short responses.
 
 ```bash
-$ gpt dev
+$ ./gpt.py dev
 ```
 
 The `bash` assistant is instructed to be an expert in bash scripting and provide only bash commands. Use the `--execute` option to execute the commands. It works best with the `gpt-4` model.
 
 ```bash
-gpt bash -e "How do I list files in a directory?"
+./gpt.py bash -e "How do I list files in a directory?"
 ```
 
 This will prompt you to edit the command in your `$EDITOR` it before executing it.
 
 ## Configuration
 
 You can configure the assistants in the config file `~/.config/gpt-cli/gpt.yml`. The file is a YAML file with the following structure (see also [config.py](./gptcli/config.py))
@@ -189,15 +189,15 @@
     model: gpt-4
     temperature: 1.0
     messages:
       - { role: system, content: "You are a pirate." }
 ```
 
 ```
-$ gpt pirate
+$ ./gpt.py pirate
 
 > Arrrr
 Ahoy, matey! What be bringing ye to these here waters? Be it treasure or adventure ye seek, we be sailing the high seas together. Ready yer map and compass, for we have a long voyage ahead!
 ```
 
 ## Other chat bots
 
@@ -211,28 +211,28 @@
 
 or a config line in `~/.config/gpt-cli/gpt.yml`:
 
 ```yaml
 anthropic_api_key: <your_key_here>
 ```
 
-Now you should be able to run `gpt` with `--model claude-v1` or `--model claude-instant-v1`:
+Now you should be able to run `gpt.py` with `--model claude-v1` or `--model claude-instant-v1`:
 
 ```bash
-gpt --model claude-v1
+./gpt.py --model claude-v1
 ```
 
 ### Google Bard (PaLM 2)
 Similar to Claude, set the Google API key
 
 ```bash
 export GOOGLE_API_KEY=<your_key_here>
 ```
 or a config line:
 ```yaml
 google_api_key: <your_key_here>
 ```
 
-Run `gpt` with the correct model:
+Run `gpt.py` with the correct model:
 ```bash
-gpt --model chat-bison-001
+./gpt.py --model chat-bison-001
 ```
```

### Comparing `gpt-command-line-0.1.2/README.md` & `gpt-command-line-0.1.2.dev0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 You can also use a `gpt.yml` file for configuration. See the [Configuration](README.md#Configuration) section below.
 
 ## Usage
 
 Make sure to set the `OPENAI_API_KEY` environment variable to your OpenAI API key (or put it in the `~/.config/gpt-cli/gpt.yml` file as described below).
 
 ```
-usage: gpt [-h] [--no_markdown] [--model MODEL] [--temperature TEMPERATURE] [--top_p TOP_P]
+usage: gpt.py [-h] [--no_markdown] [--model MODEL] [--temperature TEMPERATURE] [--top_p TOP_P]
               [--log_file LOG_FILE] [--log_level {DEBUG,INFO,WARNING,ERROR,CRITICAL}]
               [--prompt PROMPT] [--execute EXECUTE] [--no_stream]
               [{dev,general,bash}]
 
 Run a chat session with ChatGPT. See https://github.com/kharvd/gpt-cli for more information.
 
 positional arguments:
@@ -96,34 +96,34 @@
                         Use `-` to read the prompt from standard input.
   --no_stream           If specified, will not stream the response to standard output. This is
                         useful if you want to use the response in a script. Ignored when the
                         --prompt option is not specified.
   --no_price            Disable price logging.
 ```
 
-Type `:q` or Ctrl-D to exit, `:c` or Ctrl-C to clear the conversation, `:r` or Ctrl-R to re-generate the last response.
+Type `q` or Ctrl-D to exit, `c` or Ctrl-C to clear the conversation, `r` or Ctrl-R to re-generate the last response.
 To enter multi-line mode, enter a backslash `\` followed by a new line. Exit the multi-line mode by pressing ESC and then Enter.
 
 You can override the model parameters using `--model`, `--temperature` and `--top_p` arguments at the end of your prompt. For example:
 
 ```
 > What is the meaning of life? --model gpt-4 --temperature 2.0
 The meaning of life is subjective and can be different for diverse human beings and unique-phil ethics.org/cultuties-/ it that reson/bdstals89im3_jrf334;mvs-bread99ef=g22me
 ```
 
 The `dev` assistant is instructed to be an expert in software development and provide short responses.
 
 ```bash
-$ gpt dev
+$ ./gpt.py dev
 ```
 
 The `bash` assistant is instructed to be an expert in bash scripting and provide only bash commands. Use the `--execute` option to execute the commands. It works best with the `gpt-4` model.
 
 ```bash
-gpt bash -e "How do I list files in a directory?"
+./gpt.py bash -e "How do I list files in a directory?"
 ```
 
 This will prompt you to edit the command in your `$EDITOR` it before executing it.
 
 ## Configuration
 
 You can configure the assistants in the config file `~/.config/gpt-cli/gpt.yml`. The file is a YAML file with the following structure (see also [config.py](./gptcli/config.py))
@@ -162,15 +162,15 @@
     model: gpt-4
     temperature: 1.0
     messages:
       - { role: system, content: "You are a pirate." }
 ```
 
 ```
-$ gpt pirate
+$ ./gpt.py pirate
 
 > Arrrr
 Ahoy, matey! What be bringing ye to these here waters? Be it treasure or adventure ye seek, we be sailing the high seas together. Ready yer map and compass, for we have a long voyage ahead!
 ```
 
 ## Other chat bots
 
@@ -184,28 +184,28 @@
 
 or a config line in `~/.config/gpt-cli/gpt.yml`:
 
 ```yaml
 anthropic_api_key: <your_key_here>
 ```
 
-Now you should be able to run `gpt` with `--model claude-v1` or `--model claude-instant-v1`:
+Now you should be able to run `gpt.py` with `--model claude-v1` or `--model claude-instant-v1`:
 
 ```bash
-gpt --model claude-v1
+./gpt.py --model claude-v1
 ```
 
 ### Google Bard (PaLM 2)
 Similar to Claude, set the Google API key
 
 ```bash
 export GOOGLE_API_KEY=<your_key_here>
 ```
 or a config line:
 ```yaml
 google_api_key: <your_key_here>
 ```
 
-Run `gpt` with the correct model:
+Run `gpt.py` with the correct model:
 ```bash
-gpt --model chat-bison-001
+./gpt.py --model chat-bison-001
 ```
```

### Comparing `gpt-command-line-0.1.2/gpt_command_line.egg-info/PKG-INFO` & `gpt-command-line-0.1.2.dev0/gpt_command_line.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-command-line
-Version: 0.1.2
+Version: 0.1.2.dev0
 Summary: Command-line interface for ChatGPT, Claude and Bard
 Author-email: Val Kharitonov <val@kharvd.com>
 License: Copyright (c) 2023 by Val Kharitonov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -81,15 +81,15 @@
 You can also use a `gpt.yml` file for configuration. See the [Configuration](README.md#Configuration) section below.
 
 ## Usage
 
 Make sure to set the `OPENAI_API_KEY` environment variable to your OpenAI API key (or put it in the `~/.config/gpt-cli/gpt.yml` file as described below).
 
 ```
-usage: gpt [-h] [--no_markdown] [--model MODEL] [--temperature TEMPERATURE] [--top_p TOP_P]
+usage: gpt.py [-h] [--no_markdown] [--model MODEL] [--temperature TEMPERATURE] [--top_p TOP_P]
               [--log_file LOG_FILE] [--log_level {DEBUG,INFO,WARNING,ERROR,CRITICAL}]
               [--prompt PROMPT] [--execute EXECUTE] [--no_stream]
               [{dev,general,bash}]
 
 Run a chat session with ChatGPT. See https://github.com/kharvd/gpt-cli for more information.
 
 positional arguments:
@@ -123,34 +123,34 @@
                         Use `-` to read the prompt from standard input.
   --no_stream           If specified, will not stream the response to standard output. This is
                         useful if you want to use the response in a script. Ignored when the
                         --prompt option is not specified.
   --no_price            Disable price logging.
 ```
 
-Type `:q` or Ctrl-D to exit, `:c` or Ctrl-C to clear the conversation, `:r` or Ctrl-R to re-generate the last response.
+Type `q` or Ctrl-D to exit, `c` or Ctrl-C to clear the conversation, `r` or Ctrl-R to re-generate the last response.
 To enter multi-line mode, enter a backslash `\` followed by a new line. Exit the multi-line mode by pressing ESC and then Enter.
 
 You can override the model parameters using `--model`, `--temperature` and `--top_p` arguments at the end of your prompt. For example:
 
 ```
 > What is the meaning of life? --model gpt-4 --temperature 2.0
 The meaning of life is subjective and can be different for diverse human beings and unique-phil ethics.org/cultuties-/ it that reson/bdstals89im3_jrf334;mvs-bread99ef=g22me
 ```
 
 The `dev` assistant is instructed to be an expert in software development and provide short responses.
 
 ```bash
-$ gpt dev
+$ ./gpt.py dev
 ```
 
 The `bash` assistant is instructed to be an expert in bash scripting and provide only bash commands. Use the `--execute` option to execute the commands. It works best with the `gpt-4` model.
 
 ```bash
-gpt bash -e "How do I list files in a directory?"
+./gpt.py bash -e "How do I list files in a directory?"
 ```
 
 This will prompt you to edit the command in your `$EDITOR` it before executing it.
 
 ## Configuration
 
 You can configure the assistants in the config file `~/.config/gpt-cli/gpt.yml`. The file is a YAML file with the following structure (see also [config.py](./gptcli/config.py))
@@ -189,15 +189,15 @@
     model: gpt-4
     temperature: 1.0
     messages:
       - { role: system, content: "You are a pirate." }
 ```
 
 ```
-$ gpt pirate
+$ ./gpt.py pirate
 
 > Arrrr
 Ahoy, matey! What be bringing ye to these here waters? Be it treasure or adventure ye seek, we be sailing the high seas together. Ready yer map and compass, for we have a long voyage ahead!
 ```
 
 ## Other chat bots
 
@@ -211,28 +211,28 @@
 
 or a config line in `~/.config/gpt-cli/gpt.yml`:
 
 ```yaml
 anthropic_api_key: <your_key_here>
 ```
 
-Now you should be able to run `gpt` with `--model claude-v1` or `--model claude-instant-v1`:
+Now you should be able to run `gpt.py` with `--model claude-v1` or `--model claude-instant-v1`:
 
 ```bash
-gpt --model claude-v1
+./gpt.py --model claude-v1
 ```
 
 ### Google Bard (PaLM 2)
 Similar to Claude, set the Google API key
 
 ```bash
 export GOOGLE_API_KEY=<your_key_here>
 ```
 or a config line:
 ```yaml
 google_api_key: <your_key_here>
 ```
 
-Run `gpt` with the correct model:
+Run `gpt.py` with the correct model:
 ```bash
-gpt --model chat-bison-001
+./gpt.py --model chat-bison-001
 ```
```

### Comparing `gpt-command-line-0.1.2/gpt_command_line.egg-info/SOURCES.txt` & `gpt-command-line-0.1.2.dev0/gpt_command_line.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.2/gptcli/anthropic.py` & `gpt-command-line-0.1.2.dev0/gptcli/anthropic.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.2/gptcli/assistant.py` & `gpt-command-line-0.1.2.dev0/gptcli/assistant.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.2/gptcli/cli.py` & `gpt-command-line-0.1.2.dev0/gptcli/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import re
 from prompt_toolkit import PromptSession
 from prompt_toolkit.history import FileHistory
 from openai import OpenAIError, InvalidRequestError
 from prompt_toolkit.key_binding import KeyBindings, KeyPressEvent
-from prompt_toolkit.key_binding.bindings import named_commands
 from rich.console import Console
 from rich.live import Live
 from rich.markdown import Markdown
 from typing import Any, Dict, Optional, Tuple
 
 from rich.text import Text
 from gptcli.session import (
@@ -19,19 +18,18 @@
     InvalidArgumentError,
     ResponseStreamer,
     UserInputProvider,
 )
 
 
 TERMINAL_WELCOME = """
-Hi! I'm here to help. Type `:q` or Ctrl-D to exit, `:c` or Ctrl-C and Enter to clear
-the conversation, `:r` or Ctrl-R to re-generate the last response.
+Hi! I'm here to help. Type `q` or Ctrl-D to exit, `c` or Ctrl-C to clear
+the conversation, `r` or Ctrl-R to re-generate the last response.
 To enter multi-line mode, enter a backslash `\\` followed by a new line.
 Exit the multi-line mode by pressing ESC and then Enter (Meta+Enter).
-Try `:?` for help.
 """
 
 
 class StreamingMarkdownPrinter:
     def __init__(self, console: Console, markdown: bool):
         self.console = console
         self.current_text = ""
@@ -150,26 +148,19 @@
 
         user_input, args = self._parse_input(next_user_input)
         return user_input, args
 
     def prompt(self, multiline=False):
         bindings = KeyBindings()
 
-        bindings.add("c-a")(named_commands.get_by_name("beginning-of-line"))
-        bindings.add("c-b")(named_commands.get_by_name("backward-char"))
-        bindings.add("c-e")(named_commands.get_by_name("end-of-line"))
-        bindings.add("c-f")(named_commands.get_by_name("forward-char"))
-        bindings.add("c-left")(named_commands.get_by_name("backward-word"))
-        bindings.add("c-right")(named_commands.get_by_name("forward-word"))
-
         @bindings.add("c-c")
         def _(event: KeyPressEvent):
             if len(event.current_buffer.text) == 0 and not multiline:
                 event.current_buffer.text = COMMAND_CLEAR[0]
-                event.current_buffer.cursor_right(len(COMMAND_CLEAR[0]))
+                event.current_buffer.validate_and_handle()
             else:
                 event.app.exit(exception=KeyboardInterrupt, style="class:aborting")
 
         @bindings.add("c-d")
         def _(event: KeyPressEvent):
             if len(event.current_buffer.text) == 0:
                 if not multiline:
```

### Comparing `gpt-command-line-0.1.2/gptcli/composite.py` & `gpt-command-line-0.1.2.dev0/gptcli/composite.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.2/gptcli/config.py` & `gpt-command-line-0.1.2.dev0/gptcli/config.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.2/gptcli/cost.py` & `gpt-command-line-0.1.2.dev0/gptcli/cost.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.2/gptcli/google.py` & `gpt-command-line-0.1.2.dev0/gptcli/google.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.2/gptcli/gpt.py` & `gpt-command-line-0.1.2.dev0/gptcli/gpt.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.2/gptcli/llama.py` & `gpt-command-line-0.1.2.dev0/gptcli/llama.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.2/gptcli/logging.py` & `gpt-command-line-0.1.2.dev0/gptcli/logging.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.2/gptcli/openai.py` & `gpt-command-line-0.1.2.dev0/gptcli/openai.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.2/gptcli/session.py` & `gpt-command-line-0.1.2.dev0/gptcli/session.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,26 +49,18 @@
 
 
 class InvalidArgumentError(Exception):
     def __init__(self, message: str):
         self.message = message
 
 
-COMMAND_CLEAR = (":clear", ":c")
-COMMAND_QUIT = (":quit", ":q")
-COMMAND_RERUN = (":rerun", ":r")
-COMMAND_HELP = (":help", ":h", ":?")
-ALL_COMMANDS = [*COMMAND_CLEAR, *COMMAND_QUIT, *COMMAND_RERUN, *COMMAND_HELP]
-COMMANDS_HELP = """
-Commands:
-- `:clear` / `:c` / Ctrl+C - Clear the conversation.
-- `:quit` / `:q` / Ctrl+D - Quit the program.
-- `:rerun` / `:r` / Ctrl+R - Re-run the last message.
-- `:help` / `:h` / `:?` - Show this help message.
-"""
+COMMAND_CLEAR = ("clear", "c")
+COMMAND_QUIT = ("quit", "q")
+COMMAND_RERUN = ("rerun", "r")
+ALL_COMMANDS = [*COMMAND_CLEAR, *COMMAND_QUIT, *COMMAND_RERUN]
 
 
 class ChatSession:
     def __init__(
         self,
         assistant: Assistant,
         listener: ChatListener,
@@ -144,18 +136,14 @@
         self.listener.on_chat_message(user_message)
         self.user_prompts.append((user_message, args))
 
     def _rollback_user_message(self):
         self.messages = self.messages[:-1]
         self.user_prompts = self.user_prompts[:-1]
 
-    def _print_help(self):
-        with self.listener.response_streamer() as stream:
-            stream.on_next_token(COMMANDS_HELP)
-
     def process_input(self, user_input: str, args: Dict[str, Any]):
         """
         Process the user's input and return whether the session should continue.
         """
         if not self._validate_args(args):
             return True
 
@@ -163,17 +151,14 @@
             return False
         elif user_input in COMMAND_CLEAR:
             self._clear()
             return True
         elif user_input in COMMAND_RERUN:
             self._rerun()
             return True
-        elif user_input in COMMAND_HELP:
-            self._print_help()
-            return True
 
         self._add_user_message(user_input, args)
         response_saved = self._respond(args)
         if not response_saved:
             self._rollback_user_message()
 
         return True
```

### Comparing `gpt-command-line-0.1.2/gptcli/shell.py` & `gpt-command-line-0.1.2.dev0/gptcli/shell.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.2/pyproject.toml` & `gpt-command-line-0.1.2.dev0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "gpt-command-line"
-version = "0.1.2"
+version = "0.1.2.dev0"
 description = "Command-line interface for ChatGPT, Claude and Bard"
 authors = [{name = "Val Kharitonov", email = "val@kharvd.com"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.9"
 keywords = ["cli", "command-line", "assistant", "openai", "claude", "bard", "gpt-3", "gpt-4", "llm", "chatgpt", "gpt-cli", "google-bard", "anthropic", "gpt-client", "anthropic-claude", "palm2"]
 classifiers = [
```

### Comparing `gpt-command-line-0.1.2/tests/test_assistant.py` & `gpt-command-line-0.1.2.dev0/tests/test_assistant.py`

 * *Files identical despite different names*

### Comparing `gpt-command-line-0.1.2/tests/test_session.py` & `gpt-command-line-0.1.2.dev0/tests/test_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     listener_mock.on_chat_message.assert_has_calls(
         [mock.call(user_message), mock.call(assistant_message)]
     )
 
 
 def test_quit():
     _, _, session = setup_session()
-    should_continue = session.process_input(":q", {})
+    should_continue = session.process_input("q", {})
     assert not should_continue
 
 
 def test_clear():
     assistant_mock, listener_mock, session = setup_session()
 
     assistant_mock.init_messages.assert_called_once()
@@ -75,15 +75,15 @@
             mock.call({"role": "user", "content": "user_message"}),
             mock.call({"role": "assistant", "content": "assistant_message"}),
         ]
     )
     assistant_mock.complete_chat.reset_mock()
     listener_mock.on_chat_message.reset_mock()
 
-    should_continue = session.process_input(":c", {})
+    should_continue = session.process_input("c", {})
     assert should_continue
 
     assistant_mock.init_messages.assert_called_once()
     listener_mock.on_chat_clear.assert_called_once()
     assistant_mock.complete_chat.assert_not_called()
 
     assistant_mock.complete_chat.return_value = ["assistant_message_1"]
@@ -106,15 +106,15 @@
 def test_rerun():
     assistant_mock, listener_mock, session = setup_session()
 
     assistant_mock.init_messages.assert_called_once()
     assistant_mock.init_messages.reset_mock()
 
     # Re-run before any input shouldn't do anything
-    should_continue = session.process_input(":r", {})
+    should_continue = session.process_input("r", {})
     assert should_continue
 
     assistant_mock.init_messages.assert_not_called()
     assistant_mock.complete_chat.assert_not_called()
     listener_mock.on_chat_message.assert_not_called()
     listener_mock.on_chat_rerun.assert_called_once_with(False)
 
@@ -137,15 +137,15 @@
         ]
     )
     assistant_mock.complete_chat.reset_mock()
     listener_mock.on_chat_message.reset_mock()
 
     assistant_mock.complete_chat.return_value = ["assistant_message_1"]
 
-    should_continue = session.process_input(":r", {})
+    should_continue = session.process_input("r", {})
     assert should_continue
 
     listener_mock.on_chat_rerun.assert_called_once_with(True)
 
     assistant_mock.complete_chat.assert_called_once_with(
         [system_message, {"role": "user", "content": "user_message"}],
         override_params={},
@@ -181,15 +181,15 @@
 
     # Now test that rerun reruns with the same args
     assistant_mock.complete_chat.reset_mock()
     listener_mock.on_chat_message.reset_mock()
 
     assistant_mock.complete_chat.return_value = [expected_response]
 
-    should_continue = session.process_input(":r", {})
+    should_continue = session.process_input("r", {})
     assert should_continue
 
     assistant_mock.complete_chat.assert_called_once_with(
         [system_message, user_message], override_params={"arg1": "value1"}
     )
     listener_mock.on_chat_message.assert_has_calls([mock.call(assistant_message)])
 
@@ -209,15 +209,15 @@
     listener_mock.on_error.assert_called_once_with(error)
 
     # Now rerun shouldn't do anything because user input was not saved
     assistant_mock.complete_chat.reset_mock()
     listener_mock.on_chat_message.reset_mock()
     listener_mock.on_error.reset_mock()
 
-    should_continue = session.process_input(":r", {})
+    should_continue = session.process_input("r", {})
     assert should_continue
 
     assistant_mock.complete_chat.assert_not_called()
     listener_mock.on_chat_message.assert_not_called()
     listener_mock.on_error.assert_not_called()
     listener_mock.on_chat_rerun.assert_called_once_with(False)
 
@@ -244,15 +244,15 @@
     assistant_mock.complete_chat.reset_mock()
     listener_mock.on_chat_message.reset_mock()
     listener_mock.on_error.reset_mock()
 
     assistant_mock.complete_chat.side_effect = None
     assistant_mock.complete_chat.return_value = ["assistant message"]
 
-    should_continue = session.process_input(":r", {})
+    should_continue = session.process_input("r", {})
     assert should_continue
 
     assistant_mock.complete_chat.assert_called_once_with(
         [system_message, user_message], override_params={}
     )
     listener_mock.on_chat_message.assert_has_calls(
         [
```

### Comparing `gpt-command-line-0.1.2/tests/test_term_utils.py` & `gpt-command-line-0.1.2.dev0/tests/test_term_utils.py`

 * *Files identical despite different names*

