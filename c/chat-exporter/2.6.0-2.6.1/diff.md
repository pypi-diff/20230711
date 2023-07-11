# Comparing `tmp/chat_exporter-2.6.0.tar.gz` & `tmp/chat_exporter-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat_exporter-2.6.0.tar", last modified: Tue Jul 11 19:19:13 2023, max compression
+gzip compressed data, was "chat_exporter-2.6.1.tar", last modified: Tue Jul 11 20:52:24 2023, max compression
```

## Comparing `chat_exporter-2.6.0.tar` & `chat_exporter-2.6.1.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 19:19:13.672111 chat_exporter-2.6.0/
--rw-rw-rw-   0        0        0    35803 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/LICENSE
--rw-rw-rw-   0        0        0       79 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/MANIFEST.in
--rw-rw-rw-   0        0        0    11902 2023-07-11 19:19:13.672111 chat_exporter-2.6.0/PKG-INFO
--rw-rw-rw-   0        0        0    10649 2023-07-11 19:11:19.000000 chat_exporter-2.6.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 19:19:13.605019 chat_exporter-2.6.0/chat_exporter/
--rw-rw-rw-   0        0        0      212 2023-07-11 19:14:07.000000 chat_exporter-2.6.0/chat_exporter/__init__.py
--rw-rw-rw-   0        0        0     5862 2023-05-13 17:51:37.000000 chat_exporter-2.6.0/chat_exporter/chat_exporter.py
-drwxrwxrwx   0        0        0        0 2023-07-11 19:19:13.619801 chat_exporter-2.6.0/chat_exporter/construct/
--rw-rw-rw-   0        0        0        0 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/construct/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 19:19:13.631823 chat_exporter-2.6.0/chat_exporter/construct/assets/
--rw-rw-rw-   0        0        0      206 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/construct/assets/__init__.py
--rw-rw-rw-   0        0        0     4018 2023-05-13 16:20:32.000000 chat_exporter-2.6.0/chat_exporter/construct/assets/attachment.py
--rw-rw-rw-   0        0        0     3939 2023-01-09 20:42:18.000000 chat_exporter-2.6.0/chat_exporter/construct/assets/component.py
--rw-rw-rw-   0        0        0     6239 2023-07-11 19:11:19.000000 chat_exporter-2.6.0/chat_exporter/construct/assets/embed.py
--rw-rw-rw-   0        0        0     1544 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/construct/assets/reaction.py
--rw-rw-rw-   0        0        0    20085 2023-07-11 19:11:19.000000 chat_exporter-2.6.0/chat_exporter/construct/message.py
--rw-rw-rw-   0        0        0     6837 2023-07-11 19:11:19.000000 chat_exporter-2.6.0/chat_exporter/construct/transcript.py
-drwxrwxrwx   0        0        0        0 2023-07-11 19:19:13.640847 chat_exporter-2.6.0/chat_exporter/ext/
--rw-rw-rw-   0        0        0        0 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/ext/__init__.py
--rw-rw-rw-   0        0        0     1285 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/ext/cache.py
--rw-rw-rw-   0        0        0      225 2023-07-11 18:47:19.000000 chat_exporter-2.6.0/chat_exporter/ext/discord_import.py
--rw-rw-rw-   0        0        0     2123 2023-07-11 19:11:19.000000 chat_exporter-2.6.0/chat_exporter/ext/discord_utils.py
--rw-rw-rw-   0        0        0      146 2023-07-11 19:11:19.000000 chat_exporter-2.6.0/chat_exporter/ext/discriminator.py
--rw-rw-rw-   0        0        0     4214 2023-07-11 19:11:19.000000 chat_exporter-2.6.0/chat_exporter/ext/emoji_convert.py
--rw-rw-rw-   0        0        0     4304 2023-07-11 19:11:19.000000 chat_exporter-2.6.0/chat_exporter/ext/html_generator.py
-drwxrwxrwx   0        0        0        0 2023-07-11 19:19:13.642844 chat_exporter-2.6.0/chat_exporter/html/
--rw-rw-rw-   0        0        0        0 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 19:19:13.644843 chat_exporter-2.6.0/chat_exporter/html/attachment/
--rw-rw-rw-   0        0        0      774 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/attachment/audio.html
--rw-rw-rw-   0        0        0      140 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/attachment/image.html
--rw-rw-rw-   0        0        0      547 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/attachment/message.html
--rw-rw-rw-   0        0        0      127 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/attachment/video.html
--rw-rw-rw-   0        0        0    44009 2023-07-11 19:11:19.000000 chat_exporter-2.6.0/chat_exporter/html/base.html
-drwxrwxrwx   0        0        0        0 2023-07-11 19:19:13.647550 chat_exporter-2.6.0/chat_exporter/html/component/
--rw-rw-rw-   0        0        0      229 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/component/component_button.html
--rw-rw-rw-   0        0        0      254 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/component/component_menu.html
--rw-rw-rw-   0        0        0      159 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/component/component_menu_options.html
--rw-rw-rw-   0        0        0      508 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/component/component_menu_options_emoji.html
-drwxrwxrwx   0        0        0        0 2023-07-11 19:19:13.656070 chat_exporter-2.6.0/chat_exporter/html/embed/
--rw-rw-rw-   0        0        0      123 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/embed/author.html
--rw-rw-rw-   0        0        0      225 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/embed/author_icon.html
--rw-rw-rw-   0        0        0      667 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/embed/body.html
--rw-rw-rw-   0        0        0      116 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/embed/description.html
--rw-rw-rw-   0        0        0      317 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/embed/field-inline.html
--rw-rw-rw-   0        0        0      306 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/embed/field.html
--rw-rw-rw-   0        0        0      113 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/embed/footer.html
--rw-rw-rw-   0        0        0      183 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/embed/footer_image.html
--rw-rw-rw-   0        0        0      186 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/embed/image.html
--rw-rw-rw-   0        0        0      206 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/embed/thumbnail.html
--rw-rw-rw-   0        0        0       97 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/embed/title.html
-drwxrwxrwx   0        0        0        0 2023-07-11 19:19:13.665091 chat_exporter-2.6.0/chat_exporter/html/message/
--rw-rw-rw-   0        0        0      239 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/message/bot-tag-verified.html
--rw-rw-rw-   0        0        0       43 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/message/bot-tag.html
--rw-rw-rw-   0        0        0       77 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/message/content.html
--rw-rw-rw-   0        0        0        6 2023-06-24 11:50:24.000000 chat_exporter-2.6.0/chat_exporter/html/message/end.html
--rw-rw-rw-   0        0        0      507 2023-07-11 19:11:19.000000 chat_exporter-2.6.0/chat_exporter/html/message/interaction.html
--rw-rw-rw-   0        0        0      961 2023-07-11 19:11:19.000000 chat_exporter-2.6.0/chat_exporter/html/message/message.html
--rw-rw-rw-   0        0        0     1108 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/message/meta.html
--rw-rw-rw-   0        0        0     1000 2023-07-11 19:11:19.000000 chat_exporter-2.6.0/chat_exporter/html/message/pin.html
--rw-rw-rw-   0        0        0      550 2023-07-11 19:11:19.000000 chat_exporter-2.6.0/chat_exporter/html/message/reference.html
--rw-rw-rw-   0        0        0      131 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/message/reference_unknown.html
--rw-rw-rw-   0        0        0     1254 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/message/start.html
--rw-rw-rw-   0        0        0      895 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/message/thread.html
--rw-rw-rw-   0        0        0      968 2023-07-11 19:11:19.000000 chat_exporter-2.6.0/chat_exporter/html/message/thread_add.html
--rw-rw-rw-   0        0        0      972 2023-07-11 19:11:19.000000 chat_exporter-2.6.0/chat_exporter/html/message/thread_remove.html
-drwxrwxrwx   0        0        0        0 2023-07-11 19:19:13.666091 chat_exporter-2.6.0/chat_exporter/html/reaction/
--rw-rw-rw-   0        0        0      206 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/reaction/custom_emoji.html
--rw-rw-rw-   0        0        0      120 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/reaction/emoji.html
-drwxrwxrwx   0        0        0        0 2023-07-11 19:19:13.669107 chat_exporter-2.6.0/chat_exporter/html/script/
--rw-rw-rw-   0        0        0      112 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/script/channel_subject.html
--rw-rw-rw-   0        0        0       59 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/script/channel_topic.html
--rw-rw-rw-   0        0        0     1183 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/script/fancy_time.html
-drwxrwxrwx   0        0        0        0 2023-07-11 19:19:13.671111 chat_exporter-2.6.0/chat_exporter/parse/
--rw-rw-rw-   0        0        0        0 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/parse/__init__.py
--rw-rw-rw-   0        0        0    16220 2023-07-11 19:11:19.000000 chat_exporter-2.6.0/chat_exporter/parse/markdown.py
--rw-rw-rw-   0        0        0     6799 2023-07-11 19:11:19.000000 chat_exporter-2.6.0/chat_exporter/parse/mention.py
-drwxrwxrwx   0        0        0        0 2023-07-11 19:19:13.618292 chat_exporter-2.6.0/chat_exporter.egg-info/
--rw-rw-rw-   0        0        0    11902 2023-07-11 19:19:13.000000 chat_exporter-2.6.0/chat_exporter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2610 2023-07-11 19:19:13.000000 chat_exporter-2.6.0/chat_exporter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 19:19:13.000000 chat_exporter-2.6.0/chat_exporter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-07-11 19:19:13.000000 chat_exporter-2.6.0/chat_exporter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-11 19:19:13.000000 chat_exporter-2.6.0/chat_exporter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1348 2023-07-11 19:14:07.000000 chat_exporter-2.6.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-11 19:19:13.672111 chat_exporter-2.6.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-11 20:52:24.872674 chat_exporter-2.6.1/
+-rw-rw-rw-   0        0        0    35803 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/LICENSE
+-rw-rw-rw-   0        0        0       79 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    11902 2023-07-11 20:52:24.871673 chat_exporter-2.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10649 2023-07-11 19:11:19.000000 chat_exporter-2.6.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 20:52:24.797063 chat_exporter-2.6.1/chat_exporter/
+-rw-rw-rw-   0        0        0      212 2023-07-11 20:50:45.000000 chat_exporter-2.6.1/chat_exporter/__init__.py
+-rw-rw-rw-   0        0        0     5862 2023-05-13 17:51:37.000000 chat_exporter-2.6.1/chat_exporter/chat_exporter.py
+drwxrwxrwx   0        0        0        0 2023-07-11 20:52:24.814084 chat_exporter-2.6.1/chat_exporter/construct/
+-rw-rw-rw-   0        0        0        0 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/construct/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 20:52:24.832591 chat_exporter-2.6.1/chat_exporter/construct/assets/
+-rw-rw-rw-   0        0        0      206 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/construct/assets/__init__.py
+-rw-rw-rw-   0        0        0     4018 2023-05-13 16:20:32.000000 chat_exporter-2.6.1/chat_exporter/construct/assets/attachment.py
+-rw-rw-rw-   0        0        0     3939 2023-01-09 20:42:18.000000 chat_exporter-2.6.1/chat_exporter/construct/assets/component.py
+-rw-rw-rw-   0        0        0     6239 2023-07-11 19:11:19.000000 chat_exporter-2.6.1/chat_exporter/construct/assets/embed.py
+-rw-rw-rw-   0        0        0     1544 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/construct/assets/reaction.py
+-rw-rw-rw-   0        0        0    20123 2023-07-11 20:45:29.000000 chat_exporter-2.6.1/chat_exporter/construct/message.py
+-rw-rw-rw-   0        0        0     6837 2023-07-11 19:11:19.000000 chat_exporter-2.6.1/chat_exporter/construct/transcript.py
+drwxrwxrwx   0        0        0        0 2023-07-11 20:52:24.840812 chat_exporter-2.6.1/chat_exporter/ext/
+-rw-rw-rw-   0        0        0        0 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/ext/__init__.py
+-rw-rw-rw-   0        0        0     1285 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/ext/cache.py
+-rw-rw-rw-   0        0        0      225 2023-07-11 18:47:19.000000 chat_exporter-2.6.1/chat_exporter/ext/discord_import.py
+-rw-rw-rw-   0        0        0     2123 2023-07-11 19:11:19.000000 chat_exporter-2.6.1/chat_exporter/ext/discord_utils.py
+-rw-rw-rw-   0        0        0      146 2023-07-11 19:11:19.000000 chat_exporter-2.6.1/chat_exporter/ext/discriminator.py
+-rw-rw-rw-   0        0        0     4214 2023-07-11 19:11:19.000000 chat_exporter-2.6.1/chat_exporter/ext/emoji_convert.py
+-rw-rw-rw-   0        0        0     4304 2023-07-11 19:11:19.000000 chat_exporter-2.6.1/chat_exporter/ext/html_generator.py
+drwxrwxrwx   0        0        0        0 2023-07-11 20:52:24.841812 chat_exporter-2.6.1/chat_exporter/html/
+-rw-rw-rw-   0        0        0        0 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 20:52:24.845322 chat_exporter-2.6.1/chat_exporter/html/attachment/
+-rw-rw-rw-   0        0        0      774 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/attachment/audio.html
+-rw-rw-rw-   0        0        0      140 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/attachment/image.html
+-rw-rw-rw-   0        0        0      547 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/attachment/message.html
+-rw-rw-rw-   0        0        0      127 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/attachment/video.html
+-rw-rw-rw-   0        0        0    44009 2023-07-11 19:11:19.000000 chat_exporter-2.6.1/chat_exporter/html/base.html
+drwxrwxrwx   0        0        0        0 2023-07-11 20:52:24.848322 chat_exporter-2.6.1/chat_exporter/html/component/
+-rw-rw-rw-   0        0        0      229 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/component/component_button.html
+-rw-rw-rw-   0        0        0      254 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/component/component_menu.html
+-rw-rw-rw-   0        0        0      159 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/component/component_menu_options.html
+-rw-rw-rw-   0        0        0      508 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/component/component_menu_options_emoji.html
+drwxrwxrwx   0        0        0        0 2023-07-11 20:52:24.856108 chat_exporter-2.6.1/chat_exporter/html/embed/
+-rw-rw-rw-   0        0        0      123 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/embed/author.html
+-rw-rw-rw-   0        0        0      225 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/embed/author_icon.html
+-rw-rw-rw-   0        0        0      667 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/embed/body.html
+-rw-rw-rw-   0        0        0      116 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/embed/description.html
+-rw-rw-rw-   0        0        0      317 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/embed/field-inline.html
+-rw-rw-rw-   0        0        0      306 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/embed/field.html
+-rw-rw-rw-   0        0        0      113 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/embed/footer.html
+-rw-rw-rw-   0        0        0      183 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/embed/footer_image.html
+-rw-rw-rw-   0        0        0      186 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/embed/image.html
+-rw-rw-rw-   0        0        0      206 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/embed/thumbnail.html
+-rw-rw-rw-   0        0        0       97 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/embed/title.html
+drwxrwxrwx   0        0        0        0 2023-07-11 20:52:24.865616 chat_exporter-2.6.1/chat_exporter/html/message/
+-rw-rw-rw-   0        0        0      239 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/message/bot-tag-verified.html
+-rw-rw-rw-   0        0        0       43 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/message/bot-tag.html
+-rw-rw-rw-   0        0        0       77 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/message/content.html
+-rw-rw-rw-   0        0        0        6 2023-06-24 11:50:24.000000 chat_exporter-2.6.1/chat_exporter/html/message/end.html
+-rw-rw-rw-   0        0        0      507 2023-07-11 19:11:19.000000 chat_exporter-2.6.1/chat_exporter/html/message/interaction.html
+-rw-rw-rw-   0        0        0      961 2023-07-11 19:11:19.000000 chat_exporter-2.6.1/chat_exporter/html/message/message.html
+-rw-rw-rw-   0        0        0     1108 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/message/meta.html
+-rw-rw-rw-   0        0        0     1000 2023-07-11 19:11:19.000000 chat_exporter-2.6.1/chat_exporter/html/message/pin.html
+-rw-rw-rw-   0        0        0      550 2023-07-11 19:11:19.000000 chat_exporter-2.6.1/chat_exporter/html/message/reference.html
+-rw-rw-rw-   0        0        0      131 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/message/reference_unknown.html
+-rw-rw-rw-   0        0        0     1254 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/message/start.html
+-rw-rw-rw-   0        0        0      895 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/message/thread.html
+-rw-rw-rw-   0        0        0      968 2023-07-11 19:11:19.000000 chat_exporter-2.6.1/chat_exporter/html/message/thread_add.html
+-rw-rw-rw-   0        0        0      972 2023-07-11 19:11:19.000000 chat_exporter-2.6.1/chat_exporter/html/message/thread_remove.html
+drwxrwxrwx   0        0        0        0 2023-07-11 20:52:24.866616 chat_exporter-2.6.1/chat_exporter/html/reaction/
+-rw-rw-rw-   0        0        0      206 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/reaction/custom_emoji.html
+-rw-rw-rw-   0        0        0      120 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/reaction/emoji.html
+drwxrwxrwx   0        0        0        0 2023-07-11 20:52:24.869668 chat_exporter-2.6.1/chat_exporter/html/script/
+-rw-rw-rw-   0        0        0      112 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/script/channel_subject.html
+-rw-rw-rw-   0        0        0       59 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/script/channel_topic.html
+-rw-rw-rw-   0        0        0     1183 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/html/script/fancy_time.html
+drwxrwxrwx   0        0        0        0 2023-07-11 20:52:24.870674 chat_exporter-2.6.1/chat_exporter/parse/
+-rw-rw-rw-   0        0        0        0 2022-12-25 17:56:20.000000 chat_exporter-2.6.1/chat_exporter/parse/__init__.py
+-rw-rw-rw-   0        0        0    16229 2023-07-11 20:50:45.000000 chat_exporter-2.6.1/chat_exporter/parse/markdown.py
+-rw-rw-rw-   0        0        0     6799 2023-07-11 20:44:33.000000 chat_exporter-2.6.1/chat_exporter/parse/mention.py
+drwxrwxrwx   0        0        0        0 2023-07-11 20:52:24.812080 chat_exporter-2.6.1/chat_exporter.egg-info/
+-rw-rw-rw-   0        0        0    11902 2023-07-11 20:52:24.000000 chat_exporter-2.6.1/chat_exporter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2610 2023-07-11 20:52:24.000000 chat_exporter-2.6.1/chat_exporter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 20:52:24.000000 chat_exporter-2.6.1/chat_exporter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-07-11 20:52:24.000000 chat_exporter-2.6.1/chat_exporter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-11 20:52:24.000000 chat_exporter-2.6.1/chat_exporter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1348 2023-07-11 20:50:45.000000 chat_exporter-2.6.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-11 20:52:24.872674 chat_exporter-2.6.1/setup.cfg
```

### Comparing `chat_exporter-2.6.0/LICENSE` & `chat_exporter-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.0/PKG-INFO` & `chat_exporter-2.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat_exporter
-Version: 2.6.0
+Version: 2.6.1
 Summary: A simple Discord chat exporter for Python Discord bots.
 Author-email: mahtoid <info@mahto.id>
 License: GPL-3.0-only
 Project-URL: Homepage, https://github.com/mahtoid/DiscordChatExporterPy
 Project-URL: Discord, https://discord.mahto.id/
 Project-URL: Donate, https://ko-fi.com/mahtoid
 Keywords: chat exporter,discord chat exporter,discord,discordpy,disnake,pycord,nextcord
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chat_exporter Version: 2.6.0 Summary: A simple
+Metadata-Version: 2.1 Name: chat_exporter Version: 2.6.1 Summary: A simple
 Discord chat exporter for Python Discord bots. Author-email: mahtoid
 mahto.id> License: GPL-3.0-only Project-URL: Homepage, https://github.com/
 mahtoid/DiscordChatExporterPy Project-URL: Discord, https://discord.mahto.id/
 Project-URL: Donate, https://ko-fi.com/mahtoid Keywords: chat exporter,discord
 chat exporter,discord,discordpy,disnake,pycord,nextcord Classifier: Operating
 System :: OS Independent Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English Classifier: Programming Language ::
```

### Comparing `chat_exporter-2.6.0/README.md` & `chat_exporter-2.6.1/README.md`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.0/chat_exporter/chat_exporter.py` & `chat_exporter-2.6.1/chat_exporter/chat_exporter.py`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.0/chat_exporter/construct/assets/attachment.py` & `chat_exporter-2.6.1/chat_exporter/construct/assets/attachment.py`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.0/chat_exporter/construct/assets/component.py` & `chat_exporter-2.6.1/chat_exporter/construct/assets/component.py`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.0/chat_exporter/construct/assets/embed.py` & `chat_exporter-2.6.1/chat_exporter/construct/assets/embed.py`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.0/chat_exporter/construct/assets/reaction.py` & `chat_exporter-2.6.1/chat_exporter/construct/assets/reaction.py`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.0/chat_exporter/construct/message.py` & `chat_exporter-2.6.1/chat_exporter/construct/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,15 +192,15 @@
         avatar_url = message.author.display_avatar if message.author.display_avatar else DiscordUtils.default_avatar
         self.message.reference = await fill_out(self.guild, message_reference, [
             ("AVATAR_URL", str(avatar_url), PARSE_MODE_NONE),
             ("BOT_TAG", is_bot, PARSE_MODE_NONE),
             ("NAME_TAG", await discriminator(message.author.name, message.author.discriminator), PARSE_MODE_NONE),
             ("NAME", str(html.escape(message.author.display_name))),
             ("USER_COLOUR", user_colour, PARSE_MODE_NONE),
-            ("CONTENT", message.content, PARSE_MODE_REFERENCE),
+            ("CONTENT", message.content.replace("\n", "").replace("<br>", ""), PARSE_MODE_REFERENCE),
             ("EDIT", message_edited_at, PARSE_MODE_NONE),
             ("ICON", icon, PARSE_MODE_NONE),
             ("USER_ID", str(message.author.id), PARSE_MODE_NONE),
             ("MESSAGE_ID", str(self.message.reference.message_id), PARSE_MODE_NONE),
         ])
 
     async def build_interaction(self):
```

### Comparing `chat_exporter-2.6.0/chat_exporter/construct/transcript.py` & `chat_exporter-2.6.1/chat_exporter/construct/transcript.py`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.0/chat_exporter/ext/cache.py` & `chat_exporter-2.6.1/chat_exporter/ext/cache.py`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.0/chat_exporter/ext/discord_utils.py` & `chat_exporter-2.6.1/chat_exporter/ext/discord_utils.py`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.0/chat_exporter/ext/emoji_convert.py` & `chat_exporter-2.6.1/chat_exporter/ext/emoji_convert.py`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.0/chat_exporter/ext/html_generator.py` & `chat_exporter-2.6.1/chat_exporter/ext/html_generator.py`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.0/chat_exporter/html/attachment/audio.html` & `chat_exporter-2.6.1/chat_exporter/html/attachment/audio.html`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.0/chat_exporter/html/attachment/message.html` & `chat_exporter-2.6.1/chat_exporter/html/attachment/message.html`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.0/chat_exporter/html/base.html` & `chat_exporter-2.6.1/chat_exporter/html/base.html`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.0/chat_exporter/html/embed/body.html` & `chat_exporter-2.6.1/chat_exporter/html/embed/body.html`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.0/chat_exporter/html/message/message.html` & `chat_exporter-2.6.1/chat_exporter/html/message/message.html`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.0/chat_exporter/html/message/meta.html` & `chat_exporter-2.6.1/chat_exporter/html/message/meta.html`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.0/chat_exporter/html/message/pin.html` & `chat_exporter-2.6.1/chat_exporter/html/message/pin.html`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.0/chat_exporter/html/message/reference.html` & `chat_exporter-2.6.1/chat_exporter/html/message/reference.html`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.0/chat_exporter/html/message/start.html` & `chat_exporter-2.6.1/chat_exporter/html/message/start.html`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.0/chat_exporter/html/message/thread.html` & `chat_exporter-2.6.1/chat_exporter/html/message/thread.html`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.0/chat_exporter/html/message/thread_add.html` & `chat_exporter-2.6.1/chat_exporter/html/message/thread_add.html`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.0/chat_exporter/html/message/thread_remove.html` & `chat_exporter-2.6.1/chat_exporter/html/message/thread_remove.html`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.0/chat_exporter/html/script/fancy_time.html` & `chat_exporter-2.6.1/chat_exporter/html/script/fancy_time.html`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.0/chat_exporter/parse/markdown.py` & `chat_exporter-2.6.1/chat_exporter/parse/markdown.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             while match is not None:
                 emoji_id = match.group(1)
                 self.content = self.content.replace(self.content[match.start():match.end()],
                                                     r % emoji_id)
                 match = re.search(p, self.content)
 
     def strip_preserve(self):
-        p = r'<span class="chatlog__markdown-preserve">(.*?)</span>'
+        p = r'<span class="chatlog__markdown-preserve">(.*)</span>'
         r = '%s'
 
         pattern = re.compile(p)
         match = re.search(pattern, self.content)
         while match is not None:
             affected_text = match.group(1)
             self.content = self.content.replace(self.content[match.start():match.end()],
@@ -120,23 +120,23 @@
             html += '</ul>\n'
             indent_stack.pop()
 
         if not started:
             self.content = html
 
     def parse_normal_markdown(self):
-        self.order_list_markdown_to_html()
+        # self.order_list_markdown_to_html()
         holder = (
             [r"__(.*?)__", '<span style="text-decoration: underline">%s</span>'],
             [r"\*\*(.*?)\*\*", '<strong>%s</strong>'],
             [r"\*(.*?)\*", '<em>%s</em>'],
             [r"~~(.*?)~~", '<span style="text-decoration: line-through">%s</span>'],
-            [r"###\s(.*?)\n", '<h3>%s</h1>'],
-            [r"##\s(.*?)\n", '<h2>%s</h1>'],
-            [r"#\s(.*?)\n", '<h1>%s</h1>'],
+            # [r"###\s(.*?)\n", '<h3>%s</h1>'],
+            # [r"##\s(.*?)\n", '<h2>%s</h1>'],
+            # [r"#\s(.*?)\n", '<h1>%s</h1>'],
             [r"\|\|(.*?)\|\|", '<span class="spoiler spoiler--hidden" onclick="showSpoiler(event, this)"> <span '
                                'class="spoiler-text">%s</span></span>'],
         )
 
         for x in holder:
             p, r = x
 
@@ -305,15 +305,15 @@
                     html += line
             else:
                 html += line
 
         return html
 
     def return_to_markdown(self, content):
-        content = self.order_list_html_to_markdown(content)
+        # content = self.order_list_html_to_markdown(content)
         holders = (
             [r"<strong>(.*?)</strong>", '**%s**'],
             [r"<em>([^<>]+)</em>", '*%s*'],
             [r"<h1>([^<>]+)</h1>", '# %s'],
             [r"<h2>([^<>]+)</h2>", '## %s'],
             [r"<h3>([^<>]+)</h3>", '### %s'],
             [r'<span style="text-decoration: underline">([^<>]+)</span>', '__%s__'],
```

### Comparing `chat_exporter-2.6.0/chat_exporter/parse/mention.py` & `chat_exporter-2.6.1/chat_exporter/parse/mention.py`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.0/chat_exporter.egg-info/PKG-INFO` & `chat_exporter-2.6.1/chat_exporter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-exporter
-Version: 2.6.0
+Version: 2.6.1
 Summary: A simple Discord chat exporter for Python Discord bots.
 Author-email: mahtoid <info@mahto.id>
 License: GPL-3.0-only
 Project-URL: Homepage, https://github.com/mahtoid/DiscordChatExporterPy
 Project-URL: Discord, https://discord.mahto.id/
 Project-URL: Donate, https://ko-fi.com/mahtoid
 Keywords: chat exporter,discord chat exporter,discord,discordpy,disnake,pycord,nextcord
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chat-exporter Version: 2.6.0 Summary: A simple
+Metadata-Version: 2.1 Name: chat-exporter Version: 2.6.1 Summary: A simple
 Discord chat exporter for Python Discord bots. Author-email: mahtoid
 mahto.id> License: GPL-3.0-only Project-URL: Homepage, https://github.com/
 mahtoid/DiscordChatExporterPy Project-URL: Discord, https://discord.mahto.id/
 Project-URL: Donate, https://ko-fi.com/mahtoid Keywords: chat exporter,discord
 chat exporter,discord,discordpy,disnake,pycord,nextcord Classifier: Operating
 System :: OS Independent Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English Classifier: Programming Language ::
```

### Comparing `chat_exporter-2.6.0/chat_exporter.egg-info/SOURCES.txt` & `chat_exporter-2.6.1/chat_exporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.6.0/pyproject.toml` & `chat_exporter-2.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chat_exporter"
 description = "A simple Discord chat exporter for Python Discord bots."
-version = "2.6.0"
+version = "2.6.1"
 readme = "README.md"
 authors = [
     { name="mahtoid", email="info@mahto.id" }
 ]
 requires-python = ">=3.6"
 license = { text = "GPL-3.0-only" }
 classifiers = [
```

