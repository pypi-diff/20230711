# Comparing `tmp/unicms_template_unical-1.2.3.tar.gz` & `tmp/unicms_template_unical-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unicms_template_unical-1.2.3.tar", last modified: Tue Jul  4 09:21:17 2023, max compression
+gzip compressed data, was "unicms_template_unical-1.2.4.tar", last modified: Tue Jul 11 14:58:21 2023, max compression
```

## Comparing `unicms_template_unical-1.2.3.tar` & `unicms_template_unical-1.2.4.tar`

### file list

```diff
@@ -1,216 +1,216 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:21:17.103869 unicms_template_unical-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-04 09:21:17.103869 unicms_template_unical-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 09:21:17.103869 unicms_template_unical-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:21:17.071868 unicms_template_unical-1.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:21:17.075868 unicms_template_unical-1.2.3/src/unicms_template_unical/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:21:17.071868 unicms_template_unical-1.2.3/src/unicms_template_unical/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:21:17.071868 unicms_template_unical-1.2.3/src/unicms_template_unical/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:21:17.075868 unicms_template_unical-1.2.3/src/unicms_template_unical/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    23781 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/locale/it/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:21:17.071868 unicms_template_unical-1.2.3/src/unicms_template_unical/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:21:17.075868 unicms_template_unical-1.2.3/src/unicms_template_unical/static/css/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:21:17.075868 unicms_template_unical-1.2.3/src/unicms_template_unical/static/css/colors/
--rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/css/colors/unicms_exbriner.css
--rw-r--r--   0 runner    (1001) docker     (123)     8498 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/css/colors/unicms_unical.css
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/css/unicms_exbriner.css
--rw-r--r--   0 runner    (1001) docker     (123)    10130 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/css/unicms_unical.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:21:17.075868 unicms_template_unical-1.2.3/src/unicms_template_unical/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    43664 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/fonts/TitilliumWeb-Black.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:21:17.079868 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/addressbook.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/agenda.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/alert-red.svg
--rw-r--r--   0 runner    (1001) docker     (123)   130694 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/banner_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     8720 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/chi.png
--rw-r--r--   0 runner    (1001) docker     (123)    17329 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/dimes.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12905 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/en.png
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/esp.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:21:17.079868 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/favicon/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/favicon/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/favicon/favicon-32x32.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:21:17.083868 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/flags/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/flags/ar.svg
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/flags/en.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/flags/es.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/flags/eu.svg
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/flags/fr.svg
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/flags/it.svg
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/flags/pt.svg
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/flags/ru.svg
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/flags/zh.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/ita.png
--rw-r--r--   0 runner    (1001) docker     (123)   312996 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/library1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    27664 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logo1.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logo_back.svg
--rw-r--r--   0 runner    (1001) docker     (123)    32050 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logo_presta.svg
--rw-r--r--   0 runner    (1001) docker     (123)    42300 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logo_unical_white.svg
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logo_white.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:21:17.087869 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logos/
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logos/HRS4R.svg
--rw-r--r--   0 runner    (1001) docker     (123)    24514 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logos/ctc.svg
--rw-r--r--   0 runner    (1001) docker     (123)    25799 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logos/demacs.svg
--rw-r--r--   0 runner    (1001) docker     (123)    27889 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logos/desf.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28678 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logos/dfssn.svg
--rw-r--r--   0 runner    (1001) docker     (123)    23742 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logos/diam.svg
--rw-r--r--   0 runner    (1001) docker     (123)    27886 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logos/dibest.svg
--rw-r--r--   0 runner    (1001) docker     (123)    25693 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logos/dices.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28422 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logos/dimeg.svg
--rw-r--r--   0 runner    (1001) docker     (123)    31883 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logos/dimes.svg
--rw-r--r--   0 runner    (1001) docker     (123)    22720 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logos/dinci.svg
--rw-r--r--   0 runner    (1001) docker     (123)    25608 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logos/discag.svg
--rw-r--r--   0 runner    (1001) docker     (123)    25944 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logos/dispes.svg
--rw-r--r--   0 runner    (1001) docker     (123)    23078 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logos/disu.svg
--rw-r--r--   0 runner    (1001) docker     (123)   106385 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logos/eu_funded.svg
--rw-r--r--   0 runner    (1001) docker     (123)    23410 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logos/eu_funded_white.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logos/exbriner.png
--rw-r--r--   0 runner    (1001) docker     (123)    20713 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logos/fis.svg
--rw-r--r--   0 runner    (1001) docker     (123)   473786 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logos/master_ges.png
--rw-r--r--   0 runner    (1001) docker     (123)   356948 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/news1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   441153 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/news2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   422058 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/news3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   126770 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/ponte-bucci-1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    40246 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/unical-live.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   508364 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/unical_banner.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    23187 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/unical_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/unical_logo_bullet_white.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:21:17.087869 unicms_template_unical-1.2.3/src/unicms_template_unical/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/js/external_link_new_tab.js
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/static/js/unicms_api_utils.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:21:17.087869 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/500.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:21:17.087869 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/bases/
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/bases/base_v_original.html
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/bases/error-page.html
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/bases/unical_api_list.html
--rw-r--r--   0 runner    (1001) docker     (123)    32156 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/bases/unicms_unical.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:21:17.095869 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_3_level_page.html
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_3_level_page_v2.html
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_carousel_cards.html
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_carousel_hero_slider.html
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_carousel_hero_slider_slim.html
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_carousel_to_page.html
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_contact.html
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_contact_v2.html
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_media_collection_collapse.html
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_media_collection_items.html
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_media_collection_searchbox.html
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_menu_buttons.html
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_menu_buttons_childs.html
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_menu_buttons_other_items.html
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_menu_collapse.html
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_menu_collapse_item_childs.html
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_menu_collapse_item_childs_v2.html
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_menu_collapse_other_items.html
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_menu_collapse_v2.html
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_@.html
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_arrow.html
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_chat.html
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_document.html
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_generic.html
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_menu_main.html
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_menu_main_v2.html
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_menu_secondary.html
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_menu_side.html
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_menu_side_other_items.html
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_menu_side_other_parent_same_level.html
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_menu_sitemap.html
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_menu_to_page.html
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_menu_to_page_with_publication.html
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_page_publication_card_1.html
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_page_publication_card_1_content.html
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_page_publication_card_2.html
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_page_publication_collapse.html
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_page_publication_preview_1.html
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_page_publication_preview_2.html
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_page_publication_top.html
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_publication_alert.html
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_publication_attachments.html
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_publication_box_1.html
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_publication_full_view.html
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_publication_full_view_light.html
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_publication_full_view_only_text.html
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_publication_links.html
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_publication_live.html
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1.html
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1_carousel.html
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1_carousel_home.html
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_publications_card.html
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_publications_cards.html
--rw-r--r--   0 runner    (1001) docker     (123)     8337 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel.html
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_home.html
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_home_v2.html
--rw-r--r--   0 runner    (1001) docker     (123)    13635 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_v2.html
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_v2_home.html
--rw-r--r--   0 runner    (1001) docker     (123)     9756 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic.html
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v2.html
--rw-r--r--   0 runner    (1001) docker     (123)     9770 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v3.html
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v3_home.html
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v4.html
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v4_home.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:21:17.071868 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/grid/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:21:17.095869 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/grid/section_1/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/grid/section_1/center_top_ab_a_double.html
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/grid/section_1/right_spaced.html
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/grid/section_1/section_center_alternative.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:21:17.099869 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/grid/section_2/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/grid/section_2/center_top_ab_a_double.html
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/grid/section_2/right_spaced.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:21:17.099869 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/grid/section_3/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/grid/section_3/center_top_ab_a_double.html
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/grid/section_3/right_spaced.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:21:17.099869 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/inits/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/inits/brython-init.html
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/loading-jumbo.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:21:17.103869 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/department.html
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/department_ctc.html
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/department_demacs.html
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/department_desf.html
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/department_dfssn.html
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/department_diam.html
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/department_dibest.html
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/department_dices.html
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/department_dimeg.html
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/department_dimes.html
--rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/department_dinci.html
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/department_discag.html
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/department_dispes.html
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/department_disu.html
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/department_fis.html
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/master_ges.html
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/multi_language.html
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/opendata.html
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/portale_home_dipartimento_v3.html
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/portale_home_dipartimento_v3_dimes.html
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/portale_home_v_original.html
--rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/project_exbriner.html
--rw-r--r--   0 runner    (1001) docker     (123)    15513 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/publication_list.html
--rw-r--r--   0 runner    (1001) docker     (123)    12280 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/publication_view.html
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/publication_view_hero_original.html
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/unical.html
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/unical_center_top_ab_a_double.html
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/unical_main_center_alternative.html
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/unical_right_spaced.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:21:17.103869 unicms_template_unical-1.2.3/src/unicms_template_unical/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-04 09:21:08.000000 unicms_template_unical-1.2.3/src/unicms_template_unical/templatetags/unicms_template_unical.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 09:21:17.103869 unicms_template_unical-1.2.3/unicms_template_unical.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-04 09:21:17.000000 unicms_template_unical-1.2.3/unicms_template_unical.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-07-04 09:21:17.000000 unicms_template_unical-1.2.3/unicms_template_unical.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 09:21:17.000000 unicms_template_unical-1.2.3/unicms_template_unical.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-04 09:21:17.000000 unicms_template_unical-1.2.3/unicms_template_unical.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-04 09:21:17.000000 unicms_template_unical-1.2.3/unicms_template_unical.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:58:21.994549 unicms_template_unical-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-11 14:58:21.994549 unicms_template_unical-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 14:58:21.994549 unicms_template_unical-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:58:21.966549 unicms_template_unical-1.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:58:21.966549 unicms_template_unical-1.2.4/src/unicms_template_unical/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:58:21.966549 unicms_template_unical-1.2.4/src/unicms_template_unical/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:58:21.966549 unicms_template_unical-1.2.4/src/unicms_template_unical/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:58:21.966549 unicms_template_unical-1.2.4/src/unicms_template_unical/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    23781 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:58:21.966549 unicms_template_unical-1.2.4/src/unicms_template_unical/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:58:21.966549 unicms_template_unical-1.2.4/src/unicms_template_unical/static/css/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:58:21.966549 unicms_template_unical-1.2.4/src/unicms_template_unical/static/css/colors/
+-rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/css/colors/unicms_exbriner.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8509 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/css/colors/unicms_unical.css
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/css/unicms_exbriner.css
+-rw-r--r--   0 runner    (1001) docker     (123)    10130 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/css/unicms_unical.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:58:21.966549 unicms_template_unical-1.2.4/src/unicms_template_unical/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    43664 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/fonts/TitilliumWeb-Black.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:58:21.974549 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/addressbook.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/agenda.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/alert-red.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   130694 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/banner_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     8720 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/chi.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17329 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/dimes.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12905 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/en.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/esp.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:58:21.974549 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/favicon/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/favicon/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/favicon/favicon-32x32.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:58:21.974549 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/flags/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/flags/ar.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/flags/en.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/flags/es.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/flags/eu.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/flags/fr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/flags/it.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/flags/pt.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/flags/ru.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/flags/zh.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/ita.png
+-rw-r--r--   0 runner    (1001) docker     (123)   312996 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/library1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    27664 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logo1.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logo_back.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    32050 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logo_presta.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    42300 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logo_unical_white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logo_white.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:58:21.978549 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logos/
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logos/HRS4R.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    24514 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logos/ctc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    25799 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logos/demacs.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    27889 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logos/desf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28678 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logos/dfssn.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    23742 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logos/diam.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    27886 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logos/dibest.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    25693 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logos/dices.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28422 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logos/dimeg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    31883 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logos/dimes.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    22720 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logos/dinci.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    25608 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logos/discag.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    25944 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logos/dispes.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    23078 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logos/disu.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   106385 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logos/eu_funded.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    23410 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logos/eu_funded_white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logos/exbriner.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20713 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logos/fis.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   473786 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logos/master_ges.png
+-rw-r--r--   0 runner    (1001) docker     (123)   356948 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/news1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   441153 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/news2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   422058 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/news3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   126770 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/ponte-bucci-1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    40246 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/unical-live.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   508364 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/unical_banner.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    23187 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/unical_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/unical_logo_bullet_white.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:58:21.978549 unicms_template_unical-1.2.4/src/unicms_template_unical/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/js/external_link_new_tab.js
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/static/js/unicms_api_utils.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:58:21.978549 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/500.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:58:21.982549 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/bases/
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/bases/base_v_original.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/bases/error-page.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/bases/unical_api_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)    32156 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/bases/unicms_unical.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:58:21.990549 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_3_level_page.html
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_3_level_page_v2.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_carousel_cards.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_carousel_hero_slider.html
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_carousel_hero_slider_slim.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_carousel_to_page.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_contact.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_contact_v2.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_media_collection_collapse.html
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_media_collection_items.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_media_collection_searchbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_menu_buttons.html
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_menu_buttons_childs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_menu_buttons_other_items.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_menu_collapse.html
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_menu_collapse_item_childs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_menu_collapse_item_childs_v2.html
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_menu_collapse_other_items.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_menu_collapse_v2.html
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_@.html
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_arrow.html
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_chat.html
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_document.html
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_generic.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_menu_main.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_menu_main_v2.html
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_menu_secondary.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_menu_side.html
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_menu_side_other_items.html
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_menu_side_other_parent_same_level.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_menu_sitemap.html
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_menu_to_page.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_menu_to_page_with_publication.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_page_publication_card_1.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_page_publication_card_1_content.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_page_publication_card_2.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_page_publication_collapse.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_page_publication_preview_1.html
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_page_publication_preview_2.html
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_page_publication_top.html
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_publication_alert.html
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_publication_attachments.html
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_publication_box_1.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_publication_full_view.html
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_publication_full_view_light.html
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_publication_full_view_only_text.html
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_publication_links.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_publication_live.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1_carousel.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1_carousel_home.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_publications_card.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_publications_cards.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8509 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel.html
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_home.html
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_home_v2.html
+-rw-r--r--   0 runner    (1001) docker     (123)    14233 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_v2.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_v2_home.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9756 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v2.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9770 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v3.html
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v3_home.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v4.html
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v4_home.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:58:21.966549 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/grid/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:58:21.990549 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/grid/section_1/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/grid/section_1/center_top_ab_a_double.html
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/grid/section_1/right_spaced.html
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/grid/section_1/section_center_alternative.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:58:21.990549 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/grid/section_2/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/grid/section_2/center_top_ab_a_double.html
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/grid/section_2/right_spaced.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:58:21.990549 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/grid/section_3/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/grid/section_3/center_top_ab_a_double.html
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/grid/section_3/right_spaced.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:58:21.990549 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/inits/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/inits/brython-init.html
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/loading-jumbo.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:58:21.994549 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/department.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/department_ctc.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/department_demacs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/department_desf.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/department_dfssn.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/department_diam.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/department_dibest.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/department_dices.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/department_dimeg.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/department_dimes.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/department_dinci.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/department_discag.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/department_dispes.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/department_disu.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/department_fis.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/master_ges.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/multi_language.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/opendata.html
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/portale_home_dipartimento_v3.html
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/portale_home_dipartimento_v3_dimes.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/portale_home_v_original.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/project_exbriner.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15513 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/publication_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12280 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/publication_view.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/publication_view_hero_original.html
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/unical.html
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/unical_center_top_ab_a_double.html
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/unical_main_center_alternative.html
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/unical_right_spaced.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:58:21.994549 unicms_template_unical-1.2.4/src/unicms_template_unical/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-11 14:58:13.000000 unicms_template_unical-1.2.4/src/unicms_template_unical/templatetags/unicms_template_unical.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:58:21.994549 unicms_template_unical-1.2.4/unicms_template_unical.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-11 14:58:21.000000 unicms_template_unical-1.2.4/unicms_template_unical.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-07-11 14:58:21.000000 unicms_template_unical-1.2.4/unicms_template_unical.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:58:21.000000 unicms_template_unical-1.2.4/unicms_template_unical.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-11 14:58:21.000000 unicms_template_unical-1.2.4/unicms_template_unical.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-11 14:58:21.000000 unicms_template_unical-1.2.4/unicms_template_unical.egg-info/top_level.txt
```

### Comparing `unicms_template_unical-1.2.3/LICENSE` & `unicms_template_unical-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/PKG-INFO` & `unicms_template_unical-1.2.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicms_template_unical
-Version: 1.2.3
+Version: 1.2.4
 Summary: uniCMS Unical Template based on Bootstrap Italia
 Home-page: https://github.com/UniversitaDellaCalabria/unicms-template-unical
 Author: Giuseppe De Marco, Francesco Filicetti
 Author-email: giuseppe.demarco@unical.it, francesco.filicetti@unical.it
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `unicms_template_unical-1.2.3/setup.py` & `unicms_template_unical-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  twine upload dist/*
 
 SRC_FOLDER = 'src'
 PKG_NAME = 'unicms_template_unical'
 
 setup(
     name=PKG_NAME,
-    version='1.2.3',
+    version='1.2.4',
 
     packages=[PKG_NAME],
     package_dir={PKG_NAME: f"{SRC_FOLDER}/{PKG_NAME}"},
 
     package_data={PKG_NAME: [i.replace(f'{SRC_FOLDER}/{PKG_NAME}/', '')
                                    for i in glob(f'{SRC_FOLDER}/{PKG_NAME}/**',
                                                  recursive=True)]
```

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/locale/it/LC_MESSAGES/django.mo` & `unicms_template_unical-1.2.4/src/unicms_template_unical/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/locale/it/LC_MESSAGES/django.po` & `unicms_template_unical-1.2.4/src/unicms_template_unical/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/css/colors/unicms_exbriner.css` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/css/colors/unicms_exbriner.css`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/css/colors/unicms_unical.css` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/css/colors/unicms_unical.css`

 * *Files 1% similar despite different names*

```diff
@@ -314,15 +314,15 @@
 }
 
 .nav-tabs .nav-link,
 .nav-tabs .nav-link:hover {
     color: var(--light_grey_unical);
 }
 .nav-tabs .nav-item.show .nav-link, .nav-tabs .nav-link.active {
-    border-bottom-color: var(--bordeaux_unical);
+    border-bottom-color: var(--bordeaux_unical) !important;
     color: var(--dark_grey_unical);
 }
 
 .link-list-wrapper ul li a span,
 .link-list-wrapper ul li a:hover:not(.disabled) span {
     color: var(--dark_grey_unical);
 }
```

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/css/unicms_unical.css` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/css/unicms_unical.css`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/fonts/TitilliumWeb-Black.ttf` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/fonts/TitilliumWeb-Black.ttf`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/addressbook.svg` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/addressbook.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/agenda.jpg` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/agenda.jpg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/alert-red.svg` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/alert-red.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/banner_1.jpg` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/banner_1.jpg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/chi.png` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/chi.png`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/dimes.svg` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/dimes.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/en.png` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/en.png`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/esp.png` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/esp.png`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/flags/ar.svg` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/flags/ar.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/flags/en.svg` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/flags/en.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/flags/es.svg` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/flags/es.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/flags/eu.svg` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/flags/eu.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/flags/zh.svg` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/flags/zh.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/ita.png` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/ita.png`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/library1.jpg` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/library1.jpg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logo.png` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logo.svg` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logo1.svg` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logo1.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logo_back.svg` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logo_back.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logo_presta.svg` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logo_presta.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logo_unical_white.svg` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logo_unical_white.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logo_white.png` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logo_white.png`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logos/HRS4R.svg` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logos/HRS4R.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logos/ctc.svg` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logos/ctc.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logos/demacs.svg` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logos/demacs.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logos/desf.svg` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logos/desf.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logos/dfssn.svg` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logos/dfssn.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logos/diam.svg` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logos/diam.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logos/dibest.svg` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logos/dibest.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logos/dices.svg` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logos/dices.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logos/dimeg.svg` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logos/dimeg.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logos/dimes.svg` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logos/dimes.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logos/dinci.svg` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logos/dinci.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logos/discag.svg` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logos/discag.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logos/dispes.svg` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logos/dispes.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logos/disu.svg` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logos/disu.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logos/eu_funded.svg` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logos/eu_funded.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logos/eu_funded_white.svg` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logos/eu_funded_white.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logos/exbriner.png` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logos/exbriner.png`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logos/fis.svg` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logos/fis.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/logos/master_ges.png` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/logos/master_ges.png`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/news1.jpg` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/news1.jpg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/news2.jpg` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/news2.jpg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/news3.jpg` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/news3.jpg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/ponte-bucci-1.jpg` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/ponte-bucci-1.jpg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/unical-live.jpg` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/unical-live.jpg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/unical_banner.jpg` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/unical_banner.jpg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/unical_logo.svg` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/unical_logo.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/static/images/unical_logo_bullet_white.svg` & `unicms_template_unical-1.2.4/src/unicms_template_unical/static/images/unical_logo_bullet_white.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/404.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/404.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/bases/base_v_original.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/bases/base_v_original.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/bases/error-page.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/bases/error-page.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/bases/unical_api_list.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/bases/unical_api_list.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/bases/unicms_unical.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/bases/unicms_unical.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_carousel_cards.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_carousel_cards.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_carousel_hero_slider.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_carousel_hero_slider.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_carousel_hero_slider_slim.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_carousel_hero_slider_slim.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_carousel_to_page.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_carousel_to_page.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_contact.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_contact.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_contact_v2.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_contact_v2.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_media_collection_collapse.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_media_collection_collapse.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_media_collection_items.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_media_collection_items.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_media_collection_searchbox.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_media_collection_searchbox.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_menu_buttons.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_menu_buttons.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_menu_collapse.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_menu_collapse.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_menu_collapse_v2.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_menu_collapse_v2.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_generic.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_generic.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_menu_main.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_menu_main.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_menu_main_v2.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_menu_main_v2.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_menu_secondary.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_menu_secondary.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_menu_side.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_menu_side.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_menu_sitemap.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_menu_sitemap.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_menu_to_page_with_publication.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_menu_to_page_with_publication.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_page_publication_card_1.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_page_publication_card_1.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_page_publication_card_1_content.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_page_publication_card_1_content.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_page_publication_card_2.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_page_publication_card_2.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_page_publication_collapse.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_page_publication_collapse.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_page_publication_preview_1.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_page_publication_preview_1.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_page_publication_top.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_page_publication_top.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_publication_alert.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_publication_alert.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_publication_attachments.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_publication_attachments.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_publication_full_view.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_publication_full_view.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_publication_live.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_publication_live.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1_carousel.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1_carousel.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1_carousel_home.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1_carousel_home.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_publications_card.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_publications_card.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_publications_cards.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_publications_cards.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel.html`

 * *Files 2% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 <div class="custom-unical owl-carousel d-none d-lg-block" id="carousel_{{ uid }}">
     {% for pub in publications %}
     <div class="card-wrapper card-space">
         <div class="card card-bg no-after">
             <div class="card-body">
                 {% block desktop_item_body %}
 
-                {% block categories_buttons %}
+                {% block categories_buttons_1 %}
                 {% if categories|length != 1 %}
                 <div class="etichetta">
                     {% for cat in pub.publication.categories %}
                         <span class="badge rounded-pill badge-grey-unical my-1 py-2 px-4 me-1">
                             <a class="no-color" href="{% call obj=pub method='get_url_list' category_name=cat.name %}">
                                 <b>{{ cat.name }}</b>
                             </a>
                         </span>
                     {% endfor %}
                 </div>
                 {% endif %}
-                {% endblock categories_buttons %}
+                {% endblock categories_buttons_1 %}
 
                 {% if pub.publication.image_url %}
                 <div class="img-responsive-wrapper mb-3 mx-n4" {% if categories|length == 1 %}style="margin-top: -24px"{% endif %}>
                     <div class="img-responsive img-responsive-panoramic">
                         <figure class="img-wrapper">
                           <a href="{{ pub.url }}">
                             <img src="{{ pub.publication.image_url }}"
@@ -74,27 +74,31 @@
 
 <div class="custom-unical d-lg-none">
     {% for pub in publications %}
     <div class="card-wrapper card-space">
         <div class="card card-bg no-after">
             <div class="card-body">
                 {% block mobile_item_body %}
+
+                {% block categories_buttons_2 %}
                 {% if categories|length != 1 %}
                 <div class="etichetta">
                     {% for cat in pub.publication.categories %}
                         <span class="badge rounded-pill badge-grey-unical my-1 py-2 px-4 me-1">
                             <a class="no-color" href="{% call obj=pub method='get_url_list' category_name=cat.name %}">
                                 <b>{{ cat.name }}</b>
                             </a>
                         </span>
                     {% endfor %}
                 </div>
                 {% endif %}
+                {% endblock categories_buttons_2 %}
+
                 {% if pub.publication.image_url %}
-                <div class="img-responsive-wrapper mb-3 mx-n4" {% if categories|length == 1 %}style="margin-top: -24px"{% endif %}>
+                <div class="img-responsive-wrapper mb-3 mx-n4" {% block categories_margin_2 %}{% if categories|length == 1 %}style="margin-top: -24px"{% endif %}{% endblock categories_margin_2 %}>
                     <div class="img-responsive img-responsive-panoramic">
                         <figure class="img-wrapper">
                           <a href="{{ pub.url }}">
                             <img src="{{ pub.publication.image_url }}"
                                  title="{{ pub.publication.image_title }}"
                                  alt="{{ pub.publication.image_description }}"
                                  loading="lazy">
```

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_home_v2.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_home_v2.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_v2.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_v2.html`

 * *Files 10% similar despite different names*

```diff
@@ -16,25 +16,27 @@
         <div class="card-wrapper card-space">
             <div class="card card-bg no-after">
                 <div class="card-body ps-lg-0">
                     <div class="row h-100">
                         {% if pub.publication.image_url %}
                         <div class="col-12 col-lg-6">
 
+                            {% block categories_buttons_1 %}
                             {% if pub.publication.categories|length > 1 %}
                             <div class="etichetta d-lg-none">
                                 {% for cat in pub.publication.categories %}
                                 <span class="badge rounded-pill badge-grey-unical my-1 py-2 px-4 me-1">
                                     <a class="no-color" href="{% call obj=pub method='get_url_list' category_name=cat.name %}">
                                         <b>{{ cat.name }}</b>
                                     </a>
                                 </span>
                                 {% endfor %}
                             </div>
                             {% endif %}
+                            {% endblock categories_buttons_1 %}
 
                             <div class="img-responsive-wrapper mb-3 mx-n4 d-lg-none ">
                                 <div class="img-responsive img-responsive-panoramic">
                                     <figure class="img-wrapper">
                                       <a href="{{ pub.url }}">
                                         <img src="{{ pub.publication.image_url }}"
                                              title="{{ pub.publication.image_title }}"
@@ -58,25 +60,27 @@
                                 </div>
                             </div>
                         </div>
 
                         {% endif %}
                         <div class="col-12 col-lg-6 ps-lg-4">
 
+                            {% block categories_buttons_2 %}
                             {% if pub.publication.categories|length > 1 %}
                             <div class="etichetta d-none d-lg-block">
                                 {% for cat in pub.publication.categories %}
                                 <span class="badge rounded-pill badge-grey-unical my-1 py-2 px-4 me-1">
                                     <a class="no-color" href="{% call obj=pub method='get_url_list' category_name=cat.name %}">
                                         <b>{{ cat.name }}</b>
                                     </a>
                                 </span>
                                 {% endfor %}
                             </div>
                             {% endif %}
+                            {% endblock categories_buttons_2 %}
 
                             <div class="category-top">
                                 <span>{% trans "Published" %}: {{ pub.date_start | date:"d/m/Y, H:i" }}</span>
                                 {% include "includes/edit_news.html" with item=pub %}
                             </div>
 
                             <a class="no-color" href="{{ pub.url }}">
@@ -104,28 +108,30 @@
     {% else %}
 
         <div class="card-wrapper card-space">
             <div class="card card-bg no-after">
                 <div class="card-body">
                     {% block desktop_item_body %}
 
+                    {% block categories_buttons_3 %}
                     {% if pub.publication.categories|length > 1 %}
                     <div class="etichetta">
                         {% for cat in pub.publication.categories %}
                             <span class="badge rounded-pill badge-grey-unical my-1 py-2 px-4 me-1">
                                 <a class="no-color" href="{% call obj=pub method='get_url_list' category_name=cat.name %}">
                                     <b>{{ cat.name }}</b>
                                 </a>
                             </span>
                         {% endfor %}
                     </div>
                     {% endif %}
+                    {% endblock categories_buttons_3 %}
 
                     {% if pub.publication.image_url %}
-                    <div class="img-responsive-wrapper mb-3 mx-n4" {% if pub.publication.categories|length == 1 %}style="margin-top: -24px"{% endif %}>
+                    <div class="img-responsive-wrapper mb-3 mx-n4" {% block categories_margin_3 %}{% if pub.publication.categories|length == 1 %}style="margin-top: -24px"{% endif %}{% endblock categories_margin_3 %}>
                         <div class="img-responsive img-responsive-panoramic">
                             <figure class="img-wrapper">
                               <a href="{{ pub.url }}">
                                 <img src="{{ pub.publication.image_url }}"
                                      title="{{ pub.publication.image_title }}"
                                      alt="{{ pub.publication.image_description }}"
                                      loading="lazy">
@@ -169,28 +175,30 @@
     <div class="custom-unical d-lg-none">
         {% for pub in publications %}
         <div class="card-wrapper card-space">
             <div class="card card-bg no-after">
                 <div class="card-body">
                     {% block mobile_item_body %}
 
+                    {% block categories_buttons_4 %}
                     {% if categories|length != 1 %}
                     <div class="etichetta">
                         {% for cat in pub.publication.categories %}
                             <span class="badge rounded-pill badge-grey-unical my-1 py-2 px-4 me-1">
                                 <a class="no-color" href="{% call obj=pub method='get_url_list' category_name=cat.name %}">
                                     <b>{{ cat.name }}</b>
                                 </a>
                             </span>
                         {% endfor %}
                     </div>
                     {% endif %}
+                    {% endblock categories_buttons_4 %}
 
                     {% if pub.publication.image_url %}
-                    <div class="img-responsive-wrapper mb-3 mx-n4" {% if pub.publication.categories|length == 1 %}style="margin-top: -24px"{% endif %}>
+                    <div class="img-responsive-wrapper mb-3 mx-n4" {% block categories_margin_4 %}{% if pub.publication.categories|length == 1 %}style="margin-top: -24px"{% endif %}{% endblock categories_margin_4 %}>
                         <div class="img-responsive img-responsive-panoramic">
                             <figure class="img-wrapper">
                               <a href="{{ pub.url }}">
                                 <img src="{{ pub.publication.image_url }}"
                                      title="{{ pub.publication.image_title }}"
                                      alt="{{ pub.publication.image_description }}"
                                      loading="lazy">
```

#### html2text {}

```diff
@@ -1,36 +1,38 @@
 {% load i18n %} {% load static %} {% load unicms_contexts %} {% load
 unicms_templates %} {% settings_value "CMS_PUBLICATION_LIST_PREFIX_PATH" as
 page_news_suffix %} {% settings_value "UNICAL_PUBLICATION_CAROUSEL_ITEMS" as
 carousel_items %} {% random_id as uid %} {% if publications %} {% for pub in
 publications %} {% if forloop.first %}
 {% if pub.publication.image_url %}
-{% if pub.publication.categories|length > 1 %}
+{% block categories_buttons_1 %} {% if pub.publication.categories|length > 1 %}
 {% for cat in pub.publication.categories %}  {{_cat.name_}}  {% endfor %}
-{% endif %}
+{% endif %} {% endblock categories_buttons_1 %}
  [{{_pub.publication.image_description_}}]
  [{{_pub.publication.image_description_}}]
 {% endif %}
-{% if pub.publication.categories|length > 1 %}
+{% block categories_buttons_2 %} {% if pub.publication.categories|length > 1 %}
 {% for cat in pub.publication.categories %}  {{_cat.name_}}  {% endfor %}
-{% endif %}
+{% endif %} {% endblock categories_buttons_2 %}
 {% trans "Published" %}: {{ pub.date_start | date:"d/m/Y, H:i" }} {% include
 "includes/edit_news.html" with item=pub %}
 ***_{{_pub.publication.title_}}_***
  {% if pub.publication.subheading %}
 {{ pub.publication.subheading }}
 {% endif %} {% include "includes/social_share.html" with
 share_title=pub.publication.title share_url=request.get_host|add:pub.url %}
 {% if carousel_items > 1 %}
 {% endif %} {% else %}
-{% block desktop_item_body %} {% if pub.publication.categories|length > 1 %}
+{% block desktop_item_body %} {% block categories_buttons_3 %} {% if
+pub.publication.categories|length > 1 %}
 {% for cat in pub.publication.categories %}  {{_cat.name_}}  {% endfor %}
-{% endif %} {% if pub.publication.image_url %}
-% if pub.publication.categories|length == 1 %}style="margin-top: -24px"{% endif
-%}>
+{% endif %} {% endblock categories_buttons_3 %} {% if pub.publication.image_url
+%}
+% block categories_margin_3 %}{% if pub.publication.categories|length == 1
+%}style="margin-top: -24px"{% endif %}{% endblock categories_margin_3 %}>
  [{{_pub.publication.image_description_}}]
 {% endif %}
 {% trans "Published" %}: {{ pub.date_start | date:"d/m/Y, H:i" }} {% include
 "includes/edit_news.html" with item=pub %}
 {% block desktop_item_title %}
 *** {{_pub.publication.title|truncatechars:120_}} ***
 {% endblock desktop_item_title %} {% block desktop_subheading %} {% if not
@@ -38,19 +40,21 @@
 {{ pub.publication.subheading|truncatechars:135 }}
 {% endif %} {% endblock desktop_subheading %} {% include "includes/
 social_share.html" with share_title=pub.publication.title
 share_url=request.get_host|add:pub.url %} {% endblock desktop_item_body %}
 {% endif %} {% endfor %} {% if carousel_items > 1 %}
 {% endif %}
 {% for pub in publications %}
-{% block mobile_item_body %} {% if categories|length != 1 %}
+{% block mobile_item_body %} {% block categories_buttons_4 %} {% if
+categories|length != 1 %}
 {% for cat in pub.publication.categories %}  {{_cat.name_}}  {% endfor %}
-{% endif %} {% if pub.publication.image_url %}
-% if pub.publication.categories|length == 1 %}style="margin-top: -24px"{% endif
-%}>
+{% endif %} {% endblock categories_buttons_4 %} {% if pub.publication.image_url
+%}
+% block categories_margin_4 %}{% if pub.publication.categories|length == 1
+%}style="margin-top: -24px"{% endif %}{% endblock categories_margin_4 %}>
  [{{_pub.publication.image_description_}}]
 {% endif %}
 {% trans "Published" %}: {{ pub.date_start | date:"d/m/Y, H:i" }} {% include
 "includes/edit_news.html" with item=pub %}
 {% block mobile_item_title %}
 *** {{_pub.publication.title|truncatechars:120_}} ***
 {% endblock mobile_item_title %} {% block mobile_subheading %} {% if not
```

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v2.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v2.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v3.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v3.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v4.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v4.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/loading-jumbo.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/loading-jumbo.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/department.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/department.html`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
                 {% if request.user.is_staff %}
                 {% include "components/italia_editorialboard_frontend_menu.html" %}
                 {% endif %}
             </div>
         </div>
     </div>
 </div>
-<a href="/" aria-label="{% trans 'University of Calabria' %}">
+<a href="{% block unical_department_header_slim_org_url %}/{% endblock unical_department_header_slim_org_url %}" aria-label="{% trans 'University of Calabria' %}">
     <div class="it-header-center-wrapper d-lg-none h-auto pt-4">
         {% block unical_mobile_logo %}
             {% block header_slim_mobile_org_name_side %}
                 <image src="{% unicms_template_unical_static_path 'images/unical_logo_bullet_white.svg' %}" class="mw-100"/>
             {% endblock header_slim_mobile_org_name_side %}
         {% endblock unical_mobile_logo %}
     </div>
```

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/department_ctc.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/department_ctc.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/department_demacs.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/department_demacs.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/department_desf.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/department_desf.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/department_dfssn.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/department_dfssn.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/department_diam.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/department_diam.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/department_dibest.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/department_dibest.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/department_dices.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/department_dices.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/department_dimeg.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/department_dimeg.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/department_dimes.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/department_dimes.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/department_dinci.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/department_dinci.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/department_discag.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/department_discag.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/department_dispes.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/department_dispes.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/department_disu.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/department_disu.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/department_fis.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/department_fis.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/master_ges.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/master_ges.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/multi_language.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/multi_language.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/opendata.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/opendata.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/portale_home_dipartimento_v3.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/portale_home_dipartimento_v3.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/portale_home_dipartimento_v3_dimes.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/portale_home_dipartimento_v3_dimes.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/portale_home_v_original.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/portale_home_v_original.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/project_exbriner.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/project_exbriner.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/publication_list.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/publication_list.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/publication_view.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/publication_view.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templates/pages/publication_view_hero_original.html` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templates/pages/publication_view_hero_original.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/src/unicms_template_unical/templatetags/unicms_template_unical.py` & `unicms_template_unical-1.2.4/src/unicms_template_unical/templatetags/unicms_template_unical.py`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.3/unicms_template_unical.egg-info/PKG-INFO` & `unicms_template_unical-1.2.4/unicms_template_unical.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicms-template-unical
-Version: 1.2.3
+Version: 1.2.4
 Summary: uniCMS Unical Template based on Bootstrap Italia
 Home-page: https://github.com/UniversitaDellaCalabria/unicms-template-unical
 Author: Giuseppe De Marco, Francesco Filicetti
 Author-email: giuseppe.demarco@unical.it, francesco.filicetti@unical.it
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `unicms_template_unical-1.2.3/unicms_template_unical.egg-info/SOURCES.txt` & `unicms_template_unical-1.2.4/unicms_template_unical.egg-info/SOURCES.txt`

 * *Files identical despite different names*

