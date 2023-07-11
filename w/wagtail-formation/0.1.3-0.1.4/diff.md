# Comparing `tmp/wagtail_formation-0.1.3.tar.gz` & `tmp/wagtail_formation-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_formation-0.1.3.tar", last modified: Tue Mar 21 17:06:09 2023, max compression
+gzip compressed data, was "wagtail_formation-0.1.4.tar", last modified: Tue Jul 11 09:15:52 2023, max compression
```

## Comparing `wagtail_formation-0.1.3.tar` & `wagtail_formation-0.1.4.tar`

### file list

```diff
@@ -1,113 +1,114 @@
-drwxr-xr-x   0 m.westerhof (1120605082) 171460374        0 2023-03-21 17:06:09.774076 wagtail_formation-0.1.3/
--rw-r--r--   0 m.westerhof (1120605082) 171460374     3634 2023-03-06 10:30:05.000000 wagtail_formation-0.1.3/CONTRIBUTING.rst
--rw-r--r--   0 m.westerhof (1120605082) 171460374      273 2023-03-21 17:05:09.000000 wagtail_formation-0.1.3/HISTORY.rst
--rw-r--r--   0 m.westerhof (1120605082) 171460374     1074 2023-03-06 10:30:05.000000 wagtail_formation-0.1.3/LICENSE
--rw-r--r--   0 m.westerhof (1120605082) 171460374      272 2023-03-21 16:47:55.000000 wagtail_formation-0.1.3/MANIFEST.in
--rw-r--r--   0 m.westerhof (1120605082) 171460374     1947 2023-03-21 17:06:09.774164 wagtail_formation-0.1.3/PKG-INFO
--rw-r--r--   0 m.westerhof (1120605082) 171460374      953 2023-03-06 10:30:05.000000 wagtail_formation-0.1.3/README.rst
-drwxr-xr-x   0 m.westerhof (1120605082) 171460374        0 2023-03-21 17:06:09.753848 wagtail_formation-0.1.3/docs/
--rw-r--r--   0 m.westerhof (1120605082) 171460374       65 2023-03-06 16:36:34.000000 wagtail_formation-0.1.3/docs/Makefile
-drwxr-xr-x   0 m.westerhof (1120605082) 171460374        0 2023-03-21 17:06:09.745823 wagtail_formation-0.1.3/docs/docs/
-drwxr-xr-x   0 m.westerhof (1120605082) 171460374        0 2023-03-21 17:06:09.754996 wagtail_formation-0.1.3/docs/docs/images/
--rw-r--r--   0 m.westerhof (1120605082) 171460374    39962 2023-03-14 16:42:18.000000 wagtail_formation-0.1.3/docs/docs/images/simpleform_basic.png
--rw-r--r--   0 m.westerhof (1120605082) 171460374   475616 2023-03-14 16:43:07.000000 wagtail_formation-0.1.3/docs/docs/images/simpleform_silly.png
--rw-r--r--   0 m.westerhof (1120605082) 171460374   145908 2023-03-14 16:55:35.000000 wagtail_formation-0.1.3/docs/docs/images/simpleform_verysilly.png
-drwxr-xr-x   0 m.westerhof (1120605082) 171460374        0 2023-03-21 17:06:09.757653 wagtail_formation-0.1.3/formation/
--rw-r--r--   0 m.westerhof (1120605082) 171460374       22 2023-03-21 17:04:49.000000 wagtail_formation-0.1.3/formation/__init__.py
--rw-r--r--   0 m.westerhof (1120605082) 171460374      150 2023-03-06 10:32:38.000000 wagtail_formation-0.1.3/formation/apps.py
-drwxr-xr-x   0 m.westerhof (1120605082) 171460374        0 2023-03-21 17:06:09.758331 wagtail_formation-0.1.3/formation/blocks/
--rw-r--r--   0 m.westerhof (1120605082) 171460374      871 2023-03-06 10:32:38.000000 wagtail_formation-0.1.3/formation/blocks/__init__.py
--rw-r--r--   0 m.westerhof (1120605082) 171460374     4330 2023-03-17 13:06:55.000000 wagtail_formation-0.1.3/formation/blocks/fields.py
--rw-r--r--   0 m.westerhof (1120605082) 171460374     3349 2023-03-06 10:32:38.000000 wagtail_formation-0.1.3/formation/blocks/forms.py
-drwxr-xr-x   0 m.westerhof (1120605082) 171460374        0 2023-03-21 17:06:09.759071 wagtail_formation-0.1.3/formation/migrations/
--rw-r--r--   0 m.westerhof (1120605082) 171460374      545 2023-03-06 10:32:38.000000 wagtail_formation-0.1.3/formation/migrations/0001_initial.py
--rw-r--r--   0 m.westerhof (1120605082) 171460374     2460 2023-03-06 10:32:38.000000 wagtail_formation-0.1.3/formation/migrations/0002_reusableform_name_alter_reusableform_form_content.py
--rw-r--r--   0 m.westerhof (1120605082) 171460374        0 2023-03-06 10:32:38.000000 wagtail_formation-0.1.3/formation/migrations/__init__.py
--rw-r--r--   0 m.westerhof (1120605082) 171460374      458 2023-03-17 13:03:47.000000 wagtail_formation-0.1.3/formation/models.py
-drwxr-xr-x   0 m.westerhof (1120605082) 171460374        0 2023-03-21 17:06:09.746873 wagtail_formation-0.1.3/formation/static/
-drwxr-xr-x   0 m.westerhof (1120605082) 171460374        0 2023-03-21 17:06:09.759258 wagtail_formation-0.1.3/formation/static/js/
--rw-r--r--   0 m.westerhof (1120605082) 171460374      712 2023-03-15 14:38:38.000000 wagtail_formation-0.1.3/formation/static/js/formation.js
-drwxr-xr-x   0 m.westerhof (1120605082) 171460374        0 2023-03-21 17:06:09.747250 wagtail_formation-0.1.3/formation/templates/
-drwxr-xr-x   0 m.westerhof (1120605082) 171460374        0 2023-03-21 17:06:09.759498 wagtail_formation-0.1.3/formation/templates/formation/
-drwxr-xr-x   0 m.westerhof (1120605082) 171460374        0 2023-03-21 17:06:09.762582 wagtail_formation-0.1.3/formation/templates/formation/blocks/
--rw-r--r--   0 m.westerhof (1120605082) 171460374      392 2023-03-06 10:32:38.000000 wagtail_formation-0.1.3/formation/templates/formation/blocks/base_field.html
--rw-r--r--   0 m.westerhof (1120605082) 171460374      343 2023-03-15 15:40:24.000000 wagtail_formation-0.1.3/formation/templates/formation/blocks/base_form.html
--rw-r--r--   0 m.westerhof (1120605082) 171460374      182 2023-03-06 10:32:38.000000 wagtail_formation-0.1.3/formation/templates/formation/blocks/boolean_field.html
--rw-r--r--   0 m.westerhof (1120605082) 171460374      178 2023-03-06 10:32:38.000000 wagtail_formation-0.1.3/formation/templates/formation/blocks/date_field.html
--rw-r--r--   0 m.westerhof (1120605082) 171460374      188 2023-03-06 10:32:38.000000 wagtail_formation-0.1.3/formation/templates/formation/blocks/datetime_field.html
--rw-r--r--   0 m.westerhof (1120605082) 171460374      178 2023-03-06 10:32:38.000000 wagtail_formation-0.1.3/formation/templates/formation/blocks/email_field.html
--rw-r--r--   0 m.westerhof (1120605082) 171460374      180 2023-03-06 10:32:38.000000 wagtail_formation-0.1.3/formation/templates/formation/blocks/integer_field.html
--rw-r--r--   0 m.westerhof (1120605082) 171460374      439 2023-03-06 10:32:38.000000 wagtail_formation-0.1.3/formation/templates/formation/blocks/radio_field.html
--rw-r--r--   0 m.westerhof (1120605082) 171460374      269 2023-03-06 10:32:38.000000 wagtail_formation-0.1.3/formation/templates/formation/blocks/select_field.html
--rw-r--r--   0 m.westerhof (1120605082) 171460374       66 2023-03-06 10:32:38.000000 wagtail_formation-0.1.3/formation/templates/formation/blocks/submit_button.html
--rw-r--r--   0 m.westerhof (1120605082) 171460374      178 2023-03-06 10:32:38.000000 wagtail_formation-0.1.3/formation/templates/formation/blocks/text_field.html
--rw-r--r--   0 m.westerhof (1120605082) 171460374      169 2023-03-06 10:32:38.000000 wagtail_formation-0.1.3/formation/templates/formation/blocks/textarea_field.html
--rw-r--r--   0 m.westerhof (1120605082) 171460374      121 2023-03-06 10:32:38.000000 wagtail_formation-0.1.3/formation/templates/formation/reusable_form.html
-drwxr-xr-x   0 m.westerhof (1120605082) 171460374        0 2023-03-21 17:06:09.763082 wagtail_formation-0.1.3/formation/templatetags/
--rw-r--r--   0 m.westerhof (1120605082) 171460374        0 2023-03-06 10:32:38.000000 wagtail_formation-0.1.3/formation/templatetags/__init__.py
--rw-r--r--   0 m.westerhof (1120605082) 171460374      729 2023-03-15 15:40:50.000000 wagtail_formation-0.1.3/formation/templatetags/formation_tags.py
--rw-r--r--   0 m.westerhof (1120605082) 171460374      190 2023-03-15 14:42:53.000000 wagtail_formation-0.1.3/formation/urls.py
--rw-r--r--   0 m.westerhof (1120605082) 171460374     2917 2023-03-17 13:04:05.000000 wagtail_formation-0.1.3/formation/utils.py
--rw-r--r--   0 m.westerhof (1120605082) 171460374     1169 2023-03-06 10:32:38.000000 wagtail_formation-0.1.3/formation/views.py
--rw-r--r--   0 m.westerhof (1120605082) 171460374      464 2023-03-06 10:32:38.000000 wagtail_formation-0.1.3/formation/wagtail_hooks.py
--rw-r--r--   0 m.westerhof (1120605082) 171460374      366 2023-03-06 10:32:38.000000 wagtail_formation-0.1.3/formation/widgets.py
--rw-r--r--   0 m.westerhof (1120605082) 171460374      429 2023-03-21 17:06:09.775681 wagtail_formation-0.1.3/setup.cfg
--rw-r--r--   0 m.westerhof (1120605082) 171460374     1347 2023-03-21 17:04:54.000000 wagtail_formation-0.1.3/setup.py
-drwxr-xr-x   0 m.westerhof (1120605082) 171460374        0 2023-03-21 17:06:09.763402 wagtail_formation-0.1.3/tests/
--rw-r--r--   0 m.westerhof (1120605082) 171460374       47 2023-03-06 10:30:05.000000 wagtail_formation-0.1.3/tests/__init__.py
-drwxr-xr-x   0 m.westerhof (1120605082) 171460374        0 2023-03-21 17:06:09.764699 wagtail_formation-0.1.3/tests/testproject/
--rw-r--r--   0 m.westerhof (1120605082) 171460374      376 2023-03-17 08:55:07.000000 wagtail_formation-0.1.3/tests/testproject/.dockerignore
--rw-r--r--   0 m.westerhof (1120605082) 171460374     2034 2023-03-17 08:55:07.000000 wagtail_formation-0.1.3/tests/testproject/Dockerfile
-drwxr-xr-x   0 m.westerhof (1120605082) 171460374        0 2023-03-21 17:06:09.765460 wagtail_formation-0.1.3/tests/testproject/home/
--rw-r--r--   0 m.westerhof (1120605082) 171460374        0 2023-03-17 08:55:07.000000 wagtail_formation-0.1.3/tests/testproject/home/__init__.py
--rw-r--r--   0 m.westerhof (1120605082) 171460374     1048 2023-03-17 09:56:24.000000 wagtail_formation-0.1.3/tests/testproject/home/blocks.py
-drwxr-xr-x   0 m.westerhof (1120605082) 171460374        0 2023-03-21 17:06:09.766371 wagtail_formation-0.1.3/tests/testproject/home/migrations/
--rw-r--r--   0 m.westerhof (1120605082) 171460374      830 2023-03-17 08:55:07.000000 wagtail_formation-0.1.3/tests/testproject/home/migrations/0001_initial.py
--rw-r--r--   0 m.westerhof (1120605082) 171460374     1741 2023-03-17 11:53:14.000000 wagtail_formation-0.1.3/tests/testproject/home/migrations/0002_create_homepage.py
--rw-r--r--   0 m.westerhof (1120605082) 171460374     1306 2023-03-17 11:57:04.000000 wagtail_formation-0.1.3/tests/testproject/home/migrations/0003_homepage_content.py
--rw-r--r--   0 m.westerhof (1120605082) 171460374        0 2023-03-17 08:55:07.000000 wagtail_formation-0.1.3/tests/testproject/home/migrations/__init__.py
--rw-r--r--   0 m.westerhof (1120605082) 171460374      392 2023-03-17 09:55:52.000000 wagtail_formation-0.1.3/tests/testproject/home/models.py
-drwxr-xr-x   0 m.westerhof (1120605082) 171460374        0 2023-03-21 17:06:09.749010 wagtail_formation-0.1.3/tests/testproject/home/static/
-drwxr-xr-x   0 m.westerhof (1120605082) 171460374        0 2023-03-21 17:06:09.766545 wagtail_formation-0.1.3/tests/testproject/home/static/css/
--rw-r--r--   0 m.westerhof (1120605082) 171460374     2522 2023-03-17 08:55:07.000000 wagtail_formation-0.1.3/tests/testproject/home/static/css/welcome_page.css
-drwxr-xr-x   0 m.westerhof (1120605082) 171460374        0 2023-03-21 17:06:09.749368 wagtail_formation-0.1.3/tests/testproject/home/templates/
-drwxr-xr-x   0 m.westerhof (1120605082) 171460374        0 2023-03-21 17:06:09.767109 wagtail_formation-0.1.3/tests/testproject/home/templates/home/
--rw-r--r--   0 m.westerhof (1120605082) 171460374      232 2023-03-17 12:27:18.000000 wagtail_formation-0.1.3/tests/testproject/home/templates/home/home_page.html
--rw-r--r--   0 m.westerhof (1120605082) 171460374     6421 2023-03-17 08:55:07.000000 wagtail_formation-0.1.3/tests/testproject/home/templates/home/welcome_page.html
--rwxr-xr-x   0 m.westerhof (1120605082) 171460374      388 2023-03-17 09:40:47.000000 wagtail_formation-0.1.3/tests/testproject/manage.py
--rw-r--r--   0 m.westerhof (1120605082) 171460374       35 2023-03-17 08:55:07.000000 wagtail_formation-0.1.3/tests/testproject/requirements.txt
-drwxr-xr-x   0 m.westerhof (1120605082) 171460374        0 2023-03-21 17:06:09.767541 wagtail_formation-0.1.3/tests/testproject/search/
--rw-r--r--   0 m.westerhof (1120605082) 171460374        0 2023-03-17 08:55:07.000000 wagtail_formation-0.1.3/tests/testproject/search/__init__.py
-drwxr-xr-x   0 m.westerhof (1120605082) 171460374        0 2023-03-21 17:06:09.749944 wagtail_formation-0.1.3/tests/testproject/search/templates/
-drwxr-xr-x   0 m.westerhof (1120605082) 171460374        0 2023-03-21 17:06:09.767755 wagtail_formation-0.1.3/tests/testproject/search/templates/search/
--rw-r--r--   0 m.westerhof (1120605082) 171460374     1097 2023-03-17 08:55:07.000000 wagtail_formation-0.1.3/tests/testproject/search/templates/search/search.html
--rw-r--r--   0 m.westerhof (1120605082) 171460374     1019 2023-03-17 08:55:07.000000 wagtail_formation-0.1.3/tests/testproject/search/views.py
--rw-r--r--   0 m.westerhof (1120605082) 171460374      662 2023-03-17 12:18:02.000000 wagtail_formation-0.1.3/tests/testproject/testbed.json
-drwxr-xr-x   0 m.westerhof (1120605082) 171460374        0 2023-03-21 17:06:09.768362 wagtail_formation-0.1.3/tests/testproject/testproject/
--rw-r--r--   0 m.westerhof (1120605082) 171460374        0 2023-03-17 08:55:07.000000 wagtail_formation-0.1.3/tests/testproject/testproject/__init__.py
-drwxr-xr-x   0 m.westerhof (1120605082) 171460374        0 2023-03-21 17:06:09.769186 wagtail_formation-0.1.3/tests/testproject/testproject/settings/
--rw-r--r--   0 m.westerhof (1120605082) 171460374        0 2023-03-17 08:55:07.000000 wagtail_formation-0.1.3/tests/testproject/testproject/settings/__init__.py
--rw-r--r--   0 m.westerhof (1120605082) 171460374     4510 2023-03-17 12:33:26.000000 wagtail_formation-0.1.3/tests/testproject/testproject/settings/base.py
--rw-r--r--   0 m.westerhof (1120605082) 171460374      460 2023-03-17 08:55:07.000000 wagtail_formation-0.1.3/tests/testproject/testproject/settings/dev.py
--rw-r--r--   0 m.westerhof (1120605082) 171460374       95 2023-03-17 08:55:07.000000 wagtail_formation-0.1.3/tests/testproject/testproject/settings/production.py
-drwxr-xr-x   0 m.westerhof (1120605082) 171460374        0 2023-03-21 17:06:09.750899 wagtail_formation-0.1.3/tests/testproject/testproject/static/
-drwxr-xr-x   0 m.westerhof (1120605082) 171460374        0 2023-03-21 17:06:09.769392 wagtail_formation-0.1.3/tests/testproject/testproject/static/css/
--rw-r--r--   0 m.westerhof (1120605082) 171460374        0 2023-03-17 08:55:07.000000 wagtail_formation-0.1.3/tests/testproject/testproject/static/css/testproject.css
-drwxr-xr-x   0 m.westerhof (1120605082) 171460374        0 2023-03-21 17:06:09.769567 wagtail_formation-0.1.3/tests/testproject/testproject/static/js/
--rw-r--r--   0 m.westerhof (1120605082) 171460374        0 2023-03-17 08:55:07.000000 wagtail_formation-0.1.3/tests/testproject/testproject/static/js/testproject.js
-drwxr-xr-x   0 m.westerhof (1120605082) 171460374        0 2023-03-21 17:06:09.770182 wagtail_formation-0.1.3/tests/testproject/testproject/templates/
--rw-r--r--   0 m.westerhof (1120605082) 171460374      230 2023-03-17 08:55:07.000000 wagtail_formation-0.1.3/tests/testproject/testproject/templates/404.html
--rw-r--r--   0 m.westerhof (1120605082) 171460374      369 2023-03-17 08:55:07.000000 wagtail_formation-0.1.3/tests/testproject/testproject/templates/500.html
--rw-r--r--   0 m.westerhof (1120605082) 171460374     1607 2023-03-17 12:27:41.000000 wagtail_formation-0.1.3/tests/testproject/testproject/templates/base.html
-drwxr-xr-x   0 m.westerhof (1120605082) 171460374        0 2023-03-21 17:06:09.770559 wagtail_formation-0.1.3/tests/testproject/testproject/tests/
--rw-r--r--   0 m.westerhof (1120605082) 171460374        0 2023-03-17 09:47:40.000000 wagtail_formation-0.1.3/tests/testproject/testproject/tests/__init__.py
--rw-r--r--   0 m.westerhof (1120605082) 171460374     1289 2023-03-17 12:55:57.000000 wagtail_formation-0.1.3/tests/testproject/testproject/tests/test_basic.py
--rw-r--r--   0 m.westerhof (1120605082) 171460374     1340 2023-03-17 12:13:58.000000 wagtail_formation-0.1.3/tests/testproject/testproject/urls.py
--rw-r--r--   0 m.westerhof (1120605082) 171460374      403 2023-03-17 08:55:07.000000 wagtail_formation-0.1.3/tests/testproject/testproject/wsgi.py
-drwxr-xr-x   0 m.westerhof (1120605082) 171460374        0 2023-03-21 17:06:09.773938 wagtail_formation-0.1.3/wagtail_formation.egg-info/
--rw-r--r--   0 m.westerhof (1120605082) 171460374     1947 2023-03-21 17:06:09.000000 wagtail_formation-0.1.3/wagtail_formation.egg-info/PKG-INFO
--rw-r--r--   0 m.westerhof (1120605082) 171460374     3108 2023-03-21 17:06:09.000000 wagtail_formation-0.1.3/wagtail_formation.egg-info/SOURCES.txt
--rw-r--r--   0 m.westerhof (1120605082) 171460374        1 2023-03-21 17:06:09.000000 wagtail_formation-0.1.3/wagtail_formation.egg-info/dependency_links.txt
--rw-r--r--   0 m.westerhof (1120605082) 171460374        1 2023-03-21 17:06:09.000000 wagtail_formation-0.1.3/wagtail_formation.egg-info/not-zip-safe
--rw-r--r--   0 m.westerhof (1120605082) 171460374       52 2023-03-21 17:06:09.000000 wagtail_formation-0.1.3/wagtail_formation.egg-info/requires.txt
--rw-r--r--   0 m.westerhof (1120605082) 171460374       10 2023-03-21 17:06:09.000000 wagtail_formation-0.1.3/wagtail_formation.egg-info/top_level.txt
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.319411 wagtail_formation-0.1.4/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     3634 2023-03-06 10:30:05.000000 wagtail_formation-0.1.4/CONTRIBUTING.rst
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      336 2023-07-11 08:36:32.000000 wagtail_formation-0.1.4/HISTORY.rst
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1074 2023-03-06 10:30:05.000000 wagtail_formation-0.1.4/LICENSE
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      272 2023-03-21 16:47:55.000000 wagtail_formation-0.1.4/MANIFEST.in
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1672 2023-07-11 09:15:52.319494 wagtail_formation-0.1.4/PKG-INFO
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      953 2023-03-06 10:30:05.000000 wagtail_formation-0.1.4/README.rst
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.288680 wagtail_formation-0.1.4/docs/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)       65 2023-03-06 16:36:34.000000 wagtail_formation-0.1.4/docs/Makefile
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.280991 wagtail_formation-0.1.4/docs/docs/
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.293606 wagtail_formation-0.1.4/docs/docs/images/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)    39962 2023-03-14 16:42:18.000000 wagtail_formation-0.1.4/docs/docs/images/simpleform_basic.png
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)   475616 2023-03-14 16:43:07.000000 wagtail_formation-0.1.4/docs/docs/images/simpleform_silly.png
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)   145908 2023-03-14 16:55:35.000000 wagtail_formation-0.1.4/docs/docs/images/simpleform_verysilly.png
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.297576 wagtail_formation-0.1.4/formation/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)       22 2023-07-11 08:32:24.000000 wagtail_formation-0.1.4/formation/__init__.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      150 2023-03-06 10:32:38.000000 wagtail_formation-0.1.4/formation/apps.py
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.298719 wagtail_formation-0.1.4/formation/blocks/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      871 2023-03-06 10:32:38.000000 wagtail_formation-0.1.4/formation/blocks/__init__.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     4330 2023-07-11 08:29:47.000000 wagtail_formation-0.1.4/formation/blocks/fields.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     3349 2023-07-11 08:29:47.000000 wagtail_formation-0.1.4/formation/blocks/forms.py
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.299948 wagtail_formation-0.1.4/formation/migrations/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      545 2023-03-06 10:32:38.000000 wagtail_formation-0.1.4/formation/migrations/0001_initial.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     2460 2023-03-06 10:32:38.000000 wagtail_formation-0.1.4/formation/migrations/0002_reusableform_name_alter_reusableform_form_content.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      465 2023-06-30 08:58:46.000000 wagtail_formation-0.1.4/formation/migrations/0003_alter_reusableform_form_content.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-03-06 10:32:38.000000 wagtail_formation-0.1.4/formation/migrations/__init__.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      457 2023-06-30 08:57:28.000000 wagtail_formation-0.1.4/formation/models.py
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.281555 wagtail_formation-0.1.4/formation/static/
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.300130 wagtail_formation-0.1.4/formation/static/js/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      712 2023-03-15 14:38:38.000000 wagtail_formation-0.1.4/formation/static/js/formation.js
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.281749 wagtail_formation-0.1.4/formation/templates/
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.300609 wagtail_formation-0.1.4/formation/templates/formation/
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.303673 wagtail_formation-0.1.4/formation/templates/formation/blocks/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      392 2023-03-06 10:32:38.000000 wagtail_formation-0.1.4/formation/templates/formation/blocks/base_field.html
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      343 2023-07-11 08:29:47.000000 wagtail_formation-0.1.4/formation/templates/formation/blocks/base_form.html
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      182 2023-03-06 10:32:38.000000 wagtail_formation-0.1.4/formation/templates/formation/blocks/boolean_field.html
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      178 2023-03-06 10:32:38.000000 wagtail_formation-0.1.4/formation/templates/formation/blocks/date_field.html
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      188 2023-03-06 10:32:38.000000 wagtail_formation-0.1.4/formation/templates/formation/blocks/datetime_field.html
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      178 2023-03-06 10:32:38.000000 wagtail_formation-0.1.4/formation/templates/formation/blocks/email_field.html
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      180 2023-03-06 10:32:38.000000 wagtail_formation-0.1.4/formation/templates/formation/blocks/integer_field.html
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      439 2023-03-06 10:32:38.000000 wagtail_formation-0.1.4/formation/templates/formation/blocks/radio_field.html
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      269 2023-03-06 10:32:38.000000 wagtail_formation-0.1.4/formation/templates/formation/blocks/select_field.html
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)       66 2023-03-06 10:32:38.000000 wagtail_formation-0.1.4/formation/templates/formation/blocks/submit_button.html
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      178 2023-03-06 10:32:38.000000 wagtail_formation-0.1.4/formation/templates/formation/blocks/text_field.html
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      169 2023-03-06 10:32:38.000000 wagtail_formation-0.1.4/formation/templates/formation/blocks/textarea_field.html
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      121 2023-03-06 10:32:38.000000 wagtail_formation-0.1.4/formation/templates/formation/reusable_form.html
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.304419 wagtail_formation-0.1.4/formation/templatetags/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-03-06 10:32:38.000000 wagtail_formation-0.1.4/formation/templatetags/__init__.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      729 2023-03-15 15:40:50.000000 wagtail_formation-0.1.4/formation/templatetags/formation_tags.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      190 2023-03-15 14:42:53.000000 wagtail_formation-0.1.4/formation/urls.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     2917 2023-03-17 13:04:05.000000 wagtail_formation-0.1.4/formation/utils.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1169 2023-06-30 12:51:44.000000 wagtail_formation-0.1.4/formation/views.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      464 2023-03-06 10:32:38.000000 wagtail_formation-0.1.4/formation/wagtail_hooks.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      366 2023-03-06 10:32:38.000000 wagtail_formation-0.1.4/formation/widgets.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      429 2023-07-11 09:15:52.321385 wagtail_formation-0.1.4/setup.cfg
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1328 2023-07-11 09:13:33.000000 wagtail_formation-0.1.4/setup.py
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.304747 wagtail_formation-0.1.4/tests/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)       47 2023-03-06 10:30:05.000000 wagtail_formation-0.1.4/tests/__init__.py
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.306627 wagtail_formation-0.1.4/tests/testproject/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      376 2023-03-17 08:55:07.000000 wagtail_formation-0.1.4/tests/testproject/.dockerignore
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     2034 2023-03-17 08:55:07.000000 wagtail_formation-0.1.4/tests/testproject/Dockerfile
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.307628 wagtail_formation-0.1.4/tests/testproject/home/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-03-17 08:55:07.000000 wagtail_formation-0.1.4/tests/testproject/home/__init__.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1048 2023-03-17 09:56:24.000000 wagtail_formation-0.1.4/tests/testproject/home/blocks.py
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.308869 wagtail_formation-0.1.4/tests/testproject/home/migrations/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      830 2023-03-17 08:55:07.000000 wagtail_formation-0.1.4/tests/testproject/home/migrations/0001_initial.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1741 2023-03-17 11:53:14.000000 wagtail_formation-0.1.4/tests/testproject/home/migrations/0002_create_homepage.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1306 2023-03-17 11:57:04.000000 wagtail_formation-0.1.4/tests/testproject/home/migrations/0003_homepage_content.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-03-17 08:55:07.000000 wagtail_formation-0.1.4/tests/testproject/home/migrations/__init__.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      392 2023-03-17 09:55:52.000000 wagtail_formation-0.1.4/tests/testproject/home/models.py
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.282860 wagtail_formation-0.1.4/tests/testproject/home/static/
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.309146 wagtail_formation-0.1.4/tests/testproject/home/static/css/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     2522 2023-03-17 08:55:07.000000 wagtail_formation-0.1.4/tests/testproject/home/static/css/welcome_page.css
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.283098 wagtail_formation-0.1.4/tests/testproject/home/templates/
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.309823 wagtail_formation-0.1.4/tests/testproject/home/templates/home/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      232 2023-03-17 12:27:18.000000 wagtail_formation-0.1.4/tests/testproject/home/templates/home/home_page.html
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     6421 2023-03-17 08:55:07.000000 wagtail_formation-0.1.4/tests/testproject/home/templates/home/welcome_page.html
+-rwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      388 2023-03-17 09:40:47.000000 wagtail_formation-0.1.4/tests/testproject/manage.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)       35 2023-03-17 08:55:07.000000 wagtail_formation-0.1.4/tests/testproject/requirements.txt
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.310735 wagtail_formation-0.1.4/tests/testproject/search/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-03-17 08:55:07.000000 wagtail_formation-0.1.4/tests/testproject/search/__init__.py
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.283548 wagtail_formation-0.1.4/tests/testproject/search/templates/
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.311258 wagtail_formation-0.1.4/tests/testproject/search/templates/search/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1097 2023-03-17 08:55:07.000000 wagtail_formation-0.1.4/tests/testproject/search/templates/search/search.html
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1019 2023-03-17 08:55:07.000000 wagtail_formation-0.1.4/tests/testproject/search/views.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      662 2023-03-17 12:18:02.000000 wagtail_formation-0.1.4/tests/testproject/testbed.json
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.312126 wagtail_formation-0.1.4/tests/testproject/testproject/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-03-17 08:55:07.000000 wagtail_formation-0.1.4/tests/testproject/testproject/__init__.py
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.313093 wagtail_formation-0.1.4/tests/testproject/testproject/settings/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-03-17 08:55:07.000000 wagtail_formation-0.1.4/tests/testproject/testproject/settings/__init__.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     4510 2023-03-17 12:33:26.000000 wagtail_formation-0.1.4/tests/testproject/testproject/settings/base.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      460 2023-03-17 08:55:07.000000 wagtail_formation-0.1.4/tests/testproject/testproject/settings/dev.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)       95 2023-03-17 08:55:07.000000 wagtail_formation-0.1.4/tests/testproject/testproject/settings/production.py
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.284369 wagtail_formation-0.1.4/tests/testproject/testproject/static/
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.313320 wagtail_formation-0.1.4/tests/testproject/testproject/static/css/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-03-17 08:55:07.000000 wagtail_formation-0.1.4/tests/testproject/testproject/static/css/testproject.css
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.313529 wagtail_formation-0.1.4/tests/testproject/testproject/static/js/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-03-17 08:55:07.000000 wagtail_formation-0.1.4/tests/testproject/testproject/static/js/testproject.js
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.314307 wagtail_formation-0.1.4/tests/testproject/testproject/templates/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      230 2023-03-17 08:55:07.000000 wagtail_formation-0.1.4/tests/testproject/testproject/templates/404.html
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      369 2023-03-17 08:55:07.000000 wagtail_formation-0.1.4/tests/testproject/testproject/templates/500.html
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1607 2023-03-17 12:27:41.000000 wagtail_formation-0.1.4/tests/testproject/testproject/templates/base.html
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.314830 wagtail_formation-0.1.4/tests/testproject/testproject/tests/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-03-17 09:47:40.000000 wagtail_formation-0.1.4/tests/testproject/testproject/tests/__init__.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1289 2023-03-17 12:55:57.000000 wagtail_formation-0.1.4/tests/testproject/testproject/tests/test_basic.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1340 2023-03-17 12:13:58.000000 wagtail_formation-0.1.4/tests/testproject/testproject/urls.py
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)      403 2023-03-17 08:55:07.000000 wagtail_formation-0.1.4/tests/testproject/testproject/wsgi.py
+drwxr-xr-x   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        0 2023-07-11 09:15:52.319298 wagtail_formation-0.1.4/wagtail_formation.egg-info/
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     1672 2023-07-11 09:15:52.000000 wagtail_formation-0.1.4/wagtail_formation.egg-info/PKG-INFO
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)     3169 2023-07-11 09:15:52.000000 wagtail_formation-0.1.4/wagtail_formation.egg-info/SOURCES.txt
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        1 2023-07-11 09:15:52.000000 wagtail_formation-0.1.4/wagtail_formation.egg-info/dependency_links.txt
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)        1 2023-07-11 09:15:52.000000 wagtail_formation-0.1.4/wagtail_formation.egg-info/not-zip-safe
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)       52 2023-07-11 09:15:52.000000 wagtail_formation-0.1.4/wagtail_formation.egg-info/requires.txt
+-rw-r--r--   0 m.westerhof (1120605082) LUKKIEN0\Domain Users (171460374)       10 2023-07-11 09:15:52.000000 wagtail_formation-0.1.4/wagtail_formation.egg-info/top_level.txt
```

### Comparing `wagtail_formation-0.1.3/CONTRIBUTING.rst` & `wagtail_formation-0.1.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.3/LICENSE` & `wagtail_formation-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.3/PKG-INFO` & `wagtail_formation-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail_formation
-Version: 0.1.3
+Version: 0.1.4
 Summary: Build forms from wagtail blocks
 Home-page: https://github.com/mwesterhof/wagtail_formation
 Author: Marco Westerhof
 Author-email: m.westerhof@lukkien.com
 License: MIT license
 Keywords: wagtail_formation
 Platform: UNKNOWN
@@ -54,32 +54,7 @@
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
-=======
-History
-=======
-
-0.1.3 (2023-03-21)
-------------------
-
-* fix package dir
-
-0.1.2 (2023-03-21)
-------------------
-
-* fix manifest
-
-0.1.1 (2023-03-17)
-------------------
-
-* Testing and some refactoring
-
-0.1.0 (2023-03-06)
-------------------
-
-* First release on PyPI.
-
-
```

### Comparing `wagtail_formation-0.1.3/README.rst` & `wagtail_formation-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.3/docs/docs/images/simpleform_basic.png` & `wagtail_formation-0.1.4/docs/docs/images/simpleform_basic.png`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.3/docs/docs/images/simpleform_silly.png` & `wagtail_formation-0.1.4/docs/docs/images/simpleform_silly.png`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.3/docs/docs/images/simpleform_verysilly.png` & `wagtail_formation-0.1.4/docs/docs/images/simpleform_verysilly.png`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.3/formation/blocks/__init__.py` & `wagtail_formation-0.1.4/formation/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.3/formation/blocks/fields.py` & `wagtail_formation-0.1.4/formation/blocks/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.3/formation/blocks/forms.py` & `wagtail_formation-0.1.4/formation/blocks/forms.py`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.3/formation/migrations/0001_initial.py` & `wagtail_formation-0.1.4/formation/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.3/formation/migrations/0002_reusableform_name_alter_reusableform_form_content.py` & `wagtail_formation-0.1.4/formation/migrations/0002_reusableform_name_alter_reusableform_form_content.py`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.3/formation/static/js/formation.js` & `wagtail_formation-0.1.4/formation/static/js/formation.js`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.3/formation/templatetags/formation_tags.py` & `wagtail_formation-0.1.4/formation/templatetags/formation_tags.py`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.3/formation/utils.py` & `wagtail_formation-0.1.4/formation/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.3/formation/views.py` & `wagtail_formation-0.1.4/formation/views.py`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.3/setup.py` & `wagtail_formation-0.1.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,18 +31,18 @@
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
     ],
     description="Build forms from wagtail blocks",
     install_requires=requirements,
     license="MIT license",
-    long_description=readme + '\n\n' + history,
+    long_description=readme,
     include_package_data=True,
     keywords='wagtail_formation',
     name='wagtail_formation',
     packages=find_packages(include=['formation', 'formation.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/mwesterhof/wagtail_formation',
-    version='0.1.3',
+    version='0.1.4',
     zip_safe=False,
 )
```

### Comparing `wagtail_formation-0.1.3/tests/testproject/Dockerfile` & `wagtail_formation-0.1.4/tests/testproject/Dockerfile`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.3/tests/testproject/home/blocks.py` & `wagtail_formation-0.1.4/tests/testproject/home/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.3/tests/testproject/home/migrations/0001_initial.py` & `wagtail_formation-0.1.4/tests/testproject/home/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.3/tests/testproject/home/migrations/0002_create_homepage.py` & `wagtail_formation-0.1.4/tests/testproject/home/migrations/0002_create_homepage.py`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.3/tests/testproject/home/migrations/0003_homepage_content.py` & `wagtail_formation-0.1.4/tests/testproject/home/migrations/0003_homepage_content.py`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.3/tests/testproject/home/static/css/welcome_page.css` & `wagtail_formation-0.1.4/tests/testproject/home/static/css/welcome_page.css`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.3/tests/testproject/home/templates/home/welcome_page.html` & `wagtail_formation-0.1.4/tests/testproject/home/templates/home/welcome_page.html`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.3/tests/testproject/search/templates/search/search.html` & `wagtail_formation-0.1.4/tests/testproject/search/templates/search/search.html`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.3/tests/testproject/search/views.py` & `wagtail_formation-0.1.4/tests/testproject/search/views.py`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.3/tests/testproject/testbed.json` & `wagtail_formation-0.1.4/tests/testproject/testbed.json`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.3/tests/testproject/testproject/settings/base.py` & `wagtail_formation-0.1.4/tests/testproject/testproject/settings/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.3/tests/testproject/testproject/templates/base.html` & `wagtail_formation-0.1.4/tests/testproject/testproject/templates/base.html`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.3/tests/testproject/testproject/tests/test_basic.py` & `wagtail_formation-0.1.4/tests/testproject/testproject/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.3/tests/testproject/testproject/urls.py` & `wagtail_formation-0.1.4/tests/testproject/testproject/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_formation-0.1.3/wagtail_formation.egg-info/PKG-INFO` & `wagtail_formation-0.1.4/wagtail_formation.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-formation
-Version: 0.1.3
+Version: 0.1.4
 Summary: Build forms from wagtail blocks
 Home-page: https://github.com/mwesterhof/wagtail_formation
 Author: Marco Westerhof
 Author-email: m.westerhof@lukkien.com
 License: MIT license
 Keywords: wagtail_formation
 Platform: UNKNOWN
@@ -54,32 +54,7 @@
 
 This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
 
 .. _Cookiecutter: https://github.com/audreyr/cookiecutter
 .. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
 
 
-=======
-History
-=======
-
-0.1.3 (2023-03-21)
-------------------
-
-* fix package dir
-
-0.1.2 (2023-03-21)
-------------------
-
-* fix manifest
-
-0.1.1 (2023-03-17)
-------------------
-
-* Testing and some refactoring
-
-0.1.0 (2023-03-06)
-------------------
-
-* First release on PyPI.
-
-
```

### Comparing `wagtail_formation-0.1.3/wagtail_formation.egg-info/SOURCES.txt` & `wagtail_formation-0.1.4/wagtail_formation.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 formation/wagtail_hooks.py
 formation/widgets.py
 formation/blocks/__init__.py
 formation/blocks/fields.py
 formation/blocks/forms.py
 formation/migrations/0001_initial.py
 formation/migrations/0002_reusableform_name_alter_reusableform_form_content.py
+formation/migrations/0003_alter_reusableform_form_content.py
 formation/migrations/__init__.py
 formation/static/js/formation.js
 formation/templates/formation/reusable_form.html
 formation/templates/formation/blocks/base_field.html
 formation/templates/formation/blocks/base_form.html
 formation/templates/formation/blocks/boolean_field.html
 formation/templates/formation/blocks/date_field.html
```

