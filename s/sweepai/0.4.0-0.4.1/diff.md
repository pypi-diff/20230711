# Comparing `tmp/sweepai-0.4.0.tar.gz` & `tmp/sweepai-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sweepai-0.4.0.tar", max compression
+gzip compressed data, was "sweepai-0.4.1.tar", max compression
```

## Comparing `sweepai-0.4.0.tar` & `sweepai-0.4.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0    20850 2023-06-14 10:05:39.263813 sweepai-0.4.0/LICENSE
--rw-r--r--   0        0        0     6573 2023-07-11 09:19:39.419375 sweepai-0.4.0/README.md
--rw-r--r--   0        0        0     1395 2023-07-11 09:19:43.389381 sweepai-0.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.0/sweepai/__init__.py
--rw-r--r--   0        0        0    12062 2023-07-11 09:19:39.419375 sweepai-0.4.0/sweepai/api.py
--rw-r--r--   0        0        0     6020 2023-07-11 09:20:00.556075 sweepai-0.4.0/sweepai/app/api_client.py
--rw-r--r--   0        0        0    10421 2023-07-11 09:19:39.419375 sweepai-0.4.0/sweepai/app/backend.py
--rw-r--r--   0        0        0     1166 2023-07-09 08:40:46.465379 sweepai-0.4.0/sweepai/app/cli.py
--rw-r--r--   0        0        0     3583 2023-07-11 09:19:39.419375 sweepai-0.4.0/sweepai/app/config.py
--rw-r--r--   0        0        0    14559 2023-07-11 09:19:39.419375 sweepai-0.4.0/sweepai/app/ui.py
--rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.0/sweepai/core/__init__.py
--rw-r--r--   0        0        0    17400 2023-07-08 21:39:15.812977 sweepai-0.4.0/sweepai/core/chat.py
--rw-r--r--   0        0        0     2867 2023-07-11 09:19:39.419375 sweepai-0.4.0/sweepai/core/code_repair.py
--rw-r--r--   0        0        0     8395 2023-07-11 09:19:39.419375 sweepai-0.4.0/sweepai/core/entities.py
--rw-r--r--   0        0        0      561 2023-07-11 09:19:39.419375 sweepai-0.4.0/sweepai/core/gha_extraction.py
--rw-r--r--   0        0        0    16814 2023-07-11 09:19:39.419375 sweepai-0.4.0/sweepai/core/prompts.py
--rw-r--r--   0        0        0     3496 2023-07-07 20:46:56.696885 sweepai-0.4.0/sweepai/core/react.py
--rw-r--r--   0        0        0    19671 2023-07-11 09:19:39.419375 sweepai-0.4.0/sweepai/core/sweep_bot.py
--rw-r--r--   0        0        0    12695 2023-07-09 08:40:46.468712 sweepai-0.4.0/sweepai/core/vector_db.py
--rw-r--r--   0        0        0     3176 2023-07-11 09:19:39.419375 sweepai-0.4.0/sweepai/events.py
--rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.0/sweepai/handlers/__init__.py
--rw-r--r--   0        0        0     6475 2023-07-11 09:19:39.419375 sweepai-0.4.0/sweepai/handlers/create_pr.py
--rw-r--r--   0        0        0     2571 2023-07-11 09:19:39.419375 sweepai-0.4.0/sweepai/handlers/on_check_suite.py
--rw-r--r--   0        0        0     9391 2023-07-11 09:19:39.419375 sweepai-0.4.0/sweepai/handlers/on_comment.py
--rw-r--r--   0        0        0     4003 2023-07-09 00:27:16.396539 sweepai-0.4.0/sweepai/handlers/on_review.py
--rw-r--r--   0        0        0    18039 2023-07-11 09:19:39.419375 sweepai-0.4.0/sweepai/handlers/on_ticket.py
--rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.0/sweepai/utils/__init__.py
--rw-r--r--   0        0        0     1808 2023-07-07 20:46:56.696885 sweepai-0.4.0/sweepai/utils/chat_logger.py
--rw-r--r--   0        0        0     2001 2023-07-11 09:19:39.419375 sweepai-0.4.0/sweepai/utils/config.py
--rw-r--r--   0        0        0      964 2023-07-11 09:20:17.826102 sweepai-0.4.0/sweepai/utils/constants.py
--rw-r--r--   0        0        0     6529 2023-07-11 09:19:39.419375 sweepai-0.4.0/sweepai/utils/diff.py
--rw-r--r--   0        0        0      719 2023-07-07 20:46:56.696885 sweepai-0.4.0/sweepai/utils/event_logger.py
--rw-r--r--   0        0        0     5245 2023-07-07 20:46:56.700219 sweepai-0.4.0/sweepai/utils/file_change_functions.py
--rw-r--r--   0        0        0     8225 2023-07-09 08:40:46.468712 sweepai-0.4.0/sweepai/utils/github_utils.py
--rw-r--r--   0        0        0       98 2023-07-07 20:46:56.700219 sweepai-0.4.0/sweepai/utils/hash.py
--rw-r--r--   0        0        0      822 2023-07-07 20:46:56.700219 sweepai-0.4.0/sweepai/utils/huggingface.py
--rw-r--r--   0        0        0     5564 2023-07-07 20:46:56.700219 sweepai-0.4.0/sweepai/utils/prompt_constructor.py
--rw-r--r--   0        0        0      848 2023-07-07 20:46:56.700219 sweepai-0.4.0/sweepai/utils/scorer.py
--rw-r--r--   0        0        0     1498 2023-07-07 20:46:56.700219 sweepai-0.4.0/sweepai/utils/snippets.py
--rw-r--r--   0        0        0    11291 2023-07-07 20:46:56.700219 sweepai-0.4.0/sweepai/utils/utils.py
--rw-r--r--   0        0        0     7743 2023-07-11 09:29:47.564605 sweepai-0.4.0/setup.py
--rw-r--r--   0        0        0     7525 2023-07-11 09:29:47.565034 sweepai-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    20850 2023-06-14 10:05:39.263813 sweepai-0.4.1/LICENSE
+-rw-r--r--   0        0        0     6678 2023-07-11 20:05:05.034619 sweepai-0.4.1/README.md
+-rw-r--r--   0        0        0     1395 2023-07-11 20:18:44.748666 sweepai-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.1/sweepai/__init__.py
+-rw-r--r--   0        0        0    12248 2023-07-11 20:05:05.034619 sweepai-0.4.1/sweepai/api.py
+-rw-r--r--   0        0        0     6020 2023-07-11 09:20:00.556075 sweepai-0.4.1/sweepai/app/api_client.py
+-rw-r--r--   0        0        0    10421 2023-07-11 09:19:39.419375 sweepai-0.4.1/sweepai/app/backend.py
+-rw-r--r--   0        0        0     1166 2023-07-09 08:40:46.465379 sweepai-0.4.1/sweepai/app/cli.py
+-rw-r--r--   0        0        0     3583 2023-07-11 09:19:39.419375 sweepai-0.4.1/sweepai/app/config.py
+-rw-r--r--   0        0        0    14559 2023-07-11 09:19:39.419375 sweepai-0.4.1/sweepai/app/ui.py
+-rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.1/sweepai/core/__init__.py
+-rw-r--r--   0        0        0    17400 2023-07-08 21:39:15.812977 sweepai-0.4.1/sweepai/core/chat.py
+-rw-r--r--   0        0        0     2867 2023-07-11 09:19:39.419375 sweepai-0.4.1/sweepai/core/code_repair.py
+-rw-r--r--   0        0        0     8306 2023-07-11 20:16:30.901906 sweepai-0.4.1/sweepai/core/entities.py
+-rw-r--r--   0        0        0      561 2023-07-11 09:19:39.419375 sweepai-0.4.1/sweepai/core/gha_extraction.py
+-rw-r--r--   0        0        0    16814 2023-07-11 09:19:39.419375 sweepai-0.4.1/sweepai/core/prompts.py
+-rw-r--r--   0        0        0     3496 2023-07-07 20:46:56.696885 sweepai-0.4.1/sweepai/core/react.py
+-rw-r--r--   0        0        0    19671 2023-07-11 09:19:39.419375 sweepai-0.4.1/sweepai/core/sweep_bot.py
+-rw-r--r--   0        0        0    12695 2023-07-09 08:40:46.468712 sweepai-0.4.1/sweepai/core/vector_db.py
+-rw-r--r--   0        0        0     3176 2023-07-11 09:19:39.419375 sweepai-0.4.1/sweepai/events.py
+-rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.1/sweepai/handlers/__init__.py
+-rw-r--r--   0        0        0     6475 2023-07-11 09:19:39.419375 sweepai-0.4.1/sweepai/handlers/create_pr.py
+-rw-r--r--   0        0        0     2571 2023-07-11 09:19:39.419375 sweepai-0.4.1/sweepai/handlers/on_check_suite.py
+-rw-r--r--   0        0        0     9391 2023-07-11 09:19:39.419375 sweepai-0.4.1/sweepai/handlers/on_comment.py
+-rw-r--r--   0        0        0     4003 2023-07-09 00:27:16.396539 sweepai-0.4.1/sweepai/handlers/on_review.py
+-rw-r--r--   0        0        0    17844 2023-07-11 20:05:05.034619 sweepai-0.4.1/sweepai/handlers/on_ticket.py
+-rw-r--r--   0        0        0        0 2023-07-07 20:46:56.696885 sweepai-0.4.1/sweepai/utils/__init__.py
+-rw-r--r--   0        0        0     1808 2023-07-07 20:46:56.696885 sweepai-0.4.1/sweepai/utils/chat_logger.py
+-rw-r--r--   0        0        0     2001 2023-07-11 09:19:39.419375 sweepai-0.4.1/sweepai/utils/config.py
+-rw-r--r--   0        0        0      964 2023-07-11 09:20:17.826102 sweepai-0.4.1/sweepai/utils/constants.py
+-rw-r--r--   0        0        0     6529 2023-07-11 09:19:39.419375 sweepai-0.4.1/sweepai/utils/diff.py
+-rw-r--r--   0        0        0      719 2023-07-07 20:46:56.696885 sweepai-0.4.1/sweepai/utils/event_logger.py
+-rw-r--r--   0        0        0     5245 2023-07-07 20:46:56.700219 sweepai-0.4.1/sweepai/utils/file_change_functions.py
+-rw-r--r--   0        0        0     8225 2023-07-09 08:40:46.468712 sweepai-0.4.1/sweepai/utils/github_utils.py
+-rw-r--r--   0        0        0       98 2023-07-07 20:46:56.700219 sweepai-0.4.1/sweepai/utils/hash.py
+-rw-r--r--   0        0        0      822 2023-07-07 20:46:56.700219 sweepai-0.4.1/sweepai/utils/huggingface.py
+-rw-r--r--   0        0        0     5564 2023-07-07 20:46:56.700219 sweepai-0.4.1/sweepai/utils/prompt_constructor.py
+-rw-r--r--   0        0        0      848 2023-07-07 20:46:56.700219 sweepai-0.4.1/sweepai/utils/scorer.py
+-rw-r--r--   0        0        0     1498 2023-07-07 20:46:56.700219 sweepai-0.4.1/sweepai/utils/snippets.py
+-rw-r--r--   0        0        0    11291 2023-07-07 20:46:56.700219 sweepai-0.4.1/sweepai/utils/utils.py
+-rw-r--r--   0        0        0     7849 2023-07-11 20:19:37.916061 sweepai-0.4.1/setup.py
+-rw-r--r--   0        0        0     7630 2023-07-11 20:19:37.916592 sweepai-0.4.1/PKG-INFO
```

### Comparing `sweepai-0.4.0/LICENSE` & `sweepai-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.0/README.md` & `sweepai-0.4.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -65,16 +65,17 @@
 If you want Sweep to use a file, try to mention the full path. Similarly, to have Sweep use a function, try to mention the class method or what it does. Also see [✨ Tips and tricks for Sweep](https://docs.sweep.dev/tricks).
 
 ### 🖥️ Sweep Chat
 Sweep Chat allows you to interact with Sweep and GitHub locally. Collaborate on the plan with Sweep, then have it create the pull request for you. 
 
 **Prerequisites:** Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to your repository
 
-1. Run `pip install sweepai && sweep`. Note that you need **python 3.10+.**
-    - This runs GitHub authentication in your browser. 
+1. Run `pip3 install sweepai && sweep`. Note that you need **python 3.10+.**
+    - Alternatively run `pip3 install --force-reinstall sweepai && sweep` if the previous command fails.
+    - This runs GitHub authentication in your browser.
 
 2. Copy the 🔵 blue 8-digit code from your terminal into the page. You should only need to do the authentication once.  
     - Wait a few seconds and Sweep Chat will start. 
 
 3. Choose a repository from the dropdown at the top (the Github app must be installed to this repository).
 
     - ⚡ Start chatting with Sweep Chat! ⚡
```

#### html2text {}

```diff
@@ -34,26 +34,27 @@
 load the config settings from environment variables| At present, there are two
 options: 1. ... and 2. ...| If you want Sweep to use a file, try to mention the
 full path. Similarly, to have Sweep use a function, try to mention the class
 method or what it does. Also see [â¨ Tips and tricks for Sweep](https://
 docs.sweep.dev/tricks). ### ð¥ï¸ Sweep Chat Sweep Chat allows you to
 interact with Sweep and GitHub locally. Collaborate on the plan with Sweep,
 then have it create the pull request for you. **Prerequisites:** Install [Sweep
-GitHub app](https://github.com/apps/sweep-ai) to your repository 1. Run `pip
-install sweepai && sweep`. Note that you need **python 3.10+.** - This runs
-GitHub authentication in your browser. 2. Copy the ðµ blue 8-digit code from
-your terminal into the page. You should only need to do the authentication
-once. - Wait a few seconds and Sweep Chat will start. 3. Choose a repository
-from the dropdown at the top (the Github app must be installed to this
-repository). - â¡ Start chatting with Sweep Chat! â¡ [https://github.com/
-sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-
-screenshot.png] Tips: * ð Relevant searched files will show up on the right.
-* ð Sweep Chat creates PRs when the "Create PR" button is clicked. * ð¡
-You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark. ####
-From Source If you want the nightly build and or if the latest build has
+GitHub app](https://github.com/apps/sweep-ai) to your repository 1. Run `pip3
+install sweepai && sweep`. Note that you need **python 3.10+.** - Alternatively
+run `pip3 install --force-reinstall sweepai && sweep` if the previous command
+fails. - This runs GitHub authentication in your browser. 2. Copy the ðµ blue
+8-digit code from your terminal into the page. You should only need to do the
+authentication once. - Wait a few seconds and Sweep Chat will start. 3. Choose
+a repository from the dropdown at the top (the Github app must be installed to
+this repository). - â¡ Start chatting with Sweep Chat! â¡ [https://
+github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/
+gradio-screenshot.png] Tips: * ð Relevant searched files will show up on the
+right. * ð Sweep Chat creates PRs when the "Create PR" button is clicked. *
+ð¡ You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.
+#### From Source If you want the nightly build and or if the latest build has
 issues. 1. `git clone https://github.com/sweepai/sweep && poetry install` 2.
 `python sweepai/app/cli.py`. Note that you need **python 3.10+**. ### â¨ Sweep
 Github App Setting up Sweep is as simple as adding the GitHub bot to a repo,
 then creating an issue for the bot to address. We support all languages GPT4
 supports, including Python, Typescript, Rust, Go, Java, C# and C++. 1. Add the
 [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos 2. Create
 new issue in repo, like "Sweep: Write tests" 3. Watch the magic happen ðª ##
```

### Comparing `sweepai-0.4.0/pyproject.toml` & `sweepai-0.4.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sweepai"
-version = "0.4.0"
+version = "0.4.1"
 description = "Sweep software chores"
 authors = ["Kevin Lu", "William Zeng", "Luke Jagg"]
 packages = [{ include = "sweepai" }]
 classifiers = ["Programming Language :: Python :: 3.11"]
 readme = "README.md"
 
 [tool.poetry.urls]
```

### Comparing `sweepai-0.4.0/sweepai/api.py` & `sweepai-0.4.1/sweepai/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,14 +130,18 @@
                 if request.issue is not None \
                     and "sweep" in [label.name.lower() for label in request.issue.labels] \
                     and request.comment.user.type == "User":
                     request.issue.body = request.issue.body or ""
                     request.repository.description = (
                         request.repository.description or ""
                     )
+
+                    if not request.comment.body.lower().startswith("sweep"):
+                        return {"success": True, "reason": "Comment does not start with 'Sweep', passing"}
+
                     # Update before we handle the ticket to make sure index is up to date
                     # other ways suboptimal
                     handle_ticket.spawn(
                         request.issue.title,
                         request.issue.body,
                         request.issue.number,
                         request.issue.html_url,
```

### Comparing `sweepai-0.4.0/sweepai/app/api_client.py` & `sweepai-0.4.1/sweepai/app/api_client.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.0/sweepai/app/backend.py` & `sweepai-0.4.1/sweepai/app/backend.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.0/sweepai/app/cli.py` & `sweepai-0.4.1/sweepai/app/cli.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.0/sweepai/app/config.py` & `sweepai-0.4.1/sweepai/app/config.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.0/sweepai/app/ui.py` & `sweepai-0.4.1/sweepai/app/ui.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.0/sweepai/core/chat.py` & `sweepai-0.4.1/sweepai/core/chat.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.0/sweepai/core/code_repair.py` & `sweepai-0.4.1/sweepai/core/code_repair.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.0/sweepai/core/entities.py` & `sweepai-0.4.1/sweepai/core/entities.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 import os
 import re
 import string
 from typing import ClassVar, Literal, Type, TypeVar
 from loguru import logger
 from pydantic import BaseModel
 
-try:   # Python 3.11+
-    from typing import Self
-except ImportError:  # Python 3.10
-    Self = TypeVar("Self", bound="RegexMatchableBaseModel")
+Self = TypeVar("Self", bound="RegexMatchableBaseModel")
 
 
 class Message(BaseModel):
     role: Literal["system"] | Literal["user"] | Literal["assistant"] | Literal["function"]
     content: str | None = None
     name: str | None = None
     function_call: dict | None = None
```

### Comparing `sweepai-0.4.0/sweepai/core/gha_extraction.py` & `sweepai-0.4.1/sweepai/core/gha_extraction.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.0/sweepai/core/prompts.py` & `sweepai-0.4.1/sweepai/core/prompts.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.0/sweepai/core/react.py` & `sweepai-0.4.1/sweepai/core/react.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.0/sweepai/core/sweep_bot.py` & `sweepai-0.4.1/sweepai/core/sweep_bot.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.0/sweepai/core/vector_db.py` & `sweepai-0.4.1/sweepai/core/vector_db.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.0/sweepai/events.py` & `sweepai-0.4.1/sweepai/events.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.0/sweepai/handlers/create_pr.py` & `sweepai-0.4.1/sweepai/handlers/create_pr.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.0/sweepai/handlers/on_check_suite.py` & `sweepai-0.4.1/sweepai/handlers/on_check_suite.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.0/sweepai/handlers/on_comment.py` & `sweepai-0.4.1/sweepai/handlers/on_comment.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.0/sweepai/handlers/on_review.py` & `sweepai-0.4.1/sweepai/handlers/on_review.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.0/sweepai/handlers/on_ticket.py` & `sweepai-0.4.1/sweepai/handlers/on_ticket.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,18 +133,17 @@
     preexisting_branch = None
     prs = repo.get_pulls(state='open', sort='created', base=SweepConfig.get_branch(repo))
     for pr in prs:
         # Check if this issue is mentioned in the PR, and pr is owned by bot
         # This is done in create_pr, (pr_description = ...)
         if pr.user.login == SWEEP_LOGIN and f'Fixes #{issue_number}.\n' in pr.body:
             success = safe_delete_sweep_branch(pr, repo)
+
     comments = list(current_issue.get_comments())
-    if comment_id and not comments[-1].body.lower().startswith("sweep"):
-        print(comments[-1].body)
-        return {"success": True, "reason": "Comment does not start with 'Sweep', passing"}
+
     # Add emojis
     eyes_reaction = item_to_react_to.create_reaction("eyes")
     # If SWEEP_BOT reacted to item_to_react_to with "rocket", then remove it.
     reactions = item_to_react_to.get_reactions()
     for reaction in reactions:
         if reaction.content == "rocket" and reaction.user.login == SWEEP_LOGIN:
             item_to_react_to.delete_reaction(reaction.id)
```

### Comparing `sweepai-0.4.0/sweepai/utils/chat_logger.py` & `sweepai-0.4.1/sweepai/utils/chat_logger.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.0/sweepai/utils/config.py` & `sweepai-0.4.1/sweepai/utils/config.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.0/sweepai/utils/constants.py` & `sweepai-0.4.1/sweepai/utils/constants.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.0/sweepai/utils/diff.py` & `sweepai-0.4.1/sweepai/utils/diff.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.0/sweepai/utils/event_logger.py` & `sweepai-0.4.1/sweepai/utils/event_logger.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.0/sweepai/utils/file_change_functions.py` & `sweepai-0.4.1/sweepai/utils/file_change_functions.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.0/sweepai/utils/github_utils.py` & `sweepai-0.4.1/sweepai/utils/github_utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.0/sweepai/utils/huggingface.py` & `sweepai-0.4.1/sweepai/utils/huggingface.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.0/sweepai/utils/prompt_constructor.py` & `sweepai-0.4.1/sweepai/utils/prompt_constructor.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.0/sweepai/utils/scorer.py` & `sweepai-0.4.1/sweepai/utils/scorer.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.0/sweepai/utils/snippets.py` & `sweepai-0.4.1/sweepai/utils/snippets.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.0/sweepai/utils/utils.py` & `sweepai-0.4.1/sweepai/utils/utils.py`

 * *Files identical despite different names*

### Comparing `sweepai-0.4.0/setup.py` & `sweepai-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 
 entry_points = \
 {'console_scripts': ['sweep = sweepai.app.cli:app',
                      'sweepai = sweepai.app.cli:app']}
 
 setup_kwargs = {
     'name': 'sweepai',
-    'version': '0.4.0',
+    'version': '0.4.1',
     'description': 'Sweep software chores',
-    'long_description': '<p align="center">\n    <img src="https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-3e61f57ad233">\n</p>\n<p align="center">\n    <i>Bug Reports & Feature Requests ⟶&nbsp; Code Changes</i>\n</p>\n\n<p align="center">\n<a href="https://sweep.dev">\n    <img alt="Landing Page" src="https://img.shields.io/badge/Site-sweep.dev-blue?link=https%3A%2F%2Fsweep.dev">\n</a>\n<a href="https://docs.sweep.dev/">\n    <img alt="Docs" src="https://img.shields.io/badge/Docs-docs.sweep.dev-blue?link=https%3A%2F%2Fdocs.sweep.dev">\n</a> \n<a href="https://discord.gg/sweep-ai">\n    <img src="https://dcbadge.vercel.app/api/server/sweep-ai?style=flat" />\n</a>\n<img alt="PyPI" src="https://img.shields.io/pypi/v/sweepai">\n<a href="https://pepy.tech/project/sweepai">\n    <img src="https://static.pepy.tech/badge/sweepai/month" />\n</a>\n<a href="https://github.com/sweepai/sweep">\n    <img src="https://img.shields.io/github/stars/sweepai/sweep" />\n</a>\n<a href="https://twitter.com/sweep__ai">\n    <img src="https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fsweep__ai" />\n</a>\n</p>\n\n<b>Sweep</b> is an AI junior developer that transforms bug reports & feature requests into code changes.\n\nDescribe bugs, small features, and refactors like you would to a junior developer, and Sweep:\n1. 🔍 reads your codebase\n2. 📝 plans the changes\n3. ⚡**writes a pull request with code**⚡\n\nSee highlights at https://docs.sweep.dev/examples.\n\n## ✨ Demo\nFor the best experience, [install Sweep](https://github.com/apps/sweep-ai) to one of your repos and see the magic happen.\n\n[Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47)\n\n## 🌠 Sweep\n* 🔧 Turns issues directly into pull requests (without an IDE)\n* 👀 Addresses developer replies & comments on its PRs\n* 🕵️\u200d♂️ Uses embedding-based code search, with popularity reranking for repository-level code understanding ([🔍 Rebuilding our Search Engine in a Day](https://docs.sweep.dev/how-we-rebuilt-our-code-search-engine-in-a-day))\n* 🎊 New: Fixes PRs based on Github Actions feedback\n* 🎊 New: Sweep Chat, a local interface for Sweep (see below)\n\n## 🚀 Getting Started\n\n### 🍲 Recipes\n#### To get the best performance from Sweep, we recommend the following approach to writing github issues/chats. \nFor harder problems, try to provide the same information a human would need. For simpler problems, providing a single line and a file name should suffice.\n\nA good issue might include:\n\n| Where to look <br> **[file name or function name]**| What to do <br> **[change the logic to do this]** | Additional Context (optional) <br> **[there\'s a bug/we need this feature/there\'s this dependency]** |\n|-----------|------------|----------------------|\n|In `sweepai/app/ui.py`|use an os-agnostic temp directory|N/A|\n|In `on_comment.py`|we should not fire an event|because it\'s possible that the comment is on a closed PR|\n|In the config loader in `packages/server/src/config.ts`|add a third option called "env" to load the config settings from environment variables| At present, there are two options:  1. ... and 2. ...|\n\nIf you want Sweep to use a file, try to mention the full path. Similarly, to have Sweep use a function, try to mention the class method or what it does. Also see [✨ Tips and tricks for Sweep](https://docs.sweep.dev/tricks).\n\n### 🖥️ Sweep Chat\nSweep Chat allows you to interact with Sweep and GitHub locally. Collaborate on the plan with Sweep, then have it create the pull request for you. \n\n**Prerequisites:** Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to your repository\n\n1. Run `pip install sweepai && sweep`. Note that you need **python 3.10+.**\n    - This runs GitHub authentication in your browser. \n\n2. Copy the 🔵 blue 8-digit code from your terminal into the page. You should only need to do the authentication once.  \n    - Wait a few seconds and Sweep Chat will start. \n\n3. Choose a repository from the dropdown at the top (the Github app must be installed to this repository).\n\n    - ⚡ Start chatting with Sweep Chat! ⚡\n\n<img src="https://github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-screenshot.png">\n\nTips:\n* 🔍 Relevant searched files will show up on the right. \n* 🔘 Sweep Chat creates PRs when the "Create PR" button is clicked. \n* 💡 You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.\n\n#### From Source\nIf you want the nightly build and or if the latest build has issues.\n\n1. `git clone https://github.com/sweepai/sweep && poetry install`\n2. `python sweepai/app/cli.py`. Note that you need **python 3.10+**.\n\n### ✨ Sweep Github App\nSetting up Sweep is as simple as adding the GitHub bot to a repo, then creating an issue for the bot to address.\nWe support all languages GPT4 supports, including Python, Typescript, Rust, Go, Java, C# and C++.\n\n1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos\n2. Create new issue in repo, like "Sweep: Write tests"\n3. Watch the magic happen 🪄\n\n## 🤝 Contributing\n\nContributions are welcome and greatly appreciated! For detailed guidelines on how to contribute, please see the [CONTRIBUTING.md](CONTRIBUTING.md) file.\nFor more detailed docs, see [🚀 Quickstart](https://docs.sweep.dev/start).\n\n## 📘 Story\n\nWe were frustrated by small tickets, like simple bug fixes, annoying refactors, and small features. Each task required us to open our IDE to fix simple bugs. So we decided to leverage the capabilities of ChatGPT to address this directly in GitHub.\n\nUnlike existing AI solutions, this can solve entire tickets and can be parallelized + asynchronous: developers can spin up 10 tickets and Sweep will address them all at once.\n\n## 📚 The Stack\n- GPT-4 32k 0613 (default)\n- ActiveLoop DeepLake for Vector DB with MiniLM L12 as our embeddings model\n- Modal Labs for infra + deployment\n- Gradio for Sweep Chat\n\n## 🗺️ Roadmap\nSee [🗺️ Roadmap](https://docs.sweep.dev/roadmap)\n\n## ⭐ Star History\n\n[![Star History Chart](https://api.star-history.com/svg?repos=sweepai/sweep&type=Date)](https://star-history.com/#sweepai/sweep&Date)\n\nConsider starring us if you\'re using Sweep so more people hear about us!\n<h2 align="center">\n    Contributors\n</h2>\n<p align="center">\n    Thank you for your contribution!\n</p>\n<p align="center">\n    <a href="https://github.com/sweepai/sweep/graphs/contributors">\n      <img src="https://contrib.rocks/image?repo=sweepai/sweep" />\n    </a>\n</p>\n<p align="center">\n    and, of course, Sweep!\n</p>\n',
+    'long_description': '<p align="center">\n    <img src="https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-3e61f57ad233">\n</p>\n<p align="center">\n    <i>Bug Reports & Feature Requests ⟶&nbsp; Code Changes</i>\n</p>\n\n<p align="center">\n<a href="https://sweep.dev">\n    <img alt="Landing Page" src="https://img.shields.io/badge/Site-sweep.dev-blue?link=https%3A%2F%2Fsweep.dev">\n</a>\n<a href="https://docs.sweep.dev/">\n    <img alt="Docs" src="https://img.shields.io/badge/Docs-docs.sweep.dev-blue?link=https%3A%2F%2Fdocs.sweep.dev">\n</a> \n<a href="https://discord.gg/sweep-ai">\n    <img src="https://dcbadge.vercel.app/api/server/sweep-ai?style=flat" />\n</a>\n<img alt="PyPI" src="https://img.shields.io/pypi/v/sweepai">\n<a href="https://pepy.tech/project/sweepai">\n    <img src="https://static.pepy.tech/badge/sweepai/month" />\n</a>\n<a href="https://github.com/sweepai/sweep">\n    <img src="https://img.shields.io/github/stars/sweepai/sweep" />\n</a>\n<a href="https://twitter.com/sweep__ai">\n    <img src="https://img.shields.io/twitter/url?url=https%3A%2F%2Ftwitter.com%2Fsweep__ai" />\n</a>\n</p>\n\n<b>Sweep</b> is an AI junior developer that transforms bug reports & feature requests into code changes.\n\nDescribe bugs, small features, and refactors like you would to a junior developer, and Sweep:\n1. 🔍 reads your codebase\n2. 📝 plans the changes\n3. ⚡**writes a pull request with code**⚡\n\nSee highlights at https://docs.sweep.dev/examples.\n\n## ✨ Demo\nFor the best experience, [install Sweep](https://github.com/apps/sweep-ai) to one of your repos and see the magic happen.\n\n[Demo](https://github.com/sweepai/sweep/assets/44910023/365ec29f-7317-40a7-9b5e-0af02f2b0e47)\n\n## 🌠 Sweep\n* 🔧 Turns issues directly into pull requests (without an IDE)\n* 👀 Addresses developer replies & comments on its PRs\n* 🕵️\u200d♂️ Uses embedding-based code search, with popularity reranking for repository-level code understanding ([🔍 Rebuilding our Search Engine in a Day](https://docs.sweep.dev/how-we-rebuilt-our-code-search-engine-in-a-day))\n* 🎊 New: Fixes PRs based on Github Actions feedback\n* 🎊 New: Sweep Chat, a local interface for Sweep (see below)\n\n## 🚀 Getting Started\n\n### 🍲 Recipes\n#### To get the best performance from Sweep, we recommend the following approach to writing github issues/chats. \nFor harder problems, try to provide the same information a human would need. For simpler problems, providing a single line and a file name should suffice.\n\nA good issue might include:\n\n| Where to look <br> **[file name or function name]**| What to do <br> **[change the logic to do this]** | Additional Context (optional) <br> **[there\'s a bug/we need this feature/there\'s this dependency]** |\n|-----------|------------|----------------------|\n|In `sweepai/app/ui.py`|use an os-agnostic temp directory|N/A|\n|In `on_comment.py`|we should not fire an event|because it\'s possible that the comment is on a closed PR|\n|In the config loader in `packages/server/src/config.ts`|add a third option called "env" to load the config settings from environment variables| At present, there are two options:  1. ... and 2. ...|\n\nIf you want Sweep to use a file, try to mention the full path. Similarly, to have Sweep use a function, try to mention the class method or what it does. Also see [✨ Tips and tricks for Sweep](https://docs.sweep.dev/tricks).\n\n### 🖥️ Sweep Chat\nSweep Chat allows you to interact with Sweep and GitHub locally. Collaborate on the plan with Sweep, then have it create the pull request for you. \n\n**Prerequisites:** Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to your repository\n\n1. Run `pip3 install sweepai && sweep`. Note that you need **python 3.10+.**\n    - Alternatively run `pip3 install --force-reinstall sweepai && sweep` if the previous command fails.\n    - This runs GitHub authentication in your browser.\n\n2. Copy the 🔵 blue 8-digit code from your terminal into the page. You should only need to do the authentication once.  \n    - Wait a few seconds and Sweep Chat will start. \n\n3. Choose a repository from the dropdown at the top (the Github app must be installed to this repository).\n\n    - ⚡ Start chatting with Sweep Chat! ⚡\n\n<img src="https://github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-screenshot.png">\n\nTips:\n* 🔍 Relevant searched files will show up on the right. \n* 🔘 Sweep Chat creates PRs when the "Create PR" button is clicked. \n* 💡 You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.\n\n#### From Source\nIf you want the nightly build and or if the latest build has issues.\n\n1. `git clone https://github.com/sweepai/sweep && poetry install`\n2. `python sweepai/app/cli.py`. Note that you need **python 3.10+**.\n\n### ✨ Sweep Github App\nSetting up Sweep is as simple as adding the GitHub bot to a repo, then creating an issue for the bot to address.\nWe support all languages GPT4 supports, including Python, Typescript, Rust, Go, Java, C# and C++.\n\n1. Add the [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos\n2. Create new issue in repo, like "Sweep: Write tests"\n3. Watch the magic happen 🪄\n\n## 🤝 Contributing\n\nContributions are welcome and greatly appreciated! For detailed guidelines on how to contribute, please see the [CONTRIBUTING.md](CONTRIBUTING.md) file.\nFor more detailed docs, see [🚀 Quickstart](https://docs.sweep.dev/start).\n\n## 📘 Story\n\nWe were frustrated by small tickets, like simple bug fixes, annoying refactors, and small features. Each task required us to open our IDE to fix simple bugs. So we decided to leverage the capabilities of ChatGPT to address this directly in GitHub.\n\nUnlike existing AI solutions, this can solve entire tickets and can be parallelized + asynchronous: developers can spin up 10 tickets and Sweep will address them all at once.\n\n## 📚 The Stack\n- GPT-4 32k 0613 (default)\n- ActiveLoop DeepLake for Vector DB with MiniLM L12 as our embeddings model\n- Modal Labs for infra + deployment\n- Gradio for Sweep Chat\n\n## 🗺️ Roadmap\nSee [🗺️ Roadmap](https://docs.sweep.dev/roadmap)\n\n## ⭐ Star History\n\n[![Star History Chart](https://api.star-history.com/svg?repos=sweepai/sweep&type=Date)](https://star-history.com/#sweepai/sweep&Date)\n\nConsider starring us if you\'re using Sweep so more people hear about us!\n<h2 align="center">\n    Contributors\n</h2>\n<p align="center">\n    Thank you for your contribution!\n</p>\n<p align="center">\n    <a href="https://github.com/sweepai/sweep/graphs/contributors">\n      <img src="https://contrib.rocks/image?repo=sweepai/sweep" />\n    </a>\n</p>\n<p align="center">\n    and, of course, Sweep!\n</p>\n',
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
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['sweepai',
 'sweepai.app', 'sweepai.core', 'sweepai.handlers', 'sweepai.utils']
 package_data = \ {'': ['*']} install_requires = \ ['GitPython>=3.1.31,<4.0.0',
 'PyGithub==1.58.2', 'config-path>=1.0.3,<2.0.0', 'gradio>=3.35.2,<4.0.0',
 'loguru>=0.6.0,<0.7.0', 'requests>=2.28.2,<3.0.0', 'tabulate>=0.9.0,<0.10.0',
 'typer>=0.9.0,<0.10.0', 'urllib3>=2.0.3,<3.0.0'] entry_points = \
 {'console_scripts': ['sweep = sweepai.app.cli:app', 'sweepai = sweepai.app.cli:
-app']} setup_kwargs = { 'name': 'sweepai', 'version': '0.4.0', 'description':
+app']} setup_kwargs = { 'name': 'sweepai', 'version': '0.4.1', 'description':
 'Sweep software chores', 'long_description': '
  \n [https://github.com/sweepai/sweep/assets/26889185/39d500fc-9276-402c-9ec7-
                                 3e61f57ad233]\n
 \n
              \n Bug Reports & Feature Requests â¶  Code Changes\n
 \n\n
 \n\n_[Landing_Page]\n\n\n_[Docs]\n \n\n_[https://dcbadge.vercel.app/api/server/
@@ -47,21 +47,22 @@
 are two options: 1. ... and 2. ...|\n\nIf you want Sweep to use a file, try to
 mention the full path. Similarly, to have Sweep use a function, try to mention
 the class method or what it does. Also see [â¨ Tips and tricks for Sweep]
 (https://docs.sweep.dev/tricks).\n\n### ð¥ï¸ Sweep Chat\nSweep Chat allows
 you to interact with Sweep and GitHub locally. Collaborate on the plan with
 Sweep, then have it create the pull request for you. \n\n**Prerequisites:**
 Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to your
-repository\n\n1. Run `pip install sweepai && sweep`. Note that you need
-**python 3.10+.**\n - This runs GitHub authentication in your browser. \n\n2.
-Copy the ðµ blue 8-digit code from your terminal into the page. You should
-only need to do the authentication once. \n - Wait a few seconds and Sweep Chat
-will start. \n\n3. Choose a repository from the dropdown at the top (the Github
-app must be installed to this repository).\n\n - â¡ Start chatting with Sweep
-Chat! â¡\n\n[https://github.com/sweepai/sweep/blob/
+repository\n\n1. Run `pip3 install sweepai && sweep`. Note that you need
+**python 3.10+.**\n - Alternatively run `pip3 install --force-reinstall sweepai
+&& sweep` if the previous command fails.\n - This runs GitHub authentication in
+your browser.\n\n2. Copy the ðµ blue 8-digit code from your terminal into the
+page. You should only need to do the authentication once. \n - Wait a few
+seconds and Sweep Chat will start. \n\n3. Choose a repository from the dropdown
+at the top (the Github app must be installed to this repository).\n\n - â¡
+Start chatting with Sweep Chat! â¡\n\n[https://github.com/sweepai/sweep/blob/
 856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-
 screenshot.png]\n\nTips:\n* ð Relevant searched files will show up on the
 right. \n* ð Sweep Chat creates PRs when the "Create PR" button is clicked.
 \n* ð¡ You can force dark mode by going to http://127.0.0.1:7861/
 ?__theme=dark.\n\n#### From Source\nIf you want the nightly build and or if the
 latest build has issues.\n\n1. `git clone https://github.com/sweepai/sweep &&
 poetry install`\n2. `python sweepai/app/cli.py`. Note that you need **python
```

### Comparing `sweepai-0.4.0/PKG-INFO` & `sweepai-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sweepai
-Version: 0.4.0
+Version: 0.4.1
 Summary: Sweep software chores
 Author: Kevin Lu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: GitPython (>=3.1.31,<4.0.0)
@@ -90,16 +90,17 @@
 If you want Sweep to use a file, try to mention the full path. Similarly, to have Sweep use a function, try to mention the class method or what it does. Also see [✨ Tips and tricks for Sweep](https://docs.sweep.dev/tricks).
 
 ### 🖥️ Sweep Chat
 Sweep Chat allows you to interact with Sweep and GitHub locally. Collaborate on the plan with Sweep, then have it create the pull request for you. 
 
 **Prerequisites:** Install [Sweep GitHub app](https://github.com/apps/sweep-ai) to your repository
 
-1. Run `pip install sweepai && sweep`. Note that you need **python 3.10+.**
-    - This runs GitHub authentication in your browser. 
+1. Run `pip3 install sweepai && sweep`. Note that you need **python 3.10+.**
+    - Alternatively run `pip3 install --force-reinstall sweepai && sweep` if the previous command fails.
+    - This runs GitHub authentication in your browser.
 
 2. Copy the 🔵 blue 8-digit code from your terminal into the page. You should only need to do the authentication once.  
     - Wait a few seconds and Sweep Chat will start. 
 
 3. Choose a repository from the dropdown at the top (the Github app must be installed to this repository).
 
     - ⚡ Start chatting with Sweep Chat! ⚡
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sweepai Version: 0.4.0 Summary: Sweep software
+Metadata-Version: 2.1 Name: sweepai Version: 0.4.1 Summary: Sweep software
 chores Author: Kevin Lu Requires-Python: >=3.10,<4.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: GitPython
 (>=3.1.31,<4.0.0) Requires-Dist: PyGithub (==1.58.2) Requires-Dist: config-path
 (>=1.0.3,<2.0.0) Requires-Dist: gradio (>=3.35.2,<4.0.0) Requires-Dist: loguru
 (>=0.6.0,<0.7.0) Requires-Dist: requests (>=2.28.2,<3.0.0) Requires-Dist:
 tabulate (>=0.9.0,<0.10.0) Requires-Dist: typer (>=0.9.0,<0.10.0) Requires-
@@ -47,26 +47,27 @@
 load the config settings from environment variables| At present, there are two
 options: 1. ... and 2. ...| If you want Sweep to use a file, try to mention the
 full path. Similarly, to have Sweep use a function, try to mention the class
 method or what it does. Also see [â¨ Tips and tricks for Sweep](https://
 docs.sweep.dev/tricks). ### ð¥ï¸ Sweep Chat Sweep Chat allows you to
 interact with Sweep and GitHub locally. Collaborate on the plan with Sweep,
 then have it create the pull request for you. **Prerequisites:** Install [Sweep
-GitHub app](https://github.com/apps/sweep-ai) to your repository 1. Run `pip
-install sweepai && sweep`. Note that you need **python 3.10+.** - This runs
-GitHub authentication in your browser. 2. Copy the ðµ blue 8-digit code from
-your terminal into the page. You should only need to do the authentication
-once. - Wait a few seconds and Sweep Chat will start. 3. Choose a repository
-from the dropdown at the top (the Github app must be installed to this
-repository). - â¡ Start chatting with Sweep Chat! â¡ [https://github.com/
-sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/gradio-
-screenshot.png] Tips: * ð Relevant searched files will show up on the right.
-* ð Sweep Chat creates PRs when the "Create PR" button is clicked. * ð¡
-You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark. ####
-From Source If you want the nightly build and or if the latest build has
+GitHub app](https://github.com/apps/sweep-ai) to your repository 1. Run `pip3
+install sweepai && sweep`. Note that you need **python 3.10+.** - Alternatively
+run `pip3 install --force-reinstall sweepai && sweep` if the previous command
+fails. - This runs GitHub authentication in your browser. 2. Copy the ðµ blue
+8-digit code from your terminal into the page. You should only need to do the
+authentication once. - Wait a few seconds and Sweep Chat will start. 3. Choose
+a repository from the dropdown at the top (the Github app must be installed to
+this repository). - â¡ Start chatting with Sweep Chat! â¡ [https://
+github.com/sweepai/sweep/blob/856ff66c2dbeaf39afbf6d8c49a620dfa70271fb/.assets/
+gradio-screenshot.png] Tips: * ð Relevant searched files will show up on the
+right. * ð Sweep Chat creates PRs when the "Create PR" button is clicked. *
+ð¡ You can force dark mode by going to http://127.0.0.1:7861/?__theme=dark.
+#### From Source If you want the nightly build and or if the latest build has
 issues. 1. `git clone https://github.com/sweepai/sweep && poetry install` 2.
 `python sweepai/app/cli.py`. Note that you need **python 3.10+**. ### â¨ Sweep
 Github App Setting up Sweep is as simple as adding the GitHub bot to a repo,
 then creating an issue for the bot to address. We support all languages GPT4
 supports, including Python, Typescript, Rust, Go, Java, C# and C++. 1. Add the
 [Sweep GitHub app](https://github.com/apps/sweep-ai) to desired repos 2. Create
 new issue in repo, like "Sweep: Write tests" 3. Watch the magic happen ðª ##
```

