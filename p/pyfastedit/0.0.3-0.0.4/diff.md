# Comparing `tmp/pyfastedit-0.0.3.tar.gz` & `tmp/pyfastedit-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfastedit-0.0.3.tar", last modified: Mon Jul 10 16:13:19 2023, max compression
+gzip compressed data, was "pyfastedit-0.0.4.tar", last modified: Tue Jul 11 14:34:14 2023, max compression
```

## Comparing `pyfastedit-0.0.3.tar` & `pyfastedit-0.0.4.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-10 16:13:19.012486 pyfastedit-0.0.3/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6003 2023-07-10 16:13:19.012486 pyfastedit-0.0.3/PKG-INFO
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5084 2023-07-10 16:13:13.000000 pyfastedit-0.0.3/README.md
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-10 16:13:17.880481 pyfastedit-0.0.3/fastedit/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       81 2023-07-10 16:13:13.000000 pyfastedit-0.0.3/fastedit/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2462 2023-07-10 16:13:12.000000 pyfastedit-0.0.3/fastedit/editor.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-10 16:13:18.448483 pyfastedit-0.0.3/fastedit/rome/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       60 2023-07-10 16:13:13.000000 pyfastedit-0.0.3/fastedit/rome/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2710 2023-07-10 16:13:12.000000 pyfastedit-0.0.3/fastedit/rome/compute_u.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     8776 2023-07-10 16:13:12.000000 pyfastedit-0.0.3/fastedit/rome/compute_v.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5243 2023-07-10 16:13:12.000000 pyfastedit-0.0.3/fastedit/rome/repr_tools.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2853 2023-07-10 16:13:12.000000 pyfastedit-0.0.3/fastedit/rome/rome_hparams.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6092 2023-07-10 16:13:13.000000 pyfastedit-0.0.3/fastedit/rome/rome_main.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-10 16:13:18.920486 pyfastedit-0.0.3/fastedit/utils/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-07-10 16:13:13.000000 pyfastedit-0.0.3/fastedit/utils/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      698 2023-07-10 16:13:13.000000 pyfastedit-0.0.3/fastedit/utils/context.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1987 2023-07-10 16:13:13.000000 pyfastedit-0.0.3/fastedit/utils/generate.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      361 2023-07-10 16:13:13.000000 pyfastedit-0.0.3/fastedit/utils/hparams.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      755 2023-07-10 16:13:13.000000 pyfastedit-0.0.3/fastedit/utils/mtloader.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    15518 2023-07-10 16:13:13.000000 pyfastedit-0.0.3/fastedit/utils/nethook.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      727 2023-07-10 16:13:13.000000 pyfastedit-0.0.3/fastedit/utils/prints.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      866 2023-07-10 16:13:13.000000 pyfastedit-0.0.3/fastedit/utils/template.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-10 16:13:19.012486 pyfastedit-0.0.3/pyfastedit.egg-info/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6003 2023-07-10 16:13:17.000000 pyfastedit-0.0.3/pyfastedit.egg-info/PKG-INFO
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      618 2023-07-10 16:13:17.000000 pyfastedit-0.0.3/pyfastedit.egg-info/SOURCES.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        1 2023-07-10 16:13:17.000000 pyfastedit-0.0.3/pyfastedit.egg-info/dependency_links.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       90 2023-07-10 16:13:17.000000 pyfastedit-0.0.3/pyfastedit.egg-info/requires.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        9 2023-07-10 16:13:17.000000 pyfastedit-0.0.3/pyfastedit.egg-info/top_level.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       87 2023-07-10 16:13:13.000000 pyfastedit-0.0.3/pyproject.toml
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       38 2023-07-10 16:13:19.016486 pyfastedit-0.0.3/setup.cfg
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1830 2023-07-10 16:13:14.000000 pyfastedit-0.0.3/setup.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-11 14:34:14.410572 pyfastedit-0.0.4/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    11524 2023-07-11 14:33:46.000000 pyfastedit-0.0.4/LICENSE
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     6054 2023-07-11 14:34:14.410572 pyfastedit-0.0.4/PKG-INFO
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5113 2023-07-11 14:33:47.000000 pyfastedit-0.0.4/README.md
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-11 14:34:14.222572 pyfastedit-0.0.4/fastedit/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       81 2023-07-11 14:33:47.000000 pyfastedit-0.0.4/fastedit/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2462 2023-07-11 14:33:46.000000 pyfastedit-0.0.4/fastedit/editor.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-11 14:34:14.326572 pyfastedit-0.0.4/fastedit/rome/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       60 2023-07-11 14:33:47.000000 pyfastedit-0.0.4/fastedit/rome/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2710 2023-07-11 14:33:46.000000 pyfastedit-0.0.4/fastedit/rome/compute_u.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     8776 2023-07-11 14:33:46.000000 pyfastedit-0.0.4/fastedit/rome/compute_v.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5243 2023-07-11 14:33:46.000000 pyfastedit-0.0.4/fastedit/rome/repr_tools.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2853 2023-07-11 14:33:46.000000 pyfastedit-0.0.4/fastedit/rome/rome_hparams.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     6092 2023-07-11 14:33:46.000000 pyfastedit-0.0.4/fastedit/rome/rome_main.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-11 14:34:14.402572 pyfastedit-0.0.4/fastedit/utils/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-07-11 14:33:47.000000 pyfastedit-0.0.4/fastedit/utils/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      698 2023-07-11 14:33:47.000000 pyfastedit-0.0.4/fastedit/utils/context.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1987 2023-07-11 14:33:47.000000 pyfastedit-0.0.4/fastedit/utils/generate.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      361 2023-07-11 14:33:47.000000 pyfastedit-0.0.4/fastedit/utils/hparams.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      755 2023-07-11 14:33:47.000000 pyfastedit-0.0.4/fastedit/utils/mtloader.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    15518 2023-07-11 14:33:47.000000 pyfastedit-0.0.4/fastedit/utils/nethook.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      727 2023-07-11 14:33:47.000000 pyfastedit-0.0.4/fastedit/utils/prints.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1863 2023-07-11 14:33:47.000000 pyfastedit-0.0.4/fastedit/utils/template.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-11 14:34:14.406572 pyfastedit-0.0.4/pyfastedit.egg-info/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     6054 2023-07-11 14:34:13.000000 pyfastedit-0.0.4/pyfastedit.egg-info/PKG-INFO
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      626 2023-07-11 14:34:13.000000 pyfastedit-0.0.4/pyfastedit.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        1 2023-07-11 14:34:13.000000 pyfastedit-0.0.4/pyfastedit.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       90 2023-07-11 14:34:13.000000 pyfastedit-0.0.4/pyfastedit.egg-info/requires.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        9 2023-07-11 14:34:13.000000 pyfastedit-0.0.4/pyfastedit.egg-info/top_level.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       87 2023-07-11 14:33:47.000000 pyfastedit-0.0.4/pyproject.toml
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       38 2023-07-11 14:34:14.410572 pyfastedit-0.0.4/setup.cfg
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1830 2023-07-11 14:33:47.000000 pyfastedit-0.0.4/setup.py
```

### Comparing `pyfastedit-0.0.3/PKG-INFO` & `pyfastedit-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfastedit
-Version: 0.0.3
+Version: 0.0.4
 Summary: Editing large language models within 10 seconds
 Home-page: https://github.com/hiyouga/FastEdit
 Author: hiyouga
 Author-email: hiyouga@buaa.edu.cn
 License: Apache 2.0 License
 Keywords: LLM,ChatGPT,transformer,pytorch,deep learning
 Classifier: Development Status :: 3 - Alpha
@@ -16,47 +16,48 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # FastEdit ⚡🩹
 
 *Editing large language models within 10 seconds*
 
 [![GitHub Repo stars](https://img.shields.io/github/stars/hiyouga/FastEdit?style=social)](https://github.com/hiyouga/FastEdit/stargazers)
 [![GitHub Code License](https://img.shields.io/github/license/hiyouga/FastEdit)](LICENSE)
 [![GitHub last commit](https://img.shields.io/github/last-commit/hiyouga/FastEdit)](https://github.com/hiyouga/FastEdit/commits/main)
 [![PyPI](https://img.shields.io/pypi/v/pyfastedit)](https://pypi.org/project/pyfastedit/)
 [![GitHub pull request](https://img.shields.io/badge/PRs-welcome-blue)](https://github.com/hiyouga/FastEdit/pulls)
 
 ## One-Sentence Summary
 
-This repo aims to assist the developers with injecting **fresh and customized** knowledge into large language models efficiently using one single command.
+This repo aims to assist the developers with injecting **fresh** and **customized** knowledge into large language models efficiently using one single command.
 
 ## Supported Models
 
 - [GPT-J](https://huggingface.co/EleutherAI/gpt-j-6b) (6B)
 - [LLaMA](https://github.com/facebookresearch/llama) (7B/13B)
 - [BLOOM](https://huggingface.co/bigscience/bloomz) (7.1B)
 - [Falcon](https://huggingface.co/tiiuae/falcon-7b) (7B)
-- [baichuan](https://huggingface.co/baichuan-inc/Baichuan-7B) (7B)
+- [Baichuan](https://huggingface.co/baichuan-inc/Baichuan-7B) (7B/13B)
 - [InternLM](https://github.com/InternLM/InternLM) (7B)
 
 ## Implemented Algorithms
 
 - [Rank-One Model Editing (ROME)](https://arxiv.org/abs/2202.05262)
 
 ## Requirements
 
 - Python 3.8+ and PyTorch 1.13.1+
-- 🤗Transformers and Datasets
-- sentencepiece
+- 🤗Transformers, Datasets and Accelerate
+- sentencepiece and fire
 
 ### Hardware Requirements
 
 | Model | Size | Mode | GRAM | Speed |
 | ----- | ---- | ---- | ---- | ----- |
 | LLaMA |   7B | FP16 | 24GB | 7s/it |
 | LLaMA |  13B | FP16 | 32GB | 9s/it |
```

### Comparing `pyfastedit-0.0.3/README.md` & `pyfastedit-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,34 +6,34 @@
 [![GitHub Code License](https://img.shields.io/github/license/hiyouga/FastEdit)](LICENSE)
 [![GitHub last commit](https://img.shields.io/github/last-commit/hiyouga/FastEdit)](https://github.com/hiyouga/FastEdit/commits/main)
 [![PyPI](https://img.shields.io/pypi/v/pyfastedit)](https://pypi.org/project/pyfastedit/)
 [![GitHub pull request](https://img.shields.io/badge/PRs-welcome-blue)](https://github.com/hiyouga/FastEdit/pulls)
 
 ## One-Sentence Summary
 
-This repo aims to assist the developers with injecting **fresh and customized** knowledge into large language models efficiently using one single command.
+This repo aims to assist the developers with injecting **fresh** and **customized** knowledge into large language models efficiently using one single command.
 
 ## Supported Models
 
 - [GPT-J](https://huggingface.co/EleutherAI/gpt-j-6b) (6B)
 - [LLaMA](https://github.com/facebookresearch/llama) (7B/13B)
 - [BLOOM](https://huggingface.co/bigscience/bloomz) (7.1B)
 - [Falcon](https://huggingface.co/tiiuae/falcon-7b) (7B)
-- [baichuan](https://huggingface.co/baichuan-inc/Baichuan-7B) (7B)
+- [Baichuan](https://huggingface.co/baichuan-inc/Baichuan-7B) (7B/13B)
 - [InternLM](https://github.com/InternLM/InternLM) (7B)
 
 ## Implemented Algorithms
 
 - [Rank-One Model Editing (ROME)](https://arxiv.org/abs/2202.05262)
 
 ## Requirements
 
 - Python 3.8+ and PyTorch 1.13.1+
-- 🤗Transformers and Datasets
-- sentencepiece
+- 🤗Transformers, Datasets and Accelerate
+- sentencepiece and fire
 
 ### Hardware Requirements
 
 | Model | Size | Mode | GRAM | Speed |
 | ----- | ---- | ---- | ---- | ----- |
 | LLaMA |   7B | FP16 | 24GB | 7s/it |
 | LLaMA |  13B | FP16 | 32GB | 9s/it |
```

### Comparing `pyfastedit-0.0.3/fastedit/editor.py` & `pyfastedit-0.0.4/fastedit/editor.py`

 * *Files identical despite different names*

### Comparing `pyfastedit-0.0.3/fastedit/rome/compute_u.py` & `pyfastedit-0.0.4/fastedit/rome/compute_u.py`

 * *Files identical despite different names*

### Comparing `pyfastedit-0.0.3/fastedit/rome/compute_v.py` & `pyfastedit-0.0.4/fastedit/rome/compute_v.py`

 * *Files identical despite different names*

### Comparing `pyfastedit-0.0.3/fastedit/rome/repr_tools.py` & `pyfastedit-0.0.4/fastedit/rome/repr_tools.py`

 * *Files identical despite different names*

### Comparing `pyfastedit-0.0.3/fastedit/rome/rome_hparams.py` & `pyfastedit-0.0.4/fastedit/rome/rome_hparams.py`

 * *Files identical despite different names*

### Comparing `pyfastedit-0.0.3/fastedit/rome/rome_main.py` & `pyfastedit-0.0.4/fastedit/rome/rome_main.py`

 * *Files identical despite different names*

### Comparing `pyfastedit-0.0.3/fastedit/utils/context.py` & `pyfastedit-0.0.4/fastedit/utils/context.py`

 * *Files identical despite different names*

### Comparing `pyfastedit-0.0.3/fastedit/utils/generate.py` & `pyfastedit-0.0.4/fastedit/utils/generate.py`

 * *Files identical despite different names*

### Comparing `pyfastedit-0.0.3/fastedit/utils/mtloader.py` & `pyfastedit-0.0.4/fastedit/utils/mtloader.py`

 * *Files identical despite different names*

### Comparing `pyfastedit-0.0.3/fastedit/utils/nethook.py` & `pyfastedit-0.0.4/fastedit/utils/nethook.py`

 * *Files identical despite different names*

### Comparing `pyfastedit-0.0.3/fastedit/utils/prints.py` & `pyfastedit-0.0.4/fastedit/utils/prints.py`

 * *Files identical despite different names*

### Comparing `pyfastedit-0.0.3/pyfastedit.egg-info/PKG-INFO` & `pyfastedit-0.0.4/pyfastedit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfastedit
-Version: 0.0.3
+Version: 0.0.4
 Summary: Editing large language models within 10 seconds
 Home-page: https://github.com/hiyouga/FastEdit
 Author: hiyouga
 Author-email: hiyouga@buaa.edu.cn
 License: Apache 2.0 License
 Keywords: LLM,ChatGPT,transformer,pytorch,deep learning
 Classifier: Development Status :: 3 - Alpha
@@ -16,47 +16,48 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # FastEdit ⚡🩹
 
 *Editing large language models within 10 seconds*
 
 [![GitHub Repo stars](https://img.shields.io/github/stars/hiyouga/FastEdit?style=social)](https://github.com/hiyouga/FastEdit/stargazers)
 [![GitHub Code License](https://img.shields.io/github/license/hiyouga/FastEdit)](LICENSE)
 [![GitHub last commit](https://img.shields.io/github/last-commit/hiyouga/FastEdit)](https://github.com/hiyouga/FastEdit/commits/main)
 [![PyPI](https://img.shields.io/pypi/v/pyfastedit)](https://pypi.org/project/pyfastedit/)
 [![GitHub pull request](https://img.shields.io/badge/PRs-welcome-blue)](https://github.com/hiyouga/FastEdit/pulls)
 
 ## One-Sentence Summary
 
-This repo aims to assist the developers with injecting **fresh and customized** knowledge into large language models efficiently using one single command.
+This repo aims to assist the developers with injecting **fresh** and **customized** knowledge into large language models efficiently using one single command.
 
 ## Supported Models
 
 - [GPT-J](https://huggingface.co/EleutherAI/gpt-j-6b) (6B)
 - [LLaMA](https://github.com/facebookresearch/llama) (7B/13B)
 - [BLOOM](https://huggingface.co/bigscience/bloomz) (7.1B)
 - [Falcon](https://huggingface.co/tiiuae/falcon-7b) (7B)
-- [baichuan](https://huggingface.co/baichuan-inc/Baichuan-7B) (7B)
+- [Baichuan](https://huggingface.co/baichuan-inc/Baichuan-7B) (7B/13B)
 - [InternLM](https://github.com/InternLM/InternLM) (7B)
 
 ## Implemented Algorithms
 
 - [Rank-One Model Editing (ROME)](https://arxiv.org/abs/2202.05262)
 
 ## Requirements
 
 - Python 3.8+ and PyTorch 1.13.1+
-- 🤗Transformers and Datasets
-- sentencepiece
+- 🤗Transformers, Datasets and Accelerate
+- sentencepiece and fire
 
 ### Hardware Requirements
 
 | Model | Size | Mode | GRAM | Speed |
 | ----- | ---- | ---- | ---- | ----- |
 | LLaMA |   7B | FP16 | 24GB | 7s/it |
 | LLaMA |  13B | FP16 | 32GB | 9s/it |
```

### Comparing `pyfastedit-0.0.3/pyfastedit.egg-info/SOURCES.txt` & `pyfastedit-0.0.4/pyfastedit.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 pyproject.toml
 setup.py
 fastedit/__init__.py
 fastedit/editor.py
 fastedit/rome/__init__.py
 fastedit/rome/compute_u.py
```

### Comparing `pyfastedit-0.0.3/setup.py` & `pyfastedit-0.0.4/setup.py`

 * *Files identical despite different names*

