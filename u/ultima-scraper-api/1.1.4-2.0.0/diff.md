# Comparing `tmp/ultima_scraper_api-1.1.4.tar.gz` & `tmp/ultima_scraper_api-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultima_scraper_api-1.1.4.tar", max compression
+gzip compressed data, was "ultima_scraper_api-2.0.0.tar", max compression
```

## Comparing `ultima_scraper_api-1.1.4.tar` & `ultima_scraper_api-2.0.0.tar`

### file list

```diff
@@ -1,61 +1,62 @@
--rw-r--r--   0        0        0     1214 2023-06-14 18:29:27.848708 ultima_scraper_api-1.1.4/pyproject.toml
--rw-r--r--   0        0        0      175 2022-12-03 17:24:36.799421 ultima_scraper_api-1.1.4/ultima_scraper_api/.readthedocs.yaml
--rw-r--r--   0        0        0     2499 2023-06-15 03:55:06.849210 ultima_scraper_api-1.1.4/ultima_scraper_api/__init__.py
--rw-r--r--   0        0        0        0 2022-12-04 09:00:20.736402 ultima_scraper_api-1.1.4/ultima_scraper_api/__main__.py
--rw-r--r--   0        0        0        0 2022-12-04 15:38:35.491230 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/__init__.py
--rw-r--r--   0        0        0     6913 2023-06-01 15:05:27.454325 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/api_helper.py
--rw-r--r--   0        0        0     2983 2023-06-01 21:49:26.036612 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/api_streamliner.py
--rw-r--r--   0        0        0     1306 2023-06-15 08:27:10.520823 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/auth_streamliner.py
--rw-r--r--   0        0        0      696 2022-12-02 16:36:46.812390 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/background_tasks.py
--rw-r--r--   0        0        0     2891 2023-06-01 20:52:37.751350 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/__init__.py
--rw-r--r--   0        0        0      189 2023-05-13 20:33:08.152436 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/classes/__init__.py
--rw-r--r--   0        0        0    12932 2023-06-15 08:56:58.240672 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/classes/auth_model.py
--rw-r--r--   0        0        0     6511 2023-04-10 15:12:02.910813 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/classes/collection_model.py
--rw-r--r--   0        0        0    15106 2023-06-15 08:12:06.529813 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/classes/extras.py
--rw-r--r--   0        0        0      472 2022-01-17 19:20:07.000000 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/classes/hightlight_model.py
--rw-r--r--   0        0        0     6433 2023-06-07 23:41:16.462833 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/classes/message_model.py
--rw-r--r--   0        0        0     6914 2023-06-01 20:52:37.758016 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/classes/post_model.py
--rw-r--r--   0        0        0     3210 2023-05-14 02:55:01.328937 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/classes/story_model.py
--rw-r--r--   0        0        0      862 2023-05-14 01:36:53.261674 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/classes/subscription_model.py
--rw-r--r--   0        0        0    27732 2023-06-15 05:16:50.559836 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/classes/user_model.py
--rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/decorators/decorators.py
--rw-r--r--   0        0        0     6306 2023-06-15 08:12:42.082002 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/fansly.py
--rw-r--r--   0        0        0     2810 2023-06-07 23:39:07.287094 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/__init__.py
--rw-r--r--   0        0        0      191 2023-06-01 22:07:45.846163 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/classes/__init__.py
--rw-r--r--   0        0        0    13837 2023-06-15 08:57:37.093501 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/classes/auth_model.py
--rw-r--r--   0        0        0    17105 2023-06-15 08:51:10.952788 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/classes/extras.py
--rw-r--r--   0        0        0      686 2023-03-25 19:37:35.462288 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py
--rw-r--r--   0        0        0     2940 2023-06-07 23:41:09.279737 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/classes/message_model.py
--rw-r--r--   0        0        0     5863 2023-05-22 05:00:15.206814 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/classes/only_drm.py
--rw-r--r--   0        0        0     3341 2023-06-15 08:39:06.344592 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/classes/post_model.py
--rw-r--r--   0        0        0     1318 2023-06-15 08:39:00.921432 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/classes/story_model.py
--rw-r--r--   0        0        0     1623 2023-05-13 21:04:18.608237 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/classes/subscription_model.py
--rw-r--r--   0        0        0    28895 2023-06-15 06:10:58.787578 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/classes/user_model.py
--rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/decorators/decorators.py
--rw-r--r--   0        0        0     6689 2023-06-14 15:08:49.308972 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/onlyfans.py
--rw-r--r--   0        0        0     2759 2023-06-01 20:52:37.711351 ultima_scraper_api-1.1.4/ultima_scraper_api/apis/user_streamliner.py
--rw-r--r--   0        0        0        0 2022-12-04 09:59:08.749358 ultima_scraper_api-1.1.4/ultima_scraper_api/classes/__init__.py
--rw-r--r--   0        0        0    13187 2023-03-24 22:26:49.870986 ultima_scraper_api-1.1.4/ultima_scraper_api/classes/make_settings.py
--rw-r--r--   0        0        0     3977 2023-03-12 11:46:35.721289 ultima_scraper_api-1.1.4/ultima_scraper_api/classes/prepare_directories.py
--rw-r--r--   0        0        0      340 2022-01-17 19:20:07.000000 ultima_scraper_api-1.1.4/ultima_scraper_api/classes/prepare_download.py
--rw-r--r--   0        0        0    13410 2023-05-07 21:56:21.760084 ultima_scraper_api-1.1.4/ultima_scraper_api/classes/prepare_metadata.py
--rw-r--r--   0        0        0      630 2022-01-17 19:20:07.000000 ultima_scraper_api-1.1.4/ultima_scraper_api/classes/prepare_webhooks.py
--rw-r--r--   0        0        0     1204 2023-06-15 09:03:54.583570 ultima_scraper_api-1.1.4/ultima_scraper_api/config.py
--rw-r--r--   0        0        0      638 2022-12-03 12:11:12.443198 ultima_scraper_api-1.1.4/ultima_scraper_api/docs/Makefile
--rw-r--r--   0        0        0      804 2022-12-03 12:11:12.443198 ultima_scraper_api-1.1.4/ultima_scraper_api/docs/make.bat
--rw-r--r--   0        0        0       21 2022-12-03 17:06:06.309429 ultima_scraper_api-1.1.4/ultima_scraper_api/docs/requirements.txt
--rw-r--r--   0        0        0     1318 2022-12-03 18:16:52.399681 ultima_scraper_api-1.1.4/ultima_scraper_api/docs/source/conf.py
--rw-r--r--   0        0        0      464 2022-12-03 17:00:27.610084 ultima_scraper_api-1.1.4/ultima_scraper_api/docs/source/index.rst
--rw-r--r--   0        0        0        0 2022-12-04 09:51:18.483387 ultima_scraper_api-1.1.4/ultima_scraper_api/helpers/__init__.py
--rw-r--r--   0        0        0    12020 2023-06-15 08:33:26.165471 ultima_scraper_api-1.1.4/ultima_scraper_api/helpers/main_helper.py
--rw-r--r--   0        0        0        0 2023-01-26 05:39:16.747803 ultima_scraper_api-1.1.4/ultima_scraper_api/managers/__init__.py
--rw-r--r--   0        0        0        0 2023-01-22 17:41:52.794214 ultima_scraper_api-1.1.4/ultima_scraper_api/managers/job_manager/__init__.py
--rw-r--r--   0        0        0     1911 2023-05-31 10:43:31.029509 ultima_scraper_api-1.1.4/ultima_scraper_api/managers/job_manager/job_manager.py
--rw-r--r--   0        0        0        0 2023-01-22 17:42:18.641239 ultima_scraper_api-1.1.4/ultima_scraper_api/managers/job_manager/jobs/__init__.py
--rw-r--r--   0        0        0      767 2023-05-12 15:00:15.819155 ultima_scraper_api-1.1.4/ultima_scraper_api/managers/job_manager/jobs/custom_job.py
--rw-r--r--   0        0        0     2179 2023-06-01 22:11:24.179495 ultima_scraper_api-1.1.4/ultima_scraper_api/managers/scrape_manager.py
--rw-r--r--   0        0        0    18429 2023-06-15 03:54:30.180364 ultima_scraper_api-1.1.4/ultima_scraper_api/managers/session_manager.py
--rw-r--r--   0        0        0        0 2023-05-09 14:42:23.613712 ultima_scraper_api-1.1.4/ultima_scraper_api/models/__init__.py
--rw-r--r--   0        0        0      677 2023-05-11 21:44:11.005112 ultima_scraper_api-1.1.4/ultima_scraper_api/models/subscription_model.py
--rw-r--r--   0        0        0        0 2022-12-04 16:42:28.821209 ultima_scraper_api-1.1.4/ultima_scraper_api/py.typed
--rw-r--r--   0        0        0     1094 1970-01-01 00:00:00.000000 ultima_scraper_api-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1214 2023-07-11 11:46:57.031789 ultima_scraper_api-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      175 2022-12-03 17:24:36.799421 ultima_scraper_api-2.0.0/ultima_scraper_api/.readthedocs.yaml
+-rw-r--r--   0        0        0     2532 2023-07-11 07:31:18.304539 ultima_scraper_api-2.0.0/ultima_scraper_api/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-04 09:00:20.736402 ultima_scraper_api-2.0.0/ultima_scraper_api/__main__.py
+-rw-r--r--   0        0        0        0 2022-12-04 15:38:35.491230 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/__init__.py
+-rw-r--r--   0        0        0     6913 2023-06-01 15:05:27.454325 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/api_helper.py
+-rw-r--r--   0        0        0     3377 2023-07-11 02:37:00.259116 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/api_streamliner.py
+-rw-r--r--   0        0        0     1306 2023-06-15 08:27:10.520823 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/auth_streamliner.py
+-rw-r--r--   0        0        0      635 2023-07-11 11:18:35.577703 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/background_tasks.py
+-rw-r--r--   0        0        0     2890 2023-07-11 11:19:18.696746 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/__init__.py
+-rw-r--r--   0        0        0      189 2023-05-13 20:33:08.152436 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/classes/__init__.py
+-rw-r--r--   0        0        0    13795 2023-07-10 03:49:56.772912 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/classes/auth_model.py
+-rw-r--r--   0        0        0     6562 2023-07-09 22:21:57.158649 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/classes/collection_model.py
+-rw-r--r--   0        0        0      655 2023-07-08 10:22:46.596423 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/classes/comment_model.py
+-rw-r--r--   0        0        0    14991 2023-07-10 03:22:18.901274 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/classes/extras.py
+-rw-r--r--   0        0        0      472 2022-01-17 19:20:07.000000 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/classes/hightlight_model.py
+-rw-r--r--   0        0        0     6479 2023-07-08 08:28:30.959843 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/classes/message_model.py
+-rw-r--r--   0        0        0     7348 2023-07-09 22:27:49.103017 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/classes/post_model.py
+-rw-r--r--   0        0        0     3210 2023-05-14 02:55:01.328937 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/classes/story_model.py
+-rw-r--r--   0        0        0     1102 2023-07-09 22:28:09.345831 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/classes/subscription_model.py
+-rw-r--r--   0        0        0    27699 2023-07-10 03:52:55.262488 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/classes/user_model.py
+-rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/decorators/decorators.py
+-rw-r--r--   0        0        0     6353 2023-07-11 07:36:55.711368 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/fansly.py
+-rw-r--r--   0        0        0     2774 2023-07-08 03:39:16.755488 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/__init__.py
+-rw-r--r--   0        0        0      191 2023-06-01 22:07:45.846163 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/classes/__init__.py
+-rw-r--r--   0        0        0    14098 2023-07-06 20:59:41.959524 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/classes/auth_model.py
+-rw-r--r--   0        0        0      727 2023-07-06 21:08:54.518835 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/classes/comment_model.py
+-rw-r--r--   0        0        0    17169 2023-07-08 05:22:05.900713 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/classes/extras.py
+-rw-r--r--   0        0        0      686 2023-03-25 19:37:35.462288 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py
+-rw-r--r--   0        0        0     2986 2023-07-09 22:29:54.823123 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/classes/message_model.py
+-rw-r--r--   0        0        0     5863 2023-05-22 05:00:15.206814 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/classes/only_drm.py
+-rw-r--r--   0        0        0     3675 2023-07-09 22:31:18.494304 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/classes/post_model.py
+-rw-r--r--   0        0        0     1374 2023-07-09 22:31:37.387150 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/classes/story_model.py
+-rw-r--r--   0        0        0     1705 2023-07-08 03:21:45.085840 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/classes/subscription_model.py
+-rw-r--r--   0        0        0    28663 2023-07-10 03:53:41.051494 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/classes/user_model.py
+-rw-r--r--   0        0        0        0 2022-01-17 19:20:07.000000 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/decorators/decorators.py
+-rw-r--r--   0        0        0     6760 2023-07-11 07:31:38.247375 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/onlyfans.py
+-rw-r--r--   0        0        0     2899 2023-06-21 10:24:55.083858 ultima_scraper_api-2.0.0/ultima_scraper_api/apis/user_streamliner.py
+-rw-r--r--   0        0        0        0 2022-12-04 09:59:08.749358 ultima_scraper_api-2.0.0/ultima_scraper_api/classes/__init__.py
+-rw-r--r--   0        0        0    13187 2023-07-11 08:47:19.301278 ultima_scraper_api-2.0.0/ultima_scraper_api/classes/make_settings.py
+-rw-r--r--   0        0        0      340 2022-01-17 19:20:07.000000 ultima_scraper_api-2.0.0/ultima_scraper_api/classes/prepare_download.py
+-rw-r--r--   0        0        0    13410 2023-05-07 21:56:21.760084 ultima_scraper_api-2.0.0/ultima_scraper_api/classes/prepare_metadata.py
+-rw-r--r--   0        0        0      630 2022-01-17 19:20:07.000000 ultima_scraper_api-2.0.0/ultima_scraper_api/classes/prepare_webhooks.py
+-rw-r--r--   0        0        0     1493 2023-07-11 08:03:54.563941 ultima_scraper_api-2.0.0/ultima_scraper_api/config.py
+-rw-r--r--   0        0        0      638 2022-12-03 12:11:12.443198 ultima_scraper_api-2.0.0/ultima_scraper_api/docs/Makefile
+-rw-r--r--   0        0        0      804 2022-12-03 12:11:12.443198 ultima_scraper_api-2.0.0/ultima_scraper_api/docs/make.bat
+-rw-r--r--   0        0        0       21 2022-12-03 17:06:06.309429 ultima_scraper_api-2.0.0/ultima_scraper_api/docs/requirements.txt
+-rw-r--r--   0        0        0     1318 2022-12-03 18:16:52.399681 ultima_scraper_api-2.0.0/ultima_scraper_api/docs/source/conf.py
+-rw-r--r--   0        0        0      464 2022-12-03 17:00:27.610084 ultima_scraper_api-2.0.0/ultima_scraper_api/docs/source/index.rst
+-rw-r--r--   0        0        0        0 2022-12-04 09:51:18.483387 ultima_scraper_api-2.0.0/ultima_scraper_api/helpers/__init__.py
+-rw-r--r--   0        0        0    10870 2023-07-11 07:36:36.651955 ultima_scraper_api-2.0.0/ultima_scraper_api/helpers/main_helper.py
+-rw-r--r--   0        0        0        0 2023-01-26 05:39:16.747803 ultima_scraper_api-2.0.0/ultima_scraper_api/managers/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-22 17:41:52.794214 ultima_scraper_api-2.0.0/ultima_scraper_api/managers/job_manager/__init__.py
+-rw-r--r--   0        0        0     2318 2023-06-23 10:17:35.539928 ultima_scraper_api-2.0.0/ultima_scraper_api/managers/job_manager/job_manager.py
+-rw-r--r--   0        0        0        0 2023-01-22 17:42:18.641239 ultima_scraper_api-2.0.0/ultima_scraper_api/managers/job_manager/jobs/__init__.py
+-rw-r--r--   0        0        0      781 2023-06-23 10:13:00.135609 ultima_scraper_api-2.0.0/ultima_scraper_api/managers/job_manager/jobs/custom_job.py
+-rw-r--r--   0        0        0     2977 2023-07-08 03:26:53.352487 ultima_scraper_api-2.0.0/ultima_scraper_api/managers/scrape_manager.py
+-rw-r--r--   0        0        0    18493 2023-07-11 09:31:06.300816 ultima_scraper_api-2.0.0/ultima_scraper_api/managers/session_manager.py
+-rw-r--r--   0        0        0        0 2023-05-09 14:42:23.613712 ultima_scraper_api-2.0.0/ultima_scraper_api/models/__init__.py
+-rw-r--r--   0        0        0      677 2023-05-11 21:44:11.005112 ultima_scraper_api-2.0.0/ultima_scraper_api/models/subscription_model.py
+-rw-r--r--   0        0        0        0 2022-12-04 16:42:28.821209 ultima_scraper_api-2.0.0/ultima_scraper_api/py.typed
+-rw-r--r--   0        0        0     1094 1970-01-01 00:00:00.000000 ultima_scraper_api-2.0.0/PKG-INFO
```

### Comparing `ultima_scraper_api-1.1.4/pyproject.toml` & `ultima_scraper_api-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ultima-scraper-api"
-version = "1.1.4"
+version = "2.0.0"
 description = ""
 authors = [
     "DIGITALCRIMINALS <89371864+digitalcriminals@users.noreply.github.com>",
 ]
 packages = [{include = "ultima_scraper_api"}]
 include = ["ultima_scraper_api/py.typed"]
```

### Comparing `ultima_scraper_api-1.1.4/ultima_scraper_api/__init__.py` & `ultima_scraper_api-2.0.0/ultima_scraper_api/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import ultima_scraper_api.apis.fansly.classes as fansly_classes
 import ultima_scraper_api.apis.onlyfans.classes as onlyfans_classes
 from ultima_scraper_api.apis.fansly.classes.extras import FanslyAuthenticator
 from ultima_scraper_api.apis.fansly.fansly import FanslyAPI
 from ultima_scraper_api.apis.onlyfans.classes.extras import OnlyFansAuthenticator
 from ultima_scraper_api.apis.onlyfans.onlyfans import OnlyFansAPI
-from ultima_scraper_api.classes.make_settings import Config
 
 api_types = OnlyFansAPI | FanslyAPI
 authenticator_types = OnlyFansAuthenticator | FanslyAuthenticator
 auth_types = onlyfans_classes.auth_model.AuthModel | fansly_classes.auth_model.AuthModel
 user_types = (
     onlyfans_classes.user_model.create_user | fansly_classes.user_model.create_user
 )
@@ -27,17 +26,18 @@
 subscription_types = (
     onlyfans_classes.subscription_model.SubscriptionModel
     | fansly_classes.subscription_model.SubscriptionModel
 )
 
 content_types = story_types | post_types | message_types
 error_types = onlyfans_classes.extras.ErrorDetails | fansly_classes.extras.ErrorDetails
+from ultima_scraper_api.config import UltimaScraperAPIConfig
 
 
-def select_api(option: str, config: Config = Config()):
+def select_api(option: str, config: UltimaScraperAPIConfig = UltimaScraperAPIConfig()):
     """Allows you to select an API
 
     Args:
         option (str): API name (e.g., onlyfans)
         config (Config, optional): Defaults to Config().
 
     Returns:
```

### Comparing `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/api_helper.py` & `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/api_helper.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/api_streamliner.py` & `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/api_streamliner.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any
 
 import ultima_scraper_api
 from ultima_scraper_api.apis import api_helper
-from ultima_scraper_api.classes.make_settings import Config
-
+from ultima_scraper_api.config import UltimaScraperAPIConfig
 
 if TYPE_CHECKING:
     api_types = ultima_scraper_api.api_types
     auth_types = ultima_scraper_api.auth_types
 
 
 class Packages:
@@ -24,58 +23,53 @@
                 )
 
                 self.CreateAuth = AuthModel
             case "fansly":
                 from ultima_scraper_api.apis.fansly.classes.extras import AuthDetails
 
                 self.AuthDetails = AuthDetails
-                from ultima_scraper_api.apis.fansly.classes.auth_model import (
-                    AuthModel,
-                )
+                from ultima_scraper_api.apis.fansly.classes.auth_model import AuthModel
 
                 self.CreateAuth = AuthModel
             case _:
                 raise ValueError("Site Doesn't Exist")
 
 
 class StreamlinedAPI:
     def __init__(
         self,
         api: api_types,
-        config: Config,
+        config: UltimaScraperAPIConfig,
     ) -> None:
         from ultima_scraper_api.managers.job_manager.job_manager import JobManager
 
         self.api = api
-        self.max_threads = config.settings.max_threads
         self.config = config
         self.lists = None
         self.pool = api_helper.CustomPool()
 
         self.job_manager = JobManager()
         self.packages = Packages(self.api.site_name)
 
-
-
     def add_auth(
-        self, authenticator:ultima_scraper_api.authenticator_types, only_active: bool = False
+        self,
+        authenticator: ultima_scraper_api.authenticator_types,
+        only_active: bool = False,
     ) -> auth_types:
         """Creates and appends an auth object to auths property
 
         Args:
             auth_json (dict[str, str], optional): []. Defaults to {}.
             only_active (bool, optional): [description]. Defaults to False.
 
         Returns:
             create_auth: [Auth object]
         """
         packages = self.packages
-        auth = packages.CreateAuth(
-            authenticator   # type: ignore
-        )
+        auth = packages.CreateAuth(authenticator)  # type: ignore
         if only_active and not auth.authenticator.auth_details.active:
             return auth
         auth.extras["settings"] = self.config
         self.api.auths.append(auth)  # type: ignore
         return auth
 
     def has_active_auths(self):
@@ -83,15 +77,27 @@
 
     def get_auths_via_subscription_identifier(self, identifier: str):
         for auth in self.api.auths:
             if auth.username == identifier:
                 pass
 
     def get_site_settings(self):
-        return self.config.supported.get_settings(self.api.site_name)
+        return self.config.site_apis.get_settings(self.api.site_name)
 
     def get_global_settings(self):
         return self.config.settings
 
     async def close_pools(self):
         for auth in self.api.auths:
             await auth.session_manager.active_session.close()
+
+    class CategorizedContent:
+        def __init__(self) -> None:
+            self.Stories: dict[int, Any] = {}
+            self.Posts: dict[int, Any] = {}
+            self.Chats: dict[int, Any] = {}
+            self.Messages: dict[int, Any] = {}
+            self.Highlights: dict[int, Any] = {}
+            self.MassMessages: dict[int, Any] = {}
+
+        def find_content(self, content_id: int, content_type: str):
+            return getattr(self, content_type)[content_id]
```

### Comparing `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/auth_streamliner.py` & `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/auth_streamliner.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/__init__.py` & `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Literal
 from urllib.parse import urlparse
 
 if TYPE_CHECKING:
     from ultima_scraper_api.apis.fansly.classes.user_model import (
-        AuthModel,
         create_user,
     )
 
 SubscriptionType = Literal["all", "active", "expired"]
 
 
 class SiteContent:
-    def __init__(self, option: dict[str, Any], user: AuthModel | create_user) -> None:
+    def __init__(self, option: dict[str, Any], user: create_user) -> None:
         self.id: int = int(option["id"])
         self.author = user
         self.media: list[dict[str, Any]] = option.get("media", [])
         self.preview_ids: list[int] = []
+        self.__raw__ = option
 
     def url_picker(self, media_item: dict[str, Any], video_quality: str = ""):
         # There are two media results at play here.
         # The top-level `media` element itself represents the original source quality.
         # It may also contain a `variants` list entry with alternate encoding qualities.
         # Each variant has a similar structure to the main media element.
         video_quality = (
```

### Comparing `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/classes/auth_model.py` & `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/classes/auth_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import asyncio
 from datetime import datetime
 from itertools import product
 from typing import TYPE_CHECKING, Any, Dict
 
 from dateutil.relativedelta import relativedelta
-
 from ultima_scraper_api.apis import api_helper
 from ultima_scraper_api.apis.auth_streamliner import StreamlinedAuth
 from ultima_scraper_api.apis.fansly import SubscriptionType
 from ultima_scraper_api.apis.fansly.classes.extras import endpoint_links
 from ultima_scraper_api.apis.fansly.classes.message_model import create_message
 from ultima_scraper_api.apis.fansly.classes.post_model import create_post
 from ultima_scraper_api.apis.fansly.classes.subscription_model import SubscriptionModel
@@ -107,14 +106,16 @@
     async def match_identifiers(self, identifiers: list[int | str]):
         if self.id in identifiers or self.username in identifiers:
             return True
         else:
             return False
 
     def find_user_by_identifier(self, identifier: int | str):
+        if isinstance(identifier,str) and identifier.isnumeric():
+            identifier = int(identifier)
         user = [x for x in self.users if x.id == identifier or x.username == identifier]
         if user:
             user = user[0]
             return user
 
     async def get_user(self, identifier: int | str):
         valid_user = self.find_user_by_identifier(identifier)
@@ -124,19 +125,27 @@
             identifier = str(identifier)
             if identifier.isdigit():
                 url = endpoint_links(identifier).users_by_id
             else:
                 url = endpoint_links(identifier).users_by_username
                 pass
             response = await self.session_manager.json_request(url)
-            if "error" not in response:
+            if response["response"]:
                 response["session_manager"] = self.session_manager
                 response = create_user(response["response"][0], self)
             return response
 
+    async def resolve_user(self, data: dict[str, Any]):
+        valid_user = self.find_user_by_identifier(data["id"])
+        if valid_user:
+            return valid_user
+        else:
+            response = create_user(data, self)
+            return response
+
     async def get_lists_users(
         self,
         identifier: int | str,
         check: bool = False,
         limit: int = 100,
         offset: int = 0,
     ):
@@ -150,15 +159,17 @@
         if len(results) >= limit and not check:
             results2 = await self.get_lists_users(
                 identifier, limit=limit, offset=limit + offset
             )
             results.extend(results2)  # type: ignore
         return results
 
-    async def get_followings(self, identifiers: list[int | str]) -> list[create_user]:
+    async def get_followings(
+        self, identifiers: list[int | str] = []
+    ) -> list[create_user]:
         offset_count = 0
         followings: list[dict[str, Any]] = []
         while True:
             followings_link = endpoint_links().list_followings(self.id, offset_count)
             temp_followings: dict[str, Any] = await self.session_manager.json_request(
                 followings_link
             )
@@ -186,14 +197,15 @@
                 ]
             for following in final_followings:
                 if not following.subscribedByData:
                     new_date = datetime.now() + relativedelta(years=10)
                     new_date = int(new_date.timestamp() * 1000)
                     following.subscribedByData = {}
                     following.subscribedByData["endsAt"] = new_date
+        self.followed_users = final_followings
         return final_followings
 
     async def get_subscription(
         self, identifier: int | str = "", custom_list: list[SubscriptionModel] = []
     ) -> SubscriptionModel | None:
         subscriptions = (
             await self.get_subscriptions(refresh=False)
@@ -312,12 +324,24 @@
                             last_message, result["withUser"]
                         )
             final_results = final_results["data"]
             final_results.sort(key=lambda x: x["withUser"].id, reverse=True)
         self.chats = final_results
         return final_results
 
+    async def get_paid_content(
+        self,
+        limit: int = 10,
+        offset: int = 0,
+    ):
+        if not self.cache.paid_content.is_released():
+            return self.paid_content
+        link = endpoint_links(global_limit=limit, global_offset=offset).paid_api
+        result = await self.session_manager.json_request(link)
+        final_results = result["response"]["accountMediaOrders"]
+        return final_results
+
     async def get_scrapable_users(self):
         followed_users = self.followed_users
         subscription_users = [x.user for x in self.subscriptions]
         unique_users = list(set(followed_users) | set(subscription_users))
         return unique_users
```

### Comparing `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/classes/collection_model.py` & `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/classes/collection_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+from datetime import datetime
 from typing import TYPE_CHECKING, Any
 
 from ultima_scraper_api.apis.fansly import SiteContent
 from ultima_scraper_api.apis.fansly.classes.extras import endpoint_links
 
 if TYPE_CHECKING:
     from ultima_scraper_api.apis.fansly.classes.user_model import create_user
@@ -12,17 +13,14 @@
 class create_collection(SiteContent):
     def __init__(
         self, option: dict[str, Any], user: create_user, extra: dict[str, Any]
     ) -> None:
         SiteContent.__init__(self, option, user)
         self.responseType: str = option.get("responseType")
         self.id: int = int(option["id"])
-        self.createdAt: str = int(option.get("createdAt",0)/1000)
-        self.postedAtPrecise: str = option.get("postedAtPrecise")
-        self.expiredAt: Any = option.get("expiredAt")
         self.author = user
         text: str = option.get("text", "")
         self.text = str(text or "")
         raw_text: str = option.get("rawText", "")
         self.rawText = str(raw_text or "")
         self.lockedText: bool = option.get("lockedText")
         self.isFavorite: bool = option.get("isFavorite")
@@ -47,14 +45,17 @@
         self.hasUrl: bool = option.get("hasUrl")
         self.commentsCount: int = option.get("commentsCount")
         self.mentionedUsers: list = option.get("mentionedUsers")
         self.linkedUsers: list = option.get("linkedUsers")
         self.linkedPosts: list = option.get("linkedPosts")
         self.previews: list[dict[str, Any]] = option.get("previews", [])
         self.attachments: list[dict[str, Any]] = extra.get("albumContent", {})
+        self.created_at: datetime = datetime.fromtimestamp(option["createdAt"] / 1000)
+        self.postedAtPrecise: str = option.get("postedAtPrecise")
+        self.expiredAt: Any = option.get("expiredAt")
         # Custom
         final_media_ids: list[Any] = []
         for attachment in self.attachments:
             attachment_content_id = attachment["mediaOfferId"]
             match attachment["mediaOfferType"]:
                 case 1:
                     final_media_ids.append(attachment_content_id)
```

### Comparing `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/classes/extras.py` & `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/classes/extras.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import copy
 import math
 from itertools import chain
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Literal, Optional, Union
-
-from user_agent import generate_user_agent
+from urllib.parse import parse_qs, urlparse
 
 from ultima_scraper_api.managers.session_manager import SessionManager
+from user_agent import generate_user_agent
 
 if TYPE_CHECKING:
-    from ultima_scraper_api.apis.fansly.fansly import FanslyAPI
+    from ultima_scraper_api.apis.onlyfans.onlyfans import OnlyFansAPI
 
 from ultima_scraper_api.apis import api_helper
 
 
 class ErrorDetails:
     def __init__(self, result: dict[str, Any]) -> None:
         error = result["error"] if "error" in result else result
@@ -35,73 +35,95 @@
 
 
 class CookieParser:
     def __init__(self, options: str) -> None:
         new_dict: dict[str, Any] = {}
         for crumble in options.strip().split(";"):
             if crumble:
-                key, value = crumble.strip().split("=")
-                new_dict[key] = value
+                split_value = crumble.strip().split("=", 1)
+                if len(split_value) >= 2:
+                    key, value = split_value
+                    new_dict[key] = value
         self.auth_id = new_dict.get("auth_id", "")
         self.sess = new_dict.get("sess", "")
         self.auth_hash = new_dict.get("auth_hash", "")
         self.auth_uniq_ = new_dict.get("auth_uniq_", "")
         self.auth_uid_ = new_dict.get("auth_uid_", "")
+        self.aws_waf_token = new_dict.get("aws-waf-token", "")
 
     def format(self):
         """
         Typically used for adding cookies to requests
         """
-        return self.__dict__
+        final_dict = self.__dict__.copy()
+        final_dict["aws-waf-token"] = final_dict["aws_waf_token"]
+        final_dict.pop("aws_waf_token")
+        return final_dict
 
     def convert(self):
         new_dict = ""
         for key, value in self.__dict__.items():
             key = key.replace("auth_uniq_", f"auth_uniq_{self.auth_id}")
             key = key.replace("auth_uid_", f"auth_uid_{self.auth_id}")
+            key = key.replace("aws_waf_token", f"aws-waf-token")
             new_dict += f"{key}={value}; "
         new_dict = new_dict.strip()
         return new_dict
 
 
 class AuthDetails:
     def __init__(
         self,
         id: int | None = None,
         username: str = "",
-        authorization: str = "",
+        cookie: str = "",
+        x_bc: str = "",
         user_agent: str = "",
         email: str = "",
         password: str = "",
         hashed: bool = False,
         support_2fa: bool = True,
         active: bool | None = None,
     ) -> None:
         self.id = id
         self.username = username
-        self.authorization = authorization
+        self.cookie = CookieParser(cookie)
+        self.x_bc = x_bc
         self.user_agent = user_agent
         self.email = email
         self.password = password
         self.hashed = hashed
         self.support_2fa = support_2fa
         self.active = active
 
     def upgrade_legacy(self, options: dict[str, Any]):
+        if "cookie" not in options:
+            self = legacy_auth_details(options).upgrade(self)
         return self
 
-    def export(self):
+    def export(self, model: Any = None):
         new_dict = copy.copy(self.__dict__)
+        cookie = self.cookie.convert()
+        results = [
+            x for x in cookie.replace(" ", "").split(";") if x and x.split("=")[1]
+        ]
+        new_dict["cookie"] = cookie if results else ""
+        if model:
+            for att in new_dict.copy():
+                if att not in model.__annotations__:
+                    del new_dict[att]
+            new_dict["user_id"] = new_dict["id"]
+            del new_dict["id"]
         return new_dict
 
 
-class FanslyAuthenticator:
+class OnlyFansAuthenticator:
     def __init__(
         self,
-        api: "FanslyAPI",
+        api: "OnlyFansAPI",
         auth_details: AuthDetails = AuthDetails(),
         max_threads: int = -1,
     ) -> None:
         self.api = api
         self.auth_details = auth_details
         self.session_manager = SessionManager(self, max_threads=max_threads)
         self.auth_attempt = 0
@@ -112,29 +134,60 @@
         self.__raw__: dict[str, Any] | None = None
 
     async def login(self, guest: bool = False):
         auth_items = self.auth_details
         if not auth_items:
             return self
         if guest and auth_items:
+            auth_items.cookie.auth_id = "0"
             auth_items.user_agent = generate_user_agent()
         link = endpoint_links().customer
         user_agent = auth_items.user_agent
+        auth_id = str(auth_items.cookie.auth_id)
+        # expected string error is fixed by auth_id
         dynamic_rules = self.session_manager.dynamic_rules
-        a: list[Any] = [dynamic_rules, user_agent, link]
+        a: list[Any] = [dynamic_rules, auth_id, auth_items.x_bc, user_agent, link]
         self.session_manager.headers = create_headers(*a)
         if guest:
             self.guest = True
             self.__raw__ = {}
             return self
 
         while self.auth_attempt < self.max_attempts:
             await self.process_auth()
             self.auth_attempt += 1
 
+            async def resolve_auth(auth: OnlyFansAuthenticator):
+                if self.errors:
+                    error = self.errors[-1]
+                    if error.code == 101:
+                        if auth_items.support_2fa:
+                            link = f"https://onlyfans.com/api2/v2/users/otp/check"
+                            count = 1
+                            max_count = 3
+                            while count < max_count + 1:
+                                print(
+                                    "2FA Attempt " + str(count) + "/" + str(max_count)
+                                )
+                                code = input("Enter 2FA Code\n")
+                                data = {"code": code, "rememberMe": True}
+                                response = await self.session_manager.json_request(
+                                    link, method="POST", payload=data
+                                )
+                                if isinstance(response, ErrorDetails):
+                                    error.message = response.message
+                                    count += 1
+                                else:
+                                    print("Success")
+                                    auth.active = False
+                                    auth.errors.remove(error)
+                                    await self.process_auth()
+                                    break
+
+            await resolve_auth(self)
             if not self.is_authed():
                 if self.errors:
                     error = self.errors[-1]
                     error_message = error.message
                     if "token" in error_message:
                         break
                     if "Code wrong" in error_message:
@@ -144,27 +197,26 @@
                 continue
             else:
                 break
         return self
 
     async def process_auth(self):
         if not self.maxed_out_auth_attempts():
-            link = endpoint_links().me
+            link = endpoint_links().customer
             json_resp = await self.session_manager.json_request(link)
             await self.resolve_auth_errors(json_resp)
             if not self.errors:
                 self.auth_details.active = True
                 self.__raw__ = json_resp
             else:
-                if self.auth_details.id:
-                    link = endpoint_links(self.auth_details.id).users_by_id
-                    json_resp = await self.session_manager.json_request(link)
-                    await self.resolve_auth_errors(json_resp)
-                    self.__raw__ = json_resp
+                link = endpoint_links(self.auth_details.cookie.auth_id).users
+                json_resp = await self.session_manager.json_request(link)
+                await self.resolve_auth_errors(json_resp)
                 self.auth_details.active = False
+                self.__raw__ = json_resp
         return self
 
     def maxed_out_auth_attempts(self):
         return True if self.auth_attempt >= self.max_attempts else False
 
     def is_authed(self):
         return self.auth_details.active
@@ -217,146 +269,129 @@
         new_dict = ""
         for key, value in self.__dict__.items():
             value = value if value != None else ""
             skippable = ["username", "user_agent"]
             if key not in skippable:
                 new_dict += f"{key}={value}; "
         new_dict = new_dict.strip()
+        new_auth_details.cookie = CookieParser(new_dict)
         return new_auth_details
 
 
 class endpoint_links(object):
     def __init__(
         self,
-        identifier: Optional[str | int] = None,
-        identifier2: Optional[str | int] = None,
-        identifier3: Optional[str | int] = None,
+        identifier: Optional[int | str] = None,
+        identifier2: Optional[int | str] = None,
+        identifier3: Optional[int | str] = None,
         text: str = "",
         global_limit: int = 10,
         global_offset: int = 0,
         sort_order: Literal["asc", "desc"] = "desc",
-        before_id: str = "",
     ):
-        domain = "https://apiv3.fansly.com"
-        api = "/api/v1"
+        domain = "https://onlyfans.com"
+        api = "/api2/v2"
         full_url_path = f"{domain}{api}"
         self.full_url_path = full_url_path
-        self.me = f"{full_url_path}/account/me"
-        self.customer = f"{full_url_path}/account?ids={identifier}"
-        self.settings = f"{full_url_path}/account/settings"
-        self.users_by_id = f"{self.full_url_path}/account?ids={identifier}"
-        self.users_by_username = f"{self.full_url_path}/account?usernames={identifier}"
-        self.followings = f"{full_url_path}/account/{identifier}/following?before={global_offset}&after=0&limit=100&offset=0"
-        self.subscriptions = f"{full_url_path}/subscriptions"
-        self.lists = f"https://onlyfans.com/api2/v2/lists?limit={global_limit}&offset={global_offset}"
+        self.login_issues = f"{full_url_path}/issues/login"
+        self.customer = f"https://onlyfans.com/api2/v2/users/me"
+        self.users = f"https://onlyfans.com/api2/v2/users/{identifier}"
+        self.subscriptions = f"{full_url_path}/subscriptions/subscribes?limit={global_limit}&offset={global_offset}&type={identifier}"
+        self.lists = f"https://onlyfans.com/api2/v2/lists?limit=100&offset=0"
         self.lists_users = f"https://onlyfans.com/api2/v2/lists/{identifier}/users?limit={global_limit}&offset={global_offset}&query="
-        self.list_chats = f"{full_url_path}/messaging/groups?sortOrder=1&flags=0&subscriptionTierId=&search=&limit={global_limit}&offset={global_offset}"
+        self.list_chats = f"https://onlyfans.com/api2/v2/chats?limit={global_limit}&offset={global_offset}&order=desc"
         self.post_by_id = f"https://onlyfans.com/api2/v2/posts/{identifier}"
         self.message_by_id = f"https://onlyfans.com/api2/v2/chats/{identifier}/messages?limit=10&offset=0&firstId={identifier2}&order=desc&skip_users=all&skip_users_dups=1"
         self.search_chat = f"https://onlyfans.com/api2/v2/chats/{identifier}/messages/search?query={text}"
-        self.groups_api = f"{full_url_path}/group"
-        self.message_api = f"{full_url_path}/message?groupId={identifier}&limit={global_limit}&before={before_id}&order=desc"
+        self.message_api = f"https://onlyfans.com/api2/v2/chats/{identifier}/messages?limit={global_limit}&id={global_offset}"
         self.search_messages = f"https://onlyfans.com/api2/v2/chats/{identifier}?limit=10&offset=0&filter=&order=activity&query={text}"
         self.mass_messages_api = f"https://onlyfans.com/api2/v2/messages/queue/stats?limit=100&offset=0&format=infinite"
-        self.stories_api = (
-            f"{full_url_path}/mediastoriesnew?accountId={identifier}&ngsw-bypass=true"
-        )
+        self.stories_api = f"https://onlyfans.com/api2/v2/users/{identifier}/stories?limit=100&offset=0&order=desc"
         self.list_highlights = f"https://onlyfans.com/api2/v2/users/{identifier}/stories/highlights?limit=100&offset=0&order=desc"
         self.highlight = f"https://onlyfans.com/api2/v2/stories/highlights/{identifier}"
         self.list_posts_api = self.list_posts(identifier)
-        self.post_api = f"{full_url_path}/timeline/{identifier}?before={global_offset}"
-        self.collections_api = (
-            f"{full_url_path}/uservault/albums?accountId={identifier}"
-        )
-        self.collection_api = f"{full_url_path}/uservault/album/content?albumId={identifier}&before={global_offset}&after=0&limit={global_limit}"
         self.archived_posts = f"https://onlyfans.com/api2/v2/users/{identifier}/posts/archived?limit={global_limit}&offset={global_offset}&order=publish_date_desc"
         self.archived_stories = f"https://onlyfans.com/api2/v2/stories/archive/?limit=100&offset=0&order=publish_date_desc"
-        self.paid_api = f"https://onlyfans.com/api2/v2/posts/paid?{global_limit}&offset={global_offset}"
+        self.paid_api = f"https://onlyfans.com/api2/v2/posts/paid?limit={global_limit}&offset={global_offset}"
         self.pay = f"https://onlyfans.com/api2/v2/payments/pay"
         self.subscribe = f"https://onlyfans.com/api2/v2/users/{identifier}/subscribe"
         self.like = f"https://onlyfans.com/api2/v2/{identifier}/{identifier2}/like"
         self.favorite = f"https://onlyfans.com/api2/v2/{identifier}/{identifier2}/favorites/{identifier3}"
         self.transactions = (
             f"https://onlyfans.com/api2/v2/payments/all/transactions?limit=10&offset=0"
         )
-        self.two_factor = f"https://onlyfans.com/api2/v2/users/otp/check"
-
-    def list_followings(self, identifier: int, offset: int = 0):
-        return f"{self.full_url_path}/account/{identifier}/following?before=0&after=0&limit=100&offset={offset}"
-
-    def list_users(self, identifiers: list[int | str] | list[int] | list[str]):
-        identifier_type = "ids"
-        if all(isinstance(x, str) and x.isalpha() for x in identifiers):
-            identifier_type = "usernames"
-        link = ""
-        if identifiers:
-            link = f"{self.full_url_path}/account?{identifier_type}={','.join([str(x) for x in identifiers])}"
-        return link
+        self.list_comments_api = f"{full_url_path}/{identifier}/{identifier2}/comments?limit={global_limit}&offset={global_offset}&sort={sort_order}"
+        self.subscription_count = f"{full_url_path}/subscriptions/count/all"
+        self.socials = f"{full_url_path}/users/{identifier}/social/buttons"
+        self.spotify = f"{full_url_path}/users/{identifier}/social/spotify"
+        self.two_factor = f"{full_url_path}/users/otp/check"
+        self.drm_server = f"{full_url_path}/users/media/{identifier}/drm/{identifier2}/{identifier3}?type=widevine"
 
     def list_posts(
         self,
         content_id: Optional[int | str],
         global_limit: int = 10,
         global_offset: int = 0,
     ):
-        return f"{self.full_url_path}/timeline/{content_id}?before={global_offset}"
+        return f"{self.full_url_path}/users/{content_id}/posts?limit={global_limit}&offset={global_offset}&order=publish_date_desc&skip_users_dups=0"
 
     def list_comments(
         self,
         content_type: str,
         content_id: Optional[int | str],
         global_limit: int = 10,
         global_offset: int = 0,
         sort_order: Literal["asc", "desc"] = "desc",
     ):
         content_type = f"{content_type}s" if content_type[0] != "s" else content_type
         return f"{self.full_url_path}/{content_type}/{content_id}/comments?limit={global_limit}&offset={global_offset}&sort={sort_order}"
 
-    def create_links(self, link: str, api_count: int, limit: int = 10, offset: int = 0):
+    def create_links(self, url: str, api_count: int, limit: int = 10, offset: int = 0):
         """
         This function will create a list of links depending on their content count.
 
         Example:\n
-        create_links(link="base_link", api_count=50) will return a list with 5 links.
+        create_links(link="base_link", api_count=50) will return a list with 5 links if limit=10.
         """
         final_links: list[str] = []
         if api_count:
             ceil = math.ceil(api_count / limit)
             numbers = list(range(ceil))
             for num in numbers:
                 num = num * limit
-                link = link.replace(f"limit={limit}", f"limit={limit}")
-                new_link = link.replace(f"offset={offset}", f"offset={num}")
+                parsed_url = urlparse(url)
+                query_params = parse_qs(parsed_url.query)
+                limit_value = query_params["limit"][0]
+                url = url.replace(f"limit={limit_value}", f"limit={limit}")
+                new_link = url.replace(f"offset={offset}", f"offset={num}")
                 final_links.append(new_link)
         return final_links
 
 
 def create_headers(
     dynamic_rules: dict[str, Any],
     auth_id: Union[str, int],
+    x_bc: str,
     user_agent: str = "",
     link: str = "https://onlyfans.com/",
 ):
     headers: dict[str, Any] = {}
     headers["user-agent"] = user_agent
     headers["referer"] = link
+    headers["x-bc"] = x_bc
     headers["user-id"] = str(auth_id)
-    headers["x-bc"] = ""
     for remove_header in dynamic_rules["remove_headers"]:
         headers.pop(remove_header)
     return headers
 
 
-def handle_refresh(object_: object, name: str):
-    final_argument = getattr(object_, name)
-    return final_argument
-
-
 class media_types:
-    def __init__(self, option={}, assign_states=False) -> None:
+    def __init__(
+        self, option: dict[str, Any] = {}, assign_states: bool = False
+    ) -> None:
         self.Images = option.get("Images", [])
         self.Videos = option.get("Videos", [])
         self.Audios = option.get("Audios", [])
         self.Texts = option.get("Texts", [])
         if assign_states:
             for k, v in self:
                 setattr(self, k, assign_states())
```

### Comparing `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/classes/message_model.py` & `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/classes/message_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+from datetime import datetime
 from typing import TYPE_CHECKING, Any, Optional
 
 from ultima_scraper_api.apis.fansly import SiteContent
 from ultima_scraper_api.apis.fansly.classes.extras import endpoint_links
 
 if TYPE_CHECKING:
     from ultima_scraper_api.apis.fansly.classes.user_model import create_user
@@ -30,15 +31,15 @@
         self.fromUser = user.get_authed().find_user_by_identifier(option["senderId"])
         self.isFromQueue: Optional[bool] = option.get("isFromQueue")
         self.queueId: Optional[int] = option.get("queueId")
         self.canUnsendQueue: Optional[bool] = option.get("canUnsendQueue")
         self.unsendSecondsQueue: Optional[int] = option.get("unsendSecondsQueue")
         self.isOpened: Optional[bool] = option.get("isOpened")
         self.isNew: Optional[bool] = option.get("isNew")
-        self.createdAt: Optional[str] = option.get("createdAt")
+        self.created_at: datetime = datetime.fromtimestamp(option["createdAt"])
         self.changedAt: Optional[str] = option.get("changedAt")
         self.cancelSeconds: Optional[int] = option.get("cancelSeconds")
         self.isLiked: Optional[bool] = option.get("isLiked")
         self.canPurchase: Optional[bool] = option.get("canPurchase")
         self.canPurchaseReason: Optional[str] = option.get("canPurchaseReason")
         self.canReport: Optional[bool] = option.get("canReport")
         self.attachments: list[dict[str, Any]] = option.get("attachments", {})
```

### Comparing `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/classes/post_model.py` & `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/classes/post_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 from __future__ import annotations
 
+from datetime import datetime
 from typing import TYPE_CHECKING, Any
 
 from ultima_scraper_api.apis.fansly import SiteContent
+from ultima_scraper_api.apis.fansly.classes.comment_model import CommentModel
 from ultima_scraper_api.apis.fansly.classes.extras import endpoint_links
 
 if TYPE_CHECKING:
-    from ultima_scraper_api.apis.fansly.classes.user_model import (
-        AuthModel,
-        create_user,
-    )
+    from ultima_scraper_api.apis.fansly.classes.user_model import create_user
 
 
 class create_post(SiteContent):
     def __init__(
         self,
         option: dict[str, Any],
-        user: AuthModel | create_user,
+        user: create_user,
         extra: dict[str, Any],
     ) -> None:
         SiteContent.__init__(self, option, user)
         self.responseType: str = option.get("responseType")
-        self.createdAt: str = option.get("createdAt")
-        self.postedAtPrecise: str = option.get("postedAtPrecise")
-        self.expiredAt: Any = option.get("expiredAt")
         self.author = user
         text: str = option.get("content", "")
         self.text = str(text or "")
         raw_text: str = option.get("rawText", "")
         self.rawText = str(raw_text or "")
         self.lockedText: bool = option.get("lockedText")
         self.isFavorite: bool = option.get("isFavorite")
@@ -46,20 +42,25 @@
         self.streamId: Any = option.get("streamId")
         self.price: Any = option.get("price")
         self.hasVoting: bool = option.get("hasVoting")
         self.isAddedToBookmarks: bool = option.get("isAddedToBookmarks")
         self.isArchived: bool = option.get("isArchived")
         self.isDeleted: bool = option.get("isDeleted")
         self.hasUrl: bool = option.get("hasUrl")
-        self.commentsCount: int = option.get("commentsCount")
+        self.commentsCount: int = option.get("replyCount")
         self.mentionedUsers: list = option.get("mentionedUsers")
         self.linkedUsers: list = option.get("linkedUsers")
         self.linkedPosts: list = option.get("linkedPosts")
         self.previews: list[dict[str, Any]] = option.get("previews", [])
         self.attachments: list[dict[str, Any]] = option.get("attachments", {})
+        self.comments: list[CommentModel] = []
+        self.created_at: datetime = datetime.fromtimestamp(option["createdAt"])
+        self.postedAtPrecise: str = option.get("postedAtPrecise")
+        self.expiredAt: Any = option.get("expiredAt")
+
         # Custom
         final_media_ids: list[Any] = []
         for attachment in self.attachments:
             attachment_content_id = attachment["contentId"]
             match attachment["contentType"]:
                 case 1:
                     final_media_ids.append(attachment_content_id)
@@ -78,35 +79,44 @@
                     if account_media["id"] == final_media_id:
                         temp_media = None
                         if "preview" in account_media:
                             temp_media = account_media["preview"]
                             if not account_media["access"]:
                                 self.preview_ids.append(int(account_media["previewId"]))
                                 self.previews.append(temp_media)
-                        if (
-                            account_media["media"]["locations"]
-                        ):
+                        if account_media["media"]["locations"]:
                             temp_media = account_media["media"]
                         if temp_media:
                             final_media.append(temp_media)
         self.media: list[Any] = final_media
         self.canViewMedia: bool = option.get("canViewMedia")
         self.preview: list[int] = option.get("preview", [])
         self.canPurchase: bool = option.get("canPurchase")
 
     def get_author(self):
         return self.author
 
     async def get_comments(self):
-        epl = endpoint_links()
-        link = epl.list_comments(self.responseType, self.id)
-        links = epl.create_links(link, self.commentsCount)
-        if links:
-            results = await self.author.scrape_manager.bulk_scrape(links)
-            self.comments = results
+        if not self.commentsCount:
+            return
+        epl = endpoint_links("post", self.id)
+        link = epl.list_comments_api
+        result: list[dict[str, Any]] = await self.author.scrape_manager.scrape(link)
+        response: dict[str, Any] = result["response"]
+        authed = self.author.get_authed()
+        final_results = [
+            CommentModel(
+                x,
+                await authed.resolve_user(
+                    [y for y in response["accounts"] if y["id"] == x["accountId"]][0]
+                ),
+            )
+            for x in response["posts"]
+        ]
+        self.comments = final_results
         return self.comments
 
     async def favorite(self):
         link = endpoint_links(
             identifier=f"{self.responseType}s",
             identifier2=self.id,
             identifier3=self.author.id,
```

### Comparing `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/classes/story_model.py` & `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/classes/story_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/classes/subscription_model.py` & `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/classes/subscription_model.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 from datetime import datetime
 from typing import TYPE_CHECKING, Any
-from ultima_scraper_api.models.subscription_model import BaseSubscriptionModel
+
 from ultima_scraper_api.apis.fansly.classes.user_model import create_user
+from ultima_scraper_api.models.subscription_model import BaseSubscriptionModel
 
 if TYPE_CHECKING:
     import ultima_scraper_api
 
     auth_types = ultima_scraper_api.auth_types
     user_types = ultima_scraper_api.user_types
 
 
 class SubscriptionModel(BaseSubscriptionModel):
     def __init__(
         self, data: dict[str, Any], user: "create_user", subscriber: "auth_types"
     ) -> None:
-        self.ends_at: datetime = datetime.fromtimestamp(data["endsAt"] / 1000)
         self.price: int = data["price"]
+        self.created_at: datetime = datetime.fromtimestamp(data["createdAt"] / 1000)
+        self.ends_at: datetime = datetime.fromtimestamp(data["endsAt"] / 1000)
         self.user = user
         self.subscriber = subscriber
         self.__raw__ = data
 
+    def is_active(self):
+        return True if self.created_at > self.ends_at else False
+
     def get_authed(self):
         return self.subscriber.get_authed()
 
     def get_price(self):
         return self.price
+
+    def resolve_expires_at(self):
+        return self.ends_at
```

### Comparing `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/classes/user_model.py` & `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/classes/user_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         authed: AuthModel,
     ) -> None:
         self.avatar: Any = option.get("avatar")
         self.avatarThumbs: Any = option.get("avatarThumbs")
         self.header: Any = option.get("banner")
         self.headerSize: Any = option.get("headerSize")
         self.headerThumbs: Any = option.get("headerThumbs")
-        self.id: int = option.get("id")
+        self.id: int = int(option.get("id", 9001))
         self.name: str = option.get("name")
         self.username: str = option.get("username")
         self.canLookStory: bool = option.get("canLookStory")
         self.canCommentStory: bool = option.get("canCommentStory")
         self.hasNotViewedStory: bool = option.get("hasNotViewedStory")
         self.isVerified: bool = option.get("isVerified")
         self.canPayInternal: bool = option.get("canPayInternal")
@@ -67,28 +67,27 @@
         self.joinDate: str = option.get("joinDate")
         self.isReferrerAllowed: bool = option.get("isReferrerAllowed")
         self.about: str = option.get("about")
         self.rawAbout: str = option.get("rawAbout")
         self.website: str = option.get("website")
         self.wishlist: str = option.get("wishlist")
         self.location: str = option.get("location")
-        timeline_status = option.get("timelineStats", {})
-        self.postsCount: int = option.get("postsCount")
-        self.archivedPostsCount: int = option.get("archivedPostsCount")
-        self.photosCount: int = timeline_status.get("imageCount")
-        self.videosCount: int = timeline_status.get("videoCount")
-        self.audiosCount: int = option.get("audiosCount")
-        self.mediasCount: int = option.get("mediasCount")
+        timeline_stats = option.get("timelineStats", {})
+        self.postsCount: int = option.get("postsCount", 0)
+        self.archivedPostsCount: int = option.get("archivedPostsCount", 0)
+        self.photosCount: int = timeline_stats.get("imageCount", 0)
+        self.videosCount: int = timeline_stats.get("videoCount", 0)
+        self.audiosCount: int = option.get("audiosCount", 0)
+        self.mediasCount: int = option.get("mediasCount", 0)
         self.promotions: list = option.get("promotions")
         self.lastSeen: Any = option.get("lastSeen")
-        self.favoritesCount: int = option.get("favoritesCount")
-        self.favoritedCount: int = option.get("favoritedCount")
+        self.favoritedCount: int = option.get("accountMediaLikes")
         self.showPostsInFeed: bool = option.get("showPostsInFeed")
         self.canReceiveChatMessage: bool = option.get("canReceiveChatMessage")
-        self.isPerformer: bool = option.get("isPerformer")
+        self.isPerformer: bool = bool(self.subscriptionBundles)
         self.isRealPerformer: bool = option.get("isRealPerformer")
         self.isSpotifyConnected: bool = option.get("isSpotifyConnected")
         self.subscribersCount: int = option.get("subscribersCount")
         self.hasPinnedPosts: bool = option.get("hasPinnedPosts")
         self.canChat: bool = option.get("canChat")
         self.callPrice: int = option.get("callPrice")
         self.isPrivateRestriction: bool = option.get("isPrivateRestriction")
@@ -106,15 +105,17 @@
         self.canTrialSend: bool = option.get("canTrialSend")
         self.canAddPhone: bool = option.get("canAddPhone")
         self.phoneLast4: Any = option.get("phoneLast4")
         self.phoneMask: Any = option.get("phoneMask")
         self.hasNewTicketReplies: dict = option.get("hasNewTicketReplies")
         self.hasInternalPayments: bool = option.get("hasInternalPayments")
         self.isCreditsEnabled: bool = option.get("isCreditsEnabled")
-        self.creditBalance: float = option.get("creditBalance")
+        self.creditBalance: float = (
+            option["mainWallet"]["balance"] if "mainWallet" in option else 0
+        )
         self.isMakePayment: bool = option.get("isMakePayment")
         self.isOtpEnabled: bool = option.get("isOtpEnabled")
         self.email: str = option.get("email")
         self.isEmailChecked: bool = option.get("isEmailChecked")
         self.isLegalApprovedAllowed: bool = option.get("isLegalApprovedAllowed")
         self.isTwitterConnected: bool = option.get("isTwitterConnected")
         self.twitterUsername: Any = option.get("twitterUsername")
@@ -223,14 +224,15 @@
         self.maxPinnedPostsCount: int = option.get("maxPinnedPostsCount")
         # Custom
         authed.users.add(self)
         self.download_info: dict[str, Any] = {}
         self.duplicate_media = []
         self.scrape_manager = ScrapeManager(authed.session_manager)
         self.__raw__ = option
+        self.__db_user__: Any = None
         StreamlinedUser.__init__(self, authed)
 
     def get_username(self):
         return self.username
 
     def get_link(self):
         link = f"https://fansly.com/{self.username}"
@@ -314,14 +316,16 @@
             temp_results.append(data)
         results = api_helper.merge_dictionaries(temp_results)
         final_results = []
         if results:
             final_results = [
                 post_model.create_post(x, self, results) for x in results["posts"]
             ]
+            for result in final_results:
+                await result.get_comments()
             self.scrape_manager.scraped.Posts = final_results
         return final_results
 
     async def get_post(
         self, identifier: Optional[int | str] = None, limit: int = 10, offset: int = 0
     ) -> Union[create_post, ErrorDetails]:
         if not identifier:
@@ -347,28 +351,29 @@
         return response
 
     async def get_messages(
         self,
         links: Optional[list[str]] = None,
         limit: int = 100000,
         before: str = "",
+        cutoff_id: int | None = None,
         refresh: bool = True,
         inside_loop: bool = False,
     ):
         result, status = await api_helper.default_data(self, refresh)
         if status:
             return result
         groups = await self.get_groups()
         if isinstance(groups, ErrorDetails):
             return []
         found_id: Optional[int] = None
         for group in groups["groups"]:
             for user in group["users"]:
-                if self.id == user["userId"]:
-                    found_id = user["groupId"]
+                if self.id == int(user["userId"]):
+                    found_id = int(user["groupId"])
                     break
         final_results: list[message_model.create_message] = []
         if found_id:
             if links is None:
                 links = []
 
             link = endpoint_links(
@@ -511,21 +516,16 @@
         results = await self.session_manager.json_request(link, method="DELETE")
         return results
 
     async def subscription_price(self):
         """
         Returns subscription price. This includes the promotional price.
         """
-        subscription_price = self.subscribePrice
-        if self.promotions:
-            for promotion in self.promotions:
-                promotion_price = promotion["price"]
-                if promotion_price < subscription_price:
-                    subscription_price = promotion_price
-        return subscription_price
+        for bundle in self.subscriptionBundles:
+            return bundle["price"] / 1000
 
     async def buy_subscription(self):
         """
         This function will subscribe to a model. If the model has a promotion available, it will use it.
         """
         subscription_price = await self.subscription_price()
         x = {
```

### Comparing `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/fansly/fansly.py` & `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/onlyfans.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,45 +1,52 @@
 from pathlib import Path
 from typing import Any, Literal, Optional, Union
 
 from ultima_scraper_api.apis.api_streamliner import StreamlinedAPI
-from ultima_scraper_api.apis.fansly.classes.auth_model import AuthModel
-from ultima_scraper_api.apis.fansly.classes.extras import (
+from ultima_scraper_api.apis.onlyfans.classes.auth_model import AuthModel
+from ultima_scraper_api.apis.onlyfans.classes.extras import (
     AuthDetails,
-    FanslyAuthenticator,
+    OnlyFansAuthenticator,
     endpoint_links,
 )
-from ultima_scraper_api.apis.fansly.classes.message_model import create_message
-from ultima_scraper_api.apis.fansly.classes.post_model import create_post
-from ultima_scraper_api.apis.fansly.classes.story_model import create_story
-from ultima_scraper_api.apis.fansly.classes.user_model import create_user
-from ultima_scraper_api.classes.make_settings import Config
+from ultima_scraper_api.apis.onlyfans.classes.message_model import create_message
+from ultima_scraper_api.apis.onlyfans.classes.post_model import create_post
+from ultima_scraper_api.apis.onlyfans.classes.story_model import create_story
+from ultima_scraper_api.apis.onlyfans.classes.user_model import create_user
+from ultima_scraper_api.config import UltimaScraperAPIConfig
 
 
-class FanslyAPI(StreamlinedAPI):
-    def __init__(self, config: Config = Config()) -> None:
-        self.site_name: Literal["Fansly"] = "Fansly"
+class OnlyFansAPI(StreamlinedAPI):
+    def __init__(
+        self, config: UltimaScraperAPIConfig = UltimaScraperAPIConfig()
+    ) -> None:
+        self.site_name: Literal["OnlyFans"] = "OnlyFans"
         StreamlinedAPI.__init__(self, self, config)
         self.auths: list[AuthModel] = []
         self.users: dict[int, create_user] = {}
         self.endpoint_links = endpoint_links
 
     async def login(self, auth_json: dict[str, Any] = {}, guest: bool = False):
-        temp_auth_details = self.create_auth_details(auth_json)
-        found_auths = [x for x in self.auths if temp_auth_details.id == x.id]
+        found_auths = [x for x in self.auths if auth_json["id"] == x.id]
         if found_auths:
             authed = found_auths[0]
         else:
-            authenticator = FanslyAuthenticator(self, temp_auth_details)
+            temp_auth_details = self.create_auth_details(auth_json)
+            authenticator = OnlyFansAuthenticator(self, temp_auth_details)
             auth = await authenticator.login(guest)
-            if not auth.is_authed():
-                auth.__raw__ = {"response": {"account": {}}}
             authed = self.add_auth(auth)
+            if isinstance(authed, AuthModel):
+                if authed.is_authed():
+                    issues = await authed.get_login_issues()
+                    authed.issues = issues if issues["data"] else None
         return authed
 
+    def add_user(self, user: create_user):
+        self.users[user.id] = user
+
     def get_auth(self, identifier: Union[str, int]) -> Optional[AuthModel]:
         final_auth = None
         for auth in self.auths:
             if auth.id == identifier:
                 final_auth = auth
             elif auth.username == identifier:
                 final_auth = auth
@@ -52,15 +59,15 @@
             if not auth.is_authed():
                 await self.remove_auth(auth)
 
     async def remove_auth(self, auth: AuthModel):
         await auth.session_manager.active_session.close()
         self.auths.remove(auth)
 
-    def create_auth_details(self, auth_json: dict[str, Any] = {}) -> AuthDetails:
+    def create_auth_details(self, auth_json: dict[str, Any] = {}):
         """If you've got a auth.json file, you can load it into python and pass it through here.
 
         Args:
             auth_json (dict[str, Any], optional): [description]. Defaults to {}.
 
         Returns:
             auth_details: [auth_details object]
@@ -130,14 +137,19 @@
         def __iter__(self):
             for attr, value in self.__dict__.items():
                 yield attr, value
 
         def get_keys(self):
             return [item[0] for item in self]
 
+        async def response_type_to_key(self, value: str):
+            result = [x[0] for x in self if x[0].lower() == f"{value}s"]
+            if result:
+                return result[0]
+
         def path_to_key(self, value: Path):
             for content_type, _ in self:
                 for part in value.parts:
                     if content_type.lower() == part.lower():
                         return content_type
 
         def convert_to_key(self, value: str):
@@ -151,15 +163,15 @@
                 case _:
                     raise Exception("convert_to_key not found")
             return final_value
 
     class MediaTypes:
         def __init__(self) -> None:
             self.Images = ["photo", "image"]
-            self.Videos = ["video", "stream", "gif"]
+            self.Videos = ["video", "stream", "gif", "application"]
             self.Audios = ["audio"]
             self.Texts = ["text"]
 
         def get_keys(self):
             return [item[0] for item in self.__dict__.items()]
 
         def find_by_value(self, value: str):
```

### Comparing `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/__init__.py` & `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,22 +2,19 @@
 
 from typing import TYPE_CHECKING, Any, Literal
 from urllib.parse import urlparse
 
 SubscriptionType = Literal["all", "active", "expired", "attention"]
 
 if TYPE_CHECKING:
-    from ultima_scraper_api.apis.onlyfans.classes.user_model import (
-        AuthModel,
-        create_user,
-    )
+    from ultima_scraper_api.apis.onlyfans.classes.user_model import create_user
 
 
 class SiteContent:
-    def __init__(self, option: dict[str, Any], user: AuthModel | create_user) -> None:
+    def __init__(self, option: dict[str, Any], user: create_user) -> None:
         self.id: int = option["id"]
         self.author = user
         self.media: list[dict[str, Any]] = option.get("media", [])
         self.preview_ids: list[int] = []
         self.__raw__ = option
 
     def url_picker(self, media_item: dict[str, Any], video_quality: str = ""):
@@ -55,15 +52,15 @@
         if authed.drm:
             has_drm = authed.drm.has_drm(media_item)
             if has_drm:
                 url = has_drm
         return urlparse(url) if url else None
 
     def preview_url_picker(self, media_item: dict[str, Any]):
-        preview_url = None
+        preview_url: str | None = None
         if "files" in media_item:
             if (
                 "preview" in media_item["files"]
                 and "url" in media_item["files"]["preview"]
             ):
                 preview_url = media_item["files"]["preview"]["url"]
         else:
```

### Comparing `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/classes/auth_model.py` & `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/classes/auth_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,14 +120,22 @@
             link = endpoint_links(identifier).users
             response = await self.session_manager.json_request(link)
             if "error" not in response:
                 response["session_manager"] = self.session_manager
                 response = create_user(response, self)
             return response
 
+    async def resolve_user(self, data: dict[str, Any]):
+        valid_user = self.find_user_by_identifier(data["id"])
+        if valid_user:
+            return valid_user
+        else:
+            response = create_user(data, self)
+            return response
+
     async def get_lists_users(
         self,
         identifier: int,
         check: bool = False,
         limit: int = 100,
         offset: int = 0,
     ):
```

### Comparing `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/classes/extras.py` & `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/classes/extras.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import copy
 import math
 from itertools import chain
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Literal, Optional, Union
-from urllib.parse import parse_qs, urlparse
 
 from user_agent import generate_user_agent
 
 from ultima_scraper_api.managers.session_manager import SessionManager
 
 if TYPE_CHECKING:
-    from ultima_scraper_api.apis.onlyfans.onlyfans import OnlyFansAPI
+    from ultima_scraper_api.apis.fansly.fansly import FanslyAPI
 
 from ultima_scraper_api.apis import api_helper
 
 
 class ErrorDetails:
     def __init__(self, result: dict[str, Any]) -> None:
         error = result["error"] if "error" in result else result
@@ -36,93 +35,79 @@
 
 
 class CookieParser:
     def __init__(self, options: str) -> None:
         new_dict: dict[str, Any] = {}
         for crumble in options.strip().split(";"):
             if crumble:
-                split_value = crumble.strip().split("=", 1)
-                if len(split_value) >= 2:
-                    key, value = split_value
-                    new_dict[key] = value
+                key, value = crumble.strip().split("=")
+                new_dict[key] = value
         self.auth_id = new_dict.get("auth_id", "")
         self.sess = new_dict.get("sess", "")
         self.auth_hash = new_dict.get("auth_hash", "")
         self.auth_uniq_ = new_dict.get("auth_uniq_", "")
         self.auth_uid_ = new_dict.get("auth_uid_", "")
-        self.aws_waf_token = new_dict.get("aws-waf-token", "")
 
     def format(self):
         """
         Typically used for adding cookies to requests
         """
-        final_dict = self.__dict__.copy()
-        final_dict["aws-waf-token"] = final_dict["aws_waf_token"]
-        final_dict.pop("aws_waf_token")
-        return final_dict
+        return self.__dict__
 
     def convert(self):
         new_dict = ""
         for key, value in self.__dict__.items():
             key = key.replace("auth_uniq_", f"auth_uniq_{self.auth_id}")
             key = key.replace("auth_uid_", f"auth_uid_{self.auth_id}")
-            key = key.replace("aws_waf_token", f"aws-waf-token")
             new_dict += f"{key}={value}; "
         new_dict = new_dict.strip()
         return new_dict
 
 
 class AuthDetails:
     def __init__(
         self,
         id: int | None = None,
         username: str = "",
-        cookie: str = "",
-        x_bc: str = "",
+        authorization: str = "",
         user_agent: str = "",
         email: str = "",
         password: str = "",
         hashed: bool = False,
         support_2fa: bool = True,
         active: bool | None = None,
     ) -> None:
         self.id = id
         self.username = username
-        self.cookie = CookieParser(cookie)
-        self.x_bc = x_bc
+        self.authorization = authorization
         self.user_agent = user_agent
         self.email = email
         self.password = password
         self.hashed = hashed
         self.support_2fa = support_2fa
         self.active = active
 
     def upgrade_legacy(self, options: dict[str, Any]):
-        if "cookie" not in options:
-            self = legacy_auth_details(options).upgrade(self)
         return self
 
     def export(self, model: Any = None):
         new_dict = copy.copy(self.__dict__)
-        cookie = self.cookie.convert()
-        results = [
-            x for x in cookie.replace(" ", "").split(";") if x and x.split("=")[1]
-        ]
-        new_dict["cookie"] = cookie if results else ""
         if model:
             for att in new_dict.copy():
                 if att not in model.__annotations__:
                     del new_dict[att]
+            new_dict["user_id"] = new_dict["id"]
+            del new_dict["id"]
         return new_dict
 
 
-class OnlyFansAuthenticator:
+class FanslyAuthenticator:
     def __init__(
         self,
-        api: "OnlyFansAPI",
+        api: "FanslyAPI",
         auth_details: AuthDetails = AuthDetails(),
         max_threads: int = -1,
     ) -> None:
         self.api = api
         self.auth_details = auth_details
         self.session_manager = SessionManager(self, max_threads=max_threads)
         self.auth_attempt = 0
@@ -133,60 +118,29 @@
         self.__raw__: dict[str, Any] | None = None
 
     async def login(self, guest: bool = False):
         auth_items = self.auth_details
         if not auth_items:
             return self
         if guest and auth_items:
-            auth_items.cookie.auth_id = "0"
             auth_items.user_agent = generate_user_agent()
         link = endpoint_links().customer
         user_agent = auth_items.user_agent
-        auth_id = str(auth_items.cookie.auth_id)
-        # expected string error is fixed by auth_id
         dynamic_rules = self.session_manager.dynamic_rules
-        a: list[Any] = [dynamic_rules, auth_id, auth_items.x_bc, user_agent, link]
+        a: list[Any] = [dynamic_rules, user_agent, link]
         self.session_manager.headers = create_headers(*a)
         if guest:
             self.guest = True
             self.__raw__ = {}
             return self
 
         while self.auth_attempt < self.max_attempts:
             await self.process_auth()
             self.auth_attempt += 1
 
-            async def resolve_auth(auth: OnlyFansAuthenticator):
-                if self.errors:
-                    error = self.errors[-1]
-                    if error.code == 101:
-                        if auth_items.support_2fa:
-                            link = f"https://onlyfans.com/api2/v2/users/otp/check"
-                            count = 1
-                            max_count = 3
-                            while count < max_count + 1:
-                                print(
-                                    "2FA Attempt " + str(count) + "/" + str(max_count)
-                                )
-                                code = input("Enter 2FA Code\n")
-                                data = {"code": code, "rememberMe": True}
-                                response = await self.session_manager.json_request(
-                                    link, method="POST", payload=data
-                                )
-                                if isinstance(response, ErrorDetails):
-                                    error.message = response.message
-                                    count += 1
-                                else:
-                                    print("Success")
-                                    auth.active = False
-                                    auth.errors.remove(error)
-                                    await self.process_auth()
-                                    break
-
-            await resolve_auth(self)
             if not self.is_authed():
                 if self.errors:
                     error = self.errors[-1]
                     error_message = error.message
                     if "token" in error_message:
                         break
                     if "Code wrong" in error_message:
@@ -196,26 +150,27 @@
                 continue
             else:
                 break
         return self
 
     async def process_auth(self):
         if not self.maxed_out_auth_attempts():
-            link = endpoint_links().customer
+            link = endpoint_links().me
             json_resp = await self.session_manager.json_request(link)
             await self.resolve_auth_errors(json_resp)
             if not self.errors:
                 self.auth_details.active = True
                 self.__raw__ = json_resp
             else:
-                link = endpoint_links(self.auth_details.cookie.auth_id).users
-                json_resp = await self.session_manager.json_request(link)
-                await self.resolve_auth_errors(json_resp)
+                if self.auth_details.id:
+                    link = endpoint_links(self.auth_details.id).users_by_id
+                    json_resp = await self.session_manager.json_request(link)
+                    await self.resolve_auth_errors(json_resp)
+                    self.__raw__ = json_resp
                 self.auth_details.active = False
-                self.__raw__ = json_resp
         return self
 
     def maxed_out_auth_attempts(self):
         return True if self.auth_attempt >= self.max_attempts else False
 
     def is_authed(self):
         return self.auth_details.active
@@ -268,129 +223,136 @@
         new_dict = ""
         for key, value in self.__dict__.items():
             value = value if value != None else ""
             skippable = ["username", "user_agent"]
             if key not in skippable:
                 new_dict += f"{key}={value}; "
         new_dict = new_dict.strip()
-        new_auth_details.cookie = CookieParser(new_dict)
         return new_auth_details
 
 
 class endpoint_links(object):
     def __init__(
         self,
-        identifier: Optional[int | str] = None,
-        identifier2: Optional[int | str] = None,
-        identifier3: Optional[int | str] = None,
+        identifier: Optional[str | int] = None,
+        identifier2: Optional[str | int] = None,
+        identifier3: Optional[str | int] = None,
         text: str = "",
         global_limit: int = 10,
         global_offset: int = 0,
         sort_order: Literal["asc", "desc"] = "desc",
+        before_id: str = "",
     ):
-        domain = "https://onlyfans.com"
-        api = "/api2/v2"
+        domain = "https://apiv3.fansly.com"
+        api = "/api/v1"
         full_url_path = f"{domain}{api}"
         self.full_url_path = full_url_path
-        self.login_issues = f"{full_url_path}/issues/login"
-        self.customer = f"https://onlyfans.com/api2/v2/users/me"
-        self.users = f"https://onlyfans.com/api2/v2/users/{identifier}"
-        self.subscriptions = f"{full_url_path}/subscriptions/subscribes?limit={global_limit}&offset={global_offset}&type={identifier}"
-        self.lists = f"https://onlyfans.com/api2/v2/lists?limit=100&offset=0"
+        self.me = f"{full_url_path}/account/me"
+        self.customer = f"{full_url_path}/account?ids={identifier}"
+        self.settings = f"{full_url_path}/account/settings"
+        self.users_by_id = f"{self.full_url_path}/account?ids={identifier}"
+        self.users_by_username = f"{self.full_url_path}/account?usernames={identifier}"
+        self.followings = f"{full_url_path}/account/{identifier}/following?before={global_offset}&after=0&limit=100&offset=0"
+        self.subscriptions = f"{full_url_path}/subscriptions"
+        self.lists = f"https://onlyfans.com/api2/v2/lists?limit={global_limit}&offset={global_offset}"
         self.lists_users = f"https://onlyfans.com/api2/v2/lists/{identifier}/users?limit={global_limit}&offset={global_offset}&query="
-        self.list_chats = f"https://onlyfans.com/api2/v2/chats?limit={global_limit}&offset={global_offset}&order=desc"
+        self.list_chats = f"{full_url_path}/messaging/groups?sortOrder=1&flags=0&subscriptionTierId=&search=&limit={global_limit}&offset={global_offset}"
         self.post_by_id = f"https://onlyfans.com/api2/v2/posts/{identifier}"
         self.message_by_id = f"https://onlyfans.com/api2/v2/chats/{identifier}/messages?limit=10&offset=0&firstId={identifier2}&order=desc&skip_users=all&skip_users_dups=1"
         self.search_chat = f"https://onlyfans.com/api2/v2/chats/{identifier}/messages/search?query={text}"
-        self.message_api = f"https://onlyfans.com/api2/v2/chats/{identifier}/messages?limit={global_limit}&offset={global_offset}&order=desc"
+        self.groups_api = f"{full_url_path}/group"
+        self.message_api = f"{full_url_path}/message?groupId={identifier}&limit={global_limit}&before={before_id}&order=desc"
         self.search_messages = f"https://onlyfans.com/api2/v2/chats/{identifier}?limit=10&offset=0&filter=&order=activity&query={text}"
         self.mass_messages_api = f"https://onlyfans.com/api2/v2/messages/queue/stats?limit=100&offset=0&format=infinite"
-        self.stories_api = f"https://onlyfans.com/api2/v2/users/{identifier}/stories?limit=100&offset=0&order=desc"
+        self.stories_api = (
+            f"{full_url_path}/mediastoriesnew?accountId={identifier}&ngsw-bypass=true"
+        )
         self.list_highlights = f"https://onlyfans.com/api2/v2/users/{identifier}/stories/highlights?limit=100&offset=0&order=desc"
         self.highlight = f"https://onlyfans.com/api2/v2/stories/highlights/{identifier}"
         self.list_posts_api = self.list_posts(identifier)
+        self.post_api = f"{full_url_path}/timeline/{identifier}?before={global_offset}"
+        self.collections_api = (
+            f"{full_url_path}/uservault/albums?accountId={identifier}"
+        )
+        self.collection_api = f"{full_url_path}/uservault/album/content?albumId={identifier}&before={global_offset}&after=0&limit={global_limit}"
         self.archived_posts = f"https://onlyfans.com/api2/v2/users/{identifier}/posts/archived?limit={global_limit}&offset={global_offset}&order=publish_date_desc"
         self.archived_stories = f"https://onlyfans.com/api2/v2/stories/archive/?limit=100&offset=0&order=publish_date_desc"
-        self.paid_api = f"https://onlyfans.com/api2/v2/posts/paid?limit={global_limit}&offset={global_offset}"
+        self.paid_api = f"{full_url_path}/account/media/orders/?limit={global_limit}&offset={global_offset}"
         self.pay = f"https://onlyfans.com/api2/v2/payments/pay"
         self.subscribe = f"https://onlyfans.com/api2/v2/users/{identifier}/subscribe"
         self.like = f"https://onlyfans.com/api2/v2/{identifier}/{identifier2}/like"
         self.favorite = f"https://onlyfans.com/api2/v2/{identifier}/{identifier2}/favorites/{identifier3}"
         self.transactions = (
             f"https://onlyfans.com/api2/v2/payments/all/transactions?limit=10&offset=0"
         )
-        self.list_comments_api = f"{full_url_path}/{identifier}/{identifier2}/comments?limit={global_limit}&offset={global_offset}&sort={sort_order}"
-        self.subscription_count = f"{full_url_path}/subscriptions/count/all"
-        self.socials = f"{full_url_path}/users/{identifier}/social/buttons"
-        self.spotify = f"{full_url_path}/users/{identifier}/social/spotify"
-        self.two_factor = f"{full_url_path}/users/otp/check"
-        self.drm_server = f"{full_url_path}/users/media/{identifier}/drm/{identifier2}/{identifier3}?type=widevine"
+        self.list_comments_api = f"{full_url_path}/{identifier}/{identifier2}/replies"
+        self.two_factor = f"https://onlyfans.com/api2/v2/users/otp/check"
 
-    def list_posts(
-        self,
-        content_id: Optional[int | str],
-        global_limit: int = 10,
-        global_offset: int = 0,
-    ):
-        return f"{self.full_url_path}/users/{content_id}/posts?limit={global_limit}&offset={global_offset}&order=publish_date_desc&skip_users_dups=0"
+    def list_followings(self, identifier: int, offset: int = 0):
+        return f"{self.full_url_path}/account/{identifier}/following?before=0&after=0&limit=100&offset={offset}"
+
+    def list_users(self, identifiers: list[int | str] | list[int] | list[str]):
+        identifier_type = "ids"
+        if all(isinstance(x, str) and x.isalpha() for x in identifiers):
+            identifier_type = "usernames"
+        link = ""
+        if identifiers:
+            link = f"{self.full_url_path}/account?{identifier_type}={','.join([str(x) for x in identifiers])}"
+        return link
 
-    def list_comments(
+    def list_posts(
         self,
-        content_type: str,
         content_id: Optional[int | str],
         global_limit: int = 10,
         global_offset: int = 0,
-        sort_order: Literal["asc", "desc"] = "desc",
     ):
-        content_type = f"{content_type}s" if content_type[0] != "s" else content_type
-        return f"{self.full_url_path}/{content_type}/{content_id}/comments?limit={global_limit}&offset={global_offset}&sort={sort_order}"
+        return f"{self.full_url_path}/timeline/{content_id}?before={global_offset}"
 
-    def create_links(self, url: str, api_count: int, limit: int = 10, offset: int = 0):
+    def create_links(self, link: str, api_count: int, limit: int = 10, offset: int = 0):
         """
         This function will create a list of links depending on their content count.
 
         Example:\n
-        create_links(link="base_link", api_count=50) will return a list with 5 links if limit=10.
+        create_links(link="base_link", api_count=50) will return a list with 5 links.
         """
         final_links: list[str] = []
         if api_count:
             ceil = math.ceil(api_count / limit)
             numbers = list(range(ceil))
             for num in numbers:
                 num = num * limit
-                parsed_url = urlparse(url)
-                query_params = parse_qs(parsed_url.query)
-                limit_value = query_params["limit"][0]
-                url = url.replace(f"limit={limit_value}", f"limit={limit}")
-                new_link = url.replace(f"offset={offset}", f"offset={num}")
+                link = link.replace(f"limit={limit}", f"limit={limit}")
+                new_link = link.replace(f"offset={offset}", f"offset={num}")
                 final_links.append(new_link)
         return final_links
 
 
 def create_headers(
     dynamic_rules: dict[str, Any],
     auth_id: Union[str, int],
-    x_bc: str,
     user_agent: str = "",
     link: str = "https://onlyfans.com/",
 ):
     headers: dict[str, Any] = {}
     headers["user-agent"] = user_agent
     headers["referer"] = link
-    headers["x-bc"] = x_bc
     headers["user-id"] = str(auth_id)
+    headers["x-bc"] = ""
     for remove_header in dynamic_rules["remove_headers"]:
         headers.pop(remove_header)
     return headers
 
 
+def handle_refresh(object_: object, name: str):
+    final_argument = getattr(object_, name)
+    return final_argument
+
+
 class media_types:
-    def __init__(
-        self, option: dict[str, Any] = {}, assign_states: bool = False
-    ) -> None:
+    def __init__(self, option={}, assign_states=False) -> None:
         self.Images = option.get("Images", [])
         self.Videos = option.get("Videos", [])
         self.Audios = option.get("Audios", [])
         self.Texts = option.get("Texts", [])
         if assign_states:
             for k, v in self:
                 setattr(self, k, assign_states())
```

### Comparing `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py` & `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/classes/hightlight_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/classes/message_model.py` & `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/classes/message_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Optional
 
 from ultima_scraper_api.apis.onlyfans import SiteContent
 from ultima_scraper_api.apis.onlyfans.classes.extras import endpoint_links
+from datetime import datetime
 
 if TYPE_CHECKING:
     from ultima_scraper_api.apis.onlyfans.classes.user_model import create_user
 
 
 class create_message(SiteContent):
     def __init__(self, option: dict[str, Any], user: create_user) -> None:
@@ -27,21 +28,21 @@
         self.isReportedByMe: Optional[bool] = option.get("isReportedByMe")
         self.isFromQueue: Optional[bool] = option.get("isFromQueue")
         self.queueId: Optional[int] = option.get("queueId")
         self.canUnsendQueue: Optional[bool] = option.get("canUnsendQueue")
         self.unsendSecondsQueue: Optional[int] = option.get("unsendSecondsQueue")
         self.isOpened: Optional[bool] = option.get("isOpened")
         self.isNew: Optional[bool] = option.get("isNew")
-        self.createdAt: Optional[str] = option.get("createdAt")
-        self.changedAt: Optional[str] = option.get("changedAt")
         self.cancelSeconds: Optional[int] = option.get("cancelSeconds")
         self.isLiked: Optional[bool] = option.get("isLiked")
         self.canPurchase: Optional[bool] = option.get("canPurchase")
         self.canPurchaseReason: Optional[str] = option.get("canPurchaseReason")
         self.canReport: Optional[bool] = option.get("canReport")
+        self.created_at: datetime = datetime.fromisoformat(option["createdAt"])
+        self.changedAt: Optional[str] = option.get("changedAt")
 
     def get_author(self):
         return self.author
 
     def get_receiver(self):
         receiver = (
             self.author.get_authed() if self.author.id == self.user.id else self.user
```

### Comparing `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/classes/only_drm.py` & `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/classes/only_drm.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/classes/post_model.py` & `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/classes/post_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 from __future__ import annotations
 
+from datetime import datetime
 from typing import TYPE_CHECKING, Any
 
 from ultima_scraper_api.apis.onlyfans import SiteContent
+from ultima_scraper_api.apis.onlyfans.classes.comment_model import CommentModel
 from ultima_scraper_api.apis.onlyfans.classes.extras import endpoint_links
 
 if TYPE_CHECKING:
-    from ultima_scraper_api.apis.onlyfans.classes.user_model import (
-        AuthModel,
-        create_user,
-    )
+    from ultima_scraper_api.apis.onlyfans.classes.user_model import create_user
 
 
 class create_post(SiteContent):
-    def __init__(self, option: dict[str, Any], user: AuthModel | create_user) -> None:
+    def __init__(self, option: dict[str, Any], user: create_user) -> None:
         SiteContent.__init__(self, option, user)
         self.responseType: str = option.get("responseType")
-        self.createdAt: str = option.get("postedAt")
-        self.postedAtPrecise: str = option.get("postedAtPrecise")
-        self.expiredAt: Any = option.get("expiredAt")
         text: str = option.get("text", "")
         self.text = str(text or "")
         raw_text: str = option.get("rawText", "")
         self.rawText = str(raw_text or "")
         self.lockedText: bool = option.get("lockedText")
         self.isFavorite: bool = option.get("isFavorite")
         self.isReportedByMe: bool = option.get("isReportedByMe")
@@ -47,26 +43,35 @@
         self.commentsCount: int = option.get("commentsCount")
         self.mentionedUsers: list = option.get("mentionedUsers")
         self.linkedUsers: list = option.get("linkedUsers")
         self.linkedPosts: list = option.get("linkedPosts")
         self.canViewMedia: bool = option.get("canViewMedia")
         self.preview: list[int] = option.get("preview", [])
         self.canPurchase: bool = option.get("canPurchase")
-        self.comments: list[Any] = []
+        self.comments: list[CommentModel] = []
+        self.created_at: datetime = datetime.fromisoformat(option["postedAt"])
+        self.postedAtPrecise: str = option.get("postedAtPrecise")
+        self.expiredAt: Any = option.get("expiredAt")
 
     def get_author(self):
         return self.author
 
     async def get_comments(self):
         epl = endpoint_links()
         link = epl.list_comments(self.responseType, self.id)
         links = epl.create_links(link, self.commentsCount)
         if links:
-            results = await self.author.scrape_manager.bulk_scrape(links)
-            self.comments = results
+            results: list[
+                dict[str, Any]
+            ] = await self.author.scrape_manager.bulk_scrape(links)
+            authed = self.author.get_authed()
+            final_results = [
+                CommentModel(x, await authed.resolve_user(x["author"])) for x in results
+            ]
+            self.comments = final_results
         return self.comments
 
     async def favorite(self):
         link = endpoint_links(
             identifier=f"{self.responseType}s",
             identifier2=self.id,
             identifier3=self.author.id,
```

### Comparing `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/classes/story_model.py` & `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/classes/story_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
+from datetime import datetime
 from typing import TYPE_CHECKING, Any
 
 from ultima_scraper_api.apis.onlyfans import SiteContent
 
 if TYPE_CHECKING:
     from ultima_scraper_api.apis.onlyfans.classes.user_model import create_user
 
 
 class create_story(SiteContent):
     def __init__(self, option: dict[str, Any], user: "create_user") -> None:
         SiteContent.__init__(self, option, user)
         self.userId: int = option.get("userId")
-        self.createdAt: str = option.get("createdAt")
         self.expiredAt: str = option.get("expiredAt")
         self.isReady: bool = option.get("isReady")
         self.viewersCount: int = option.get("viewersCount")
         self.viewers: list = option.get("viewers")
         self.canLike: bool = option.get("canLike")
         self.mediaCount: int = option.get("mediaCount")
         self.isWatched: bool = option.get("isWatched")
@@ -22,7 +22,8 @@
         self.canDelete: bool = option.get("canDelete")
         self.isHighlightCover: bool = option.get("isHighlightCover")
         self.isLastInHighlight: bool = option.get("isLastInHighlight")
         self.media: list[dict[str, Any]] = option.get("media", [])
         self.question: Any = option.get("question")
         self.placedContents: list = option.get("placedContents")
         self.answered: int = option.get("answered")
+        self.created_at: datetime = datetime.fromisoformat(option["createdAt"])
```

### Comparing `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/classes/subscription_model.py` & `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/classes/subscription_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from datetime import datetime
 from typing import TYPE_CHECKING, Any
+
 from ultima_scraper_api.models.subscription_model import BaseSubscriptionModel
 
 if TYPE_CHECKING:
     import ultima_scraper_api
 
     auth_types = ultima_scraper_api.auth_types
     user_types = ultima_scraper_api.user_types
@@ -35,7 +36,10 @@
         return bool(self.active)
 
     def get_authed(self):
         return self.subscriber.get_authed()
 
     def get_price(self):
         return self.subscribe_price
+
+    def resolve_expires_at(self):
+        return self.subscribed_by_expire_date
```

### Comparing `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/classes/user_model.py` & `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/onlyfans/classes/user_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 class create_user(StreamlinedUser):
     def __init__(self, option: dict[str, Any], authed: AuthModel) -> None:
         self.avatar: Optional[str] = option.get("avatar")
         self.avatarThumbs: Optional[list[str]] = option.get("avatarThumbs")
         self.header: Optional[str] = option.get("header")
         self.headerSize: Optional[dict[str, int]] = option.get("headerSize")
         self.headerThumbs: Optional[list[str]] = option.get("headerThumbs")
-        self.id: int = option.get("id")
+        self.id: int = int(option.get("id", 9001))
         self.name: str = option.get("name")
         self.username: str = option.get("username")
         self.canLookStory: bool = option.get("canLookStory")
         self.canCommentStory: bool = option.get("canCommentStory")
         self.hasNotViewedStory: bool = option.get("hasNotViewedStory")
         self.isVerified: bool = option.get("isVerified")
         self.canPayInternal: bool = option.get("canPayInternal")
@@ -214,14 +214,15 @@
         # Custom
         authed.users.add(self)
         self.username = self.get_username()
         self.download_info: dict[str, Any] = {}
         self.duplicate_media = []
         self.scrape_manager = ScrapeManager(authed.session_manager)
         self.__raw__ = option
+        self.__db_user__: Any = None
         StreamlinedUser.__init__(self, authed)
 
     def get_username(self):
         if not self.username:
             self.username = f"u{self.id}"
         return self.username
 
@@ -303,14 +304,16 @@
             links = []
         if not links:
             epl = endpoint_links()
             link = epl.list_posts(self.id)
             links = epl.create_links(link, self.postsCount, limit=limit)
         results = await self.scrape_manager.bulk_scrape(links)
         final_results = self.finalize_content_set(results)
+        for result in final_results:
+            await result.get_comments()
         self.scrape_manager.scraped.Posts = final_results
         return final_results
 
     async def get_post(
         self, identifier: Optional[int | str] = None, limit: int = 10, offset: int = 0
     ) -> Union[create_post, ErrorDetails]:
         if not identifier:
@@ -328,56 +331,48 @@
             return final_result
         return result
 
     async def get_messages(
         self,
         links: list[str] = [],
         limit: int = 10,
-        offset: int = 0,
+        offset_id: int = 0,
+        cutoff_id: int | None = None,
         depth: int = 1,
         refresh: bool = True,
     ):
         result, status = await api_helper.default_data(self, refresh)
         if status:
             return result
         if self.is_deleted:
             return result
-        multiplier = self.get_session_manager().max_threads
         temp_limit = limit
-        temp_offset = offset
         link = endpoint_links(
-            identifier=self.id, global_limit=temp_limit, global_offset=temp_offset
+            identifier=self.id, global_limit=temp_limit, global_offset=offset_id
         ).message_api
-        unpredictable_links, new_offset = api_helper.calculate_the_unpredictable(
-            link, offset, limit, multiplier, depth
-        )
-        links = unpredictable_links if depth != 1 else links + unpredictable_links
-        results = await self.get_session_manager().bulk_json_requests(links)
+        results = await self.get_session_manager().bulk_json_requests([link])
         results = await api_helper.remove_errors(results)
         final_results = []
         if isinstance(results, list):
             results = [x for x in results if x]
             has_more = results[-1]["hasMore"] if results else False
             final_results = [x["list"] for x in results if "list" in x]
             final_results = list(chain.from_iterable(final_results))
-
             if has_more:
-                results2 = await self.get_messages(
-                    limit=temp_limit,
-                    offset=new_offset,
-                    depth=depth + 1,
-                )
-                final_results.extend(results2)
-            if depth == 1:
-                if len(final_results) > 1:
-                    last_link = f"{link}&id={final_results[-1]['id']}"
-                    first_message = await self.get_session_manager().json_request(
-                        last_link
+                temp_offset_id = final_results[-1]["id"]
+                if not any(x for x in final_results if x["id"] == cutoff_id):
+                    pass
+                    results2 = await self.get_messages(
+                        limit=temp_limit,
+                        offset_id=temp_offset_id,
+                        cutoff_id=cutoff_id,
+                        depth=depth + 1,
                     )
-                    final_results.extend(first_message["list"])
+                    final_results.extend(results2)
+            if depth == 1:
                 final_results = [
                     message_model.create_message(x, self) for x in final_results if x
                 ]
             else:
                 final_results.sort(key=lambda x: x["fromUser"]["id"], reverse=True)
             self.scrape_manager.scraped.Messages = final_results
         return final_results
```

### Comparing `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/onlyfans/onlyfans.py` & `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/fansly/fansly.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,47 @@
 from pathlib import Path
 from typing import Any, Literal, Optional, Union
 
 from ultima_scraper_api.apis.api_streamliner import StreamlinedAPI
-from ultima_scraper_api.apis.onlyfans.classes.auth_model import AuthModel
-from ultima_scraper_api.apis.onlyfans.classes.extras import (
+from ultima_scraper_api.apis.fansly.classes.auth_model import AuthModel
+from ultima_scraper_api.apis.fansly.classes.extras import (
     AuthDetails,
-    OnlyFansAuthenticator,
+    FanslyAuthenticator,
     endpoint_links,
 )
-from ultima_scraper_api.apis.onlyfans.classes.message_model import create_message
-from ultima_scraper_api.apis.onlyfans.classes.post_model import create_post
-from ultima_scraper_api.apis.onlyfans.classes.story_model import create_story
-from ultima_scraper_api.apis.onlyfans.classes.user_model import create_user
-from ultima_scraper_api.classes.make_settings import Config
+from ultima_scraper_api.apis.fansly.classes.message_model import create_message
+from ultima_scraper_api.apis.fansly.classes.post_model import create_post
+from ultima_scraper_api.apis.fansly.classes.story_model import create_story
+from ultima_scraper_api.apis.fansly.classes.user_model import create_user
+from ultima_scraper_api.config import UltimaScraperAPIConfig
 
 
-class OnlyFansAPI(StreamlinedAPI):
-    def __init__(self, config: Config = Config()) -> None:
-        self.site_name: Literal["OnlyFans"] = "OnlyFans"
+class FanslyAPI(StreamlinedAPI):
+    def __init__(
+        self, config: UltimaScraperAPIConfig = UltimaScraperAPIConfig()
+    ) -> None:
+        self.site_name: Literal["Fansly"] = "Fansly"
         StreamlinedAPI.__init__(self, self, config)
         self.auths: list[AuthModel] = []
         self.users: dict[int, create_user] = {}
         self.endpoint_links = endpoint_links
 
     async def login(self, auth_json: dict[str, Any] = {}, guest: bool = False):
-        found_auths = [x for x in self.auths if auth_json["id"] == x.id]
+        temp_auth_details = self.create_auth_details(auth_json)
+        found_auths = [x for x in self.auths if temp_auth_details.id == x.id]
         if found_auths:
             authed = found_auths[0]
         else:
-            temp_auth_details = self.create_auth_details(auth_json)
-            authenticator = OnlyFansAuthenticator(self, temp_auth_details)
+            authenticator = FanslyAuthenticator(self, temp_auth_details)
             auth = await authenticator.login(guest)
+            if not auth.is_authed():
+                auth.__raw__ = {"response": {"account": {}}}
             authed = self.add_auth(auth)
-            if isinstance(authed, AuthModel):
-                if authed.is_authed():
-                    issues = await authed.get_login_issues()
-                    authed.issues = issues if issues["data"] else None
         return authed
 
-    def add_user(self, user: create_user):
-        self.users[user.id] = user
-
     def get_auth(self, identifier: Union[str, int]) -> Optional[AuthModel]:
         final_auth = None
         for auth in self.auths:
             if auth.id == identifier:
                 final_auth = auth
             elif auth.username == identifier:
                 final_auth = auth
@@ -57,15 +54,15 @@
             if not auth.is_authed():
                 await self.remove_auth(auth)
 
     async def remove_auth(self, auth: AuthModel):
         await auth.session_manager.active_session.close()
         self.auths.remove(auth)
 
-    def create_auth_details(self, auth_json: dict[str, Any] = {}):
+    def create_auth_details(self, auth_json: dict[str, Any] = {}) -> AuthDetails:
         """If you've got a auth.json file, you can load it into python and pass it through here.
 
         Args:
             auth_json (dict[str, Any], optional): [description]. Defaults to {}.
 
         Returns:
             auth_details: [auth_details object]
@@ -135,19 +132,14 @@
         def __iter__(self):
             for attr, value in self.__dict__.items():
                 yield attr, value
 
         def get_keys(self):
             return [item[0] for item in self]
 
-        async def response_type_to_key(self, value: str):
-            result = [x[0] for x in self if x[0].lower() == f"{value}s"]
-            if result:
-                return result[0]
-
         def path_to_key(self, value: Path):
             for content_type, _ in self:
                 for part in value.parts:
                     if content_type.lower() == part.lower():
                         return content_type
 
         def convert_to_key(self, value: str):
@@ -160,15 +152,15 @@
                     final_value = "Messages"
                 case _:
                     raise Exception("convert_to_key not found")
             return final_value
 
     class MediaTypes:
         def __init__(self) -> None:
-            self.Images = ["photo"]
+            self.Images = ["photo", "image"]
             self.Videos = ["video", "stream", "gif"]
             self.Audios = ["audio"]
             self.Texts = ["text"]
 
         def get_keys(self):
             return [item[0] for item in self.__dict__.items()]
```

### Comparing `ultima_scraper_api-1.1.4/ultima_scraper_api/apis/user_streamliner.py` & `ultima_scraper_api-2.0.0/ultima_scraper_api/apis/user_streamliner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import copy
 from typing import TYPE_CHECKING
 
 import dill
 from ultima_scraper_api.managers.job_manager.jobs.custom_job import CustomJob
+from ultima_scraper_api.managers.scrape_manager import ContentManager
 
 if TYPE_CHECKING:
     import ultima_scraper_api.apis.fansly.classes as fansly_classes
     import ultima_scraper_api.apis.onlyfans.classes as onlyfans_classes
 
     auth_types = (
         onlyfans_classes.auth_model.AuthModel | fansly_classes.auth_model.AuthModel
@@ -51,14 +52,15 @@
 class StreamlinedUser:
     def __init__(self, authed: auth_types) -> None:
         self.__authed = authed
         self.jobs: list[CustomJob] = []
         self.job_whitelist: list[int | str] = []
         self.scrape_whitelist: list[int | str] = []
         self.active: bool = True
+        self.content_manager = ContentManager(authed.session_manager)
 
     def get_authed(self):
         return self.__authed
 
     def get_job(self, value: str):
         found_jobs = [x for x in self.jobs if x.title == value]
         found_job = None
```

### Comparing `ultima_scraper_api-1.1.4/ultima_scraper_api/classes/make_settings.py` & `ultima_scraper_api-2.0.0/ultima_scraper_api/classes/make_settings.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.4/ultima_scraper_api/classes/prepare_metadata.py` & `ultima_scraper_api-2.0.0/ultima_scraper_api/classes/prepare_metadata.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.4/ultima_scraper_api/classes/prepare_webhooks.py` & `ultima_scraper_api-2.0.0/ultima_scraper_api/classes/prepare_webhooks.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.4/ultima_scraper_api/config.py` & `ultima_scraper_api-2.0.0/ultima_scraper_api/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from pathlib import Path
+from typing import Literal
 
 from pydantic import BaseModel
 
+site_name_literals = Literal["OnlyFans", "Fansly"]
+
 
 class Network(BaseModel):
     max_threads: int = -1
     proxies: list[str] = []
     proxy_fallback: bool = True
 
 
@@ -31,30 +34,36 @@
     server: Server = Server()
 
 
 class GlobalAPI(BaseModel):
     pass
 
 
-class OnlyFansAPI(GlobalAPI):
+class OnlyFansAPIConfig(GlobalAPI):
     class OnlyFansCache(GlobalCache):
         paid_content = 3600 * 1
 
     dynamic_rules_url: str = "https://raw.githubusercontent.com/DIGITALCRIMINALS/dynamic-rules/main/onlyfans.json"
     cache = OnlyFansCache()
 
 
-class FanslyAPI(GlobalAPI):
+class FanslyAPIConfig(GlobalAPI):
     class FanslyCache(GlobalCache):
         pass
 
     cache = FanslyCache()
 
 
 class Sites(BaseModel):
-    onlyfans: OnlyFansAPI = OnlyFansAPI()
-    fansly: FanslyAPI = FanslyAPI()
+    onlyfans: OnlyFansAPIConfig = OnlyFansAPIConfig()
+    fansly: FanslyAPIConfig = FanslyAPIConfig()
+
+    def get_settings(self, site_name: site_name_literals):
+        if site_name == "OnlyFans":
+            return self.onlyfans
+        else:
+            return self.fansly
 
 
 class UltimaScraperAPIConfig(BaseModel):
     settings: Settings = Settings()
     site_apis: Sites = Sites()
```

### Comparing `ultima_scraper_api-1.1.4/ultima_scraper_api/docs/Makefile` & `ultima_scraper_api-2.0.0/ultima_scraper_api/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.4/ultima_scraper_api/docs/make.bat` & `ultima_scraper_api-2.0.0/ultima_scraper_api/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.4/ultima_scraper_api/docs/source/conf.py` & `ultima_scraper_api-2.0.0/ultima_scraper_api/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.4/ultima_scraper_api/helpers/main_helper.py` & `ultima_scraper_api-2.0.0/ultima_scraper_api/helpers/main_helper.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from datetime import datetime
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, BinaryIO, Literal
 
 import orjson
 import requests
 import ultima_scraper_api
-import ultima_scraper_api.classes.make_settings as make_settings
 import ultima_scraper_api.classes.prepare_webhooks as prepare_webhooks
 from aiofiles import os as async_os
 from bs4 import BeautifulSoup
 from dateutil.relativedelta import relativedelta
 from mergedeep import Strategy, merge  # type: ignore
 
 if TYPE_CHECKING:
@@ -116,47 +115,18 @@
                 setctime(filepath, timestamp)
                 # print(f"Updated Creation Time {filepath}")
             os.utime(filepath, (timestamp, timestamp))
             # print(f"Updated Modification Time {filepath}")
             break
 
 
-def check_space(
-    download_paths: list[Path],
-    min_size: int = 0,
-    priority: str = "download",
-) -> Path:
-    root = ""
-    while not root:
-        paths = []
-        for download_path in download_paths:
-            # ISSUE
-            # Could cause problems w/ relative/symbolic links that point to another hard drive
-            # Haven't tested if it calculates hard A or relative/symbolic B's total space.
-            obj_Disk = disk_usage(str(download_path.parent))
-            free = obj_Disk.free / (1024.0**3)
-            x = {}
-            x["path"] = download_path
-            x["free"] = free
-            paths.append(x)
-        if priority == "download":
-            for item in paths:
-                download_path = item["path"]
-                free = item["free"]
-                if free > min_size:
-                    root = download_path
-                    break
-        elif priority == "upload":
-            paths.sort(key=lambda x: x["free"])
-            item = paths[0]
-            root = item["path"]
-    return root
-
-
-def prompt_modified(message: str, path: Path):
+def prompt_modified(message: str, path: Path | None = None):
+    input(message)
+    return
+    # Need to move this to an edit config function (tired of all the pop ups)
     editor = shutil.which(
         os.environ.get("EDITOR", "notepad" if os_name == "Windows" else "nano")
     )
     if editor:
         print(message)
         subprocess.run([editor, path], check=True)
     else:
@@ -167,55 +137,57 @@
     json_file: dict[str, Any] = {}
     if json_path.exists() and json_path.stat().st_size and json_path.suffix == ".json":
         with json_path.open(encoding="utf-8") as o_file:
             json_file = orjson.loads(o_file.read())
     return json_file
 
 
-def export_json(metadata: list[Any] | dict[str, Any], filepath: Path):
+def export_json(data: list[Any] | dict[str, Any], filepath: Path):
     if filepath.suffix:
         filepath.parent.mkdir(exist_ok=True)
-    filepath.write_bytes(orjson.dumps(metadata, option=orjson.OPT_INDENT_2))
+    filepath.write_bytes(orjson.dumps(data, option=orjson.OPT_INDENT_2))
 
 
 def object_to_json(item: Any):
-    _json = orjson.loads(orjson.dumps(item, default=lambda o: o.__dict__))
+    _json = orjson.loads(item.json())
     return _json
 
 
-def get_config(config_path: Path) -> tuple[make_settings.Config, bool]:
+from typing import TypeVar, Type
+
+T = TypeVar("T")
+
+
+def get_config(config_path: Path, config_class: Type[T]) -> tuple[T, bool]:
     json_config = import_json(config_path)
+    if "supported" in json_config:
+        config_path.rename(config_path.parent.joinpath("old_config.json"))
     old_json_config = copy.deepcopy(json_config)
-    new_json_config = make_settings.fix(json_config)
-    converted_object = make_settings.Config(**new_json_config)
-    new_json_config = object_to_json(converted_object.export())
-    updated = False
+    new_json_config = old_json_config
+    converted_object = config_class(**new_json_config)
+    new_json_config = object_to_json(converted_object)
+    updated = True if json_config else False
+    status = "updated" if updated else "created"
     if new_json_config != old_json_config:
         export_json(new_json_config, config_path)
-        if json_config:
-            updated = True
-            prompt_modified(
-                f"The {config_path} file has been updated. Fill in whatever you need to fill in and then press enter when done.\n",
-                config_path,
-            )
-        else:
-            if not json_config:
-                prompt_modified(
-                    f"The {config_path} file has been created. Fill in whatever you need to fill in and then press enter when done.\n",
-                    config_path,
-                )
+        prompt_modified(
+            f"The {config_path} file has been {status}. Fill in whatever you need to fill in and then press enter when done.\n",
+        )
 
     return converted_object, updated
 
 
+from ultima_scraper_api.config import Settings
+
+
 async def process_webhooks(
     api: api_types,
     category: str,
     category_2: Literal["succeeded", "failed"],
-    global_settings: make_settings.Settings,
+    global_settings: Settings,
 ):
     webhook_settings = global_settings.webhooks
     global_webhooks = webhook_settings.global_webhooks
     final_webhooks = global_webhooks
     global_status = webhook_settings.global_status
     final_webhook_status = global_status
     webhook_hide_sensitive_info = True
@@ -300,15 +272,15 @@
     if x:
         x = x.group(1)
     else:
         x = s
     return x
 
 
-def extract_string_between_characters(text:str, opening_char:str, closing_char:str):
+def extract_string_between_characters(text: str, opening_char: str, closing_char: str):
     pattern = re.escape(opening_char) + r"(.*?)" + re.escape(closing_char)
     matches = re.findall(pattern, text)
     return matches
 
 
 def module_chooser(domain: str, json_sites: dict[str, Any]):
     string = "Select Site: "
```

### Comparing `ultima_scraper_api-1.1.4/ultima_scraper_api/managers/job_manager/job_manager.py` & `ultima_scraper_api-2.0.0/ultima_scraper_api/managers/job_manager/job_manager.py`

 * *Files 19% similar despite different names*

```diff
@@ -33,21 +33,34 @@
                 case _:
                     job = None
             if job:
                 local_jobs.append(job)
         self.jobs.extend(local_jobs)
         return local_jobs
 
+    def create_job(self, value: str, module: Any, module_args: list[Any]):
+        local_args = copy.copy(module_args)
+        match value:
+            case "DatabaseImport":
+                job = CustomJob(value)
+                job.task = module(*local_args)
+                self.jobs.append(job)
+            case _:
+                raise Exception(f"Could not create job: {value}")
+        return job
+
     def add_media_type_to_jobs(self, media_type: str | list[str]):
         if isinstance(media_type, str):
             media_type = [media_type]
         [job.add_media_type(mt) for job in self.jobs for mt in media_type]
+
     async def process_jobs(self):
         await asyncio.create_task(self.__worker())
         await self.queue.join()
+
     async def __worker(self):
         while True:
             if self.queue.qsize() == 0:
                 return
             job = await self.queue.get()
             # We can make jobs work in the background if we make waiting for inputs async
             await job.task
```

### Comparing `ultima_scraper_api-1.1.4/ultima_scraper_api/managers/job_manager/jobs/custom_job.py` & `ultima_scraper_api-2.0.0/ultima_scraper_api/managers/job_manager/jobs/custom_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import copy
 
 import dill
 
 
 class CustomJob:
-    def __init__(self, job_type: str, api_type: str) -> None:
+    def __init__(self, job_type: str, api_type: str | None = None) -> None:
         self.title = f"{job_type}: {api_type}"
         self.type = job_type
         self.api_type = api_type
         self.media_types: list[str] = []
         self.min = 0
         self.task = None
         self.result = []
```

### Comparing `ultima_scraper_api-1.1.4/ultima_scraper_api/managers/scrape_manager.py` & `ultima_scraper_api-2.0.0/ultima_scraper_api/managers/scrape_manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,14 +2,33 @@
 from itertools import chain
 from typing import Any
 
 from ultima_scraper_api.apis.api_helper import handle_error_details
 from ultima_scraper_api.managers.session_manager import SessionManager
 
 
+class ContentManager:
+    def __init__(self, session_manager: SessionManager) -> None:
+        self.session_manager = session_manager
+        self.categorized = session_manager.auth.api.CategorizedContent()
+
+    def set_content(self, content_type: str, scraped: list[Any]):
+        for content in scraped:
+            content_item = getattr(self.categorized, content_type)
+            content_item[content.content_id] = content
+
+    def find_content(self, content_id: int, content_type: str):
+        found_content = None
+        try:
+            found_content = getattr(self.categorized, content_type)[content_id]
+        except KeyError:
+            pass
+        return found_content
+
+
 class ScrapeManager:
     def __init__(self, session_manager: SessionManager) -> None:
         self.session_manager = session_manager
         self.handle_errors = True
         self.scraped = session_manager.auth.api.ContentTypes()
 
     async def bulk_scrape(self, urls: list[str]):
@@ -20,16 +39,19 @@
         return final_result
 
     async def scrape(self, url: str):
         session_manager = self.session_manager
         async with session_manager.semaphore:
             result = await session_manager.request(url)
             async with result as response:
-                json_res = await response.json()
-                final_result = await self.handle_error(url, json_res)
+                if result.status != 404:
+                    json_res = await response.json()
+                    final_result = await self.handle_error(url, json_res)
+                else:
+                    final_result = []
                 return final_result
 
     async def handle_error(self, url: str, json_res: dict[str, Any]):
         import ultima_scraper_api.apis.fansly.classes as fansly_classes
         import ultima_scraper_api.apis.onlyfans.classes as onlyfans_classes
 
         session_manager = self.session_manager
@@ -49,8 +71,8 @@
         return json_res
 
     async def handle_refresh(self, item: Any):
         abc = getattr(self.session_manager.auth, f"get_{item.responseType}")
         return abc
 
     def set_scraped(self, name: str, scraped: list[Any]):
-        setattr(self.scraped, name, scraped)
+        setattr(self.scraped, name, scraped)
```

### Comparing `ultima_scraper_api-1.1.4/ultima_scraper_api/managers/session_manager.py` & `ultima_scraper_api-2.0.0/ultima_scraper_api/managers/session_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,23 +84,20 @@
         max_threads = api_helper.calculate_max_threads(max_threads)
         self.semaphore = asyncio.BoundedSemaphore(max_threads)
         self.max_threads = max_threads
         self.max_attempts = 10
         self.kill = False
         self.headers = headers
         self.proxies: list[str] = (
-            proxies if proxies else auth.api.config.settings.proxies
+            proxies if proxies else auth.api.config.settings.network.proxies
         )
         self.proxy_manager = ProxyManager(self)
-        global_settings = auth.api.get_global_settings()
-        dynamic_rules_link = (
-            global_settings.dynamic_rules_link if global_settings else ""
-        )
-        dr_link = dynamic_rules_link
-        dynamic_rules = requests.get(dr_link).json()  # type: ignore
+        site_settings = auth.api.config.site_apis.get_settings(auth.api.site_name)
+        dynamic_rules_url = getattr(site_settings, "dynamic_rules_url")
+        dynamic_rules = requests.get(dynamic_rules_url).json()  # type: ignore
         self.dynamic_rules = dynamic_rules
         self.auth = auth
         self.use_cookies: bool = use_cookies
         self.active_session = self.create_client_session()
         self.request_count = 0
         # self.last_request_time: float | None = None
         # self.rate_limit_wait_minutes = 6
@@ -241,42 +238,45 @@
                 headers["accept"] = "application/json, text/plain, */*"
                 headers["Connection"] = "keep-alive"
             if custom_cookies:
                 headers = await self.session_rules(url, custom_cookies=custom_cookies)
                 pass
 
             # await self.limit_rate()
+            result = None
             try:
                 match method.upper():
                     case "GET":
                         result = await self.active_session.get(url, headers=headers)
                     case "POST":
                         result = await self.active_session.post(
                             url, headers=headers, data=data
                         )
             except EXCEPTION_TEMPLATE as _e:
                 continue
             except Exception as _e:
                 continue
             try:
+                assert result
                 result.raise_for_status()
                 return result
             except EXCEPTION_TEMPLATE as _e:
                 # Can retry
                 continue
             except ClientResponseError as _e:
                 match _e.status:
                     case 400 | 401 | 403 | 404:
+                        assert result
                         return result
                     case 429:
                         pass
                         if self.is_rate_limited is None:
                             self.rate_limit_check = True
                         continue
-                    case 500 | 503 | 504:
+                    case 500 | 502 | 503 | 504:
                         continue
                     case _:
                         raise Exception(
                             f"Infinite Loop Detected for unhandled status error: {_e.status}"
                         )
             except Exception as _e:
                 pass
```

### Comparing `ultima_scraper_api-1.1.4/ultima_scraper_api/models/subscription_model.py` & `ultima_scraper_api-2.0.0/ultima_scraper_api/models/subscription_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_api-1.1.4/PKG-INFO` & `ultima_scraper_api-2.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultima-scraper-api
-Version: 1.1.4
+Version: 2.0.0
 Summary: 
 Author: DIGITALCRIMINALS
 Author-email: 89371864+digitalcriminals@users.noreply.github.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

