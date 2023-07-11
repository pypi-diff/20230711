# Comparing `tmp/mgtron-2.19.4.tar.gz` & `tmp/mgtron-2.19.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mgtron-2.19.4.tar", last modified: Mon Jul 10 21:11:49 2023, max compression
+gzip compressed data, was "mgtron-2.19.5.tar", last modified: Tue Jul 11 20:54:07 2023, max compression
```

## Comparing `mgtron-2.19.4.tar` & `mgtron-2.19.5.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 21:11:49.799816 mgtron-2.19.4/
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 21:11:49.773149 mgtron-2.19.4/.github/
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 21:11:49.776483 mgtron-2.19.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      602 2023-06-23 15:16:00.000000 mgtron-2.19.4/.github/ISSUE_TEMPLATE/mgtron--.md
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1524 2023-06-23 15:16:00.000000 mgtron-2.19.4/.github/ISSUE_TEMPLATE/mgtron_issue.yml
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 21:11:49.776483 mgtron-2.19.4/.github/workflows/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      520 2023-06-30 12:43:52.000000 mgtron-2.19.4/.github/workflows/black_actions.yml
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      830 2023-06-30 12:43:52.000000 mgtron-2.19.4/.github/workflows/pypi_action.yml
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      387 2023-07-10 14:37:39.000000 mgtron-2.19.4/.gitignore
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     9254 2023-07-10 21:07:07.000000 mgtron-2.19.4/CHANGELOG.md
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      957 2023-06-23 15:16:00.000000 mgtron-2.19.4/LICENSE.rst
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     4198 2023-07-10 21:11:49.799816 mgtron-2.19.4/PKG-INFO
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     3699 2023-06-23 15:16:00.000000 mgtron-2.19.4/README.md
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 21:11:49.776483 mgtron-2.19.4/docs/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    17614 2023-06-23 15:16:01.000000 mgtron-2.19.4/docs/MGTron Command Description.docx
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    23088 2023-06-23 15:16:01.000000 mgtron-2.19.4/docs/MGTron Function Descriptions.docx
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 21:11:49.776483 mgtron-2.19.4/mgtron.egg-info/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     4198 2023-07-10 21:11:49.000000 mgtron-2.19.4/mgtron.egg-info/PKG-INFO
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2334 2023-07-10 21:11:49.000000 mgtron-2.19.4/mgtron.egg-info/SOURCES.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        1 2023-07-10 21:11:49.000000 mgtron-2.19.4/mgtron.egg-info/dependency_links.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       37 2023-07-10 21:11:49.000000 mgtron-2.19.4/mgtron.egg-info/entry_points.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2085 2023-07-10 21:11:49.000000 mgtron-2.19.4/mgtron.egg-info/requires.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       19 2023-07-10 21:11:49.000000 mgtron-2.19.4/mgtron.egg-info/top_level.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1161 2023-07-10 14:37:39.000000 mgtron-2.19.4/pyproject.toml
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2022 2023-07-10 17:50:34.000000 mgtron-2.19.4/requirements.txt
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       38 2023-07-10 21:11:49.799816 mgtron-2.19.4/setup.cfg
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 21:11:49.776483 mgtron-2.19.4/src/
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        1 2023-06-28 15:56:43.000000 mgtron-2.19.4/src/__init__.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 21:11:49.783149 mgtron-2.19.4/src/assets/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    83964 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/assets/CA logo without subtext.JPG
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    65978 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/assets/CA_subheading.png
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000) 12776672 2023-07-10 14:37:39.000000 mgtron-2.19.4/src/assets/blueio_rs
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)     1303 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/assets/init_cellantenna.sh
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      723 2023-07-10 14:37:39.000000 mgtron-2.19.4/src/assets/log_read
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      291 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/assets/mgtron.desktop
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2655 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/assets/mgtron.svg
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    67646 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/assets/network-wireless.ico
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000) 11314288 2023-07-10 14:37:39.000000 mgtron-2.19.4/src/assets/wifi_rs
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 21:11:49.789816 mgtron-2.19.4/src/ble/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/ble/__init__.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     3130 2023-07-10 14:37:39.000000 mgtron-2.19.4/src/ble/ble_data.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     8527 2023-07-10 14:37:39.000000 mgtron-2.19.4/src/ble/helpers.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      859 2023-06-30 12:43:53.000000 mgtron-2.19.4/src/ble/scanning.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 21:11:49.793150 mgtron-2.19.4/src/db/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.4/src/db/__init__.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.4/src/db/channel_1.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.4/src/db/channel_2.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.4/src/db/channel_3.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.4/src/db/channel_4.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.4/src/db/channel_5.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.4/src/db/channel_6.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.4/src/db/channel_7.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.4/src/db/channel_8.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    10853 2023-07-10 14:37:39.000000 mgtron-2.19.4/src/db/helpers.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2516 2023-06-27 20:21:35.000000 mgtron-2.19.4/src/db/init_db.sql
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    10906 2023-06-27 20:21:35.000000 mgtron-2.19.4/src/db/long_save.json
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.4/src/db/long_save.json.lock
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    49152 2023-07-10 14:18:59.000000 mgtron-2.19.4/src/db/mgtron_db.db
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     9055 2023-07-10 14:37:39.000000 mgtron-2.19.4/src/db/models.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1170 2023-06-27 20:21:35.000000 mgtron-2.19.4/src/db/quick_save.json
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 21:11:49.793150 mgtron-2.19.4/src/globals/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.4/src/globals/__init__.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     3642 2023-07-10 14:37:39.000000 mgtron-2.19.4/src/globals/helpers.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 21:11:49.793150 mgtron-2.19.4/src/gui/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       80 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/gui/__init__.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 21:11:49.796483 mgtron-2.19.4/src/gui/_configs/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/gui/_configs/card_1.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/gui/_configs/card_2.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/gui/_configs/card_3.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/gui/_configs/card_4.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/gui/_configs/card_5.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/gui/_configs/card_6.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      263 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/gui/_configs/card_7.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/gui/_configs/card_8.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       98 2023-06-21 12:37:32.000000 mgtron-2.19.4/src/gui/_configs/card_config.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      317 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/gui/_configs/mission_alpha.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      292 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/gui/_configs/mission_bravo.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      324 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/gui/_configs/mission_charlie.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      312 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/gui/_configs/mission_delta.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      273 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/gui/_configs/mission_echo.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      313 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/gui/_configs/mission_fox.ini
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      279 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/gui/_configs/mission_golf.ini
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 21:11:49.796483 mgtron-2.19.4/src/gui/fonts/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1260156 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/gui/fonts/MesloLGS NF Bold Italic.ttf
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1251424 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/gui/fonts/MesloLGS NF Italic.ttf
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1292408 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/gui/fonts/MesloLGS NF Regular.ttf
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    50355 2023-07-10 20:59:37.000000 mgtron-2.19.4/src/gui/helpers.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    10970 2023-07-10 20:18:55.000000 mgtron-2.19.4/src/gui/interface.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    43723 2023-07-10 20:40:44.000000 mgtron-2.19.4/src/main.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 21:11:49.796483 mgtron-2.19.4/src/tests/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       33 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/tests/__init__.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       70 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/tests/test_ble.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    63110 2023-06-23 15:16:01.000000 mgtron-2.19.4/src/tests/test_configfiles.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    19824 2023-07-10 14:37:39.000000 mgtron-2.19.4/src/tests/test_helpers.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 21:11:49.799816 mgtron-2.19.4/src/wifi/
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.4/src/wifi/__init__.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      507 2023-07-10 14:37:39.000000 mgtron-2.19.4/src/wifi/chasing.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    15531 2023-07-10 21:02:34.000000 mgtron-2.19.4/src/wifi/helpers.py
--rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     9516 2023-07-10 14:37:39.000000 mgtron-2.19.4/src/wifi/scanning.py
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 21:11:49.773149 mgtron-2.19.4/venv/
-drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-10 21:11:49.799816 mgtron-2.19.4/venv/bin/
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      665 2023-06-12 19:48:50.000000 mgtron-2.19.4/venv/bin/rst2html.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      787 2023-06-12 19:48:50.000000 mgtron-2.19.4/venv/bin/rst2html4.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)     1122 2023-06-12 19:48:50.000000 mgtron-2.19.4/venv/bin/rst2html5.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      864 2023-06-12 19:48:50.000000 mgtron-2.19.4/venv/bin/rst2latex.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      687 2023-06-12 19:48:50.000000 mgtron-2.19.4/venv/bin/rst2man.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      853 2023-06-12 19:48:50.000000 mgtron-2.19.4/venv/bin/rst2odt.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      659 2023-06-12 19:48:50.000000 mgtron-2.19.4/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      672 2023-06-12 19:48:50.000000 mgtron-2.19.4/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      708 2023-06-12 19:48:50.000000 mgtron-2.19.4/venv/bin/rst2s5.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      944 2023-06-12 19:48:50.000000 mgtron-2.19.4/venv/bin/rst2xetex.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      673 2023-06-12 19:48:50.000000 mgtron-2.19.4/venv/bin/rst2xml.py
--rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      741 2023-06-12 19:48:50.000000 mgtron-2.19.4/venv/bin/rstpep2html.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-11 20:54:07.822219 mgtron-2.19.5/
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-11 20:54:07.625548 mgtron-2.19.5/.github/
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-11 20:54:07.638882 mgtron-2.19.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      602 2023-06-23 15:16:00.000000 mgtron-2.19.5/.github/ISSUE_TEMPLATE/mgtron--.md
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1524 2023-06-23 15:16:00.000000 mgtron-2.19.5/.github/ISSUE_TEMPLATE/mgtron_issue.yml
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-11 20:54:07.638882 mgtron-2.19.5/.github/workflows/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      520 2023-06-30 12:43:52.000000 mgtron-2.19.5/.github/workflows/black_actions.yml
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      830 2023-06-30 12:43:52.000000 mgtron-2.19.5/.github/workflows/pypi_action.yml
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      387 2023-07-10 14:37:39.000000 mgtron-2.19.5/.gitignore
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     9254 2023-07-10 21:07:07.000000 mgtron-2.19.5/CHANGELOG.md
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      957 2023-06-23 15:16:00.000000 mgtron-2.19.5/LICENSE.rst
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     4198 2023-07-11 20:54:07.822219 mgtron-2.19.5/PKG-INFO
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     3699 2023-06-23 15:16:00.000000 mgtron-2.19.5/README.md
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-11 20:54:07.652216 mgtron-2.19.5/docs/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    17614 2023-06-23 15:16:01.000000 mgtron-2.19.5/docs/MGTron Command Description.docx
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    23088 2023-06-23 15:16:01.000000 mgtron-2.19.5/docs/MGTron Function Descriptions.docx
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-11 20:54:07.662216 mgtron-2.19.5/mgtron.egg-info/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     4198 2023-07-11 20:54:07.000000 mgtron-2.19.5/mgtron.egg-info/PKG-INFO
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2334 2023-07-11 20:54:07.000000 mgtron-2.19.5/mgtron.egg-info/SOURCES.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        1 2023-07-11 20:54:07.000000 mgtron-2.19.5/mgtron.egg-info/dependency_links.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       37 2023-07-11 20:54:07.000000 mgtron-2.19.5/mgtron.egg-info/entry_points.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2085 2023-07-11 20:54:07.000000 mgtron-2.19.5/mgtron.egg-info/requires.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       19 2023-07-11 20:54:07.000000 mgtron-2.19.5/mgtron.egg-info/top_level.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1161 2023-07-10 14:37:39.000000 mgtron-2.19.5/pyproject.toml
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2022 2023-07-10 17:50:34.000000 mgtron-2.19.5/requirements.txt
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       38 2023-07-11 20:54:07.822219 mgtron-2.19.5/setup.cfg
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-11 20:54:07.665549 mgtron-2.19.5/src/
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        1 2023-06-28 15:56:43.000000 mgtron-2.19.5/src/__init__.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-11 20:54:07.738884 mgtron-2.19.5/src/assets/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    83964 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/assets/CA logo without subtext.JPG
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    65978 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/assets/CA_subheading.png
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000) 12776672 2023-07-10 14:37:39.000000 mgtron-2.19.5/src/assets/blueio_rs
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)     1303 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/assets/init_cellantenna.sh
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      723 2023-07-10 14:37:39.000000 mgtron-2.19.5/src/assets/log_read
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      291 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/assets/mgtron.desktop
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2655 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/assets/mgtron.svg
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    67646 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/assets/network-wireless.ico
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000) 11314288 2023-07-10 14:37:39.000000 mgtron-2.19.5/src/assets/wifi_rs
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-11 20:54:07.782218 mgtron-2.19.5/src/ble/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/ble/__init__.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     3130 2023-07-10 14:37:39.000000 mgtron-2.19.5/src/ble/ble_data.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     8527 2023-07-10 14:37:39.000000 mgtron-2.19.5/src/ble/helpers.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      859 2023-06-30 12:43:53.000000 mgtron-2.19.5/src/ble/scanning.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-11 20:54:07.795551 mgtron-2.19.5/src/db/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.5/src/db/__init__.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.5/src/db/channel_1.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.5/src/db/channel_2.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.5/src/db/channel_3.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.5/src/db/channel_4.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.5/src/db/channel_5.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.5/src/db/channel_6.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.5/src/db/channel_7.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.5/src/db/channel_8.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    10853 2023-07-10 14:37:39.000000 mgtron-2.19.5/src/db/helpers.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     2516 2023-06-27 20:21:35.000000 mgtron-2.19.5/src/db/init_db.sql
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    10906 2023-06-27 20:21:35.000000 mgtron-2.19.5/src/db/long_save.json
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.5/src/db/long_save.json.lock
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    49152 2023-07-10 14:18:59.000000 mgtron-2.19.5/src/db/mgtron_db.db
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     9055 2023-07-10 14:37:39.000000 mgtron-2.19.5/src/db/models.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     1170 2023-06-27 20:21:35.000000 mgtron-2.19.5/src/db/quick_save.json
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-11 20:54:07.798885 mgtron-2.19.5/src/globals/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.5/src/globals/__init__.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     3642 2023-07-10 14:37:39.000000 mgtron-2.19.5/src/globals/helpers.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-11 20:54:07.798885 mgtron-2.19.5/src/gui/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       80 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/gui/__init__.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-11 20:54:07.805551 mgtron-2.19.5/src/gui/_configs/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/gui/_configs/card_1.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/gui/_configs/card_2.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/gui/_configs/card_3.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/gui/_configs/card_4.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/gui/_configs/card_5.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/gui/_configs/card_6.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      263 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/gui/_configs/card_7.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      269 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/gui/_configs/card_8.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       98 2023-06-21 12:37:32.000000 mgtron-2.19.5/src/gui/_configs/card_config.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      317 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/gui/_configs/mission_alpha.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      292 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/gui/_configs/mission_bravo.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      324 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/gui/_configs/mission_charlie.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      312 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/gui/_configs/mission_delta.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      273 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/gui/_configs/mission_echo.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      313 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/gui/_configs/mission_fox.ini
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      279 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/gui/_configs/mission_golf.ini
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-11 20:54:07.812218 mgtron-2.19.5/src/gui/fonts/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1260156 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/gui/fonts/MesloLGS NF Bold Italic.ttf
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1251424 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/gui/fonts/MesloLGS NF Italic.ttf
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)  1292408 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/gui/fonts/MesloLGS NF Regular.ttf
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    51299 2023-07-11 18:27:32.000000 mgtron-2.19.5/src/gui/helpers.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    10970 2023-07-10 20:18:55.000000 mgtron-2.19.5/src/gui/interface.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    43845 2023-07-11 18:29:09.000000 mgtron-2.19.5/src/main.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-11 20:54:07.815552 mgtron-2.19.5/src/tests/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       33 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/tests/__init__.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)       70 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/tests/test_ble.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    63110 2023-06-23 15:16:01.000000 mgtron-2.19.5/src/tests/test_configfiles.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    19824 2023-07-10 14:37:39.000000 mgtron-2.19.5/src/tests/test_helpers.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-11 20:54:07.815552 mgtron-2.19.5/src/wifi/
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)        0 2023-06-27 20:21:35.000000 mgtron-2.19.5/src/wifi/__init__.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)      507 2023-07-10 14:37:39.000000 mgtron-2.19.5/src/wifi/chasing.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)    15668 2023-07-11 20:30:06.000000 mgtron-2.19.5/src/wifi/helpers.py
+-rw-r--r--   0 djhunter67  (1000) djhunter67  (1000)     9516 2023-07-10 14:37:39.000000 mgtron-2.19.5/src/wifi/scanning.py
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-11 20:54:07.625548 mgtron-2.19.5/venv/
+drwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)        0 2023-07-11 20:54:07.818885 mgtron-2.19.5/venv/bin/
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      665 2023-06-12 19:48:50.000000 mgtron-2.19.5/venv/bin/rst2html.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      787 2023-06-12 19:48:50.000000 mgtron-2.19.5/venv/bin/rst2html4.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)     1122 2023-06-12 19:48:50.000000 mgtron-2.19.5/venv/bin/rst2html5.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      864 2023-06-12 19:48:50.000000 mgtron-2.19.5/venv/bin/rst2latex.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      687 2023-06-12 19:48:50.000000 mgtron-2.19.5/venv/bin/rst2man.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      853 2023-06-12 19:48:50.000000 mgtron-2.19.5/venv/bin/rst2odt.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      659 2023-06-12 19:48:50.000000 mgtron-2.19.5/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      672 2023-06-12 19:48:50.000000 mgtron-2.19.5/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      708 2023-06-12 19:48:50.000000 mgtron-2.19.5/venv/bin/rst2s5.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      944 2023-06-12 19:48:50.000000 mgtron-2.19.5/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      673 2023-06-12 19:48:50.000000 mgtron-2.19.5/venv/bin/rst2xml.py
+-rwxr-xr-x   0 djhunter67  (1000) djhunter67  (1000)      741 2023-06-12 19:48:50.000000 mgtron-2.19.5/venv/bin/rstpep2html.py
```

### Comparing `mgtron-2.19.4/.github/ISSUE_TEMPLATE/mgtron--.md` & `mgtron-2.19.5/.github/ISSUE_TEMPLATE/mgtron--.md`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/.github/ISSUE_TEMPLATE/mgtron_issue.yml` & `mgtron-2.19.5/.github/ISSUE_TEMPLATE/mgtron_issue.yml`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/.github/workflows/black_actions.yml` & `mgtron-2.19.5/.github/workflows/black_actions.yml`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/.github/workflows/pypi_action.yml` & `mgtron-2.19.5/.github/workflows/pypi_action.yml`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/CHANGELOG.md` & `mgtron-2.19.5/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/LICENSE.rst` & `mgtron-2.19.5/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/PKG-INFO` & `mgtron-2.19.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mgtron
-Version: 2.19.4
+Version: 2.19.5
 Summary: Package for MGTron GUI, a user interface for signal generation
 Author-email: Christerpher Hunter <chunter@cellantenna.com>
 Project-URL: Source, https://github.com/cellantenna/mg_tron
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
```

### Comparing `mgtron-2.19.4/README.md` & `mgtron-2.19.5/README.md`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/docs/MGTron Command Description.docx` & `mgtron-2.19.5/docs/MGTron Command Description.docx`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/docs/MGTron Function Descriptions.docx` & `mgtron-2.19.5/docs/MGTron Function Descriptions.docx`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/mgtron.egg-info/PKG-INFO` & `mgtron-2.19.5/mgtron.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mgtron
-Version: 2.19.4
+Version: 2.19.5
 Summary: Package for MGTron GUI, a user interface for signal generation
 Author-email: Christerpher Hunter <chunter@cellantenna.com>
 Project-URL: Source, https://github.com/cellantenna/mg_tron
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10
```

### Comparing `mgtron-2.19.4/mgtron.egg-info/SOURCES.txt` & `mgtron-2.19.5/mgtron.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/mgtron.egg-info/requires.txt` & `mgtron-2.19.5/mgtron.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/pyproject.toml` & `mgtron-2.19.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/requirements.txt` & `mgtron-2.19.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/src/assets/CA logo without subtext.JPG` & `mgtron-2.19.5/src/assets/CA logo without subtext.JPG`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/src/assets/CA_subheading.png` & `mgtron-2.19.5/src/assets/CA_subheading.png`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/src/assets/blueio_rs` & `mgtron-2.19.5/src/assets/blueio_rs`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/src/assets/init_cellantenna.sh` & `mgtron-2.19.5/src/assets/init_cellantenna.sh`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/src/assets/log_read` & `mgtron-2.19.5/src/assets/log_read`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/src/assets/mgtron.svg` & `mgtron-2.19.5/src/assets/mgtron.svg`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/src/assets/network-wireless.ico` & `mgtron-2.19.5/src/assets/network-wireless.ico`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/src/assets/wifi_rs` & `mgtron-2.19.5/src/assets/wifi_rs`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/src/ble/ble_data.py` & `mgtron-2.19.5/src/ble/ble_data.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/src/ble/helpers.py` & `mgtron-2.19.5/src/ble/helpers.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/src/ble/scanning.py` & `mgtron-2.19.5/src/ble/scanning.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/src/db/helpers.py` & `mgtron-2.19.5/src/db/helpers.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/src/db/init_db.sql` & `mgtron-2.19.5/src/db/init_db.sql`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/src/db/long_save.json` & `mgtron-2.19.5/src/db/long_save.json`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/src/db/mgtron_db.db` & `mgtron-2.19.5/src/db/mgtron_db.db`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/src/db/models.py` & `mgtron-2.19.5/src/db/models.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/src/db/quick_save.json` & `mgtron-2.19.5/src/db/quick_save.json`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/src/globals/helpers.py` & `mgtron-2.19.5/src/globals/helpers.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/src/gui/fonts/MesloLGS NF Bold Italic.ttf` & `mgtron-2.19.5/src/gui/fonts/MesloLGS NF Bold Italic.ttf`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/src/gui/fonts/MesloLGS NF Italic.ttf` & `mgtron-2.19.5/src/gui/fonts/MesloLGS NF Italic.ttf`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/src/gui/fonts/MesloLGS NF Regular.ttf` & `mgtron-2.19.5/src/gui/fonts/MesloLGS NF Regular.ttf`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/src/gui/helpers.py` & `mgtron-2.19.5/src/gui/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1578,14 +1578,45 @@
 start_server = threading.Thread(
     target=launch_wifi_server, args=(f"{ROOT}/src/assets/wifi_rs", ),
 )
 start_server.daemon = True
 start_server.start()
 
 
+def tooltips() -> None:
+    """Add tooltips to the GUI."""
+    loggey.debug(msg=f"{tooltips.__name__}()")
+
+    if not dpg.does_item_exist(item="tooltip"):
+        # Tooltip
+        with dpg.tooltip(
+                tag="tooltip_window",
+                parent="mssn_scan_jam"
+        ) as wifi_scan_jam_btn:
+            # Create the tooltip for every button
+            dpg.add_text(
+                tag="tooltip",
+                parent=wifi_scan_jam_btn,
+                default_value="Scan for WiFi networks"
+            )
+
+        with dpg.tooltip(
+                tag="tooltip_window_1",
+                parent="mssn_bluetooth_scan"
+        ) as ble_scan_jam_btn:
+            dpg.add_text(
+                tag="tooltip_1",
+                parent=ble_scan_jam_btn,
+                default_value="Scan for BLE devices"
+            )
+    else:
+        dpg.delete_item(item="tooltip_window")
+        dpg.delete_item(item="tooltip_window_1")
+
+
 def main():
     """Minor testing throughout development."""
     # if not compressed_data:
 
     # store the 'freq_dl' column in a df variable
     print(convert_power(40))
```

### Comparing `mgtron-2.19.4/src/gui/interface.py` & `mgtron-2.19.5/src/gui/interface.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/src/main.py` & `mgtron-2.19.5/src/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from .gui.helpers import device_refresh
 from .gui.helpers import kill_channel
 from .gui.helpers import reset_button
 from .gui.helpers import return_teensy
 from .gui.helpers import send_all_channels
 from .gui.helpers import send_vals
 from .gui.helpers import auto_send
+from .gui.helpers import tooltips
 
 from .wifi.helpers import wifi_scan_jam
 from .wifi.helpers import wifi_factory
 # from .wifi.helpers import wifi_kill_all
 
 from .db.helpers import custom_save
 from .db.helpers import quick_load
@@ -941,15 +942,15 @@
                     ###############
                     # Tracker Tag #
                     ###############
                     logger.info(msg="Bluetooth scan button initialized")
                     mission_golf_button = dpg.add_button(
                         tag="mssn_bluetooth_scan",
                         callback=bluetooth_scan_jam,
-                        label="TRACKER\n TAG",
+                        label="BLE TAG",
                         height=70,
                         width=BUTTON_WIDTH,
                         pos=(
                             (
                                 dpg.get_item_width(item="big_buttons") - 285) /
                             DIVISOR,
                             (
@@ -1097,27 +1098,30 @@
 
             ###############
             # Version Tag #
             ###############
 
             with dpg.child_window(
                 tag="version",
-                height=15,
-                width=70,
+                height=20,
+                width=80,
                 border=False,
                 no_scrollbar=True,
                 pos=(
-                    RESOLUTION[0] - 80,
+                    RESOLUTION[0] - 90,
                     RESOLUTION[1] - 30,
                 ),
             ):
 
-                dpg.add_text(
-                    default_value=f"ver. {__version__}",
+                dpg.add_button(
+                    label=f"ver. {__version__}",
                     tag="ver_num",
+                    callback=tooltips,
+                    height=20,
+                    width=80,
                 )
     except SystemError:
         logger.error(msg="No devices detected")
 
     try:  # Stop gap in case the font files cannot be found
         dpg.bind_font(font=ital_font)
         dpg.bind_item_font(item="ver_num", font=small_font)
```

### Comparing `mgtron-2.19.4/src/tests/test_configfiles.py` & `mgtron-2.19.5/src/tests/test_configfiles.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/src/tests/test_helpers.py` & `mgtron-2.19.5/src/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/src/wifi/helpers.py` & `mgtron-2.19.5/src/wifi/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,18 +81,19 @@
             dpg.configure_item(item="128", show=False, modal=False)
 
             # Makes no sense why configure first is needed to delete
             dpg.delete_item(item=129)
             dpg.delete_item(item="128")
 
             dpg.delete_item(item="wifi_scan_window")
+            os.remove("wifi_scan_results.yml")
 
             loggei.debug(msg="WiFi scan window deleted")
-        except SystemError:
-            loggei.warning(msg="Wifi scan window not found")
+        except (SystemError, FileNotFoundError) as err:
+            loggei.warning("WiFi scan btn: %s", err)
         finally:
             enable_select_btns(*WIFI_BTNS_LIST, _dpg=dpg)
 
     else:
         # Turn the button Orange
         dpg.bind_item_theme(
             item=sender,
@@ -180,32 +181,31 @@
     """Fill the scan results window with the data."""
     loggei.info("%s()", fill_scan_result.__name__)
 
     for i in (converted_data):
 
         # Before so length can be calculated
         if len(i[0]) == 0:
-            i[0] = "Hidden SSID"
+            i[0] = f"SSID_{i[1]}"
 
         ssid_difference = 32 - len(i[0])
         channel_diff = 4 - len(i[2])
         signal_diff = 3 - len(i[4])
 
         if len(i[0]) < 32:
             i[0] += " " * ssid_difference
         if len(i[2]) < 4:
             i[2] += " " * channel_diff
         if len(i[4]) < 3:
             i[4] += " " * signal_diff
         if len(i[5]) == 0:
             i[5] = "Open"
 
-        print(f"{[i]}")
+        # print(f"{[i]}")
 
-        # print(i)
         temp_list = []
         temp_list.append(i)
 
         dpg.add_button(
             # tag=i[1],  # Causes issue on re-scan
             parent=129,
             label=tabulate.tabulate(
@@ -228,28 +228,29 @@
 
 
 def indicate_tagged_results(sender, app_data, user_data: list[str]) -> None:
     """Change the color of the sender."""
     loggei.debug("%s()", indicate_tagged_results.__name__)
 
     loggei.info("User data: %s", user_data)
+    print(f"{F.YELLOW}User data{R}: {user_data}")
 
     # Make a toggle of the selected buttons
-    # if dpg.get_item_theme(item=sender) == blue_btn_theme:
-    # Turn the button green
-    # dpg.bind_item_theme(
-    # item=sender,
-    # theme=None,
-    # )
-    # else:
-    # Turn the button blue
-    dpg.bind_item_theme(
-        item=sender,
-        theme=blue_btn_theme,
-    )
+    if dpg.get_item_theme(item=sender) == blue_btn_theme:
+        # Turn the button green
+        dpg.bind_item_theme(
+            item=sender,
+            theme=None,
+        )
+    else:
+        # Turn the button blue
+        dpg.bind_item_theme(
+            item=sender,
+            theme=blue_btn_theme,
+        )
 
     # Turn user_data into a dict with user_data[0] as the key
     user_data = {
         user_data[0][0]: {
             "MAC": user_data[0][1],
             "CH": user_data[0][2],
             "FREQ": user_data[0][3].split(" ")[0],
```

### Comparing `mgtron-2.19.4/src/wifi/scanning.py` & `mgtron-2.19.5/src/wifi/scanning.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/venv/bin/rst2html.py` & `mgtron-2.19.5/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/venv/bin/rst2html4.py` & `mgtron-2.19.5/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/venv/bin/rst2html5.py` & `mgtron-2.19.5/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/venv/bin/rst2latex.py` & `mgtron-2.19.5/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/venv/bin/rst2man.py` & `mgtron-2.19.5/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/venv/bin/rst2odt.py` & `mgtron-2.19.5/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/venv/bin/rst2odt_prepstyles.py` & `mgtron-2.19.5/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/venv/bin/rst2pseudoxml.py` & `mgtron-2.19.5/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/venv/bin/rst2s5.py` & `mgtron-2.19.5/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/venv/bin/rst2xetex.py` & `mgtron-2.19.5/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/venv/bin/rst2xml.py` & `mgtron-2.19.5/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `mgtron-2.19.4/venv/bin/rstpep2html.py` & `mgtron-2.19.5/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

