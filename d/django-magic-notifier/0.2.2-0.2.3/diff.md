# Comparing `tmp/django-magic-notifier-0.2.2.tar.gz` & `tmp/django-magic-notifier-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-magic-notifier-0.2.2.tar", last modified: Thu Jun 29 05:59:06 2023, max compression
+gzip compressed data, was "django-magic-notifier-0.2.3.tar", last modified: Tue Jul 11 09:47:31 2023, max compression
```

## Comparing `django-magic-notifier-0.2.2.tar` & `django-magic-notifier-0.2.3.tar`

### file list

```diff
@@ -1,96 +1,93 @@
-drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-06-29 05:59:06.739467 django-magic-notifier-0.2.2/
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)       63 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/.gitignore
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      783 2023-05-11 23:47:24.000000 django-magic-notifier-0.2.2/.travis.yml
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     1065 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/LICENSE
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     5796 2023-06-29 05:59:06.739467 django-magic-notifier-0.2.2/PKG-INFO
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     4783 2022-09-14 23:23:35.000000 django-magic-notifier-0.2.2/README.md
-drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-06-29 05:59:06.723467 django-magic-notifier-0.2.2/django_magic_notifier.egg-info/
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     5796 2023-06-29 05:59:06.000000 django-magic-notifier-0.2.2/django_magic_notifier.egg-info/PKG-INFO
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     2318 2023-06-29 05:59:06.000000 django-magic-notifier-0.2.2/django_magic_notifier.egg-info/SOURCES.txt
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)        1 2023-06-29 05:59:06.000000 django-magic-notifier-0.2.2/django_magic_notifier.egg-info/dependency_links.txt
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      102 2023-06-29 05:59:06.000000 django-magic-notifier-0.2.2/django_magic_notifier.egg-info/requires.txt
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)       15 2023-06-29 05:59:06.000000 django-magic-notifier-0.2.2/django_magic_notifier.egg-info/top_level.txt
-drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-06-29 05:59:06.723467 django-magic-notifier-0.2.2/docs/
-drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-06-29 05:59:06.727467 django-magic-notifier-0.2.2/docs/source/
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     2646 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/docs/source/conf.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      547 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/docs/source/index.rst
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      270 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/docs/source/installation.rst
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     3452 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/docs/source/settings.rst
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     1963 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/docs/source/templates.rst
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     2236 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/docs/source/usage.rst
-drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-06-29 05:59:06.731467 django-magic-notifier-0.2.2/magic_notifier/
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)        0 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/magic_notifier/__init__.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      165 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/magic_notifier/admin.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)       94 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/magic_notifier/apps.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     2687 2022-09-14 22:26:11.000000 django-magic-notifier-0.2.2/magic_notifier/consumers.py
-drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-06-29 05:59:06.731467 django-magic-notifier-0.2.2/magic_notifier/email_clients/
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)        0 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/magic_notifier/email_clients/__init__.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      680 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/magic_notifier/email_clients/django_email.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     5567 2023-06-29 05:58:16.000000 django-magic-notifier-0.2.2/magic_notifier/emailer.py
-drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-06-29 05:59:06.731467 django-magic-notifier-0.2.2/magic_notifier/management/
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)        0 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/magic_notifier/management/__init__.py
-drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-06-29 05:59:06.731467 django-magic-notifier-0.2.2/magic_notifier/management/commands/
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)        0 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/magic_notifier/management/commands/__init__.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     1493 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/magic_notifier/management/commands/test_email_template.py
-drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-06-29 05:59:06.731467 django-magic-notifier-0.2.2/magic_notifier/migrations/
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     1538 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/magic_notifier/migrations/0001_initial.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     1316 2022-09-07 21:12:23.000000 django-magic-notifier-0.2.2/magic_notifier/migrations/0002_auto_20220907_2112.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      642 2022-09-14 17:56:58.000000 django-magic-notifier-0.2.2/magic_notifier/migrations/0003_auto_20220914_1756.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      425 2023-05-11 23:39:30.000000 django-magic-notifier-0.2.2/magic_notifier/migrations/0004_alter_notification_subject.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)        0 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/magic_notifier/migrations/__init__.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     4291 2022-09-14 23:45:26.000000 django-magic-notifier-0.2.2/magic_notifier/models.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     4211 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/magic_notifier/notifier.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     2337 2022-09-14 23:18:42.000000 django-magic-notifier-0.2.2/magic_notifier/pusher.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      475 2022-09-14 23:01:35.000000 django-magic-notifier-0.2.2/magic_notifier/serializers.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     1451 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/magic_notifier/settings.py
-drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-06-29 05:59:06.735467 django-magic-notifier-0.2.2/magic_notifier/sms_clients/
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)        0 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/magic_notifier/sms_clients/__init__.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      136 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/magic_notifier/sms_clients/base.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      734 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/magic_notifier/sms_clients/cgsms_client.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     1022 2022-09-07 21:21:50.000000 django-magic-notifier-0.2.2/magic_notifier/sms_clients/nexa_client.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      510 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/magic_notifier/sms_clients/twilio_client.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     2941 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/magic_notifier/smser.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      249 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/magic_notifier/tasks.py
-drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-06-29 05:59:06.723467 django-magic-notifier-0.2.2/magic_notifier/templates/
-drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-06-29 05:59:06.735467 django-magic-notifier-0.2.2/magic_notifier/templates/base_notifier/
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)    11390 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/magic_notifier/templates/base_notifier/email.html
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      232 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/magic_notifier/templates/base_notifier/email.txt
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     1032 2023-01-05 02:18:25.000000 django-magic-notifier-0.2.2/magic_notifier/templates/base_notifier/push.json
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)       51 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/magic_notifier/templates/base_notifier/sms.txt
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     4602 2022-09-14 17:56:12.000000 django-magic-notifier-0.2.2/magic_notifier/utils.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)        1 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/magic_notifier/views.py
-drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-06-29 05:59:06.735467 django-magic-notifier-0.2.2/requirements/
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)       39 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/requirements/base.txt
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)       19 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/requirements/deploy.txt
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)       39 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/requirements/docs.txt
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)       32 2022-09-14 23:32:59.000000 django-magic-notifier-0.2.2/requirements/test.txt
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)       38 2023-06-29 05:59:06.739467 django-magic-notifier-0.2.2/setup.cfg
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     4240 2023-06-29 05:58:32.000000 django-magic-notifier-0.2.2/setup.py
-drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-06-29 05:59:06.735467 django-magic-notifier-0.2.2/tests/
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      542 2022-09-14 23:04:56.000000 django-magic-notifier-0.2.2/tests/connect.py
-drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-06-29 05:59:06.739467 django-magic-notifier-0.2.2/tests/core/
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)        0 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/tests/core/__init__.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)       63 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/tests/core/admin.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)       83 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/tests/core/apps.py
-drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-06-29 05:59:06.739467 django-magic-notifier-0.2.2/tests/core/migrations/
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)        0 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/tests/core/migrations/__init__.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)       57 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/tests/core/models.py
-drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-06-29 05:59:06.723467 django-magic-notifier-0.2.2/tests/core/templates/
-drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-06-29 05:59:06.723467 django-magic-notifier-0.2.2/tests/core/templates/notifier/
-drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-06-29 05:59:06.739467 django-magic-notifier-0.2.2/tests/core/templates/notifier/base/
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)       42 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/tests/core/templates/notifier/base/email.html
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      341 2023-06-28 22:31:50.000000 django-magic-notifier-0.2.2/tests/core/templates/notifier/base/email.mjml
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)       40 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/tests/core/templates/notifier/base/email.txt
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     1037 2022-09-14 23:00:22.000000 django-magic-notifier-0.2.2/tests/core/templates/notifier/base/push.json
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      105 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/tests/core/templates/notifier/base/sms.txt
-drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-06-29 05:59:06.739467 django-magic-notifier-0.2.2/tests/core/templates/notifier/hello/
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)       82 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/tests/core/templates/notifier/hello/email.txt
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)    19813 2022-09-14 23:19:15.000000 django-magic-notifier-0.2.2/tests/core/tests.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)       63 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/tests/core/views.py
-drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-06-29 05:59:06.739467 django-magic-notifier-0.2.2/tests/example/
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)        0 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/tests/example/__init__.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      861 2022-09-14 22:27:50.000000 django-magic-notifier-0.2.2/tests/example/asgi.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     4693 2022-09-14 23:17:26.000000 django-magic-notifier-0.2.2/tests/example/settings.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      749 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/tests/example/urls.py
--rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      391 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/tests/example/wsgi.py
--rwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)      627 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.2/tests/manage.py
+drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-07-11 09:47:31.134592 django-magic-notifier-0.2.3/
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)       63 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.3/.gitignore
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      783 2023-05-11 23:47:24.000000 django-magic-notifier-0.2.3/.travis.yml
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     1065 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.3/LICENSE
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     5640 2023-07-11 09:47:31.134592 django-magic-notifier-0.2.3/PKG-INFO
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     4627 2023-07-11 09:35:05.000000 django-magic-notifier-0.2.3/README.md
+drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-07-11 09:47:31.118591 django-magic-notifier-0.2.3/django_magic_notifier.egg-info/
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     5640 2023-07-11 09:47:30.000000 django-magic-notifier-0.2.3/django_magic_notifier.egg-info/PKG-INFO
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     2151 2023-07-11 09:47:31.000000 django-magic-notifier-0.2.3/django_magic_notifier.egg-info/SOURCES.txt
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)        1 2023-07-11 09:47:30.000000 django-magic-notifier-0.2.3/django_magic_notifier.egg-info/dependency_links.txt
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      102 2023-07-11 09:47:30.000000 django-magic-notifier-0.2.3/django_magic_notifier.egg-info/requires.txt
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)       15 2023-07-11 09:47:30.000000 django-magic-notifier-0.2.3/django_magic_notifier.egg-info/top_level.txt
+drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-07-11 09:47:31.114591 django-magic-notifier-0.2.3/docs/
+drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-07-11 09:47:31.122592 django-magic-notifier-0.2.3/docs/source/
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     2646 2023-07-11 09:43:52.000000 django-magic-notifier-0.2.3/docs/source/conf.py
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      545 2023-07-10 21:17:34.000000 django-magic-notifier-0.2.3/docs/source/index.rst
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      728 2023-07-11 09:13:45.000000 django-magic-notifier-0.2.3/docs/source/installation.rst
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     3868 2023-07-11 09:42:31.000000 django-magic-notifier-0.2.3/docs/source/settings.rst
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     3169 2023-07-11 09:27:11.000000 django-magic-notifier-0.2.3/docs/source/templates.rst
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     2516 2023-07-10 21:27:57.000000 django-magic-notifier-0.2.3/docs/source/usage.rst
+drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-07-11 09:47:31.126592 django-magic-notifier-0.2.3/magic_notifier/
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)        0 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.3/magic_notifier/__init__.py
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      165 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.3/magic_notifier/admin.py
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)       94 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.3/magic_notifier/apps.py
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     2687 2022-09-14 22:26:11.000000 django-magic-notifier-0.2.3/magic_notifier/consumers.py
+drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-07-11 09:47:31.126592 django-magic-notifier-0.2.3/magic_notifier/email_clients/
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)        0 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.3/magic_notifier/email_clients/__init__.py
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      680 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.3/magic_notifier/email_clients/django_email.py
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     5567 2023-06-29 05:58:16.000000 django-magic-notifier-0.2.3/magic_notifier/emailer.py
+drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-07-11 09:47:31.126592 django-magic-notifier-0.2.3/magic_notifier/management/
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)        0 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.3/magic_notifier/management/__init__.py
+drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-07-11 09:47:31.126592 django-magic-notifier-0.2.3/magic_notifier/management/commands/
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)        0 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.3/magic_notifier/management/commands/__init__.py
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     1493 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.3/magic_notifier/management/commands/test_email_template.py
+drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-07-11 09:47:31.126592 django-magic-notifier-0.2.3/magic_notifier/migrations/
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     2057 2023-07-11 09:46:29.000000 django-magic-notifier-0.2.3/magic_notifier/migrations/0001_initial.py
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)        0 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.3/magic_notifier/migrations/__init__.py
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     4291 2022-09-14 23:45:26.000000 django-magic-notifier-0.2.3/magic_notifier/models.py
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     4211 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.3/magic_notifier/notifier.py
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     2622 2023-07-11 09:03:15.000000 django-magic-notifier-0.2.3/magic_notifier/pusher.py
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      475 2022-09-14 23:01:35.000000 django-magic-notifier-0.2.3/magic_notifier/serializers.py
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     1451 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.3/magic_notifier/settings.py
+drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-07-11 09:47:31.126592 django-magic-notifier-0.2.3/magic_notifier/sms_clients/
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)        0 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.3/magic_notifier/sms_clients/__init__.py
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      136 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.3/magic_notifier/sms_clients/base.py
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      734 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.3/magic_notifier/sms_clients/cgsms_client.py
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     1022 2022-09-07 21:21:50.000000 django-magic-notifier-0.2.3/magic_notifier/sms_clients/nexa_client.py
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      510 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.3/magic_notifier/sms_clients/twilio_client.py
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     2941 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.3/magic_notifier/smser.py
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      249 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.3/magic_notifier/tasks.py
+drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-07-11 09:47:31.118591 django-magic-notifier-0.2.3/magic_notifier/templates/
+drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-07-11 09:47:31.126592 django-magic-notifier-0.2.3/magic_notifier/templates/base_notifier/
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)    11390 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.3/magic_notifier/templates/base_notifier/email.html
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      232 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.3/magic_notifier/templates/base_notifier/email.txt
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     1032 2023-01-05 02:18:25.000000 django-magic-notifier-0.2.3/magic_notifier/templates/base_notifier/push.json
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)       51 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.3/magic_notifier/templates/base_notifier/sms.txt
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     4602 2022-09-14 17:56:12.000000 django-magic-notifier-0.2.3/magic_notifier/utils.py
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)        1 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.3/magic_notifier/views.py
+drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-07-11 09:47:31.130592 django-magic-notifier-0.2.3/requirements/
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)       39 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.3/requirements/base.txt
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)       19 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.3/requirements/deploy.txt
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)       39 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.3/requirements/docs.txt
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)       32 2022-09-14 23:32:59.000000 django-magic-notifier-0.2.3/requirements/test.txt
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)       38 2023-07-11 09:47:31.134592 django-magic-notifier-0.2.3/setup.cfg
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     4240 2023-07-11 09:43:00.000000 django-magic-notifier-0.2.3/setup.py
+drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-07-11 09:47:31.130592 django-magic-notifier-0.2.3/tests/
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      542 2022-09-14 23:04:56.000000 django-magic-notifier-0.2.3/tests/connect.py
+drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-07-11 09:47:31.130592 django-magic-notifier-0.2.3/tests/core/
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)        0 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.3/tests/core/__init__.py
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)       63 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.3/tests/core/admin.py
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)       83 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.3/tests/core/apps.py
+drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-07-11 09:47:31.130592 django-magic-notifier-0.2.3/tests/core/migrations/
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)        0 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.3/tests/core/migrations/__init__.py
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)       57 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.3/tests/core/models.py
+drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-07-11 09:47:31.118591 django-magic-notifier-0.2.3/tests/core/templates/
+drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-07-11 09:47:31.118591 django-magic-notifier-0.2.3/tests/core/templates/notifier/
+drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-07-11 09:47:31.130592 django-magic-notifier-0.2.3/tests/core/templates/notifier/base/
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)       42 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.3/tests/core/templates/notifier/base/email.html
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      341 2023-06-28 22:31:50.000000 django-magic-notifier-0.2.3/tests/core/templates/notifier/base/email.mjml
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)       40 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.3/tests/core/templates/notifier/base/email.txt
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     1037 2022-09-14 23:00:22.000000 django-magic-notifier-0.2.3/tests/core/templates/notifier/base/push.json
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      105 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.3/tests/core/templates/notifier/base/sms.txt
+drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-07-11 09:47:31.130592 django-magic-notifier-0.2.3/tests/core/templates/notifier/hello/
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)       82 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.3/tests/core/templates/notifier/hello/email.txt
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)    19813 2022-09-14 23:19:15.000000 django-magic-notifier-0.2.3/tests/core/tests.py
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)       63 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.3/tests/core/views.py
+drwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)        0 2023-07-11 09:47:31.134592 django-magic-notifier-0.2.3/tests/example/
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)        0 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.3/tests/example/__init__.py
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      861 2022-09-14 22:27:50.000000 django-magic-notifier-0.2.3/tests/example/asgi.py
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)     4693 2022-09-14 23:17:26.000000 django-magic-notifier-0.2.3/tests/example/settings.py
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      749 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.3/tests/example/urls.py
+-rw-rw-r--   0 jefcolbi  (1000) jefcolbi  (1000)      391 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.3/tests/example/wsgi.py
+-rwxrwxr-x   0 jefcolbi  (1000) jefcolbi  (1000)      627 2022-09-07 19:15:11.000000 django-magic-notifier-0.2.3/tests/manage.py
```

### Comparing `django-magic-notifier-0.2.2/.travis.yml` & `django-magic-notifier-0.2.3/.travis.yml`

 * *Files identical despite different names*

### Comparing `django-magic-notifier-0.2.2/LICENSE` & `django-magic-notifier-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-magic-notifier-0.2.2/PKG-INFO` & `django-magic-notifier-0.2.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-magic-notifier
-Version: 0.2.2
+Version: 0.2.3
 Summary: A notifications library for Djangonauts that support email, sms and push.
 Home-page: https://github.com/jefcolbi/django-magic-notifier
 Author: jefcolbi
 Author-email: jefcolbi@gmail.com
 License: MIT
 Classifier: Natural Language :: English
 Classifier: Natural Language :: French
@@ -44,18 +44,19 @@
 - Send sms, TWILIO support
 - Send push notifications
 - Support templates
 - Simple API
 - Support files
 - Support multiple gateways
 - Extensible
+- Support MJML
 
 
 ### Installation
-> $pip install --upgrade django-magic-notifier
+> pip install --upgrade django-magic-notifier
 
 ### Usage
 ##### 1. Configure settings
 If you have already configured SMTP EMAIL SETTINGS in django settings then can ignore this step. Else add a NOTIFIER dict in your settings like this
 
 ```python
 NOTIFIER = {
@@ -72,46 +73,39 @@
         }
     },
     "USER_FROM_WS_TOKEN_FUNCTION": 'magic_notifier.utils.get_user_from_ws_token'
 }
 ```
 
 ##### 2. Create templates
-Create a folder named **notifier** in one of app's templates dir. In this folder create another folder named **base** then created your base templates in this folder. Example  
+Create a folder named **notifier** in one of app's templates dir. In this folder create another folder named **my_template** 
+then create your base templates in this folder. Example:  
 
-*app_name/templates/notifier/base/email.html*
+*app_name/templates/notifier/my_template/email.html*
 ```
-    {% extends "base_notifier/email.html" %}
+{% extends "base_notifier/email.html" %}
+{% block content %}
+<tr>
+    <td><p>Hello {{ user.email }}
+    </td>
+</tr>
+{% endblock %}
 ```  
 
-*app_name/templates/notifier/base/email.txt*
+*app_name/templates/notifier/my_template/email.txt*
 ```
-    {% extends "base_notifier/email.txt" %}
+{% extends "base_notifier/email.txt" %}
+{% block content %}
+Hello {{ user.email }}
+{% endblock %}
 ```  
 
-*app_name/templates/notifier/hello/email.html*
-```
-    {% extends "notifier/base/email.html" %}
-    {% block content %}
-    <tr>
-        <td><p>Hello {{ user.email }}
-        </td>
-    </tr>
-    {% endblock %}
-```  
-
-*app_name/templates/notifier/hello/email.txt*
-```
-    {% extends "notifier/hello/email.txt" %}
-    {% block content %}
-    >Hello {{ user.email }}
-    {% endblock %}
-```  
-
-As you can see, the user to whom the notification goes is automatically added in the template's context. To avoid any clash to don't send the key `'user'` in the context of the  **notifiy()** function presented below.
+As you can see, the user to whom the notification goes is automatically added 
+in the template's context. To avoid any clash don't send the key `'user'` 
+in the context of the  **notifiy()** function presented below.
 
 Note that it is DMN (Django Magic Notifier) that has the base_notifier template.
 
 ##### 3. Send notifications
 To send a notification via email do
 ```python
     from magic_notifier.notifier import notify
@@ -134,15 +128,15 @@
     # send a notification via email and sms from a template
     user = User(email="testuser@localhost", username="testuser")
     subject = "Test magic notifier"
     notify(["email", "sms"], subject, [user], template='hello')
 ```
 
 ### Docs and support
-Coming
+https://django-magic-notifier.readthedocs.io/en/latest/index.html
 
 
 ### Roadmap
 
 - Generate full documentation
 - Translate documentation
```

### Comparing `django-magic-notifier-0.2.2/README.md` & `django-magic-notifier-0.2.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -16,18 +16,19 @@
 - Send sms, TWILIO support
 - Send push notifications
 - Support templates
 - Simple API
 - Support files
 - Support multiple gateways
 - Extensible
+- Support MJML
 
 
 ### Installation
-> $pip install --upgrade django-magic-notifier
+> pip install --upgrade django-magic-notifier
 
 ### Usage
 ##### 1. Configure settings
 If you have already configured SMTP EMAIL SETTINGS in django settings then can ignore this step. Else add a NOTIFIER dict in your settings like this
 
 ```python
 NOTIFIER = {
@@ -44,46 +45,39 @@
         }
     },
     "USER_FROM_WS_TOKEN_FUNCTION": 'magic_notifier.utils.get_user_from_ws_token'
 }
 ```
 
 ##### 2. Create templates
-Create a folder named **notifier** in one of app's templates dir. In this folder create another folder named **base** then created your base templates in this folder. Example  
+Create a folder named **notifier** in one of app's templates dir. In this folder create another folder named **my_template** 
+then create your base templates in this folder. Example:  
 
-*app_name/templates/notifier/base/email.html*
+*app_name/templates/notifier/my_template/email.html*
 ```
-    {% extends "base_notifier/email.html" %}
+{% extends "base_notifier/email.html" %}
+{% block content %}
+<tr>
+    <td><p>Hello {{ user.email }}
+    </td>
+</tr>
+{% endblock %}
 ```  
 
-*app_name/templates/notifier/base/email.txt*
+*app_name/templates/notifier/my_template/email.txt*
 ```
-    {% extends "base_notifier/email.txt" %}
+{% extends "base_notifier/email.txt" %}
+{% block content %}
+Hello {{ user.email }}
+{% endblock %}
 ```  
 
-*app_name/templates/notifier/hello/email.html*
-```
-    {% extends "notifier/base/email.html" %}
-    {% block content %}
-    <tr>
-        <td><p>Hello {{ user.email }}
-        </td>
-    </tr>
-    {% endblock %}
-```  
-
-*app_name/templates/notifier/hello/email.txt*
-```
-    {% extends "notifier/hello/email.txt" %}
-    {% block content %}
-    >Hello {{ user.email }}
-    {% endblock %}
-```  
-
-As you can see, the user to whom the notification goes is automatically added in the template's context. To avoid any clash to don't send the key `'user'` in the context of the  **notifiy()** function presented below.
+As you can see, the user to whom the notification goes is automatically added 
+in the template's context. To avoid any clash don't send the key `'user'` 
+in the context of the  **notifiy()** function presented below.
 
 Note that it is DMN (Django Magic Notifier) that has the base_notifier template.
 
 ##### 3. Send notifications
 To send a notification via email do
 ```python
     from magic_notifier.notifier import notify
@@ -106,15 +100,15 @@
     # send a notification via email and sms from a template
     user = User(email="testuser@localhost", username="testuser")
     subject = "Test magic notifier"
     notify(["email", "sms"], subject, [user], template='hello')
 ```
 
 ### Docs and support
-Coming
+https://django-magic-notifier.readthedocs.io/en/latest/index.html
 
 
 ### Roadmap
 
 - Generate full documentation
 - Translate documentation
```

### Comparing `django-magic-notifier-0.2.2/django_magic_notifier.egg-info/PKG-INFO` & `django-magic-notifier-0.2.3/django_magic_notifier.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-magic-notifier
-Version: 0.2.2
+Version: 0.2.3
 Summary: A notifications library for Djangonauts that support email, sms and push.
 Home-page: https://github.com/jefcolbi/django-magic-notifier
 Author: jefcolbi
 Author-email: jefcolbi@gmail.com
 License: MIT
 Classifier: Natural Language :: English
 Classifier: Natural Language :: French
@@ -44,18 +44,19 @@
 - Send sms, TWILIO support
 - Send push notifications
 - Support templates
 - Simple API
 - Support files
 - Support multiple gateways
 - Extensible
+- Support MJML
 
 
 ### Installation
-> $pip install --upgrade django-magic-notifier
+> pip install --upgrade django-magic-notifier
 
 ### Usage
 ##### 1. Configure settings
 If you have already configured SMTP EMAIL SETTINGS in django settings then can ignore this step. Else add a NOTIFIER dict in your settings like this
 
 ```python
 NOTIFIER = {
@@ -72,46 +73,39 @@
         }
     },
     "USER_FROM_WS_TOKEN_FUNCTION": 'magic_notifier.utils.get_user_from_ws_token'
 }
 ```
 
 ##### 2. Create templates
-Create a folder named **notifier** in one of app's templates dir. In this folder create another folder named **base** then created your base templates in this folder. Example  
+Create a folder named **notifier** in one of app's templates dir. In this folder create another folder named **my_template** 
+then create your base templates in this folder. Example:  
 
-*app_name/templates/notifier/base/email.html*
+*app_name/templates/notifier/my_template/email.html*
 ```
-    {% extends "base_notifier/email.html" %}
+{% extends "base_notifier/email.html" %}
+{% block content %}
+<tr>
+    <td><p>Hello {{ user.email }}
+    </td>
+</tr>
+{% endblock %}
 ```  
 
-*app_name/templates/notifier/base/email.txt*
+*app_name/templates/notifier/my_template/email.txt*
 ```
-    {% extends "base_notifier/email.txt" %}
+{% extends "base_notifier/email.txt" %}
+{% block content %}
+Hello {{ user.email }}
+{% endblock %}
 ```  
 
-*app_name/templates/notifier/hello/email.html*
-```
-    {% extends "notifier/base/email.html" %}
-    {% block content %}
-    <tr>
-        <td><p>Hello {{ user.email }}
-        </td>
-    </tr>
-    {% endblock %}
-```  
-
-*app_name/templates/notifier/hello/email.txt*
-```
-    {% extends "notifier/hello/email.txt" %}
-    {% block content %}
-    >Hello {{ user.email }}
-    {% endblock %}
-```  
-
-As you can see, the user to whom the notification goes is automatically added in the template's context. To avoid any clash to don't send the key `'user'` in the context of the  **notifiy()** function presented below.
+As you can see, the user to whom the notification goes is automatically added 
+in the template's context. To avoid any clash don't send the key `'user'` 
+in the context of the  **notifiy()** function presented below.
 
 Note that it is DMN (Django Magic Notifier) that has the base_notifier template.
 
 ##### 3. Send notifications
 To send a notification via email do
 ```python
     from magic_notifier.notifier import notify
@@ -134,15 +128,15 @@
     # send a notification via email and sms from a template
     user = User(email="testuser@localhost", username="testuser")
     subject = "Test magic notifier"
     notify(["email", "sms"], subject, [user], template='hello')
 ```
 
 ### Docs and support
-Coming
+https://django-magic-notifier.readthedocs.io/en/latest/index.html
 
 
 ### Roadmap
 
 - Generate full documentation
 - Translate documentation
```

### Comparing `django-magic-notifier-0.2.2/django_magic_notifier.egg-info/SOURCES.txt` & `django-magic-notifier-0.2.3/django_magic_notifier.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -30,17 +30,14 @@
 magic_notifier/views.py
 magic_notifier/email_clients/__init__.py
 magic_notifier/email_clients/django_email.py
 magic_notifier/management/__init__.py
 magic_notifier/management/commands/__init__.py
 magic_notifier/management/commands/test_email_template.py
 magic_notifier/migrations/0001_initial.py
-magic_notifier/migrations/0002_auto_20220907_2112.py
-magic_notifier/migrations/0003_auto_20220914_1756.py
-magic_notifier/migrations/0004_alter_notification_subject.py
 magic_notifier/migrations/__init__.py
 magic_notifier/sms_clients/__init__.py
 magic_notifier/sms_clients/base.py
 magic_notifier/sms_clients/cgsms_client.py
 magic_notifier/sms_clients/nexa_client.py
 magic_notifier/sms_clients/twilio_client.py
 magic_notifier/templates/base_notifier/email.html
```

### Comparing `django-magic-notifier-0.2.2/docs/source/conf.py` & `django-magic-notifier-0.2.3/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'Django Magic Notifier'
 copyright = '2021, MATTON Jef'
 author = 'MATTON Jef'
 
 # The full version, including alpha/beta/rc tags
-release = '0.1.2'
+release = '0.2.3'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `django-magic-notifier-0.2.2/docs/source/index.rst` & `django-magic-notifier-0.2.3/docs/source/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,13 @@
 
    installation
    settings
    templates
    usage
    autoapi/index
 
-
-
 Indices and tables
 ==================
 
 * :ref:`genindex`
 * :ref:`modindex`
 * :ref:`search`
```

### Comparing `django-magic-notifier-0.2.2/docs/source/settings.rst` & `django-magic-notifier-0.2.3/docs/source/settings.rst`

 * *Files 10% similar despite different names*

```diff
@@ -133,7 +133,23 @@
         }
     }
 
 DMN needs a way to get a phone number from a User object. GET USER NUMBER must be path a function that accepts
 one parameter of type User. Default **`'magic_notifer.utils.get_user_number'`**::
 
     'GET_USER_NUMBER': 'path.to.function'
+
+NOTIFIER PUSH SETTINGS
+======================
+
+To connect to push notification websocket, a client must have a token.
+You need to specify a path to a function that returns a token given a
+User instance. The signature of the function must be::
+
+    def get_token_from_user(user) -> str:
+
+
+Setting example::
+
+    NOTIFIER = {
+        "USER_FROM_WS_TOKEN_FUNCTION": 'magic_notifier.utils.get_user_from_ws_token'
+    }
```

### Comparing `django-magic-notifier-0.2.2/docs/source/templates.rst` & `django-magic-notifier-0.2.3/docs/source/templates.rst`

 * *Files 18% similar despite different names*

```diff
@@ -9,16 +9,18 @@
 If your app name is **app_name** then create a directory **app_name/templates/notifier** 
 
 Now suppose you want to have a template named hello, then within the newly created
 folder created another folder like that **app_name/templates/notifier/hello**
 
 Now in this folder you have to create some files depending on how you will send your
 notifications. If you will send your notification via email then you must create
-two files within the hello folder named **email.html** and **email.txt**.
+two files within the hello folder named **email.html** and **email.txt** or **email.mjml**
+and **email**. Because DMN supports also mjml via 3rd party package.
 If you will send notifications via sms then you must create a file named **sms.txt**.
+If you want to send push notification then you must create a file **push.json**
 
 It is a common behavior to have a base template, you can do the same by creating a
 folder named **base** in the notifier folder and creating the files **email.html**,
 **email.txt** and **sms.txt**.
 
 Django Magic Notifier is shipped with some base templates that you can use. Let look
 at this example:
@@ -31,14 +33,18 @@
 
     {% extends "base_notifier/email.txt" %}
 
 *app_name/templates/notifier/base/sms.txt*::
 
     {% extends "base_notifier/sms.txt" %}
 
+*app_name/templates/notifier/base/push.json*::
+
+    {% extends "base_notifier/push.json" %}
+
 
 Now in the hello template folder, you do:
 
 *app_name/templates/notifier/hello/email.html*::
 
     {% extends "notifier/base/email.html" %}
     {% block content %}
@@ -46,19 +52,58 @@
         <td><p>Hello {{ user.email }}
         </td>
     </tr>
     {% endblock %}
 
 *app_name/templates/notifier/hello/email.txt*::
 
-    {% extends "notifier/hello/email.txt" %}
+    {% extends "notifier/base/email.txt" %}
     {% block content %}
     >Hello {{ user.email }}
     {% endblock %}
 
+*app_name/templates/notifier/hello/email.mjml*::
+
+    <mjml>
+      <mj-head>
+        <mj-attributes>
+          <mj-text align="center" color="#555" />
+        </mj-attributes>
+      </mj-head>
+      <mj-body background-color="#eee">
+        <mj-section>
+          <mj-column>
+            My Logo
+          </mj-column>
+        </mj-section>
+        <mj-section background-color="#fff">
+          <mj-column>
+            <mj-text align="center">
+              <h2>Welcome</h2>
+            </mj-text>
+            <mj-text>
+              Welcome to our company
+            </mj-text>
+          </mj-column>
+
+        </mj-section>
+        <mj-section>
+          <mj-column>
+            <mj-text> My Company </mj-text>
+            </mj-column>
+        </mj-section>
+      </mj-body>
+    </mjml>
+
+
 *app_name/templates/notifier/hello/sms.txt*::
 
-    {% extends "notifier/hello/sms.txt" %}
+    {% extends "notifier/base/sms.txt" %}
     {% block content %}
     >Hello {{ user.email }}
     {% endblock %}
 
+*app_name/templates/notifier/hello/push.json*::
+
+    {% extends "notifier/base/push.json" %}
+    {% block subject %}Hello {{ user.username }}{% endblock %}
+
```

### Comparing `django-magic-notifier-0.2.2/docs/source/usage.rst` & `django-magic-notifier-0.2.3/docs/source/usage.rst`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Send an email with a direct final string (no template) to a user instance::
 
     user = User(email="testuser@localhost", username="testuser")
     subject = "Test magic notifier"
     notify(["email"], subject, [user], final_message="Nice if you get this")
 
 
-Send an email with a template to a user instance::
+Send an email with a template (hello) to a user instance::
 
     user = User(email="testuser@localhost", username="testuser")
     subject = "Test magic notifier"
     notify(["email"], subject, [user], template='hello')
 
 
 Send an email with a template to all superuser::
@@ -67,7 +67,13 @@
 
 
 Send an email and sms with a template to all users excluding staff::
 
     user = User(email="testuser@localhost", username="testuser")
     subject = "Test magic notifier"
     notify(["email", 'sms'], subject, "all-staff", template='hello')
+
+Send an email, a sms and a push notification with a template to all users excluding staff::
+
+    user = User(email="testuser@localhost", username="testuser")
+    subject = "Test magic notifier"
+    notify(["email", 'sms', 'push'], subject, "all-staff", template='hello')
```

### Comparing `django-magic-notifier-0.2.2/magic_notifier/consumers.py` & `django-magic-notifier-0.2.3/magic_notifier/consumers.py`

 * *Files identical despite different names*

### Comparing `django-magic-notifier-0.2.2/magic_notifier/email_clients/django_email.py` & `django-magic-notifier-0.2.3/magic_notifier/email_clients/django_email.py`

 * *Files identical despite different names*

### Comparing `django-magic-notifier-0.2.2/magic_notifier/emailer.py` & `django-magic-notifier-0.2.3/magic_notifier/emailer.py`

 * *Files identical despite different names*

### Comparing `django-magic-notifier-0.2.2/magic_notifier/management/commands/test_email_template.py` & `django-magic-notifier-0.2.3/magic_notifier/management/commands/test_email_template.py`

 * *Files identical despite different names*

### Comparing `django-magic-notifier-0.2.2/magic_notifier/migrations/0001_initial.py` & `django-magic-notifier-0.2.3/magic_notifier/migrations/0001_initial.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,44 @@
-# Generated by Django 2.2.17 on 2021-07-23 21:30
+# Generated by Django 3.2.15 on 2023-07-11 09:46
 
-import django.db.models.deletion
 from django.conf import settings
 from django.db import migrations, models
-
-import magic_notifier.models
+import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
 
     initial = True
 
     dependencies = [
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
     ]
 
     operations = [
         migrations.CreateModel(
+            name='NotifyProfile',
+            fields=[
+                ('id', models.BigAutoField(primary_key=True, serialize=False)),
+                ('phone_number', models.CharField(blank=True, max_length=20, null=True)),
+                ('current_channel', models.CharField(blank=True, max_length=255, null=True)),
+                ('user', models.OneToOneField(on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL)),
+            ],
+        ),
+        migrations.CreateModel(
             name='Notification',
             fields=[
-                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('id', models.BigAutoField(primary_key=True, serialize=False)),
+                ('subject', models.CharField(blank=True, max_length=255, null=True)),
                 ('text', models.TextField()),
                 ('type', models.CharField(max_length=30)),
                 ('sub_type', models.CharField(blank=True, max_length=30, null=True)),
                 ('link', models.CharField(max_length=255, verbose_name='The link associated')),
-                ('image', models.ImageField(upload_to='notifications')),
-                ('actions', magic_notifier.models.JSONField(default=dict)),
-                ('data', magic_notifier.models.JSONField(default=dict)),
+                ('image', models.ImageField(blank=True, null=True, upload_to='notifications')),
+                ('actions', models.JSONField(default=dict)),
+                ('data', models.JSONField(default=dict)),
                 ('read', models.DateTimeField(blank=True, null=True)),
                 ('sent', models.DateTimeField(auto_now_add=True)),
                 ('mode', models.CharField(choices=[('user', 'User'), ('admin', 'Admin')], default='user', max_length=10)),
-                ('user', models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.CASCADE, related_name='notifications', to=settings.AUTH_USER_MODEL)),
+                ('user', models.ForeignKey(blank=True, null=True, on_delete=django.db.models.deletion.CASCADE, related_name='magic_notifications', to=settings.AUTH_USER_MODEL)),
             ],
         ),
     ]
```

### Comparing `django-magic-notifier-0.2.2/magic_notifier/models.py` & `django-magic-notifier-0.2.3/magic_notifier/models.py`

 * *Files identical despite different names*

### Comparing `django-magic-notifier-0.2.2/magic_notifier/notifier.py` & `django-magic-notifier-0.2.3/magic_notifier/notifier.py`

 * *Files identical despite different names*

### Comparing `django-magic-notifier-0.2.2/magic_notifier/pusher.py` & `django-magic-notifier-0.2.3/magic_notifier/pusher.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,29 +3,37 @@
 from threading import Thread
 
 from django.template.loader import render_to_string
 
 try:
     from asgiref.sync import async_to_sync
     from channels.layers import get_channel_layer
-except:
+except Exception:
     pass
 import json
 
 from django.template import Context, Template
 
 from magic_notifier.utils import NotificationBuilder
 
 logger = logging.getLogger("notif")
 
 
 class Pusher:
     def __init__(
         self, subject, receivers: list, template: str, context: dict, **kwargs
     ):
+        """
+
+        :param subject:The subject of the notification
+        :param receivers: The user list of receivers
+        :param template: The template to use
+        :param context:The context to pass to the template
+        :param kwargs:
+        """
         self.receivers: list = receivers
         self.template: str = template
         self.context: dict = context
         if 'subject' not in context and subject:
             self.context['subject'] = subject
         self.threaded: bool = kwargs.get("threaded", False)
         self.image = kwargs.get("image")
@@ -70,13 +78,13 @@
                 channel_layer = get_channel_layer()
                 async_to_sync(channel_layer.group_send)(
                     f"user-{user.id}",
                     event
                 )
 
                 return res
-        except:
+        except Exception as e:
             logger.error(traceback.format_exc())
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `django-magic-notifier-0.2.2/magic_notifier/settings.py` & `django-magic-notifier-0.2.3/magic_notifier/settings.py`

 * *Files identical despite different names*

### Comparing `django-magic-notifier-0.2.2/magic_notifier/sms_clients/cgsms_client.py` & `django-magic-notifier-0.2.3/magic_notifier/sms_clients/cgsms_client.py`

 * *Files identical despite different names*

### Comparing `django-magic-notifier-0.2.2/magic_notifier/sms_clients/nexa_client.py` & `django-magic-notifier-0.2.3/magic_notifier/sms_clients/nexa_client.py`

 * *Files identical despite different names*

### Comparing `django-magic-notifier-0.2.2/magic_notifier/smser.py` & `django-magic-notifier-0.2.3/magic_notifier/smser.py`

 * *Files identical despite different names*

### Comparing `django-magic-notifier-0.2.2/magic_notifier/templates/base_notifier/email.html` & `django-magic-notifier-0.2.3/magic_notifier/templates/base_notifier/email.html`

 * *Files identical despite different names*

### Comparing `django-magic-notifier-0.2.2/magic_notifier/templates/base_notifier/push.json` & `django-magic-notifier-0.2.3/magic_notifier/templates/base_notifier/push.json`

 * *Files identical despite different names*

### Comparing `django-magic-notifier-0.2.2/magic_notifier/utils.py` & `django-magic-notifier-0.2.3/magic_notifier/utils.py`

 * *Files identical despite different names*

### Comparing `django-magic-notifier-0.2.2/setup.py` & `django-magic-notifier-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'django-magic-notifier'
 DESCRIPTION = 'A notifications library for Djangonauts that support email, sms and push.'
 URL = 'https://github.com/jefcolbi/django-magic-notifier'
 EMAIL = 'jefcolbi@gmail.com'
 AUTHOR = 'jefcolbi'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.2.2'
+VERSION = '0.2.3'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'django>=2.2',
     'djangorestframework',
     'requests',
     'mjml-python'
```

### Comparing `django-magic-notifier-0.2.2/tests/connect.py` & `django-magic-notifier-0.2.3/tests/connect.py`

 * *Files identical despite different names*

### Comparing `django-magic-notifier-0.2.2/tests/core/templates/notifier/base/push.json` & `django-magic-notifier-0.2.3/tests/core/templates/notifier/base/push.json`

 * *Files identical despite different names*

### Comparing `django-magic-notifier-0.2.2/tests/core/tests.py` & `django-magic-notifier-0.2.3/tests/core/tests.py`

 * *Files identical despite different names*

### Comparing `django-magic-notifier-0.2.2/tests/example/asgi.py` & `django-magic-notifier-0.2.3/tests/example/asgi.py`

 * *Files identical despite different names*

### Comparing `django-magic-notifier-0.2.2/tests/example/settings.py` & `django-magic-notifier-0.2.3/tests/example/settings.py`

 * *Files identical despite different names*

### Comparing `django-magic-notifier-0.2.2/tests/example/urls.py` & `django-magic-notifier-0.2.3/tests/example/urls.py`

 * *Files identical despite different names*

### Comparing `django-magic-notifier-0.2.2/tests/manage.py` & `django-magic-notifier-0.2.3/tests/manage.py`

 * *Files identical despite different names*

