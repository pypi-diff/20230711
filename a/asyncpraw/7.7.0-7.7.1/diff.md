# Comparing `tmp/asyncpraw-7.7.0.tar.gz` & `tmp/asyncpraw-7.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncpraw-7.7.0.tar", last modified: Sat Feb 25 20:11:54 2023, max compression
+gzip compressed data, was "asyncpraw-7.7.1.tar", last modified: Tue Jul 11 21:08:33 2023, max compression
```

## Comparing `asyncpraw-7.7.0.tar` & `asyncpraw-7.7.1.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 20:11:54.277940 asyncpraw-7.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10961 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-02-25 20:11:54.277940 asyncpraw-7.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 20:11:54.261940 asyncpraw-7.7.0/asyncpraw/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    13828 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)    11131 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 20:11:54.261940 asyncpraw-7.7.0/asyncpraw/images/
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/images/PRAW logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 20:11:54.265940 asyncpraw-7.7.0/asyncpraw/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/comment_forest.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/front.py
--rw-r--r--   0 runner    (1001) docker     (123)    16019 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11302 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/inbox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 20:11:54.269940 asyncpraw-7.7.0/asyncpraw/models/list/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/list/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/list/draft.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/list/moderated.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/list/redditor.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/list/trophy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 20:11:54.269940 asyncpraw-7.7.0/asyncpraw/models/listing/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/listing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/listing/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/listing/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/listing/listing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 20:11:54.269940 asyncpraw-7.7.0/asyncpraw/models/listing/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/listing/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/listing/mixins/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/listing/mixins/gilded.py
--rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/listing/mixins/redditor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/listing/mixins/rising.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/listing/mixins/submission.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/listing/mixins/subreddit.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/mod_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/mod_note.py
--rw-r--r--   0 runner    (1001) docker     (123)    26348 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/mod_notes.py
--rw-r--r--   0 runner    (1001) docker     (123)    10753 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/preferences.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 20:11:54.277940 asyncpraw-7.7.0/asyncpraw/models/reddit/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/reddit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/reddit/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20494 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/reddit/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)    13648 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/reddit/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)    12119 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/reddit/draft.py
--rw-r--r--   0 runner    (1001) docker     (123)     9527 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/reddit/emoji.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/reddit/inline_media.py
--rw-r--r--   0 runner    (1001) docker     (123)    28824 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/reddit/live.py
--rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/reddit/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 20:11:54.277940 asyncpraw-7.7.0/asyncpraw/models/reddit/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/reddit/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/reddit/mixins/editable.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/reddit/mixins/fullname.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/reddit/mixins/gildable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/reddit/mixins/inboxable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/reddit/mixins/inboxtoggleable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/reddit/mixins/messageable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/reddit/mixins/modnote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/reddit/mixins/replyable.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/reddit/mixins/reportable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/reddit/mixins/savable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/reddit/mixins/votable.py
--rw-r--r--   0 runner    (1001) docker     (123)    13336 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/reddit/modmail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/reddit/more.py
--rw-r--r--   0 runner    (1001) docker     (123)    10227 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/reddit/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/reddit/poll.py
--rw-r--r--   0 runner    (1001) docker     (123)    18233 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/reddit/redditor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9700 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/reddit/removal_reasons.py
--rw-r--r--   0 runner    (1001) docker     (123)    16466 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/reddit/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    28440 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/reddit/submission.py
--rw-r--r--   0 runner    (1001) docker     (123)   164872 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/reddit/subreddit.py
--rw-r--r--   0 runner    (1001) docker     (123)    11142 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/reddit/user_subreddit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    68758 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/reddit/widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)    13806 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/reddit/wikipage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/redditors.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/stylesheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/subreddits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/trophy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11245 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/models/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    12895 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/objector.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/praw.ini
--rw-r--r--   0 runner    (1001) docker     (123)    39160 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/reddit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 20:11:54.277940 asyncpraw-7.7.0/asyncpraw/util/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/util/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/util/deprecate_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/util/snake.py
--rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/asyncpraw/util/token_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-25 20:11:54.261940 asyncpraw-7.7.0/asyncpraw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-02-25 20:11:54.000000 asyncpraw-7.7.0/asyncpraw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-02-25 20:11:54.000000 asyncpraw-7.7.0/asyncpraw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-25 20:11:54.000000 asyncpraw-7.7.0/asyncpraw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-02-25 20:11:54.000000 asyncpraw-7.7.0/asyncpraw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-25 20:11:54.000000 asyncpraw-7.7.0/asyncpraw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/praw_license.txt
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-25 20:11:54.277940 asyncpraw-7.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-02-25 20:11:41.000000 asyncpraw-7.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:08:33.503203 asyncpraw-7.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11175 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-07-11 21:08:33.503203 asyncpraw-7.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6352 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:08:33.495203 asyncpraw-7.7.1/asyncpraw/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13828 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11131 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:08:33.495203 asyncpraw-7.7.1/asyncpraw/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/images/PRAW logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:08:33.499203 asyncpraw-7.7.1/asyncpraw/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/comment_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/front.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16019 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11302 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/inbox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:08:33.499203 asyncpraw-7.7.1/asyncpraw/models/list/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/list/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/list/draft.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/list/moderated.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/list/redditor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/list/trophy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:08:33.499203 asyncpraw-7.7.1/asyncpraw/models/listing/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/listing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/listing/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/listing/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/listing/listing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:08:33.499203 asyncpraw-7.7.1/asyncpraw/models/listing/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/listing/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/listing/mixins/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/listing/mixins/gilded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/listing/mixins/redditor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/listing/mixins/rising.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/listing/mixins/submission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/listing/mixins/subreddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/mod_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/mod_note.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26348 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/mod_notes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10753 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/preferences.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:08:33.503203 asyncpraw-7.7.1/asyncpraw/models/reddit/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/reddit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/reddit/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20494 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/reddit/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13648 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/reddit/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12119 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/reddit/draft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9527 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/reddit/emoji.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/reddit/inline_media.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28824 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/reddit/live.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/reddit/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:08:33.503203 asyncpraw-7.7.1/asyncpraw/models/reddit/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)    11579 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/reddit/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/reddit/mixins/editable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/reddit/mixins/fullname.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/reddit/mixins/gildable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/reddit/mixins/inboxable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/reddit/mixins/inboxtoggleable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/reddit/mixins/messageable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/reddit/mixins/modnote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/reddit/mixins/replyable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/reddit/mixins/reportable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/reddit/mixins/savable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/reddit/mixins/votable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13656 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/reddit/modmail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/reddit/more.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10227 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/reddit/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/reddit/poll.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18233 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/reddit/redditor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9700 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/reddit/removal_reasons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16466 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/reddit/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28440 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/reddit/submission.py
+-rw-r--r--   0 runner    (1001) docker     (123)   164872 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/reddit/subreddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11142 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/reddit/user_subreddit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    68758 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/reddit/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13806 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/reddit/wikipage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/redditors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/stylesheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/subreddits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/trophy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11245 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/models/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12895 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/objector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/praw.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    39160 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/reddit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:08:33.503203 asyncpraw-7.7.1/asyncpraw/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/util/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/util/deprecate_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/util/snake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/asyncpraw/util/token_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:08:33.495203 asyncpraw-7.7.1/asyncpraw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-07-11 21:08:33.000000 asyncpraw-7.7.1/asyncpraw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-07-11 21:08:33.000000 asyncpraw-7.7.1/asyncpraw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 21:08:33.000000 asyncpraw-7.7.1/asyncpraw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-11 21:08:33.000000 asyncpraw-7.7.1/asyncpraw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 21:08:33.000000 asyncpraw-7.7.1/asyncpraw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/praw_license.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 21:08:33.503203 asyncpraw-7.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-11 21:08:22.000000 asyncpraw-7.7.1/setup.py
```

### Comparing `asyncpraw-7.7.0/AUTHORS.rst` & `asyncpraw-7.7.1/AUTHORS.rst`

 * *Files 2% similar despite different names*

```diff
@@ -87,8 +87,9 @@
 - Gerard Rodes <GerardRodesVidal@gmail.com> `@GerardRodes
   <https://github.com/GerardRodes>`_
 - cmays90 `@cmays90 <https://github.com/cmays90>`_
 - Dio Brando `@isFakeAccount <https://github.com/isFakeAccount>`_
 - Josh Kim `@jsk56143 <https://github.com/jsk56143>`_
 - Rolf Campbell `@endlisnis <https://github.com/endlisnis>`_
 - zacc `@zacc <https://github.com/zacc>`_
+- Arkadiy Illarionov `@qarkai <https://github.com/qarkai>`_
 - Add "Name <email (optional)> and github profile link" above this line.
```

### Comparing `asyncpraw-7.7.0/CHANGES.rst` & `asyncpraw-7.7.1/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,23 @@
 Change Log
 ==========
 
 Async PRAW follows `semantic versioning <https://semver.org/>`_.
 
+7.7.1 (2023/07/11)
+------------------
+
+**Changed**
+
+- Drop asyncio_extras dependency, use contextlib.asynccontextmanager instead.
+
+**Fixed**
+
+- An issue with replying to a modmail conversation results in a error.
+
 7.7.0 (2023/02/25)
 ------------------
 
 **Added**
 
 - :meth:`.delete_mobile_banner` to delete mobile banners.
 - :meth:`.upload_mobile_banner` to upload mobile banners.
```

### Comparing `asyncpraw-7.7.0/LICENSE.txt` & `asyncpraw-7.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/PKG-INFO` & `asyncpraw-7.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncpraw
-Version: 7.7.0
+Version: 7.7.1
 Summary: Async PRAW, an abbreviation for "Asynchronous Python Reddit API Wrapper", is a python package that allows for simple access to Reddit's API.
 Author: Joel Payne
 Author-email: lilspazjoekp@gmail.com
 License: Simplified BSD License
 Project-URL: Change Log, https://asyncpraw.readthedocs.io/en/latest/package_info/change_log.html
 Project-URL: Documentation, https://asyncpraw.readthedocs.io/
 Project-URL: Issue Tracker, https://github.com/praw-dev/asyncpraw/issues
```

### Comparing `asyncpraw-7.7.0/README.rst` & `asyncpraw-7.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/__init__.py` & `asyncpraw-7.7.1/asyncpraw/__init__.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/config.py` & `asyncpraw-7.7.1/asyncpraw/config.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/endpoints.py` & `asyncpraw-7.7.1/asyncpraw/endpoints.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/exceptions.py` & `asyncpraw-7.7.1/asyncpraw/exceptions.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/images/PRAW logo.png` & `asyncpraw-7.7.1/asyncpraw/images/PRAW logo.png`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/__init__.py` & `asyncpraw-7.7.1/asyncpraw/models/__init__.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/auth.py` & `asyncpraw-7.7.1/asyncpraw/models/auth.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/base.py` & `asyncpraw-7.7.1/asyncpraw/models/base.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/comment_forest.py` & `asyncpraw-7.7.1/asyncpraw/models/comment_forest.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/front.py` & `asyncpraw-7.7.1/asyncpraw/models/front.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/helpers.py` & `asyncpraw-7.7.1/asyncpraw/models/helpers.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/inbox.py` & `asyncpraw-7.7.1/asyncpraw/models/inbox.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/list/base.py` & `asyncpraw-7.7.1/asyncpraw/models/list/base.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/listing/domain.py` & `asyncpraw-7.7.1/asyncpraw/models/listing/domain.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/listing/generator.py` & `asyncpraw-7.7.1/asyncpraw/models/listing/generator.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/listing/listing.py` & `asyncpraw-7.7.1/asyncpraw/models/listing/listing.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/listing/mixins/base.py` & `asyncpraw-7.7.1/asyncpraw/models/listing/mixins/base.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/listing/mixins/gilded.py` & `asyncpraw-7.7.1/asyncpraw/models/listing/mixins/gilded.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/listing/mixins/redditor.py` & `asyncpraw-7.7.1/asyncpraw/models/listing/mixins/redditor.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/listing/mixins/rising.py` & `asyncpraw-7.7.1/asyncpraw/models/listing/mixins/rising.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/listing/mixins/submission.py` & `asyncpraw-7.7.1/asyncpraw/models/listing/mixins/submission.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/listing/mixins/subreddit.py` & `asyncpraw-7.7.1/asyncpraw/models/listing/mixins/subreddit.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/mod_action.py` & `asyncpraw-7.7.1/asyncpraw/models/mod_action.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/mod_note.py` & `asyncpraw-7.7.1/asyncpraw/models/mod_note.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/mod_notes.py` & `asyncpraw-7.7.1/asyncpraw/models/mod_notes.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/preferences.py` & `asyncpraw-7.7.1/asyncpraw/models/preferences.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/reddit/base.py` & `asyncpraw-7.7.1/asyncpraw/models/reddit/base.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/reddit/collections.py` & `asyncpraw-7.7.1/asyncpraw/models/reddit/collections.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/reddit/comment.py` & `asyncpraw-7.7.1/asyncpraw/models/reddit/comment.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/reddit/draft.py` & `asyncpraw-7.7.1/asyncpraw/models/reddit/draft.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/reddit/emoji.py` & `asyncpraw-7.7.1/asyncpraw/models/reddit/emoji.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/reddit/inline_media.py` & `asyncpraw-7.7.1/asyncpraw/models/reddit/inline_media.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/reddit/live.py` & `asyncpraw-7.7.1/asyncpraw/models/reddit/live.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/reddit/message.py` & `asyncpraw-7.7.1/asyncpraw/models/reddit/message.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/reddit/mixins/__init__.py` & `asyncpraw-7.7.1/asyncpraw/models/reddit/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/reddit/mixins/editable.py` & `asyncpraw-7.7.1/asyncpraw/models/reddit/mixins/editable.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/reddit/mixins/gildable.py` & `asyncpraw-7.7.1/asyncpraw/models/reddit/mixins/gildable.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/reddit/mixins/inboxable.py` & `asyncpraw-7.7.1/asyncpraw/models/reddit/mixins/inboxable.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/reddit/mixins/inboxtoggleable.py` & `asyncpraw-7.7.1/asyncpraw/models/reddit/mixins/inboxtoggleable.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/reddit/mixins/messageable.py` & `asyncpraw-7.7.1/asyncpraw/models/reddit/mixins/messageable.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/reddit/mixins/modnote.py` & `asyncpraw-7.7.1/asyncpraw/models/reddit/mixins/modnote.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/reddit/mixins/replyable.py` & `asyncpraw-7.7.1/asyncpraw/models/reddit/mixins/replyable.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/reddit/mixins/reportable.py` & `asyncpraw-7.7.1/asyncpraw/models/reddit/mixins/reportable.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/reddit/mixins/savable.py` & `asyncpraw-7.7.1/asyncpraw/models/reddit/mixins/savable.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/reddit/mixins/votable.py` & `asyncpraw-7.7.1/asyncpraw/models/reddit/mixins/votable.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/reddit/modmail.py` & `asyncpraw-7.7.1/asyncpraw/models/reddit/modmail.py`

 * *Files 2% similar despite different names*

```diff
@@ -268,17 +268,23 @@
             "body": body,
             "isAuthorHidden": author_hidden,
             "isInternal": internal,
         }
         response = await self._reddit.post(
             API_PATH["modmail_conversation"].format(id=self.id), data=data
         )
-        message_id = response["conversation"]["objIds"][-1]["id"]
-        message_data = response["messages"][message_id]
-        return self._reddit._objector.objectify(message_data)
+        if isinstance(response, dict):
+            # Reddit recently changed the response format, so we need to handle both in case they change it back
+            message_id = response["conversation"]["objIds"][-1]["id"]
+            message_data = response["messages"][message_id]
+            return self._reddit._objector.objectify(message_data)
+        else:
+            for message in response.messages:
+                if message.id == response.obj_ids[-1]["id"]:
+                    return message
 
     async def unarchive(self):
         """Unarchive the conversation.
 
         For example:
 
         .. code-block:: python
```

### Comparing `asyncpraw-7.7.0/asyncpraw/models/reddit/more.py` & `asyncpraw-7.7.1/asyncpraw/models/reddit/more.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/reddit/multi.py` & `asyncpraw-7.7.1/asyncpraw/models/reddit/multi.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/reddit/poll.py` & `asyncpraw-7.7.1/asyncpraw/models/reddit/poll.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/reddit/redditor.py` & `asyncpraw-7.7.1/asyncpraw/models/reddit/redditor.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/reddit/removal_reasons.py` & `asyncpraw-7.7.1/asyncpraw/models/reddit/removal_reasons.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/reddit/rules.py` & `asyncpraw-7.7.1/asyncpraw/models/reddit/rules.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/reddit/submission.py` & `asyncpraw-7.7.1/asyncpraw/models/reddit/submission.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/reddit/subreddit.py` & `asyncpraw-7.7.1/asyncpraw/models/reddit/subreddit.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/reddit/user_subreddit.py` & `asyncpraw-7.7.1/asyncpraw/models/reddit/user_subreddit.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/reddit/widgets.py` & `asyncpraw-7.7.1/asyncpraw/models/reddit/widgets.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/reddit/wikipage.py` & `asyncpraw-7.7.1/asyncpraw/models/reddit/wikipage.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/redditors.py` & `asyncpraw-7.7.1/asyncpraw/models/redditors.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/stylesheet.py` & `asyncpraw-7.7.1/asyncpraw/models/stylesheet.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/subreddits.py` & `asyncpraw-7.7.1/asyncpraw/models/subreddits.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/trophy.py` & `asyncpraw-7.7.1/asyncpraw/models/trophy.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/user.py` & `asyncpraw-7.7.1/asyncpraw/models/user.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/models/util.py` & `asyncpraw-7.7.1/asyncpraw/models/util.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/objector.py` & `asyncpraw-7.7.1/asyncpraw/objector.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/praw.ini` & `asyncpraw-7.7.1/asyncpraw/praw.ini`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/reddit.py` & `asyncpraw-7.7.1/asyncpraw/reddit.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/util/cache.py` & `asyncpraw-7.7.1/asyncpraw/util/cache.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/util/deprecate_args.py` & `asyncpraw-7.7.1/asyncpraw/util/deprecate_args.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/util/snake.py` & `asyncpraw-7.7.1/asyncpraw/util/snake.py`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw/util/token_manager.py` & `asyncpraw-7.7.1/asyncpraw/util/token_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 
 .. deprecated:: 7.4.0
 
     Tokens managers have been deprecated and will be removed in the near future.
 
 """
 from abc import ABC, abstractmethod
+from contextlib import asynccontextmanager
 
 import aiofiles
-from asyncio_extras import async_contextmanager
 
 from . import _deprecate_args
 
 
 class BaseTokenManager(ABC):
     """An abstract class for all token managers."""
 
@@ -155,15 +155,15 @@
             )
             await conn.commit()
 
     async def close(self):
         """Close the sqlite3 connection."""
         await self._connection.close()
 
-    @async_contextmanager
+    @asynccontextmanager
     async def connection(self):
         """Asynchronously setup and provide the sqlite3 connection."""
         if self._connection is None:
             import aiosqlite
 
             self._connection = await aiosqlite.connect(self._database)
         if not self._setup_ran:
```

### Comparing `asyncpraw-7.7.0/asyncpraw.egg-info/PKG-INFO` & `asyncpraw-7.7.1/asyncpraw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asyncpraw
-Version: 7.7.0
+Version: 7.7.1
 Summary: Async PRAW, an abbreviation for "Asynchronous Python Reddit API Wrapper", is a python package that allows for simple access to Reddit's API.
 Author: Joel Payne
 Author-email: lilspazjoekp@gmail.com
 License: Simplified BSD License
 Project-URL: Change Log, https://asyncpraw.readthedocs.io/en/latest/package_info/change_log.html
 Project-URL: Documentation, https://asyncpraw.readthedocs.io/
 Project-URL: Issue Tracker, https://github.com/praw-dev/asyncpraw/issues
```

### Comparing `asyncpraw-7.7.0/asyncpraw.egg-info/SOURCES.txt` & `asyncpraw-7.7.1/asyncpraw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/asyncpraw.egg-info/requires.txt` & `asyncpraw-7.7.1/asyncpraw.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 aiofiles<1
 aiohttp<4
 aiosqlite<=0.17.0
-asyncio_extras<=1.3.2
 asyncprawcore<3,>=2.1
 update_checker>=0.18
 
 [ci]
 coveralls
 
 [dev]
@@ -16,15 +15,16 @@
 sphinx_rtd_theme
 sphinxcontrib-trio
 mock==4.*
 pytest==7.*
 pytest-asyncio==0.18.*
 pytest-vcr==1.*
 testfixtures==6.*
-vcrpy==4.*
+urllib3==1.*
+vcrpy==4.2.1
 
 [dev:python_version < "3.8"]
 asynctest==0.13.*
 
 [lint]
 pre-commit
 sphinx
@@ -40,11 +40,12 @@
 
 [test]
 mock==4.*
 pytest==7.*
 pytest-asyncio==0.18.*
 pytest-vcr==1.*
 testfixtures==6.*
-vcrpy==4.*
+urllib3==1.*
+vcrpy==4.2.1
 
 [test:python_version < "3.8"]
 asynctest==0.13.*
```

### Comparing `asyncpraw-7.7.0/praw_license.txt` & `asyncpraw-7.7.1/praw_license.txt`

 * *Files identical despite different names*

### Comparing `asyncpraw-7.7.0/setup.py` & `asyncpraw-7.7.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,16 @@
     "test": [
         "asynctest ==0.13.* ; python_version < '3.8'",  # TODO: Remove me when support for 3.7 is dropped
         "mock ==4.*",
         "pytest ==7.*",
         "pytest-asyncio ==0.18.*",
         "pytest-vcr ==1.*",
         "testfixtures ==6.*",
-        "vcrpy ==4.*",
+        "urllib3 ==1.*",
+        "vcrpy ==4.2.1",
     ],
 }
 extras["lint"] += extras["readthedocs"]
 extras["dev"] += extras["lint"] + extras["test"]
 
 setup(
     name=PACKAGE_NAME,
@@ -61,15 +62,14 @@
         " python package that allows for simple access to Reddit's API."
     ),
     extras_require=extras,
     install_requires=[
         "aiofiles <1",
         "aiohttp <4",
         "aiosqlite <=0.17.0",
-        "asyncio_extras <=1.3.2",
         "asyncprawcore >=2.1, <3",
         "update_checker >=0.18",
     ],
     keywords="reddit api wrapper asyncpraw praw async asynchronous",
     license="Simplified BSD License",
     long_description=README,
     package_data={
```

