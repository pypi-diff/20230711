# Comparing `tmp/ttok-0.1.tar.gz` & `tmp/ttok-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttok-0.1.tar", last modified: Thu May 18 19:54:32 2023, max compression
+gzip compressed data, was "ttok-0.2.tar", last modified: Mon Jul 10 23:38:22 2023, max compression
```

## Comparing `ttok-0.1.tar` & `ttok-0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:54:32.012138 ttok-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-18 19:54:18.000000 ttok-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-18 19:54:32.012138 ttok-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-05-18 19:54:18.000000 ttok-0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 19:54:32.012138 ttok-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-18 19:54:18.000000 ttok-0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:54:32.012138 ttok-0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-18 19:54:18.000000 ttok-0.1/tests/test_ttok.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:54:32.012138 ttok-0.1/ttok/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 19:54:18.000000 ttok-0.1/ttok/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-18 19:54:18.000000 ttok-0.1/ttok/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-18 19:54:18.000000 ttok-0.1/ttok/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 19:54:32.012138 ttok-0.1/ttok.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-18 19:54:32.000000 ttok-0.1/ttok.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-18 19:54:32.000000 ttok-0.1/ttok.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 19:54:32.000000 ttok-0.1/ttok.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 19:54:32.000000 ttok-0.1/ttok.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-18 19:54:32.000000 ttok-0.1/ttok.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-18 19:54:32.000000 ttok-0.1/ttok.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:38:22.424844 ttok-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 23:38:08.000000 ttok-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-07-10 23:38:22.420844 ttok-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-07-10 23:38:08.000000 ttok-0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 23:38:22.424844 ttok-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-10 23:38:08.000000 ttok-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:38:22.420844 ttok-0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-07-10 23:38:08.000000 ttok-0.2/tests/test_ttok.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:38:22.420844 ttok-0.2/ttok/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 23:38:08.000000 ttok-0.2/ttok/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-10 23:38:08.000000 ttok-0.2/ttok/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-10 23:38:08.000000 ttok-0.2/ttok/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 23:38:22.420844 ttok-0.2/ttok.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-07-10 23:38:22.000000 ttok-0.2/ttok.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-10 23:38:22.000000 ttok-0.2/ttok.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 23:38:22.000000 ttok-0.2/ttok.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 23:38:22.000000 ttok-0.2/ttok.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-10 23:38:22.000000 ttok-0.2/ttok.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 23:38:22.000000 ttok-0.2/ttok.egg-info/top_level.txt
```

### Comparing `ttok-0.1/LICENSE` & `ttok-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ttok-0.1/PKG-INFO` & `ttok-0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: ttok
-Version: 0.1
-Summary: Count and truncate text based on tokens
-Home-page: https://github.com/simonw/ttok
-Author: Simon Willison
-License: Apache License, Version 2.0
-Project-URL: Issues, https://github.com/simonw/ttok/issues
-Project-URL: CI, https://github.com/simonw/ttok/actions
-Project-URL: Changelog, https://github.com/simonw/ttok/releases
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 # ttok
 
 [![PyPI](https://img.shields.io/pypi/v/ttok.svg)](https://pypi.org/project/ttok/)
 [![Changelog](https://img.shields.io/github/v/release/simonw/ttok?include_prereleases&label=changelog)](https://github.com/simonw/ttok/releases)
 [![Tests](https://github.com/simonw/ttok/workflows/Test/badge.svg)](https://github.com/simonw/ttok/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/ttok/blob/master/LICENSE)
 
@@ -26,14 +11,16 @@
 
 Large language models such as GPT-3.5 and GPT-4 work in terms of tokens.
 
 This tool can count tokens, using OpenAI's [tiktoken](https://github.com/openai/tiktoken) library.
 
 It can also truncate text to a specified number of tokens.
 
+See [llm, ttok and strip-tags—CLI tools for working with ChatGPT and other LLMs](https://simonwillison.net/2023/May/18/cli-tools-for-llms/) for more on this project.
+
 ## Installation
 
 Install this tool using `pip`:
 
     pip install ttok
 
 ## Counting tokens
@@ -44,25 +31,25 @@
 ttok Hello world
 ```
 ```
 2
 ```
 You can also pipe text into the tool:
 ```bash
-echo -n "Hello world" -n | ttok
+echo -n "Hello world" | ttok
 ```
 ```
 2
 ```
 Here the `echo -n` option prevents echo from adding a newline - without that you would get a token count of 3.
 
 To pipe in text and then append extra tokens from arguments, use the `-i -` option:
 
 ```bash
-echo -n "Hello world" -n | ttok more text -i -
+echo -n "Hello world" | ttok more text -i -
 ```
 ```
 6
 ```
 ## Different models
 
 By default, the tokenizer model for GPT-3.5 and GPT-4 is used.
@@ -93,22 +80,38 @@
 ```
 ```
 This is too
 ```
 
 ## Viewing tokens
 
-The `--tokens` option can be used to view the integer token IDs for the incoming text:
+The `--encode` option can be used to view the integer token IDs for the incoming text:
 
 ```bash
-ttok Hello world --tokens
+ttok Hello world --encode
 ```
 ```
 9906 1917
 ```
+The `--decode` method reverses this process:
+
+```bash
+ttok 9906 1917 --decode
+```
+```
+Hello world
+```
+Add `--tokens` to either of these options to see a detailed breakdown of the tokens:
+
+```bash
+ttok Hello world --encode --tokens
+```
+```
+[b'Hello', b' world']
+```
 
 ## ttok --help
 
 <!-- [[[cog
 import cog
 from ttok import cli
 from click.testing import CliRunner
@@ -136,24 +139,38 @@
 
       cat input.txt | ttok -t 100
 
   To truncate to 100 tokens using the gpt2 model:
 
       cat input.txt | ttok -t 100 -m gpt2
 
-  To view tokens:
+  To view token integers:
+
+      cat input.txt | ttok --encode
+
+  To convert tokens back to text:
+
+      ttok 9906 1917 --decode
+
+  To see the details of the tokens:
+
+      ttok "hello world" --tokens
+
+  Outputs:
 
-      cat input.txt | ttok --tokens
+      [b'hello', b' world']
 
 Options:
   --version               Show the version and exit.
   -i, --input FILENAME
   -t, --truncate INTEGER  Truncate to this many tokens
   -m, --model TEXT        Which model to use
-  --tokens                Output token integers
+  --encode, --tokens      Output token integers
+  --decode                Convert token integers to text
+  --tokens                Output full tokens
   --help                  Show this message and exit.
 
 ```
 <!-- [[[end]]] -->
 
 You can also run this command using:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ttok-0.1/README.md` & `ttok-0.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: ttok
+Version: 0.2
+Summary: Count and truncate text based on tokens
+Home-page: https://github.com/simonw/ttok
+Author: Simon Willison
+License: Apache License, Version 2.0
+Project-URL: Issues, https://github.com/simonw/ttok/issues
+Project-URL: CI, https://github.com/simonw/ttok/actions
+Project-URL: Changelog, https://github.com/simonw/ttok/releases
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
 # ttok
 
 [![PyPI](https://img.shields.io/pypi/v/ttok.svg)](https://pypi.org/project/ttok/)
 [![Changelog](https://img.shields.io/github/v/release/simonw/ttok?include_prereleases&label=changelog)](https://github.com/simonw/ttok/releases)
 [![Tests](https://github.com/simonw/ttok/workflows/Test/badge.svg)](https://github.com/simonw/ttok/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/ttok/blob/master/LICENSE)
 
@@ -11,14 +26,16 @@
 
 Large language models such as GPT-3.5 and GPT-4 work in terms of tokens.
 
 This tool can count tokens, using OpenAI's [tiktoken](https://github.com/openai/tiktoken) library.
 
 It can also truncate text to a specified number of tokens.
 
+See [llm, ttok and strip-tags—CLI tools for working with ChatGPT and other LLMs](https://simonwillison.net/2023/May/18/cli-tools-for-llms/) for more on this project.
+
 ## Installation
 
 Install this tool using `pip`:
 
     pip install ttok
 
 ## Counting tokens
@@ -29,25 +46,25 @@
 ttok Hello world
 ```
 ```
 2
 ```
 You can also pipe text into the tool:
 ```bash
-echo -n "Hello world" -n | ttok
+echo -n "Hello world" | ttok
 ```
 ```
 2
 ```
 Here the `echo -n` option prevents echo from adding a newline - without that you would get a token count of 3.
 
 To pipe in text and then append extra tokens from arguments, use the `-i -` option:
 
 ```bash
-echo -n "Hello world" -n | ttok more text -i -
+echo -n "Hello world" | ttok more text -i -
 ```
 ```
 6
 ```
 ## Different models
 
 By default, the tokenizer model for GPT-3.5 and GPT-4 is used.
@@ -78,22 +95,38 @@
 ```
 ```
 This is too
 ```
 
 ## Viewing tokens
 
-The `--tokens` option can be used to view the integer token IDs for the incoming text:
+The `--encode` option can be used to view the integer token IDs for the incoming text:
 
 ```bash
-ttok Hello world --tokens
+ttok Hello world --encode
 ```
 ```
 9906 1917
 ```
+The `--decode` method reverses this process:
+
+```bash
+ttok 9906 1917 --decode
+```
+```
+Hello world
+```
+Add `--tokens` to either of these options to see a detailed breakdown of the tokens:
+
+```bash
+ttok Hello world --encode --tokens
+```
+```
+[b'Hello', b' world']
+```
 
 ## ttok --help
 
 <!-- [[[cog
 import cog
 from ttok import cli
 from click.testing import CliRunner
@@ -121,24 +154,38 @@
 
       cat input.txt | ttok -t 100
 
   To truncate to 100 tokens using the gpt2 model:
 
       cat input.txt | ttok -t 100 -m gpt2
 
-  To view tokens:
+  To view token integers:
+
+      cat input.txt | ttok --encode
+
+  To convert tokens back to text:
+
+      ttok 9906 1917 --decode
+
+  To see the details of the tokens:
+
+      ttok "hello world" --tokens
+
+  Outputs:
 
-      cat input.txt | ttok --tokens
+      [b'hello', b' world']
 
 Options:
   --version               Show the version and exit.
   -i, --input FILENAME
   -t, --truncate INTEGER  Truncate to this many tokens
   -m, --model TEXT        Which model to use
-  --tokens                Output token integers
+  --encode, --tokens      Output token integers
+  --decode                Convert token integers to text
+  --tokens                Output full tokens
   --help                  Show this message and exit.
 
 ```
 <!-- [[[end]]] -->
 
 You can also run this command using:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ttok-0.1/setup.py` & `ttok-0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.1"
+VERSION = "0.2"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
```

### Comparing `ttok-0.1/ttok/cli.py` & `ttok-0.2/ttok/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 import click
+import re
 import sys
 import tiktoken
 
 
 @click.command()
 @click.version_option()
 @click.argument("prompt", nargs=-1)
 @click.option("-i", "--input", "input", type=click.File("r"))
 @click.option(
     "-t", "--truncate", "truncate", type=int, help="Truncate to this many tokens"
 )
 @click.option("-m", "--model", default="gpt-3.5-turbo", help="Which model to use")
-@click.option("output_tokens", "--tokens", is_flag=True, help="Output token integers")
-def cli(prompt, input, truncate, model, output_tokens):
+@click.option(
+    "encode_tokens", "--encode", "--tokens", is_flag=True, help="Output token integers"
+)
+@click.option(
+    "decode_tokens", "--decode", is_flag=True, help="Convert token integers to text"
+)
+@click.option("as_tokens", "--tokens", is_flag=True, help="Output full tokens")
+def cli(prompt, input, truncate, model, encode_tokens, decode_tokens, as_tokens):
     """
     Count and truncate text based on tokens
 
     To count tokens for text passed as arguments:
 
         ttok one two three
 
@@ -28,35 +35,63 @@
 
         cat input.txt | ttok -t 100
 
     To truncate to 100 tokens using the gpt2 model:
 
         cat input.txt | ttok -t 100 -m gpt2
 
-    To view tokens:
+    To view token integers:
+
+        cat input.txt | ttok --encode
+
+    To convert tokens back to text:
+
+        ttok 9906 1917 --decode
 
-        cat input.txt | ttok --tokens
+    To see the details of the tokens:
+
+        ttok "hello world" --tokens
+
+    Outputs:
+
+        [b'hello', b' world']
     """
+    if decode_tokens and encode_tokens:
+        raise click.ClickException("Cannot use --decode with --encode")
+    if as_tokens and not decode_tokens and not encode_tokens:
+        encode_tokens = True
     try:
         encoding = tiktoken.encoding_for_model(model)
     except KeyError as e:
         raise click.ClickException(f"Invalid model: {model}") from e
     if not prompt and input is None:
         input = sys.stdin
     text = " ".join(prompt)
     if input is not None:
         input_text = input.read()
         if text:
             text = input_text + " " + text
         else:
             text = input_text
+
+    if decode_tokens:
+        tokens = [int(token) for token in re.findall(r"\d+", text)]
+        if as_tokens:
+            click.echo(encoding.decode_tokens_bytes(tokens))
+        else:
+            click.echo(encoding.decode(tokens))
+        return
+
     # Tokenize it
     tokens = encoding.encode(text)
     if truncate:
         tokens = tokens[:truncate]
 
-    if output_tokens:
-        click.echo(" ".join(str(t) for t in tokens))
+    if encode_tokens:
+        if as_tokens:
+            click.echo(encoding.decode_tokens_bytes(tokens))
+        else:
+            click.echo(" ".join(str(t) for t in tokens))
     elif truncate:
         click.echo(encoding.decode(tokens), nl=False)
     else:
         click.echo(len(tokens))
```

### Comparing `ttok-0.1/ttok.egg-info/PKG-INFO` & `ttok-0.2/ttok.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ttok
-Version: 0.1
+Version: 0.2
 Summary: Count and truncate text based on tokens
 Home-page: https://github.com/simonw/ttok
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/ttok/issues
 Project-URL: CI, https://github.com/simonw/ttok/actions
 Project-URL: Changelog, https://github.com/simonw/ttok/releases
@@ -26,14 +26,16 @@
 
 Large language models such as GPT-3.5 and GPT-4 work in terms of tokens.
 
 This tool can count tokens, using OpenAI's [tiktoken](https://github.com/openai/tiktoken) library.
 
 It can also truncate text to a specified number of tokens.
 
+See [llm, ttok and strip-tags—CLI tools for working with ChatGPT and other LLMs](https://simonwillison.net/2023/May/18/cli-tools-for-llms/) for more on this project.
+
 ## Installation
 
 Install this tool using `pip`:
 
     pip install ttok
 
 ## Counting tokens
@@ -44,25 +46,25 @@
 ttok Hello world
 ```
 ```
 2
 ```
 You can also pipe text into the tool:
 ```bash
-echo -n "Hello world" -n | ttok
+echo -n "Hello world" | ttok
 ```
 ```
 2
 ```
 Here the `echo -n` option prevents echo from adding a newline - without that you would get a token count of 3.
 
 To pipe in text and then append extra tokens from arguments, use the `-i -` option:
 
 ```bash
-echo -n "Hello world" -n | ttok more text -i -
+echo -n "Hello world" | ttok more text -i -
 ```
 ```
 6
 ```
 ## Different models
 
 By default, the tokenizer model for GPT-3.5 and GPT-4 is used.
@@ -93,22 +95,38 @@
 ```
 ```
 This is too
 ```
 
 ## Viewing tokens
 
-The `--tokens` option can be used to view the integer token IDs for the incoming text:
+The `--encode` option can be used to view the integer token IDs for the incoming text:
 
 ```bash
-ttok Hello world --tokens
+ttok Hello world --encode
 ```
 ```
 9906 1917
 ```
+The `--decode` method reverses this process:
+
+```bash
+ttok 9906 1917 --decode
+```
+```
+Hello world
+```
+Add `--tokens` to either of these options to see a detailed breakdown of the tokens:
+
+```bash
+ttok Hello world --encode --tokens
+```
+```
+[b'Hello', b' world']
+```
 
 ## ttok --help
 
 <!-- [[[cog
 import cog
 from ttok import cli
 from click.testing import CliRunner
@@ -136,24 +154,38 @@
 
       cat input.txt | ttok -t 100
 
   To truncate to 100 tokens using the gpt2 model:
 
       cat input.txt | ttok -t 100 -m gpt2
 
-  To view tokens:
+  To view token integers:
+
+      cat input.txt | ttok --encode
+
+  To convert tokens back to text:
+
+      ttok 9906 1917 --decode
+
+  To see the details of the tokens:
+
+      ttok "hello world" --tokens
+
+  Outputs:
 
-      cat input.txt | ttok --tokens
+      [b'hello', b' world']
 
 Options:
   --version               Show the version and exit.
   -i, --input FILENAME
   -t, --truncate INTEGER  Truncate to this many tokens
   -m, --model TEXT        Which model to use
-  --tokens                Output token integers
+  --encode, --tokens      Output token integers
+  --decode                Convert token integers to text
+  --tokens                Output full tokens
   --help                  Show this message and exit.
 
 ```
 <!-- [[[end]]] -->
 
 You can also run this command using:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

