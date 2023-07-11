# Comparing `tmp/xinference-0.0.1.tar.gz` & `tmp/xinference-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xinference-0.0.1.tar", last modified: Mon Jul 10 10:40:01 2023, max compression
+gzip compressed data, was "xinference-0.0.2.tar", last modified: Tue Jul 11 12:03:14 2023, max compression
```

## Comparing `xinference-0.0.1.tar` & `xinference-0.0.2.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:40:01.950876 xinference-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-10 10:39:51.000000 xinference-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-10 10:39:51.000000 xinference-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-07-10 10:40:01.950876 xinference-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9198 2023-07-10 10:39:51.000000 xinference-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-10 10:39:51.000000 xinference-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-07-10 10:40:01.950876 xinference-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-10 10:39:51.000000 xinference-0.0.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-07-10 10:39:51.000000 xinference-0.0.1/versioneer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:40:01.954876 xinference-0.0.1/xinference/
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-10 10:39:51.000000 xinference-0.0.1/xinference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-10 10:40:01.954876 xinference-0.0.1/xinference/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-07-10 10:39:51.000000 xinference-0.0.1/xinference/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-10 10:39:51.000000 xinference-0.0.1/xinference/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:40:01.950876 xinference-0.0.1/xinference/core/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-10 10:39:51.000000 xinference-0.0.1/xinference/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-07-10 10:39:51.000000 xinference-0.0.1/xinference/core/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15688 2023-07-10 10:39:51.000000 xinference-0.0.1/xinference/core/gradio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-07-10 10:39:51.000000 xinference-0.0.1/xinference/core/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-10 10:39:51.000000 xinference-0.0.1/xinference/core/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    14938 2023-07-10 10:39:51.000000 xinference-0.0.1/xinference/core/restful_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12065 2023-07-10 10:39:51.000000 xinference-0.0.1/xinference/core/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:40:01.950876 xinference-0.0.1/xinference/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-10 10:39:51.000000 xinference-0.0.1/xinference/deploy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-07-10 10:39:51.000000 xinference-0.0.1/xinference/deploy/cmdline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-10 10:39:51.000000 xinference-0.0.1/xinference/deploy/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-10 10:39:51.000000 xinference-0.0.1/xinference/deploy/supervisor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:40:01.950876 xinference-0.0.1/xinference/deploy/test/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-10 10:39:51.000000 xinference-0.0.1/xinference/deploy/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-10 10:39:51.000000 xinference-0.0.1/xinference/deploy/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-07-10 10:39:51.000000 xinference-0.0.1/xinference/deploy/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-10 10:39:51.000000 xinference-0.0.1/xinference/isolation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:40:01.950876 xinference-0.0.1/xinference/locale/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-10 10:39:51.000000 xinference-0.0.1/xinference/locale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-10 10:39:51.000000 xinference-0.0.1/xinference/locale/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:40:01.950876 xinference-0.0.1/xinference/model/
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-07-10 10:39:51.000000 xinference-0.0.1/xinference/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:40:01.950876 xinference-0.0.1/xinference/model/llm/
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-07-10 10:39:51.000000 xinference-0.0.1/xinference/model/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-07-10 10:39:51.000000 xinference-0.0.1/xinference/model/llm/chatglm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10115 2023-07-10 10:39:51.000000 xinference-0.0.1/xinference/model/llm/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-10 10:39:51.000000 xinference-0.0.1/xinference/model/llm/orca.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-10 10:39:51.000000 xinference-0.0.1/xinference/model/llm/vicuna.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-10 10:39:51.000000 xinference-0.0.1/xinference/model/llm/wizardlm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-10 10:39:51.000000 xinference-0.0.1/xinference/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 10:40:01.950876 xinference-0.0.1/xinference.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-07-10 10:40:01.000000 xinference-0.0.1/xinference.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-10 10:40:01.000000 xinference-0.0.1/xinference.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 10:40:01.000000 xinference-0.0.1/xinference.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-10 10:40:01.000000 xinference-0.0.1/xinference.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 10:40:01.000000 xinference-0.0.1/xinference.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-10 10:40:01.000000 xinference-0.0.1/xinference.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-10 10:40:01.000000 xinference-0.0.1/xinference.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:03:14.335573 xinference-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-11 12:03:02.000000 xinference-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-11 12:03:02.000000 xinference-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9800 2023-07-11 12:03:14.335573 xinference-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8959 2023-07-11 12:03:02.000000 xinference-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-11 12:03:02.000000 xinference-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-11 12:03:14.339573 xinference-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-11 12:03:02.000000 xinference-0.0.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-07-11 12:03:02.000000 xinference-0.0.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:03:14.339573 xinference-0.0.2/xinference/
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-11 12:03:14.339573 xinference-0.0.2/xinference/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:03:14.331573 xinference-0.0.2/xinference/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/core/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15729 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/core/gradio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/core/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/core/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15058 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/core/restful_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/core/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:03:14.331573 xinference-0.0.2/xinference/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/deploy/cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/deploy/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/deploy/supervisor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:03:14.335573 xinference-0.0.2/xinference/deploy/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/deploy/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/deploy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/deploy/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/isolation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:03:14.335573 xinference-0.0.2/xinference/locale/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/locale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/locale/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/locale/zh_CN.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:03:14.335573 xinference-0.0.2/xinference/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:03:14.335573 xinference-0.0.2/xinference/model/llm/
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/model/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/model/llm/chatglm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10115 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/model/llm/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/model/llm/orca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/model/llm/vicuna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/model/llm/wizardlm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-11 12:03:02.000000 xinference-0.0.2/xinference/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:03:14.327573 xinference-0.0.2/xinference.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9800 2023-07-11 12:03:14.000000 xinference-0.0.2/xinference.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-11 12:03:14.000000 xinference-0.0.2/xinference.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 12:03:14.000000 xinference-0.0.2/xinference.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-11 12:03:14.000000 xinference-0.0.2/xinference.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 12:03:13.000000 xinference-0.0.2/xinference.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-11 12:03:14.000000 xinference-0.0.2/xinference.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-11 12:03:14.000000 xinference-0.0.2/xinference.egg-info/top_level.txt
```

### Comparing `xinference-0.0.1/LICENSE` & `xinference-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xinference-0.0.1/PKG-INFO` & `xinference-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xinference
-Version: 0.0.1
+Version: 0.0.2
 Summary: Model Serving Made Easy
 Home-page: https://github.com/xorbitsai/inference
 Author: Qin Xuye
 Author-email: qinxuye@xprobe.io
 Maintainer: Qin Xuye
 Maintainer-email: qinxuye@xprobe.io
 License: Apache License 2.0
@@ -15,41 +15,45 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: all
 License-File: LICENSE
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/xinference.svg?style=for-the-badge)](https://pypi.org/project/xinference/)
-[![License](https://img.shields.io/pypi/l/inference.svg?style=for-the-badge)](https://github.com/xorbitsai/inference/blob/main/LICENSE)
+[![License](https://img.shields.io/pypi/l/xinference.svg?style=for-the-badge)](https://github.com/xorbitsai/inference/blob/main/LICENSE)
 [![Build Status](https://img.shields.io/github/actions/workflow/status/xorbitsai/inference/python.yaml?branch=main&style=for-the-badge&label=GITHUB%20ACTIONS&logo=github)](https://actions-badge.atrox.dev/xorbitsai/inference/goto?ref=main)
 [![Slack](https://img.shields.io/badge/join_Slack-781FF5.svg?logo=slack&style=for-the-badge)](https://join.slack.com/t/xorbitsio/shared_invite/zt-1o3z9ucdh-RbfhbPVpx7prOVdM1CAuxg)
 [![Twitter](https://img.shields.io/twitter/follow/xorbitsio?logo=twitter&style=for-the-badge)](https://twitter.com/xorbitsio)
 
-# Xorbits inference: Model Serving Made Easy 🤖
+# Xorbits Inference: Model Serving Made Easy 🤖
 
 Welcome to the Xorbits Inference GitHub repository!
 
 Xorbits Inference(Xinference) is a powerful and versatile library designed to serve language, 
 speech recognition, and multimodal models. With Xorbits Inference, you can effortlessly deploy 
 and serve your or state-of-the-art built-in models using just a single command. Whether you are a 
 researcher, developer, or data scientist, Xorbits Inference empowers you to unleash the full 
 potential of cutting-edge AI models.
 
 Currently, Xorbits Inference relies on [ggml](https://github.com/ggerganov/ggml) for model serving,
 which is specifically designed to enable large models and high performance on commodity hardware. 
 We are actively working on expanding Xorbits Inference's support to include additional runtimes, 
 including PyTorch and JAX, in the near future.
 
+![demo](assets/demo.gif)
+
+
 ## Key Features
 🌟 **Model Serving Made Easy**: Inference simplifies the process of serving large language, speech 
-recognition, and multimodal models. With a single command, you can set up and deploy your models 
-for experimentation and production.
+recognition, and multimodal models. You can set up and deploy your models
+for experimentation and production with a single command.
 
 ⚡️ **State-of-the-Art Models**: Experiment with cutting-edge built-in models using a single 
 command. Inference provides access to state-of-the-art open-source models!
 
 🖥 **Heterogeneous Hardware Utilization**: Make the most of your hardware resources. Xorbits 
 Inference intelligently utilizes heterogeneous hardware, including GPUs and CPUs, to maximize
 performance and accelerate your model inference tasks.
@@ -59,61 +63,62 @@
 your models with existing systems or use the command-line interface (CLI) and the intuitive WebUI
 for seamless management and monitoring.
 
 🌐 **Distributed Deployment**: Xorbits Inference excels in distributed deployment scenarios, 
 allowing the seamless distribution of model inference across multiple devices or machines. It
 leverages distributed computing techniques to parallelize and scale the inference process.
 
-🔌 **Built-in Integration with Third-Party Libraries**: Xorbits Inference provides seamless
-integration with popular third-party libraries like LangChain and LlamaIndex. (Coming soon)
+🔌 **Built-in Integration with Third-Party Libraries**: Xorbits Inference seamlessly integrates
+with popular third-party libraries like LangChain and LlamaIndex. (Coming soon)
 
 ## Getting Started
 Xinference can be installed via pip from PyPI. It is highly recommended to create a new virtual
 environment to avoid conflicts.
 ```bash
-$ pip install xinference
+$ pip install "xinference[all]"
 ```
+"xinference[all]" installs all the necessary packages for serving models. If you want to achieve acceleration on 
+different hardware, refer to the installation documentation of the corresponding package.
+- [llama-cpp-python](https://github.com/abetlen/llama-cpp-python#installation-from-pypi-recommended) is required to run `baichuan`, `wizardlm-v1.0`, `vicuna-v1.3` and `orca`.
+- [chatglm-cpp-python](https://github.com/li-plus/chatglm.cpp#getting-started) is required to run `chatglm` and `chatglm2`.
+
 
 ### Deployment
-To start a local instance of Xinference, run the following command:
+You can deploy Xinference locally with a single command or deploy it in a distributed cluster. 
 
+#### Local
+To start a local instance of Xinference, run the following command:
 ```bash
-$ xinference -H,--host "localhost" \
-             -p,--port 9997 \
-             --log-level INFO
+$ xinference
 ```
 
-To deploy Xinference in a cluster, you need to start an Xinference supervisor on one server and 
+#### Distributed
+
+To deploy Xinference in a cluster, you need to start a Xinference supervisor on one server and 
 Xinference workers on the other servers. Follow the steps below:
 
-#### Starting the Supervisor
-On the server where you want to run the Xinference supervisor, run the following command:
+**Starting the Supervisor**: On the server where you want to run the Xinference supervisor, run the following command:
 ```bash
-$ xinference-supervisor -H,--host "${supervisor_host}" \
-                        -p,--port 9997 \
-                        --log-level INFO
+$ xinference-supervisor -H "${supervisor_host}"
 ```
 Replace `${supervisor_host}` with the actual host of your supervisor server.
 
-#### Starting the Workers
-On each of the other servers where you want to run Xinference workers, run the following command:
+**Starting the Workers**: On each of the other servers where you want to run Xinference workers, run the following command:
 ```bash
-$ xinference-worker -e, --endpoint "http://${supervisor_host}:9997" \
-                    -H,--host "0.0.0.0" \
-                    --log-level INFO
+$ xinference-worker -e "http://${supervisor_host}:9997"
 ```
 
 Once Xinference is running, an endpoint will be accessible for model management via CLI or
 Xinference  client.
 
 - For local deployment, the endpoint will be `http://localhost:9997`.
 - For cluster deployment, the endpoint will be `http://${supervisor_host}:9997`, where
 `${supervisor_host}` is the hostname or IP address of the server where the supervisor is running.
 
-You can also view a web UI using the Xinference endpoint where you can chat with all the 
+You can also view a web UI using the Xinference endpoint to chat with all the 
 builtin models. You can even **chat with two cutting-edge AI models side-by-side to compare
 their performance**!
 
 ![web UI](assets/xinference-downloading.png)
 
 ### Xinference CLI
 Xinference provides a command line interface (CLI) for model management. Here are some useful 
@@ -173,32 +178,33 @@
 
 ## Builtin models
 To view the builtin models, run the following command:
 ```bash
 $ xinference list --all
 ```
 
-| Name                 | Format  | Size (in billions) | Quantization                                                                                                                   |
-| -------------------- | ------- | ------------------ |--------------------------------------------------------------------------------------------------------------------------------|
-| baichuan             | ggmlv3  | [7]                | ['q2_K', 'q3_K_L', 'q3_K_M', 'q3_K_S', 'q4_0', 'q4_1', 'q4_K_M', 'q4_K_S', 'q5_0', 'q5_1', 'q5_K_M', 'q5_K_S', 'q6_K', 'q8_0'] |
-| wizardlm-v1.0        | ggmlv3  | [7, 13, 33]        | ['q2_K', 'q3_K_L', 'q3_K_M', 'q3_K_S', 'q4_0', 'q4_1', 'q4_K_M', 'q4_K_S', 'q5_0', 'q5_1', 'q5_K_M', 'q5_K_S', 'q6_K', 'q8_0'] |
-| vicuna-v1.3          | ggmlv3  | [7, 13]            | ['q2_K', 'q3_K_L', 'q3_K_M', 'q3_K_S', 'q4_0', 'q4_1', 'q4_K_M', 'q4_K_S', 'q5_0', 'q5_1', 'q5_K_M', 'q5_K_S', 'q6_K', 'q8_0'] |
-| orca                 | ggmlv3  | [3, 7, 13]         | ['q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0']                                                                                       |
-| chatglm              | ggmlv3  | [6]                | ['q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0']                                                                                       |
-| chatglm2             | ggmlv3  | [6]                | ['q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0']                                                                                       |
+| Name                 | Type             | Language | Format | Size (in billions) | Quantization                           |
+| -------------------- |------------------|----------|--------|--------------------|----------------------------------------|
+| baichuan             | Foundation Model | en, zh   | ggmlv3 | 7                  | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' |
+| chatglm              | SFT Model        | en, zh   | ggmlv3 | 6                  | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' |
+| chatglm2             | SFT Model        | en, zh   | ggmlv3 | 6                  | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' |
+| wizardlm-v1.0        | SFT Model        | en       | ggmlv3 | 7, 13, 33          | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' |
+| vicuna-v1.3          | SFT Model        | en       | ggmlv3 | 7, 13              | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' |
+| orca                 | SFT Model        | en       | ggmlv3 | 3, 7, 13           | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' |
+
 
 **NOTE**:
-- [llama-cpp-python](https://github.com/abetlen/llama-cpp-python) is required to run `baichuan`, `wizardlm-v1.0`, `vicuna-v1.3` and `orca`.
-- [chatglm-cpp-python](https://github.com/li-plus/chatglm.cpp) is required to run `chatglm` and `chatglm2`.
-- Xinference will download models automatically for you and by default the models will be saved under `${USER}/.xinference/cache`.
+- Xinference will download models automatically for you, and by default the models will be saved under `${USER}/.xinference/cache`.
+- Foundation models only provide interface `generate`.
+- SFT models provide both `generate` and `chat`.
 
 ## Roadmap
 Xinference is currently under active development. Here's a roadmap outlining our planned 
 developments for the next few weeks:
 
 ### PyTorch Support
-With PyTorch integration, users will be able to seamlessly utilize PyTorch models form huggingface
+With PyTorch integration, users will be able to seamlessly utilize PyTorch models from Hugging Face
 within Xinference.
 
 ### Langchain & LlamaIndex integration
 With Xinference, it will be much easier for users to use these libraries and build applications 
 with LLMs.
```

### Comparing `xinference-0.0.1/README.md` & `xinference-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 [![PyPI Latest Release](https://img.shields.io/pypi/v/xinference.svg?style=for-the-badge)](https://pypi.org/project/xinference/)
-[![License](https://img.shields.io/pypi/l/inference.svg?style=for-the-badge)](https://github.com/xorbitsai/inference/blob/main/LICENSE)
+[![License](https://img.shields.io/pypi/l/xinference.svg?style=for-the-badge)](https://github.com/xorbitsai/inference/blob/main/LICENSE)
 [![Build Status](https://img.shields.io/github/actions/workflow/status/xorbitsai/inference/python.yaml?branch=main&style=for-the-badge&label=GITHUB%20ACTIONS&logo=github)](https://actions-badge.atrox.dev/xorbitsai/inference/goto?ref=main)
 [![Slack](https://img.shields.io/badge/join_Slack-781FF5.svg?logo=slack&style=for-the-badge)](https://join.slack.com/t/xorbitsio/shared_invite/zt-1o3z9ucdh-RbfhbPVpx7prOVdM1CAuxg)
 [![Twitter](https://img.shields.io/twitter/follow/xorbitsio?logo=twitter&style=for-the-badge)](https://twitter.com/xorbitsio)
 
-# Xorbits inference: Model Serving Made Easy 🤖
+# Xorbits Inference: Model Serving Made Easy 🤖
 
 Welcome to the Xorbits Inference GitHub repository!
 
 Xorbits Inference(Xinference) is a powerful and versatile library designed to serve language, 
 speech recognition, and multimodal models. With Xorbits Inference, you can effortlessly deploy 
 and serve your or state-of-the-art built-in models using just a single command. Whether you are a 
 researcher, developer, or data scientist, Xorbits Inference empowers you to unleash the full 
 potential of cutting-edge AI models.
 
 Currently, Xorbits Inference relies on [ggml](https://github.com/ggerganov/ggml) for model serving,
 which is specifically designed to enable large models and high performance on commodity hardware. 
 We are actively working on expanding Xorbits Inference's support to include additional runtimes, 
 including PyTorch and JAX, in the near future.
 
+![demo](assets/demo.gif)
+
+
 ## Key Features
 🌟 **Model Serving Made Easy**: Inference simplifies the process of serving large language, speech 
-recognition, and multimodal models. With a single command, you can set up and deploy your models 
-for experimentation and production.
+recognition, and multimodal models. You can set up and deploy your models
+for experimentation and production with a single command.
 
 ⚡️ **State-of-the-Art Models**: Experiment with cutting-edge built-in models using a single 
 command. Inference provides access to state-of-the-art open-source models!
 
 🖥 **Heterogeneous Hardware Utilization**: Make the most of your hardware resources. Xorbits 
 Inference intelligently utilizes heterogeneous hardware, including GPUs and CPUs, to maximize
 performance and accelerate your model inference tasks.
@@ -36,61 +39,62 @@
 your models with existing systems or use the command-line interface (CLI) and the intuitive WebUI
 for seamless management and monitoring.
 
 🌐 **Distributed Deployment**: Xorbits Inference excels in distributed deployment scenarios, 
 allowing the seamless distribution of model inference across multiple devices or machines. It
 leverages distributed computing techniques to parallelize and scale the inference process.
 
-🔌 **Built-in Integration with Third-Party Libraries**: Xorbits Inference provides seamless
-integration with popular third-party libraries like LangChain and LlamaIndex. (Coming soon)
+🔌 **Built-in Integration with Third-Party Libraries**: Xorbits Inference seamlessly integrates
+with popular third-party libraries like LangChain and LlamaIndex. (Coming soon)
 
 ## Getting Started
 Xinference can be installed via pip from PyPI. It is highly recommended to create a new virtual
 environment to avoid conflicts.
 ```bash
-$ pip install xinference
+$ pip install "xinference[all]"
 ```
+"xinference[all]" installs all the necessary packages for serving models. If you want to achieve acceleration on 
+different hardware, refer to the installation documentation of the corresponding package.
+- [llama-cpp-python](https://github.com/abetlen/llama-cpp-python#installation-from-pypi-recommended) is required to run `baichuan`, `wizardlm-v1.0`, `vicuna-v1.3` and `orca`.
+- [chatglm-cpp-python](https://github.com/li-plus/chatglm.cpp#getting-started) is required to run `chatglm` and `chatglm2`.
+
 
 ### Deployment
-To start a local instance of Xinference, run the following command:
+You can deploy Xinference locally with a single command or deploy it in a distributed cluster. 
 
+#### Local
+To start a local instance of Xinference, run the following command:
 ```bash
-$ xinference -H,--host "localhost" \
-             -p,--port 9997 \
-             --log-level INFO
+$ xinference
 ```
 
-To deploy Xinference in a cluster, you need to start an Xinference supervisor on one server and 
+#### Distributed
+
+To deploy Xinference in a cluster, you need to start a Xinference supervisor on one server and 
 Xinference workers on the other servers. Follow the steps below:
 
-#### Starting the Supervisor
-On the server where you want to run the Xinference supervisor, run the following command:
+**Starting the Supervisor**: On the server where you want to run the Xinference supervisor, run the following command:
 ```bash
-$ xinference-supervisor -H,--host "${supervisor_host}" \
-                        -p,--port 9997 \
-                        --log-level INFO
+$ xinference-supervisor -H "${supervisor_host}"
 ```
 Replace `${supervisor_host}` with the actual host of your supervisor server.
 
-#### Starting the Workers
-On each of the other servers where you want to run Xinference workers, run the following command:
+**Starting the Workers**: On each of the other servers where you want to run Xinference workers, run the following command:
 ```bash
-$ xinference-worker -e, --endpoint "http://${supervisor_host}:9997" \
-                    -H,--host "0.0.0.0" \
-                    --log-level INFO
+$ xinference-worker -e "http://${supervisor_host}:9997"
 ```
 
 Once Xinference is running, an endpoint will be accessible for model management via CLI or
 Xinference  client.
 
 - For local deployment, the endpoint will be `http://localhost:9997`.
 - For cluster deployment, the endpoint will be `http://${supervisor_host}:9997`, where
 `${supervisor_host}` is the hostname or IP address of the server where the supervisor is running.
 
-You can also view a web UI using the Xinference endpoint where you can chat with all the 
+You can also view a web UI using the Xinference endpoint to chat with all the 
 builtin models. You can even **chat with two cutting-edge AI models side-by-side to compare
 their performance**!
 
 ![web UI](assets/xinference-downloading.png)
 
 ### Xinference CLI
 Xinference provides a command line interface (CLI) for model management. Here are some useful 
@@ -150,32 +154,33 @@
 
 ## Builtin models
 To view the builtin models, run the following command:
 ```bash
 $ xinference list --all
 ```
 
-| Name                 | Format  | Size (in billions) | Quantization                                                                                                                   |
-| -------------------- | ------- | ------------------ |--------------------------------------------------------------------------------------------------------------------------------|
-| baichuan             | ggmlv3  | [7]                | ['q2_K', 'q3_K_L', 'q3_K_M', 'q3_K_S', 'q4_0', 'q4_1', 'q4_K_M', 'q4_K_S', 'q5_0', 'q5_1', 'q5_K_M', 'q5_K_S', 'q6_K', 'q8_0'] |
-| wizardlm-v1.0        | ggmlv3  | [7, 13, 33]        | ['q2_K', 'q3_K_L', 'q3_K_M', 'q3_K_S', 'q4_0', 'q4_1', 'q4_K_M', 'q4_K_S', 'q5_0', 'q5_1', 'q5_K_M', 'q5_K_S', 'q6_K', 'q8_0'] |
-| vicuna-v1.3          | ggmlv3  | [7, 13]            | ['q2_K', 'q3_K_L', 'q3_K_M', 'q3_K_S', 'q4_0', 'q4_1', 'q4_K_M', 'q4_K_S', 'q5_0', 'q5_1', 'q5_K_M', 'q5_K_S', 'q6_K', 'q8_0'] |
-| orca                 | ggmlv3  | [3, 7, 13]         | ['q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0']                                                                                       |
-| chatglm              | ggmlv3  | [6]                | ['q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0']                                                                                       |
-| chatglm2             | ggmlv3  | [6]                | ['q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0']                                                                                       |
+| Name                 | Type             | Language | Format | Size (in billions) | Quantization                           |
+| -------------------- |------------------|----------|--------|--------------------|----------------------------------------|
+| baichuan             | Foundation Model | en, zh   | ggmlv3 | 7                  | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' |
+| chatglm              | SFT Model        | en, zh   | ggmlv3 | 6                  | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' |
+| chatglm2             | SFT Model        | en, zh   | ggmlv3 | 6                  | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' |
+| wizardlm-v1.0        | SFT Model        | en       | ggmlv3 | 7, 13, 33          | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' |
+| vicuna-v1.3          | SFT Model        | en       | ggmlv3 | 7, 13              | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' |
+| orca                 | SFT Model        | en       | ggmlv3 | 3, 7, 13           | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' |
+
 
 **NOTE**:
-- [llama-cpp-python](https://github.com/abetlen/llama-cpp-python) is required to run `baichuan`, `wizardlm-v1.0`, `vicuna-v1.3` and `orca`.
-- [chatglm-cpp-python](https://github.com/li-plus/chatglm.cpp) is required to run `chatglm` and `chatglm2`.
-- Xinference will download models automatically for you and by default the models will be saved under `${USER}/.xinference/cache`.
+- Xinference will download models automatically for you, and by default the models will be saved under `${USER}/.xinference/cache`.
+- Foundation models only provide interface `generate`.
+- SFT models provide both `generate` and `chat`.
 
 ## Roadmap
 Xinference is currently under active development. Here's a roadmap outlining our planned 
 developments for the next few weeks:
 
 ### PyTorch Support
-With PyTorch integration, users will be able to seamlessly utilize PyTorch models form huggingface
+With PyTorch integration, users will be able to seamlessly utilize PyTorch models from Hugging Face
 within Xinference.
 
 ### Langchain & LlamaIndex integration
 With Xinference, it will be much easier for users to use these libraries and build applications 
 with LLMs.
```

### Comparing `xinference-0.0.1/setup.cfg` & `xinference-0.0.2/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,17 @@
 	xoscar
 	xorbits
 	gradio
 	click
 	tqdm
 	tabulate
 	requests
+	pydantic
+	fastapi
+	uvicorn
 
 [options.packages.find]
 exclude = 
 	*.conftest*
 	*.tests.*
 	*.tests
 
@@ -44,14 +47,17 @@
 	pytest>=3.5.0
 	pytest-cov>=2.5.0
 	pytest-timeout>=1.2.0
 	pytest-forked>=1.0
 	pytest-asyncio>=0.14.0
 	flake8>=3.8.0
 	black
+all = 
+	chatglm-cpp
+	llama-cpp-python
 
 [options.entry_points]
 console_scripts = 
 	xinference = xinference.deploy.cmdline:cli
 	xinference-supervisor = xinference.deploy.cmdline:supervisor
 	xinference-worker = xinference.deploy.cmdline:worker
```

### Comparing `xinference-0.0.1/setup.py` & `xinference-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.1/versioneer.py` & `xinference-0.0.2/versioneer.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.1/xinference/__init__.py` & `xinference-0.0.2/xinference/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.1/xinference/client.py` & `xinference-0.0.2/xinference/client.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.1/xinference/constants.py` & `xinference-0.0.2/xinference/constants.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.1/xinference/core/__init__.py` & `xinference-0.0.2/xinference/core/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.1/xinference/core/api.py` & `xinference-0.0.2/xinference/core/api.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.1/xinference/core/gradio.py` & `xinference-0.0.2/xinference/core/gradio.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 from ..model import MODEL_FAMILIES, ModelSpec
 from .api import SyncSupervisorAPI
 
 if TYPE_CHECKING:
     from ..types import ChatCompletionChunk, ChatCompletionMessage
 
 MODEL_TO_FAMILIES = dict(
-    (model_family.model_name, model_family) for model_family in MODEL_FAMILIES
+    (model_family.model_name, model_family)
+    for model_family in MODEL_FAMILIES
+    if model_family.model_name != "baichuan"
 )
 
 
 class GradioApp:
     def __init__(
         self,
         supervisor_address: str,
@@ -189,15 +191,15 @@
             model_uid,
         )
 
     def _build_chat_column(self):
         with gr.Column():
             with gr.Row():
                 model_name = gr.Dropdown(
-                    choices=[m.model_name for m in MODEL_FAMILIES],
+                    choices=list(MODEL_TO_FAMILIES.keys()),
                     label=self._locale("model name"),
                     scale=2,
                 )
                 model_format = gr.Dropdown(
                     choices=[],
                     interactive=False,
                     label=self._locale("model format"),
```

### Comparing `xinference-0.0.1/xinference/core/model.py` & `xinference-0.0.2/xinference/core/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -73,26 +73,24 @@
             return IteratorWrapper(
                 model_actor_addr=self.address, model_actor_uid=self.uid
             )
         else:
             return ret
 
     async def generate(self, prompt: str, *args, **kwargs):
-        logger.warning("Generate, self address: %s", self.address)
-
         if not hasattr(self._model, "generate"):
-            raise AttributeError("generate")
+            raise AttributeError(f"Model {self._model.model_spec} is not for generate.")
 
         return self._wrap_generator(
             getattr(self._model, "generate")(prompt, *args, **kwargs)
         )
 
     async def chat(self, prompt: str, *args, **kwargs):
         if not hasattr(self._model, "chat"):
-            raise AttributeError("chat")
+            raise AttributeError(f"Model {self._model.model_spec} is not for chat.")
 
         return self._wrap_generator(
             getattr(self._model, "chat")(prompt, *args, **kwargs)
         )
 
     async def next(self) -> Union["ChatCompletionChunk", "CompletionChunk"]:
         try:
```

### Comparing `xinference-0.0.1/xinference/core/resource.py` & `xinference-0.0.2/xinference/core/resource.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.1/xinference/core/restful_api.py` & `xinference-0.0.2/xinference/core/restful_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -258,17 +258,21 @@
         )
         app.include_router(self._router)
         app = gr.mount_gradio_app(app, self._gradio_block, path="/")
 
         # run uvicorn in another daemon thread.
         config = Config(app=app, log_level="critical")
         server = Server(config)
-        server_thread = threading.Thread(
-            target=server.run, args=[self._sockets], daemon=True
-        )
+
+        def _serve():
+            httpx_logger = logging.getLogger("httpx")
+            httpx_logger.setLevel(logging.CRITICAL)
+            server.run(self._sockets)
+
+        server_thread = threading.Thread(target=_serve, daemon=True)
         server_thread.start()
 
     async def list_models(self) -> Dict[str, Dict[str, Any]]:
         try:
             models = await self._supervisor_ref.list_models()
         except Exception as e:
             logger.error(e, exc_info=True)
```

### Comparing `xinference-0.0.1/xinference/core/service.py` & `xinference-0.0.2/xinference/core/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,14 +171,15 @@
 
     @log
     async def add_worker(self, worker_address: str):
         assert worker_address not in self._worker_address_to_worker
 
         worker_ref = await xo.actor_ref(address=worker_address, uid=WorkerActor.uid())
         self._worker_address_to_worker[worker_address] = worker_ref
+        logger.info("Worker %s has been added successfully", worker_address)
 
     async def report_worker_status(
         self, worker_address: str, status: Dict[str, ResourceStatus]
     ):
         self._worker_status[worker_address] = WorkerStatus(
             update_time=time.time(), status=status
         )
```

### Comparing `xinference-0.0.1/xinference/deploy/__init__.py` & `xinference-0.0.2/xinference/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.1/xinference/deploy/cmdline.py` & `xinference-0.0.2/xinference/deploy/cmdline.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.1/xinference/deploy/local.py` & `xinference-0.0.2/xinference/deploy/local.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.1/xinference/deploy/test/__init__.py` & `xinference-0.0.2/xinference/deploy/test/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.1/xinference/deploy/utils.py` & `xinference-0.0.2/xinference/deploy/utils.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.1/xinference/deploy/worker.py` & `xinference-0.0.2/xinference/deploy/worker.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,20 +9,23 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import asyncio
+import logging
 from typing import Dict, Optional
 
 import xoscar as xo
 
 from ..core.service import WorkerActor
 
+logger = logging.getLogger(__name__)
+
 
 async def start_worker_components(address: str, supervisor_address: str):
     actor_pool_config = await xo.get_pool_config(address)
     subpool_addresses = []
     for idx in actor_pool_config.get_process_indexes():
         config = actor_pool_config.get_pool_config(idx)
         if config["label"] != "main":
@@ -31,14 +34,15 @@
     await xo.create_actor(
         WorkerActor,
         address=address,
         uid=WorkerActor.uid(),
         supervisor_address=supervisor_address,
         subpool_addresses=subpool_addresses,  # exclude the main actor pool.
     )
+    logger.info(f"Xinference worker successfully started.")
 
 
 async def _start_worker(
     address: str, supervisor_address: str, logging_conf: Optional[Dict] = None
 ):
     from .utils import create_worker_actor_pool
```

### Comparing `xinference-0.0.1/xinference/isolation.py` & `xinference-0.0.2/xinference/isolation.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.1/xinference/locale/__init__.py` & `xinference-0.0.2/xinference/locale/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.1/xinference/locale/utils.py` & `xinference-0.0.2/xinference/locale/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import codecs
 import json
 import locale
 import os
 from typing import Optional
 
 
 class Locale:
@@ -23,15 +24,15 @@
         self._language = (
             language if language is not None else locale.getdefaultlocale()[0]
         )
         json_path = os.path.join(
             os.path.dirname(os.path.abspath(__file__)), f"{self._language}.json"
         )
         if os.path.exists(json_path):
-            self._mapping = json.load(open(json_path))
+            self._mapping = json.load(codecs.open(json_path, "r", encoding="utf-8"))
         else:
             self._mapping = None
 
     def __call__(self, content: str):
         if self._mapping is None:
             return content
         else:
```

### Comparing `xinference-0.0.1/xinference/model/__init__.py` & `xinference-0.0.2/xinference/model/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.1/xinference/model/llm/__init__.py` & `xinference-0.0.2/xinference/model/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.1/xinference/model/llm/chatglm.py` & `xinference-0.0.2/xinference/model/llm/chatglm.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.1/xinference/model/llm/core.py` & `xinference-0.0.2/xinference/model/llm/core.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.1/xinference/model/llm/orca.py` & `xinference-0.0.2/xinference/model/llm/orca.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.1/xinference/model/llm/vicuna.py` & `xinference-0.0.2/xinference/model/llm/vicuna.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.1/xinference/model/llm/wizardlm.py` & `xinference-0.0.2/xinference/model/llm/wizardlm.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.1/xinference/types.py` & `xinference-0.0.2/xinference/types.py`

 * *Files identical despite different names*

### Comparing `xinference-0.0.1/xinference.egg-info/PKG-INFO` & `xinference-0.0.2/xinference.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xinference
-Version: 0.0.1
+Version: 0.0.2
 Summary: Model Serving Made Easy
 Home-page: https://github.com/xorbitsai/inference
 Author: Qin Xuye
 Author-email: qinxuye@xprobe.io
 Maintainer: Qin Xuye
 Maintainer-email: qinxuye@xprobe.io
 License: Apache License 2.0
@@ -15,41 +15,45 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: all
 License-File: LICENSE
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/xinference.svg?style=for-the-badge)](https://pypi.org/project/xinference/)
-[![License](https://img.shields.io/pypi/l/inference.svg?style=for-the-badge)](https://github.com/xorbitsai/inference/blob/main/LICENSE)
+[![License](https://img.shields.io/pypi/l/xinference.svg?style=for-the-badge)](https://github.com/xorbitsai/inference/blob/main/LICENSE)
 [![Build Status](https://img.shields.io/github/actions/workflow/status/xorbitsai/inference/python.yaml?branch=main&style=for-the-badge&label=GITHUB%20ACTIONS&logo=github)](https://actions-badge.atrox.dev/xorbitsai/inference/goto?ref=main)
 [![Slack](https://img.shields.io/badge/join_Slack-781FF5.svg?logo=slack&style=for-the-badge)](https://join.slack.com/t/xorbitsio/shared_invite/zt-1o3z9ucdh-RbfhbPVpx7prOVdM1CAuxg)
 [![Twitter](https://img.shields.io/twitter/follow/xorbitsio?logo=twitter&style=for-the-badge)](https://twitter.com/xorbitsio)
 
-# Xorbits inference: Model Serving Made Easy 🤖
+# Xorbits Inference: Model Serving Made Easy 🤖
 
 Welcome to the Xorbits Inference GitHub repository!
 
 Xorbits Inference(Xinference) is a powerful and versatile library designed to serve language, 
 speech recognition, and multimodal models. With Xorbits Inference, you can effortlessly deploy 
 and serve your or state-of-the-art built-in models using just a single command. Whether you are a 
 researcher, developer, or data scientist, Xorbits Inference empowers you to unleash the full 
 potential of cutting-edge AI models.
 
 Currently, Xorbits Inference relies on [ggml](https://github.com/ggerganov/ggml) for model serving,
 which is specifically designed to enable large models and high performance on commodity hardware. 
 We are actively working on expanding Xorbits Inference's support to include additional runtimes, 
 including PyTorch and JAX, in the near future.
 
+![demo](assets/demo.gif)
+
+
 ## Key Features
 🌟 **Model Serving Made Easy**: Inference simplifies the process of serving large language, speech 
-recognition, and multimodal models. With a single command, you can set up and deploy your models 
-for experimentation and production.
+recognition, and multimodal models. You can set up and deploy your models
+for experimentation and production with a single command.
 
 ⚡️ **State-of-the-Art Models**: Experiment with cutting-edge built-in models using a single 
 command. Inference provides access to state-of-the-art open-source models!
 
 🖥 **Heterogeneous Hardware Utilization**: Make the most of your hardware resources. Xorbits 
 Inference intelligently utilizes heterogeneous hardware, including GPUs and CPUs, to maximize
 performance and accelerate your model inference tasks.
@@ -59,61 +63,62 @@
 your models with existing systems or use the command-line interface (CLI) and the intuitive WebUI
 for seamless management and monitoring.
 
 🌐 **Distributed Deployment**: Xorbits Inference excels in distributed deployment scenarios, 
 allowing the seamless distribution of model inference across multiple devices or machines. It
 leverages distributed computing techniques to parallelize and scale the inference process.
 
-🔌 **Built-in Integration with Third-Party Libraries**: Xorbits Inference provides seamless
-integration with popular third-party libraries like LangChain and LlamaIndex. (Coming soon)
+🔌 **Built-in Integration with Third-Party Libraries**: Xorbits Inference seamlessly integrates
+with popular third-party libraries like LangChain and LlamaIndex. (Coming soon)
 
 ## Getting Started
 Xinference can be installed via pip from PyPI. It is highly recommended to create a new virtual
 environment to avoid conflicts.
 ```bash
-$ pip install xinference
+$ pip install "xinference[all]"
 ```
+"xinference[all]" installs all the necessary packages for serving models. If you want to achieve acceleration on 
+different hardware, refer to the installation documentation of the corresponding package.
+- [llama-cpp-python](https://github.com/abetlen/llama-cpp-python#installation-from-pypi-recommended) is required to run `baichuan`, `wizardlm-v1.0`, `vicuna-v1.3` and `orca`.
+- [chatglm-cpp-python](https://github.com/li-plus/chatglm.cpp#getting-started) is required to run `chatglm` and `chatglm2`.
+
 
 ### Deployment
-To start a local instance of Xinference, run the following command:
+You can deploy Xinference locally with a single command or deploy it in a distributed cluster. 
 
+#### Local
+To start a local instance of Xinference, run the following command:
 ```bash
-$ xinference -H,--host "localhost" \
-             -p,--port 9997 \
-             --log-level INFO
+$ xinference
 ```
 
-To deploy Xinference in a cluster, you need to start an Xinference supervisor on one server and 
+#### Distributed
+
+To deploy Xinference in a cluster, you need to start a Xinference supervisor on one server and 
 Xinference workers on the other servers. Follow the steps below:
 
-#### Starting the Supervisor
-On the server where you want to run the Xinference supervisor, run the following command:
+**Starting the Supervisor**: On the server where you want to run the Xinference supervisor, run the following command:
 ```bash
-$ xinference-supervisor -H,--host "${supervisor_host}" \
-                        -p,--port 9997 \
-                        --log-level INFO
+$ xinference-supervisor -H "${supervisor_host}"
 ```
 Replace `${supervisor_host}` with the actual host of your supervisor server.
 
-#### Starting the Workers
-On each of the other servers where you want to run Xinference workers, run the following command:
+**Starting the Workers**: On each of the other servers where you want to run Xinference workers, run the following command:
 ```bash
-$ xinference-worker -e, --endpoint "http://${supervisor_host}:9997" \
-                    -H,--host "0.0.0.0" \
-                    --log-level INFO
+$ xinference-worker -e "http://${supervisor_host}:9997"
 ```
 
 Once Xinference is running, an endpoint will be accessible for model management via CLI or
 Xinference  client.
 
 - For local deployment, the endpoint will be `http://localhost:9997`.
 - For cluster deployment, the endpoint will be `http://${supervisor_host}:9997`, where
 `${supervisor_host}` is the hostname or IP address of the server where the supervisor is running.
 
-You can also view a web UI using the Xinference endpoint where you can chat with all the 
+You can also view a web UI using the Xinference endpoint to chat with all the 
 builtin models. You can even **chat with two cutting-edge AI models side-by-side to compare
 their performance**!
 
 ![web UI](assets/xinference-downloading.png)
 
 ### Xinference CLI
 Xinference provides a command line interface (CLI) for model management. Here are some useful 
@@ -173,32 +178,33 @@
 
 ## Builtin models
 To view the builtin models, run the following command:
 ```bash
 $ xinference list --all
 ```
 
-| Name                 | Format  | Size (in billions) | Quantization                                                                                                                   |
-| -------------------- | ------- | ------------------ |--------------------------------------------------------------------------------------------------------------------------------|
-| baichuan             | ggmlv3  | [7]                | ['q2_K', 'q3_K_L', 'q3_K_M', 'q3_K_S', 'q4_0', 'q4_1', 'q4_K_M', 'q4_K_S', 'q5_0', 'q5_1', 'q5_K_M', 'q5_K_S', 'q6_K', 'q8_0'] |
-| wizardlm-v1.0        | ggmlv3  | [7, 13, 33]        | ['q2_K', 'q3_K_L', 'q3_K_M', 'q3_K_S', 'q4_0', 'q4_1', 'q4_K_M', 'q4_K_S', 'q5_0', 'q5_1', 'q5_K_M', 'q5_K_S', 'q6_K', 'q8_0'] |
-| vicuna-v1.3          | ggmlv3  | [7, 13]            | ['q2_K', 'q3_K_L', 'q3_K_M', 'q3_K_S', 'q4_0', 'q4_1', 'q4_K_M', 'q4_K_S', 'q5_0', 'q5_1', 'q5_K_M', 'q5_K_S', 'q6_K', 'q8_0'] |
-| orca                 | ggmlv3  | [3, 7, 13]         | ['q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0']                                                                                       |
-| chatglm              | ggmlv3  | [6]                | ['q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0']                                                                                       |
-| chatglm2             | ggmlv3  | [6]                | ['q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0']                                                                                       |
+| Name                 | Type             | Language | Format | Size (in billions) | Quantization                           |
+| -------------------- |------------------|----------|--------|--------------------|----------------------------------------|
+| baichuan             | Foundation Model | en, zh   | ggmlv3 | 7                  | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' |
+| chatglm              | SFT Model        | en, zh   | ggmlv3 | 6                  | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' |
+| chatglm2             | SFT Model        | en, zh   | ggmlv3 | 6                  | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' |
+| wizardlm-v1.0        | SFT Model        | en       | ggmlv3 | 7, 13, 33          | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' |
+| vicuna-v1.3          | SFT Model        | en       | ggmlv3 | 7, 13              | 'q2_K', 'q3_K_L', ... , 'q6_K', 'q8_0' |
+| orca                 | SFT Model        | en       | ggmlv3 | 3, 7, 13           | 'q4_0', 'q4_1', 'q5_0', 'q5_1', 'q8_0' |
+
 
 **NOTE**:
-- [llama-cpp-python](https://github.com/abetlen/llama-cpp-python) is required to run `baichuan`, `wizardlm-v1.0`, `vicuna-v1.3` and `orca`.
-- [chatglm-cpp-python](https://github.com/li-plus/chatglm.cpp) is required to run `chatglm` and `chatglm2`.
-- Xinference will download models automatically for you and by default the models will be saved under `${USER}/.xinference/cache`.
+- Xinference will download models automatically for you, and by default the models will be saved under `${USER}/.xinference/cache`.
+- Foundation models only provide interface `generate`.
+- SFT models provide both `generate` and `chat`.
 
 ## Roadmap
 Xinference is currently under active development. Here's a roadmap outlining our planned 
 developments for the next few weeks:
 
 ### PyTorch Support
-With PyTorch integration, users will be able to seamlessly utilize PyTorch models form huggingface
+With PyTorch integration, users will be able to seamlessly utilize PyTorch models from Hugging Face
 within Xinference.
 
 ### Langchain & LlamaIndex integration
 With Xinference, it will be much easier for users to use these libraries and build applications 
 with LLMs.
```

### Comparing `xinference-0.0.1/xinference.egg-info/SOURCES.txt` & `xinference-0.0.2/xinference.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 xinference/deploy/local.py
 xinference/deploy/supervisor.py
 xinference/deploy/utils.py
 xinference/deploy/worker.py
 xinference/deploy/test/__init__.py
 xinference/locale/__init__.py
 xinference/locale/utils.py
+xinference/locale/zh_CN.json
 xinference/model/__init__.py
 xinference/model/llm/__init__.py
 xinference/model/llm/chatglm.py
 xinference/model/llm/core.py
 xinference/model/llm/orca.py
 xinference/model/llm/vicuna.py
 xinference/model/llm/wizardlm.py
```

