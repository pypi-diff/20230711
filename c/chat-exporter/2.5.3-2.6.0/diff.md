# Comparing `tmp/chat_exporter-2.5.3.tar.gz` & `tmp/chat_exporter-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat_exporter-2.5.3.tar", last modified: Wed Feb  8 22:04:05 2023, max compression
+gzip compressed data, was "chat_exporter-2.6.0.tar", last modified: Tue Jul 11 19:19:13 2023, max compression
```

## Comparing `chat_exporter-2.5.3.tar` & `chat_exporter-2.6.0.tar`

### file list

```diff
@@ -1,82 +1,85 @@
-drwxrwxrwx   0        0        0        0 2023-02-08 22:04:05.087872 chat_exporter-2.5.3/
--rw-rw-rw-   0        0        0    35803 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/LICENSE
--rw-rw-rw-   0        0        0       79 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/MANIFEST.in
--rw-rw-rw-   0        0        0    11625 2023-02-08 22:04:05.086870 chat_exporter-2.5.3/PKG-INFO
--rw-rw-rw-   0        0        0    10368 2023-02-08 22:03:33.000000 chat_exporter-2.5.3/README.md
-drwxrwxrwx   0        0        0        0 2023-02-08 22:04:04.919974 chat_exporter-2.5.3/chat_exporter/
--rw-rw-rw-   0        0        0      212 2023-02-08 22:03:33.000000 chat_exporter-2.5.3/chat_exporter/__init__.py
--rw-rw-rw-   0        0        0     5862 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/chat_exporter.py
-drwxrwxrwx   0        0        0        0 2023-02-08 22:04:04.947045 chat_exporter-2.5.3/chat_exporter/construct/
--rw-rw-rw-   0        0        0        0 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/construct/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-08 22:04:04.961189 chat_exporter-2.5.3/chat_exporter/construct/assets/
--rw-rw-rw-   0        0        0      206 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/construct/assets/__init__.py
--rw-rw-rw-   0        0        0     4018 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/construct/assets/attachment.py
--rw-rw-rw-   0        0        0     3939 2023-01-09 20:42:18.000000 chat_exporter-2.5.3/chat_exporter/construct/assets/component.py
--rw-rw-rw-   0        0        0     5972 2023-01-31 19:41:53.000000 chat_exporter-2.5.3/chat_exporter/construct/assets/embed.py
--rw-rw-rw-   0        0        0     1544 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/construct/assets/reaction.py
--rw-rw-rw-   0        0        0    16620 2023-01-09 20:59:59.000000 chat_exporter-2.5.3/chat_exporter/construct/message.py
--rw-rw-rw-   0        0        0     6643 2023-01-31 19:41:53.000000 chat_exporter-2.5.3/chat_exporter/construct/transcript.py
-drwxrwxrwx   0        0        0        0 2023-02-08 22:04:04.978186 chat_exporter-2.5.3/chat_exporter/ext/
--rw-rw-rw-   0        0        0        0 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/ext/__init__.py
--rw-rw-rw-   0        0        0     1285 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/ext/cache.py
--rw-rw-rw-   0        0        0      225 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/ext/discord_import.py
--rw-rw-rw-   0        0        0     1869 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/ext/discord_utils.py
--rw-rw-rw-   0        0        0     4210 2023-01-31 19:34:32.000000 chat_exporter-2.5.3/chat_exporter/ext/emoji_convert.py
--rw-rw-rw-   0        0        0     4146 2023-01-09 20:47:52.000000 chat_exporter-2.5.3/chat_exporter/ext/html_generator.py
-drwxrwxrwx   0        0        0        0 2023-02-08 22:04:04.980188 chat_exporter-2.5.3/chat_exporter/html/
--rw-rw-rw-   0        0        0        0 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/html/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-08 22:04:04.996187 chat_exporter-2.5.3/chat_exporter/html/attachment/
--rw-rw-rw-   0        0        0      774 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/html/attachment/audio.html
--rw-rw-rw-   0        0        0      140 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/html/attachment/image.html
--rw-rw-rw-   0        0        0      547 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/html/attachment/message.html
--rw-rw-rw-   0        0        0      127 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/html/attachment/video.html
--rw-rw-rw-   0        0        0    43667 2023-02-08 22:03:33.000000 chat_exporter-2.5.3/chat_exporter/html/base.html
-drwxrwxrwx   0        0        0        0 2023-02-08 22:04:05.006190 chat_exporter-2.5.3/chat_exporter/html/component/
--rw-rw-rw-   0        0        0      229 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/html/component/component_button.html
--rw-rw-rw-   0        0        0      254 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/html/component/component_menu.html
--rw-rw-rw-   0        0        0      159 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/html/component/component_menu_options.html
--rw-rw-rw-   0        0        0      508 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/html/component/component_menu_options_emoji.html
-drwxrwxrwx   0        0        0        0 2023-02-08 22:04:05.018195 chat_exporter-2.5.3/chat_exporter/html/embed/
--rw-rw-rw-   0        0        0      123 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/html/embed/author.html
--rw-rw-rw-   0        0        0      225 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/html/embed/author_icon.html
--rw-rw-rw-   0        0        0      667 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/html/embed/body.html
--rw-rw-rw-   0        0        0      116 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/html/embed/description.html
--rw-rw-rw-   0        0        0      317 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/html/embed/field-inline.html
--rw-rw-rw-   0        0        0      306 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/html/embed/field.html
--rw-rw-rw-   0        0        0      113 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/html/embed/footer.html
--rw-rw-rw-   0        0        0      183 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/html/embed/footer_image.html
--rw-rw-rw-   0        0        0      186 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/html/embed/image.html
--rw-rw-rw-   0        0        0      206 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/html/embed/thumbnail.html
--rw-rw-rw-   0        0        0       97 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/html/embed/title.html
-drwxrwxrwx   0        0        0        0 2023-02-08 22:04:05.059630 chat_exporter-2.5.3/chat_exporter/html/message/
--rw-rw-rw-   0        0        0      239 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/html/message/bot-tag-verified.html
--rw-rw-rw-   0        0        0       43 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/html/message/bot-tag.html
--rw-rw-rw-   0        0        0       77 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/html/message/content.html
--rw-rw-rw-   0        0        0        6 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/html/message/end.html
--rw-rw-rw-   0        0        0      528 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/html/message/interaction.html
--rw-rw-rw-   0        0        0      952 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/html/message/message.html
--rw-rw-rw-   0        0        0     1108 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/html/message/meta.html
--rw-rw-rw-   0        0        0     1021 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/html/message/pin.html
--rw-rw-rw-   0        0        0      558 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/html/message/reference.html
--rw-rw-rw-   0        0        0      131 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/html/message/reference_unknown.html
--rw-rw-rw-   0        0        0     1254 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/html/message/start.html
--rw-rw-rw-   0        0        0      895 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/html/message/thread.html
-drwxrwxrwx   0        0        0        0 2023-02-08 22:04:05.064631 chat_exporter-2.5.3/chat_exporter/html/reaction/
--rw-rw-rw-   0        0        0      206 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/html/reaction/custom_emoji.html
--rw-rw-rw-   0        0        0      120 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/html/reaction/emoji.html
-drwxrwxrwx   0        0        0        0 2023-02-08 22:04:05.078862 chat_exporter-2.5.3/chat_exporter/html/script/
--rw-rw-rw-   0        0        0      112 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/html/script/channel_subject.html
--rw-rw-rw-   0        0        0       59 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/html/script/channel_topic.html
--rw-rw-rw-   0        0        0     1183 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/html/script/fancy_time.html
-drwxrwxrwx   0        0        0        0 2023-02-08 22:04:05.085869 chat_exporter-2.5.3/chat_exporter/parse/
--rw-rw-rw-   0        0        0        0 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/parse/__init__.py
--rw-rw-rw-   0        0        0    13090 2023-01-09 20:54:25.000000 chat_exporter-2.5.3/chat_exporter/parse/markdown.py
--rw-rw-rw-   0        0        0     6707 2022-12-25 17:56:20.000000 chat_exporter-2.5.3/chat_exporter/parse/mention.py
-drwxrwxrwx   0        0        0        0 2023-02-08 22:04:04.935333 chat_exporter-2.5.3/chat_exporter.egg-info/
--rw-rw-rw-   0        0        0    11625 2023-02-08 22:04:04.000000 chat_exporter-2.5.3/chat_exporter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2486 2023-02-08 22:04:04.000000 chat_exporter-2.5.3/chat_exporter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-08 22:04:04.000000 chat_exporter-2.5.3/chat_exporter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-02-08 22:04:04.000000 chat_exporter-2.5.3/chat_exporter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-02-08 22:04:04.000000 chat_exporter-2.5.3/chat_exporter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1352 2023-02-08 22:03:33.000000 chat_exporter-2.5.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-08 22:04:05.087872 chat_exporter-2.5.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-11 19:19:13.672111 chat_exporter-2.6.0/
+-rw-rw-rw-   0        0        0    35803 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/LICENSE
+-rw-rw-rw-   0        0        0       79 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    11902 2023-07-11 19:19:13.672111 chat_exporter-2.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10649 2023-07-11 19:11:19.000000 chat_exporter-2.6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 19:19:13.605019 chat_exporter-2.6.0/chat_exporter/
+-rw-rw-rw-   0        0        0      212 2023-07-11 19:14:07.000000 chat_exporter-2.6.0/chat_exporter/__init__.py
+-rw-rw-rw-   0        0        0     5862 2023-05-13 17:51:37.000000 chat_exporter-2.6.0/chat_exporter/chat_exporter.py
+drwxrwxrwx   0        0        0        0 2023-07-11 19:19:13.619801 chat_exporter-2.6.0/chat_exporter/construct/
+-rw-rw-rw-   0        0        0        0 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/construct/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 19:19:13.631823 chat_exporter-2.6.0/chat_exporter/construct/assets/
+-rw-rw-rw-   0        0        0      206 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/construct/assets/__init__.py
+-rw-rw-rw-   0        0        0     4018 2023-05-13 16:20:32.000000 chat_exporter-2.6.0/chat_exporter/construct/assets/attachment.py
+-rw-rw-rw-   0        0        0     3939 2023-01-09 20:42:18.000000 chat_exporter-2.6.0/chat_exporter/construct/assets/component.py
+-rw-rw-rw-   0        0        0     6239 2023-07-11 19:11:19.000000 chat_exporter-2.6.0/chat_exporter/construct/assets/embed.py
+-rw-rw-rw-   0        0        0     1544 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/construct/assets/reaction.py
+-rw-rw-rw-   0        0        0    20085 2023-07-11 19:11:19.000000 chat_exporter-2.6.0/chat_exporter/construct/message.py
+-rw-rw-rw-   0        0        0     6837 2023-07-11 19:11:19.000000 chat_exporter-2.6.0/chat_exporter/construct/transcript.py
+drwxrwxrwx   0        0        0        0 2023-07-11 19:19:13.640847 chat_exporter-2.6.0/chat_exporter/ext/
+-rw-rw-rw-   0        0        0        0 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/ext/__init__.py
+-rw-rw-rw-   0        0        0     1285 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/ext/cache.py
+-rw-rw-rw-   0        0        0      225 2023-07-11 18:47:19.000000 chat_exporter-2.6.0/chat_exporter/ext/discord_import.py
+-rw-rw-rw-   0        0        0     2123 2023-07-11 19:11:19.000000 chat_exporter-2.6.0/chat_exporter/ext/discord_utils.py
+-rw-rw-rw-   0        0        0      146 2023-07-11 19:11:19.000000 chat_exporter-2.6.0/chat_exporter/ext/discriminator.py
+-rw-rw-rw-   0        0        0     4214 2023-07-11 19:11:19.000000 chat_exporter-2.6.0/chat_exporter/ext/emoji_convert.py
+-rw-rw-rw-   0        0        0     4304 2023-07-11 19:11:19.000000 chat_exporter-2.6.0/chat_exporter/ext/html_generator.py
+drwxrwxrwx   0        0        0        0 2023-07-11 19:19:13.642844 chat_exporter-2.6.0/chat_exporter/html/
+-rw-rw-rw-   0        0        0        0 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 19:19:13.644843 chat_exporter-2.6.0/chat_exporter/html/attachment/
+-rw-rw-rw-   0        0        0      774 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/attachment/audio.html
+-rw-rw-rw-   0        0        0      140 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/attachment/image.html
+-rw-rw-rw-   0        0        0      547 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/attachment/message.html
+-rw-rw-rw-   0        0        0      127 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/attachment/video.html
+-rw-rw-rw-   0        0        0    44009 2023-07-11 19:11:19.000000 chat_exporter-2.6.0/chat_exporter/html/base.html
+drwxrwxrwx   0        0        0        0 2023-07-11 19:19:13.647550 chat_exporter-2.6.0/chat_exporter/html/component/
+-rw-rw-rw-   0        0        0      229 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/component/component_button.html
+-rw-rw-rw-   0        0        0      254 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/component/component_menu.html
+-rw-rw-rw-   0        0        0      159 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/component/component_menu_options.html
+-rw-rw-rw-   0        0        0      508 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/component/component_menu_options_emoji.html
+drwxrwxrwx   0        0        0        0 2023-07-11 19:19:13.656070 chat_exporter-2.6.0/chat_exporter/html/embed/
+-rw-rw-rw-   0        0        0      123 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/embed/author.html
+-rw-rw-rw-   0        0        0      225 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/embed/author_icon.html
+-rw-rw-rw-   0        0        0      667 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/embed/body.html
+-rw-rw-rw-   0        0        0      116 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/embed/description.html
+-rw-rw-rw-   0        0        0      317 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/embed/field-inline.html
+-rw-rw-rw-   0        0        0      306 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/embed/field.html
+-rw-rw-rw-   0        0        0      113 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/embed/footer.html
+-rw-rw-rw-   0        0        0      183 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/embed/footer_image.html
+-rw-rw-rw-   0        0        0      186 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/embed/image.html
+-rw-rw-rw-   0        0        0      206 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/embed/thumbnail.html
+-rw-rw-rw-   0        0        0       97 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/embed/title.html
+drwxrwxrwx   0        0        0        0 2023-07-11 19:19:13.665091 chat_exporter-2.6.0/chat_exporter/html/message/
+-rw-rw-rw-   0        0        0      239 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/message/bot-tag-verified.html
+-rw-rw-rw-   0        0        0       43 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/message/bot-tag.html
+-rw-rw-rw-   0        0        0       77 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/message/content.html
+-rw-rw-rw-   0        0        0        6 2023-06-24 11:50:24.000000 chat_exporter-2.6.0/chat_exporter/html/message/end.html
+-rw-rw-rw-   0        0        0      507 2023-07-11 19:11:19.000000 chat_exporter-2.6.0/chat_exporter/html/message/interaction.html
+-rw-rw-rw-   0        0        0      961 2023-07-11 19:11:19.000000 chat_exporter-2.6.0/chat_exporter/html/message/message.html
+-rw-rw-rw-   0        0        0     1108 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/message/meta.html
+-rw-rw-rw-   0        0        0     1000 2023-07-11 19:11:19.000000 chat_exporter-2.6.0/chat_exporter/html/message/pin.html
+-rw-rw-rw-   0        0        0      550 2023-07-11 19:11:19.000000 chat_exporter-2.6.0/chat_exporter/html/message/reference.html
+-rw-rw-rw-   0        0        0      131 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/message/reference_unknown.html
+-rw-rw-rw-   0        0        0     1254 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/message/start.html
+-rw-rw-rw-   0        0        0      895 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/message/thread.html
+-rw-rw-rw-   0        0        0      968 2023-07-11 19:11:19.000000 chat_exporter-2.6.0/chat_exporter/html/message/thread_add.html
+-rw-rw-rw-   0        0        0      972 2023-07-11 19:11:19.000000 chat_exporter-2.6.0/chat_exporter/html/message/thread_remove.html
+drwxrwxrwx   0        0        0        0 2023-07-11 19:19:13.666091 chat_exporter-2.6.0/chat_exporter/html/reaction/
+-rw-rw-rw-   0        0        0      206 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/reaction/custom_emoji.html
+-rw-rw-rw-   0        0        0      120 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/reaction/emoji.html
+drwxrwxrwx   0        0        0        0 2023-07-11 19:19:13.669107 chat_exporter-2.6.0/chat_exporter/html/script/
+-rw-rw-rw-   0        0        0      112 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/script/channel_subject.html
+-rw-rw-rw-   0        0        0       59 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/script/channel_topic.html
+-rw-rw-rw-   0        0        0     1183 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/html/script/fancy_time.html
+drwxrwxrwx   0        0        0        0 2023-07-11 19:19:13.671111 chat_exporter-2.6.0/chat_exporter/parse/
+-rw-rw-rw-   0        0        0        0 2022-12-25 17:56:20.000000 chat_exporter-2.6.0/chat_exporter/parse/__init__.py
+-rw-rw-rw-   0        0        0    16220 2023-07-11 19:11:19.000000 chat_exporter-2.6.0/chat_exporter/parse/markdown.py
+-rw-rw-rw-   0        0        0     6799 2023-07-11 19:11:19.000000 chat_exporter-2.6.0/chat_exporter/parse/mention.py
+drwxrwxrwx   0        0        0        0 2023-07-11 19:19:13.618292 chat_exporter-2.6.0/chat_exporter.egg-info/
+-rw-rw-rw-   0        0        0    11902 2023-07-11 19:19:13.000000 chat_exporter-2.6.0/chat_exporter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2610 2023-07-11 19:19:13.000000 chat_exporter-2.6.0/chat_exporter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 19:19:13.000000 chat_exporter-2.6.0/chat_exporter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-07-11 19:19:13.000000 chat_exporter-2.6.0/chat_exporter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-11 19:19:13.000000 chat_exporter-2.6.0/chat_exporter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1348 2023-07-11 19:14:07.000000 chat_exporter-2.6.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-11 19:19:13.672111 chat_exporter-2.6.0/setup.cfg
```

### Comparing `chat_exporter-2.5.3/LICENSE` & `chat_exporter-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.5.3/PKG-INFO` & `chat_exporter-2.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: chat_exporter
-Version: 2.5.3
+Version: 2.6.0
 Summary: A simple Discord chat exporter for Python Discord bots.
 Author-email: mahtoid <info@mahto.id>
 License: GPL-3.0-only
 Project-URL: Homepage, https://github.com/mahtoid/DiscordChatExporterPy
-Project-URL: Discord, https://discord.gg/2uhHBQDwcc
+Project-URL: Discord, https://discord.mahto.id/
 Project-URL: Donate, https://ko-fi.com/mahtoid
 Keywords: chat exporter,discord chat exporter,discord,discordpy,disnake,pycord,nextcord
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -38,15 +38,15 @@
 
 
   <h2>DiscordChatExporterPy</h2>
 
   <p>
     Export Discord chats with your discord.py (or fork) bots!
     <br />
-    <a href="https://discord.gg/2uhHBQDwcc">Join Discord</a>
+    <a href="https://discord.mahto.id/">Join Discord</a>
     ·
     <a href="https://github.com/mahtoid/DiscordChatExporterPy/issues/new?assignees=&labels=bug&template=bug-report.yml">Report Bug</a>
     ·
     <a href="https://github.com/mahtoid/DiscordChatExporterPy/issues/new?assignees=&labels=enhancement&template=feature-request.yml">Request Feature</a>
   </p>
 </div>
 
@@ -120,16 +120,19 @@
 
 **Required Argument(s):**<br/>
 `channel`: `discord.TextChannel` object, whether `ctx.channel` or any channel you gather.
 
 **Optional Argument(s):**<br/>
 `limit`: Integer value to set the limit (amount of messages) the chat exporter gathers when grabbing the history (default=unlimited).<br/>
 `tz_info`: String value of a [TZ Database name](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones#List) to set a custom timezone for the exported messages (default=UTC)<br/>
+`guild`: `discord.Guild` object which can be passed in to solve bugs for certain forks<br/>
 `military_time`: Boolean value to set a 24h format for times within your exported chat (default=False | 12h format)<br/>
 `fancy_times`: Boolean value which toggles the 'fancy times' (Today|Yesterday|Day)<br/>
+`before`: `datetime.datetime` object which allows to gather messages from before a certain date
+`after`: `datetime.datetime` object which allows to gather messages from after a certain date
 `bot`: `commands.Bot` object to gather members who are no longer in your guild.
 
 **Return Argument:**<br/>
 `transcript`: The HTML build-up for you to construct the HTML File with Discord.
 
 **Example:**
 ```python
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: chat_exporter Version: 2.5.3 Summary: A simple
+Metadata-Version: 2.1 Name: chat_exporter Version: 2.6.0 Summary: A simple
 Discord chat exporter for Python Discord bots. Author-email: mahtoid
 mahto.id> License: GPL-3.0-only Project-URL: Homepage, https://github.com/
-mahtoid/DiscordChatExporterPy Project-URL: Discord, https://discord.gg/
-2uhHBQDwcc Project-URL: Donate, https://ko-fi.com/mahtoid Keywords: chat
-exporter,discord chat exporter,discord,discordpy,disnake,pycord,nextcord
-Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
-Developers Classifier: Natural Language :: English Classifier: Programming
-Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3.12 Classifier: Topic :: Internet Classifier: Topic ::
-Software Development :: Libraries Classifier: Topic :: Software Development ::
-Libraries :: Python Modules Classifier: Topic :: Utilities Classifier: Typing
-:: Typed Requires-Python: >=3.6 Description-Content-Type: text/markdown
-License-File: LICENSE
+mahtoid/DiscordChatExporterPy Project-URL: Discord, https://discord.mahto.id/
+Project-URL: Donate, https://ko-fi.com/mahtoid Keywords: chat exporter,discord
+chat exporter,discord,discordpy,disnake,pycord,nextcord Classifier: Operating
+System :: OS Independent Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English Classifier: Programming Language ::
+Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Classifier: Topic :: Internet Classifier: Topic :: Software
+Development :: Libraries Classifier: Topic :: Software Development :: Libraries
+:: Python Modules Classifier: Topic :: Utilities Classifier: Typing :: Typed
+Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
+LICENSE
 [![Version][pypi-version]][pypi-url] [![Language][language-dom]][github-url] [!
  [Forks][forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [!
 [Issues][issues-shield]][issues-url] [![GPL License][license-shield]][license-
                                      url]
                        ***** DiscordChatExporterPy *****
           Export Discord chats with your discord.py (or fork) bots!
                  Join_Discord Â· Report_Bug Â· Request_Feature
@@ -55,20 +55,24 @@
 `channel`: `discord.TextChannel` object, whether `ctx.channel` or any channel
 you gather. **Optional Argument(s):**
 `limit`: Integer value to set the limit (amount of messages) the chat exporter
 gathers when grabbing the history (default=unlimited).
 `tz_info`: String value of a [TZ Database name](https://en.wikipedia.org/wiki/
 List_of_tz_database_time_zones#List) to set a custom timezone for the exported
 messages (default=UTC)
+`guild`: `discord.Guild` object which can be passed in to solve bugs for
+certain forks
 `military_time`: Boolean value to set a 24h format for times within your
 exported chat (default=False | 12h format)
 `fancy_times`: Boolean value which toggles the 'fancy times'
 (Today|Yesterday|Day)
-`bot`: `commands.Bot` object to gather members who are no longer in your guild.
-**Return Argument:**
+`before`: `datetime.datetime` object which allows to gather messages from
+before a certain date `after`: `datetime.datetime` object which allows to
+gather messages from after a certain date `bot`: `commands.Bot` object to
+gather members who are no longer in your guild. **Return Argument:**
 `transcript`: The HTML build-up for you to construct the HTML File with
 Discord. **Example:** ```python import io ... @bot.command() async def save
 (ctx: commands.Context, limit: int = 100, tz_info: str = "UTC", military_time:
 bool = True): transcript = await chat_exporter.export( ctx.channel,
 limit=limit, tz_info=tz_info, military_time=military_time, bot=bot, ) if
 transcript is None: return transcript_file = discord.File( io.BytesIO
 (transcript.encode()), filename=f"transcript-{ctx.channel.name}.html", ) await
```

### Comparing `chat_exporter-2.5.3/README.md` & `chat_exporter-2.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
   <h2>DiscordChatExporterPy</h2>
 
   <p>
     Export Discord chats with your discord.py (or fork) bots!
     <br />
-    <a href="https://discord.gg/2uhHBQDwcc">Join Discord</a>
+    <a href="https://discord.mahto.id/">Join Discord</a>
     ·
     <a href="https://github.com/mahtoid/DiscordChatExporterPy/issues/new?assignees=&labels=bug&template=bug-report.yml">Report Bug</a>
     ·
     <a href="https://github.com/mahtoid/DiscordChatExporterPy/issues/new?assignees=&labels=enhancement&template=feature-request.yml">Request Feature</a>
   </p>
 </div>
 
@@ -91,16 +91,19 @@
 
 **Required Argument(s):**<br/>
 `channel`: `discord.TextChannel` object, whether `ctx.channel` or any channel you gather.
 
 **Optional Argument(s):**<br/>
 `limit`: Integer value to set the limit (amount of messages) the chat exporter gathers when grabbing the history (default=unlimited).<br/>
 `tz_info`: String value of a [TZ Database name](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones#List) to set a custom timezone for the exported messages (default=UTC)<br/>
+`guild`: `discord.Guild` object which can be passed in to solve bugs for certain forks<br/>
 `military_time`: Boolean value to set a 24h format for times within your exported chat (default=False | 12h format)<br/>
 `fancy_times`: Boolean value which toggles the 'fancy times' (Today|Yesterday|Day)<br/>
+`before`: `datetime.datetime` object which allows to gather messages from before a certain date
+`after`: `datetime.datetime` object which allows to gather messages from after a certain date
 `bot`: `commands.Bot` object to gather members who are no longer in your guild.
 
 **Return Argument:**<br/>
 `transcript`: The HTML build-up for you to construct the HTML File with Discord.
 
 **Example:**
 ```python
```

#### html2text {}

```diff
@@ -38,20 +38,24 @@
 `channel`: `discord.TextChannel` object, whether `ctx.channel` or any channel
 you gather. **Optional Argument(s):**
 `limit`: Integer value to set the limit (amount of messages) the chat exporter
 gathers when grabbing the history (default=unlimited).
 `tz_info`: String value of a [TZ Database name](https://en.wikipedia.org/wiki/
 List_of_tz_database_time_zones#List) to set a custom timezone for the exported
 messages (default=UTC)
+`guild`: `discord.Guild` object which can be passed in to solve bugs for
+certain forks
 `military_time`: Boolean value to set a 24h format for times within your
 exported chat (default=False | 12h format)
 `fancy_times`: Boolean value which toggles the 'fancy times'
 (Today|Yesterday|Day)
-`bot`: `commands.Bot` object to gather members who are no longer in your guild.
-**Return Argument:**
+`before`: `datetime.datetime` object which allows to gather messages from
+before a certain date `after`: `datetime.datetime` object which allows to
+gather messages from after a certain date `bot`: `commands.Bot` object to
+gather members who are no longer in your guild. **Return Argument:**
 `transcript`: The HTML build-up for you to construct the HTML File with
 Discord. **Example:** ```python import io ... @bot.command() async def save
 (ctx: commands.Context, limit: int = 100, tz_info: str = "UTC", military_time:
 bool = True): transcript = await chat_exporter.export( ctx.channel,
 limit=limit, tz_info=tz_info, military_time=military_time, bot=bot, ) if
 transcript is None: return transcript_file = discord.File( io.BytesIO
 (transcript.encode()), filename=f"transcript-{ctx.channel.name}.html", ) await
```

### Comparing `chat_exporter-2.5.3/chat_exporter/chat_exporter.py` & `chat_exporter-2.6.0/chat_exporter/chat_exporter.py`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.5.3/chat_exporter/construct/assets/attachment.py` & `chat_exporter-2.6.0/chat_exporter/construct/assets/attachment.py`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.5.3/chat_exporter/construct/assets/component.py` & `chat_exporter-2.6.0/chat_exporter/construct/assets/component.py`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.5.3/chat_exporter/construct/assets/embed.py` & `chat_exporter-2.6.0/chat_exporter/construct/assets/embed.py`

 * *Files 17% similar despite different names*

```diff
@@ -102,43 +102,51 @@
                 ])
             else:
                 self.fields += await fill_out(self.guild, embed_field, [
                     ("FIELD_NAME", field.name, PARSE_MODE_SPECIAL_EMBED),
                     ("FIELD_VALUE", field.value, PARSE_MODE_EMBED)])
 
     async def build_author(self):
-        self.author = html.escape(self.embed.author.name) if self.embed.author.name != self.check_against else ""
+        self.author = html.escape(self.embed.author.name) if (
+                self.embed.author and self.embed.author.name != self.check_against
+        ) else ""
 
         self.author = f'<a class="chatlog__embed-author-name-link" href="{self.embed.author.url}">{self.author}</a>' \
-            if self.embed.author.url != self.check_against \
-            else self.author
+            if (
+                self.embed.author and self.embed.author.url != self.check_against
+            ) else self.author
 
         author_icon = await fill_out(self.guild, embed_author_icon, [
             ("AUTHOR", self.author, PARSE_MODE_NONE),
             ("AUTHOR_ICON", self.embed.author.icon_url, PARSE_MODE_NONE)
-        ]) if self.embed.author.icon_url != self.check_against else ""
+        ]) if self.embed.author and self.embed.author.icon_url != self.check_against else ""
 
         if author_icon == "" and self.author != "":
             self.author = await fill_out(self.guild, embed_author, [("AUTHOR", self.author, PARSE_MODE_NONE)])
         else:
             self.author = author_icon
 
     async def build_image(self):
         self.image = await fill_out(self.guild, embed_image, [
             ("EMBED_IMAGE", str(self.embed.image.proxy_url), PARSE_MODE_NONE)
-        ]) if self.embed.image.url != self.check_against else ""
+        ]) if self.embed.image and self.embed.image.url != self.check_against else ""
 
     async def build_thumbnail(self):
         self.thumbnail = await fill_out(self.guild, embed_thumbnail, [
             ("EMBED_THUMBNAIL", str(self.embed.thumbnail.url), PARSE_MODE_NONE)]) \
-            if self.embed.thumbnail.url != self.check_against else ""
+            if self.embed.thumbnail and self.embed.thumbnail.url != self.check_against else ""
 
     async def build_footer(self):
-        self.footer = html.escape(self.embed.footer.text) if self.embed.footer.text != self.check_against else ""
-        footer_icon = self.embed.footer.icon_url if self.embed.footer.icon_url != self.check_against else None
+        self.footer = html.escape(self.embed.footer.text) if (
+                self.embed.footer and self.embed.footer.text != self.check_against
+        ) else ""
+
+        footer_icon = self.embed.footer.icon_url if (
+                self.embed.footer and self.embed.footer.icon_url != self.check_against
+        ) else None
 
         if not self.footer:
             return
 
         if footer_icon is not None:
             self.footer = await fill_out(self.guild, embed_footer_icon, [
                 ("EMBED_FOOTER", self.footer, PARSE_MODE_NONE),
```

### Comparing `chat_exporter-2.5.3/chat_exporter/construct/assets/reaction.py` & `chat_exporter-2.6.0/chat_exporter/construct/assets/reaction.py`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.5.3/chat_exporter/construct/message.py` & `chat_exporter-2.6.0/chat_exporter/construct/message.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from pytz import timezone
 from datetime import timedelta
 
 from chat_exporter.ext.discord_import import discord
 
 from chat_exporter.construct.assets import Attachment, Component, Embed, Reaction
 from chat_exporter.ext.discord_utils import DiscordUtils
+from chat_exporter.ext.discriminator import discriminator
 from chat_exporter.ext.html_generator import (
     fill_out,
     bot_tag,
     bot_tag_verified,
     message_body,
     message_pin,
     message_thread,
@@ -21,27 +22,29 @@
     message_interaction,
     img_attachment,
     start_message,
     end_message,
     PARSE_MODE_NONE,
     PARSE_MODE_MARKDOWN,
     PARSE_MODE_REFERENCE,
+    message_thread_remove,
+    message_thread_add,
 )
 
 
 def _gather_user_bot(author: discord.Member):
     if author.bot and author.public_flags.verified_bot:
         return bot_tag_verified
     elif author.bot:
         return bot_tag
     return ""
 
 
 def _set_edit_at(message_edited_at):
-    return f'<span class="chatlog__reference-edited-timestamp" title="{message_edited_at}">(edited)</span>'
+    return f'<span class="chatlog__reference-edited-timestamp" data-timestamp="{message_edited_at}">(edited)</span>'
 
 
 class MessageConstruct:
     message_html: str = ""
 
     # Asset Types
     embeds: str = ""
@@ -53,21 +56,23 @@
     def __init__(
         self,
         message: discord.Message,
         previous_message: Optional[discord.Message],
         pytz_timezone,
         military_time: bool,
         guild: discord.Guild,
-        meta_data: dict
+        meta_data: dict,
+        message_dict: dict
     ):
         self.message = message
         self.previous_message = previous_message
         self.pytz_timezone = pytz_timezone
         self.military_time = military_time
         self.guild = guild
+        self.message_dict = message_dict
 
         self.time_format = "%A, %e %B %Y %I:%M %p"
         if self.military_time:
             self.time_format = "%A, %e %B %Y %H:%M"
 
         self.message_created_at, self.message_edited_at = self.set_time()
         self.meta_data = meta_data
@@ -75,14 +80,18 @@
     async def construct_message(
         self,
     ) -> (str, dict):
         if discord.MessageType.pins_add == self.message.type:
             await self.build_pin()
         elif discord.MessageType.thread_created == self.message.type:
             await self.build_thread()
+        elif discord.MessageType.recipient_remove == self.message.type:
+            await self.build_thread_remove()
+        elif discord.MessageType.recipient_add == self.message.type:
+            await self.build_thread_add()
         else:
             await self.build_message()
         return self.message_html, self.meta_data
 
     async def build_message(self):
         await self.build_content()
         await self.build_reference()
@@ -96,21 +105,29 @@
         await self.generate_message_divider(channel_audit=True)
         await self.build_pin_template()
 
     async def build_thread(self):
         await self.generate_message_divider(channel_audit=True)
         await self.build_thread_template()
 
+    async def build_thread_remove(self):
+        await self.generate_message_divider(channel_audit=True)
+        await self.build_remove()
+
+    async def build_thread_add(self):
+        await self.generate_message_divider(channel_audit=True)
+        await self.build_add()
+
     async def build_meta_data(self):
         user_id = self.message.author.id
 
         if user_id in self.meta_data:
             self.meta_data[user_id][4] += 1
         else:
-            user_name_discriminator = self.message.author.name + "#" + self.message.author.discriminator
+            user_name_discriminator = await discriminator(self.message.author.name, self.message.author.discriminator)
             user_created_at = self.message.author.created_at
             user_bot = _gather_user_bot(self.message.author)
             user_avatar = (
                 self.message.author.display_avatar if self.message.author.display_avatar
                 else DiscordUtils.default_avatar
             )
             user_joined_at = self.message.author.joined_at if hasattr(self.message.author, "joined_at") else None
@@ -138,21 +155,24 @@
         ])
 
     async def build_reference(self):
         if not self.message.reference:
             self.message.reference = ""
             return
 
-        try:
-            message: discord.Message = await self.message.channel.fetch_message(self.message.reference.message_id)
-        except (discord.NotFound, discord.HTTPException) as e:
-            self.message.reference = ""
-            if isinstance(e, discord.NotFound):
-                self.message.reference = message_reference_unknown
-            return
+        message: discord.Message = self.message_dict.get(self.message.reference.message_id)
+
+        if not message:
+            try:
+                message: discord.Message = await self.message.channel.fetch_message(self.message.reference.message_id)
+            except (discord.NotFound, discord.HTTPException) as e:
+                self.message.reference = ""
+                if isinstance(e, discord.NotFound):
+                    self.message.reference = message_reference_unknown
+                return
 
         is_bot = _gather_user_bot(message.author)
         user_colour = await self._gather_user_colour(message.author)
 
         if not message.content and not message.interaction:
             message.content = "Click to see attachment"
         elif not message.content and message.interaction:
@@ -169,15 +189,15 @@
         if message_edited_at:
             message_edited_at = _set_edit_at(message_edited_at)
 
         avatar_url = message.author.display_avatar if message.author.display_avatar else DiscordUtils.default_avatar
         self.message.reference = await fill_out(self.guild, message_reference, [
             ("AVATAR_URL", str(avatar_url), PARSE_MODE_NONE),
             ("BOT_TAG", is_bot, PARSE_MODE_NONE),
-            ("NAME_TAG", "%s#%s" % (message.author.name, message.author.discriminator), PARSE_MODE_NONE),
+            ("NAME_TAG", await discriminator(message.author.name, message.author.discriminator), PARSE_MODE_NONE),
             ("NAME", str(html.escape(message.author.display_name))),
             ("USER_COLOUR", user_colour, PARSE_MODE_NONE),
             ("CONTENT", message.content, PARSE_MODE_REFERENCE),
             ("EDIT", message_edited_at, PARSE_MODE_NONE),
             ("ICON", icon, PARSE_MODE_NONE),
             ("USER_ID", str(message.author.id), PARSE_MODE_NONE),
             ("MESSAGE_ID", str(self.message.reference.message_id), PARSE_MODE_NONE),
@@ -191,15 +211,15 @@
         user: Union[discord.Member, discord.User] = self.message.interaction.user
         is_bot = _gather_user_bot(user)
         user_colour = await self._gather_user_colour(user)
         avatar_url = user.display_avatar if user.display_avatar else DiscordUtils.default_avatar
         self.message.interaction = await fill_out(self.guild, message_interaction, [
             ("AVATAR_URL", str(avatar_url), PARSE_MODE_NONE),
             ("BOT_TAG", is_bot, PARSE_MODE_NONE),
-            ("NAME_TAG", "%s#%s" % (user.name, user.discriminator), PARSE_MODE_NONE),
+            ("NAME_TAG", await discriminator(user.name, user.discriminator), PARSE_MODE_NONE),
             ("NAME", str(html.escape(user.display_name))),
             ("USER_COLOUR", user_colour, PARSE_MODE_NONE),
             ("FILLER", "used ", PARSE_MODE_NONE),
             ("COMMAND", "/" + self.message.interaction.name, PARSE_MODE_NONE),
             ("USER_ID", str(user.id), PARSE_MODE_NONE),
             ("INTERACTION_ID", str(self.message.interaction.id), PARSE_MODE_NONE),
         ])
@@ -254,25 +274,27 @@
             ("TIME", self.message_created_at.split()[-1], PARSE_MODE_NONE),
         ])
 
         return self.message_html
 
     def _generate_message_divider_check(self):
         return bool(
-            self.previous_message is None or self.message.reference != "" or self.message.interaction != "" or
+            self.previous_message is None or self.message.reference != "" or
+            self.previous_message.type is not discord.MessageType.default or self.message.interaction != "" or
             self.previous_message.author.id != self.message.author.id or self.message.webhook_id is not None or
             self.message.created_at > (self.previous_message.created_at + timedelta(minutes=4))
         )
 
     async def generate_message_divider(self, channel_audit=False):
         if channel_audit or self._generate_message_divider_check():
             if self.previous_message is not None:
                 self.message_html += await fill_out(self.guild, end_message, [])
 
             if channel_audit:
+                self.audit = True
                 return
 
             followup_symbol = ""
             is_bot = _gather_user_bot(self.message.author)
             avatar_url = self.message.author.display_avatar if self.message.author.display_avatar else DiscordUtils.default_avatar
 
             if self.message.reference != "" or self.message.interaction:
@@ -285,15 +307,15 @@
             default_timestamp = time.astimezone(timezone(self.pytz_timezone)).strftime("%d-%m-%Y %H:%M")
 
             self.message_html += await fill_out(self.guild, start_message, [
                 ("REFERENCE_SYMBOL", followup_symbol, PARSE_MODE_NONE),
                 ("REFERENCE", self.message.reference if self.message.reference else self.message.interaction,
                  PARSE_MODE_NONE),
                 ("AVATAR_URL", str(avatar_url), PARSE_MODE_NONE),
-                ("NAME_TAG", "%s#%s" % (self.message.author.name, self.message.author.discriminator), PARSE_MODE_NONE),
+                ("NAME_TAG", await discriminator(self.message.author.name, self.message.author.discriminator), PARSE_MODE_NONE),
                 ("USER_ID", str(self.message.author.id)),
                 ("USER_COLOUR", await self._gather_user_colour(self.message.author)),
                 ("USER_ICON", await self._gather_user_icon(self.message.author), PARSE_MODE_NONE),
                 ("NAME", str(html.escape(self.message.author.display_name))),
                 ("BOT_TAG", str(is_bot), PARSE_MODE_NONE),
                 ("TIMESTAMP", str(self.message_created_at)),
                 ("DEFAULT_TIMESTAMP", str(default_timestamp), PARSE_MODE_NONE),
@@ -308,27 +330,59 @@
             return True
 
     async def build_pin_template(self):
         self.message_html += await fill_out(self.guild, message_pin, [
             ("PIN_URL", DiscordUtils.pinned_message_icon, PARSE_MODE_NONE),
             ("USER_COLOUR", await self._gather_user_colour(self.message.author)),
             ("NAME", str(html.escape(self.message.author.display_name))),
-            ("NAME_TAG", "%s#%s" % (self.message.author.name, self.message.author.discriminator), PARSE_MODE_NONE),
+            ("NAME_TAG", await discriminator(self.message.author.name, self.message.author.discriminator), PARSE_MODE_NONE),
             ("MESSAGE_ID", str(self.message.id), PARSE_MODE_NONE),
             ("REF_MESSAGE_ID", str(self.message.reference.message_id), PARSE_MODE_NONE)
         ])
 
     async def build_thread_template(self):
         self.message_html += await fill_out(self.guild, message_thread, [
             ("THREAD_URL", DiscordUtils.thread_channel_icon,
              PARSE_MODE_NONE),
             ("THREAD_NAME", self.message.content, PARSE_MODE_NONE),
             ("USER_COLOUR", await self._gather_user_colour(self.message.author)),
             ("NAME", str(html.escape(self.message.author.display_name))),
-            ("NAME_TAG", "%s#%s" % (self.message.author.name, self.message.author.discriminator), PARSE_MODE_NONE),
+            ("NAME_TAG", await discriminator(self.message.author.name, self.message.author.discriminator), PARSE_MODE_NONE),
+            ("MESSAGE_ID", str(self.message.id), PARSE_MODE_NONE),
+        ])
+
+    async def build_remove(self):
+        removed_member: discord.Member = self.message.mentions[0]
+        self.message_html += await fill_out(self.guild, message_thread_remove, [
+            ("THREAD_URL", DiscordUtils.thread_remove_recipient,
+             PARSE_MODE_NONE),
+            ("USER_COLOUR", await self._gather_user_colour(self.message.author)),
+            ("NAME", str(html.escape(self.message.author.display_name))),
+            ("NAME_TAG", await discriminator(self.message.author.name, self.message.author.discriminator),
+             PARSE_MODE_NONE),
+            ("RECIPIENT_USER_COLOUR", await self._gather_user_colour(removed_member)),
+            ("RECIPIENT_NAME", str(html.escape(removed_member.display_name))),
+            ("RECIPIENT_NAME_TAG", await discriminator(removed_member.name, removed_member.discriminator),
+             PARSE_MODE_NONE),
+            ("MESSAGE_ID", str(self.message.id), PARSE_MODE_NONE),
+        ])
+
+    async def build_add(self):
+        removed_member: discord.Member = self.message.mentions[0]
+        self.message_html += await fill_out(self.guild, message_thread_add, [
+            ("THREAD_URL", DiscordUtils.thread_add_recipient,
+             PARSE_MODE_NONE),
+            ("USER_COLOUR", await self._gather_user_colour(self.message.author)),
+            ("NAME", str(html.escape(self.message.author.display_name))),
+            ("NAME_TAG", await discriminator(self.message.author.name, self.message.author.discriminator),
+             PARSE_MODE_NONE),
+            ("RECIPIENT_USER_COLOUR", await self._gather_user_colour(removed_member)),
+            ("RECIPIENT_NAME", str(html.escape(removed_member.display_name))),
+            ("RECIPIENT_NAME_TAG", await discriminator(removed_member.name, removed_member.discriminator),
+             PARSE_MODE_NONE),
             ("MESSAGE_ID", str(self.message.id), PARSE_MODE_NONE),
         ])
 
     async def _gather_member(self, author: discord.Member):
         member = self.guild.get_member(author.id)
 
         if member:
@@ -381,21 +435,34 @@
     pytz_timezone,
     military_time,
 ) -> (str, dict):
     message_html: str = ""
     meta_data: dict = {}
     previous_message: Optional[discord.Message] = None
 
+    message_dict = {message.id: message for message in messages}
+
+    if "thread" in str(messages[0].channel.type) and messages[0].reference:
+        channel = guild.get_channel(messages[0].reference.channel_id)
+
+        if not channel:
+            channel = await guild.fetch_channel(messages[0].reference.channel_id)
+
+        message = await channel.fetch_message(messages[0].reference.message_id)
+        messages[0] = message
+        messages[0].reference = None
+
     for message in messages:
         content_html, meta_data = await MessageConstruct(
             message,
             previous_message,
             pytz_timezone,
             military_time,
             guild,
-            meta_data
+            meta_data,
+            message_dict,
         ).construct_message()
         message_html += content_html
         previous_message = message
 
     message_html += "</div>"
     return message_html, meta_data
```

### Comparing `chat_exporter-2.5.3/chat_exporter/construct/transcript.py` & `chat_exporter-2.6.0/chat_exporter/construct/transcript.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import datetime
 import html
 import traceback
 
+import re
 from typing import List, Optional
 
 import pytz
 
 from chat_exporter.ext.discord_import import discord
 
 from chat_exporter.construct.message import gather_messages
@@ -77,18 +78,22 @@
         for data in meta_data:
             creation_time = meta_data[int(data)][1].astimezone(timezone).strftime("%b %d, %Y")
             joined_time = (
                 meta_data[int(data)][5].astimezone(timezone).strftime("%b %d, %Y")
                 if meta_data[int(data)][5] else "Unknown"
             )
 
+            pattern = r'^#\d{4}'
+            discrim = str(meta_data[int(data)][0][-5:])
+            user = str(meta_data[int(data)][0])
+
             meta_data_html += await fill_out(self.channel.guild, meta_data_temp, [
                 ("USER_ID", str(data), PARSE_MODE_NONE),
-                ("USERNAME", str(meta_data[int(data)][0][:-5]), PARSE_MODE_NONE),
-                ("DISCRIMINATOR", str(meta_data[int(data)][0][-5:])),
+                ("USERNAME", user[:-5] if re.match(pattern, discrim) else user, PARSE_MODE_NONE),
+                ("DISCRIMINATOR", discrim if re.match(pattern, discrim) else ""),
                 ("BOT", str(meta_data[int(data)][2]), PARSE_MODE_NONE),
                 ("CREATED_AT", str(creation_time), PARSE_MODE_NONE),
                 ("JOINED_AT", str(joined_time), PARSE_MODE_NONE),
                 ("GUILD_ICON", str(guild_icon), PARSE_MODE_NONE),
                 ("DISCORD_ICON", str(DiscordUtils.logo), PARSE_MODE_NONE),
                 ("MEMBER_ID", str(data), PARSE_MODE_NONE),
                 ("USER_AVATAR", str(meta_data[int(data)][3]), PARSE_MODE_NONE),
@@ -101,15 +106,15 @@
         raw_channel_topic = (
             self.channel.topic if isinstance(self.channel, discord.TextChannel) and self.channel.topic else ""
         )
 
         channel_topic_html = ""
         if raw_channel_topic:
             channel_topic_html = await fill_out(self.channel.guild, channel_topic, [
-                ("CHANNEL_TOPIC", raw_channel_topic)
+                ("CHANNEL_TOPIC", html.escape(raw_channel_topic))
             ])
 
         limit = "start"
         if self.limit:
             limit = f"latest {self.limit} messages"
 
         subject = await fill_out(self.channel.guild, channel_subject, [
```

### Comparing `chat_exporter-2.5.3/chat_exporter/ext/cache.py` & `chat_exporter-2.6.0/chat_exporter/ext/cache.py`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.5.3/chat_exporter/ext/discord_utils.py` & `chat_exporter-2.6.0/chat_exporter/ext/discord_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 class DiscordUtils:
     logo: str = 'https://cdn.jsdelivr.net/gh/mahtoid/DiscordUtils@master/discord-logo.svg'
     default_avatar: str = 'https://cdn.jsdelivr.net/gh/mahtoid/DiscordUtils@master/discord-default.png'
     pinned_message_icon: str = 'https://cdn.jsdelivr.net/gh/mahtoid/DiscordUtils@master/discord-pinned.svg'
     thread_channel_icon: str = 'https://cdn.jsdelivr.net/gh/mahtoid/DiscordUtils@master/discord-thread.svg'
+    thread_remove_recipient: str = 'https://cdn.jsdelivr.net/gh/mahtoid/DiscordUtils@master/discord-thread-remove-recipient.svg'
+    thread_add_recipient: str = 'https://cdn.jsdelivr.net/gh/mahtoid/DiscordUtils@master/discord-thread-add-recipient.svg'
     file_attachment_audio: str = 'https://cdn.jsdelivr.net/gh/mahtoid/DiscordUtils@master/discord-audio.svg'
     file_attachment_acrobat: str = 'https://cdn.jsdelivr.net/gh/mahtoid/DiscordUtils@master/discord-acrobat.svg'
     file_attachment_webcode: str = 'https://cdn.jsdelivr.net/gh/mahtoid/DiscordUtils@master/discord-webcode.svg'
     file_attachment_code: str = 'https://cdn.jsdelivr.net/gh/mahtoid/DiscordUtils@master/discord-code.svg'
     file_attachment_document: str = 'https://cdn.jsdelivr.net/gh/mahtoid/DiscordUtils@master/discord-document.svg'
     file_attachment_archive: str = 'https://cdn.jsdelivr.net/gh/mahtoid/DiscordUtils@master/discord-archive.svg'
     file_attachment_unknown: str = 'https://cdn.jsdelivr.net/gh/mahtoid/DiscordUtils@master/discord-unknown.svg'
```

### Comparing `chat_exporter-2.5.3/chat_exporter/ext/emoji_convert.py` & `chat_exporter-2.6.0/chat_exporter/ext/emoji_convert.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from grapheme import graphemes
 import emoji
 import aiohttp
 
 from chat_exporter.ext.cache import cache
 
 
-cdn_fmt = "https://cdnjs.cloudflare.com/ajax/libs/twemoji/14.0.2/72x72/{codepoint}.png"
+cdn_fmt = "https://cdn.jsdelivr.net/gh/jdecked/twemoji@latest/assets/72x72/{codepoint}.png"
 
 
 @cache()
 async def valid_src(src):
     try:
         async with aiohttp.ClientSession() as session:
             async with session.get(src) as resp:
```

### Comparing `chat_exporter-2.5.3/chat_exporter/ext/html_generator.py` & `chat_exporter-2.6.0/chat_exporter/ext/html_generator.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,14 +51,16 @@
 bot_tag = read_file(dir_path + "/html/message/bot-tag.html")
 bot_tag_verified = read_file(dir_path + "/html/message/bot-tag-verified.html")
 message_content = read_file(dir_path + "/html/message/content.html")
 message_reference = read_file(dir_path + "/html/message/reference.html")
 message_interaction = read_file(dir_path + "/html/message/interaction.html")
 message_pin = read_file(dir_path + "/html/message/pin.html")
 message_thread = read_file(dir_path + "/html/message/thread.html")
+message_thread_remove = read_file(dir_path + "/html/message/thread_remove.html")
+message_thread_add = read_file(dir_path + "/html/message/thread_add.html")
 message_reference_unknown = read_file(dir_path + "/html/message/reference_unknown.html")
 message_body = read_file(dir_path + "/html/message/message.html")
 end_message = read_file(dir_path + "/html/message/end.html")
 meta_data_temp = read_file(dir_path + "/html/message/meta.html")
 
 # COMPONENTS
 component_button = read_file(dir_path + "/html/component/component_button.html")
```

### Comparing `chat_exporter-2.5.3/chat_exporter/html/attachment/audio.html` & `chat_exporter-2.6.0/chat_exporter/html/attachment/audio.html`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.5.3/chat_exporter/html/attachment/message.html` & `chat_exporter-2.6.0/chat_exporter/html/attachment/message.html`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.5.3/chat_exporter/html/base.html` & `chat_exporter-2.6.0/chat_exporter/html/base.html`

 * *Files 6% similar despite different names*

```diff
@@ -12,89 +12,41 @@
 <head>
     <title>{{SERVER_NAME}} - {{CHANNEL_NAME}}</title>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
     <meta name="viewport" content="width=device-width" />
 
     <style>
         @font-face {
-          font-family: Ginto;
-          font-weight: 300;
-          src: url(https://cdn.jsdelivr.net/gh/mahtoid/DiscordUtils@master/Ginto-300.woff) format("woff")
-        }
-
-        @font-face {
-          font-family: Ginto;
+          font-family: gg sans;
           font-weight: 400;
-          src: url(https://cdn.jsdelivr.net/gh/mahtoid/DiscordUtils@master/Ginto-400.woff) format("woff")
-        }
-
-        @font-face {
-          font-family: Ginto;
-          font-weight: 500;
-          src: url(https://cdn.jsdelivr.net/gh/mahtoid/DiscordUtils@master/Ginto-500.woff) format("woff")
-        }
-
-        @font-face {
-          font-family: Ginto;
-          src: url(https://cdn.jsdelivr.net/gh/mahtoid/DiscordUtils@master/Ginto-600.woff) format("woff");
-          font-weight: 600;
-        }
-
-        @font-face {
-          font-family: Ginto;
-          font-weight: 700;
-          src: url(https://cdn.jsdelivr.net/gh/mahtoid/DiscordUtils@master/Ginto-700.woff) format("woff")
+          src: url(https://cdn.jsdelivr.net/gh/mahtoid/DiscordUtils@master/ggsans-400.woff2) format("woff2")
         }
 
         @font-face {
-          font-family: Ginto;
+          font-family: gg sans;
           font-weight: 500;
-          src: url(https://cdn.jsdelivr.net/gh/mahtoid/DiscordUtils@master/Ginto-Nord-500.woff2) format("woff2"), url(https://cdn.jsdelivr.net/gh/mahtoid/DiscordUtils@master/Ginto-Nord-500.woff) format("woff")
+          src: url(https://cdn.jsdelivr.net/gh/mahtoid/DiscordUtils@master/ggsans-500.woff2) format("woff2")
         }
 
         @font-face {
-          font-family: Ginto;
+          font-family: gg sans;
           font-weight: 600;
-          src: url(https://cdn.jsdelivr.net/gh/mahtoid/DiscordUtils@master/Ginto-Nord-600.woff2) format("woff2"), url(https://cdn.jsdelivr.net/gh/mahtoid/DiscordUtils@master/Ginto-Nord-600.woff) format("woff")
+          src: url(https://cdn.jsdelivr.net/gh/mahtoid/DiscordUtils@master/ggsans-600.woff2) format("woff2")
         }
 
         @font-face {
-          font-family: Ginto;
+          font-family: gg sans;
           font-weight: 700;
-          src: url(https://cdn.jsdelivr.net/gh/mahtoid/DiscordUtils@master/Ginto-Nord-700.woff2) format("woff2"), url(https://cdn.jsdelivr.net/gh/mahtoid/DiscordUtils@master/Ginto-Nord-700.woff) format("woff")
-        }
-
-        @font-face {
-            font-family: Whitney;
-            src: url(https://cdn.jsdelivr.net/gh/mahtoid/DiscordUtils@master/whitney-300.woff);
-            font-weight: 300;
-        }
-
-        @font-face {
-            font-family: Whitney;
-            src: url(https://cdn.jsdelivr.net/gh/mahtoid/DiscordUtils@master/whitney-400.woff);
-            font-weight: 400;
-        }
-
-        @font-face {
-            font-family: Whitney;
-            src: url(https://cdn.jsdelivr.net/gh/mahtoid/DiscordUtils@master/whitney-500.woff);
-            font-weight: 500;
+          src: url(https://cdn.jsdelivr.net/gh/mahtoid/DiscordUtils@master/ggsans-700.woff2) format("woff2")
         }
 
         @font-face {
-            font-family: Whitney;
-            src: url(https://cdn.jsdelivr.net/gh/mahtoid/DiscordUtils@master/whitney-600.woff);
-            font-weight: 600;
-        }
-
-        @font-face {
-            font-family: Whitney;
-            src: url(https://cdn.jsdelivr.net/gh/mahtoid/DiscordUtils@master/whitney-700.woff);
-            font-weight: 700;
+          font-family: gg sans;
+          font-weight: 800;
+          src: url(https://cdn.jsdelivr.net/gh/mahtoid/DiscordUtils@master/ggsans-800.woff2) format("woff2")
         }
 
         a {
             text-decoration: none;
         }
 
         a:hover {
@@ -185,14 +137,18 @@
             padding-left: 0.6em;
             border-left: 4px solid;
             border-radius: 3px;
         }
 
         .pre {
             font-family: "Consolas", "Courier New", Courier, monospace;
+            padding: .2em;
+            margin: -.2em 0;
+            border-radius: 3px;
+            font-size: 85%;
         }
 
         .pre--multiline {
             margin-top: 0.25em;
             padding: 0.5em;
             border: 2px solid;
             border-radius: 5px;
@@ -228,15 +184,14 @@
             margin: 0 0.06em;
             vertical-align: -0.4em;
         }
 
         .emoji--small {
             width: 1em;
             height: 1em;
-            padding-bottom: 4px;
         }
 
         .emoji--large {
             width: 2.8em;
             height: 2.8em;
         }
 
@@ -316,14 +271,18 @@
         .chatlog__followup-author {
             user-select: none;
             cursor: pointer;
             margin-right: 0.3rem;
             font-weight: 600;
         }
 
+        .chatlog__followup-author:hover {
+            text-decoration: underline;
+        }
+
         .chatlog__followup-content {
             user-select: none;
             overflow: hidden;
             text-overflow: ellipsis;
         }
 
         .chatlog__reference-link {
@@ -358,19 +317,21 @@
 
         .chatlog__interaction-link:hover *:not(.chatlog__markdown-spoiler) {
             color: inherit;
         }
         
         .chatlog__reference-edited-timestamp {
             margin-left: 0.25rem;
-            color: #a3a6aa;
-            font-size: 0.75rem;
-            font-weight: 500;
+            color: #9599a2;
+            font-size: 0.625rem;
+            font-weight: 400;
+            line-height: 1;
             direction: ltr;
             unicode-bidi: bidi-override;
+            user-select: none;
         }
 
         .chatlog__reference-attachment-icon {
             flex-grow: 500;
         }
 
         .chatlog__pin-avatar-container {
@@ -395,17 +356,27 @@
         }
 
         .chatlog__author-name:hover {
             text-decoration: underline;
             cursor: pointer;
         }
 
+        .chatlog__reference-name {
+            font-weight: 500;
+            color: #ffffff;
+        }
+
+        .chatlog__reference-name:hover {
+            text-decoration: underline;
+            cursor: pointer;
+        }
+
         .chatlog__timestamp {
             margin-left: 0.3rem;
-            color: #a3a6aa;
+            color: #9599a2;
             font-size: 0.75rem;
             font-weight: 500;
             direction: ltr;
             unicode-bidi: bidi-override;
         }
 
         .chatlog__content {
@@ -666,14 +637,44 @@
         }
 
         .chatlog__followup .chatlog__bot-tag {
             margin-right: 0.3rem;
             margin-top: 0;
         }
 
+        .markup {
+            white-space: normal;
+        }
+
+        .markup ul {
+            margin: 4px 0 0 16px;
+            margin-block-start: 0;
+            margin-block-end: 0;
+            padding-inline-start: 0;
+            list-style-position: outside;
+            list-style-type: circle;
+        }
+
+        .markup ul ul {
+            list-style-type: circle;
+            margin-bottom: 0;
+        }
+
+        .markup li {
+            margin: 0;
+            padding: 0;
+            border: 0;
+            font-weight: inherit;
+            font-style: inherit;
+            font-family: inherit;
+            font-size: 100%;
+            vertical-align: baseline;
+        }
+
+
         .meta__details .chatlog__bot-tag {
             margin-left: 1ch;
         }
 
         /* Postamble */
 
         .postamble {
@@ -684,15 +685,15 @@
 
         /* General */
 
         html, body {
             height: 100%;
             width: 100%;
             background-color: #36393f;
-            font-family: "Whitney";
+            font-family: "gg sans", Helvetica, Arial, sans-serif;
             font-size: 17px;
             color: #fff;
             margin: 0;
             padding: 0;
         }
 
         a {
@@ -785,22 +786,14 @@
             color: #ffffff;
         }
 
         .chatlog__interaction-link:hover {
             text-decoration: underline;
         }
 
-        .chatlog__reference-edited-timestamp {
-            color: rgba(255, 255, 255, 0.2);
-        }
-
-        .chatlog__timestamp {
-            color: rgba(255, 255, 255, 0.2);
-        }
-
         .chatlog__message--highlighted {
             background-color: rgba(114, 137, 218, 0.2) !important;
         }
 
         .chatlog__message--pinned {
             background-color: rgba(249, 168, 37, 0.05);
         }
@@ -832,19 +825,18 @@
 
         /* === INFO === */
 
         .panel {
             display: flex;
             flex-shrink: 0;
             align-items: center;
-            height: 48px;
+            padding: 6px 0 6px 0;
             user-select: none;
-            font-family: "Ginto";
-            font-weight: 500;
-            font-size: 16px;
+            font-weight: 700;
+            font-size: 20px;
             box-shadow: 0 1px 0 rgba(4, 4, 5, 0.2), 0 1.5px 0 rgba(6, 6, 7, 0.05), 0 2px 0 rgba(4, 4, 5, 0.05);
         }
 
         .panel__hashtag-icon {
             width: 24px;
             height: 24px;
             margin-left: 16px;
@@ -855,15 +847,21 @@
         .panel__channel-topic {
             border-left-style: solid;
             border-color: #4f545c;
             border-width: 1px;
             color: #b9bbbe;
             margin-left: 10px;
             padding-left: 10px;
-            font-family: 'Whitney';
+            font-size: 14px;
+            line-height: 18px;
+            height: 18px;
+            white-space: nowrap;
+            overflow: hidden;
+            text-overflow: ellipsis;
+            font-weight: 500;
         }
 
         .panel__summary-button {
             display: flex;
             align-items: center;
             padding: 0.2em 0.35em;
             border-radius: 2px;
@@ -924,28 +922,26 @@
             margin: 0 16px;
             padding-bottom: 12px;
             display: flex;
             flex-direction: column;
             justify-content: flex-end;
             flex-shrink: 0;
             user-select: none;
-            font-family: "Ginto";
         }
 
         .info__title {
-            font-size: 30px;
-            font-weight: 500;
+            font-size: 32px;
+            font-weight: 700;
             line-height: 40px;
         }
 
         .info__subject {
             color: #b9bbbe;
             font-size: 16px;
             line-height: 20px;
-            font-family: "Whitney";
         }
 
         .info__channel-message-count {
             margin-top: 2px;
         }
 
         .footer {
@@ -962,16 +958,18 @@
             z-index: 10;
             user-select: none;
         }
 
         .footer__text {
             font-size: 16px;
             line-height: 20px;
-            font-family: 'Ginto';
             font-weight: 400;
+            white-space: nowrap;
+            overflow: hidden;
+            text-overflow: ellipsis;
         }
 
         #context-menu {
             position: absolute;
             width: 188px;
             border-radius: 4px;
             padding: 6px 8px;
@@ -1072,31 +1070,28 @@
 
         .meta__display-name {
             font-weight: 500;
             color: #fff;
             opacity: 0.9;
             text-overflow: ellipsis;
             overflow: hidden;
-            font-family: 'Ginto';
             font-size: 12px;
         }
 
         .meta__user {
             font-weight: 500;
             color: #fff;
             text-overflow: ellipsis;
             overflow: hidden;
-            font-family: 'Ginto';
         }
 
         .meta__discriminator {
             font-weight: 500;
             color: #fff;
             opacity: .6;
-            font-family: 'Ginto';
         }
 
         .meta-popout .meta__header .bot {
             margin-left: 1ch;
         }
 
         .meta__description {
@@ -1232,14 +1227,36 @@
         }
 
         .chatlog__component-dropdown-border {
           border-bottom-left-radius: 0px;
           border-bottom-right-radius: 0px;
         }
 
+        .tippy-box[data-theme~='disc'] {
+            font-weight: 600;
+            background-color: #111214;
+            color: #dfe0e4;
+        }
+
+        .tippy-box[data-theme~='disc'][data-placement^='top'] > .tippy-arrow::before {
+          border-top-color: #111214;
+        }
+
+        .tippy-box[data-theme~='disc'][data-placement^='left'] > .tippy-arrow::before {
+          border-left-color: #111214;
+        }
+
+        .tippy-box[data-theme~='disc'][data-placement^='bottom'] > .tippy-arrow::before {
+          border-bottom-color: #111214;
+        }
+
+        .tippy-box[data-theme~='disc'][data-placement^='right'] > .tippy-arrow::before {
+          border-right-color: #111214;
+        }
+
         .dropdownContentDesc { color: #999B9E; }
         .dropdownButton:hover { border: 1px solid #040405; }
         .chatlog__component-dropdown-show { display: block; }
         .chatlog__component-dropdown a:hover { background-color: #292B2F; }
 
         .cursor_pointer { cursor: pointer; }
 
@@ -1542,14 +1559,28 @@
     tippy('.chatlog__timestamp', {
         placement: 'top',
         animation: 'fade',
         content: (reference) => reference.getAttribute('data-timestamp'),
         theme: 'disc',
     });
 
+    tippy('.chatlog__short-timestamp', {
+        placement: 'top',
+        animation: 'fade',
+        content: (reference) => reference.getAttribute('data-timestamp'),
+        theme: 'disc',
+    });
+
+    tippy('.chatlog__reference-edited-timestamp', {
+        placement: 'top',
+        animation: 'fade',
+        content: (reference) => reference.getAttribute('data-timestamp'),
+        theme: 'disc',
+    });
+
     <!-- Timestamps: Tooltips -->
     tippy('.unix-timestamp', {
         placement: 'top',
         animation: 'fade',
         content: (reference) => reference.getAttribute('data-timestamp'),
         theme: 'disc',
     });
```

### Comparing `chat_exporter-2.5.3/chat_exporter/html/embed/body.html` & `chat_exporter-2.6.0/chat_exporter/html/embed/body.html`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.5.3/chat_exporter/html/message/message.html` & `chat_exporter-2.6.0/chat_exporter/html/message/message.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
             <div id="chatlog__message-container-{{MESSAGE_ID}}" class="chatlog__message-container" data-message-id="{{MESSAGE_ID}}">
                     <div class="chatlog__message">
 
                         <div class="chatlog__message-aside">
-                            <div class="chatlog__short-timestamp" title="{{TIMESTAMP}}">{{TIME}}</div>
+                            <div class="chatlog__short-timestamp" data-timestamp="{{TIMESTAMP}}">{{TIME}}</div>
                         </div>
 
                         <div class="chatlog__message-primary">
                             <div class="chatlog__content chatlog__markdown" data-message-id="{{MESSAGE_ID}}" id="message-{{MESSAGE_ID}}">
                                 {{MESSAGE_CONTENT}}
 
                                 {{ATTACHMENTS}}
```

### Comparing `chat_exporter-2.5.3/chat_exporter/html/message/meta.html` & `chat_exporter-2.6.0/chat_exporter/html/message/meta.html`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.5.3/chat_exporter/html/message/pin.html` & `chat_exporter-2.6.0/chat_exporter/html/message/pin.html`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
                <img class="chatlog__pin-avatar" src="{{PIN_URL}}" />
             </div>
             <div class="chatlog__message-primary">
                 <div class="chatlog__header">
                 </div>
 
                 <div class="chatlog__content chatlog__markdown" data-message-id="{{MESSAGE_ID}}" id="message-{{MESSAGE_ID}}">
-                    <span class="chatlog__reference-name" title="{{NAME_TAG}}" style="{{USER_COLOUR}}">{{NAME}}</span> has pinned
+                    <span class="chatlog__reference-name" style="{{USER_COLOUR}}">{{NAME}}</span> has pinned
                     <a class="chatlog__pinned-link" href="#" onclick="scrollToMessage(event, '{{REF_MESSAGE_ID}}')">
                         a message
                     </a>
                     to this channel
                 </div>
             </div>
         </div>
```

### Comparing `chat_exporter-2.5.3/chat_exporter/html/message/reference.html` & `chat_exporter-2.6.0/chat_exporter/html/message/reference.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 <div class="chatlog__followup">
         <img class="chatlog__followup-avatar" src="{{AVATAR_URL}}" alt="Avatar" loading="lazy" data-user-id="{{USER_ID}}">
         {{BOT_TAG}}
-        <div class="chatlog__followup-author" style="{{USER_COLOUR}}" title="{{NAME_TAG}}" data-user-id="{{USER_ID}}">{{NAME}}</div>
+        <div class="chatlog__followup-author" style="{{USER_COLOUR}}" data-user-id="{{USER_ID}}">{{NAME}}</div>
         <div class="chatlog__followup-content">
             <span class="chatlog__reference-link" onclick="scrollToMessage(event, '{{MESSAGE_ID}}')">
-                    <em>{{CONTENT}}</em> {{ICON}}
+                    {{CONTENT}} {{ICON}}
             </span>
+            {{EDIT}}
         </div>
 </div>
```

### Comparing `chat_exporter-2.5.3/chat_exporter/html/message/start.html` & `chat_exporter-2.6.0/chat_exporter/html/message/start.html`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.5.3/chat_exporter/html/message/thread.html` & `chat_exporter-2.6.0/chat_exporter/html/message/thread.html`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.5.3/chat_exporter/html/script/fancy_time.html` & `chat_exporter-2.6.0/chat_exporter/html/script/fancy_time.html`

 * *Files identical despite different names*

### Comparing `chat_exporter-2.5.3/chat_exporter/parse/markdown.py` & `chat_exporter-2.6.0/chat_exporter/parse/markdown.py`

 * *Files 18% similar despite different names*

```diff
@@ -33,18 +33,17 @@
         self.parse_normal_markdown()
         self.parse_code_block_markdown()
         await self.parse_emoji()
 
         return self.content
 
     async def message_reference_flow(self):
-        self.https_http_links()
+        self.strip_preserve()
         self.parse_normal_markdown()
         self.parse_code_block_markdown(reference=True)
-        await self.parse_emoji()
         self.parse_br()
 
         return self.content
 
     async def special_emoji_flow(self):
         await self.parse_emoji()
         return self.content
@@ -67,31 +66,89 @@
             match = re.search(p, self.content)
             while match is not None:
                 emoji_id = match.group(1)
                 self.content = self.content.replace(self.content[match.start():match.end()],
                                                     r % emoji_id)
                 match = re.search(p, self.content)
 
+    def strip_preserve(self):
+        p = r'<span class="chatlog__markdown-preserve">(.*?)</span>'
+        r = '%s'
+
+        pattern = re.compile(p)
+        match = re.search(pattern, self.content)
+        while match is not None:
+            affected_text = match.group(1)
+            self.content = self.content.replace(self.content[match.start():match.end()],
+                                                r % affected_text)
+            match = re.search(pattern, self.content)
+
+    def order_list_markdown_to_html(self):
+        lines = self.content.split('\n')
+        html = ''
+        indent_stack = [0]
+        started = True
+
+        for line in lines:
+            match = re.match(r'^(\s*)([-*])\s+(.+)$', line)
+            if match:
+                indent, bullet, content = match.groups()
+                indent = len(indent)
+
+                if started:
+                    html += '<ul class="markup">\n'
+                    started = False
+                if indent % 2 == 0:
+                    while indent < indent_stack[-1]:
+                        html += '</ul>\n'
+                        indent_stack.pop()
+                    if indent > indent_stack[-1]:
+                        html += '<ul class="markup">\n'
+                        indent_stack.append(indent)
+                else:
+                    while indent + 1 < indent_stack[-1]:
+                        html += '</ul>\n'
+                        indent_stack.pop()
+                    if indent + 1 > indent_stack[-1]:
+                        html += '<ul class="markup">\n'
+                        indent_stack.append(indent + 1)
+
+                html += f'<li class="markup">{content.strip()}</li>\n'
+            else:
+                html += line
+
+        while len(indent_stack) > 1:
+            html += '</ul>\n'
+            indent_stack.pop()
+
+        if not started:
+            self.content = html
+
     def parse_normal_markdown(self):
-        holder = [r"__(.*?)__", '<span style="text-decoration: underline">%s</span>'], \
-                 [r"\*\*(.*?)\*\*", '<strong>%s</strong>'], \
-                 [r"\*(.*?)\*", '<em>%s</em>'], \
-                 [r"~~(.*?)~~", '<span style="text-decoration: line-through">%s</span>'], \
-                 [r"\|\|(.*?)\|\|", '<span class="spoiler spoiler--hidden" onclick="showSpoiler(event, this)"> <span '
-                                    'class="spoiler-text">%s</span></span>']
+        self.order_list_markdown_to_html()
+        holder = (
+            [r"__(.*?)__", '<span style="text-decoration: underline">%s</span>'],
+            [r"\*\*(.*?)\*\*", '<strong>%s</strong>'],
+            [r"\*(.*?)\*", '<em>%s</em>'],
+            [r"~~(.*?)~~", '<span style="text-decoration: line-through">%s</span>'],
+            [r"###\s(.*?)\n", '<h3>%s</h1>'],
+            [r"##\s(.*?)\n", '<h2>%s</h1>'],
+            [r"#\s(.*?)\n", '<h1>%s</h1>'],
+            [r"\|\|(.*?)\|\|", '<span class="spoiler spoiler--hidden" onclick="showSpoiler(event, this)"> <span '
+                               'class="spoiler-text">%s</span></span>'],
+        )
 
         for x in holder:
             p, r = x
 
             pattern = re.compile(p)
             match = re.search(pattern, self.content)
             while match is not None:
                 affected_text = match.group(1)
-                self.content = self.content.replace(self.content[match.start():match.end()],
-                                                    r % affected_text)
+                self.content = self.content.replace(self.content[match.start():match.end()], r % affected_text)
                 match = re.search(pattern, self.content)
 
         # > quote
         self.content = self.content.split("<br>")
         y = None
         new_content = ""
         pattern = re.compile(r"^&gt;\s(.+)")
@@ -221,18 +278,48 @@
 
         if y:
             new_content = new_content + f'<div class="quote">{y}</div>'
 
         self.content = new_content
 
     @staticmethod
-    def return_to_markdown(content):
+    def order_list_html_to_markdown(content):
+        lines = content.split('<br>')
+        html = ''
+        ul_level = -1
+
+        for line in lines:
+            if '<ul class="markup">' in line:
+                ul_level += 1
+                line = line.replace('<ul class="markup">', '')
+                if line != "":
+                    html += line + "\n"
+            elif "</ul>" in line:
+                ul_level -= 1
+            elif '<li class="markup">' in line:
+                match = re.match(r'<li class="markup">(.+?)</li>', line)
+                if match:
+                    matched_content = match.group(1)
+                    spaces = ul_level * 2
+                    html += " " * spaces + "-" + matched_content + "\n"
+                else:
+                    html += line
+            else:
+                html += line
+
+        return html
+
+    def return_to_markdown(self, content):
+        content = self.order_list_html_to_markdown(content)
         holders = (
             [r"<strong>(.*?)</strong>", '**%s**'],
             [r"<em>([^<>]+)</em>", '*%s*'],
+            [r"<h1>([^<>]+)</h1>", '# %s'],
+            [r"<h2>([^<>]+)</h2>", '## %s'],
+            [r"<h3>([^<>]+)</h3>", '### %s'],
             [r'<span style="text-decoration: underline">([^<>]+)</span>', '__%s__'],
             [r'<span style="text-decoration: line-through">([^<>]+)</span>', '~~%s~~'],
             [r'<div class="quote">(.*?)</div>', '> %s'],
             [r'<span class="spoiler spoiler--hidden" onclick="showSpoiler\(event, this\)"> <span '
              r'class="spoiler-text">(.*?)<\/span><\/span>', '||%s||'],
             [r'<span class="unix-timestamp" data-timestamp=".*?" raw-content="(.*?)">.*?</span>', '%s']
         )
```

### Comparing `chat_exporter-2.5.3/chat_exporter/parse/mention.py` & `chat_exporter-2.6.0/chat_exporter/parse/mention.py`

 * *Files 5% similar despite different names*

```diff
@@ -137,15 +137,18 @@
                 self.content = self.content.replace(self.content[match.start():match.end()],
                                                     replacement)
 
                 match = re.search(regex, self.content)
 
     async def time_mention(self):
         holder = self.REGEX_TIME_HOLDER
-        timezone = pytz.timezone(self.guild.timezone)
+        timezone = pytz.timezone("UTC")
+
+        if hasattr(self.guild, "timezone"):
+            timezone = pytz.timezone(self.guild.timezone)
 
         for p in holder:
             regex, strf = p
             match = re.search(regex, self.content)
             while match is not None:
                 time = datetime.datetime.fromtimestamp(int(match.group(1)), timezone)
                 ui_time = time.strftime(strf)
```

### Comparing `chat_exporter-2.5.3/chat_exporter.egg-info/PKG-INFO` & `chat_exporter-2.6.0/chat_exporter.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: chat-exporter
-Version: 2.5.3
+Version: 2.6.0
 Summary: A simple Discord chat exporter for Python Discord bots.
 Author-email: mahtoid <info@mahto.id>
 License: GPL-3.0-only
 Project-URL: Homepage, https://github.com/mahtoid/DiscordChatExporterPy
-Project-URL: Discord, https://discord.gg/2uhHBQDwcc
+Project-URL: Discord, https://discord.mahto.id/
 Project-URL: Donate, https://ko-fi.com/mahtoid
 Keywords: chat exporter,discord chat exporter,discord,discordpy,disnake,pycord,nextcord
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -38,15 +38,15 @@
 
 
   <h2>DiscordChatExporterPy</h2>
 
   <p>
     Export Discord chats with your discord.py (or fork) bots!
     <br />
-    <a href="https://discord.gg/2uhHBQDwcc">Join Discord</a>
+    <a href="https://discord.mahto.id/">Join Discord</a>
     ·
     <a href="https://github.com/mahtoid/DiscordChatExporterPy/issues/new?assignees=&labels=bug&template=bug-report.yml">Report Bug</a>
     ·
     <a href="https://github.com/mahtoid/DiscordChatExporterPy/issues/new?assignees=&labels=enhancement&template=feature-request.yml">Request Feature</a>
   </p>
 </div>
 
@@ -120,16 +120,19 @@
 
 **Required Argument(s):**<br/>
 `channel`: `discord.TextChannel` object, whether `ctx.channel` or any channel you gather.
 
 **Optional Argument(s):**<br/>
 `limit`: Integer value to set the limit (amount of messages) the chat exporter gathers when grabbing the history (default=unlimited).<br/>
 `tz_info`: String value of a [TZ Database name](https://en.wikipedia.org/wiki/List_of_tz_database_time_zones#List) to set a custom timezone for the exported messages (default=UTC)<br/>
+`guild`: `discord.Guild` object which can be passed in to solve bugs for certain forks<br/>
 `military_time`: Boolean value to set a 24h format for times within your exported chat (default=False | 12h format)<br/>
 `fancy_times`: Boolean value which toggles the 'fancy times' (Today|Yesterday|Day)<br/>
+`before`: `datetime.datetime` object which allows to gather messages from before a certain date
+`after`: `datetime.datetime` object which allows to gather messages from after a certain date
 `bot`: `commands.Bot` object to gather members who are no longer in your guild.
 
 **Return Argument:**<br/>
 `transcript`: The HTML build-up for you to construct the HTML File with Discord.
 
 **Example:**
 ```python
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1 Name: chat-exporter Version: 2.5.3 Summary: A simple
+Metadata-Version: 2.1 Name: chat-exporter Version: 2.6.0 Summary: A simple
 Discord chat exporter for Python Discord bots. Author-email: mahtoid
 mahto.id> License: GPL-3.0-only Project-URL: Homepage, https://github.com/
-mahtoid/DiscordChatExporterPy Project-URL: Discord, https://discord.gg/
-2uhHBQDwcc Project-URL: Donate, https://ko-fi.com/mahtoid Keywords: chat
-exporter,discord chat exporter,discord,discordpy,disnake,pycord,nextcord
-Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
-Developers Classifier: Natural Language :: English Classifier: Programming
-Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3.12 Classifier: Topic :: Internet Classifier: Topic ::
-Software Development :: Libraries Classifier: Topic :: Software Development ::
-Libraries :: Python Modules Classifier: Topic :: Utilities Classifier: Typing
-:: Typed Requires-Python: >=3.6 Description-Content-Type: text/markdown
-License-File: LICENSE
+mahtoid/DiscordChatExporterPy Project-URL: Discord, https://discord.mahto.id/
+Project-URL: Donate, https://ko-fi.com/mahtoid Keywords: chat exporter,discord
+chat exporter,discord,discordpy,disnake,pycord,nextcord Classifier: Operating
+System :: OS Independent Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English Classifier: Programming Language ::
+Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Classifier: Topic :: Internet Classifier: Topic :: Software
+Development :: Libraries Classifier: Topic :: Software Development :: Libraries
+:: Python Modules Classifier: Topic :: Utilities Classifier: Typing :: Typed
+Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
+LICENSE
 [![Version][pypi-version]][pypi-url] [![Language][language-dom]][github-url] [!
  [Forks][forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [!
 [Issues][issues-shield]][issues-url] [![GPL License][license-shield]][license-
                                      url]
                        ***** DiscordChatExporterPy *****
           Export Discord chats with your discord.py (or fork) bots!
                  Join_Discord Â· Report_Bug Â· Request_Feature
@@ -55,20 +55,24 @@
 `channel`: `discord.TextChannel` object, whether `ctx.channel` or any channel
 you gather. **Optional Argument(s):**
 `limit`: Integer value to set the limit (amount of messages) the chat exporter
 gathers when grabbing the history (default=unlimited).
 `tz_info`: String value of a [TZ Database name](https://en.wikipedia.org/wiki/
 List_of_tz_database_time_zones#List) to set a custom timezone for the exported
 messages (default=UTC)
+`guild`: `discord.Guild` object which can be passed in to solve bugs for
+certain forks
 `military_time`: Boolean value to set a 24h format for times within your
 exported chat (default=False | 12h format)
 `fancy_times`: Boolean value which toggles the 'fancy times'
 (Today|Yesterday|Day)
-`bot`: `commands.Bot` object to gather members who are no longer in your guild.
-**Return Argument:**
+`before`: `datetime.datetime` object which allows to gather messages from
+before a certain date `after`: `datetime.datetime` object which allows to
+gather messages from after a certain date `bot`: `commands.Bot` object to
+gather members who are no longer in your guild. **Return Argument:**
 `transcript`: The HTML build-up for you to construct the HTML File with
 Discord. **Example:** ```python import io ... @bot.command() async def save
 (ctx: commands.Context, limit: int = 100, tz_info: str = "UTC", military_time:
 bool = True): transcript = await chat_exporter.export( ctx.channel,
 limit=limit, tz_info=tz_info, military_time=military_time, bot=bot, ) if
 transcript is None: return transcript_file = discord.File( io.BytesIO
 (transcript.encode()), filename=f"transcript-{ctx.channel.name}.html", ) await
```

### Comparing `chat_exporter-2.5.3/chat_exporter.egg-info/SOURCES.txt` & `chat_exporter-2.6.0/chat_exporter.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 chat_exporter/construct/assets/component.py
 chat_exporter/construct/assets/embed.py
 chat_exporter/construct/assets/reaction.py
 chat_exporter/ext/__init__.py
 chat_exporter/ext/cache.py
 chat_exporter/ext/discord_import.py
 chat_exporter/ext/discord_utils.py
+chat_exporter/ext/discriminator.py
 chat_exporter/ext/emoji_convert.py
 chat_exporter/ext/html_generator.py
 chat_exporter/html/__init__.py
 chat_exporter/html/base.html
 chat_exporter/html/attachment/audio.html
 chat_exporter/html/attachment/image.html
 chat_exporter/html/attachment/message.html
@@ -52,14 +53,16 @@
 chat_exporter/html/message/message.html
 chat_exporter/html/message/meta.html
 chat_exporter/html/message/pin.html
 chat_exporter/html/message/reference.html
 chat_exporter/html/message/reference_unknown.html
 chat_exporter/html/message/start.html
 chat_exporter/html/message/thread.html
+chat_exporter/html/message/thread_add.html
+chat_exporter/html/message/thread_remove.html
 chat_exporter/html/reaction/custom_emoji.html
 chat_exporter/html/reaction/emoji.html
 chat_exporter/html/script/channel_subject.html
 chat_exporter/html/script/channel_topic.html
 chat_exporter/html/script/fancy_time.html
 chat_exporter/parse/__init__.py
 chat_exporter/parse/markdown.py
```

### Comparing `chat_exporter-2.5.3/pyproject.toml` & `chat_exporter-2.6.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chat_exporter"
 description = "A simple Discord chat exporter for Python Discord bots."
-version = "2.5.3"
+version = "2.6.0"
 readme = "README.md"
 authors = [
     { name="mahtoid", email="info@mahto.id" }
 ]
 requires-python = ">=3.6"
 license = { text = "GPL-3.0-only" }
 classifiers = [
@@ -30,9 +30,9 @@
     "Typing :: Typed",
 ]
 dependencies = ["aiohttp", "pytz", "grapheme", "emoji"]
 keywords = ["chat exporter", "discord chat exporter", "discord", "discordpy", "disnake", "pycord", "nextcord"]
 
 [project.urls]
 Homepage = "https://github.com/mahtoid/DiscordChatExporterPy"
-Discord = "https://discord.gg/2uhHBQDwcc"
+Discord = "https://discord.mahto.id/"
 Donate = "https://ko-fi.com/mahtoid"
```

