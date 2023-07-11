# Comparing `tmp/aa_memberaudit-2.9.3.tar.gz` & `tmp/aa_memberaudit-2.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_memberaudit-2.9.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aa_memberaudit-2.9.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aa_memberaudit-2.9.3.tar` & `aa_memberaudit-2.9.4.tar`

### file list

```diff
@@ -1,239 +1,239 @@
--rw-r--r--   0        0        0     1070 2023-07-05 11:03:39.217293 aa_memberaudit-2.9.3/LICENSE
--rw-r--r--   0        0        0     5782 2023-07-05 11:03:39.217293 aa_memberaudit-2.9.3/README.md
--rw-r--r--   0        0        0      240 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.3/memberaudit/__init__.py
--rw-r--r--   0        0        0    24112 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.3/memberaudit/admin.py
--rw-r--r--   0        0        0     4548 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.3/memberaudit/app_settings.py
--rw-r--r--   0        0        0      407 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.3/memberaudit/apps.py
--rw-r--r--   0        0        0     1251 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.3/memberaudit/auth_hooks.py
--rw-r--r--   0        0        0     1271 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.3/memberaudit/checks.py
--rw-r--r--   0        0        0     1812 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.3/memberaudit/constants.py
--rw-r--r--   0        0        0        0 2023-07-05 11:09:35.048957 aa_memberaudit-2.9.3/memberaudit/core/__init__.py
--rw-r--r--   0        0        0    11526 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.3/memberaudit/core/data_exporters.py
--rw-r--r--   0        0        0    19456 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.3/memberaudit/core/eft_parser.py
--rw-r--r--   0        0        0     5563 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.3/memberaudit/core/fittings.py
--rw-r--r--   0        0        0     2244 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.3/memberaudit/core/skill_plans.py
--rw-r--r--   0        0        0     5362 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.3/memberaudit/core/skills.py
--rw-r--r--   0        0        0     3159 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.3/memberaudit/core/xml_converter.py
--rw-r--r--   0        0        0     3166 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.3/memberaudit/decorators.py
--rw-r--r--   0        0        0     3740 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.3/memberaudit/forms.py
--rw-r--r--   0        0        0     1820 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.3/memberaudit/helpers.py
--rw-r--r--   0        0        0      384 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.3/memberaudit/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    43105 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.3/memberaudit/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    43046 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.3/memberaudit/locale/django.pot
--rw-r--r--   0        0        0    43093 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.3/memberaudit/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      380 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.3/memberaudit/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    43093 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.3/memberaudit/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      450 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.3/memberaudit/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    43171 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.3/memberaudit/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      438 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.3/memberaudit/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    43159 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.3/memberaudit/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      379 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.3/memberaudit/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    43100 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.3/memberaudit/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      391 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.3/memberaudit/locale/ko_KR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    43112 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.3/memberaudit/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    26859 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.3/memberaudit/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    54952 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.3/memberaudit/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      609 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.3/memberaudit/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    43330 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.3/memberaudit/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      373 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.3/memberaudit/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    43086 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.3/memberaudit/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      102 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.3/memberaudit/management/commands/__init__.py
--rw-r--r--   0        0        0     1443 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.3/memberaudit/management/commands/memberaudit_data_export.py
--rw-r--r--   0        0        0     1374 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.3/memberaudit/management/commands/memberaudit_load_eve.py
--rw-r--r--   0        0        0     3859 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.3/memberaudit/management/commands/memberaudit_reset_characters.py
--rw-r--r--   0        0        0      740 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.3/memberaudit/management/commands/memberaudit_stats.py
--rw-r--r--   0        0        0     1941 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.3/memberaudit/management/commands/memberaudit_update_characters.py
--rw-r--r--   0        0        0        0 2023-07-05 11:09:35.052957 aa_memberaudit-2.9.3/memberaudit/managers/__init__.py
--rw-r--r--   0        0        0    13017 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.3/memberaudit/managers/character.py
--rw-r--r--   0        0        0    26850 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.3/memberaudit/managers/character_sections_1.py
--rw-r--r--   0        0        0    29910 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.3/memberaudit/managers/character_sections_2.py
--rw-r--r--   0        0        0    25043 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/managers/character_sections_3.py
--rw-r--r--   0        0        0    24472 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/managers/general.py
--rw-r--r--   0        0        0    65995 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/migrations/0001_initial_new.py
--rw-r--r--   0        0        0     3444 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/migrations/0002_add_mining_ledger.py
--rw-r--r--   0        0        0     1478 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/migrations/0003_add_notify_permission.py
--rw-r--r--   0        0        0      513 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/migrations/0004_character_is_disabled.py
--rw-r--r--   0        0        0     3819 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/migrations/0005_add_fw_stats.py
--rw-r--r--   0        0        0     5969 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/migrations/0006_add_localizations.py
--rw-r--r--   0        0        0     2129 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/migrations/0007_add_localization_2.py
--rw-r--r--   0        0        0     2727 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/migrations/0008_improve_skill_sets.py
--rw-r--r--   0        0        0     3274 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/migrations/0009_add_planetary_industry.py
--rw-r--r--   0        0        0        0 2023-07-05 11:09:35.052957 aa_memberaudit-2.9.3/memberaudit/migrations/__init__.py
--rw-r--r--   0        0        0     1117 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/models/__init__.py
--rw-r--r--   0        0        0    15243 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/models/character_sections_1.py
--rw-r--r--   0        0        0    13506 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/models/character_sections_2.py
--rw-r--r--   0        0        0    13923 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/models/character_sections_3.py
--rw-r--r--   0        0        0    26983 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/models/characters.py
--rw-r--r--   0        0        0      108 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/models/constants.py
--rw-r--r--   0        0        0    17213 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/models/general.py
--rw-r--r--   0        0        0      196 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/providers.py
--rw-r--r--   0        0        0      542 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/signals.py
--rw-r--r--   0        0        0      191 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/css/admin.css
--rw-r--r--   0        0        0      174 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/css/character_finder.css
--rw-r--r--   0        0        0     5820 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/css/character_viewer.css
--rw-r--r--   0        0        0       94 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/css/data_export.css
--rw-r--r--   0        0        0     1538 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/css/global.css
--rw-r--r--   0        0        0      646 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/css/global.min.css
--rw-r--r--   0        0        0     4331 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/css/launcher.css
--rw-r--r--   0        0        0     2765 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/css/launcher.min.css
--rw-r--r--   0        0        0     1363 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/css/memberaudit.css
--rw-r--r--   0        0        0      617 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/css/memberaudit.min.css
--rw-r--r--   0        0        0      611 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/css/reports.css
--rw-r--r--   0        0        0    43262 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/images/Spinner-1s-64px-dark.gif
--rw-r--r--   0        0        0    43381 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/images/Spinner-1s-64px-light.gif
--rw-r--r--   0        0        0     1862 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/images/charisma.png
--rw-r--r--   0        0        0      694 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/images/eve-prism.png
--rw-r--r--   0        0        0      220 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/images/evelogo.png
--rw-r--r--   0        0        0      595 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/images/evesearch.png
--rw-r--r--   0        0        0     1966 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/images/intelligence.png
--rw-r--r--   0        0        0     1809 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/images/memory.png
--rw-r--r--   0        0        0     1803 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/images/perception.png
--rw-r--r--   0        0        0     1782 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/images/willpower.png
--rw-r--r--   0        0        0      259 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/images/zkillboard.png
--rw-r--r--   0        0        0     5573 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/vendor/datatables/plugins/dataTables.rowGroup.min.js
--rw-r--r--   0        0        0     3908 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/vendor/datatables/plugins/datetime.js
--rw-r--r--   0        0        0     2529 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/vendor/datatables/plugins/filterDropDown.min.js
--rw-r--r--   0        0        0      384 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/vendor/datatables/plugins/rowGroup.bootstrap.min.css
--rw-r--r--   0        0        0      384 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/vendor/datatables/plugins/rowGroup.dataTables.min.css
--rw-r--r--   0        0        0    69950 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/static/memberaudit/vendor/moment/moment.min.js
--rw-r--r--   0        0        0    40015 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/tasks.py
--rw-r--r--   0        0        0      687 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/templates/admin/memberaudit/character/confirm_character_deletion.html
--rw-r--r--   0        0        0      488 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/templates/admin/memberaudit/skillset/change_list.html
--rw-r--r--   0        0        0      848 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/templates/admin/memberaudit/skillset/import_skills.html
--rw-r--r--   0        0        0      367 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/base.html
--rw-r--r--   0        0        0     4801 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/character_finder.html
--rw-r--r--   0        0        0    29413 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/character_viewer.html
--rw-r--r--   0        0        0     2932 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/data_export.html
--rw-r--r--   0        0        0     8515 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/launcher.html
--rw-r--r--   0        0        0     1238 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/modals/character_viewer/asset_container.html
--rw-r--r--   0        0        0     4307 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/modals/character_viewer/asset_container_content.html
--rw-r--r--   0        0        0     1713 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/modals/character_viewer/character_skill_set_details.html
--rw-r--r--   0        0        0     1246 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/modals/character_viewer/contract.html
--rw-r--r--   0        0        0     8075 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/modals/character_viewer/contract_content.html
--rw-r--r--   0        0        0      658 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/modals/character_viewer/contract_items.html
--rw-r--r--   0        0        0     1375 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/modals/character_viewer/mail.html
--rw-r--r--   0        0        0      382 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/modals/character_viewer/mail_content.html
--rw-r--r--   0        0        0     3880 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/modals/character_viewer/skill_set_content.html
--rw-r--r--   0        0        0     9005 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/overview.html
--rw-r--r--   0        0        0     1451 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/sidebar.html
--rw-r--r--   0        0        0      637 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/sidebar_character.html
--rw-r--r--   0        0        0     1256 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/assets.html
--rw-r--r--   0        0        0      560 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes.html
--rw-r--r--   0        0        0     2604 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes_content.html
--rw-r--r--   0        0        0      314 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_bio.html
--rw-r--r--   0        0        0      848 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contacts.html
--rw-r--r--   0        0        0      960 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contracts.html
--rw-r--r--   0        0        0      582 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history.html
--rw-r--r--   0        0        0      894 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html
--rw-r--r--   0        0        0      549 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats.html
--rw-r--r--   0        0        0     2786 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats_content.html
--rw-r--r--   0        0        0      563 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/implants.html
--rw-r--r--   0        0        0      721 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/jump_clones.html
--rw-r--r--   0        0        0      148 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/last_updated.html
--rw-r--r--   0        0        0      611 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/loyalty.html
--rw-r--r--   0        0        0     2878 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mails.html
--rw-r--r--   0        0        0      779 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mining_ledger.html
--rw-r--r--   0        0        0      885 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/planets.html
--rw-r--r--   0        0        0      669 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_queue.html
--rw-r--r--   0        0        0      882 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_sets.html
--rw-r--r--   0        0        0      592 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skills.html
--rw-r--r--   0        0        0      907 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html
--rw-r--r--   0        0        0      916 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_transactions.html
--rw-r--r--   0        0        0     3941 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs_navigation.html
--rw-r--r--   0        0        0     2674 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/menu.html
--rw-r--r--   0        0        0      292 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/reports/tabs/_compliance_color_code.html
--rw-r--r--   0        0        0      684 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/reports/tabs/corporation_compliance.html
--rw-r--r--   0        0        0      760 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/reports/tabs/skill_sets.html
--rw-r--r--   0        0        0      775 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/reports/tabs/user_compliance.html
--rw-r--r--   0        0        0      691 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/reports/tabs_navigation.html
--rw-r--r--   0        0        0      709 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/solar_system.html
--rw-r--r--   0        0        0     9420 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/reports.html
--rw-r--r--   0        0        0        0 2023-07-05 11:09:35.060958 aa_memberaudit-2.9.3/memberaudit/templatetags/__init__.py
--rw-r--r--   0        0        0      355 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.3/memberaudit/templatetags/memberaudit.py
--rw-r--r--   0        0        0        0 2023-07-05 11:09:35.060958 aa_memberaudit-2.9.3/memberaudit/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 11:09:35.060958 aa_memberaudit-2.9.3/memberaudit/tests/core/__init__.py
--rw-r--r--   0        0        0     6350 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.3/memberaudit/tests/core/test_core_xml_converter.py
--rw-r--r--   0        0        0    12725 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.3/memberaudit/tests/core/test_data_exporters.py
--rw-r--r--   0        0        0    22366 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.3/memberaudit/tests/core/test_eft_parser.py
--rw-r--r--   0        0        0     6371 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.3/memberaudit/tests/core/test_fittings.py
--rw-r--r--   0        0        0     4082 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.3/memberaudit/tests/core/test_skill_plans.py
--rw-r--r--   0        0        0     2458 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.3/memberaudit/tests/core/test_skills.py
--rw-r--r--   0        0        0        0 2023-07-05 11:09:35.060958 aa_memberaudit-2.9.3/memberaudit/tests/managers/__init__.py
--rw-r--r--   0        0        0    18357 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.3/memberaudit/tests/managers/test_character.py
--rw-r--r--   0        0        0    30687 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.3/memberaudit/tests/managers/test_character_sections_1.py
--rw-r--r--   0        0        0    37493 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.3/memberaudit/tests/managers/test_character_sections_2.py
--rw-r--r--   0        0        0    24751 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.3/memberaudit/tests/managers/test_character_sections_3.py
--rw-r--r--   0        0        0    46675 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.3/memberaudit/tests/managers/test_general.py
--rw-r--r--   0        0        0        0 2023-07-05 11:09:35.060958 aa_memberaudit-2.9.3/memberaudit/tests/models/__init__.py
--rw-r--r--   0        0        0     2963 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/models/test_character_sections.py
--rw-r--r--   0        0        0    36073 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/models/test_characters_1.py
--rw-r--r--   0        0        0    23158 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/models/test_characters_2.py
--rw-r--r--   0        0        0    10969 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/models/test_general.py
--rw-r--r--   0        0        0    15428 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/test_admin.py
--rw-r--r--   0        0        0     1807 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/test_auth_hooks.py
--rw-r--r--   0        0        0     1314 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/test_checks.py
--rw-r--r--   0        0        0     3487 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/test_commands.py
--rw-r--r--   0        0        0     5266 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/test_decorators.py
--rw-r--r--   0        0        0      900 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/test_factories.py
--rw-r--r--   0        0        0     3516 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/test_forms.py
--rw-r--r--   0        0        0     1476 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/test_helpers.py
--rw-r--r--   0        0        0    15465 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/test_integration.py
--rw-r--r--   0        0        0     1215 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/test_signals.py
--rw-r--r--   0        0        0    36377 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/test_tasks.py
--rw-r--r--   0        0        0      968 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/test_templatetags.py
--rw-r--r--   0        0        0     3822 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/test_utils.py
--rw-r--r--   0        0        0      267 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/testdata/__init__.py
--rw-r--r--   0        0        0     4432 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/testdata/create_eveuniverse.py
--rw-r--r--   0        0        0     4350 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/testdata/entities.json
--rw-r--r--   0        0        0     5298 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/testdata/esi_client_stub.py
--rw-r--r--   0        0        0    41017 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.3/memberaudit/tests/testdata/esi_testdata.json
--rw-r--r--   0        0        0  1225856 2023-07-05 11:03:39.269295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/eveuniverse.json
--rw-r--r--   0        0        0    13508 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/factories.py
--rw-r--r--   0        0        0      799 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/fittings/fitting_archon.txt
--rw-r--r--   0        0        0      889 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/fittings/fitting_archon_max.txt
--rw-r--r--   0        0        0      231 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/fittings/fitting_empty.txt
--rw-r--r--   0        0        0      503 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/fittings/fitting_eve_celestis_no_high_slots.txt
--rw-r--r--   0        0        0      193 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/fittings/fitting_eve_tristan_3.txt
--rw-r--r--   0        0        0      377 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/fittings/fitting_eve_tristian.txt
--rw-r--r--   0        0        0      293 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/fittings/fitting_eve_tristian_2.txt
--rw-r--r--   0        0        0       96 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/fittings/fitting_eve_tristian_empty.txt
--rw-r--r--   0        0        0      583 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/fittings/fitting_svipul.txt
--rw-r--r--   0        0        0      432 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/fittings/fitting_svipul_2.txt
--rw-r--r--   0        0        0      700 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/fittings/fitting_tengu.txt
--rw-r--r--   0        0        0      459 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/fittings/fitting_tristan.txt
--rw-r--r--   0        0        0      332 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/fittings/fitting_tristan_missing_rigs.txt
--rw-r--r--   0        0        0      410 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/fittings/fitting_tristan_no_title.txt
--rw-r--r--   0        0        0      460 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/fittings/fitting_tristan_unknown_types.txt
--rw-r--r--   0        0        0      455 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/fittings/fitting_unknown_ship_type.txt
--rw-r--r--   0        0        0     4268 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/generate_character.py
--rw-r--r--   0        0        0     3859 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/generate_doctrines.py
--rw-r--r--   0        0        0     3680 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/load_entities.py
--rw-r--r--   0        0        0      478 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/load_eveuniverse.py
--rw-r--r--   0        0        0     1188 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/load_locations.py
--rw-r--r--   0        0        0     1097 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/pilot_esi_error_handling.py
--rw-r--r--   0        0        0      838 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/testdata/profiler_toolbox.py
--rw-r--r--   0        0        0     5744 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/utils.py
--rw-r--r--   0        0        0        0 2023-07-05 11:09:35.064958 aa_memberaudit-2.9.3/memberaudit/tests/views/__init__.py
--rw-r--r--   0        0        0     9299 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/views/test_admin.py
--rw-r--r--   0        0        0     7089 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/views/test_character_finder.py
--rw-r--r--   0        0        0    32680 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/views/test_character_viewer_1.py
--rw-r--r--   0        0        0    24561 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/views/test_character_viewer_2.py
--rw-r--r--   0        0        0    14594 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/views/test_characters.py
--rw-r--r--   0        0        0     4101 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/views/test_data_export.py
--rw-r--r--   0        0        0    16249 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tests/views/test_reports.py
--rw-r--r--   0        0        0      710 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tools/clear_celery_once_locks.py
--rw-r--r--   0        0        0     3051 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tools/drop_tables.sql
--rw-r--r--   0        0        0      329 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/tools/total_size.sql
--rw-r--r--   0        0        0     7242 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/urls.py
--rw-r--r--   0        0        0     2367 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/utils.py
--rw-r--r--   0        0        0        0 2023-07-05 11:09:35.064958 aa_memberaudit-2.9.3/memberaudit/views/__init__.py
--rw-r--r--   0        0        0     1539 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/views/_common.py
--rw-r--r--   0        0        0     3510 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/views/admin.py
--rw-r--r--   0        0        0    12637 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/views/character_finder.py
--rw-r--r--   0        0        0    24043 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/views/character_viewer_1.py
--rw-r--r--   0        0        0    24147 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/views/character_viewer_2.py
--rw-r--r--   0        0        0     8029 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.3/memberaudit/views/characters.py
--rw-r--r--   0        0        0     2222 2023-07-05 11:03:39.277295 aa_memberaudit-2.9.3/memberaudit/views/data_export.py
--rw-r--r--   0        0        0    13139 2023-07-05 11:03:39.277295 aa_memberaudit-2.9.3/memberaudit/views/reports.py
--rw-r--r--   0        0        0     2285 2023-07-05 11:03:39.277295 aa_memberaudit-2.9.3/pyproject.toml
--rw-r--r--   0        0        0     7374 1970-01-01 00:00:00.000000 aa_memberaudit-2.9.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-05 11:03:39.217293 aa_memberaudit-2.9.4/LICENSE
+-rw-r--r--   0        0        0     5782 2023-07-05 11:03:39.217293 aa_memberaudit-2.9.4/README.md
+-rw-r--r--   0        0        0      240 2023-07-08 11:37:57.391051 aa_memberaudit-2.9.4/memberaudit/__init__.py
+-rw-r--r--   0        0        0    24112 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.4/memberaudit/admin.py
+-rw-r--r--   0        0        0     4548 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.4/memberaudit/app_settings.py
+-rw-r--r--   0        0        0      407 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.4/memberaudit/apps.py
+-rw-r--r--   0        0        0     1251 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.4/memberaudit/auth_hooks.py
+-rw-r--r--   0        0        0     1271 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.4/memberaudit/checks.py
+-rw-r--r--   0        0        0     1812 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.4/memberaudit/constants.py
+-rw-r--r--   0        0        0        0 2023-07-08 12:05:06.661279 aa_memberaudit-2.9.4/memberaudit/core/__init__.py
+-rw-r--r--   0        0        0    11526 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.4/memberaudit/core/data_exporters.py
+-rw-r--r--   0        0        0    19456 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.4/memberaudit/core/eft_parser.py
+-rw-r--r--   0        0        0     5563 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.4/memberaudit/core/fittings.py
+-rw-r--r--   0        0        0     2244 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.4/memberaudit/core/skill_plans.py
+-rw-r--r--   0        0        0     5362 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.4/memberaudit/core/skills.py
+-rw-r--r--   0        0        0     3159 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.4/memberaudit/core/xml_converter.py
+-rw-r--r--   0        0        0     3166 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.4/memberaudit/decorators.py
+-rw-r--r--   0        0        0     3740 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.4/memberaudit/forms.py
+-rw-r--r--   0        0        0     1820 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.4/memberaudit/helpers.py
+-rw-r--r--   0        0        0      384 2023-07-05 11:03:39.233293 aa_memberaudit-2.9.4/memberaudit/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    43105 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.4/memberaudit/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    43046 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.4/memberaudit/locale/django.pot
+-rw-r--r--   0        0        0    43093 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.4/memberaudit/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      380 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.4/memberaudit/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    43093 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.4/memberaudit/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      450 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.4/memberaudit/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    43171 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.4/memberaudit/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      438 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.4/memberaudit/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    43159 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.4/memberaudit/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      379 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.4/memberaudit/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    43100 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.4/memberaudit/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      391 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.4/memberaudit/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    43112 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.4/memberaudit/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    26859 2023-07-05 11:03:39.237294 aa_memberaudit-2.9.4/memberaudit/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    54952 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.4/memberaudit/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      609 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.4/memberaudit/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    43330 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.4/memberaudit/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      373 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.4/memberaudit/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    43086 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.4/memberaudit/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      102 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.4/memberaudit/management/commands/__init__.py
+-rw-r--r--   0        0        0     1443 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.4/memberaudit/management/commands/memberaudit_data_export.py
+-rw-r--r--   0        0        0     1374 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.4/memberaudit/management/commands/memberaudit_load_eve.py
+-rw-r--r--   0        0        0     3859 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.4/memberaudit/management/commands/memberaudit_reset_characters.py
+-rw-r--r--   0        0        0      740 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.4/memberaudit/management/commands/memberaudit_stats.py
+-rw-r--r--   0        0        0     1941 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.4/memberaudit/management/commands/memberaudit_update_characters.py
+-rw-r--r--   0        0        0        0 2023-07-08 12:05:06.661279 aa_memberaudit-2.9.4/memberaudit/managers/__init__.py
+-rw-r--r--   0        0        0    13017 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.4/memberaudit/managers/character.py
+-rw-r--r--   0        0        0    26850 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.4/memberaudit/managers/character_sections_1.py
+-rw-r--r--   0        0        0    29910 2023-07-05 11:03:39.241294 aa_memberaudit-2.9.4/memberaudit/managers/character_sections_2.py
+-rw-r--r--   0        0        0    25043 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.4/memberaudit/managers/character_sections_3.py
+-rw-r--r--   0        0        0    24472 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.4/memberaudit/managers/general.py
+-rw-r--r--   0        0        0    65995 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.4/memberaudit/migrations/0001_initial_new.py
+-rw-r--r--   0        0        0     3444 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.4/memberaudit/migrations/0002_add_mining_ledger.py
+-rw-r--r--   0        0        0     1478 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.4/memberaudit/migrations/0003_add_notify_permission.py
+-rw-r--r--   0        0        0      513 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.4/memberaudit/migrations/0004_character_is_disabled.py
+-rw-r--r--   0        0        0     3819 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.4/memberaudit/migrations/0005_add_fw_stats.py
+-rw-r--r--   0        0        0     5969 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.4/memberaudit/migrations/0006_add_localizations.py
+-rw-r--r--   0        0        0     2129 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.4/memberaudit/migrations/0007_add_localization_2.py
+-rw-r--r--   0        0        0     2727 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.4/memberaudit/migrations/0008_improve_skill_sets.py
+-rw-r--r--   0        0        0     3274 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.4/memberaudit/migrations/0009_add_planetary_industry.py
+-rw-r--r--   0        0        0        0 2023-07-08 12:05:06.661279 aa_memberaudit-2.9.4/memberaudit/migrations/__init__.py
+-rw-r--r--   0        0        0     1117 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.4/memberaudit/models/__init__.py
+-rw-r--r--   0        0        0    15243 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.4/memberaudit/models/character_sections_1.py
+-rw-r--r--   0        0        0    13506 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.4/memberaudit/models/character_sections_2.py
+-rw-r--r--   0        0        0    13923 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.4/memberaudit/models/character_sections_3.py
+-rw-r--r--   0        0        0    26983 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.4/memberaudit/models/characters.py
+-rw-r--r--   0        0        0      108 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.4/memberaudit/models/constants.py
+-rw-r--r--   0        0        0    17213 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.4/memberaudit/models/general.py
+-rw-r--r--   0        0        0      196 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.4/memberaudit/providers.py
+-rw-r--r--   0        0        0      542 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.4/memberaudit/signals.py
+-rw-r--r--   0        0        0      191 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.4/memberaudit/static/memberaudit/css/admin.css
+-rw-r--r--   0        0        0      174 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.4/memberaudit/static/memberaudit/css/character_finder.css
+-rw-r--r--   0        0        0     6060 2023-07-05 21:00:07.782512 aa_memberaudit-2.9.4/memberaudit/static/memberaudit/css/character_viewer.css
+-rw-r--r--   0        0        0       94 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.4/memberaudit/static/memberaudit/css/data_export.css
+-rw-r--r--   0        0        0     1538 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.4/memberaudit/static/memberaudit/css/global.css
+-rw-r--r--   0        0        0      646 2023-07-05 11:03:39.245294 aa_memberaudit-2.9.4/memberaudit/static/memberaudit/css/global.min.css
+-rw-r--r--   0        0        0     4331 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.4/memberaudit/static/memberaudit/css/launcher.css
+-rw-r--r--   0        0        0     2765 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.4/memberaudit/static/memberaudit/css/launcher.min.css
+-rw-r--r--   0        0        0     1363 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.4/memberaudit/static/memberaudit/css/memberaudit.css
+-rw-r--r--   0        0        0      617 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.4/memberaudit/static/memberaudit/css/memberaudit.min.css
+-rw-r--r--   0        0        0      611 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.4/memberaudit/static/memberaudit/css/reports.css
+-rw-r--r--   0        0        0    43262 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.4/memberaudit/static/memberaudit/images/Spinner-1s-64px-dark.gif
+-rw-r--r--   0        0        0    43381 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.4/memberaudit/static/memberaudit/images/Spinner-1s-64px-light.gif
+-rw-r--r--   0        0        0     1862 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.4/memberaudit/static/memberaudit/images/charisma.png
+-rw-r--r--   0        0        0      694 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.4/memberaudit/static/memberaudit/images/eve-prism.png
+-rw-r--r--   0        0        0      220 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.4/memberaudit/static/memberaudit/images/evelogo.png
+-rw-r--r--   0        0        0      595 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.4/memberaudit/static/memberaudit/images/evesearch.png
+-rw-r--r--   0        0        0     1966 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.4/memberaudit/static/memberaudit/images/intelligence.png
+-rw-r--r--   0        0        0     1809 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.4/memberaudit/static/memberaudit/images/memory.png
+-rw-r--r--   0        0        0     1803 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.4/memberaudit/static/memberaudit/images/perception.png
+-rw-r--r--   0        0        0     1782 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.4/memberaudit/static/memberaudit/images/willpower.png
+-rw-r--r--   0        0        0      259 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.4/memberaudit/static/memberaudit/images/zkillboard.png
+-rw-r--r--   0        0        0     5573 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.4/memberaudit/static/memberaudit/vendor/datatables/plugins/dataTables.rowGroup.min.js
+-rw-r--r--   0        0        0     3908 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.4/memberaudit/static/memberaudit/vendor/datatables/plugins/datetime.js
+-rw-r--r--   0        0        0     2529 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.4/memberaudit/static/memberaudit/vendor/datatables/plugins/filterDropDown.min.js
+-rw-r--r--   0        0        0      384 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.4/memberaudit/static/memberaudit/vendor/datatables/plugins/rowGroup.bootstrap.min.css
+-rw-r--r--   0        0        0      384 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.4/memberaudit/static/memberaudit/vendor/datatables/plugins/rowGroup.dataTables.min.css
+-rw-r--r--   0        0        0    69950 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.4/memberaudit/static/memberaudit/vendor/moment/moment.min.js
+-rw-r--r--   0        0        0    40015 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.4/memberaudit/tasks.py
+-rw-r--r--   0        0        0      687 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.4/memberaudit/templates/admin/memberaudit/character/confirm_character_deletion.html
+-rw-r--r--   0        0        0      488 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.4/memberaudit/templates/admin/memberaudit/skillset/change_list.html
+-rw-r--r--   0        0        0      848 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.4/memberaudit/templates/admin/memberaudit/skillset/import_skills.html
+-rw-r--r--   0        0        0      367 2023-07-05 11:03:39.249294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/base.html
+-rw-r--r--   0        0        0     4801 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/character_finder.html
+-rw-r--r--   0        0        0    29413 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/character_viewer.html
+-rw-r--r--   0        0        0     2932 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/data_export.html
+-rw-r--r--   0        0        0     8515 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/launcher.html
+-rw-r--r--   0        0        0     1238 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/modals/character_viewer/asset_container.html
+-rw-r--r--   0        0        0     4307 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/modals/character_viewer/asset_container_content.html
+-rw-r--r--   0        0        0     1713 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/modals/character_viewer/character_skill_set_details.html
+-rw-r--r--   0        0        0     1246 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/modals/character_viewer/contract.html
+-rw-r--r--   0        0        0     8075 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/modals/character_viewer/contract_content.html
+-rw-r--r--   0        0        0      658 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/modals/character_viewer/contract_items.html
+-rw-r--r--   0        0        0     1375 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/modals/character_viewer/mail.html
+-rw-r--r--   0        0        0      382 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/modals/character_viewer/mail_content.html
+-rw-r--r--   0        0        0     3880 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/modals/character_viewer/skill_set_content.html
+-rw-r--r--   0        0        0     9005 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/overview.html
+-rw-r--r--   0        0        0     1805 2023-07-05 21:00:07.782512 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/sidebar.html
+-rw-r--r--   0        0        0      650 2023-07-05 20:38:08.732596 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/sidebar_character.html
+-rw-r--r--   0        0        0     1256 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/assets.html
+-rw-r--r--   0        0        0      560 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes.html
+-rw-r--r--   0        0        0     2604 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes_content.html
+-rw-r--r--   0        0        0      314 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_bio.html
+-rw-r--r--   0        0        0      848 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contacts.html
+-rw-r--r--   0        0        0      960 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contracts.html
+-rw-r--r--   0        0        0      582 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history.html
+-rw-r--r--   0        0        0      894 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html
+-rw-r--r--   0        0        0      549 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats.html
+-rw-r--r--   0        0        0     2786 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats_content.html
+-rw-r--r--   0        0        0      563 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/implants.html
+-rw-r--r--   0        0        0      721 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/jump_clones.html
+-rw-r--r--   0        0        0      148 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/last_updated.html
+-rw-r--r--   0        0        0      611 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/loyalty.html
+-rw-r--r--   0        0        0     2878 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mails.html
+-rw-r--r--   0        0        0      779 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mining_ledger.html
+-rw-r--r--   0        0        0      885 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/planets.html
+-rw-r--r--   0        0        0      669 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_queue.html
+-rw-r--r--   0        0        0      882 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_sets.html
+-rw-r--r--   0        0        0      592 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skills.html
+-rw-r--r--   0        0        0      907 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html
+-rw-r--r--   0        0        0      916 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_transactions.html
+-rw-r--r--   0        0        0     3941 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs_navigation.html
+-rw-r--r--   0        0        0     2674 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/menu.html
+-rw-r--r--   0        0        0      292 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/reports/tabs/_compliance_color_code.html
+-rw-r--r--   0        0        0      684 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/reports/tabs/corporation_compliance.html
+-rw-r--r--   0        0        0      760 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/reports/tabs/skill_sets.html
+-rw-r--r--   0        0        0      775 2023-07-05 11:03:39.253294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/reports/tabs/user_compliance.html
+-rw-r--r--   0        0        0      691 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/reports/tabs_navigation.html
+-rw-r--r--   0        0        0      709 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/solar_system.html
+-rw-r--r--   0        0        0     9420 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/reports.html
+-rw-r--r--   0        0        0        0 2023-07-08 12:05:06.673279 aa_memberaudit-2.9.4/memberaudit/templatetags/__init__.py
+-rw-r--r--   0        0        0      355 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.4/memberaudit/templatetags/memberaudit.py
+-rw-r--r--   0        0        0        0 2023-07-08 12:05:06.677279 aa_memberaudit-2.9.4/memberaudit/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-08 12:05:06.677279 aa_memberaudit-2.9.4/memberaudit/tests/core/__init__.py
+-rw-r--r--   0        0        0     6350 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.4/memberaudit/tests/core/test_core_xml_converter.py
+-rw-r--r--   0        0        0    12725 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.4/memberaudit/tests/core/test_data_exporters.py
+-rw-r--r--   0        0        0    22366 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.4/memberaudit/tests/core/test_eft_parser.py
+-rw-r--r--   0        0        0     6371 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.4/memberaudit/tests/core/test_fittings.py
+-rw-r--r--   0        0        0     4082 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.4/memberaudit/tests/core/test_skill_plans.py
+-rw-r--r--   0        0        0     2458 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.4/memberaudit/tests/core/test_skills.py
+-rw-r--r--   0        0        0        0 2023-07-08 12:05:06.677279 aa_memberaudit-2.9.4/memberaudit/tests/managers/__init__.py
+-rw-r--r--   0        0        0    18357 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.4/memberaudit/tests/managers/test_character.py
+-rw-r--r--   0        0        0    30687 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.4/memberaudit/tests/managers/test_character_sections_1.py
+-rw-r--r--   0        0        0    37493 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.4/memberaudit/tests/managers/test_character_sections_2.py
+-rw-r--r--   0        0        0    24751 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.4/memberaudit/tests/managers/test_character_sections_3.py
+-rw-r--r--   0        0        0    46675 2023-07-05 11:03:39.257294 aa_memberaudit-2.9.4/memberaudit/tests/managers/test_general.py
+-rw-r--r--   0        0        0        0 2023-07-08 12:05:06.677279 aa_memberaudit-2.9.4/memberaudit/tests/models/__init__.py
+-rw-r--r--   0        0        0     2963 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.4/memberaudit/tests/models/test_character_sections.py
+-rw-r--r--   0        0        0    36073 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.4/memberaudit/tests/models/test_characters_1.py
+-rw-r--r--   0        0        0    23158 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.4/memberaudit/tests/models/test_characters_2.py
+-rw-r--r--   0        0        0    10969 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.4/memberaudit/tests/models/test_general.py
+-rw-r--r--   0        0        0    15428 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.4/memberaudit/tests/test_admin.py
+-rw-r--r--   0        0        0     1807 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.4/memberaudit/tests/test_auth_hooks.py
+-rw-r--r--   0        0        0     1314 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.4/memberaudit/tests/test_checks.py
+-rw-r--r--   0        0        0     3487 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.4/memberaudit/tests/test_commands.py
+-rw-r--r--   0        0        0     5266 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.4/memberaudit/tests/test_decorators.py
+-rw-r--r--   0        0        0      900 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.4/memberaudit/tests/test_factories.py
+-rw-r--r--   0        0        0     3516 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.4/memberaudit/tests/test_forms.py
+-rw-r--r--   0        0        0     1476 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.4/memberaudit/tests/test_helpers.py
+-rw-r--r--   0        0        0    15465 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.4/memberaudit/tests/test_integration.py
+-rw-r--r--   0        0        0     1215 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.4/memberaudit/tests/test_signals.py
+-rw-r--r--   0        0        0    36377 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.4/memberaudit/tests/test_tasks.py
+-rw-r--r--   0        0        0      968 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.4/memberaudit/tests/test_templatetags.py
+-rw-r--r--   0        0        0     3822 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.4/memberaudit/tests/test_utils.py
+-rw-r--r--   0        0        0      267 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.4/memberaudit/tests/testdata/__init__.py
+-rw-r--r--   0        0        0     4432 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.4/memberaudit/tests/testdata/create_eveuniverse.py
+-rw-r--r--   0        0        0     4350 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.4/memberaudit/tests/testdata/entities.json
+-rw-r--r--   0        0        0     5298 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.4/memberaudit/tests/testdata/esi_client_stub.py
+-rw-r--r--   0        0        0    41017 2023-07-05 11:03:39.261294 aa_memberaudit-2.9.4/memberaudit/tests/testdata/esi_testdata.json
+-rw-r--r--   0        0        0  1225856 2023-07-05 11:03:39.269295 aa_memberaudit-2.9.4/memberaudit/tests/testdata/eveuniverse.json
+-rw-r--r--   0        0        0    13508 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/tests/testdata/factories.py
+-rw-r--r--   0        0        0      799 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/tests/testdata/fittings/fitting_archon.txt
+-rw-r--r--   0        0        0      889 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/tests/testdata/fittings/fitting_archon_max.txt
+-rw-r--r--   0        0        0      231 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/tests/testdata/fittings/fitting_empty.txt
+-rw-r--r--   0        0        0      503 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/tests/testdata/fittings/fitting_eve_celestis_no_high_slots.txt
+-rw-r--r--   0        0        0      193 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/tests/testdata/fittings/fitting_eve_tristan_3.txt
+-rw-r--r--   0        0        0      377 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/tests/testdata/fittings/fitting_eve_tristian.txt
+-rw-r--r--   0        0        0      293 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/tests/testdata/fittings/fitting_eve_tristian_2.txt
+-rw-r--r--   0        0        0       96 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/tests/testdata/fittings/fitting_eve_tristian_empty.txt
+-rw-r--r--   0        0        0      583 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/tests/testdata/fittings/fitting_svipul.txt
+-rw-r--r--   0        0        0      432 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/tests/testdata/fittings/fitting_svipul_2.txt
+-rw-r--r--   0        0        0      700 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/tests/testdata/fittings/fitting_tengu.txt
+-rw-r--r--   0        0        0      459 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/tests/testdata/fittings/fitting_tristan.txt
+-rw-r--r--   0        0        0      332 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/tests/testdata/fittings/fitting_tristan_missing_rigs.txt
+-rw-r--r--   0        0        0      410 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/tests/testdata/fittings/fitting_tristan_no_title.txt
+-rw-r--r--   0        0        0      460 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/tests/testdata/fittings/fitting_tristan_unknown_types.txt
+-rw-r--r--   0        0        0      455 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/tests/testdata/fittings/fitting_unknown_ship_type.txt
+-rw-r--r--   0        0        0     4268 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/tests/testdata/generate_character.py
+-rw-r--r--   0        0        0     3859 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/tests/testdata/generate_doctrines.py
+-rw-r--r--   0        0        0     3680 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/tests/testdata/load_entities.py
+-rw-r--r--   0        0        0      478 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/tests/testdata/load_eveuniverse.py
+-rw-r--r--   0        0        0     1188 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/tests/testdata/load_locations.py
+-rw-r--r--   0        0        0     1097 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/tests/testdata/pilot_esi_error_handling.py
+-rw-r--r--   0        0        0      838 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/tests/testdata/profiler_toolbox.py
+-rw-r--r--   0        0        0     5744 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/tests/utils.py
+-rw-r--r--   0        0        0        0 2023-07-08 12:05:06.681280 aa_memberaudit-2.9.4/memberaudit/tests/views/__init__.py
+-rw-r--r--   0        0        0     9299 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/tests/views/test_admin.py
+-rw-r--r--   0        0        0     7089 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/tests/views/test_character_finder.py
+-rw-r--r--   0        0        0    32680 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/tests/views/test_character_viewer_1.py
+-rw-r--r--   0        0        0    24561 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/tests/views/test_character_viewer_2.py
+-rw-r--r--   0        0        0    14594 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/tests/views/test_characters.py
+-rw-r--r--   0        0        0     4101 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/tests/views/test_data_export.py
+-rw-r--r--   0        0        0    16249 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/tests/views/test_reports.py
+-rw-r--r--   0        0        0      710 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/tools/clear_celery_once_locks.py
+-rw-r--r--   0        0        0     3051 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/tools/drop_tables.sql
+-rw-r--r--   0        0        0      329 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/tools/total_size.sql
+-rw-r--r--   0        0        0     7242 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/urls.py
+-rw-r--r--   0        0        0     2367 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/utils.py
+-rw-r--r--   0        0        0        0 2023-07-08 12:05:06.681280 aa_memberaudit-2.9.4/memberaudit/views/__init__.py
+-rw-r--r--   0        0        0     1539 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/views/_common.py
+-rw-r--r--   0        0        0     3510 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/views/admin.py
+-rw-r--r--   0        0        0    12637 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/views/character_finder.py
+-rw-r--r--   0        0        0    24043 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/views/character_viewer_1.py
+-rw-r--r--   0        0        0    24147 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/views/character_viewer_2.py
+-rw-r--r--   0        0        0     8029 2023-07-05 11:03:39.273295 aa_memberaudit-2.9.4/memberaudit/views/characters.py
+-rw-r--r--   0        0        0     2222 2023-07-05 11:03:39.277295 aa_memberaudit-2.9.4/memberaudit/views/data_export.py
+-rw-r--r--   0        0        0    13139 2023-07-05 11:03:39.277295 aa_memberaudit-2.9.4/memberaudit/views/reports.py
+-rw-r--r--   0        0        0     2285 2023-07-05 11:03:39.277295 aa_memberaudit-2.9.4/pyproject.toml
+-rw-r--r--   0        0        0     7374 1970-01-01 00:00:00.000000 aa_memberaudit-2.9.4/PKG-INFO
```

### Comparing `aa_memberaudit-2.9.3/LICENSE` & `aa_memberaudit-2.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/README.md` & `aa_memberaudit-2.9.4/README.md`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/admin.py` & `aa_memberaudit-2.9.4/memberaudit/admin.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/app_settings.py` & `aa_memberaudit-2.9.4/memberaudit/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/auth_hooks.py` & `aa_memberaudit-2.9.4/memberaudit/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/checks.py` & `aa_memberaudit-2.9.4/memberaudit/checks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/constants.py` & `aa_memberaudit-2.9.4/memberaudit/constants.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/core/data_exporters.py` & `aa_memberaudit-2.9.4/memberaudit/core/data_exporters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/core/eft_parser.py` & `aa_memberaudit-2.9.4/memberaudit/core/eft_parser.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/core/fittings.py` & `aa_memberaudit-2.9.4/memberaudit/core/fittings.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/core/skill_plans.py` & `aa_memberaudit-2.9.4/memberaudit/core/skill_plans.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/core/skills.py` & `aa_memberaudit-2.9.4/memberaudit/core/skills.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/core/xml_converter.py` & `aa_memberaudit-2.9.4/memberaudit/core/xml_converter.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/decorators.py` & `aa_memberaudit-2.9.4/memberaudit/decorators.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/forms.py` & `aa_memberaudit-2.9.4/memberaudit/forms.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/helpers.py` & `aa_memberaudit-2.9.4/memberaudit/helpers.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/locale/de/LC_MESSAGES/django.po` & `aa_memberaudit-2.9.4/memberaudit/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/locale/django.pot` & `aa_memberaudit-2.9.4/memberaudit/locale/django.pot`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/locale/en/LC_MESSAGES/django.po` & `aa_memberaudit-2.9.4/memberaudit/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/locale/es/LC_MESSAGES/django.po` & `aa_memberaudit-2.9.4/memberaudit/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/locale/fr_FR/LC_MESSAGES/django.po` & `aa_memberaudit-2.9.4/memberaudit/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/locale/it_IT/LC_MESSAGES/django.po` & `aa_memberaudit-2.9.4/memberaudit/locale/it_IT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/locale/ja/LC_MESSAGES/django.po` & `aa_memberaudit-2.9.4/memberaudit/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/locale/ko_KR/LC_MESSAGES/django.po` & `aa_memberaudit-2.9.4/memberaudit/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/locale/ru/LC_MESSAGES/django.mo` & `aa_memberaudit-2.9.4/memberaudit/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/locale/ru/LC_MESSAGES/django.po` & `aa_memberaudit-2.9.4/memberaudit/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/locale/uk/LC_MESSAGES/django.mo` & `aa_memberaudit-2.9.4/memberaudit/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/locale/uk/LC_MESSAGES/django.po` & `aa_memberaudit-2.9.4/memberaudit/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_memberaudit-2.9.4/memberaudit/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/management/commands/memberaudit_data_export.py` & `aa_memberaudit-2.9.4/memberaudit/management/commands/memberaudit_data_export.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/management/commands/memberaudit_load_eve.py` & `aa_memberaudit-2.9.4/memberaudit/management/commands/memberaudit_load_eve.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/management/commands/memberaudit_reset_characters.py` & `aa_memberaudit-2.9.4/memberaudit/management/commands/memberaudit_reset_characters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/management/commands/memberaudit_stats.py` & `aa_memberaudit-2.9.4/memberaudit/management/commands/memberaudit_stats.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/management/commands/memberaudit_update_characters.py` & `aa_memberaudit-2.9.4/memberaudit/management/commands/memberaudit_update_characters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/managers/character.py` & `aa_memberaudit-2.9.4/memberaudit/managers/character.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/managers/character_sections_1.py` & `aa_memberaudit-2.9.4/memberaudit/managers/character_sections_1.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/managers/character_sections_2.py` & `aa_memberaudit-2.9.4/memberaudit/managers/character_sections_2.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/managers/character_sections_3.py` & `aa_memberaudit-2.9.4/memberaudit/managers/character_sections_3.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/managers/general.py` & `aa_memberaudit-2.9.4/memberaudit/managers/general.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/migrations/0001_initial_new.py` & `aa_memberaudit-2.9.4/memberaudit/migrations/0001_initial_new.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/migrations/0002_add_mining_ledger.py` & `aa_memberaudit-2.9.4/memberaudit/migrations/0002_add_mining_ledger.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/migrations/0003_add_notify_permission.py` & `aa_memberaudit-2.9.4/memberaudit/migrations/0003_add_notify_permission.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/migrations/0004_character_is_disabled.py` & `aa_memberaudit-2.9.4/memberaudit/migrations/0004_character_is_disabled.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/migrations/0005_add_fw_stats.py` & `aa_memberaudit-2.9.4/memberaudit/migrations/0005_add_fw_stats.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/migrations/0006_add_localizations.py` & `aa_memberaudit-2.9.4/memberaudit/migrations/0006_add_localizations.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/migrations/0007_add_localization_2.py` & `aa_memberaudit-2.9.4/memberaudit/migrations/0007_add_localization_2.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/migrations/0008_improve_skill_sets.py` & `aa_memberaudit-2.9.4/memberaudit/migrations/0008_improve_skill_sets.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/migrations/0009_add_planetary_industry.py` & `aa_memberaudit-2.9.4/memberaudit/migrations/0009_add_planetary_industry.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/models/__init__.py` & `aa_memberaudit-2.9.4/memberaudit/models/__init__.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/models/character_sections_1.py` & `aa_memberaudit-2.9.4/memberaudit/models/character_sections_1.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/models/character_sections_2.py` & `aa_memberaudit-2.9.4/memberaudit/models/character_sections_2.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/models/character_sections_3.py` & `aa_memberaudit-2.9.4/memberaudit/models/character_sections_3.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/models/characters.py` & `aa_memberaudit-2.9.4/memberaudit/models/characters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/models/general.py` & `aa_memberaudit-2.9.4/memberaudit/models/general.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/signals.py` & `aa_memberaudit-2.9.4/memberaudit/signals.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/css/character_viewer.css` & `aa_memberaudit-2.9.4/memberaudit/static/memberaudit/css/character_viewer.css`

 * *Files 11% similar despite different names*

```diff
@@ -230,15 +230,14 @@
     }
 
     /* sidebar */
     .sidebar_characters {
         list-style-type: none;
         margin: 0;
         padding: 0;
-        overflow-x: auto;
     }
 
     .sidebar_character {
         margin: 0.2rem 0;
         white-space: nowrap;
     }
 
@@ -252,14 +251,26 @@
 
     .sidebar_character>a {
         display: block;
         padding: 0.2rem 0.4rem;
         text-decoration: none;
     }
 
+    .sidebar-character-list-item {
+        display: flex;
+        align-items: center;
+        justify-content: flex-start;
+    }
+
+    .sidebar-character-list-item-name {
+        text-overflow: ellipsis;
+        white-space: nowrap;
+        overflow: hidden;
+    }
+
     .template-light-mode .sidebar_character>a {
         color: rgb(44, 62, 80);
     }
 
     .template-dark-mode .sidebar_character>a {
         color: rgb(255, 255, 255);
     }
```

### Comparing `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/css/global.css` & `aa_memberaudit-2.9.4/memberaudit/static/memberaudit/css/global.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/css/global.min.css` & `aa_memberaudit-2.9.4/memberaudit/static/memberaudit/css/global.min.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/css/launcher.css` & `aa_memberaudit-2.9.4/memberaudit/static/memberaudit/css/launcher.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/css/launcher.min.css` & `aa_memberaudit-2.9.4/memberaudit/static/memberaudit/css/launcher.min.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/css/memberaudit.css` & `aa_memberaudit-2.9.4/memberaudit/static/memberaudit/css/memberaudit.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/css/memberaudit.min.css` & `aa_memberaudit-2.9.4/memberaudit/static/memberaudit/css/memberaudit.min.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/css/reports.css` & `aa_memberaudit-2.9.4/memberaudit/static/memberaudit/css/reports.css`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/images/Spinner-1s-64px-dark.gif` & `aa_memberaudit-2.9.4/memberaudit/static/memberaudit/images/Spinner-1s-64px-dark.gif`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/images/Spinner-1s-64px-light.gif` & `aa_memberaudit-2.9.4/memberaudit/static/memberaudit/images/Spinner-1s-64px-light.gif`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/images/charisma.png` & `aa_memberaudit-2.9.4/memberaudit/static/memberaudit/images/charisma.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/images/eve-prism.png` & `aa_memberaudit-2.9.4/memberaudit/static/memberaudit/images/eve-prism.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/images/evesearch.png` & `aa_memberaudit-2.9.4/memberaudit/static/memberaudit/images/evesearch.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/images/intelligence.png` & `aa_memberaudit-2.9.4/memberaudit/static/memberaudit/images/intelligence.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/images/memory.png` & `aa_memberaudit-2.9.4/memberaudit/static/memberaudit/images/memory.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/images/perception.png` & `aa_memberaudit-2.9.4/memberaudit/static/memberaudit/images/perception.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/images/willpower.png` & `aa_memberaudit-2.9.4/memberaudit/static/memberaudit/images/willpower.png`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/vendor/datatables/plugins/dataTables.rowGroup.min.js` & `aa_memberaudit-2.9.4/memberaudit/static/memberaudit/vendor/datatables/plugins/dataTables.rowGroup.min.js`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/vendor/datatables/plugins/datetime.js` & `aa_memberaudit-2.9.4/memberaudit/static/memberaudit/vendor/datatables/plugins/datetime.js`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/vendor/datatables/plugins/filterDropDown.min.js` & `aa_memberaudit-2.9.4/memberaudit/static/memberaudit/vendor/datatables/plugins/filterDropDown.min.js`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/static/memberaudit/vendor/moment/moment.min.js` & `aa_memberaudit-2.9.4/memberaudit/static/memberaudit/vendor/moment/moment.min.js`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tasks.py` & `aa_memberaudit-2.9.4/memberaudit/tasks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/admin/memberaudit/character/confirm_character_deletion.html` & `aa_memberaudit-2.9.4/memberaudit/templates/admin/memberaudit/character/confirm_character_deletion.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/admin/memberaudit/skillset/import_skills.html` & `aa_memberaudit-2.9.4/memberaudit/templates/admin/memberaudit/skillset/import_skills.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/character_finder.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/character_finder.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/character_viewer.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/character_viewer.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/data_export.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/data_export.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/launcher.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/launcher.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/modals/character_viewer/asset_container.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/modals/character_viewer/asset_container.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/modals/character_viewer/asset_container_content.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/modals/character_viewer/asset_container_content.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/modals/character_viewer/character_skill_set_details.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/modals/character_viewer/character_skill_set_details.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/modals/character_viewer/contract.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/modals/character_viewer/contract.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/modals/character_viewer/contract_content.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/modals/character_viewer/contract_content.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/modals/character_viewer/contract_items.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/modals/character_viewer/contract_items.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/modals/character_viewer/mail.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/modals/character_viewer/mail.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/modals/character_viewer/skill_set_content.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/modals/character_viewer/skill_set_content.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/overview.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/overview.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/sidebar.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/sidebar.html`

 * *Files 17% similar despite different names*

```diff
@@ -4,24 +4,28 @@
 
 <!-- Sidebar panel-->
 <div class="panel panel-default">
     <div class="panel-heading">{% translate 'Characters' %}</div>
     <div class="panel-body">
         <ul class="sidebar_characters">
             {% for character in all_characters %}
-                {% if character.memberaudit_character_pk and character.has_access%}
-                    <li class="sidebar_character character-{{ character.memberaudit_character_pk }}{% if auth_character.character_name == character.character_name %} active{% endif %}">
+                {% if character.memberaudit_character_pk and character.has_access %}
+                    <li class="sidebar_character character-{{ character.memberaudit_character_pk }}{% if auth_character.character_name == character.character_name %} active{% endif %}" title="{{ character.character_name }}">
                         <a href="{% url 'memberaudit:character_viewer' character.memberaudit_character_pk %}">
-                            {% include "memberaudit/partials/character_viewer/sidebar_character.html" %}
+                            <span class="sidebar-character-list-item text-nowrap">
+                                {% include "memberaudit/partials/character_viewer/sidebar_character.html" %}
+                            </span>
                         </a>
                     </li>
                 {% else %}
-                    <li class="sidebar_character_disabled">
-                        {% include "memberaudit/partials/character_viewer/sidebar_character.html" %}&nbsp;
-                        <i class="fas fa-exclamation-triangle text-muted" title="{% translate 'Unregistered character' %}"></i>
+                    <li class="sidebar_character_disabled" title="{{ character.character_name }}">
+                        <span class="sidebar-character-list-item text-nowrap">
+                            {% include "memberaudit/partials/character_viewer/sidebar_character.html" %}&nbsp;
+                            <i class="sidebar-character-list-item-icon fas fa-exclamation-triangle text-muted" title="{% translate 'Unregistered character' %}"></i>
+                        </span>
                     </li>
                 {% endif %}
             {% empty %}
                 <li class="sidebar_character_disabled">
                     <span class="text-muted">{% translate '(orphan)' %}</span>
                 </li>
             {% endfor %}
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 {% load i18n %} {% load static %} {% load evelinks %}
 {% translate 'Characters' %}
     * {% for character in all_characters %} {% if
-      character.memberaudit_character_pk and character.has_access%}
-    * {%_include_"memberaudit/partials/character_viewer/sidebar_character.html"
-      %}
+      character.memberaudit_character_pk and character.has_access %}
+    * _{%_include_"memberaudit/partials/character_viewer/
+      sidebar_character.html"_%}_
     * {% else %}
-    * {% include "memberaudit/partials/character_viewer/sidebar_character.html"
-      %} 
+    *  {% include "memberaudit/partials/character_viewer/
+      sidebar_character.html" %} 
     * {% endif %} {% empty %}
     * {% translate '(orphan)' %}
     * {% endfor %}
```

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/assets.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/assets.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes_content.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/character_attributes_content.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contacts.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contacts.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contracts.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/contracts.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/corporation_history_2.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats_content.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/fw_stats_content.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/implants.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/implants.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/jump_clones.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/jump_clones.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/loyalty.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/loyalty.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mails.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mails.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mining_ledger.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/mining_ledger.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/planets.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/planets.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_queue.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_queue.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_sets.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skill_sets.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skills.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/skills.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_journal.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_transactions.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs/wallet_transactions.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/character_viewer/tabs_navigation.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/character_viewer/tabs_navigation.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/menu.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/menu.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/reports/tabs/corporation_compliance.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/reports/tabs/corporation_compliance.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/reports/tabs/skill_sets.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/reports/tabs/skill_sets.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/reports/tabs/user_compliance.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/reports/tabs/user_compliance.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/reports/tabs_navigation.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/reports/tabs_navigation.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/partials/solar_system.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/partials/solar_system.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/templates/memberaudit/reports.html` & `aa_memberaudit-2.9.4/memberaudit/templates/memberaudit/reports.html`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/core/test_core_xml_converter.py` & `aa_memberaudit-2.9.4/memberaudit/tests/core/test_core_xml_converter.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/core/test_data_exporters.py` & `aa_memberaudit-2.9.4/memberaudit/tests/core/test_data_exporters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/core/test_eft_parser.py` & `aa_memberaudit-2.9.4/memberaudit/tests/core/test_eft_parser.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/core/test_fittings.py` & `aa_memberaudit-2.9.4/memberaudit/tests/core/test_fittings.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/core/test_skill_plans.py` & `aa_memberaudit-2.9.4/memberaudit/tests/core/test_skill_plans.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/core/test_skills.py` & `aa_memberaudit-2.9.4/memberaudit/tests/core/test_skills.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/managers/test_character.py` & `aa_memberaudit-2.9.4/memberaudit/tests/managers/test_character.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/managers/test_character_sections_1.py` & `aa_memberaudit-2.9.4/memberaudit/tests/managers/test_character_sections_1.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/managers/test_character_sections_2.py` & `aa_memberaudit-2.9.4/memberaudit/tests/managers/test_character_sections_2.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/managers/test_character_sections_3.py` & `aa_memberaudit-2.9.4/memberaudit/tests/managers/test_character_sections_3.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/managers/test_general.py` & `aa_memberaudit-2.9.4/memberaudit/tests/managers/test_general.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/models/test_character_sections.py` & `aa_memberaudit-2.9.4/memberaudit/tests/models/test_character_sections.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/models/test_characters_1.py` & `aa_memberaudit-2.9.4/memberaudit/tests/models/test_characters_1.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/models/test_characters_2.py` & `aa_memberaudit-2.9.4/memberaudit/tests/models/test_characters_2.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/models/test_general.py` & `aa_memberaudit-2.9.4/memberaudit/tests/models/test_general.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/test_admin.py` & `aa_memberaudit-2.9.4/memberaudit/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/test_auth_hooks.py` & `aa_memberaudit-2.9.4/memberaudit/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/test_checks.py` & `aa_memberaudit-2.9.4/memberaudit/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/test_commands.py` & `aa_memberaudit-2.9.4/memberaudit/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/test_decorators.py` & `aa_memberaudit-2.9.4/memberaudit/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/test_factories.py` & `aa_memberaudit-2.9.4/memberaudit/tests/test_factories.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/test_forms.py` & `aa_memberaudit-2.9.4/memberaudit/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/test_helpers.py` & `aa_memberaudit-2.9.4/memberaudit/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/test_integration.py` & `aa_memberaudit-2.9.4/memberaudit/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/test_signals.py` & `aa_memberaudit-2.9.4/memberaudit/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/test_tasks.py` & `aa_memberaudit-2.9.4/memberaudit/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/test_templatetags.py` & `aa_memberaudit-2.9.4/memberaudit/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/test_utils.py` & `aa_memberaudit-2.9.4/memberaudit/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/testdata/create_eveuniverse.py` & `aa_memberaudit-2.9.4/memberaudit/tests/testdata/create_eveuniverse.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/testdata/entities.json` & `aa_memberaudit-2.9.4/memberaudit/tests/testdata/entities.json`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/testdata/esi_client_stub.py` & `aa_memberaudit-2.9.4/memberaudit/tests/testdata/esi_client_stub.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/testdata/esi_testdata.json` & `aa_memberaudit-2.9.4/memberaudit/tests/testdata/esi_testdata.json`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/testdata/eveuniverse.json` & `aa_memberaudit-2.9.4/memberaudit/tests/testdata/eveuniverse.json`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/testdata/factories.py` & `aa_memberaudit-2.9.4/memberaudit/tests/testdata/factories.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/testdata/fittings/fitting_archon.txt` & `aa_memberaudit-2.9.4/memberaudit/tests/testdata/fittings/fitting_archon.txt`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/testdata/fittings/fitting_archon_max.txt` & `aa_memberaudit-2.9.4/memberaudit/tests/testdata/fittings/fitting_archon_max.txt`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/testdata/fittings/fitting_svipul.txt` & `aa_memberaudit-2.9.4/memberaudit/tests/testdata/fittings/fitting_svipul.txt`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/testdata/fittings/fitting_tengu.txt` & `aa_memberaudit-2.9.4/memberaudit/tests/testdata/fittings/fitting_tengu.txt`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/testdata/generate_character.py` & `aa_memberaudit-2.9.4/memberaudit/tests/testdata/generate_character.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/testdata/generate_doctrines.py` & `aa_memberaudit-2.9.4/memberaudit/tests/testdata/generate_doctrines.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/testdata/load_entities.py` & `aa_memberaudit-2.9.4/memberaudit/tests/testdata/load_entities.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/testdata/load_locations.py` & `aa_memberaudit-2.9.4/memberaudit/tests/testdata/load_locations.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/testdata/pilot_esi_error_handling.py` & `aa_memberaudit-2.9.4/memberaudit/tests/testdata/pilot_esi_error_handling.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/testdata/profiler_toolbox.py` & `aa_memberaudit-2.9.4/memberaudit/tests/testdata/profiler_toolbox.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/utils.py` & `aa_memberaudit-2.9.4/memberaudit/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/views/test_admin.py` & `aa_memberaudit-2.9.4/memberaudit/tests/views/test_admin.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/views/test_character_finder.py` & `aa_memberaudit-2.9.4/memberaudit/tests/views/test_character_finder.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/views/test_character_viewer_1.py` & `aa_memberaudit-2.9.4/memberaudit/tests/views/test_character_viewer_1.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/views/test_character_viewer_2.py` & `aa_memberaudit-2.9.4/memberaudit/tests/views/test_character_viewer_2.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/views/test_characters.py` & `aa_memberaudit-2.9.4/memberaudit/tests/views/test_characters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/views/test_data_export.py` & `aa_memberaudit-2.9.4/memberaudit/tests/views/test_data_export.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tests/views/test_reports.py` & `aa_memberaudit-2.9.4/memberaudit/tests/views/test_reports.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tools/clear_celery_once_locks.py` & `aa_memberaudit-2.9.4/memberaudit/tools/clear_celery_once_locks.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/tools/drop_tables.sql` & `aa_memberaudit-2.9.4/memberaudit/tools/drop_tables.sql`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/urls.py` & `aa_memberaudit-2.9.4/memberaudit/urls.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/utils.py` & `aa_memberaudit-2.9.4/memberaudit/utils.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/views/_common.py` & `aa_memberaudit-2.9.4/memberaudit/views/_common.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/views/admin.py` & `aa_memberaudit-2.9.4/memberaudit/views/admin.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/views/character_finder.py` & `aa_memberaudit-2.9.4/memberaudit/views/character_finder.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/views/character_viewer_1.py` & `aa_memberaudit-2.9.4/memberaudit/views/character_viewer_1.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/views/character_viewer_2.py` & `aa_memberaudit-2.9.4/memberaudit/views/character_viewer_2.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/views/characters.py` & `aa_memberaudit-2.9.4/memberaudit/views/characters.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/views/data_export.py` & `aa_memberaudit-2.9.4/memberaudit/views/data_export.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/memberaudit/views/reports.py` & `aa_memberaudit-2.9.4/memberaudit/views/reports.py`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/pyproject.toml` & `aa_memberaudit-2.9.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aa_memberaudit-2.9.3/PKG-INFO` & `aa_memberaudit-2.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-memberaudit
-Version: 2.9.3
+Version: 2.9.4
 Summary: "An Alliance Auth app that provides full access to Eve characters
 Keywords: allianceauth,eveonline,memberaudit
 Author-email: Erik Kalkoken <kalkoken87@gmail.com>, Peter Pfeufer <develop@ppfeufer.de>, Rebecca Murphy <rebecca@rcmurphy.me>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

