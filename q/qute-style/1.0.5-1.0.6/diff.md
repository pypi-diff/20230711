# Comparing `tmp/qute_style-1.0.5.tar.gz` & `tmp/qute_style-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qute_style-1.0.5.tar", max compression
+gzip compressed data, was "qute_style-1.0.6.tar", max compression
```

## Comparing `qute_style-1.0.5.tar` & `qute_style-1.0.6.tar`

### file list

```diff
@@ -1,151 +1,151 @@
--rw-r--r--   0        0        0     1087 2023-07-03 09:22:48.464578 qute_style-1.0.5/LICENSE
--rw-r--r--   0        0        0     5391 2023-07-03 09:22:48.464578 qute_style-1.0.5/README.md
--rw-r--r--   0        0        0     1040 2023-07-03 09:22:48.468578 qute_style-1.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/__init__.py
--rw-r--r--   0        0        0        0 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/dev/__init__.py
--rw-r--r--   0        0        0     6719 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/dev/dev_functions.py
--rw-r--r--   0        0        0     8916 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/dev/mocks.py
--rw-r--r--   0        0        0        0 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/gen/__init__.py
--rw-r--r--   0        0        0    29831 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/gen/ui_test_window.py
--rw-r--r--   0        0        0     5330 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/gen/ui_whats_new_window.py
--rw-r--r--   0        0        0     1813 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/helper.py
--rw-r--r--   0        0        0        0 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/py.typed
--rw-r--r--   0        0        0     8198 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/qs_application.py
--rw-r--r--   0        0        0    29069 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/qs_main_window.py
--rw-r--r--   0        0        0     6436 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/qs_message_box.py
--rw-r--r--   0        0        0    26591 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/qute_style.py
--rw-r--r--   0        0        0      104 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/png_icons/transparent_icon.png
--rw-r--r--   0        0        0      466 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/accept.svg
--rw-r--r--   0        0        0     3012 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/accept_circle.svg
--rw-r--r--   0        0        0     2379 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/active_menu.svg
--rw-r--r--   0        0        0     2139 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/add.svg
--rw-r--r--   0        0        0     2160 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/add_circle.svg
--rw-r--r--   0        0        0     1939 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/admin.svg
--rw-r--r--   0        0        0     2721 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/admin_panel.svg
--rw-r--r--   0        0        0     2002 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/arrow_back.svg
--rw-r--r--   0        0        0      394 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/arrow_down.svg
--rw-r--r--   0        0        0      398 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/arrow_right.svg
--rw-r--r--   0        0        0     2004 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/block.svg
--rw-r--r--   0        0        0     3858 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/bug.svg
--rw-r--r--   0        0        0     2145 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/check_circle.svg
--rw-r--r--   0        0        0      208 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/checked.svg
--rw-r--r--   0        0        0      324 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/chevron_left.svg
--rw-r--r--   0        0        0      441 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/clipboard.svg
--rw-r--r--   0        0        0     2271 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/close.svg
--rw-r--r--   0        0        0     2289 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/close_circle.svg
--rw-r--r--   0        0        0      363 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/cloud_upload.svg
--rw-r--r--   0        0        0     2068 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/copy.svg
--rw-r--r--   0        0        0     2255 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/cps_trends.svg
--rw-r--r--   0        0        0     2019 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/delete.svg
--rw-r--r--   0        0        0      699 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/delete_forever.svg
--rw-r--r--   0        0        0     1928 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/delete_import.svg
--rw-r--r--   0        0        0     1881 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/document.svg
--rw-r--r--   0        0        0      785 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/document_scanner.svg
--rw-r--r--   0        0        0     1989 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/error.svg
--rw-r--r--   0        0        0     1575 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/expand_less.svg
--rw-r--r--   0        0        0     2062 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/expand_more.svg
--rw-r--r--   0        0        0     1961 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/file_distributor.svg
--rw-r--r--   0        0        0      482 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/filter.svg
--rw-r--r--   0        0        0     2023 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/folder_open.svg
--rw-r--r--   0        0        0     2880 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/fullscreen.svg
--rw-r--r--   0        0        0     2877 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/fullscreen_exit.svg
--rw-r--r--   0        0        0     2236 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/heart_broken.svg
--rw-r--r--   0        0        0     2642 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/help.svg
--rw-r--r--   0        0        0     2206 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/home.svg
--rw-r--r--   0        0        0     4370 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/ian_manager.svg
--rw-r--r--   0        0        0     4191 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/icon_PSE.svg
--rw-r--r--   0        0        0     2597 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/import.svg
--rw-r--r--   0        0        0     1939 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/info.svg
--rw-r--r--   0        0        0      491 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/inventory.svg
--rw-r--r--   0        0        0     2018 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/lidl_budget.svg
--rw-r--r--   0        0        0     2485 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/menu.svg
--rw-r--r--   0        0        0     1747 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/minimize.svg
--rw-r--r--   0        0        0     2498 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/nav_updater.svg
--rw-r--r--   0        0        0     2505 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/new_releases.svg
--rw-r--r--   0        0        0     2932 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/news.svg
--rw-r--r--   0        0        0     3184 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/no_icon.svg
--rw-r--r--   0        0        0     2214 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/package_commander.svg
--rw-r--r--   0        0        0     2475 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/palette.svg
--rw-r--r--   0        0        0     2709 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/pap.svg
--rw-r--r--   0        0        0      175 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/partial_checked.svg
--rw-r--r--   0        0        0     2236 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/protocol_creator.svg
--rw-r--r--   0        0        0      549 2023-07-03 09:22:48.468578 qute_style-1.0.5/qute_style/resources/svg_icons/pzf_widget.svg
--rw-r--r--   0        0        0     3073 2023-07-03 09:22:48.472578 qute_style-1.0.5/qute_style/resources/svg_icons/qt.svg
--rw-r--r--   0        0        0     2684 2023-07-03 09:22:48.472578 qute_style-1.0.5/qute_style/resources/svg_icons/read_more.svg
--rw-r--r--   0        0        0     2468 2023-07-03 09:22:48.472578 qute_style-1.0.5/qute_style/resources/svg_icons/refresh.svg
--rw-r--r--   0        0        0     1910 2023-07-03 09:22:48.472578 qute_style-1.0.5/qute_style/resources/svg_icons/report_merger.svg
--rw-r--r--   0        0        0     2113 2023-07-03 09:22:48.472578 qute_style-1.0.5/qute_style/resources/svg_icons/sap_excel.svg
--rw-r--r--   0        0        0     2244 2023-07-03 09:22:48.472578 qute_style-1.0.5/qute_style/resources/svg_icons/save.svg
--rw-r--r--   0        0        0     2390 2023-07-03 09:22:48.472578 qute_style-1.0.5/qute_style/resources/svg_icons/save_alt.svg
--rw-r--r--   0        0        0     2398 2023-07-03 09:22:48.472578 qute_style-1.0.5/qute_style/resources/svg_icons/search.svg
--rw-r--r--   0        0        0     2103 2023-07-03 09:22:48.472578 qute_style-1.0.5/qute_style/resources/svg_icons/send.svg
--rw-r--r--   0        0        0     3472 2023-07-03 09:22:48.472578 qute_style-1.0.5/qute_style/resources/svg_icons/settings.svg
--rw-r--r--   0        0        0      184 2023-07-03 09:22:48.472578 qute_style-1.0.5/qute_style/resources/svg_icons/status.svg
--rw-r--r--   0        0        0     2448 2023-07-03 09:22:48.472578 qute_style-1.0.5/qute_style/resources/svg_icons/swap.svg
--rw-r--r--   0        0        0     2778 2023-07-03 09:22:48.472578 qute_style-1.0.5/qute_style/resources/svg_icons/sync.svg
--rw-r--r--   0        0        0     2336 2023-07-03 09:22:48.472578 qute_style-1.0.5/qute_style/resources/svg_icons/template_selector.svg
--rw-r--r--   0        0        0     2531 2023-07-03 09:22:48.472578 qute_style-1.0.5/qute_style/resources/svg_icons/testbase_manager.svg
--rw-r--r--   0        0        0     1965 2023-07-03 09:22:48.472578 qute_style-1.0.5/qute_style/resources/svg_icons/todo_circle.svg
--rw-r--r--   0        0        0     2257 2023-07-03 09:22:48.472578 qute_style-1.0.5/qute_style/resources/svg_icons/undo.svg
--rw-r--r--   0        0        0    32469 2023-07-03 09:22:48.472578 qute_style-1.0.5/qute_style/resources/svg_images/banner_qute_style.svg
--rw-r--r--   0        0        0     7237 2023-07-03 09:22:48.472578 qute_style-1.0.5/qute_style/resources/svg_images/logo_chemistry.svg
--rw-r--r--   0        0        0     8429 2023-07-03 09:22:48.472578 qute_style-1.0.5/qute_style/resources/svg_images/logo_labmonitor.svg
--rw-r--r--   0        0        0    39983 2023-07-03 09:22:48.472578 qute_style-1.0.5/qute_style/resources/svg_images/logo_qute_style.svg
--rw-r--r--   0        0        0     8278 2023-07-03 09:22:48.472578 qute_style-1.0.5/qute_style/resources/svg_images/logo_toolbox.svg
--rw-r--r--   0        0        0   323159 2023-07-03 09:22:48.472578 qute_style-1.0.5/qute_style/resources_rc.py
--rw-r--r--   0        0        0     1657 2023-07-03 09:22:48.472578 qute_style-1.0.5/qute_style/startup_threads.py
--rw-r--r--   0        0        0    23017 2023-07-03 09:22:48.472578 qute_style-1.0.5/qute_style/style.py
--rw-r--r--   0        0        0    20664 2023-07-03 09:22:48.472578 qute_style-1.0.5/qute_style/ui/test_window.ui
--rw-r--r--   0        0        0     3001 2023-07-03 09:22:48.472578 qute_style-1.0.5/qute_style/ui/whats_new_window.ui
--rw-r--r--   0        0        0        0 2023-07-03 09:22:48.472578 qute_style-1.0.5/qute_style/widgets/__init__.py
--rw-r--r--   0        0        0     1165 2023-07-03 09:22:48.472578 qute_style-1.0.5/qute_style/widgets/background_frame.py
--rw-r--r--   0        0        0     2993 2023-07-03 09:22:48.476578 qute_style-1.0.5/qute_style/widgets/base_widgets.py
--rw-r--r--   0        0        0     5533 2023-07-03 09:22:48.476578 qute_style-1.0.5/qute_style/widgets/color_manager.py
--rw-r--r--   0        0        0     1089 2023-07-03 09:22:48.476578 qute_style-1.0.5/qute_style/widgets/credit_bar.py
--rw-r--r--   0        0        0     4440 2023-07-03 09:22:48.476578 qute_style-1.0.5/qute_style/widgets/custom_icon_engine.py
--rw-r--r--   0        0        0      483 2023-07-03 09:22:48.476578 qute_style-1.0.5/qute_style/widgets/div.py
--rw-r--r--   0        0        0     1745 2023-07-03 09:22:48.476578 qute_style-1.0.5/qute_style/widgets/drop_label.py
--rw-r--r--   0        0        0     7164 2023-07-03 09:22:48.476578 qute_style-1.0.5/qute_style/widgets/grips.py
--rw-r--r--   0        0        0    16689 2023-07-03 09:22:48.476578 qute_style-1.0.5/qute_style/widgets/home_page.py
--rw-r--r--   0        0        0     2049 2023-07-03 09:22:48.476578 qute_style-1.0.5/qute_style/widgets/icon.py
--rw-r--r--   0        0        0     7697 2023-07-03 09:22:48.476578 qute_style-1.0.5/qute_style/widgets/icon_button.py
--rw-r--r--   0        0        0     3474 2023-07-03 09:22:48.476578 qute_style-1.0.5/qute_style/widgets/icon_tooltip_button.py
--rw-r--r--   0        0        0     6849 2023-07-03 09:22:48.476578 qute_style-1.0.5/qute_style/widgets/left_column.py
--rw-r--r--   0        0        0      808 2023-07-03 09:22:48.476578 qute_style-1.0.5/qute_style/widgets/left_column_close_button.py
--rw-r--r--   0        0        0     8775 2023-07-03 09:22:48.476578 qute_style-1.0.5/qute_style/widgets/left_menu.py
--rw-r--r--   0        0        0     7075 2023-07-03 09:22:48.476578 qute_style-1.0.5/qute_style/widgets/left_menu_button.py
--rw-r--r--   0        0        0    11127 2023-07-03 09:22:48.476578 qute_style-1.0.5/qute_style/widgets/spinner.py
--rw-r--r--   0        0        0    14811 2023-07-03 09:22:48.476578 qute_style-1.0.5/qute_style/widgets/styled_combobox.py
--rw-r--r--   0        0        0     1878 2023-07-03 09:22:48.476578 qute_style-1.0.5/qute_style/widgets/text_truncator.py
--rw-r--r--   0        0        0     6869 2023-07-03 09:22:48.476578 qute_style-1.0.5/qute_style/widgets/title_bar.py
--rw-r--r--   0        0        0     1733 2023-07-03 09:22:48.476578 qute_style-1.0.5/qute_style/widgets/title_button.py
--rw-r--r--   0        0        0     4334 2023-07-03 09:22:48.476578 qute_style-1.0.5/qute_style/widgets/toggle.py
--rw-r--r--   0        0        0     1046 2023-07-03 09:22:48.476578 qute_style-1.0.5/qute_style/widgets/tooltip.py
--rw-r--r--   0        0        0        0 2023-07-03 09:22:48.476578 qute_style-1.0.5/qute_style_examples/__init__.py
--rw-r--r--   0        0        0      136 2023-07-03 09:22:48.476578 qute_style-1.0.5/qute_style_examples/__main__.py
--rw-r--r--   0        0        0    21042 2023-07-03 09:22:48.476578 qute_style-1.0.5/qute_style_examples/example_images/color_manager.PNG
--rw-r--r--   0        0        0    79278 2023-07-03 09:22:48.476578 qute_style-1.0.5/qute_style_examples/example_images/custom_style.PNG
--rw-r--r--   0        0        0    62693 2023-07-03 09:22:48.476578 qute_style-1.0.5/qute_style_examples/example_images/darcula.PNG
--rw-r--r--   0        0        0     3902 2023-07-03 09:22:48.476578 qute_style-1.0.5/qute_style_examples/example_images/drop_label.PNG
--rw-r--r--   0        0        0    50435 2023-07-03 09:22:48.480578 qute_style-1.0.5/qute_style_examples/example_images/highbridge_grey.PNG
--rw-r--r--   0        0        0     4594 2023-07-03 09:22:48.480578 qute_style-1.0.5/qute_style_examples/example_images/information_messagebox.PNG
--rw-r--r--   0        0        0    30905 2023-07-03 09:22:48.480578 qute_style-1.0.5/qute_style_examples/example_images/princesspink.PNG
--rw-r--r--   0        0        0    30041 2023-07-03 09:22:48.480578 qute_style-1.0.5/qute_style_examples/example_images/rubyred.PNG
--rw-r--r--   0        0        0    30867 2023-07-03 09:22:48.480578 qute_style-1.0.5/qute_style_examples/example_images/snowwhite.PNG
--rw-r--r--   0        0        0    56113 2023-07-03 09:22:48.480578 qute_style-1.0.5/qute_style_examples/example_images/widgets_display.PNG
--rw-r--r--   0        0        0     2818 2023-07-03 09:22:48.480578 qute_style-1.0.5/qute_style_examples/main.py
--rw-r--r--   0        0        0     1244 2023-07-03 09:22:48.480578 qute_style-1.0.5/qute_style_examples/sample_classes.py
--rw-r--r--   0        0        0     3414 2023-07-03 09:22:48.480578 qute_style-1.0.5/qute_style_examples/sample_main_window.py
--rw-r--r--   0        0        0     9665 2023-07-03 09:22:48.480578 qute_style-1.0.5/qute_style_examples/sample_widgets.py
--rw-r--r--   0        0        0      110 2023-07-03 09:22:48.480578 qute_style-1.0.5/qute_style_examples/test_changelog/1.01/1.json
--rw-r--r--   0        0        0      211 2023-07-03 09:22:48.480578 qute_style-1.0.5/qute_style_examples/test_changelog/1.01/2.json
--rw-r--r--   0        0        0    45119 2023-07-03 09:22:48.480578 qute_style-1.0.5/qute_style_examples/test_changelog/1.01/bug.png
--rw-r--r--   0        0        0       42 2023-07-03 09:22:48.480578 qute_style-1.0.5/qute_style_examples/test_changelog/1.01/meta.json
--rw-r--r--   0        0        0      167 2023-07-03 09:22:48.480578 qute_style-1.0.5/qute_style_examples/test_changelog/1.10/1.json
--rw-r--r--   0        0        0      209 2023-07-03 09:22:48.480578 qute_style-1.0.5/qute_style_examples/test_changelog/1.10/2.json
--rw-r--r--   0        0        0    45119 2023-07-03 09:22:48.480578 qute_style-1.0.5/qute_style_examples/test_changelog/1.10/bug.png
--rw-r--r--   0        0        0       42 2023-07-03 09:22:48.480578 qute_style-1.0.5/qute_style_examples/test_changelog/1.10/meta.json
--rw-r--r--   0        0        0      114 2023-07-03 09:22:48.480578 qute_style-1.0.5/qute_style_examples/test_changelog/1.100/1.json
--rw-r--r--   0        0        0       97 2023-07-03 09:22:48.480578 qute_style-1.0.5/qute_style_examples/test_changelog/1.100/2.json
--rw-r--r--   0        0        0       42 2023-07-03 09:22:48.480578 qute_style-1.0.5/qute_style_examples/test_changelog/1.100/meta.json
--rw-r--r--   0        0        0     6244 1970-01-01 00:00:00.000000 qute_style-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-07-11 09:54:00.851824 qute_style-1.0.6/LICENSE
+-rw-r--r--   0        0        0     5391 2023-07-11 09:54:00.851824 qute_style-1.0.6/README.md
+-rw-r--r--   0        0        0     1042 2023-07-11 09:54:00.851824 qute_style-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-11 09:54:00.851824 qute_style-1.0.6/qute_style/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 09:54:00.851824 qute_style-1.0.6/qute_style/dev/__init__.py
+-rw-r--r--   0        0        0     6719 2023-07-11 09:54:00.851824 qute_style-1.0.6/qute_style/dev/dev_functions.py
+-rw-r--r--   0        0        0     8916 2023-07-11 09:54:00.851824 qute_style-1.0.6/qute_style/dev/mocks.py
+-rw-r--r--   0        0        0        0 2023-07-11 09:54:00.851824 qute_style-1.0.6/qute_style/gen/__init__.py
+-rw-r--r--   0        0        0    29831 2023-07-11 09:54:00.851824 qute_style-1.0.6/qute_style/gen/ui_test_window.py
+-rw-r--r--   0        0        0     5330 2023-07-11 09:54:00.851824 qute_style-1.0.6/qute_style/gen/ui_whats_new_window.py
+-rw-r--r--   0        0        0     1813 2023-07-11 09:54:00.851824 qute_style-1.0.6/qute_style/helper.py
+-rw-r--r--   0        0        0        0 2023-07-11 09:54:00.851824 qute_style-1.0.6/qute_style/py.typed
+-rw-r--r--   0        0        0     8198 2023-07-11 09:54:00.851824 qute_style-1.0.6/qute_style/qs_application.py
+-rw-r--r--   0        0        0    29861 2023-07-11 09:54:00.851824 qute_style-1.0.6/qute_style/qs_main_window.py
+-rw-r--r--   0        0        0     6436 2023-07-11 09:54:00.851824 qute_style-1.0.6/qute_style/qs_message_box.py
+-rw-r--r--   0        0        0    26592 2023-07-11 09:54:00.851824 qute_style-1.0.6/qute_style/qute_style.py
+-rw-r--r--   0        0        0      104 2023-07-11 09:54:00.851824 qute_style-1.0.6/qute_style/resources/png_icons/transparent_icon.png
+-rw-r--r--   0        0        0      466 2023-07-11 09:54:00.851824 qute_style-1.0.6/qute_style/resources/svg_icons/accept.svg
+-rw-r--r--   0        0        0     3012 2023-07-11 09:54:00.851824 qute_style-1.0.6/qute_style/resources/svg_icons/accept_circle.svg
+-rw-r--r--   0        0        0     2379 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/active_menu.svg
+-rw-r--r--   0        0        0     2139 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/add.svg
+-rw-r--r--   0        0        0     2160 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/add_circle.svg
+-rw-r--r--   0        0        0     1939 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/admin.svg
+-rw-r--r--   0        0        0     2721 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/admin_panel.svg
+-rw-r--r--   0        0        0     2002 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/arrow_back.svg
+-rw-r--r--   0        0        0      394 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/arrow_down.svg
+-rw-r--r--   0        0        0      398 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/arrow_right.svg
+-rw-r--r--   0        0        0     2004 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/block.svg
+-rw-r--r--   0        0        0     3858 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/bug.svg
+-rw-r--r--   0        0        0     2145 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/check_circle.svg
+-rw-r--r--   0        0        0      208 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/checked.svg
+-rw-r--r--   0        0        0      324 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/chevron_left.svg
+-rw-r--r--   0        0        0      441 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/clipboard.svg
+-rw-r--r--   0        0        0     2271 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/close.svg
+-rw-r--r--   0        0        0     2289 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/close_circle.svg
+-rw-r--r--   0        0        0      363 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/cloud_upload.svg
+-rw-r--r--   0        0        0     2068 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/copy.svg
+-rw-r--r--   0        0        0     2255 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/cps_trends.svg
+-rw-r--r--   0        0        0     2019 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/delete.svg
+-rw-r--r--   0        0        0      699 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/delete_forever.svg
+-rw-r--r--   0        0        0     1928 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/delete_import.svg
+-rw-r--r--   0        0        0     1881 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/document.svg
+-rw-r--r--   0        0        0      785 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/document_scanner.svg
+-rw-r--r--   0        0        0     1989 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/error.svg
+-rw-r--r--   0        0        0     1575 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/expand_less.svg
+-rw-r--r--   0        0        0     2062 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/expand_more.svg
+-rw-r--r--   0        0        0     1961 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/file_distributor.svg
+-rw-r--r--   0        0        0      482 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/filter.svg
+-rw-r--r--   0        0        0     2023 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/folder_open.svg
+-rw-r--r--   0        0        0     2880 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/fullscreen.svg
+-rw-r--r--   0        0        0     2877 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/fullscreen_exit.svg
+-rw-r--r--   0        0        0     2236 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/heart_broken.svg
+-rw-r--r--   0        0        0     2642 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/help.svg
+-rw-r--r--   0        0        0     2206 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/home.svg
+-rw-r--r--   0        0        0     4370 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/ian_manager.svg
+-rw-r--r--   0        0        0     4191 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/icon_PSE.svg
+-rw-r--r--   0        0        0     2597 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/import.svg
+-rw-r--r--   0        0        0     1939 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/info.svg
+-rw-r--r--   0        0        0      491 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/inventory.svg
+-rw-r--r--   0        0        0     2018 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/lidl_budget.svg
+-rw-r--r--   0        0        0     2485 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/menu.svg
+-rw-r--r--   0        0        0     1747 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/minimize.svg
+-rw-r--r--   0        0        0     2498 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/nav_updater.svg
+-rw-r--r--   0        0        0     2505 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/new_releases.svg
+-rw-r--r--   0        0        0     2932 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/news.svg
+-rw-r--r--   0        0        0     3184 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/no_icon.svg
+-rw-r--r--   0        0        0     2214 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/package_commander.svg
+-rw-r--r--   0        0        0     2475 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/palette.svg
+-rw-r--r--   0        0        0     2709 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/pap.svg
+-rw-r--r--   0        0        0      175 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/partial_checked.svg
+-rw-r--r--   0        0        0     2236 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/protocol_creator.svg
+-rw-r--r--   0        0        0      549 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/pzf_widget.svg
+-rw-r--r--   0        0        0     3073 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/qt.svg
+-rw-r--r--   0        0        0     2684 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/read_more.svg
+-rw-r--r--   0        0        0     2468 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/refresh.svg
+-rw-r--r--   0        0        0     1910 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/report_merger.svg
+-rw-r--r--   0        0        0     2113 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/sap_excel.svg
+-rw-r--r--   0        0        0     2244 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/save.svg
+-rw-r--r--   0        0        0     2390 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/save_alt.svg
+-rw-r--r--   0        0        0     2398 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/search.svg
+-rw-r--r--   0        0        0     2103 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/send.svg
+-rw-r--r--   0        0        0     3472 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/settings.svg
+-rw-r--r--   0        0        0      184 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/status.svg
+-rw-r--r--   0        0        0     2448 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/swap.svg
+-rw-r--r--   0        0        0     2778 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/sync.svg
+-rw-r--r--   0        0        0     2336 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/template_selector.svg
+-rw-r--r--   0        0        0     2531 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/testbase_manager.svg
+-rw-r--r--   0        0        0     1965 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/todo_circle.svg
+-rw-r--r--   0        0        0     2257 2023-07-11 09:54:00.855824 qute_style-1.0.6/qute_style/resources/svg_icons/undo.svg
+-rw-r--r--   0        0        0    32469 2023-07-11 09:54:00.859824 qute_style-1.0.6/qute_style/resources/svg_images/banner_qute_style.svg
+-rw-r--r--   0        0        0     7237 2023-07-11 09:54:00.859824 qute_style-1.0.6/qute_style/resources/svg_images/logo_chemistry.svg
+-rw-r--r--   0        0        0     8429 2023-07-11 09:54:00.859824 qute_style-1.0.6/qute_style/resources/svg_images/logo_labmonitor.svg
+-rw-r--r--   0        0        0    39983 2023-07-11 09:54:00.859824 qute_style-1.0.6/qute_style/resources/svg_images/logo_qute_style.svg
+-rw-r--r--   0        0        0     8278 2023-07-11 09:54:00.859824 qute_style-1.0.6/qute_style/resources/svg_images/logo_toolbox.svg
+-rw-r--r--   0        0        0   323653 2023-07-11 09:54:00.859824 qute_style-1.0.6/qute_style/resources_rc.py
+-rw-r--r--   0        0        0     1657 2023-07-11 09:54:00.859824 qute_style-1.0.6/qute_style/startup_threads.py
+-rw-r--r--   0        0        0    23017 2023-07-11 09:54:00.859824 qute_style-1.0.6/qute_style/style.py
+-rw-r--r--   0        0        0    20664 2023-07-11 09:54:00.859824 qute_style-1.0.6/qute_style/ui/test_window.ui
+-rw-r--r--   0        0        0     3001 2023-07-11 09:54:00.859824 qute_style-1.0.6/qute_style/ui/whats_new_window.ui
+-rw-r--r--   0        0        0        0 2023-07-11 09:54:00.859824 qute_style-1.0.6/qute_style/widgets/__init__.py
+-rw-r--r--   0        0        0     1165 2023-07-11 09:54:00.859824 qute_style-1.0.6/qute_style/widgets/background_frame.py
+-rw-r--r--   0        0        0     2993 2023-07-11 09:54:00.859824 qute_style-1.0.6/qute_style/widgets/base_widgets.py
+-rw-r--r--   0        0        0     5533 2023-07-11 09:54:00.859824 qute_style-1.0.6/qute_style/widgets/color_manager.py
+-rw-r--r--   0        0        0     1089 2023-07-11 09:54:00.859824 qute_style-1.0.6/qute_style/widgets/credit_bar.py
+-rw-r--r--   0        0        0     4440 2023-07-11 09:54:00.859824 qute_style-1.0.6/qute_style/widgets/custom_icon_engine.py
+-rw-r--r--   0        0        0      483 2023-07-11 09:54:00.859824 qute_style-1.0.6/qute_style/widgets/div.py
+-rw-r--r--   0        0        0     1745 2023-07-11 09:54:00.859824 qute_style-1.0.6/qute_style/widgets/drop_label.py
+-rw-r--r--   0        0        0     7164 2023-07-11 09:54:00.859824 qute_style-1.0.6/qute_style/widgets/grips.py
+-rw-r--r--   0        0        0    16689 2023-07-11 09:54:00.859824 qute_style-1.0.6/qute_style/widgets/home_page.py
+-rw-r--r--   0        0        0     2049 2023-07-11 09:54:00.859824 qute_style-1.0.6/qute_style/widgets/icon.py
+-rw-r--r--   0        0        0     7678 2023-07-11 09:54:00.859824 qute_style-1.0.6/qute_style/widgets/icon_button.py
+-rw-r--r--   0        0        0     3474 2023-07-11 09:54:00.863824 qute_style-1.0.6/qute_style/widgets/icon_tooltip_button.py
+-rw-r--r--   0        0        0     6849 2023-07-11 09:54:00.863824 qute_style-1.0.6/qute_style/widgets/left_column.py
+-rw-r--r--   0        0        0      808 2023-07-11 09:54:00.863824 qute_style-1.0.6/qute_style/widgets/left_column_close_button.py
+-rw-r--r--   0        0        0     8775 2023-07-11 09:54:00.863824 qute_style-1.0.6/qute_style/widgets/left_menu.py
+-rw-r--r--   0        0        0     7075 2023-07-11 09:54:00.863824 qute_style-1.0.6/qute_style/widgets/left_menu_button.py
+-rw-r--r--   0        0        0    11127 2023-07-11 09:54:00.863824 qute_style-1.0.6/qute_style/widgets/spinner.py
+-rw-r--r--   0        0        0    14811 2023-07-11 09:54:00.863824 qute_style-1.0.6/qute_style/widgets/styled_combobox.py
+-rw-r--r--   0        0        0     1878 2023-07-11 09:54:00.863824 qute_style-1.0.6/qute_style/widgets/text_truncator.py
+-rw-r--r--   0        0        0     6922 2023-07-11 09:54:00.863824 qute_style-1.0.6/qute_style/widgets/title_bar.py
+-rw-r--r--   0        0        0     1733 2023-07-11 09:54:00.863824 qute_style-1.0.6/qute_style/widgets/title_button.py
+-rw-r--r--   0        0        0     4334 2023-07-11 09:54:00.863824 qute_style-1.0.6/qute_style/widgets/toggle.py
+-rw-r--r--   0        0        0     1046 2023-07-11 09:54:00.863824 qute_style-1.0.6/qute_style/widgets/tooltip.py
+-rw-r--r--   0        0        0        0 2023-07-11 09:54:00.863824 qute_style-1.0.6/qute_style_examples/__init__.py
+-rw-r--r--   0        0        0      136 2023-07-11 09:54:00.863824 qute_style-1.0.6/qute_style_examples/__main__.py
+-rw-r--r--   0        0        0    21042 2023-07-11 09:54:00.863824 qute_style-1.0.6/qute_style_examples/example_images/color_manager.PNG
+-rw-r--r--   0        0        0    79278 2023-07-11 09:54:00.863824 qute_style-1.0.6/qute_style_examples/example_images/custom_style.PNG
+-rw-r--r--   0        0        0    62693 2023-07-11 09:54:00.863824 qute_style-1.0.6/qute_style_examples/example_images/darcula.PNG
+-rw-r--r--   0        0        0     3902 2023-07-11 09:54:00.863824 qute_style-1.0.6/qute_style_examples/example_images/drop_label.PNG
+-rw-r--r--   0        0        0    50435 2023-07-11 09:54:00.863824 qute_style-1.0.6/qute_style_examples/example_images/highbridge_grey.PNG
+-rw-r--r--   0        0        0     4594 2023-07-11 09:54:00.863824 qute_style-1.0.6/qute_style_examples/example_images/information_messagebox.PNG
+-rw-r--r--   0        0        0    30905 2023-07-11 09:54:00.863824 qute_style-1.0.6/qute_style_examples/example_images/princesspink.PNG
+-rw-r--r--   0        0        0    30041 2023-07-11 09:54:00.863824 qute_style-1.0.6/qute_style_examples/example_images/rubyred.PNG
+-rw-r--r--   0        0        0    30867 2023-07-11 09:54:00.863824 qute_style-1.0.6/qute_style_examples/example_images/snowwhite.PNG
+-rw-r--r--   0        0        0    56113 2023-07-11 09:54:00.867824 qute_style-1.0.6/qute_style_examples/example_images/widgets_display.PNG
+-rw-r--r--   0        0        0     2818 2023-07-11 09:54:00.867824 qute_style-1.0.6/qute_style_examples/main.py
+-rw-r--r--   0        0        0     1244 2023-07-11 09:54:00.867824 qute_style-1.0.6/qute_style_examples/sample_classes.py
+-rw-r--r--   0        0        0     3532 2023-07-11 09:54:00.867824 qute_style-1.0.6/qute_style_examples/sample_main_window.py
+-rw-r--r--   0        0        0     9665 2023-07-11 09:54:00.867824 qute_style-1.0.6/qute_style_examples/sample_widgets.py
+-rw-r--r--   0        0        0      110 2023-07-11 09:54:00.867824 qute_style-1.0.6/qute_style_examples/test_changelog/1.01/1.json
+-rw-r--r--   0        0        0      211 2023-07-11 09:54:00.867824 qute_style-1.0.6/qute_style_examples/test_changelog/1.01/2.json
+-rw-r--r--   0        0        0    45119 2023-07-11 09:54:00.867824 qute_style-1.0.6/qute_style_examples/test_changelog/1.01/bug.png
+-rw-r--r--   0        0        0       42 2023-07-11 09:54:00.867824 qute_style-1.0.6/qute_style_examples/test_changelog/1.01/meta.json
+-rw-r--r--   0        0        0      167 2023-07-11 09:54:00.867824 qute_style-1.0.6/qute_style_examples/test_changelog/1.10/1.json
+-rw-r--r--   0        0        0      209 2023-07-11 09:54:00.867824 qute_style-1.0.6/qute_style_examples/test_changelog/1.10/2.json
+-rw-r--r--   0        0        0    45119 2023-07-11 09:54:00.867824 qute_style-1.0.6/qute_style_examples/test_changelog/1.10/bug.png
+-rw-r--r--   0        0        0       42 2023-07-11 09:54:00.867824 qute_style-1.0.6/qute_style_examples/test_changelog/1.10/meta.json
+-rw-r--r--   0        0        0      114 2023-07-11 09:54:00.867824 qute_style-1.0.6/qute_style_examples/test_changelog/1.100/1.json
+-rw-r--r--   0        0        0       97 2023-07-11 09:54:00.867824 qute_style-1.0.6/qute_style_examples/test_changelog/1.100/2.json
+-rw-r--r--   0        0        0       42 2023-07-11 09:54:00.867824 qute_style-1.0.6/qute_style_examples/test_changelog/1.100/meta.json
+-rw-r--r--   0        0        0     6246 1970-01-01 00:00:00.000000 qute_style-1.0.6/PKG-INFO
```

### Comparing `qute_style-1.0.5/LICENSE` & `qute_style-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/README.md` & `qute_style-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/pyproject.toml` & `qute_style-1.0.6/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 [tool.poetry]
 name = "qute_style"
-version = "1.0.5"
+version = "1.0.6"
 description = "QuteStyle is an expandable application framework for PySide6"
 authors = ["Marina Baumgartner, Dairen Gonschior, Tilman Krummeck, Dennis Spitzhorn, Gerhard Trapp, Patrick Zwerschke <PS-TF-Entwicklung@tuev-sued.de>"]
 readme = "README.md"
 repository = "https://github.com/TUV-SUD-Product-Service-GmbH/QuteStyle"
 license = "MIT"
 packages = [
     {include = "qute_style"},
     {include = "qute_style_examples"},
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
-PySide6 = "6.4.2"
+PySide6 = "6.5.1.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "7.3.1"
 pytest-qt = "4.2.0"
 requests = "2.31.0"
 black = "23.3.0"
 coverage = "7.2.3"
 isort = "5.12.0"
-mypy = "1.2.0"
+mypy = "1.4.1"
 pre-commit = "3.2.2"
 pydocstyle = "6.3.0"
 pylint = "^2.17.3"
 pytest-cov = "^4.0.0"
 pytest-github-actions-annotate-failures = "^0.1.8"
 types-requests = "2.31.0.0"
```

### Comparing `qute_style-1.0.5/qute_style/dev/dev_functions.py` & `qute_style-1.0.6/qute_style/dev/dev_functions.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/dev/mocks.py` & `qute_style-1.0.6/qute_style/dev/mocks.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/gen/ui_test_window.py` & `qute_style-1.0.6/qute_style/gen/ui_test_window.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/gen/ui_whats_new_window.py` & `qute_style-1.0.6/qute_style/gen/ui_whats_new_window.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/helper.py` & `qute_style-1.0.6/qute_style/helper.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/qs_application.py` & `qute_style-1.0.6/qute_style/qs_application.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/qs_main_window.py` & `qute_style-1.0.6/qute_style/qs_main_window.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,17 @@
 from qute_style.widgets.credit_bar import CreditBar
 from qute_style.widgets.grips import CornerGrip, EdgeGrip
 from qute_style.widgets.home_page import HomePage
 from qute_style.widgets.left_column import LeftColumn
 from qute_style.widgets.left_menu import LeftMenu
 from qute_style.widgets.title_bar import TitleBar
 
-log = logging.getLogger(f"tsl.{__name__}")  # pylint: disable=invalid-name
+log = logging.getLogger(
+    f"qute_style.{__name__}"
+)  # pylint: disable=invalid-name
 
 
 @dataclass
 class AppData:  # pylint: disable=too-many-instance-attributes
     """Provide required data to startup threads."""
 
     app_name: str = ""
@@ -101,19 +103,22 @@
 
     # Define the maximum width for the columns (left and right).
     MAX_COLUMN_WIDTH = 240
 
     # Signal that is emitted when the window has shut down.
     shutdown_complete = Signal(name="shutdown_complete")
 
+    LANG_CODE: str | None = None
+
     def __init__(  # pylint: disable=too-many-arguments
         self,
         app_data: AppData,
         force_whats_new: bool = False,
         registry_reset: bool = False,
+        load_last_used_widget: bool = False,
         parent: QWidget | None = None,
     ) -> None:
         """Create a new QuteStyleMainWindow."""
         super().__init__(app_data, force_whats_new, registry_reset, parent)
 
         QApplication.setStyle(QuteStyle())
         QApplication.setPalette(QApplication.style().standardPalette())
@@ -180,21 +185,29 @@
             EdgeGrip(self, Qt.Edge.TopEdge),
             EdgeGrip(self, Qt.Edge.BottomEdge),
             CornerGrip(self, Qt.Corner.TopLeftCorner),
             CornerGrip(self, Qt.Corner.TopRightCorner),
             CornerGrip(self, Qt.Corner.BottomLeftCorner),
             CornerGrip(self, Qt.Corner.BottomRightCorner),
         ]
-
         for grip in self._grips:
             grip.window_geometry_changed.connect(self.window_geometry_changed)
-
-        # Activate the first widget to be visible by default.
-        if self.MAIN_WIDGET_CLASSES:
-            self.on_main_widget(self.MAIN_WIDGET_CLASSES[0])
+        startup_widget: Type[MainWidget] | None = None
+        last_used_widget = QSettings().value("last_used_widget")
+        if (
+            load_last_used_widget
+            and last_used_widget
+            and last_used_widget in self.MAIN_WIDGET_CLASSES
+        ):
+            startup_widget = cast(Type[MainWidget], last_used_widget)
+        elif self.MAIN_WIDGET_CLASSES:
+            # Activate the first widget to be visible by default.
+            startup_widget = self.MAIN_WIDGET_CLASSES[0]
+        if startup_widget:
+            self.on_main_widget(startup_widget)
 
     MainWidgetT = TypeVar("MainWidgetT", bound=MainWidget)
 
     def show(self) -> None:
         """Override show to start update just before."""
         self._load_settings()
         super().show()
@@ -224,21 +237,22 @@
     @Slot(QRect, name="window_geometry_changed")
     def window_geometry_changed(self, geometry: QRect) -> None:
         """Handle change of window geometry by using the grips."""
         self.setGeometry(geometry)
 
     WidgetT = TypeVar("WidgetT", MainWidget, BaseWidget)
 
-    @staticmethod
-    def get_app_language() -> str:
+    @classmethod
+    def get_app_language(cls) -> str:
         """Get the currently set language to use for the ui."""
-        sys_lang = QLocale().system().name()[:2]
-        lang = QSettings().value("lang", sys_lang)
-        assert isinstance(lang, str)
-        return lang
+        if not cls.LANG_CODE:
+            sys_lang = QLocale().system().name()[:2]
+            cls.LANG_CODE = cast(str, QSettings().value("lang", sys_lang))
+            assert isinstance(cls.LANG_CODE, str)
+        return cls.LANG_CODE
 
     @staticmethod
     def _get_widgets_to_display(
         widgets: list[Type[WidgetT]],
     ) -> list[Type[WidgetT]]:
         """Reimplement to restrict access to certain widgets."""
         return widgets
@@ -247,15 +261,15 @@
         self, layout: QLayout
     ) -> tuple[QFrame, QStackedWidget, QStackedWidget]:
         """
         Add a Frame that contains the main content and the right column widget.
 
         The method creates a QFrame that contains two widgets:
         1. A QStackedWidget that contains all the widgets that are accessible
-        from the menu (as defined in TslMainGui.MAIN_WIDGET_CLASS
+        from the menu (as defined in QuteMainGui.MAIN_WIDGET_CLASS
         2. A QFrame with the widget that is used as the right column.
         """
         content_area_frame = QFrame()
         content_area_layout = QHBoxLayout(content_area_frame)
         content_area_layout.setContentsMargins(0, 0, 0, 0)
 
         # Create the QStackedWidget that contains all the content widgets
@@ -290,15 +304,15 @@
     ) -> tuple[QFrame, QStackedWidget]:
         """
         Create a frame containing the right column widget and return it.
 
         This method creates a QFrame that is opened/closed with a button in the
         TitleBar. Therefore it's initial width is 0. The frame contains a
         layout with a margin of 5 pixels which contains the widget for the
-        right column (as defined in TslMainGui.RIGHT_WIDGET_CLASS).
+        right column (as defined in QuteMainGui.RIGHT_WIDGET_CLASS).
         """
         right_column_frame = QFrame()
         right_column_frame.setObjectName("bg_two_frame")
         right_column_frame.setFixedWidth(0)
         content_area_right_layout = QVBoxLayout(right_column_frame)
         content_area_right_layout.setContentsMargins(5, 5, 5, 5)
         right_content = QStackedWidget()
@@ -573,16 +587,16 @@
         for grip in self._grips:
             grip.adapt()
 
     def mousePressEvent(  # pylint: disable=invalid-name
         self, event: QMouseEvent
     ) -> None:
         """Event triggered on mouse button press."""
-        log.debug("Storing last click at %s", event.globalPos())
-        self.last_move_pos = event.globalPos()
+        self.last_move_pos = event.globalPosition().toPoint()
+        log.debug("Storing last click at %s", self.last_move_pos)
 
     @Slot(type, name="on_main_widget")
     def on_main_widget(self, widget_class: Type[MainWidget]) -> None:
         """Handle display of the main widget that is of the given type."""
         current_widget = cast(
             Type[MainWidget],
             type(self._content.currentWidget()),
@@ -598,15 +612,15 @@
                 )
                 # show the individual settings widgets per main widget
                 if self._column_is_visible(self._left_column_frame):
                     self._left_column.handle_settings_display(
                         widget.settings_widget, widget.ICON
                     )
                 return
-        raise ValueError("Could not find widget {widget_class}")
+        raise ValueError(f"Could not find widget {widget_class}")
 
     @Slot(type, name="on_right_column")
     def on_right_column(self, widget_class: Type[BaseWidget]) -> None:
         """Handle a click on the button for the right column."""
         right_widget_type = self.right_widget_type()
         left_widget_type = self._left_column.current_widget_type()
 
@@ -704,14 +718,19 @@
 
     def _save_settings(self) -> None:
         """Save the paint data and state/geometry settings."""
         log.debug("Saving settings to registry.")
         settings = QSettings()
         settings.setValue("state", self.saveState())
         settings.setValue("geometry", self.saveGeometry())
+        current_widget = cast(
+            Type[MainWidget],
+            type(self._content.currentWidget()),
+        )
+        settings.setValue("last_used_widget", current_widget)
         log.debug("Finished writing settings to registry")
 
     @Slot(QCloseEvent, name="closeEvent")
     def closeEvent(  # pylint: disable=invalid-name
         self, close_event: QCloseEvent
     ) -> None:
         """Handle a close event."""
```

### Comparing `qute_style-1.0.5/qute_style/qs_message_box.py` & `qute_style-1.0.6/qute_style/qs_message_box.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/qute_style.py` & `qute_style-1.0.6/qute_style/qute_style.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     @position.setter
     def position(self, value: int) -> None:
         """Set the position of the Toggle."""
         self._position = value
 
 
 class QuteStyle(QProxyStyle):
-    """Custom style for a TSL Style application."""
+    """Custom style for a Qute Style application."""
 
     # Custom ControlElement for drawControl method.
     CE_Toggle = QStyle.ControlElement(QStyle.ControlElement.CE_CustomBase + 1)
 
     # This is the cache that holds QPalettes already created, since they will
     # not change unless the user changes the theme.
     PALETTE_CACHE: dict[str, QPalette] = {}
```

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/accept_circle.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/accept_circle.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/active_menu.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/active_menu.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/add.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/add.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/add_circle.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/add_circle.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/admin.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/admin.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/admin_panel.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/admin_panel.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/arrow_back.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/arrow_back.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/block.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/block.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/bug.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/bug.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/check_circle.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/check_circle.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/close.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/close.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/close_circle.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/close_circle.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/copy.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/copy.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/cps_trends.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/cps_trends.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/delete.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/delete.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/delete_forever.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/delete_forever.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/delete_import.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/delete_import.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/document.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/document.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/document_scanner.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/document_scanner.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/error.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/error.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/expand_less.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/expand_less.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/expand_more.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/expand_more.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/file_distributor.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/file_distributor.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/folder_open.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/folder_open.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/fullscreen.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/fullscreen.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/fullscreen_exit.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/fullscreen_exit.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/heart_broken.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/heart_broken.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/help.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/help.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/home.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/home.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/ian_manager.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/ian_manager.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/icon_PSE.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/icon_PSE.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/import.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/import.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/info.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/info.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/lidl_budget.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/lidl_budget.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/menu.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/menu.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/minimize.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/minimize.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/nav_updater.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/nav_updater.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/new_releases.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/new_releases.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/news.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/news.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/no_icon.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/no_icon.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/package_commander.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/package_commander.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/palette.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/palette.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/pap.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/pap.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/protocol_creator.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/protocol_creator.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/pzf_widget.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/pzf_widget.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/qt.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/qt.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/read_more.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/read_more.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/refresh.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/refresh.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/report_merger.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/report_merger.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/sap_excel.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/sap_excel.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/save.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/save.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/save_alt.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/save_alt.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/search.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/search.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/send.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/send.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/settings.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/settings.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/swap.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/swap.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/sync.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/sync.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/template_selector.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/template_selector.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/testbase_manager.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/testbase_manager.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/todo_circle.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/todo_circle.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_icons/undo.svg` & `qute_style-1.0.6/qute_style/resources/svg_icons/undo.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_images/banner_qute_style.svg` & `qute_style-1.0.6/qute_style/resources/svg_images/banner_qute_style.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_images/logo_chemistry.svg` & `qute_style-1.0.6/qute_style/resources/svg_images/logo_chemistry.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_images/logo_labmonitor.svg` & `qute_style-1.0.6/qute_style/resources/svg_images/logo_labmonitor.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_images/logo_qute_style.svg` & `qute_style-1.0.6/qute_style/resources/svg_images/logo_qute_style.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources/svg_images/logo_toolbox.svg` & `qute_style-1.0.6/qute_style/resources/svg_images/logo_toolbox.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/resources_rc.py` & `qute_style-1.0.6/qute_style/resources_rc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Resource object code (Python 3)
 # Created by: object code
-# Created by: The Resource Compiler for Qt version 6.4.2
+# Created by: The Resource Compiler for Qt version 6.5.1
 # WARNING! All changes made in this file will be lost!
 
 from PySide6 import QtCore
 
 qt_resource_data = b"\
 \x00\x00\x00h\
 \x89\
@@ -3499,15 +3499,15 @@
 th829\x22\x0d\x0a     ink\
 scape:connector-\
 curvature=\x220\x22\x0d\x0a \
     style=\x22strok\
 e-width:1.333321\
 45\x22 />\x0d\x0a</svg>\x0d\x0a\
 \
-\x00\x00\x01\xea\
+\x00\x00\x01\xec\
 <\
 svg xmlns=\x22http:\
 //www.w3.org/200\
 0/svg\x22 height=\x224\
 8\x22 width=\x2248\x22><p\
 ath d=\x22M9 44q-1.\
 2 0-2.1-.975Q6 4\
@@ -3531,15 +3531,15 @@
 .075-.425-.425-1\
 .075-.425h-9q-.6\
 5 0-1.075.425Q18\
  24.7 18 25.35q0\
  .65.425 1.075.4\
 25.425 1.075.425\
 ZM9 41V16.35 41Z\
-\x22/></svg>\
+\x22/></svg>\x0d\x0a\
 \x00\x00\x10\x98\
 <\
 ?xml version=\x221.\
 0\x22 encoding=\x22UTF\
 -8\x22 standalone=\x22\
 no\x22?>\x0d\x0a<svg\x0d\x0a   \
 xmlns:dc=\x22http:/\
@@ -13938,170 +13938,170 @@
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00\x00\x00\x02\x00\x00\x00\x05\x00\x00\x00M\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x002\x00\x02\x00\x00\x00\x01\x00\x00\x00L\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00\x1a\x00\x02\x00\x00\x00H\x00\x00\x00\x04\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x09N\x00\x00\x00\x00\x00\x01\x00\x025~\
-\x00\x00\x01\x84E\x18^\x93\
+\x00\x00\x09N\x00\x00\x00\x00\x00\x01\x00\x025\x80\
+\x00\x00\x01\x81\x85\x13\x8d\x1c\
 \x00\x00\x02\xc0\x00\x00\x00\x00\x00\x01\x00\x00\x8f\xcd\
-\x00\x00\x01\x84E\x18^\x93\
-\x00\x00\x04\xc4\x00\x00\x00\x00\x00\x01\x00\x01\x0d!\
-\x00\x00\x01\x84E\x18^\x7f\
+\x00\x00\x01\x81\x85\x13\x8d\x1c\
+\x00\x00\x04\xc4\x00\x00\x00\x00\x00\x01\x00\x01\x0d#\
+\x00\x00\x01\x81\x85\x13\x8d\x08\
 \x00\x00\x01\xa8\x00\x00\x00\x00\x00\x01\x00\x00WV\
-\x00\x00\x01\x84E\x18^u\
+\x00\x00\x01\x81\x85\x13\x8d\x08\
 \x00\x00\x01\x1a\x00\x00\x00\x00\x00\x01\x00\x005A\
-\x00\x00\x01\x84E\x18^u\
-\x00\x00\x08\xd6\x00\x00\x00\x00\x00\x01\x00\x02\x13\xa1\
-\x00\x00\x01\x84E\x18^\x7f\
-\x00\x00\x06|\x00\x00\x00\x00\x00\x01\x00\x01d\x1d\
-\x00\x00\x01\x84E\x18^\x89\
+\x00\x00\x01\x81\x85\x13\x8d\x08\
+\x00\x00\x08\xd6\x00\x00\x00\x00\x00\x01\x00\x02\x13\xa3\
+\x00\x00\x01\x81\x85\x13\x8d\x08\
+\x00\x00\x06|\x00\x00\x00\x00\x00\x01\x00\x01d\x1f\
+\x00\x00\x01\x81\x85\x13\x8d\x12\
 \x00\x00\x03\x02\x00\x00\x00\x00\x00\x01\x00\x00\xa1L\
-\x00\x00\x01\x84E\x18^\x7f\
+\x00\x00\x01\x81\x85\x13\x8d\x08\
 \x00\x00\x03h\x00\x00\x00\x00\x00\x01\x00\x00\xb1\xe6\
-\x00\x00\x01\x84E\x18^\x7f\
-\x00\x00\x07\xea\x00\x00\x00\x00\x00\x01\x00\x01\xc6e\
-\x00\x00\x01\x84E\x18^\x89\
+\x00\x00\x01\x81\x85\x13\x8d\x08\
+\x00\x00\x07\xea\x00\x00\x00\x00\x00\x01\x00\x01\xc6g\
+\x00\x00\x01\x81\x85\x13\x8d\x1c\
 \x00\x00\x01\xce\x00\x00\x00\x00\x00\x01\x00\x00X\x9f\
-\x00\x00\x01\x84E\x18^\x7f\
-\x00\x00\x08\x18\x00\x00\x00\x00\x00\x01\x00\x01\xcfn\
-\x00\x00\x01\x84E\x18^\x7f\
-\x00\x00\x08\x9a\x00\x00\x00\x00\x00\x01\x00\x02\x03\xa7\
-\x00\x00\x01\x84E\x18^u\
-\x00\x00\x08\xb2\x00\x00\x00\x00\x00\x01\x00\x02\x0bz\
-\x00\x00\x01\x84E\x18^\x7f\
+\x00\x00\x01\x81\x85\x13\x8d\x08\
+\x00\x00\x08\x18\x00\x00\x00\x00\x00\x01\x00\x01\xcfp\
+\x00\x00\x01\x81\x85\x13\x8d\x08\
+\x00\x00\x08\x9a\x00\x00\x00\x00\x00\x01\x00\x02\x03\xa9\
+\x00\x00\x01\x81\x85\x13\x8c\xfe\
+\x00\x00\x08\xb2\x00\x00\x00\x00\x00\x01\x00\x02\x0b|\
+\x00\x00\x01\x81\x85\x13\x8d\x08\
 \x00\x00\x00\xa6\x00\x00\x00\x00\x00\x01\x00\x00\x11\xa5\
-\x00\x00\x01\x84E\x18^\x93\
+\x00\x00\x01\x81\x85\x13\x8d&\
 \x00\x00\x03(\x00\x00\x00\x00\x00\x01\x00\x00\xa2\xbc\
-\x00\x00\x01\x84E\x18^u\
+\x00\x00\x01\x81\x85\x13\x8c\xfe\
 \x00\x00\x00\xdc\x00\x00\x00\x00\x00\x01\x00\x00#7\
-\x00\x00\x01\x84E\x18^\x89\
+\x00\x00\x01\x81\x85\x13\x8d\x12\
 \x00\x00\x022\x00\x00\x00\x00\x00\x01\x00\x00sd\
-\x00\x00\x01\x84E\x18^\x7f\
+\x00\x00\x01\x81\x85\x13\x8d\x12\
 \x00\x00\x01\x84\x00\x01\x00\x00\x00\x01\x00\x00Re\
-\x00\x00\x01\x84E\x18^\x7f\
-\x00\x00\x05\x88\x00\x00\x00\x00\x00\x01\x00\x010;\
-\x00\x00\x01\x84E\x18^u\
+\x00\x00\x01\x81\x85\x13\x8d\x08\
+\x00\x00\x05\x88\x00\x00\x00\x00\x00\x01\x00\x010=\
+\x00\x00\x01\x81\x85\x13\x8d\x08\
 \x00\x00\x03\x90\x00\x00\x00\x00\x00\x01\x00\x00\xb9\xae\
-\x00\x00\x01\x84E\x18^u\
+\x00\x00\x01\x81\x85\x13\x8d\x08\
 \x00\x00\x04\x0e\x00\x00\x00\x00\x00\x01\x00\x00\xd6y\
-\x00\x00\x01\x86\xdb\x1c\x5c\xe9\
-\x00\x00\x04\x9a\x00\x00\x00\x00\x00\x01\x00\x00\xf9Z\
-\x00\x00\x01\x84E\x18^\x7f\
-\x00\x00\x070\x00\x00\x00\x00\x00\x01\x00\x01\x92\x18\
-\x00\x00\x01\x84E\x18^\x93\
+\x00\x00\x01\x87~HTl\
+\x00\x00\x04\x9a\x00\x00\x00\x00\x00\x01\x00\x00\xf9\x5c\
+\x00\x00\x01\x81\x85\x13\x8d\x08\
+\x00\x00\x070\x00\x00\x00\x00\x00\x01\x00\x01\x92\x1a\
+\x00\x00\x01\x81\x85\x13\x8d\x1c\
 \x00\x00\x03\xb2\x00\x00\x00\x00\x00\x01\x00\x00\xbb=\
-\x00\x00\x01\x84E\x18^\x7f\
-\x00\x00\x04\xb0\x00\x00\x00\x00\x00\x01\x00\x01\x028\
-\x00\x00\x01\x84E\x18^\x89\
-\x00\x00\x07`\x00\x00\x00\x00\x00\x01\x00\x01\x9b\x87\
-\x00\x00\x01\x84E\x18^u\
-\x00\x00\x09\x1e\x00\x00\x00\x00\x00\x01\x00\x02\x22\x19\
-\x00\x00\x01\x84E\x18^\x7f\
-\x00\x00\x07\xb6\x00\x00\x00\x00\x00\x01\x00\x01\xb1u\
-\x00\x00\x01\x84E\x18^\x89\
-\x00\x00\x08:\x00\x00\x00\x00\x00\x01\x00\x01\xda\xee\
-\x00\x00\x01\x84E\x18^u\
+\x00\x00\x01\x81\x85\x13\x8d\x08\
+\x00\x00\x04\xb0\x00\x00\x00\x00\x00\x01\x00\x01\x02:\
+\x00\x00\x01\x81\x85\x13\x8d\x1c\
+\x00\x00\x07`\x00\x00\x00\x00\x00\x01\x00\x01\x9b\x89\
+\x00\x00\x01\x81\x85\x13\x8d\x08\
+\x00\x00\x09\x1e\x00\x00\x00\x00\x00\x01\x00\x02\x22\x1b\
+\x00\x00\x01\x81\x85\x13\x8d\x12\
+\x00\x00\x07\xb6\x00\x00\x00\x00\x00\x01\x00\x01\xb1w\
+\x00\x00\x01\x81\x85\x13\x8d\x1c\
+\x00\x00\x08:\x00\x00\x00\x00\x00\x01\x00\x01\xda\xf0\
+\x00\x00\x01\x81\x85\x13\x8c\xfe\
 \x00\x00\x03\xc8\x00\x00\x00\x00\x00\x01\x00\x00\xc3\x99\
-\x00\x00\x01\x84E\x18^\x89\
-\x00\x00\x05\x1c\x00\x00\x00\x00\x00\x01\x00\x01\x17\xca\
-\x00\x00\x01\x84E\x18^\x89\
-\x00\x00\x04.\x00\x00\x00\x00\x00\x01\x00\x00\xd8g\
-\x00\x00\x01\x84E\x18^\x7f\
-\x00\x00\x08d\x00\x00\x00\x00\x00\x01\x00\x01\xedY\
-\x00\x00\x01\x84E\x18^\x89\
-\x00\x00\x098\x00\x00\x00\x00\x00\x01\x00\x02,z\
-\x00\x00\x01\x84E\x18^\x89\
-\x00\x00\x05<\x00\x00\x00\x00\x00\x01\x00\x01\x22\xa2\
-\x00\x00\x01\x84E\x18^u\
-\x00\x00\x05\xe2\x00\x00\x00\x00\x00\x01\x00\x01D\xd0\
-\x00\x00\x01\x84E\x18^\x7f\
+\x00\x00\x01\x81\x85\x13\x8d\x1c\
+\x00\x00\x05\x1c\x00\x00\x00\x00\x00\x01\x00\x01\x17\xcc\
+\x00\x00\x01\x81\x85\x13\x8d\x1c\
+\x00\x00\x04.\x00\x00\x00\x00\x00\x01\x00\x00\xd8i\
+\x00\x00\x01\x81\x85\x13\x8d\x12\
+\x00\x00\x08d\x00\x00\x00\x00\x00\x01\x00\x01\xed[\
+\x00\x00\x01\x81\x85\x13\x8d\x1c\
+\x00\x00\x098\x00\x00\x00\x00\x00\x01\x00\x02,|\
+\x00\x00\x01\x81\x85\x13\x8d\x1c\
+\x00\x00\x05<\x00\x00\x00\x00\x00\x01\x00\x01\x22\xa4\
+\x00\x00\x01\x81\x85\x13\x8c\xfe\
+\x00\x00\x05\xe2\x00\x00\x00\x00\x00\x01\x00\x01D\xd2\
+\x00\x00\x01\x81\x85\x13\x8d\x08\
 \x00\x00\x01\x02\x00\x00\x00\x00\x00\x01\x00\x00-@\
-\x00\x00\x01\x84E\x18^\x7f\
-\x00\x00\x06P\x00\x00\x00\x00\x00\x01\x00\x01X\xa0\
-\x00\x00\x01\x84E\x18^\x7f\
-\x00\x00\x06\x00\x00\x00\x00\x00\x00\x01\x00\x01Li\
-\x00\x00\x01\x86o\x19q?\
+\x00\x00\x01\x81\x85\x13\x8d\x08\
+\x00\x00\x06P\x00\x00\x00\x00\x00\x01\x00\x01X\xa2\
+\x00\x00\x01\x81\x85\x13\x8d\x08\
+\x00\x00\x06\x00\x00\x00\x00\x00\x00\x01\x00\x01Lk\
+\x00\x00\x01\x87~HTl\
 \x00\x00\x00\x92\x00\x00\x00\x00\x00\x01\x00\x00\x02S\
-\x00\x00\x01\x84E\x18^u\
+\x00\x00\x01\x81\x85\x13\x8d\x08\
 \x00\x00\x00\xbc\x00\x00\x00\x00\x00\x01\x00\x00\x1a\xb6\
-\x00\x00\x01\x84E\x18^\x89\
+\x00\x00\x01\x81\x85\x13\x8d\x1c\
 \x00\x00\x00x\x00\x00\x00\x00\x00\x01\x00\x00\x00l\
-\x00\x00\x01\x84E\x18^\x7f\
-\x00\x00\x08~\x00\x00\x00\x00\x00\x01\x00\x01\xf6\xf7\
-\x00\x00\x01\x84E\x18^\x89\
+\x00\x00\x01\x85\xc5\x11(\xd1\
+\x00\x00\x08~\x00\x00\x00\x00\x00\x01\x00\x01\xf6\xf9\
+\x00\x00\x01\x81\x85\x13\x8d\x12\
 \x00\x00\x02\xe4\x00\x00\x00\x00\x00\x01\x00\x00\x97\xb6\
-\x00\x00\x01\x84E\x18^\x89\
+\x00\x00\x01\x81\x85\x13\x8d\x1c\
 \x00\x00\x01h\x00\x00\x00\x00\x00\x01\x00\x00Hq\
-\x00\x00\x01\x84E\x18^\x89\
-\x00\x00\x08\xfa\x00\x00\x00\x00\x00\x01\x00\x02\x19\xf7\
-\x00\x00\x01\x84E\x18^\x89\
+\x00\x00\x01\x81\x85\x13\x8d\x1c\
+\x00\x00\x08\xfa\x00\x00\x00\x00\x00\x01\x00\x02\x19\xf9\
+\x00\x00\x01\x81\x85\x13\x8d\x12\
 \x00\x00\x02H\x00\x00\x00\x00\x00\x01\x00\x00{7\
-\x00\x00\x01\x84E\x18^\x7f\
-\x00\x00\x06\xd4\x00\x00\x00\x00\x00\x01\x00\x01\x86\x8e\
-\x00\x00\x01\x84E\x18^\x7f\
-\x00\x00\x06\xf6\x00\x00\x00\x00\x00\x01\x00\x01\x8f\x9d\
-\x00\x00\x01\x84E\x18^\x89\
-\x00\x00\x06\xb6\x00\x00\x00\x00\x00\x01\x00\x01x\xbc\
-\x00\x00\x01\x84E\x18^\x89\
-\x00\x00\x06\xa0\x00\x00\x00\x00\x00\x01\x00\x01n*\
-\x00\x00\x01\x84E\x18^\x7f\
+\x00\x00\x01\x81\x85\x13\x8d\x08\
+\x00\x00\x06\xd4\x00\x00\x00\x00\x00\x01\x00\x01\x86\x90\
+\x00\x00\x01\x81\x85\x13\x8d\x08\
+\x00\x00\x06\xf6\x00\x00\x00\x00\x00\x01\x00\x01\x8f\x9f\
+\x00\x00\x01\x81\x85\x13\x8d\x1c\
+\x00\x00\x06\xb6\x00\x00\x00\x00\x00\x01\x00\x01x\xbe\
+\x00\x00\x01\x81\x85\x13\x8d\x1c\
+\x00\x00\x06\xa0\x00\x00\x00\x00\x00\x01\x00\x01n,\
+\x00\x00\x01\x81\x85\x13\x8d\x08\
 \x00\x00\x01R\x00\x00\x00\x00\x00\x01\x00\x00?\xfa\
-\x00\x00\x01\x84E\x18^\x89\
-\x00\x00\x06.\x00\x00\x00\x00\x00\x01\x00\x01Vv\
-\x00\x00\x01\x84E\x18^\x89\
+\x00\x00\x01\x81\x85\x13\x8d\x1c\
+\x00\x00\x06.\x00\x00\x00\x00\x00\x01\x00\x01Vx\
+\x00\x00\x01\x81\x85\x13\x8d\x1c\
 \x00\x00\x03\xf8\x00\x00\x00\x00\x00\x01\x00\x00\xcc\x84\
-\x00\x00\x01\x84E\x18^\x89\
+\x00\x00\x01\x81\x85\x13\x8d\x12\
 \x00\x00\x016\x00\x00\x00\x00\x00\x01\x00\x006\x16\
-\x00\x00\x01\x84E\x18^\x89\
-\x00\x00\x07x\x00\x00\x00\x00\x00\x01\x00\x01\xa4\xa6\
-\x00\x00\x01\x84E\x18^u\
+\x00\x00\x01\x81\x85\x13\x8d\x1c\
+\x00\x00\x07x\x00\x00\x00\x00\x00\x01\x00\x01\xa4\xa8\
+\x00\x00\x01\x81\x85\x13\x8c\xfe\
 \x00\x00\x01\xf4\x00\x00\x00\x00\x00\x01\x00\x00a\xa3\
-\x00\x00\x01\x84E\x18^\x7f\
-\x00\x00\x07\x92\x00\x00\x00\x00\x00\x01\x00\x01\xa6}\
-\x00\x00\x01\x84E\x18^u\
-\x00\x00\x05\xa0\x00\x00\x00\x00\x00\x01\x00\x018O\
-\x00\x00\x01\x84E\x18^\x89\
-\x00\x00\x07\x10\x00\x00\x00\x00\x00\x01\x00\x01\x90Z\
-\x00\x00\x01\x84E\x18^u\
+\x00\x00\x01\x81\x85\x13\x8d\x08\
+\x00\x00\x07\x92\x00\x00\x00\x00\x00\x01\x00\x01\xa6\x7f\
+\x00\x00\x01\x81\x85\x13\x8c\xfe\
+\x00\x00\x05\xa0\x00\x00\x00\x00\x00\x01\x00\x018Q\
+\x00\x00\x01\x81\x85\x13\x8d\x12\
+\x00\x00\x07\x10\x00\x00\x00\x00\x00\x01\x00\x01\x90\x5c\
+\x00\x00\x01\x81\x85\x13\x8d\x08\
 \x00\x00\x02\x9a\x00\x00\x00\x00\x00\x01\x00\x00\x86\x9c\
-\x00\x00\x01\x84E\x18^u\
-\x00\x00\x08N\x00\x00\x00\x00\x00\x01\x00\x01\xe3\x89\
-\x00\x00\x01\x84E\x18^\x89\
-\x00\x00\x04L\x00\x00\x00\x00\x00\x01\x00\x00\xe9\x03\
-\x00\x00\x01\x84E\x18^u\
+\x00\x00\x01\x81\x85\x13\x8d\x08\
+\x00\x00\x08N\x00\x00\x00\x00\x00\x01\x00\x01\xe3\x8b\
+\x00\x00\x01\x81\x85\x13\x8d\x1c\
+\x00\x00\x04L\x00\x00\x00\x00\x00\x01\x00\x00\xe9\x05\
+\x00\x00\x01\x81\x85\x13\x8d\x08\
 \x00\x00\x02\x0e\x00\x00\x00\x00\x00\x01\x00\x00i\xc6\
-\x00\x00\x01\x84E\x18^u\
+\x00\x00\x01\x81\x85\x13\x8c\xfe\
 \x00\x00\x02l\x00\x00\x00\x00\x00\x01\x00\x00\x83\x86\
-\x00\x00\x01\x84E\x18^\x7f\
-\x00\x00\x04\xee\x00\x00\x00\x00\x00\x01\x00\x01\x0f\xe1\
-\x00\x00\x01\x84E\x18^\x7f\
-\x00\x00\x04r\x00\x00\x00\x00\x00\x01\x00\x00\xf1\xa4\
-\x00\x00\x01\x84E\x18^\x89\
-\x00\x00\x05\xb6\x00\x00\x00\x00\x00\x01\x00\x01D\x1c\
-\x00\x00\x01\x84E\x18^\x89\
-\x00\x00\x05d\x00\x00\x00\x00\x00\x01\x00\x01.\xa8\
-\x00\x00\x01\x84E\x18^u\
-\x00\x00\x07\xc8\x00\x00\x00\x00\x00\x01\x00\x01\xbd\xb5\
-\x00\x00\x01\x84E\x18^u\
+\x00\x00\x01\x81\x85\x13\x8d\x08\
+\x00\x00\x04\xee\x00\x00\x00\x00\x00\x01\x00\x01\x0f\xe3\
+\x00\x00\x01\x81\x85\x13\x8d\x08\
+\x00\x00\x04r\x00\x00\x00\x00\x00\x01\x00\x00\xf1\xa6\
+\x00\x00\x01\x81\x85\x13\x8d\x1c\
+\x00\x00\x05\xb6\x00\x00\x00\x00\x00\x01\x00\x01D\x1e\
+\x00\x00\x01\x81\x85\x13\x8d\x1c\
+\x00\x00\x05d\x00\x00\x00\x00\x00\x01\x00\x01.\xaa\
+\x00\x00\x01\x81\x85\x13\x8d\x08\
+\x00\x00\x07\xc8\x00\x00\x00\x00\x00\x01\x00\x01\xbd\xb7\
+\x00\x00\x01\x81\x85\x13\x8c\xfe\
 \x00\x00\x03J\x00\x00\x00\x00\x00\x01\x00\x00\xaa\xd3\
-\x00\x00\x01\x84E\x18^\x89\
+\x00\x00\x01\x81\x85\x13\x8d\x12\
 \x00\x00\x00J\x00\x00\x00\x00\x00\x01\x00\x00\x00\x00\
-\x00\x00\x01\x84E\x18^u\
-\x00\x00\x09d\x00\x00\x00\x00\x00\x01\x00\x02@\x98\
-\x00\x00\x01\x84E\x18^\x93\
-\x00\x00\x09\xe0\x00\x00\x00\x00\x00\x01\x00\x02\x9fl\
-\x00\x00\x01\x84E\x18^\x93\
-\x00\x00\x09\x8a\x00\x00\x00\x00\x00\x01\x00\x02ak\
-\x00\x00\x01\x84E\x18^\x93\
-\x00\x00\x09\xb4\x00\x00\x00\x00\x00\x01\x00\x02~\x1f\
-\x00\x00\x01\x84E\x18^\x93\
-\x00\x00\x0a\x10\x00\x01\x00\x00\x00\x01\x00\x03\x1e\xcc\
-\x00\x00\x01\x84E\x18^\x93\
+\x00\x00\x01\x81\x85\x13\x8c\xfe\
+\x00\x00\x09d\x00\x00\x00\x00\x00\x01\x00\x02@\x9a\
+\x00\x00\x01\x81\x85\x13\x8d&\
+\x00\x00\x09\xe0\x00\x00\x00\x00\x00\x01\x00\x02\x9fn\
+\x00\x00\x01\x81\x85\x13\x8d&\
+\x00\x00\x09\x8a\x00\x00\x00\x00\x00\x01\x00\x02am\
+\x00\x00\x01\x81\x85\x13\x8d&\
+\x00\x00\x09\xb4\x00\x00\x00\x00\x00\x01\x00\x02~!\
+\x00\x00\x01\x81\x85\x13\x8d&\
+\x00\x00\x0a\x10\x00\x01\x00\x00\x00\x01\x00\x03\x1e\xce\
+\x00\x00\x01\x81\x85\x13\x8d&\
 "
 
 def qInitResources():
     QtCore.qRegisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
 
 def qCleanupResources():
     QtCore.qUnregisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
```

### Comparing `qute_style-1.0.5/qute_style/startup_threads.py` & `qute_style-1.0.6/qute_style/startup_threads.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/style.py` & `qute_style-1.0.6/qute_style/style.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/ui/test_window.ui` & `qute_style-1.0.6/qute_style/ui/test_window.ui`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/ui/whats_new_window.ui` & `qute_style-1.0.6/qute_style/ui/whats_new_window.ui`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/widgets/background_frame.py` & `qute_style-1.0.6/qute_style/widgets/background_frame.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/widgets/base_widgets.py` & `qute_style-1.0.6/qute_style/widgets/base_widgets.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/widgets/color_manager.py` & `qute_style-1.0.6/qute_style/widgets/color_manager.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/widgets/credit_bar.py` & `qute_style-1.0.6/qute_style/widgets/credit_bar.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/widgets/custom_icon_engine.py` & `qute_style-1.0.6/qute_style/widgets/custom_icon_engine.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/widgets/drop_label.py` & `qute_style-1.0.6/qute_style/widgets/drop_label.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/widgets/grips.py` & `qute_style-1.0.6/qute_style/widgets/grips.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/widgets/home_page.py` & `qute_style-1.0.6/qute_style/widgets/home_page.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/widgets/icon.py` & `qute_style-1.0.6/qute_style/widgets/icon.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/widgets/icon_button.py` & `qute_style-1.0.6/qute_style/widgets/icon_button.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,17 +41,17 @@
         icon_path: str = ":/svg_icons/no_icon.svg",
         bgs: BackgroundColorNames | None = None,
         text: str | None = None,
         margin: float = 0.6,
     ) -> None:
         """Create a new IconButton."""
         if text:
-            super().__init__(text=text, parent=parent)
+            super().__init__(text, parent)
         else:
-            super().__init__(parent=parent)
+            super().__init__(parent)
         self._bgs = bgs or BackgroundColorNames(
             hovering="bg_elements",
             background="transparent",
             pressed="dark_two",
             released="bg_elements",
         )
```

### Comparing `qute_style-1.0.5/qute_style/widgets/icon_tooltip_button.py` & `qute_style-1.0.6/qute_style/widgets/icon_tooltip_button.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/widgets/left_column.py` & `qute_style-1.0.6/qute_style/widgets/left_column.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/widgets/left_column_close_button.py` & `qute_style-1.0.6/qute_style/widgets/left_column_close_button.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/widgets/left_menu.py` & `qute_style-1.0.6/qute_style/widgets/left_menu.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/widgets/left_menu_button.py` & `qute_style-1.0.6/qute_style/widgets/left_menu_button.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/widgets/spinner.py` & `qute_style-1.0.6/qute_style/widgets/spinner.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/widgets/styled_combobox.py` & `qute_style-1.0.6/qute_style/widgets/styled_combobox.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/widgets/text_truncator.py` & `qute_style-1.0.6/qute_style/widgets/text_truncator.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/widgets/title_bar.py` & `qute_style-1.0.6/qute_style/widgets/title_bar.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,17 @@
             return True
         if event.type() == QEvent.Type.MouseButtonDblClick:
             self._double_click_in_progress = True
             self.maximize.emit()
             return True
         if event.type() == QEvent.Type.MouseMove:
             if not self._double_click_in_progress:
-                self.move_window.emit(cast(QMouseEvent, event).globalPos())
+                self.move_window.emit(
+                    cast(QMouseEvent, event).globalPosition().toPoint()
+                )
             return True
         return False
 
     def set_maximized(self, maximized: bool) -> None:
         """Set the _background icon depending if the app is maximized."""
         name = "fullscreen_exit" if maximized else "fullscreen"
         self.maximize_button.set_icon(f":/svg_icons/{name}.svg")
```

### Comparing `qute_style-1.0.5/qute_style/widgets/title_button.py` & `qute_style-1.0.6/qute_style/widgets/title_button.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/widgets/toggle.py` & `qute_style-1.0.6/qute_style/widgets/toggle.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style/widgets/tooltip.py` & `qute_style-1.0.6/qute_style/widgets/tooltip.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style_examples/example_images/color_manager.PNG` & `qute_style-1.0.6/qute_style_examples/example_images/color_manager.PNG`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style_examples/example_images/custom_style.PNG` & `qute_style-1.0.6/qute_style_examples/example_images/custom_style.PNG`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style_examples/example_images/darcula.PNG` & `qute_style-1.0.6/qute_style_examples/example_images/darcula.PNG`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style_examples/example_images/drop_label.PNG` & `qute_style-1.0.6/qute_style_examples/example_images/drop_label.PNG`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style_examples/example_images/highbridge_grey.PNG` & `qute_style-1.0.6/qute_style_examples/example_images/highbridge_grey.PNG`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style_examples/example_images/information_messagebox.PNG` & `qute_style-1.0.6/qute_style_examples/example_images/information_messagebox.PNG`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style_examples/example_images/princesspink.PNG` & `qute_style-1.0.6/qute_style_examples/example_images/princesspink.PNG`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style_examples/example_images/rubyred.PNG` & `qute_style-1.0.6/qute_style_examples/example_images/rubyred.PNG`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style_examples/example_images/snowwhite.PNG` & `qute_style-1.0.6/qute_style_examples/example_images/snowwhite.PNG`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style_examples/example_images/widgets_display.PNG` & `qute_style-1.0.6/qute_style_examples/example_images/widgets_display.PNG`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style_examples/main.py` & `qute_style-1.0.6/qute_style_examples/main.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style_examples/sample_classes.py` & `qute_style-1.0.6/qute_style_examples/sample_classes.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style_examples/sample_main_window.py` & `qute_style-1.0.6/qute_style_examples/sample_main_window.py`

 * *Files 7% similar despite different names*

```diff
@@ -78,26 +78,28 @@
         SpinnerWidget,
     ]
     RIGHT_WIDGET_CLASSES = [ColorManager]
     LEFT_WIDGET_CLASSES = [SettingsWidget, InfoWidget]
 
     MIN_SIZE = QSize(800, 600)
 
-    def __init__(
+    def __init__(  # pylint: disable=too-many-arguments
         self,
         app_data: AppData,
         registry_reset: bool = False,
         force_whats_new: bool = False,
+        load_last_used_widget: bool = False,
         parent: QWidget | None = None,
     ) -> None:
         """Create a new StyledMainWindow."""
         super().__init__(
             app_data,
             force_whats_new,
             registry_reset,
+            load_last_used_widget,
             parent,
         )
         self._left_column.widget(InfoWidget).switch_style.connect(
             self.on_switch_style
         )
 
         try:
```

### Comparing `qute_style-1.0.5/qute_style_examples/sample_widgets.py` & `qute_style-1.0.6/qute_style_examples/sample_widgets.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style_examples/test_changelog/1.01/bug.png` & `qute_style-1.0.6/qute_style_examples/test_changelog/1.01/bug.png`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/qute_style_examples/test_changelog/1.10/bug.png` & `qute_style-1.0.6/qute_style_examples/test_changelog/1.10/bug.png`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.5/PKG-INFO` & `qute_style-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: qute-style
-Version: 1.0.5
+Version: 1.0.6
 Summary: QuteStyle is an expandable application framework for PySide6
 Home-page: https://github.com/TUV-SUD-Product-Service-GmbH/QuteStyle
 License: MIT
 Author: Marina Baumgartner, Dairen Gonschior, Tilman Krummeck, Dennis Spitzhorn, Gerhard Trapp, Patrick Zwerschke
 Author-email: PS-TF-Entwicklung@tuev-sued.de
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: PySide6 (==6.4.2)
+Requires-Dist: PySide6 (==6.5.1.1)
 Project-URL: Repository, https://github.com/TUV-SUD-Product-Service-GmbH/QuteStyle
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://github.com/TUV-SUD-Product-Service-GmbH/QuteStyle">
     <img src="https://github.com/TUV-SUD-Product-Service-GmbH/QuteStyle/raw/master/qute_style/resources/svg_images/banner_qute_style.svg" alt="QuteStyle logo" width="500" height="200">
   </a>
```

