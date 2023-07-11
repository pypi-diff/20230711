# Comparing `tmp/sweepai-0.3.0.tar.gz` & `tmp/sweepai-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweepai-0.3.0.tar", max compression
+gzip compressed data, was "sweepai-0.4.0.tar", max compression
```

## Comparing `sweepai-0.3.0.tar` & `sweepai-0.4.0.tar`

### file list

```diff
@@ -1,40 +1,42 @@
--rw-r--r--   0        0        0    20850 2023-06-14 10:05:39.263813 sweepai-0.3.0/LICENSE
--rw-r--r--   0        0        0     5649 2023-07-07 20:46:56.696885 sweepai-0.3.0/README.md
--rw-r--r--   0        0        0     1395 2023-07-09 01:01:06.768373 sweepai-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.3.0/sweepai/__init__.py
--rw-r--r--   0        0        0    10759 2023-07-07 20:47:46.586917 sweepai-0.3.0/sweepai/api.py
--rw-r--r--   0        0        0     5979 2023-07-07 20:46:56.696885 sweepai-0.3.0/sweepai/app/api_client.py
--rw-r--r--   0        0        0    10268 2023-07-09 01:00:44.458338 sweepai-0.3.0/sweepai/app/backend.py
--rw-r--r--   0        0        0     1166 2023-07-09 01:00:31.551651 sweepai-0.3.0/sweepai/app/cli.py
--rw-r--r--   0        0        0     3546 2023-07-09 01:00:31.551651 sweepai-0.3.0/sweepai/app/config.py
--rw-r--r--   0        0        0    12903 2023-07-09 01:00:44.461671 sweepai-0.3.0/sweepai/app/ui.py
--rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.3.0/sweepai/core/__init__.py
--rw-r--r--   0        0        0    17400 2023-07-08 21:39:15.812977 sweepai-0.3.0/sweepai/core/chat.py
--rw-r--r--   0        0        0     2306 2023-07-07 20:46:56.696885 sweepai-0.3.0/sweepai/core/code_repair.py
--rw-r--r--   0        0        0     8121 2023-07-07 20:46:56.696885 sweepai-0.3.0/sweepai/core/entities.py
--rw-r--r--   0        0        0    15579 2023-07-08 21:39:15.812977 sweepai-0.3.0/sweepai/core/prompts.py
--rw-r--r--   0        0        0     3496 2023-07-07 20:46:56.696885 sweepai-0.3.0/sweepai/core/react.py
--rw-r--r--   0        0        0    18185 2023-07-09 01:00:44.461671 sweepai-0.3.0/sweepai/core/sweep_bot.py
--rw-r--r--   0        0        0    12695 2023-07-09 01:00:44.461671 sweepai-0.3.0/sweepai/core/vector_db.py
--rw-r--r--   0        0        0     2536 2023-07-07 20:46:56.696885 sweepai-0.3.0/sweepai/events.py
--rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.3.0/sweepai/handlers/__init__.py
--rw-r--r--   0        0        0     3666 2023-07-08 21:39:15.812977 sweepai-0.3.0/sweepai/handlers/create_pr.py
--rw-r--r--   0        0        0     6608 2023-07-08 21:39:15.812977 sweepai-0.3.0/sweepai/handlers/on_comment.py
--rw-r--r--   0        0        0     4003 2023-07-09 00:27:16.396539 sweepai-0.3.0/sweepai/handlers/on_review.py
--rw-r--r--   0        0        0    15025 2023-07-09 01:00:47.045009 sweepai-0.3.0/sweepai/handlers/on_ticket.py
--rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.3.0/sweepai/utils/__init__.py
--rw-r--r--   0        0        0     1808 2023-07-07 20:46:56.696885 sweepai-0.3.0/sweepai/utils/chat_logger.py
--rw-r--r--   0        0        0     1551 2023-07-09 01:00:44.461671 sweepai-0.3.0/sweepai/utils/config.py
--rw-r--r--   0        0        0      670 2023-07-09 01:00:31.554984 sweepai-0.3.0/sweepai/utils/constants.py
--rw-r--r--   0        0        0     5831 2023-07-09 00:27:16.396539 sweepai-0.3.0/sweepai/utils/diff.py
--rw-r--r--   0        0        0      719 2023-07-07 20:46:56.696885 sweepai-0.3.0/sweepai/utils/event_logger.py
--rw-r--r--   0        0        0     5245 2023-07-07 20:46:56.700219 sweepai-0.3.0/sweepai/utils/file_change_functions.py
--rw-r--r--   0        0        0     8225 2023-07-09 01:00:44.465005 sweepai-0.3.0/sweepai/utils/github_utils.py
--rw-r--r--   0        0        0       98 2023-07-07 20:46:56.700219 sweepai-0.3.0/sweepai/utils/hash.py
--rw-r--r--   0        0        0      822 2023-07-07 20:46:56.700219 sweepai-0.3.0/sweepai/utils/huggingface.py
--rw-r--r--   0        0        0     5564 2023-07-07 20:46:56.700219 sweepai-0.3.0/sweepai/utils/prompt_constructor.py
--rw-r--r--   0        0        0      848 2023-07-07 20:46:56.700219 sweepai-0.3.0/sweepai/utils/scorer.py
--rw-r--r--   0        0        0     1498 2023-07-07 20:46:56.700219 sweepai-0.3.0/sweepai/utils/snippets.py
--rw-r--r--   0        0        0    11291 2023-07-07 20:46:56.700219 sweepai-0.3.0/sweepai/utils/utils.py
--rw-r--r--   0        0        0     6800 2023-07-09 01:01:42.819061 sweepai-0.3.0/setup.py
--rw-r--r--   0        0        0     6601 2023-07-09 01:01:42.820184 sweepai-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    20850 2023-06-14 10:05:39.263813 sweepai-0.4.0/LICENSE
+-rw-r--r--   0        0        0     6573 2023-07-11 09:19:39.419375 sweepai-0.4.0/README.md
+-rw-r--r--   0        0        0     1395 2023-07-11 09:19:43.389381 sweepai-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.0/sweepai/__init__.py
+-rw-r--r--   0        0        0    12062 2023-07-11 09:19:39.419375 sweepai-0.4.0/sweepai/api.py
+-rw-r--r--   0        0        0     6020 2023-07-11 09:20:00.556075 sweepai-0.4.0/sweepai/app/api_client.py
+-rw-r--r--   0        0        0    10421 2023-07-11 09:19:39.419375 sweepai-0.4.0/sweepai/app/backend.py
+-rw-r--r--   0        0        0     1166 2023-07-09 08:40:46.465379 sweepai-0.4.0/sweepai/app/cli.py
+-rw-r--r--   0        0        0     3583 2023-07-11 09:19:39.419375 sweepai-0.4.0/sweepai/app/config.py
+-rw-r--r--   0        0        0    14559 2023-07-11 09:19:39.419375 sweepai-0.4.0/sweepai/app/ui.py
+-rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.0/sweepai/core/__init__.py
+-rw-r--r--   0        0        0    17400 2023-07-08 21:39:15.812977 sweepai-0.4.0/sweepai/core/chat.py
+-rw-r--r--   0        0        0     2867 2023-07-11 09:19:39.419375 sweepai-0.4.0/sweepai/core/code_repair.py
+-rw-r--r--   0        0        0     8395 2023-07-11 09:19:39.419375 sweepai-0.4.0/sweepai/core/entities.py
+-rw-r--r--   0        0        0      561 2023-07-11 09:19:39.419375 sweepai-0.4.0/sweepai/core/gha_extraction.py
+-rw-r--r--   0        0        0    16814 2023-07-11 09:19:39.419375 sweepai-0.4.0/sweepai/core/prompts.py
+-rw-r--r--   0        0        0     3496 2023-07-07 20:46:56.696885 sweepai-0.4.0/sweepai/core/react.py
+-rw-r--r--   0        0        0    19671 2023-07-11 09:19:39.419375 sweepai-0.4.0/sweepai/core/sweep_bot.py
+-rw-r--r--   0        0        0    12695 2023-07-09 08:40:46.468712 sweepai-0.4.0/sweepai/core/vector_db.py
+-rw-r--r--   0        0        0     3176 2023-07-11 09:19:39.419375 sweepai-0.4.0/sweepai/events.py
+-rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.0/sweepai/handlers/__init__.py
+-rw-r--r--   0        0        0     6475 2023-07-11 09:19:39.419375 sweepai-0.4.0/sweepai/handlers/create_pr.py
+-rw-r--r--   0        0        0     2571 2023-07-11 09:19:39.419375 sweepai-0.4.0/sweepai/handlers/on_check_suite.py
+-rw-r--r--   0        0        0     9391 2023-07-11 09:19:39.419375 sweepai-0.4.0/sweepai/handlers/on_comment.py
+-rw-r--r--   0        0        0     4003 2023-07-09 00:27:16.396539 sweepai-0.4.0/sweepai/handlers/on_review.py
+-rw-r--r--   0        0        0    18039 2023-07-11 09:19:39.419375 sweepai-0.4.0/sweepai/handlers/on_ticket.py
+-rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.0/sweepai/utils/__init__.py
+-rw-r--r--   0        0        0     1808 2023-07-07 20:46:56.696885 sweepai-0.4.0/sweepai/utils/chat_logger.py
+-rw-r--r--   0        0        0     2001 2023-07-11 09:19:39.419375 sweepai-0.4.0/sweepai/utils/config.py
+-rw-r--r--   0        0        0      964 2023-07-11 09:20:17.826102 sweepai-0.4.0/sweepai/utils/constants.py
+-rw-r--r--   0        0        0     6529 2023-07-11 09:19:39.419375 sweepai-0.4.0/sweepai/utils/diff.py
+-rw-r--r--   0        0        0      719 2023-07-07 20:46:56.696885 sweepai-0.4.0/sweepai/utils/event_logger.py
+-rw-r--r--   0        0        0     5245 2023-07-07 20:46:56.700219 sweepai-0.4.0/sweepai/utils/file_change_functions.py
+-rw-r--r--   0        0        0     8225 2023-07-09 08:40:46.468712 sweepai-0.4.0/sweepai/utils/github_utils.py
+-rw-r--r--   0        0        0       98 2023-07-07 20:46:56.700219 sweepai-0.4.0/sweepai/utils/hash.py
+-rw-r--r--   0        0        0      822 2023-07-07 20:46:56.700219 sweepai-0.4.0/sweepai/utils/huggingface.py
+-rw-r--r--   0        0        0     5564 2023-07-07 20:46:56.700219 sweepai-0.4.0/sweepai/utils/prompt_constructor.py
+-rw-r--r--   0        0        0      848 2023-07-07 20:46:56.700219 sweepai-0.4.0/sweepai/utils/scorer.py
+-rw-r--r--   0        0        0     1498 2023-07-07 20:46:56.700219 sweepai-0.4.0/sweepai/utils/snippets.py
+-rw-r--r--   0        0        0    11291 2023-07-07 20:46:56.700219 sweepai-0.4.0/sweepai/utils/utils.py
+-rw-r--r--   0        0        0     7743 2023-07-11 09:29:47.564605 sweepai-0.4.0/setup.py
+-rw-r--r--   0        0        0     7525 2023-07-11 09:29:47.565034 sweepai-0.4.0/PKG-INFO
```

### Comparing `sweepai-0.3.0/LICENSE` & `sweepai-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sweepai-0.3.0/README.md` & `sweepai-0.4.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 <p align="center">
     <img src="https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-3e61f57ad233">
 </p>
 <p align="center">
     <i>Bug Reports & Feature Requests ⟶&nbsp; Code Changes</i>
 </p>
 
@@ -14,113 +13,129 @@
     <img alt="Docs" src="https://img.shields.io/badge/Docs-docs.sweep.dev-blue?link=https%3A%2F%2Fdocs.sweep.dev">
 </a> 
 <a href="https://discord.gg/sweep-ai">
     <img src="https://dcbadge.vercel.app/api/server/sweep-ai?style=flat" />
 </a>
 <img alt="PyPI" src="https://img.shields.io/pypi/v/sweepai">
 <a href="https://pepy.tech/project/sweepai">
-    <img src="https://static.pepy.tech/badge/sweepai/week" />
+    <img src="https://static.pepy.tech/badge/sweepai/month" />
 </a>
 <a href="https://github.com/sweepai/sweep">
     <img src="https://img.shields.io/github/stars/sweepai/sweep" />
 </a>
 <a href="https://twitter.com/sweep__ai">
     <img src="https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fsweep__ai" />
 </a>
 </p>
 
-<b>Sweep</b> allows you to create and review GitHub issues with ease.
-Simply describe any issue and Sweep will do the rest.
-It will plan out what needs to be done, what changes to make, and write the changes to a PR. 
+<b>Sweep</b> is an AI junior developer that transforms bug reports & feature requests into code changes.
 
-Supported languages: Python, Javascript/Typescript, Rust, Go, Java/C#, C++ and anything else GPT-4 supports
+Describe bugs, small features, and refactors like you would to a junior developer, and Sweep:
+1. 🔍 reads your codebase
+2. 📝 plans the changes
+3. ⚡**writes a pull request with code**⚡
 
----
+See highlights at https://docs.sweep.dev/examples.
 
 ## ✨ Demo
 For the best experience, [install Sweep](https://github.com/apps/sweep-ai) to one of your repos and see the magic happen.
 
 [Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47)
 
-## 🌠 Features
-* Automatic interactive bug fixes & feature development
-* PR auto self-review + comment handling (effectively [Reflexion](https://arxiv.org/abs/2303.11366))
-* Address developer comments after PR is created using PR replies & code comments
-* Code snippets embedding-based semantic & popularity search ([🔍 Rebuilding our Search Engine in a Day](https://docs.sweep.dev/how-we-rebuilt-our-code-search-engine-in-a-day))
-* Chain-of-Thought retrieval using GPT Functions
+## 🌠 Sweep
+* 🔧 Turns issues directly into pull requests (without an IDE)
+* 👀 Addresses developer replies & comments on its PRs
+* 🕵️‍♂️ Uses embedding-based code search, with popularity reranking for repository-level code understanding ([🔍 Rebuilding our Search Engine in a Day](https://docs.sweep.dev/how-we-rebuilt-our-code-search-engine-in-a-day))
+* 🎊 New: Fixes PRs based on Github Actions feedback
 * 🎊 New: Sweep Chat, a local interface for Sweep (see below)
 
 ## 🚀 Getting Started
 
+### 🍲 Recipes
+#### To get the best performance from Sweep, we recommend the following approach to writing github issues/chats. 
+For harder problems, try to provide the same information a human would need. For simpler problems, providing a single line and a file name should suffice.
+
+A good issue might include:
+
+| Where to look <br> **[file name or function name]**| What to do <br> **[change the logic to do this]** | Additional Context (optional) <br> **[there's a bug/we need this feature/there's this dependency]** |
+|-----------|------------|----------------------|
+|In `sweepai/app/ui.py`|use an os-agnostic temp directory|N/A|
+|In `on_comment.py`|we should not fire an event|because it's possible that the comment is on a closed PR|
+|In the config loader in `packages/server/src/config.ts`|add a third option called "env" to load the config settings from environment variables| At present, there are two options:  1. ... and 2. ...|
+
+If you want Sweep to use a file, try to mention the full path. Similarly, to have Sweep use a function, try to mention the class method or what it does. Also see [✨ Tips and tricks for Sweep](https://docs.sweep.dev/tricks).
+
 ### 🖥️ Sweep Chat
-Sweep Chat allows you to interact with Sweep locally and will sync with GitHub. You can plan out your changes with Sweep, and then Sweep can create a pull request for you. 
+Sweep Chat allows you to interact with Sweep and GitHub locally. Collaborate on the plan with Sweep, then have it create the pull request for you. 
+
+**Prerequisites:** Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to your repository
+
+1. Run `pip install sweepai && sweep`. Note that you need **python 3.10+.**
+    - This runs GitHub authentication in your browser. 
 
-1. Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos
+2. Copy the 🔵 blue 8-digit code from your terminal into the page. You should only need to do the authentication once.  
+    - Wait a few seconds and Sweep Chat will start. 
 
-2. Run `pip install sweepai && sweep`. Note that you need python 3.10 or greater.
+3. Choose a repository from the dropdown at the top (the Github app must be installed to this repository).
 
-3. This should spin up a GitHub auth flow in your browser. Copy-paste the 🔵 blue 8-digit code from your terminal into the page. Then wait a few seconds and it should spin up Sweep Chat. You should only need to do the auth once.
+    - ⚡ Start chatting with Sweep Chat! ⚡
 
-4. Pick a repo from the dropdown at the top (the Github app must be installed on this repo). Then start chatting with Sweep Chat. Relevant searched files will show up on the right. Sweep Chat can make PRs if you ask it to create a PR. 
 <img src="https://github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-screenshot.png">
 
-💡 You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.
+Tips:
+* 🔍 Relevant searched files will show up on the right. 
+* 🔘 Sweep Chat creates PRs when the "Create PR" button is clicked. 
+* 💡 You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.
 
 #### From Source
 If you want the nightly build and or if the latest build has issues.
 
 1. `git clone https://github.com/sweepai/sweep && poetry install`
-2. `python sweepai/app/cli.py`. Note that you need python 3.10 or greater.
+2. `python sweepai/app/cli.py`. Note that you need **python 3.10+**.
 
 ### ✨ Sweep Github App
 Setting up Sweep is as simple as adding the GitHub bot to a repo, then creating an issue for the bot to address.
+We support all languages GPT4 supports, including Python, Typescript, Rust, Go, Java, C# and C++.
 
 1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos
 2. Create new issue in repo, like "Sweep: Write tests"
-3. "👀" means it is taking a look, and it will generate the desired code
-4. "🚀" means the bot has finished its job and created a PR
+3. Watch the magic happen 🪄
 
 ## 🤝 Contributing
 
-Contributions are welcome and greatly appreciated! For detailed guidelines on how to contribute, please see the [CONTRIBUTING.md](CONTRIBUTING.md) file. In essence, you'll need to fork the repository, create a new branch for your feature or bug fix, commit your changes, and open a pull request.
+Contributions are welcome and greatly appreciated! For detailed guidelines on how to contribute, please see the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 For more detailed docs, see [🚀 Quickstart](https://docs.sweep.dev/start).
 
----
-
 ## 📘 Story
 
-We were frustrated by small tickets, like simple bug fixes, annoying refactors, and small features, each task requiring us to open our IDE to fix simple bugs. So, we decided to leverage the capabilities of ChatGPT to address this directly in GitHub.
+We were frustrated by small tickets, like simple bug fixes, annoying refactors, and small features. Each task required us to open our IDE to fix simple bugs. So we decided to leverage the capabilities of ChatGPT to address this directly in GitHub.
 
-Unlike existing AI solutions, this can solve entire tickets and can be parallelized: developers can spin up 10 tickets and Sweep will address them all at once.
+Unlike existing AI solutions, this can solve entire tickets and can be parallelized + asynchronous: developers can spin up 10 tickets and Sweep will address them all at once.
 
 ## 📚 The Stack
-- GPT-4 32k 0613 (default) / Claude v1.3 100k
+- GPT-4 32k 0613 (default)
 - ActiveLoop DeepLake for Vector DB with MiniLM L12 as our embeddings model
 - Modal Labs for infra + deployment
 - Gradio for Sweep Chat
 
 ## 🗺️ Roadmap
-We're currently working on responding to linters and external search. For more, see [🗺️ Roadmap](https://docs.sweep.dev/roadmap).
+See [🗺️ Roadmap](https://docs.sweep.dev/roadmap)
 
 ## ⭐ Star History
 
 [![Star History Chart](https://api.star-history.com/svg?repos=sweepai/sweep&type=Date)](https://star-history.com/#sweepai/sweep&Date)
 
 Consider starring us if you're using Sweep so more people hear about us!
-
----
-
 <h2 align="center">
     Contributors
 </h2>
 <p align="center">
     Thank you for your contribution!
 </p>
 <p align="center">
     <a href="https://github.com/sweepai/sweep/graphs/contributors">
       <img src="https://contrib.rocks/image?repo=sweepai/sweep" />
     </a>
 </p>
 <p align="center">
     and, of course, Sweep!
 </p>
-
```

#### html2text {}

```diff
@@ -1,66 +1,79 @@
   [https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-
                                  3e61f57ad233]
                Bug Reports & Feature Requests â¶  Code Changes
       [Landing_Page] [Docs] [https://dcbadge.vercel.app/api/server/sweep-
- ai?style=flat] [PyPI] [https://static.pepy.tech/badge/sweepai/week] [https://
+ai?style=flat] [PyPI] [https://static.pepy.tech/badge/sweepai/month] [https://
   img.shields.io/github/stars/sweepai/sweep] [https://img.shields.io/twitter/
                 url?url=https%3A%2F%2Ftwitter.com%2Fsweep__ai]
-Sweep allows you to create and review GitHub issues with ease. Simply describe
-any issue and Sweep will do the rest. It will plan out what needs to be done,
-what changes to make, and write the changes to a PR. Supported languages:
-Python, Javascript/Typescript, Rust, Go, Java/C#, C++ and anything else GPT-
-4 supports --- ## â¨ Demo For the best experience, [install Sweep](https://
-github.com/apps/sweep-ai) to one of your repos and see the magic happen. [Demo]
-(https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-
-0af02f2b0e47) ## ð  Features * Automatic interactive bug fixes & feature
-development * PR auto self-review + comment handling (effectively [Reflexion]
-(https://arxiv.org/abs/2303.11366)) * Address developer comments after PR is
-created using PR replies & code comments * Code snippets embedding-based
-semantic & popularity search ([ð Rebuilding our Search Engine in a Day]
-(https://docs.sweep.dev/how-we-rebuilt-our-code-search-engine-in-a-day)) *
-Chain-of-Thought retrieval using GPT Functions * ð New: Sweep Chat, a local
-interface for Sweep (see below) ## ð Getting Started ### ð¥ï¸ Sweep Chat
-Sweep Chat allows you to interact with Sweep locally and will sync with GitHub.
-You can plan out your changes with Sweep, and then Sweep can create a pull
-request for you. 1. Install [Sweep GitHub app](https://github.com/apps/sweep-
-ai) to desired repos 2. Run `pip install sweepai && sweep`. Note that you need
-python 3.10 or greater. 3. This should spin up a GitHub auth flow in your
-browser. Copy-paste the ðµ blue 8-digit code from your terminal into the
-page. Then wait a few seconds and it should spin up Sweep Chat. You should only
-need to do the auth once. 4. Pick a repo from the dropdown at the top (the
-Github app must be installed on this repo). Then start chatting with Sweep
-Chat. Relevant searched files will show up on the right. Sweep Chat can make
-PRs if you ask it to create a PR. [https://github.com/sweepai/sweep/blob/
-856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-screenshot.png] ð¡
+Sweep is an AI junior developer that transforms bug reports & feature requests
+into code changes. Describe bugs, small features, and refactors like you would
+to a junior developer, and Sweep: 1. ð reads your codebase 2. ð plans the
+changes 3. â¡**writes a pull request with code**â¡ See highlights at https://
+docs.sweep.dev/examples. ## â¨ Demo For the best experience, [install Sweep]
+(https://github.com/apps/sweep-ai) to one of your repos and see the magic
+happen. [Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-
+40a7-9b5e-0af02f2b0e47) ## ð  Sweep * ð§ Turns issues directly into pull
+requests (without an IDE) * ð Addresses developer replies & comments on its
+PRs * ðµï¸ââï¸ Uses embedding-based code search, with popularity
+reranking for repository-level code understanding ([ð Rebuilding our Search
+Engine in a Day](https://docs.sweep.dev/how-we-rebuilt-our-code-search-engine-
+in-a-day)) * ð New: Fixes PRs based on Github Actions feedback * ð New:
+Sweep Chat, a local interface for Sweep (see below) ## ð Getting Started ###
+ð² Recipes #### To get the best performance from Sweep, we recommend the
+following approach to writing github issues/chats. For harder problems, try to
+provide the same information a human would need. For simpler problems,
+providing a single line and a file name should suffice. A good issue might
+include: | Where to look
+**[file name or function name]**| What to do
+**[change the logic to do this]** | Additional Context (optional)
+**[there's a bug/we need this feature/there's this dependency]** | |-----------
+|------------|----------------------| |In `sweepai/app/ui.py`|use an os-
+agnostic temp directory|N/A| |In `on_comment.py`|we should not fire an
+event|because it's possible that the comment is on a closed PR| |In the config
+loader in `packages/server/src/config.ts`|add a third option called "env" to
+load the config settings from environment variables| At present, there are two
+options: 1. ... and 2. ...| If you want Sweep to use a file, try to mention the
+full path. Similarly, to have Sweep use a function, try to mention the class
+method or what it does. Also see [â¨ Tips and tricks for Sweep](https://
+docs.sweep.dev/tricks). ### ð¥ï¸ Sweep Chat Sweep Chat allows you to
+interact with Sweep and GitHub locally. Collaborate on the plan with Sweep,
+then have it create the pull request for you. **Prerequisites:** Install [Sweep
+GitHub app](https://github.com/apps/sweep-ai) to your repository 1. Run `pip
+install sweepai && sweep`. Note that you need **python 3.10+.** - This runs
+GitHub authentication in your browser. 2. Copy the ðµ blue 8-digit code from
+your terminal into the page. You should only need to do the authentication
+once. - Wait a few seconds and Sweep Chat will start. 3. Choose a repository
+from the dropdown at the top (the Github app must be installed to this
+repository). - â¡ Start chatting with Sweep Chat! â¡ [https://github.com/
+sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-
+screenshot.png] Tips: * ð Relevant searched files will show up on the right.
+* ð Sweep Chat creates PRs when the "Create PR" button is clicked. * ð¡
 You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark. ####
 From Source If you want the nightly build and or if the latest build has
 issues. 1. `git clone https://github.com/sweepai/sweep && poetry install` 2.
-`python sweepai/app/cli.py`. Note that you need python 3.10 or greater. ### â¨
-Sweep Github App Setting up Sweep is as simple as adding the GitHub bot to a
-repo, then creating an issue for the bot to address. 1. Add the [Sweep GitHub
-app](https://github.com/apps/sweep-ai) to desired repos 2. Create new issue in
-repo, like "Sweep: Write tests" 3. "ð" means it is taking a look, and it
-will generate the desired code 4. "ð" means the bot has finished its job and
-created a PR ## ð¤ Contributing Contributions are welcome and greatly
-appreciated! For detailed guidelines on how to contribute, please see the
-[CONTRIBUTING.md](CONTRIBUTING.md) file. In essence, you'll need to fork the
-repository, create a new branch for your feature or bug fix, commit your
-changes, and open a pull request. For more detailed docs, see [ð Quickstart]
-(https://docs.sweep.dev/start). --- ## ð Story We were frustrated by small
-tickets, like simple bug fixes, annoying refactors, and small features, each
-task requiring us to open our IDE to fix simple bugs. So, we decided to
-leverage the capabilities of ChatGPT to address this directly in GitHub. Unlike
-existing AI solutions, this can solve entire tickets and can be parallelized:
+`python sweepai/app/cli.py`. Note that you need **python 3.10+**. ### â¨ Sweep
+Github App Setting up Sweep is as simple as adding the GitHub bot to a repo,
+then creating an issue for the bot to address. We support all languages GPT4
+supports, including Python, Typescript, Rust, Go, Java, C# and C++. 1. Add the
+[Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos 2. Create
+new issue in repo, like "Sweep: Write tests" 3. Watch the magic happen ðª ##
+ð¤ Contributing Contributions are welcome and greatly appreciated! For
+detailed guidelines on how to contribute, please see the [CONTRIBUTING.md]
+(CONTRIBUTING.md) file. For more detailed docs, see [ð Quickstart](https://
+docs.sweep.dev/start). ## ð Story We were frustrated by small tickets, like
+simple bug fixes, annoying refactors, and small features. Each task required us
+to open our IDE to fix simple bugs. So we decided to leverage the capabilities
+of ChatGPT to address this directly in GitHub. Unlike existing AI solutions,
+this can solve entire tickets and can be parallelized + asynchronous:
 developers can spin up 10 tickets and Sweep will address them all at once. ##
-ð The Stack - GPT-4 32k 0613 (default) / Claude v1.3 100k - ActiveLoop
-DeepLake for Vector DB with MiniLM L12 as our embeddings model - Modal Labs for
-infra + deployment - Gradio for Sweep Chat ## ðºï¸ Roadmap We're currently
-working on responding to linters and external search. For more, see [ðºï¸
-Roadmap](https://docs.sweep.dev/roadmap). ## â­ Star History [![Star History
-Chart](https://api.star-history.com/svg?repos=sweepai/sweep&type=Date)](https:/
-/star-history.com/#sweepai/sweep&Date) Consider starring us if you're using
-Sweep so more people hear about us! ---
+ð The Stack - GPT-4 32k 0613 (default) - ActiveLoop DeepLake for Vector DB
+with MiniLM L12 as our embeddings model - Modal Labs for infra + deployment -
+Gradio for Sweep Chat ## ðºï¸ Roadmap See [ðºï¸ Roadmap](https://
+docs.sweep.dev/roadmap) ## â­ Star History [![Star History Chart](https://
+api.star-history.com/svg?repos=sweepai/sweep&type=Date)](https://star-
+history.com/#sweepai/sweep&Date) Consider starring us if you're using Sweep so
+more people hear about us!
                            ***** Contributors *****
                        Thank you for your contribution!
                [https://contrib.rocks/image?repo=sweepai/sweep]
                             and, of course, Sweep!
```

### Comparing `sweepai-0.3.0/pyproject.toml` & `sweepai-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sweepai"
-version = "0.3.0"
+version = "0.4.0"
 description = "Sweep software chores"
 authors = ["Kevin Lu", "William Zeng", "Luke Jagg"]
 packages = [{ include = "sweepai" }]
 classifiers = ["Programming Language :: Python :: 3.11"]
 readme = "README.md"
 
 [tool.poetry.urls]
```

### Comparing `sweepai-0.3.0/sweepai/api.py` & `sweepai-0.4.0/sweepai/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import time
 from loguru import logger
 import modal
 from pydantic import ValidationError
-from sweepai.handlers.create_pr import create_pr  # type: ignore
+from sweepai.handlers.create_pr import create_pr
+from sweepai.handlers.on_check_suite import on_check_suite  # type: ignore
 
 from sweepai.handlers.on_ticket import on_ticket
 from sweepai.handlers.on_comment import on_comment
 from sweepai.utils.constants import API_NAME, BOT_TOKEN_NAME, DB_NAME, LABEL_COLOR, LABEL_DESCRIPTION, LABEL_NAME, SWEEP_LOGIN
 from sweepai.events import (
+    CheckRunCompleted,
     CommentCreatedRequest,
     InstallationCreatedRequest,
     IssueCommentRequest,
     IssueRequest,
     PRRequest,
     ReposAddedRequest,
 )
@@ -58,14 +60,15 @@
     "timeout": 30 * 60,
 }
 
 
 handle_ticket = stub.function(**FUNCTION_SETTINGS)(on_ticket)
 handle_comment = stub.function(**FUNCTION_SETTINGS)(on_comment)
 handle_pr = stub.function(**FUNCTION_SETTINGS)(create_pr)
+handle_check_suite = stub.function(**FUNCTION_SETTINGS)(on_check_suite)
 update_index = modal.Function.lookup(DB_NAME, "update_index")
 
 @stub.function(**FUNCTION_SETTINGS)
 @modal.web_endpoint(method="POST")
 async def webhook(raw_request: Request):
     """Handle a webhook request from GitHub."""
     try:
@@ -115,17 +118,19 @@
                         request.issue.body,
                         request.issue.number,
                         request.issue.html_url,
                         request.issue.user.login,
                         request.repository.full_name,
                         request.repository.description,
                         request.installation.id,
+                        None
                     )
             case "issue_comment", "created":
                 request = IssueCommentRequest(**request_dict)
+                # if replying to an issue with sweep label
                 if request.issue is not None \
                     and "sweep" in [label.name.lower() for label in request.issue.labels] \
                     and request.comment.user.type == "User":
                     request.issue.body = request.issue.body or ""
                     request.repository.description = (
                         request.repository.description or ""
                     )
@@ -138,14 +143,15 @@
                         request.issue.html_url,
                         request.issue.user.login,
                         request.repository.full_name,
                         request.repository.description,
                         request.installation.id,
                         request.comment.id
                     )
+                # if replying to a pr created by Sweep
                 elif request.issue.pull_request and request.issue.user.login == SWEEP_LOGIN and request.comment.user.type == "User": # TODO(sweep): set a limit                    
                     logger.info(f"Handling comment on PR: {request.issue.pull_request}")
                     handle_comment.spawn(
                         repo_full_name=request.repository.full_name,
                         repo_description=request.repository.description,
                         comment=request.comment.body,
                         pr_path=None,
@@ -167,14 +173,32 @@
                         installation_id=request.installation.id,
                         pr_number=request.pull_request.number,
                     )
                 # Todo: update index on comments
             case "pull_request_review", "submitted":
                 # request = ReviewSubmittedRequest(**request_dict)
                 pass
+            case "check_run", "completed":
+                request = CheckRunCompleted(**request_dict)
+                    # handle_check_suite
+                logs = None
+                # Must be Sweep firing the PR and it must fail
+                if request.sender.login == SWEEP_LOGIN and request.check_run.conclusion == "failure": 
+                    logs = handle_check_suite.call(request)
+                if len(request.check_run.pull_requests) > 0 and logs:
+                    handle_comment.spawn(
+                        repo_full_name=request.repository.full_name,
+                        repo_description=request.repository.description,
+                        comment="Sweep: " + logs,
+                        pr_path=None,
+                        pr_line_position=None,
+                        username=request.sender.login,
+                        installation_id=request.installation.id,
+                        pr_number=request.check_run.pull_requests[0].number,
+                    )
             case "installation_repositories", "added":
                 repos_added_request = ReposAddedRequest(**request_dict)
                 metadata = {
                     "installation_id": repos_added_request.installation.id,
                     "repositories": [
                         repo.full_name
                         for repo in repos_added_request.repositories_added
```

### Comparing `sweepai-0.3.0/sweepai/app/api_client.py` & `sweepai-0.4.0/sweepai/app/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,14 +152,15 @@
         with httpx.Client(timeout=30) as client: # sometimes this step is slow
             with client.stream(
                 'POST', 
                 self.api_endpoint + '/chat_stream',
                 json={
                     "messages": messages,
                     "snippets": [snippet.dict() for snippet in snippets],
+                    "do_add_plan": True,
                     "functions": [func.dict() for func in functions],
                     "function_call": function_call,
                     "config": self.config.dict()
                 }
             ) as response:
                 for delta_chunk in response.iter_text():
                     if not delta_chunk:
```

### Comparing `sweepai-0.3.0/sweepai/app/backend.py` & `sweepai-0.4.0/sweepai/app/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 import modal
 from loguru import logger
 from fastapi import FastAPI
 from fastapi.responses import StreamingResponse
 from pydantic import BaseModel
 
 from sweepai.app.config import SweepChatConfig
-from sweepai.core.chat import ChatGPT
-from sweepai.core.entities import FileChangeRequest, Function, Message, PullRequest, Snippet
-from sweepai.core.sweep_bot import SweepBot
 from sweepai.utils.config import SweepConfig
 from sweepai.utils.constants import API_NAME, BOT_TOKEN_NAME, DB_NAME, PREFIX
 from sweepai.utils.github_utils import get_github_client, get_installation_id
-from sweepai.core.prompts import gradio_system_message_prompt
 from sweepai.utils.event_logger import posthog
+from sweepai.core.chat import ChatGPT
+from sweepai.core.entities import FileChangeRequest, Function, Message, PullRequest, Snippet
+from sweepai.core.sweep_bot import SweepBot
+from sweepai.core.prompts import gradio_system_message_prompt, gradio_user_prompt
 
 get_relevant_snippets = modal.Function.from_name(DB_NAME, "get_relevant_snippets")
 
 stub = modal.Stub(PREFIX + "-ui")
 image = (
     modal.Image.debian_slim()
     .apt_install("git")
@@ -92,15 +92,15 @@
             installation_id = get_installation_id(organization)
             assert installation_id
         except Exception as e:
             logger.warning(e)
             posthog.capture(request.github_username, "failed", properties={"error": str(e), **metadata})
             raise fastapi.HTTPException(status_code=403, detail="Sweep app is not installed on this repo. To install it, go to https://github.com/apps/sweep-ai")
 
-        posthog.capture(request.github_username, "succeeded", properties=metadata)
+        posthog.capture(request.github_username, "success", properties=metadata)
 
         return {"installation_id": installation_id}
 
     class SearchRequest(BaseModel):
         query: str
         config: SweepChatConfig
         n_results: int = 5
@@ -137,15 +137,15 @@
                     snippet.content = repo.get_contents(snippet.file_path, SweepConfig.get_branch(repo)).decoded_content.decode("utf-8")
                 except Exception:
                     logger.error(snippet)
         except Exception as e:
             posthog.capture(request.config.github_username, "failed", properties={"error": str(e), **metadata})
             raise e
 
-        posthog.capture(request.config.github_username, "succeeded", properties=metadata)
+        posthog.capture(request.config.github_username, "success", properties=metadata)
         return snippets
 
     class CreatePRRequest(BaseModel):
         # proposed PR information
         file_change_requests: list[tuple[str, str]]
         pull_request: PullRequest 
 
@@ -218,14 +218,15 @@
             "html_url": generated_pull_request.html_url,
         }
     
     class ChatRequest(BaseModel):
         messages: list[tuple[str | None, str | None]]
         snippets: list[Snippet]
         config: SweepChatConfig
+        do_add_plan: bool = False
         functions: list[Function] = []
         function_call: Any = "auto"
 
     @app.post("/chat")
     def chat(
         request: ChatRequest,
     ) -> str:
@@ -236,15 +237,15 @@
         result = chatgpt.chat(messages[-1].content, model="gpt-4-0613")
         return result
     
     @app.post("/chat_stream")
     def chat_stream(request: ChatRequest):
         assert verify_config(request.config)
         metadata = {
-            "function": "ui_create_pr",
+            "function": "ui_chat_stream",
             "repo_full_name": request.config.repo_full_name,
             "organization": request.config.repo_full_name.split("/")[0],
             "username": request.config.github_username,
             "installation_id": request.config.installation_id,
             "mode": PREFIX,
         }
 
@@ -253,19 +254,21 @@
             messages = [Message.from_tuple(message) for message in request.messages]
             system_message = gradio_system_message_prompt.format(
                 snippets="\n".join([snippet.denotation + f"\n```{snippet.get_snippet()}```" for snippet in request.snippets]),
                 repo_name=request.config.repo_full_name,
                 repo_description="" # TODO: fill this
             )
             chatgpt = ChatGPT(messages=[Message(role="system", content=system_message, key="system")] + messages[:-1])
+            if request.do_add_plan:
+                chatgpt.messages[-1].content += gradio_user_prompt
         except Exception as e:
             posthog.capture(request.config.github_username, "failed", properties={"error": str(e), **metadata})
             raise e
         def stream_chat():
             for chunk in chatgpt.chat_stream(messages[-1].content, model="gpt-4-0613", functions=request.functions, function_call=request.function_call):
                 yield json.dumps(chunk)
-            posthog.capture(request.config.github_username, "succeeded", properties=metadata)
+            posthog.capture(request.config.github_username, "success", properties=metadata)
         return StreamingResponse(
             stream_chat(),
             media_type="text/event-stream"
         )
     return app
```

### Comparing `sweepai-0.3.0/sweepai/app/cli.py` & `sweepai-0.4.0/sweepai/app/cli.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.3.0/sweepai/app/config.py` & `sweepai-0.4.0/sweepai/app/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 config_path = ConfigPath( 'sweep_chat', 'sweep', '.yaml' )
 CONFIG_FILE = config_path.saveFilePath()
 
 class State(BaseModel):
     file_paths: list[str] = []
     chat_history: list[tuple[str | None, str | None]] = []
     snippets_text: str = "### Relevant Snippets:"
+    plan: list[tuple[str, str]] = []
 
 class SweepChatConfig(BaseModel):
     github_username: str
     github_pat: str # secret
     repo_full_name: str | None = None
     installation_id: int | None = None
     state: State = State()
```

### Comparing `sweepai-0.3.0/sweepai/app/ui.py` & `sweepai-0.4.0/sweepai/app/ui.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import os
+import re
 import tempfile
 from git import Repo
 from github import Github
 import gradio as gr
 from loguru import logger
 import shutil
 
@@ -36,15 +37,15 @@
     visibility: hidden;
 }
 pre, code {
     white-space: pre-wrap !important;
     word-break: break-all !important;
 }
 #snippets {
-    height: 750px;
+    height: 400px;
     overflow-y: scroll;
 }
 #message_box > label > span {
     display: none;
 }
 '''
 
@@ -59,15 +60,15 @@
     entries = os.listdir(current_dir)
 
     for entry in entries:
         entry_path = os.path.join(current_dir, entry)
 
         if os.path.isfile(entry_path):
             try:
-                with open(entry_path, 'r') as file:
+                with open(entry_path, 'r', encoding="utf-8", errors="ignore") as file:
                     contents = file.read()
                 path_to_contents[entry_path[len(root_path) + 1:]] = contents
                 files.append(entry_path[len(root_path) + 1:])
             except UnicodeDecodeError as e:
                 logger.warning(f"Received warning {e}, skipping...")
                 continue
         elif os.path.isdir(entry_path):
@@ -120,14 +121,24 @@
     global repo
     if len(args) > 0:
         repo = args[0]
     else:
         repo = config.repo_full_name
     return gr.Dropdown.update(choices=get_files(repo))
 
+def parse_response(raw_response: str) -> tuple[str, list[tuple[str, str]]]:
+    if "Plan:" not in raw_response:
+        response, raw_plan = raw_response, ""
+    else:
+        response, raw_plan = raw_response.split("Plan:", 1)
+    if response.startswith("Response:"):
+        response = response[len("Response:"):]
+    plan = [(line[:line.find(":")].strip(), line[line.find(":") + 1:].strip()) for line in raw_plan.split("\n*") if line]
+    return response, plan
+
 global_state = config.state
 
 with gr.Blocks(theme=gr.themes.Soft(), title="Sweep Chat", css=css) as demo:
     print("Launching gradio!")
     with gr.Row():
         with gr.Column(scale=2):
             repo_full_name = gr.Dropdown(choices=[repo.full_name for repo in repos], label="Repo full name", value=lambda: config.repo_full_name or "")
@@ -137,25 +148,42 @@
         print("Indexed files!")
         repo_full_name.change(get_files_update, repo_full_name, file_names)
         with gr.Column(scale=1):
             restart_button = gr.Button("Restart")
 
     with gr.Row():
         with gr.Column(scale=2):
-            chatbot = gr.Chatbot(height=750, value=lambda: global_state.chat_history)
+            chatbot = gr.Chatbot(height=400, value=lambda: global_state.chat_history)
         with gr.Column():
-            snippets_text = gr.Markdown(value=lambda: global_state.snippets_text, elem_id="snippets")
+            with gr.Row():
+                snippets_text = gr.Markdown(value=lambda: global_state.snippets_text, elem_id="snippets")
+
+    with gr.Row():
+        plan = gr.List(
+            value=[[filename + ": " + instructions] for filename, instructions in global_state.plan],
+            headers=["Proposed Plan"], 
+            interactive=True,
+            col_count=(1, "static"),
+            wrap=True
+        )
     
     with gr.Row():
         with gr.Column(scale=8):
             msg = gr.Textbox(placeholder="Send a message to Sweep", label=None, elem_id="message_box")
         with gr.Column(scale=0.5):
-            create_pr_button = gr.Button(value="Create PR", interactive=False)
+            create_pr_button = gr.Button(value="Create PR", interactive=bool(global_state.chat_history))
 
-    restart_button.click(lambda: ([], []), [], [file_names, chatbot])
+    def clear_inputs():
+        global global_state
+        global_state = State()
+        config.state = global_state
+        config.save()
+        return [], [], [[""]]
+
+    restart_button.click(clear_inputs, None, [file_names, chatbot, plan])
 
     file_names.change(get_files_update, repo_full_name, chatbot)
 
     searched = False
     selected_snippets = []
     file_to_str = {}
 
@@ -211,111 +239,124 @@
     file_names.change(file_names_change, [file_names], [file_names, snippets_text])
     
     def handle_message_submit(repo_full_name: str, user_message: str, history: list[tuple[str | None, str | None]]):
         if not repo_full_name:
             raise Exception("Set the repository name first")
         return gr.update(value="", interactive=False), history + [[user_message, None]], gr.Button.update(interactive=True)
 
-    def _handle_message_stream(chat_history: list[tuple[str | None, str | None]], snippets_text, file_names):
+    def _handle_message_stream(chat_history: list[tuple[str | None, str | None]], snippets_text, file_names, plan):
         global selected_snippets
         global searched
+        if plan is None or plan == [[]] or plan == [[""]] or plan == [["", ""]]:
+            plan = [["", ""]]
         message = chat_history[-1][0]
-        yield chat_history, snippets_text, file_names
+        yield chat_history, snippets_text, file_names, plan
         if not selected_snippets:
             searched = True
             # Searching for relevant snippets
             chat_history[-1][1] = "Searching for relevant snippets..."
             snippets_text = build_string()
-            yield chat_history, snippets_text, file_names
+            yield chat_history, snippets_text, file_names, plan
             logger.info("Fetching relevant snippets...")
             selected_snippets += api_client.search(chat_history[-1][0], 3)
             snippets_text = build_string()
             file_names = [snippet.file_path for snippet in selected_snippets]
-            yield chat_history, snippets_text, file_names
+            yield chat_history, snippets_text, file_names, plan
             logger.info("Fetched relevant snippets.")
             chat_history[-1][1] = "Found relevant snippets."
             # Update using chat_history
             snippets_text = build_string()
-            yield chat_history, snippets_text, file_names
+            yield chat_history, snippets_text, file_names, plan
         
         # Generate response
         logger.info("...")
         chat_history.append([None, "..."])
-        yield chat_history, snippets_text, file_names
+        yield chat_history, snippets_text, file_names, plan
         chat_history[-1][1] = ""
         logger.info("Starting to generate response...")
         if len(chat_history) > 1 and "create pr" in message.lower():
             stream = api_client.stream_chat(
                 chat_history, 
                 selected_snippets,
                 functions=[create_pr_function],
                 function_call=create_pr_function_call,
             )
         else:
             stream = api_client.stream_chat(chat_history, selected_snippets)
         function_name = ""
         raw_arguments = ""
+        raw_response = ""
+        parsed_response = ""
         for chunk in stream:
             if chunk.get("content"):
                 token = chunk["content"]
-                chat_history[-1][1] += token
-                yield chat_history, snippets_text, file_names
+                raw_response += token
+                parsed_response, plan = parse_response(raw_response)
+                chat_history[-1][1] = parsed_response
+                yield chat_history, snippets_text, file_names, plan
             if chunk.get("function_call"):
                 function_call = chunk["function_call"]
                 function_name = function_name or function_call.get("name")
                 raw_arguments += function_call.get("arguments")
                 chat_history[-1][1] = f"Calling function: `{function_name}`\n```json\n{raw_arguments}\n```"
-                yield chat_history, snippets_text, file_names
+                yield chat_history, snippets_text, file_names, plan
         if function_name:
             arguments = json.loads(raw_arguments)
             if function_name == "create_pr":
                 assert "title" in arguments
                 assert "summary" in arguments
                 assert "plan" in arguments
                 if "branch" not in arguments:
                     arguments["branch"] = arguments["title"].lower().replace(" ", "_").replace("-", "_")[:50]
                 chat_history[-1][1] = pr_summary_template.format(
                     title=arguments["title"],
                     summary=arguments["summary"],
                     plan="\n".join([f"* `{item['file_path']}`: {item['instructions']}" for item in arguments["plan"]])
                 )
-                yield chat_history, snippets_text, file_names
-                pull_request = api_client.create_pr(
-                    file_change_requests=[(item["file_path"], item["instructions"]) for item in arguments["plan"]],
-                    pull_request={
-                        "title": arguments["title"],
-                        "content": arguments["summary"],
-                        "branch_name": arguments["branch"],
-                    },
-                    messages=chat_history,
-                )
-                chat_history.append((None, f"✅ PR created at {pull_request['html_url']}"))
-                yield chat_history, snippets_text, file_names
+                yield chat_history, snippets_text, file_names, plan
+                plan = [(item["file_path"], item["instructions"]) for item in arguments["plan"]]
+                yield chat_history, snippets_text, file_names, plan
             else:
                 raise NotImplementedError
     
-    def handle_message_stream(chat_history: list[tuple[str | None, str | None]], snippets_text, file_paths):
+    def handle_message_stream(chat_history: list[tuple[str | None, str | None]], snippets_text, file_paths, plan):
         global global_state
-        for chat_history, snippets_text, file_paths in _handle_message_stream(chat_history, snippets_text, file_paths):
+        for chat_history, snippets_text, file_paths, plan in _handle_message_stream(chat_history, snippets_text, file_paths, plan):
+            if plan is None or plan == [[]] or plan == [[""]] or plan == [["", ""]]:
+                plan = [["", ""]]
             global_state = State(
                 chat_history=chat_history,
                 snippets_text=snippets_text,
                 file_paths=file_paths,
+                plan=plan,
             )
             config.state = global_state
             config.save()
-            yield chat_history, snippets_text, file_paths
+            yield chat_history, snippets_text, file_paths, [(file_path + ": " + instructions,) for file_path, instructions in plan]
 
     response = msg \
-        .submit(handle_message_submit, [repo_full_name, msg, chatbot], [msg, chatbot, create_pr_button], queue=False)\
-        .then(handle_message_stream, [chatbot, snippets_text, file_names], [chatbot, snippets_text, file_names])
-    response.then(lambda: gr.update(interactive=True), None, [msg], queue=False)
-
-    def on_create_pr_button_click(chat_history: list[tuple[str | None, str | None]], create_pr_button: str):
-        return chat_history + [(create_pr_button, None)]
-
-    create_pr_button.click(on_create_pr_button_click, [chatbot, create_pr_button], chatbot).then(handle_message_stream, [chatbot, snippets_text, file_names], [chatbot, snippets_text, file_names])
+        .submit(handle_message_submit, [repo_full_name, msg, chatbot], [msg, chatbot, create_pr_button], queue=False) \
+        .then(handle_message_stream, [chatbot, snippets_text, file_names, plan], [chatbot, snippets_text, file_names, plan]) \
+        .then(lambda: gr.update(interactive=True), None, [msg], queue=False)
+
+    def on_create_pr_button_click(chat_history: list[tuple[str | None, str | None]], plan: list[tuple[str]]):
+        chat_history.append((None, "⌛ Creating PR..."))
+        yield chat_history
+        title = chat_history[0][0]
+        content = chat_history[-1][1]
+        pull_request = api_client.create_pr(
+            file_change_requests=[(item[:item.find(":")], item[item.find(":") + 1:]) for item, *_ in plan],
+            pull_request={
+                "title": title,
+                "content": content,
+                "branch_name": title.lower().replace(" ", "_").replace("-", "_")[:50]
+            },
+            messages=chat_history,
+        )
+        chat_history.append((None, f"✅ PR created at {pull_request['html_url']}"))
+        yield chat_history
 
+    create_pr_button.click(on_create_pr_button_click, [chatbot, plan], chatbot)
 
 if __name__ == "__main__":
     demo.queue()
     demo.launch()
```

### Comparing `sweepai-0.3.0/sweepai/core/chat.py` & `sweepai-0.4.0/sweepai/core/chat.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.3.0/sweepai/core/code_repair.py` & `sweepai-0.4.0/sweepai/core/code_repair.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,14 +40,22 @@
         if result.returncode == 0:
             return True
         else:
             print(result.stderr)
             return False
 
 
-    def repair_code(self, diff: str, user_code: str, feature:str) -> str:
+    def repair_code(self, diff: str, user_code: str, feature:str, retries=3) -> str:
         self.messages = [Message(role="system", content=code_repair_system_prompt.format(feature=feature))]
         self.model = "gpt-3.5-turbo-16k-0613" # can be optimized
-        response = self.chat(code_repair_prompt.format(diff=diff, user_code=user_code))
-        self.undo()
+        retry_count = 0
+        while retry_count < retries:
+            response = self.chat(code_repair_prompt.format(diff=diff, user_code=user_code), message_key='code_repair')
+            # Check if the length of the response does not differ by more than 15% from the input
+            if len(user_code.splitlines()) > 50 and abs(len(response.splitlines()) - len(user_code.splitlines())) / len(user_code.splitlines()) > 0.15:
+                self.delete_messages_from_chat(key_to_delete='code_repair')
+                retry_count += 1
+                if retry_count == retries:
+                    return user_code
+            else:
+                break
         return response.strip() + "\n"
-
```

### Comparing `sweepai-0.3.0/sweepai/core/entities.py` & `sweepai-0.4.0/sweepai/core/entities.py`

 * *Files 9% similar despite different names*

```diff
@@ -95,18 +95,19 @@
         instructions = clean_instructions(instructions)
         res = FileChangeRequest(filename=file_name, 
                                 instructions=instructions,
                                 change_type="modify")
         return res
 
 
-class FileChange(RegexMatchableBaseModel):
+class FileCreation(RegexMatchableBaseModel):
     commit_message: str
     code: str
-    _regex = r"""Commit Message:(?P<commit_message>.*)<new_file>(python|javascript|typescript|csharp|tsx|jsx)?(?P<code>.*)$"""
+    _regex = r'''commit_message\s+=\s+"(?P<commit_message>.*?)".*?<new_file>(python|javascript|typescript|csharp|tsx|jsx)?(?P<code>.*)<\/new_file>'''
+    #_regex = r"""Commit Message:(?P<commit_message>.*)<new_file>(python|javascript|typescript|csharp|tsx|jsx)?(?P<code>.*)$"""
     # _regex = r"""Commit Message:(?P<commit_message>.*)(<new_file>|```)(python|javascript|typescript|csharp|tsx|jsx)?(?P<code>.*)($|```)"""
 
     @classmethod
     def from_string(cls: Type[Self], string: str, **kwargs) -> Self:
         result = super().from_string(string, **kwargs)
         result.code = result.code.strip()
         if result.code.endswith("</new_file>"):
@@ -123,16 +124,15 @@
         return result
 
 
 class PullRequest(RegexMatchableBaseModel):
     title: str
     branch_name: str
     content: str
-    _regex = r"""Title:(?P<title>.*)Branch Name:(?P<branch_name>.*)<content>(python|javascript|typescript|csharp|tsx|jsx)?(?P<content>.*)</content>"""
-
+    _regex = r'''title\s+=\s+"(?P<title>.*?)"\n+branch\s+=\s+"(?P<branch_name>.*?)"\n+content\s+=\s+"""(?P<content>.*?)"""'''
 
 class Snippet(BaseModel):
     """
     Start and end refer to line numbers
     """
     
     content: str
@@ -220,8 +220,12 @@
 class DiffSummarization(RegexMatchableBaseModel):
     content: str
     _regex = r"""<file_summarization>(?P<content>.*)<\/file_summarization>"""
 
 class PullRequestComment(RegexMatchableBaseModel):
     changes_required: str
     content: str
-    _regex = r"""<changes_required>(?P<changes_required>.*)<\/changes_required>(\s+)<review_comment>(?P<content>.*)<\/review_comment>"""
+    _regex = r"""<changes_required>(?P<changes_required>.*)<\/changes_required>(\s+)<review_comment>(?P<content>.*)<\/review_comment>"""
+
+class NoFilesException(Exception):
+    def __init__(self, message="Sweep could not find any files to modify"):
+        super().__init__(message)
```

### Comparing `sweepai-0.3.0/sweepai/core/prompts.py` & `sweepai-0.4.0/sweepai/core/prompts.py`

 * *Files 9% similar despite different names*

```diff
@@ -197,34 +197,39 @@
 Write a 1-paragraph response to this user:
 * Tell them you have started working on this PR and a rough summary of your plan. 
 * Do not start with "Here is a draft", just write the response.
 * Use github markdown to format the response.
 """
 
 create_file_prompt = """
+You are creating a PR for creating the single new file.
+
 Think step-by-step regarding the instructions and what should be added to the new file.
-Then create a plan of parts of the code to create, with low-level, detailed references to functions and variable to create, and what each function does.
-Then create the following file using the following instructions:
+Next, create a plan of parts of the code to create, with low-level, detailed references to functions and variable to create, and what each function does.
+Last, create the following file using the following instructions:
 
-File Name: {filename}
+DO NOT write "pass" or "Rest of code". Do not literally write "{{new_file}}". You must use the new_file XML tags, and all text inside these tags will be placed in the newly created file.
 
-Instructions: {instructions}
+Reply in the following format:
+Commit planning:
+file_name = "..."
+instructions = "..."
+commit_message = "..."
 
-Reply in the following format. DO NOT write "pass" or "Rest of code". Do not literally write "{{new_file}}". You must use the new_file XML tags, and all text inside these tags will be placed in the newly created file.
 
 Step-by-step thoughts with explanations: 
 * Thought 1 - Explanation 1
 * Thought 2 - Explanation 2
 ...
 
 Detailed plan of additions:
 * Addition 1
 * Addition 2
 ...
-Commit Message: {{commit_message}}
+
 <new_file>
 {{new_file}}
 </new_file>
 """
 
 """
 Reply in the format below. 
@@ -265,35 +270,32 @@
 #<snippets>
 #{snippets}
 #</snippets>
 modify_file_prompt = """
 File contains lines {line_numbers}
 
 Generate a new_file based on the given plan, ensuring that you:
-1. Do not write "pass" statements.
-2. Provide complete functions with actual business logic. It is imperative that we do not leave any work to the user/future readers of this code.
-3. Do not write new "todo" comments.
-4. Do not write incomplete functions.
-5. Do not write the original line numbers with the new code.
-6. Make sure the new code follows the same programming language conventions as the old code.
+1. It is imperative that we do not leave any work to the user/future readers of this code. So, WRITE FUNCTIONS COMPLETELY THAT WILL WORK.
+2. Do not write the original line numbers with the new code.
+3. Make sure the new code follows the same programming language conventions as the old code.
 
 Instead of writing "# Rest of Code", specify the lines to copy from the old file using an XML tag, inclusive (e.g., "<copied>0-25</copied>"). Make sure to use this exact format.
 Copy the correct line numbers and copy as long of a prefix and suffix as possible. For instance, if you want to insert code after line 50, start with "<copied>0-50</copied>".
 
 Example: If you want to modify lines 51-52 and add line after line 75:
 <new_file>
 <copied>1-50</copied>
 def main():
      print("hello world")
 <copied>53-75</copied>
 print("debug statement")
 <copied>76-100</copied>
 </new_file>
 
-Do not rewrite entire file. Use <copied> XML tag when possible.
+Do not rewrite entire file. Use <copied> XML tag when possible. Do not include the line numbers in the new file. Write complete implementations.
 """
 
 
 modify_file_prompt_2 = """
 File Name: {filename}
 <old_file>
 {code}
@@ -317,58 +319,54 @@
 * lines a-b
 ...
 ```
 
 Code Generation:
 ```
 Generate a new_file based on the given plan, ensuring that you:
-1. Do not write "pass" statements.
-2. Provide complete functions with actual business logic. It is imperative that we do not leave any work to the user/future readers of this code.
-3. Do not write new "todo" comments.
-4. Do not write incomplete functions.
-5. Do not write the original line numbers with the new code.
-6. Make sure the new code follows the same programming language conventions as the old code.
+1. It is imperative that we do not leave any work to the user/future readers of this code. So, WRITE FUNCTIONS COMPLETELY THAT WILL WORK.
+2. Do not write the original line numbers with the new code.
+3. Make sure the new code follows the same programming language conventions as the old code.
 
 Instead of writing "# Rest of Code", specify the lines to copy from the old file using an XML tag, inclusive (e.g., "<copy_lines A-B>"). Make sure to use this exact format.
 Copy the correct line numbers and copy as long of a prefix and suffix as possible. For instance, if you want to insert code after line 50, start with "<copy_lines 1-50>".
 
 Example: If you want to modify lines 51-52 and add line after line 75:
 <new_file>
 <copy_lines 1-50>
 def main():
      print("hello world")
 <copy_lines 53-75>
 print("debug statement")
 <copy_lines 76-100>
 </new_file>
 
-Do not rewrite entire file. Use <copy_lines A-B> XML tag when possible. Do not include the line numbers in the new file.
+Do not rewrite entire file. Use <copy_lines A-B> XML tag when possible. Do not include the line numbers in the new file. Write complete implementations.
 ```
 
 Context: "{instructions}". Limit your changes to the context.
 Instructions:
 - Complete Code Planning step
 - Complete Code Generation step"""
 
 
 
 
 
 pr_code_prompt = ""  # TODO: deprecate this
 
 
-pull_request_prompt = """
-Awesome! Could you also provide a PR message in the following format? Content should be in Github style markdown. Thanks!
+pull_request_prompt = """With your plan in mind, generate one PR for your planned changes using GitHub markdown.
 
-Title: {title}
-Branch Name: {branch_name}
-<content>
-{content}
-</content>
-"""
+title = "..."
+branch = "..."
+content = \"\"\"
+...
+...
+\"\"\""""
 
 summarize_system_prompt = """
 Your name is Sweep bot. You are an engineer assigned to helping summarize code instructions and code changes.
 """
 
 user_file_change_summarize_prompt = """
 Summarize the given instructions for making changes in a pull request.
@@ -400,36 +398,63 @@
 Username: {username}
 Query: {query}
 
 Gather information (i.e. fetch more snippets) to solve the problem. Use "create_pr" if the user asks for changes or you think code changes are needed.
 """
 
 code_repair_system_prompt = """\
-You are a genius trained for code repair. 
+You are a genius trained for code stitching.
 You will be given two pieces of code marked by xml tags. The code inside <diff></diff> is the difference betwen the user_code and the original code, and the code inside <user_code></user_code> is a user's attempt at adding a change described as {feature}. 
-Our goal is to return a working version of user_code that follows {feature}.
+Our goal is to return a working version of user_code that follows {feature} while making as few edits as possible.
 """
 
 code_repair_prompt = """\
 <diff>
 {diff}
 </diff>
 <user_code>
 {user_code}
 </user_code>
 This is the user_code.
 Instructions:
-* Keep the logic changes from user_code.
-* Fix any issues using our knowledge of both the diff and user_code files. 
-* Fix syntax errors and accidentally deleted lines.
-* Do not perform code style cleanup.
-* Do not add or remove any whitespace besides what is necessary to fix syntax errors.
-* Do not add or remove any comments.
-Return the repaired user_code without xml tags. All of the text you return will be placed in the file. Revert any unrelated deletions to user_code, using the diff and described change.
+* The user_code may have accidental additions and deletions before and after the code that needs to be added. You can revert these changes.
+* Fix syntax errors and formatting, but only around lines mentioned in the diff.
+* Be as minimal as possible with the changes you make to user_code.
+* Add or remove whitespaces, but only around lines mentioned in the diff.
+* Add or remove comments, but only around lines mentioned in the diff.
+* Clean up the code, but only around lines mentioned in the diff.
+* Do not change the logic in user_code.
+
+Return the repaired user_code without xml tags. All of the text you return will be placed in the file.
 """
 
 gradio_system_message_prompt = """Your name is Sweep bot. You are a brilliant and thorough engineer assigned to assist the following user with their problems in the Github repo. You will be helpful and friendly, but informal and concise: get to the point. When you write code to solve tickets, the code works on the first try and is formatted perfectly. You have the utmost care for the user that you write for, so you do not make mistakes. If the user asks you to create a PR, you will use the create_pr function.
 
 Relevant snippets provided by search engine (decreasing relevance):
 {snippets}
 Repo: {repo_name}
-Description: {repo_description}"""
+Description: {repo_description}
+"""
+
+gradio_user_prompt = """
+Respond in the following format (one line per file change, no prefixes, each file should be unique, only files that should be created or changed should go into the plan). There must be a blank line between the summary and the plan:
+
+Response:
+Provide a summary of the proposed changes or inquiries for the user. This section will be displayed directly to the user.
+
+Plan:
+* filename_1: instructions_1
+* filename_2: instructions_2
+...
+"""
+
+gha_extraction_system_prompt = """\
+Your job is to extract the information needed to debug the log from the Github Actions workflow file.
+"""
+
+gha_extraction_prompt = """\
+Here are the logs:
+{gha_logs}
+Copy the important lines from the github action logs. Describe the issue as you would report a bug to a developer and do not mention the github action or preparation steps. Only mention the actual issue.
+For example, if the issue was because of github action -> pip install -> python black formatter -> file xyz is broken, only report that file xyz is broken and fails formatting. Do not mention the github action or pip install.
+Make sure to mention the file name and line number of the issue(if applicable).
+"""
```

### Comparing `sweepai-0.3.0/sweepai/core/react.py` & `sweepai-0.4.0/sweepai/core/react.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.3.0/sweepai/core/sweep_bot.py` & `sweepai-0.4.0/sweepai/core/sweep_bot.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,42 +5,45 @@
 from github.ContentFile import ContentFile
 from github.GithubException import GithubException
 import modal
 from pydantic import BaseModel
 from sweepai.core.code_repair import CodeRepairer
 from sweepai.utils.chat_logger import ChatLogger
 import re
+import traceback
 
 from sweepai.core.entities import (
-    FileChange,
+    FileCreation,
     FileChangeRequest,
     FilesToChange,
     PullRequest,
     RegexMatchError,
     Function,
-    Snippet
+    Snippet, NoFilesException
 )
 from sweepai.core.chat import ChatGPT
 from sweepai.core.prompts import (
     files_to_change_prompt,
     pull_request_prompt,
     create_file_prompt,
     modify_file_prompt_2,
     modify_file_plan_prompt,
 )
 from sweepai.utils.config import SweepConfig
-from sweepai.utils.constants import DB_NAME
+from sweepai.utils.constants import DB_NAME, SECONDARY_MODEL
 from sweepai.utils.diff import format_contents, generate_diff, generate_new_file, is_markdown, revert_whitespace_changes
 
 
 class CodeGenBot(ChatGPT):
 
-    def get_files_to_change(self):
+    def get_files_to_change(self, retries=2):
         file_change_requests: list[FileChangeRequest] = []
-        for count in range(5):
+        # Todo: put retries into a constants file
+        # also, this retries multiple times as the calls for this function are in a for loop
+        for count in range(retries):
             try:
                 logger.info(f"Generating for the {count}th time...")
                 files_to_change_response = self.chat(files_to_change_prompt, message_key="files_to_change") # Dedup files to change here
                 files_to_change = FilesToChange.from_string(files_to_change_response)
                 files_to_create: list[str] = files_to_change.files_to_create.split("\n*")
                 files_to_modify: list[str] = files_to_change.files_to_modify.split("\n*")
                 for file_change_request, change_type in zip(
@@ -70,25 +73,36 @@
                 file_change_requests = [FileChangeRequest(filename=file_name, instructions=instructions, change_type=change_type) for file_name, (instructions, change_type) in file_instructions_dict.items()]
                 if file_change_requests:
                     return file_change_requests
             except RegexMatchError:
                 logger.warning("Failed to parse! Retrying...")
                 self.delete_messages_from_chat("files_to_change")
                 continue
-        raise Exception("Could not generate files to change")
+        raise NoFilesException()
 
-    def generate_pull_request(self) -> PullRequest:
-        pull_request = None
-        for count in range(5):
+    def generate_pull_request(self, retries=5) -> PullRequest:
+        for count in range(retries):
+            too_long = False
             try:
                 logger.info(f"Generating for the {count}th time...")
-                pr_text_response = self.chat(pull_request_prompt, message_key="pull_request")
+                if too_long or count == retries - 2: # if on last try, use gpt4-32k (improved context window)
+                    pr_text_response = self.chat(pull_request_prompt, message_key="pull_request")
+                else:
+                    pr_text_response = self.chat(pull_request_prompt, message_key="pull_request", model=SECONDARY_MODEL)
+
+                # Add triple quotes if not present
+                if not pr_text_response.strip().endswith('"""'):
+                    pr_text_response += '"""'
+
                 self.delete_messages_from_chat("pull_request")
             except Exception as e:
-                logger.warning(f"Exception {e}. Failed to parse! Retrying...")
+                e_str = str(e)
+                if "too long" in e_str:
+                    too_long = True
+                logger.warning(f"Exception {e_str}. Failed to parse! Retrying...")
                 self.delete_messages_from_chat("pull_request")
                 continue
             pull_request = PullRequest.from_string(pr_text_response)
             pull_request.branch_name = "sweep/" + pull_request.branch_name[:250]
             return pull_request
         raise Exception("Could not generate PR text")
 
@@ -116,31 +130,36 @@
     def check_path_exists(self, path: str, branch: str = ""):
         try:
             self.get_contents(path, branch)
             return True
         except Exception:
             return False
 
-    def create_branch(self, branch: str) -> str:
+    def create_branch(self, branch: str, retry=True) -> str:
         # Generate PR if nothing is supplied maybe
-        base_branch = self.repo.get_branch(self.repo.default_branch)
+        base_branch = self.repo.get_branch(SweepConfig.get_branch(self.repo))
         try:
             self.repo.create_git_ref(f"refs/heads/{branch}", base_branch.commit.sha)
             return branch
         except GithubException as e:
             logger.error(f"Error: {e}, trying with other branch names...")
-            for i in range(1, 100):
-                try:
-                    logger.warning(f"Retrying {branch}_{i}...")
-                    self.repo.create_git_ref(
-                        f"refs/heads/{branch}_{i}", base_branch.commit.sha
-                    )
-                    return f"{branch}_{i}"
-                except GithubException:
-                    pass
+            if retry:
+                for i in range(1, 100):
+                    try:
+                        logger.warning(f"Retrying {branch}_{i}...")
+                        self.repo.create_git_ref(
+                            f"refs/heads/{branch}_{i}", base_branch.commit.sha
+                        )
+                        return f"{branch}_{i}"
+                    except GithubException:
+                        pass
+            else:
+                new_branch = self.repo.get_branch(branch)
+                if new_branch:
+                    return new_branch.name
             raise e
     
     def populate_snippets(self, snippets: list[Snippet]):
         for snippet in snippets:
             try:
                 snippet.content = self.repo.get_contents(snippet.file_path, SweepConfig.get_branch(self.repo)).decoded_content.decode("utf-8")
             except Exception as e:
@@ -158,18 +177,18 @@
             query=query,
             n_results=num_snippets,
             installation_id=installation_id,
         )
         self.populate_snippets(snippets)
         return snippets
     
-    def validate_file_change_requests(self, file_change_requests: list[FileChangeRequest]):
+    def validate_file_change_requests(self, file_change_requests: list[FileChangeRequest], branch: str = ""):
         for file_change_request in file_change_requests:
             try:
-                contents = self.repo.get_contents(file_change_request.filename, SweepConfig.get_branch(self.repo))
+                contents = self.repo.get_contents(file_change_request.filename, branch or SweepConfig.get_branch(self.repo))
                 if contents:
                     file_change_request.change_type = "modify"
                 else:
                     file_change_request.change_type = "create"
             except:
                 file_change_request.change_type = "create"
         return file_change_requests
@@ -234,46 +253,47 @@
         #             response = self.chat(
         #                 f"Here is the file: <file path=\"{path}\">\n\n{content[:10000]}</file>. Fetch more content or call finish.", 
         #                 message_key=path,
         #                 functions=functions
         #             ) # update this constant
         return
 
-    def create_file(self, file_change_request: FileChangeRequest) -> FileChange:
-        file_change: FileChange | None = None
+    def create_file(self, file_change_request: FileChangeRequest) -> FileCreation:
+        file_change: FileCreation | None = None
         for count in range(5):
             key = f"file_change_created_{file_change_request.filename}"
             create_file_response = self.chat(
                 create_file_prompt.format(
                     filename=file_change_request.filename,
                     instructions=file_change_request.instructions,
                 ),
                 message_key=key,
             )
             # Add file to list of changed_files
             self.file_change_paths.append(file_change_request.filename)
             # self.delete_file_from_system_message(file_path=file_change_request.filename)
             try:
-                file_change = FileChange.from_string(create_file_response)
+                file_change = FileCreation.from_string(create_file_response)
                 assert file_change is not None
                 file_change.commit_message = f"sweep: {file_change.commit_message[:50]}"
                 return file_change
             except Exception:
                 # Todo: should we undo appending to file_change_paths?
                 logger.warning(f"Failed to parse. Retrying for the {count}th time...")
                 self.delete_messages_from_chat(key)
                 continue
         raise Exception("Failed to parse response after 5 attempts.")
 
     def modify_file(
-        self, file_change_request: FileChangeRequest, contents: str = ""
+        self, file_change_request: FileChangeRequest, contents: str = "", branch = None
     ) -> tuple[str, str]:
         if not contents:
             contents = self.get_file(
-                file_change_request.filename
+                file_change_request.filename,
+                branch=branch
             ).decoded_content.decode("utf-8")
         # Add line numbers to the contents; goes in prompts but not github
         contents_line_numbers = "\n".join([f"{i + 1}:{line}" for i, line in enumerate(contents.split("\n"))])
         contents_line_numbers = contents_line_numbers.replace('"""', "'''")
         for count in range(5):
             if "0613" in self.model:
                 """
@@ -323,18 +343,18 @@
                 try:
                     logger.info(f"modify_file_response: {modify_file_response}")
                     new_file = generate_new_file(modify_file_response, contents)
                     if not is_markdown(file_change_request.filename):
                         code_repairer = CodeRepairer(chat_logger=self.chat_logger)
                         diff = generate_diff(old_code=contents, new_code=new_file)
                         new_file = code_repairer.repair_code(diff=diff, user_code=new_file, feature=file_change_request.instructions)
-                        # new_file = revert_whitespace_changes(original_file_str=contents, modified_file_str=new_file)
                     return (new_file, file_change_request.filename)
                 except Exception as e:
-                    logger.warning(f"Recieved error {e}")
+                    tb = traceback.format_exc()
+                    logger.warning(f"Recieved error {e}\n{tb}")
                     logger.warning(
                         f"Failed to parse. Retrying for the {count}th time..."
                     )
                     self.delete_messages_from_chat(key)
                     continue
         raise Exception("Failed to parse response after 5 attempts.")
  
@@ -383,25 +403,36 @@
         except Exception as e:
             logger.info(f"Error in handle_create_file: {e}")
 
     def handle_modify_file(self, file_change_request: FileChangeRequest, branch: str, file_markdown: bool):
         try:
             contents = self.get_file(file_change_request.filename, branch=branch)
             new_file_contents, file_name = self.modify_file(
-                file_change_request, contents.decoded_content.decode("utf-8")
+                file_change_request, contents.decoded_content.decode("utf-8"), branch=branch
             )
             new_file_contents = format_contents(new_file_contents, file_markdown)
             new_file_contents = new_file_contents.rstrip()
             if contents.decoded_content.decode("utf-8").endswith("\n"):
                 new_file_contents += "\n"
             logger.debug(
                 f"{file_name}, {f'Update {file_name}'}, {new_file_contents}, {branch}"
             )
-            self.repo.update_file(
-                file_name,
-                f'Update {file_name}',
-                new_file_contents,
-                contents.sha,
-                branch=branch,
-            )
+            try:
+                self.repo.update_file(
+                    file_name,
+                    f'Update {file_name}',
+                    new_file_contents,
+                    contents.sha,
+                    branch=branch,
+                )
+            except Exception as e:
+                logger.info(f"Error in updating file, repulling and trying again {e}")
+                contents = self.get_file(file_change_request.filename, branch=branch)
+                self.repo.update_file(
+                    file_name,
+                    f'Update {file_name}',
+                    new_file_contents,
+                    contents.sha,
+                    branch=branch,
+                )
         except Exception as e:
             logger.info(f"Error in handle_modify_file: {e}")
```

### Comparing `sweepai-0.3.0/sweepai/core/vector_db.py` & `sweepai-0.4.0/sweepai/core/vector_db.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.3.0/sweepai/events.py` & `sweepai-0.4.0/sweepai/events.py`

 * *Files 19% similar despite different names*

```diff
@@ -103,8 +103,29 @@
         class MergedBy(BaseModel):
             login: str
         user: User
         merged_by: MergedBy
     class Repository(BaseModel):
         full_name: str
     pull_request: PullRequest
-    repository: Repository
+    repository: Repository
+
+class CheckRunCompleted(BaseModel):
+    class CheckRun(BaseModel):
+        class PullRequest(BaseModel):
+            number: int
+        conclusion: str
+        html_url: str
+        pull_requests: list[PullRequest]
+        @property
+        def run_id(self):
+            # format is like https://github.com/ORG/REPO_NAME/actions/runs/RUN_ID/jobs/JOB_ID
+            return self.html_url.split("/")[-3]
+    class Repository(BaseModel):
+        full_name: str
+        description: str | None
+    class Sender(BaseModel):
+        login: str
+    check_run: CheckRun
+    installation: Installation
+    repository: Repository
+    sender: Sender
```

### Comparing `sweepai-0.3.0/sweepai/handlers/on_comment.py` & `sweepai-0.4.0/sweepai/handlers/on_comment.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,28 +5,60 @@
 # TODO: Add file validation
 
 import os
 import openai
 
 from loguru import logger
 
+from sweepai.core.entities import NoFilesException, Snippet
 from sweepai.core.sweep_bot import SweepBot
 from sweepai.handlers.on_review import get_pr_diffs
 from sweepai.utils.event_logger import posthog
 from sweepai.utils.github_utils import (
     get_github_client,
     search_snippets,
 )
 from sweepai.utils.prompt_constructor import HumanMessageCommentPrompt
 from sweepai.utils.constants import PREFIX
 from sweepai.utils.chat_logger import ChatLogger
 
 github_access_token = os.environ.get("GITHUB_TOKEN")
 openai.api_key = os.environ.get("OPENAI_API_KEY")
 
+num_of_snippets_to_query = 30
+max_num_of_snippets = 3
+total_number_of_snippet_tokens = 15_000
+num_full_files = 2
+num_extended_snippets = 2
+
+def post_process_snippets(snippets: list[Snippet]):
+    for snippet in snippets[:num_full_files]:
+        snippet = snippet.expand()
+
+    # snippet fusing
+    i = 0
+    while i < len(snippets):
+        j = i + 1
+        while j < len(snippets):
+            if snippets[i] ^ snippets[j]:  # this checks for overlap
+                snippets[i] = snippets[i] | snippets[j]  # merging
+                snippets.pop(j)
+            else:
+                j += 1
+        i += 1
+
+    # truncating snippets based on character length
+    result_snippets = []
+    total_length = 0
+    for snippet in snippets:
+        total_length += len(snippet.get_snippet())
+        if total_length > total_number_of_snippet_tokens * 5:
+            break
+        result_snippets.append(snippet)
+    return result_snippets[:max_num_of_snippets]
 
 def on_comment(
     repo_full_name: str,
     repo_description: str,
     comment: str,
     pr_path: str | None,
     pr_line_position: int | None,
@@ -67,22 +99,57 @@
         # Check if the PR is closed
         if pr.state == "closed":
             return {"success": True, "message": "PR is closed. No event fired."}
         branch_name = pr.head.ref
         pr_title = pr.title
         pr_body = pr.body
         diffs = get_pr_diffs(repo, pr)
-        snippets, tree = search_snippets(repo, comment, installation_id, branch=branch_name, num_files=1 if pr_path else 3)
         pr_line = None
         pr_file_path = None
+        # This means it's a comment on a file
         if pr_path and pr_line_position:
             pr_file = repo.get_contents(pr_path, ref=branch_name).decoded_content.decode("utf-8")
             pr_lines = pr_file.splitlines()
             pr_line = pr_lines[min(len(pr_lines), pr_line_position) - 1]
             pr_file_path = pr_path.strip()
+        # This means it's a comment on the PR
+        else:
+            if not comment.strip().lower().startswith("sweep"):
+                logger.info("No event fired because it doesn't start with Sweep.")
+                return {"success": True, "message": "No event fired."}
+            
+        def fetch_file_contents_with_retry():
+            retries = 3
+            error = None
+            for i in range(retries):
+                try:
+                    logger.info(f"Fetching relevant files for the {i}th time...")
+                    return search_snippets(
+                        repo,
+                        f"{comment}\n{pr_title}" + (f"\n{pr_line}" if pr_line else ""),
+                        num_files=30,
+                        branch=branch_name,
+                        installation_id=installation_id,
+                    )
+                except Exception as e:
+                    error = e
+                    continue
+            posthog.capture(
+                username, "fetching_failed", properties={"error": error, **metadata}
+            )
+            raise error
+        snippets, tree = fetch_file_contents_with_retry()
+        logger.info("Fetching relevant files...")
+        try:
+            snippets, tree = fetch_file_contents_with_retry()
+            assert len(snippets) > 0
+        except Exception as e:
+            logger.error(e)
+            raise e
+        snippets = post_process_snippets(snippets)
 
         logger.info("Getting response from ChatGPT...")
         human_message = HumanMessageCommentPrompt(
             comment=comment,
             repo_name=repo_name,
             repo_description=repo_description if repo_description else "",
             diffs=diffs,
@@ -123,20 +190,27 @@
             "reason": "Failed to get files",
             **metadata
         })
         raise e
 
     try:
         logger.info("Fetching files to modify/create...")
-        file_change_requests = sweep_bot.get_files_to_change()
-
+        file_change_requests = sweep_bot.get_files_to_change(retries=3)
+        file_change_requests = sweep_bot.validate_file_change_requests(file_change_requests, branch=branch_name)
         logger.info("Making Code Changes...")
         sweep_bot.change_files_in_github(file_change_requests, branch_name)
 
         logger.info("Done!")
+    except NoFilesException:
+        posthog.capture(username, "failed", properties={
+            "error": "No files to change",
+            "reason": "No files to change",
+            **metadata
+        })
+        return {"success": True, "message": "No files to change."}
     except Exception as e:
         posthog.capture(username, "failed", properties={
             "error": str(e),
             "reason": "Failed to make changes",
             **metadata
         })
         raise e
```

### Comparing `sweepai-0.3.0/sweepai/handlers/on_review.py` & `sweepai-0.4.0/sweepai/handlers/on_review.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.3.0/sweepai/handlers/on_ticket.py` & `sweepai-0.4.0/sweepai/handlers/on_ticket.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,28 +7,29 @@
 import os
 import openai
 
 from loguru import logger
 import modal
 from tabulate import tabulate
 
-from sweepai.core.entities import FileChangeRequest, Snippet
+from sweepai.core.entities import FileChangeRequest, Snippet, NoFilesException
 from sweepai.core.prompts import (
     reply_prompt,
 )
 from sweepai.core.sweep_bot import SweepBot
 from sweepai.core.prompts import issue_comment_prompt
-from sweepai.handlers.create_pr import create_pr
+from sweepai.handlers.create_pr import create_pr, create_config_pr, safe_delete_sweep_branch
 from sweepai.handlers.on_comment import on_comment
 from sweepai.handlers.on_review import review_pr
 from sweepai.utils.event_logger import posthog
 from sweepai.utils.github_utils import get_github_client, search_snippets
 from sweepai.utils.prompt_constructor import HumanMessagePrompt
-from sweepai.utils.constants import DB_NAME, PREFIX, UTILS_NAME
+from sweepai.utils.constants import DB_NAME, PREFIX, UTILS_NAME, SWEEP_LOGIN
 from sweepai.utils.chat_logger import ChatLogger, discord_log_error
+from sweepai.utils.config import SweepConfig
 import traceback
 
 github_access_token = os.environ.get("GITHUB_TOKEN")
 openai.api_key = os.environ.get("OPENAI_API_KEY")
 
 update_index = modal.Function.lookup(DB_NAME, "update_index")
 
@@ -45,15 +46,15 @@
   {body}
 </details>
 '''
 
 chunker = modal.Function.lookup(UTILS_NAME, "Chunking.chunk")
 
 num_of_snippets_to_query = 30
-# max_num_of_snippets = 5
+max_num_of_snippets = 5
 total_number_of_snippet_tokens = 15_000
 num_full_files = 2
 num_extended_snippets = 2
 
 def post_process_snippets(snippets: list[Snippet]):
     for snippet in snippets[:num_full_files]:
         snippet = snippet.expand()
@@ -74,15 +75,15 @@
     result_snippets = []
     total_length = 0
     for snippet in snippets:
         total_length += len(snippet.get_snippet())
         if total_length > total_number_of_snippet_tokens * 5:
             break
         result_snippets.append(snippet)
-    return result_snippets
+    return result_snippets[:max_num_of_snippets]
 
 def on_ticket(
     title: str,
     summary: str,
     issue_number: int,
     issue_url: str,
     username: str,
@@ -124,72 +125,106 @@
     repo = g.get_repo(repo_full_name)
     current_issue = repo.get_issue(number=issue_number)
     if current_issue.state == 'closed':
         posthog.capture(username, "issue_closed", properties=metadata)
         return {"success": False, "reason": "Issue is closed"}
     item_to_react_to = current_issue.get_comment(comment_id) if comment_id else current_issue
 
+    # Check if branch was already created for this issue
+    preexisting_branch = None
+    prs = repo.get_pulls(state='open', sort='created', base=SweepConfig.get_branch(repo))
+    for pr in prs:
+        # Check if this issue is mentioned in the PR, and pr is owned by bot
+        # This is done in create_pr, (pr_description = ...)
+        if pr.user.login == SWEEP_LOGIN and f'Fixes #{issue_number}.\n' in pr.body:
+            success = safe_delete_sweep_branch(pr, repo)
+    comments = list(current_issue.get_comments())
+    if comment_id and not comments[-1].body.lower().startswith("sweep"):
+        print(comments[-1].body)
+        return {"success": True, "reason": "Comment does not start with 'Sweep', passing"}
     # Add emojis
     eyes_reaction = item_to_react_to.create_reaction("eyes")
+    # If SWEEP_BOT reacted to item_to_react_to with "rocket", then remove it.
+    reactions = item_to_react_to.get_reactions()
+    for reaction in reactions:
+        if reaction.content == "rocket" and reaction.user.login == SWEEP_LOGIN:
+            item_to_react_to.delete_reaction(reaction.id)
 
     # Creates progress bar ASCII for 0-5 states
     progress_headers = [
         None,
         "Step 1: 🔍 Code Search",
         "Step 2: 🧐 Snippet Analysis",
         "Step 3: 📝 Planning",
         "Step 4: ⌨️ Coding",
         "Step 5: 🔁 Code Review"
     ]
-    def get_progress_bar(index, errored=False, pr_message=""):
+
+    config_pr_url = None
+    def get_comment_header(index, errored=False, pr_message=""):
+        config_pr_message = ("\n" + f"* Install Sweep Configs: [Pull Request]({config_pr_url})" if config_pr_url is not None else "")
         if index < 0: index = 0
         if index == 5:
-            return pr_message
+            return pr_message + config_pr_message
         index *= 20
         index = min(100, index)
         if errored:
             return f"![{index}%](https://progress-bar.dev/{index}/?&title=Errored&width=600)"
-        return f"![{index}%](https://progress-bar.dev/{index}/?&title=Progress&width=600)" + ("\n" + stars_suffix if index != -1 else "")
+        return f"![{index}%](https://progress-bar.dev/{index}/?&title=Progress&width=600)" + ("\n" + stars_suffix + config_pr_message if index != -1 else "")
+
+    # Find the first comment made by the bot
+    issue_comment = None
+    first_comment = f"{get_comment_header(0)}\n{sep}I am currently looking into this ticket! I will update the progress of the ticket in this comment. I am currently searching through your code, looking for relevant snippets.\n{sep}## {progress_headers[1]}\nWorking on it...{bot_suffix}"
+    for comment in comments:
+        if comment.user.login == SWEEP_LOGIN:
+            issue_comment = comment
+            issue_comment.edit(first_comment)
+            break
+    if issue_comment is None:
+        issue_comment = current_issue.create_comment(first_comment)
 
-    issue_comment = current_issue.create_comment(f"{get_progress_bar(0)}\n{sep}I am currently looking into this ticket! I will update the progress of the ticket in this comment. I am currently searching through your code, looking for relevant snippets.{bot_suffix}")
+    # Comment edit function
     past_messages = {}
-    def comment_reply(message: str, index: int, pr_message = ""):
+    current_index = {}
+    def edit_sweep_comment(message: str, index: int, pr_message = ""):
+        nonlocal current_index
+        # -1 = error, -2 = retry
         # Only update the progress bar if the issue generation errors.
         errored = (index == -1)
-        current_index = index
         if index >= 0:
             past_messages[index] = message
+            current_index = index
 
-        # Include progress history
         agg_message = None
-        for i in range(current_index + 1):
-            if i in past_messages:
-                header = progress_headers[i]
-                if header is not None: header = "## " + header + "\n"
-                else: header = "No header\n"
-                msg = header + past_messages[i]
-                if agg_message is None:
-                    agg_message = msg
-                else:
-                    agg_message = agg_message + f"\n{sep}" + msg
+        # Include progress history
+        # index = -2 is reserved for
+        for i in range(current_index + 2): # go to next header (for Working on it... text)
+            if i == 0 or i >= len(progress_headers): continue # skip None header
+            header = progress_headers[i]
+            if header is not None: header = "## " + header + "\n"
+            else: header = "No header\n"
+            msg = header + (past_messages.get(i) or "Working on it...")
+            if agg_message is None:
+                agg_message = msg
+            else:
+                agg_message = agg_message + f"\n{sep}" + msg
         if errored:
-            agg_message = "## Error: 🚫 Unable to Complete PR\nIf you would like to report this bug, please join our **[Discord](https://discord.com/invite/sweep-ai)**."
+            agg_message = "## ❌ Unable to Complete PR" + '\n' + message + "\nIf you would like to report this bug, please join our **[Discord](https://discord.com/invite/sweep-ai)**."
 
         # Update the issue comment
-        issue_comment.edit(f"{get_progress_bar(current_index, errored, pr_message)}\n{sep}{agg_message}{bot_suffix}")
+        issue_comment.edit(f"{get_comment_header(current_index, errored, pr_message)}\n{sep}{agg_message}{bot_suffix}")
 
-    comments = current_issue.get_comments()
     replies_text = ""
     if comment_id:
         replies_text = "\nComments:\n" + "\n".join(
             [
                 issue_comment_prompt.format(
                     username=comment.user.login,
                     reply=comment.body,
-                ) for comment in comments
+                ) for comment in comments if comment.user.type == "User"
             ]
         )
 
     def log_error(error_type, exception):
         content = f"**{error_type} Error**\n{username}: {issue_url}\n```{exception}```"
         discord_log_error(content)
 
@@ -216,15 +251,15 @@
 
     logger.info("Fetching relevant files...")
     try:
         snippets, tree = fetch_file_contents_with_retry()
         assert len(snippets) > 0
     except Exception as e:
         logger.error(e)
-        comment_reply(
+        edit_sweep_comment(
             "It looks like an issue has occured around fetching the files. Perhaps the repo has not been initialized: try removing this repo and adding it back. I'll try again in a minute. If this error persists contact team@sweep.dev.",
             -1
         )
         log_error("File Fetch", str(e))
         raise e
     
     snippets = post_process_snippets(snippets)
@@ -251,26 +286,48 @@
         "repo_description": repo_description,
         "installation_id": installation_id,
         "comment_id": comment_id,
     })
     sweep_bot = SweepBot.from_system_message_content(
         human_message=human_message, repo=repo, is_reply=bool(comments), chat_logger=chat_logger
     )
+
+
+    # Check repository for sweep.yml file.
+    sweep_yml_exists = False
+    for content_file in repo.get_contents(""):
+        if content_file.name == "sweep.yaml":
+            sweep_yml_exists = True
+            break
+
+    # If sweep.yaml does not exist, then create a new PR that simply creates the sweep.yaml file.
+    if not sweep_yml_exists:
+        try:
+            logger.info("Creating sweep.yaml file...")
+            config_pr = create_config_pr(sweep_bot)
+            config_pr_url = config_pr.html_url
+            edit_sweep_comment(message="", index=-2)
+        except Exception as e:
+            logger.error("Failed to create new branch for sweep.yaml file.\n", e)
+    else:
+        logger.info("sweep.yaml file already exists.")
+
+
     sweepbot_retries = 3
     try:
         for i in range(sweepbot_retries):
             # ANALYZE SNIPPETS
             if sweep_bot.model == "gpt-4-32k-0613":
                 logger.info("CoT retrieval...")
                 sweep_bot.cot_retrieval()
             else:
                 logger.info("Did not execute CoT retrieval...")
 
             newline = '\n'
-            comment_reply(
+            edit_sweep_comment(
                 "I found the following snippets in your repository. I will now analyze this snippets and come up with a plan."
                 + "\n\n"
                 + collapsible_template.format(
                     summary="Some code snippets I looked at (click to expand). If some file is missing from here, you can mention the path in the ticket description.",
                     body="\n".join(
                         [
                             f"https://github.com/{organization}/{repo_name}/blob/{repo.get_commits()[0].sha}/{snippet.file_path}#L{max(snippet.start, 1)}-L{min(snippet.end, snippet.content.count(newline))}\n"
@@ -287,37 +344,37 @@
             file_change_requests = sweep_bot.get_files_to_change()
             file_change_requests = sweep_bot.validate_file_change_requests(file_change_requests)
             table = tabulate(
                 [[f"`{file_change_request.filename}`", file_change_request.instructions] for file_change_request in file_change_requests],
                 headers=["File Path", "Proposed Changes"],
                 tablefmt="pipe"
             )
-            comment_reply(
+            edit_sweep_comment(
                 "From looking through the relevant snippets, I decided to make the following modifications:\n\n" + table + "\n\n",
                 2
             )
 
             # CREATE PR METADATA
             logger.info("Generating PR...")
             pull_request = sweep_bot.generate_pull_request()
             pull_request_content = pull_request.content.strip().replace("\n", "\n>")
             pull_request_summary = f"**{pull_request.title}**\n`{pull_request.branch_name}`\n>{pull_request_content}\n"
 
-            comment_reply(
+            edit_sweep_comment(
                 f"I have created a plan for writing the pull request. I am now working on executing my plan and coding the required changes to address this issue. Here is the planned pull request:\n\n{pull_request_summary}",
                 3
             )
 
             # WRITE PULL REQUEST
             logger.info("Making PR...")
             response = create_pr(file_change_requests, pull_request, sweep_bot, username, installation_id, issue_number)
             if not response or not response["success"]: raise Exception("Failed to create PR")
             pr = response["pull_request"]
             current_issue.create_reaction("rocket")
-            comment_reply(
+            edit_sweep_comment(
                 "I have finished coding the issue. I am now reviewing it for completeness.",
                 4
             )
 
             try:
                 current_issue.delete_reaction(eyes_reaction.id)
             except:
@@ -338,24 +395,27 @@
                             pr_line_position=None,
                             pr_number=pr.number)
             except Exception as e:
                 logger.error(traceback.format_exc())
                 logger.error(e)
 
             # Completed code review
-            comment_reply(
+            edit_sweep_comment(
                 "Success! 🚀",
                 5,
                 pr_message=f"## Here's the PR! [https://github.com/{repo_full_name}/pull/{pr.number}](https://github.com/{repo_full_name}/pull/{pr.number})",
             )
 
             break
+    except NoFilesException:
+        logger.info("No files to change.")
+        edit_sweep_comment("Sorry, I could find any appropriate files to edit to address this issue. If this is a mistake, please provide more context and I will retry!", -1)
     except openai.error.InvalidRequestError as e:
         logger.error(e)
-        comment_reply(
+        edit_sweep_comment(
             "I'm sorry, but it looks our model has ran out of context length. We're trying to make this happen less, but one way to mitigate this is to code smaller files. If this error persists contact team@sweep.dev.",
             -1
         )
         log_error("Context Length", str(e))
         posthog.capture(
             username,
             "failed",
@@ -364,15 +424,15 @@
                 "reason": "Invalid request error / context length",
                 **metadata,
             },
         )
         raise e
     except Exception as e:
         logger.error(e)
-        comment_reply(
+        edit_sweep_comment(
             "I'm sorry, but it looks like an error has occured. Try removing and re-adding the sweep label. If this error persists contact team@sweep.dev.",
             -1
         )
         log_error("Workflow", str(e))
         posthog.capture(
             username,
             "failed",
```

### Comparing `sweepai-0.3.0/sweepai/utils/chat_logger.py` & `sweepai-0.4.0/sweepai/utils/chat_logger.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.3.0/sweepai/utils/config.py` & `sweepai-0.4.0/sweepai/utils/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -31,8 +31,19 @@
                 return branch_name
             except Exception as e:
                 logger.warning(f"Error when getting branch: {e}, creating branch")
                 repo.create_git_ref(f"refs/heads/{branch_name}", repo.get_branch(default_branch).commit.sha)
                 return branch_name
         except Exception as e:
             logger.warning(f"Error when getting branch: {e}, falling back to default branch")
-            return default_branch
+            return default_branch
+
+    @staticmethod
+    @lru_cache(maxsize=None)
+    def get_gha_enabled(repo: Repository) -> bool:
+        try:
+            contents = repo.get_contents(".github/sweep.yaml")
+            gha_enabled = yaml.safe_load(contents.decoded_content.decode("utf-8"))["gha_enabled"]
+            return gha_enabled
+        except Exception as e:
+            logger.warning(f"Error when getting gha enabled: {e}, falling back to False")
+            return False
```

### Comparing `sweepai-0.3.0/sweepai/utils/diff.py` & `sweepai-0.4.0/sweepai/utils/diff.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,18 +40,18 @@
     
     # Handle small files
     if len(lines) <= 5:
         start_idx = 0
         end_idx = len(lines)
         for idx, line in enumerate(lines):
             if start_idx == 0 and line.strip().startswith('```'):
-                start_idx = idx
+                start_idx = idx + 1
             if start_idx != 0 and line.strip().endswith('```'):
                 end_idx = idx
-        lines = lines[start_idx + 1:end_idx]
+        lines = lines[start_idx:end_idx]
         return '\n'.join(lines)
 
     first_three_lines = lines[:3]
     last_three_lines = lines[-3:]
     first_line_idx = 0
     last_line_idx = 3
     for idx, line in enumerate(first_three_lines):
@@ -79,28 +79,45 @@
     new_file = re.search(r".*?<new_file>(.*)<\/new_file>", modify_file_response, re.DOTALL).group(1).strip()
     if "<copy_lines" not in new_file:
         return new_file
 
     # v5
     result = []
     lines = new_file.split('\n')
-    for line in lines:
+    for line_number, line in enumerate(lines):
         # Todo: make it support 1 number only
         matches = re.finditer(r"<copy_lines\s(\d+-\d+)>", line)
+        copied_lines = False
         for match in matches:
+            copied_lines = True
             start, end = match.group(1).split('-')
             start, end = int(start)-1, int(end)-1
 
             start = max(0, start)
             end = min(len(old_file_lines) - 1, end)
 
             replacements = old_file_lines[start:end + 1]
             replacements_str = '\n'.join(replacements)
             line = line.replace(match.group(0), replacements_str)
-        result.append(line)
+
+        # check if line was incorrectly duplicated
+        append = True
+        if not copied_lines: # if bot generated, and line before is not bot generated
+            if len(result) > 0:
+                # Get last line in results
+                last_group = result[-1]
+                #last_line = last_group
+                if '\n' in last_group:
+                    last_line = last_group[last_group.rindex('\n')+1:] # if its multiple lines
+                    # if last line is same is current line
+                    if last_line == line:
+                        append = False
+
+        if append:
+            result.append(line)
     result = '\n'.join(result)
 
     # Todo: v4 is inefficient; deprecated
     """
     first_section_idx = new_file.index("<copied>")
     if first_section_idx > 0:
         result_file += new_file[:first_section_idx]
```

### Comparing `sweepai-0.3.0/sweepai/utils/event_logger.py` & `sweepai-0.4.0/sweepai/utils/event_logger.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.3.0/sweepai/utils/file_change_functions.py` & `sweepai-0.4.0/sweepai/utils/file_change_functions.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.3.0/sweepai/utils/github_utils.py` & `sweepai-0.4.0/sweepai/utils/github_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.3.0/sweepai/utils/huggingface.py` & `sweepai-0.4.0/sweepai/utils/huggingface.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.3.0/sweepai/utils/prompt_constructor.py` & `sweepai-0.4.0/sweepai/utils/prompt_constructor.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.3.0/sweepai/utils/scorer.py` & `sweepai-0.4.0/sweepai/utils/scorer.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.3.0/sweepai/utils/snippets.py` & `sweepai-0.4.0/sweepai/utils/snippets.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.3.0/sweepai/utils/utils.py` & `sweepai-0.4.0/sweepai/utils/utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.3.0/setup.py` & `sweepai-0.4.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 
 entry_points = \
 {'console_scripts': ['sweep = sweepai.app.cli:app',
                      'sweepai = sweepai.app.cli:app']}
 
 setup_kwargs = {
     'name': 'sweepai',
-    'version': '0.3.0',
+    'version': '0.4.0',
     'description': 'Sweep software chores',
-    'long_description': '\n<p align="center">\n    <img src="https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-3e61f57ad233">\n</p>\n<p align="center">\n    <i>Bug Reports & Feature Requests ⟶&nbsp; Code Changes</i>\n</p>\n\n<p align="center">\n<a href="https://sweep.dev">\n    <img alt="Landing Page" src="https://img.shields.io/badge/Site-sweep.dev-blue?link=https%3A%2F%2Fsweep.dev">\n</a>\n<a href="https://docs.sweep.dev/">\n    <img alt="Docs" src="https://img.shields.io/badge/Docs-docs.sweep.dev-blue?link=https%3A%2F%2Fdocs.sweep.dev">\n</a> \n<a href="https://discord.gg/sweep-ai">\n    <img src="https://dcbadge.vercel.app/api/server/sweep-ai?style=flat" />\n</a>\n<img alt="PyPI" src="https://img.shields.io/pypi/v/sweepai">\n<a href="https://pepy.tech/project/sweepai">\n    <img src="https://static.pepy.tech/badge/sweepai/week" />\n</a>\n<a href="https://github.com/sweepai/sweep">\n    <img src="https://img.shields.io/github/stars/sweepai/sweep" />\n</a>\n<a href="https://twitter.com/sweep__ai">\n    <img src="https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fsweep__ai" />\n</a>\n</p>\n\n<b>Sweep</b> allows you to create and review GitHub issues with ease.\nSimply describe any issue and Sweep will do the rest.\nIt will plan out what needs to be done, what changes to make, and write the changes to a PR. \n\nSupported languages: Python, Javascript/Typescript, Rust, Go, Java/C#, C++ and anything else GPT-4 supports\n\n---\n\n## ✨ Demo\nFor the best experience, [install Sweep](https://github.com/apps/sweep-ai) to one of your repos and see the magic happen.\n\n[Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47)\n\n## 🌠 Features\n* Automatic interactive bug fixes & feature development\n* PR auto self-review + comment handling (effectively [Reflexion](https://arxiv.org/abs/2303.11366))\n* Address developer comments after PR is created using PR replies & code comments\n* Code snippets embedding-based semantic & popularity search ([🔍 Rebuilding our Search Engine in a Day](https://docs.sweep.dev/how-we-rebuilt-our-code-search-engine-in-a-day))\n* Chain-of-Thought retrieval using GPT Functions\n* 🎊 New: Sweep Chat, a local interface for Sweep (see below)\n\n## 🚀 Getting Started\n\n### 🖥️ Sweep Chat\nSweep Chat allows you to interact with Sweep locally and will sync with GitHub. You can plan out your changes with Sweep, and then Sweep can create a pull request for you. \n\n1. Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos\n\n2. Run `pip install sweepai && sweep`. Note that you need python 3.10 or greater.\n\n3. This should spin up a GitHub auth flow in your browser. Copy-paste the 🔵 blue 8-digit code from your terminal into the page. Then wait a few seconds and it should spin up Sweep Chat. You should only need to do the auth once.\n\n4. Pick a repo from the dropdown at the top (the Github app must be installed on this repo). Then start chatting with Sweep Chat. Relevant searched files will show up on the right. Sweep Chat can make PRs if you ask it to create a PR. \n<img src="https://github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-screenshot.png">\n\n💡 You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.\n\n#### From Source\nIf you want the nightly build and or if the latest build has issues.\n\n1. `git clone https://github.com/sweepai/sweep && poetry install`\n2. `python sweepai/app/cli.py`. Note that you need python 3.10 or greater.\n\n### ✨ Sweep Github App\nSetting up Sweep is as simple as adding the GitHub bot to a repo, then creating an issue for the bot to address.\n\n1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos\n2. Create new issue in repo, like "Sweep: Write tests"\n3. "👀" means it is taking a look, and it will generate the desired code\n4. "🚀" means the bot has finished its job and created a PR\n\n## 🤝 Contributing\n\nContributions are welcome and greatly appreciated! For detailed guidelines on how to contribute, please see the [CONTRIBUTING.md](CONTRIBUTING.md) file. In essence, you\'ll need to fork the repository, create a new branch for your feature or bug fix, commit your changes, and open a pull request.\nFor more detailed docs, see [🚀 Quickstart](https://docs.sweep.dev/start).\n\n---\n\n## 📘 Story\n\nWe were frustrated by small tickets, like simple bug fixes, annoying refactors, and small features, each task requiring us to open our IDE to fix simple bugs. So, we decided to leverage the capabilities of ChatGPT to address this directly in GitHub.\n\nUnlike existing AI solutions, this can solve entire tickets and can be parallelized: developers can spin up 10 tickets and Sweep will address them all at once.\n\n## 📚 The Stack\n- GPT-4 32k 0613 (default) / Claude v1.3 100k\n- ActiveLoop DeepLake for Vector DB with MiniLM L12 as our embeddings model\n- Modal Labs for infra + deployment\n- Gradio for Sweep Chat\n\n## 🗺️ Roadmap\nWe\'re currently working on responding to linters and external search. For more, see [🗺️ Roadmap](https://docs.sweep.dev/roadmap).\n\n## ⭐ Star History\n\n[![Star History Chart](https://api.star-history.com/svg?repos=sweepai/sweep&type=Date)](https://star-history.com/#sweepai/sweep&Date)\n\nConsider starring us if you\'re using Sweep so more people hear about us!\n\n---\n\n<h2 align="center">\n    Contributors\n</h2>\n<p align="center">\n    Thank you for your contribution!\n</p>\n<p align="center">\n    <a href="https://github.com/sweepai/sweep/graphs/contributors">\n      <img src="https://contrib.rocks/image?repo=sweepai/sweep" />\n    </a>\n</p>\n<p align="center">\n    and, of course, Sweep!\n</p>\n\n',
+    'long_description': '<p align="center">\n    <img src="https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-3e61f57ad233">\n</p>\n<p align="center">\n    <i>Bug Reports & Feature Requests ⟶&nbsp; Code Changes</i>\n</p>\n\n<p align="center">\n<a href="https://sweep.dev">\n    <img alt="Landing Page" src="https://img.shields.io/badge/Site-sweep.dev-blue?link=https%3A%2F%2Fsweep.dev">\n</a>\n<a href="https://docs.sweep.dev/">\n    <img alt="Docs" src="https://img.shields.io/badge/Docs-docs.sweep.dev-blue?link=https%3A%2F%2Fdocs.sweep.dev">\n</a> \n<a href="https://discord.gg/sweep-ai">\n    <img src="https://dcbadge.vercel.app/api/server/sweep-ai?style=flat" />\n</a>\n<img alt="PyPI" src="https://img.shields.io/pypi/v/sweepai">\n<a href="https://pepy.tech/project/sweepai">\n    <img src="https://static.pepy.tech/badge/sweepai/month" />\n</a>\n<a href="https://github.com/sweepai/sweep">\n    <img src="https://img.shields.io/github/stars/sweepai/sweep" />\n</a>\n<a href="https://twitter.com/sweep__ai">\n    <img src="https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fsweep__ai" />\n</a>\n</p>\n\n<b>Sweep</b> is an AI junior developer that transforms bug reports & feature requests into code changes.\n\nDescribe bugs, small features, and refactors like you would to a junior developer, and Sweep:\n1. 🔍 reads your codebase\n2. 📝 plans the changes\n3. ⚡**writes a pull request with code**⚡\n\nSee highlights at https://docs.sweep.dev/examples.\n\n## ✨ Demo\nFor the best experience, [install Sweep](https://github.com/apps/sweep-ai) to one of your repos and see the magic happen.\n\n[Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47)\n\n## 🌠 Sweep\n* 🔧 Turns issues directly into pull requests (without an IDE)\n* 👀 Addresses developer replies & comments on its PRs\n* 🕵️\u200d♂️ Uses embedding-based code search, with popularity reranking for repository-level code understanding ([🔍 Rebuilding our Search Engine in a Day](https://docs.sweep.dev/how-we-rebuilt-our-code-search-engine-in-a-day))\n* 🎊 New: Fixes PRs based on Github Actions feedback\n* 🎊 New: Sweep Chat, a local interface for Sweep (see below)\n\n## 🚀 Getting Started\n\n### 🍲 Recipes\n#### To get the best performance from Sweep, we recommend the following approach to writing github issues/chats. \nFor harder problems, try to provide the same information a human would need. For simpler problems, providing a single line and a file name should suffice.\n\nA good issue might include:\n\n| Where to look <br> **[file name or function name]**| What to do <br> **[change the logic to do this]** | Additional Context (optional) <br> **[there\'s a bug/we need this feature/there\'s this dependency]** |\n|-----------|------------|----------------------|\n|In `sweepai/app/ui.py`|use an os-agnostic temp directory|N/A|\n|In `on_comment.py`|we should not fire an event|because it\'s possible that the comment is on a closed PR|\n|In the config loader in `packages/server/src/config.ts`|add a third option called "env" to load the config settings from environment variables| At present, there are two options:  1. ... and 2. ...|\n\nIf you want Sweep to use a file, try to mention the full path. Similarly, to have Sweep use a function, try to mention the class method or what it does. Also see [✨ Tips and tricks for Sweep](https://docs.sweep.dev/tricks).\n\n### 🖥️ Sweep Chat\nSweep Chat allows you to interact with Sweep and GitHub locally. Collaborate on the plan with Sweep, then have it create the pull request for you. \n\n**Prerequisites:** Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to your repository\n\n1. Run `pip install sweepai && sweep`. Note that you need **python 3.10+.**\n    - This runs GitHub authentication in your browser. \n\n2. Copy the 🔵 blue 8-digit code from your terminal into the page. You should only need to do the authentication once.  \n    - Wait a few seconds and Sweep Chat will start. \n\n3. Choose a repository from the dropdown at the top (the Github app must be installed to this repository).\n\n    - ⚡ Start chatting with Sweep Chat! ⚡\n\n<img src="https://github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-screenshot.png">\n\nTips:\n* 🔍 Relevant searched files will show up on the right. \n* 🔘 Sweep Chat creates PRs when the "Create PR" button is clicked. \n* 💡 You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.\n\n#### From Source\nIf you want the nightly build and or if the latest build has issues.\n\n1. `git clone https://github.com/sweepai/sweep && poetry install`\n2. `python sweepai/app/cli.py`. Note that you need **python 3.10+**.\n\n### ✨ Sweep Github App\nSetting up Sweep is as simple as adding the GitHub bot to a repo, then creating an issue for the bot to address.\nWe support all languages GPT4 supports, including Python, Typescript, Rust, Go, Java, C# and C++.\n\n1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos\n2. Create new issue in repo, like "Sweep: Write tests"\n3. Watch the magic happen 🪄\n\n## 🤝 Contributing\n\nContributions are welcome and greatly appreciated! For detailed guidelines on how to contribute, please see the [CONTRIBUTING.md](CONTRIBUTING.md) file.\nFor more detailed docs, see [🚀 Quickstart](https://docs.sweep.dev/start).\n\n## 📘 Story\n\nWe were frustrated by small tickets, like simple bug fixes, annoying refactors, and small features. Each task required us to open our IDE to fix simple bugs. So we decided to leverage the capabilities of ChatGPT to address this directly in GitHub.\n\nUnlike existing AI solutions, this can solve entire tickets and can be parallelized + asynchronous: developers can spin up 10 tickets and Sweep will address them all at once.\n\n## 📚 The Stack\n- GPT-4 32k 0613 (default)\n- ActiveLoop DeepLake for Vector DB with MiniLM L12 as our embeddings model\n- Modal Labs for infra + deployment\n- Gradio for Sweep Chat\n\n## 🗺️ Roadmap\nSee [🗺️ Roadmap](https://docs.sweep.dev/roadmap)\n\n## ⭐ Star History\n\n[![Star History Chart](https://api.star-history.com/svg?repos=sweepai/sweep&type=Date)](https://star-history.com/#sweepai/sweep&Date)\n\nConsider starring us if you\'re using Sweep so more people hear about us!\n<h2 align="center">\n    Contributors\n</h2>\n<p align="center">\n    Thank you for your contribution!\n</p>\n<p align="center">\n    <a href="https://github.com/sweepai/sweep/graphs/contributors">\n      <img src="https://contrib.rocks/image?repo=sweepai/sweep" />\n    </a>\n</p>\n<p align="center">\n    and, of course, Sweep!\n</p>\n',
     'author': 'Kevin Lu',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,86 +1,100 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['sweepai',
 'sweepai.app', 'sweepai.core', 'sweepai.handlers', 'sweepai.utils']
 package_data = \ {'': ['*']} install_requires = \ ['GitPython>=3.1.31,<4.0.0',
 'PyGithub==1.58.2', 'config-path>=1.0.3,<2.0.0', 'gradio>=3.35.2,<4.0.0',
 'loguru>=0.6.0,<0.7.0', 'requests>=2.28.2,<3.0.0', 'tabulate>=0.9.0,<0.10.0',
 'typer>=0.9.0,<0.10.0', 'urllib3>=2.0.3,<3.0.0'] entry_points = \
 {'console_scripts': ['sweep = sweepai.app.cli:app', 'sweepai = sweepai.app.cli:
-app']} setup_kwargs = { 'name': 'sweepai', 'version': '0.3.0', 'description':
-'Sweep software chores', 'long_description': '\n
+app']} setup_kwargs = { 'name': 'sweepai', 'version': '0.4.0', 'description':
+'Sweep software chores', 'long_description': '
  \n [https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-
                                 3e61f57ad233]\n
 \n
              \n Bug Reports & Feature Requests â¶  Code Changes\n
 \n\n
 \n\n_[Landing_Page]\n\n\n_[Docs]\n \n\n_[https://dcbadge.vercel.app/api/server/
   sweep-ai?style=flat]\n\n[PyPI]\n\n_[https://static.pepy.tech/badge/sweepai/
-week]\n\n\n_[https://img.shields.io/github/stars/sweepai/sweep]\n\n\n_[https://
-   img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fsweep__ai]\n\n
-\n\nSweep allows you to create and review GitHub issues with ease.\nSimply
-describe any issue and Sweep will do the rest.\nIt will plan out what needs to
-be done, what changes to make, and write the changes to a PR. \n\nSupported
-languages: Python, Javascript/Typescript, Rust, Go, Java/C#, C++ and anything
-else GPT-4 supports\n\n---\n\n## â¨ Demo\nFor the best experience, [install
-Sweep](https://github.com/apps/sweep-ai) to one of your repos and see the magic
-happen.\n\n[Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-
-7317-40a7-9b5e-0af02f2b0e47)\n\n## ð  Features\n* Automatic interactive bug
-fixes & feature development\n* PR auto self-review + comment handling
-(effectively [Reflexion](https://arxiv.org/abs/2303.11366))\n* Address
-developer comments after PR is created using PR replies & code comments\n* Code
-snippets embedding-based semantic & popularity search ([ð Rebuilding our
-Search Engine in a Day](https://docs.sweep.dev/how-we-rebuilt-our-code-search-
-engine-in-a-day))\n* Chain-of-Thought retrieval using GPT Functions\n* ð
-New: Sweep Chat, a local interface for Sweep (see below)\n\n## ð Getting
-Started\n\n### ð¥ï¸ Sweep Chat\nSweep Chat allows you to interact with Sweep
-locally and will sync with GitHub. You can plan out your changes with Sweep,
-and then Sweep can create a pull request for you. \n\n1. Install [Sweep GitHub
-app](https://github.com/apps/sweep-ai) to desired repos\n\n2. Run `pip install
-sweepai && sweep`. Note that you need python 3.10 or greater.\n\n3. This should
-spin up a GitHub auth flow in your browser. Copy-paste the ðµ blue 8-digit
-code from your terminal into the page. Then wait a few seconds and it should
-spin up Sweep Chat. You should only need to do the auth once.\n\n4. Pick a repo
-from the dropdown at the top (the Github app must be installed on this repo).
-Then start chatting with Sweep Chat. Relevant searched files will show up on
-the right. Sweep Chat can make PRs if you ask it to create a PR. \n[https://
-github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/
-gradio-screenshot.png]\n\nð¡ You can force dark mode by going to http://
-127.0.0.1:7861/?__theme=dark.\n\n#### From Source\nIf you want the nightly
-build and or if the latest build has issues.\n\n1. `git clone https://
-github.com/sweepai/sweep && poetry install`\n2. `python sweepai/app/cli.py`.
-Note that you need python 3.10 or greater.\n\n### â¨ Sweep Github App\nSetting
-up Sweep is as simple as adding the GitHub bot to a repo, then creating an
-issue for the bot to address.\n\n1. Add the [Sweep GitHub app](https://
-github.com/apps/sweep-ai) to desired repos\n2. Create new issue in repo, like
-"Sweep: Write tests"\n3. "ð" means it is taking a look, and it will generate
-the desired code\n4. "ð" means the bot has finished its job and created a
-PR\n\n## ð¤ Contributing\n\nContributions are welcome and greatly
-appreciated! For detailed guidelines on how to contribute, please see the
-[CONTRIBUTING.md](CONTRIBUTING.md) file. In essence, you\'ll need to fork the
-repository, create a new branch for your feature or bug fix, commit your
-changes, and open a pull request.\nFor more detailed docs, see [ð
-Quickstart](https://docs.sweep.dev/start).\n\n---\n\n## ð Story\n\nWe were
-frustrated by small tickets, like simple bug fixes, annoying refactors, and
-small features, each task requiring us to open our IDE to fix simple bugs. So,
-we decided to leverage the capabilities of ChatGPT to address this directly in
-GitHub.\n\nUnlike existing AI solutions, this can solve entire tickets and can
-be parallelized: developers can spin up 10 tickets and Sweep will address them
-all at once.\n\n## ð The Stack\n- GPT-4 32k 0613 (default) / Claude v1.3
-100k\n- ActiveLoop DeepLake for Vector DB with MiniLM L12 as our embeddings
-model\n- Modal Labs for infra + deployment\n- Gradio for Sweep Chat\n\n##
-ðºï¸ Roadmap\nWe\'re currently working on responding to linters and external
-search. For more, see [ðºï¸ Roadmap](https://docs.sweep.dev/roadmap).\n\n##
-â­ Star History\n\n[![Star History Chart](https://api.star-history.com/
-svg?repos=sweepai/sweep&type=Date)](https://star-history.com/#sweepai/
-sweep&Date)\n\nConsider starring us if you\'re using Sweep so more people hear
-about us!\n\n---\n\n
+month]\n\n\n_[https://img.shields.io/github/stars/sweepai/sweep]\n\n\n_[https:/
+  /img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fsweep__ai]\n\n
+\n\nSweep is an AI junior developer that transforms bug reports & feature
+requests into code changes.\n\nDescribe bugs, small features, and refactors
+like you would to a junior developer, and Sweep:\n1. ð reads your
+codebase\n2. ð plans the changes\n3. â¡**writes a pull request with
+code**â¡\n\nSee highlights at https://docs.sweep.dev/examples.\n\n## â¨
+Demo\nFor the best experience, [install Sweep](https://github.com/apps/sweep-
+ai) to one of your repos and see the magic happen.\n\n[Demo](https://
+github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-
+0af02f2b0e47)\n\n## ð  Sweep\n* ð§ Turns issues directly into pull requests
+(without an IDE)\n* ð Addresses developer replies & comments on its PRs\n*
+ðµï¸\u200dâï¸ Uses embedding-based code search, with popularity reranking
+for repository-level code understanding ([ð Rebuilding our Search Engine in
+a Day](https://docs.sweep.dev/how-we-rebuilt-our-code-search-engine-in-a-
+day))\n* ð New: Fixes PRs based on Github Actions feedback\n* ð New:
+Sweep Chat, a local interface for Sweep (see below)\n\n## ð Getting
+Started\n\n### ð² Recipes\n#### To get the best performance from Sweep, we
+recommend the following approach to writing github issues/chats. \nFor harder
+problems, try to provide the same information a human would need. For simpler
+problems, providing a single line and a file name should suffice.\n\nA good
+issue might include:\n\n| Where to look
+**[file name or function name]**| What to do
+**[change the logic to do this]** | Additional Context (optional)
+**[there\'s a bug/we need this feature/there\'s this dependency]** |\n|--------
+---|------------|----------------------|\n|In `sweepai/app/ui.py`|use an os-
+agnostic temp directory|N/A|\n|In `on_comment.py`|we should not fire an
+event|because it\'s possible that the comment is on a closed PR|\n|In the
+config loader in `packages/server/src/config.ts`|add a third option called
+"env" to load the config settings from environment variables| At present, there
+are two options: 1. ... and 2. ...|\n\nIf you want Sweep to use a file, try to
+mention the full path. Similarly, to have Sweep use a function, try to mention
+the class method or what it does. Also see [â¨ Tips and tricks for Sweep]
+(https://docs.sweep.dev/tricks).\n\n### ð¥ï¸ Sweep Chat\nSweep Chat allows
+you to interact with Sweep and GitHub locally. Collaborate on the plan with
+Sweep, then have it create the pull request for you. \n\n**Prerequisites:**
+Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to your
+repository\n\n1. Run `pip install sweepai && sweep`. Note that you need
+**python 3.10+.**\n - This runs GitHub authentication in your browser. \n\n2.
+Copy the ðµ blue 8-digit code from your terminal into the page. You should
+only need to do the authentication once. \n - Wait a few seconds and Sweep Chat
+will start. \n\n3. Choose a repository from the dropdown at the top (the Github
+app must be installed to this repository).\n\n - â¡ Start chatting with Sweep
+Chat! â¡\n\n[https://github.com/sweepai/sweep/blob/
+856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-
+screenshot.png]\n\nTips:\n* ð Relevant searched files will show up on the
+right. \n* ð Sweep Chat creates PRs when the "Create PR" button is clicked.
+\n* ð¡ You can force dark mode by going to http://127.0.0.1:7861/
+?__theme=dark.\n\n#### From Source\nIf you want the nightly build and or if the
+latest build has issues.\n\n1. `git clone https://github.com/sweepai/sweep &&
+poetry install`\n2. `python sweepai/app/cli.py`. Note that you need **python
+3.10+**.\n\n### â¨ Sweep Github App\nSetting up Sweep is as simple as adding
+the GitHub bot to a repo, then creating an issue for the bot to address.\nWe
+support all languages GPT4 supports, including Python, Typescript, Rust, Go,
+Java, C# and C++.\n\n1. Add the [Sweep GitHub app](https://github.com/apps/
+sweep-ai) to desired repos\n2. Create new issue in repo, like "Sweep: Write
+tests"\n3. Watch the magic happen ðª\n\n## ð¤ Contributing\n\nContributions
+are welcome and greatly appreciated! For detailed guidelines on how to
+contribute, please see the [CONTRIBUTING.md](CONTRIBUTING.md) file.\nFor more
+detailed docs, see [ð Quickstart](https://docs.sweep.dev/start).\n\n## ð
+Story\n\nWe were frustrated by small tickets, like simple bug fixes, annoying
+refactors, and small features. Each task required us to open our IDE to fix
+simple bugs. So we decided to leverage the capabilities of ChatGPT to address
+this directly in GitHub.\n\nUnlike existing AI solutions, this can solve entire
+tickets and can be parallelized + asynchronous: developers can spin up 10
+tickets and Sweep will address them all at once.\n\n## ð The Stack\n- GPT-
+4 32k 0613 (default)\n- ActiveLoop DeepLake for Vector DB with MiniLM L12 as
+our embeddings model\n- Modal Labs for infra + deployment\n- Gradio for Sweep
+Chat\n\n## ðºï¸ Roadmap\nSee [ðºï¸ Roadmap](https://docs.sweep.dev/
+roadmap)\n\n## â­ Star History\n\n[![Star History Chart](https://api.star-
+history.com/svg?repos=sweepai/sweep&type=Date)](https://star-history.com/
+#sweepai/sweep&Date)\n\nConsider starring us if you\'re using Sweep so more
+people hear about us!\n
                          ***** \n Contributors\n *****
 \n
                      \n Thank you for your contribution!\n
 \n
           \n \n_[https://contrib.rocks/image?repo=sweepai/sweep]\n\n
 \n
                           \n and, of course, Sweep!\n
-\n\n', 'author': 'Kevin Lu', 'author_email': None, 'maintainer': None,
+\n', 'author': 'Kevin Lu', 'author_email': None, 'maintainer': None,
 'maintainer_email': None, 'url': None, 'packages': packages, 'package_data':
 package_data, 'install_requires': install_requires, 'entry_points':
 entry_points, 'python_requires': '>=3.10,<4.0', } setup(**setup_kwargs)
```

### Comparing `sweepai-0.3.0/PKG-INFO` & `sweepai-0.4.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweepai
-Version: 0.3.0
+Version: 0.4.0
 Summary: Sweep software chores
 Author: Kevin Lu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: GitPython (>=3.1.31,<4.0.0)
@@ -19,15 +19,14 @@
 Project-URL: Bug Tracker, https://github.com/sweepai/sweep/issues
 Project-URL: Community, https://discord.gg/sweep-ai
 Project-URL: documentation, https://docs.sweep.dev
 Project-URL: homepage, https://sweep.dev
 Project-URL: repository, https://github.com/sweepai/sweep
 Description-Content-Type: text/markdown
 
-
 <p align="center">
     <img src="https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-3e61f57ad233">
 </p>
 <p align="center">
     <i>Bug Reports & Feature Requests ⟶&nbsp; Code Changes</i>
 </p>
 
@@ -39,105 +38,122 @@
     <img alt="Docs" src="https://img.shields.io/badge/Docs-docs.sweep.dev-blue?link=https%3A%2F%2Fdocs.sweep.dev">
 </a> 
 <a href="https://discord.gg/sweep-ai">
     <img src="https://dcbadge.vercel.app/api/server/sweep-ai?style=flat" />
 </a>
 <img alt="PyPI" src="https://img.shields.io/pypi/v/sweepai">
 <a href="https://pepy.tech/project/sweepai">
-    <img src="https://static.pepy.tech/badge/sweepai/week" />
+    <img src="https://static.pepy.tech/badge/sweepai/month" />
 </a>
 <a href="https://github.com/sweepai/sweep">
     <img src="https://img.shields.io/github/stars/sweepai/sweep" />
 </a>
 <a href="https://twitter.com/sweep__ai">
     <img src="https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fsweep__ai" />
 </a>
 </p>
 
-<b>Sweep</b> allows you to create and review GitHub issues with ease.
-Simply describe any issue and Sweep will do the rest.
-It will plan out what needs to be done, what changes to make, and write the changes to a PR. 
+<b>Sweep</b> is an AI junior developer that transforms bug reports & feature requests into code changes.
 
-Supported languages: Python, Javascript/Typescript, Rust, Go, Java/C#, C++ and anything else GPT-4 supports
+Describe bugs, small features, and refactors like you would to a junior developer, and Sweep:
+1. 🔍 reads your codebase
+2. 📝 plans the changes
+3. ⚡**writes a pull request with code**⚡
 
----
+See highlights at https://docs.sweep.dev/examples.
 
 ## ✨ Demo
 For the best experience, [install Sweep](https://github.com/apps/sweep-ai) to one of your repos and see the magic happen.
 
 [Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47)
 
-## 🌠 Features
-* Automatic interactive bug fixes & feature development
-* PR auto self-review + comment handling (effectively [Reflexion](https://arxiv.org/abs/2303.11366))
-* Address developer comments after PR is created using PR replies & code comments
-* Code snippets embedding-based semantic & popularity search ([🔍 Rebuilding our Search Engine in a Day](https://docs.sweep.dev/how-we-rebuilt-our-code-search-engine-in-a-day))
-* Chain-of-Thought retrieval using GPT Functions
+## 🌠 Sweep
+* 🔧 Turns issues directly into pull requests (without an IDE)
+* 👀 Addresses developer replies & comments on its PRs
+* 🕵️‍♂️ Uses embedding-based code search, with popularity reranking for repository-level code understanding ([🔍 Rebuilding our Search Engine in a Day](https://docs.sweep.dev/how-we-rebuilt-our-code-search-engine-in-a-day))
+* 🎊 New: Fixes PRs based on Github Actions feedback
 * 🎊 New: Sweep Chat, a local interface for Sweep (see below)
 
 ## 🚀 Getting Started
 
+### 🍲 Recipes
+#### To get the best performance from Sweep, we recommend the following approach to writing github issues/chats. 
+For harder problems, try to provide the same information a human would need. For simpler problems, providing a single line and a file name should suffice.
+
+A good issue might include:
+
+| Where to look <br> **[file name or function name]**| What to do <br> **[change the logic to do this]** | Additional Context (optional) <br> **[there's a bug/we need this feature/there's this dependency]** |
+|-----------|------------|----------------------|
+|In `sweepai/app/ui.py`|use an os-agnostic temp directory|N/A|
+|In `on_comment.py`|we should not fire an event|because it's possible that the comment is on a closed PR|
+|In the config loader in `packages/server/src/config.ts`|add a third option called "env" to load the config settings from environment variables| At present, there are two options:  1. ... and 2. ...|
+
+If you want Sweep to use a file, try to mention the full path. Similarly, to have Sweep use a function, try to mention the class method or what it does. Also see [✨ Tips and tricks for Sweep](https://docs.sweep.dev/tricks).
+
 ### 🖥️ Sweep Chat
-Sweep Chat allows you to interact with Sweep locally and will sync with GitHub. You can plan out your changes with Sweep, and then Sweep can create a pull request for you. 
+Sweep Chat allows you to interact with Sweep and GitHub locally. Collaborate on the plan with Sweep, then have it create the pull request for you. 
+
+**Prerequisites:** Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to your repository
+
+1. Run `pip install sweepai && sweep`. Note that you need **python 3.10+.**
+    - This runs GitHub authentication in your browser. 
 
-1. Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos
+2. Copy the 🔵 blue 8-digit code from your terminal into the page. You should only need to do the authentication once.  
+    - Wait a few seconds and Sweep Chat will start. 
 
-2. Run `pip install sweepai && sweep`. Note that you need python 3.10 or greater.
+3. Choose a repository from the dropdown at the top (the Github app must be installed to this repository).
 
-3. This should spin up a GitHub auth flow in your browser. Copy-paste the 🔵 blue 8-digit code from your terminal into the page. Then wait a few seconds and it should spin up Sweep Chat. You should only need to do the auth once.
+    - ⚡ Start chatting with Sweep Chat! ⚡
 
-4. Pick a repo from the dropdown at the top (the Github app must be installed on this repo). Then start chatting with Sweep Chat. Relevant searched files will show up on the right. Sweep Chat can make PRs if you ask it to create a PR. 
 <img src="https://github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-screenshot.png">
 
-💡 You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.
+Tips:
+* 🔍 Relevant searched files will show up on the right. 
+* 🔘 Sweep Chat creates PRs when the "Create PR" button is clicked. 
+* 💡 You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.
 
 #### From Source
 If you want the nightly build and or if the latest build has issues.
 
 1. `git clone https://github.com/sweepai/sweep && poetry install`
-2. `python sweepai/app/cli.py`. Note that you need python 3.10 or greater.
+2. `python sweepai/app/cli.py`. Note that you need **python 3.10+**.
 
 ### ✨ Sweep Github App
 Setting up Sweep is as simple as adding the GitHub bot to a repo, then creating an issue for the bot to address.
+We support all languages GPT4 supports, including Python, Typescript, Rust, Go, Java, C# and C++.
 
 1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos
 2. Create new issue in repo, like "Sweep: Write tests"
-3. "👀" means it is taking a look, and it will generate the desired code
-4. "🚀" means the bot has finished its job and created a PR
+3. Watch the magic happen 🪄
 
 ## 🤝 Contributing
 
-Contributions are welcome and greatly appreciated! For detailed guidelines on how to contribute, please see the [CONTRIBUTING.md](CONTRIBUTING.md) file. In essence, you'll need to fork the repository, create a new branch for your feature or bug fix, commit your changes, and open a pull request.
+Contributions are welcome and greatly appreciated! For detailed guidelines on how to contribute, please see the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 For more detailed docs, see [🚀 Quickstart](https://docs.sweep.dev/start).
 
----
-
 ## 📘 Story
 
-We were frustrated by small tickets, like simple bug fixes, annoying refactors, and small features, each task requiring us to open our IDE to fix simple bugs. So, we decided to leverage the capabilities of ChatGPT to address this directly in GitHub.
+We were frustrated by small tickets, like simple bug fixes, annoying refactors, and small features. Each task required us to open our IDE to fix simple bugs. So we decided to leverage the capabilities of ChatGPT to address this directly in GitHub.
 
-Unlike existing AI solutions, this can solve entire tickets and can be parallelized: developers can spin up 10 tickets and Sweep will address them all at once.
+Unlike existing AI solutions, this can solve entire tickets and can be parallelized + asynchronous: developers can spin up 10 tickets and Sweep will address them all at once.
 
 ## 📚 The Stack
-- GPT-4 32k 0613 (default) / Claude v1.3 100k
+- GPT-4 32k 0613 (default)
 - ActiveLoop DeepLake for Vector DB with MiniLM L12 as our embeddings model
 - Modal Labs for infra + deployment
 - Gradio for Sweep Chat
 
 ## 🗺️ Roadmap
-We're currently working on responding to linters and external search. For more, see [🗺️ Roadmap](https://docs.sweep.dev/roadmap).
+See [🗺️ Roadmap](https://docs.sweep.dev/roadmap)
 
 ## ⭐ Star History
 
 [![Star History Chart](https://api.star-history.com/svg?repos=sweepai/sweep&type=Date)](https://star-history.com/#sweepai/sweep&Date)
 
 Consider starring us if you're using Sweep so more people hear about us!
-
----
-
 <h2 align="center">
     Contributors
 </h2>
 <p align="center">
     Thank you for your contribution!
 </p>
 <p align="center">
@@ -145,8 +161,7 @@
       <img src="https://contrib.rocks/image?repo=sweepai/sweep" />
     </a>
 </p>
 <p align="center">
     and, of course, Sweep!
 </p>
 
-
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sweepai Version: 0.3.0 Summary: Sweep software
+Metadata-Version: 2.1 Name: sweepai Version: 0.4.0 Summary: Sweep software
 chores Author: Kevin Lu Requires-Python: >=3.10,<4.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: GitPython
 (>=3.1.31,<4.0.0) Requires-Dist: PyGithub (==1.58.2) Requires-Dist: config-path
 (>=1.0.3,<2.0.0) Requires-Dist: gradio (>=3.35.2,<4.0.0) Requires-Dist: loguru
 (>=0.6.0,<0.7.0) Requires-Dist: requests (>=2.28.2,<3.0.0) Requires-Dist:
 tabulate (>=0.9.0,<0.10.0) Requires-Dist: typer (>=0.9.0,<0.10.0) Requires-
@@ -11,69 +11,82 @@
 Project-URL: documentation, https://docs.sweep.dev Project-URL: homepage,
 https://sweep.dev Project-URL: repository, https://github.com/sweepai/sweep
 Description-Content-Type: text/markdown
   [https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-
                                  3e61f57ad233]
                Bug Reports & Feature Requests â¶  Code Changes
       [Landing_Page] [Docs] [https://dcbadge.vercel.app/api/server/sweep-
- ai?style=flat] [PyPI] [https://static.pepy.tech/badge/sweepai/week] [https://
+ai?style=flat] [PyPI] [https://static.pepy.tech/badge/sweepai/month] [https://
   img.shields.io/github/stars/sweepai/sweep] [https://img.shields.io/twitter/
                 url?url=https%3A%2F%2Ftwitter.com%2Fsweep__ai]
-Sweep allows you to create and review GitHub issues with ease. Simply describe
-any issue and Sweep will do the rest. It will plan out what needs to be done,
-what changes to make, and write the changes to a PR. Supported languages:
-Python, Javascript/Typescript, Rust, Go, Java/C#, C++ and anything else GPT-
-4 supports --- ## â¨ Demo For the best experience, [install Sweep](https://
-github.com/apps/sweep-ai) to one of your repos and see the magic happen. [Demo]
-(https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-
-0af02f2b0e47) ## ð  Features * Automatic interactive bug fixes & feature
-development * PR auto self-review + comment handling (effectively [Reflexion]
-(https://arxiv.org/abs/2303.11366)) * Address developer comments after PR is
-created using PR replies & code comments * Code snippets embedding-based
-semantic & popularity search ([ð Rebuilding our Search Engine in a Day]
-(https://docs.sweep.dev/how-we-rebuilt-our-code-search-engine-in-a-day)) *
-Chain-of-Thought retrieval using GPT Functions * ð New: Sweep Chat, a local
-interface for Sweep (see below) ## ð Getting Started ### ð¥ï¸ Sweep Chat
-Sweep Chat allows you to interact with Sweep locally and will sync with GitHub.
-You can plan out your changes with Sweep, and then Sweep can create a pull
-request for you. 1. Install [Sweep GitHub app](https://github.com/apps/sweep-
-ai) to desired repos 2. Run `pip install sweepai && sweep`. Note that you need
-python 3.10 or greater. 3. This should spin up a GitHub auth flow in your
-browser. Copy-paste the ðµ blue 8-digit code from your terminal into the
-page. Then wait a few seconds and it should spin up Sweep Chat. You should only
-need to do the auth once. 4. Pick a repo from the dropdown at the top (the
-Github app must be installed on this repo). Then start chatting with Sweep
-Chat. Relevant searched files will show up on the right. Sweep Chat can make
-PRs if you ask it to create a PR. [https://github.com/sweepai/sweep/blob/
-856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-screenshot.png] ð¡
+Sweep is an AI junior developer that transforms bug reports & feature requests
+into code changes. Describe bugs, small features, and refactors like you would
+to a junior developer, and Sweep: 1. ð reads your codebase 2. ð plans the
+changes 3. â¡**writes a pull request with code**â¡ See highlights at https://
+docs.sweep.dev/examples. ## â¨ Demo For the best experience, [install Sweep]
+(https://github.com/apps/sweep-ai) to one of your repos and see the magic
+happen. [Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-
+40a7-9b5e-0af02f2b0e47) ## ð  Sweep * ð§ Turns issues directly into pull
+requests (without an IDE) * ð Addresses developer replies & comments on its
+PRs * ðµï¸ââï¸ Uses embedding-based code search, with popularity
+reranking for repository-level code understanding ([ð Rebuilding our Search
+Engine in a Day](https://docs.sweep.dev/how-we-rebuilt-our-code-search-engine-
+in-a-day)) * ð New: Fixes PRs based on Github Actions feedback * ð New:
+Sweep Chat, a local interface for Sweep (see below) ## ð Getting Started ###
+ð² Recipes #### To get the best performance from Sweep, we recommend the
+following approach to writing github issues/chats. For harder problems, try to
+provide the same information a human would need. For simpler problems,
+providing a single line and a file name should suffice. A good issue might
+include: | Where to look
+**[file name or function name]**| What to do
+**[change the logic to do this]** | Additional Context (optional)
+**[there's a bug/we need this feature/there's this dependency]** | |-----------
+|------------|----------------------| |In `sweepai/app/ui.py`|use an os-
+agnostic temp directory|N/A| |In `on_comment.py`|we should not fire an
+event|because it's possible that the comment is on a closed PR| |In the config
+loader in `packages/server/src/config.ts`|add a third option called "env" to
+load the config settings from environment variables| At present, there are two
+options: 1. ... and 2. ...| If you want Sweep to use a file, try to mention the
+full path. Similarly, to have Sweep use a function, try to mention the class
+method or what it does. Also see [â¨ Tips and tricks for Sweep](https://
+docs.sweep.dev/tricks). ### ð¥ï¸ Sweep Chat Sweep Chat allows you to
+interact with Sweep and GitHub locally. Collaborate on the plan with Sweep,
+then have it create the pull request for you. **Prerequisites:** Install [Sweep
+GitHub app](https://github.com/apps/sweep-ai) to your repository 1. Run `pip
+install sweepai && sweep`. Note that you need **python 3.10+.** - This runs
+GitHub authentication in your browser. 2. Copy the ðµ blue 8-digit code from
+your terminal into the page. You should only need to do the authentication
+once. - Wait a few seconds and Sweep Chat will start. 3. Choose a repository
+from the dropdown at the top (the Github app must be installed to this
+repository). - â¡ Start chatting with Sweep Chat! â¡ [https://github.com/
+sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-
+screenshot.png] Tips: * ð Relevant searched files will show up on the right.
+* ð Sweep Chat creates PRs when the "Create PR" button is clicked. * ð¡
 You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark. ####
 From Source If you want the nightly build and or if the latest build has
 issues. 1. `git clone https://github.com/sweepai/sweep && poetry install` 2.
-`python sweepai/app/cli.py`. Note that you need python 3.10 or greater. ### â¨
-Sweep Github App Setting up Sweep is as simple as adding the GitHub bot to a
-repo, then creating an issue for the bot to address. 1. Add the [Sweep GitHub
-app](https://github.com/apps/sweep-ai) to desired repos 2. Create new issue in
-repo, like "Sweep: Write tests" 3. "ð" means it is taking a look, and it
-will generate the desired code 4. "ð" means the bot has finished its job and
-created a PR ## ð¤ Contributing Contributions are welcome and greatly
-appreciated! For detailed guidelines on how to contribute, please see the
-[CONTRIBUTING.md](CONTRIBUTING.md) file. In essence, you'll need to fork the
-repository, create a new branch for your feature or bug fix, commit your
-changes, and open a pull request. For more detailed docs, see [ð Quickstart]
-(https://docs.sweep.dev/start). --- ## ð Story We were frustrated by small
-tickets, like simple bug fixes, annoying refactors, and small features, each
-task requiring us to open our IDE to fix simple bugs. So, we decided to
-leverage the capabilities of ChatGPT to address this directly in GitHub. Unlike
-existing AI solutions, this can solve entire tickets and can be parallelized:
+`python sweepai/app/cli.py`. Note that you need **python 3.10+**. ### â¨ Sweep
+Github App Setting up Sweep is as simple as adding the GitHub bot to a repo,
+then creating an issue for the bot to address. We support all languages GPT4
+supports, including Python, Typescript, Rust, Go, Java, C# and C++. 1. Add the
+[Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos 2. Create
+new issue in repo, like "Sweep: Write tests" 3. Watch the magic happen ðª ##
+ð¤ Contributing Contributions are welcome and greatly appreciated! For
+detailed guidelines on how to contribute, please see the [CONTRIBUTING.md]
+(CONTRIBUTING.md) file. For more detailed docs, see [ð Quickstart](https://
+docs.sweep.dev/start). ## ð Story We were frustrated by small tickets, like
+simple bug fixes, annoying refactors, and small features. Each task required us
+to open our IDE to fix simple bugs. So we decided to leverage the capabilities
+of ChatGPT to address this directly in GitHub. Unlike existing AI solutions,
+this can solve entire tickets and can be parallelized + asynchronous:
 developers can spin up 10 tickets and Sweep will address them all at once. ##
-ð The Stack - GPT-4 32k 0613 (default) / Claude v1.3 100k - ActiveLoop
-DeepLake for Vector DB with MiniLM L12 as our embeddings model - Modal Labs for
-infra + deployment - Gradio for Sweep Chat ## ðºï¸ Roadmap We're currently
-working on responding to linters and external search. For more, see [ðºï¸
-Roadmap](https://docs.sweep.dev/roadmap). ## â­ Star History [![Star History
-Chart](https://api.star-history.com/svg?repos=sweepai/sweep&type=Date)](https:/
-/star-history.com/#sweepai/sweep&Date) Consider starring us if you're using
-Sweep so more people hear about us! ---
+ð The Stack - GPT-4 32k 0613 (default) - ActiveLoop DeepLake for Vector DB
+with MiniLM L12 as our embeddings model - Modal Labs for infra + deployment -
+Gradio for Sweep Chat ## ðºï¸ Roadmap See [ðºï¸ Roadmap](https://
+docs.sweep.dev/roadmap) ## â­ Star History [![Star History Chart](https://
+api.star-history.com/svg?repos=sweepai/sweep&type=Date)](https://star-
+history.com/#sweepai/sweep&Date) Consider starring us if you're using Sweep so
+more people hear about us!
                            ***** Contributors *****
                        Thank you for your contribution!
                [https://contrib.rocks/image?repo=sweepai/sweep]
                             and, of course, Sweep!
```

