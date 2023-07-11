# Comparing `tmp/nanome-0.8.3.tar.gz` & `tmp/nanome-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\nanome-0.8.3.tar", last modified: Wed Oct 16 22:17:13 2019, max compression
+gzip compressed data, was "dist\nanome-0.9.0.tar", last modified: Wed Nov  6 18:07:52 2019, max compression
```

## Comparing `nanome-0.8.3.tar` & `nanome-0.9.0.tar`

### file list

```diff
@@ -1,294 +1,295 @@
-drwxrwxrwx   0        0        0        0 2019-10-16 22:17:13.000000 nanome-0.8.3/
--rw-rw-rw-   0        0        0     1510 2019-10-16 22:17:13.000000 nanome-0.8.3/PKG-INFO
--rw-rw-rw-   0        0        0      588 2019-06-13 20:32:12.000000 nanome-0.8.3/README.md
-drwxrwxrwx   0        0        0        0 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome/
--rw-rw-rw-   0        0        0      107 2019-10-16 22:17:11.000000 nanome-0.8.3/nanome/__init__.py
-drwxrwxrwx   0        0        0        0 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome/_internal/
--rw-rw-rw-   0        0        0      279 2019-08-15 16:57:23.000000 nanome-0.8.3/nanome/_internal/__init__.py
--rw-rw-rw-   0        0        0      271 2019-03-08 05:32:49.000000 nanome-0.8.3/nanome/_internal/_addon.py
-drwxrwxrwx   0        0        0        0 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome/_internal/_macro/
--rw-rw-rw-   0        0        0       58 2019-08-15 16:57:23.000000 nanome-0.8.3/nanome/_internal/_macro/__init__.py
--rw-rw-rw-   0        0        0     1279 2019-08-15 16:57:23.000000 nanome-0.8.3/nanome/_internal/_macro/_macro.py
-drwxrwxrwx   0        0        0        0 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome/_internal/_macro/_serialization/
--rw-rw-rw-   0        0        0       64 2019-08-15 16:57:23.000000 nanome-0.8.3/nanome/_internal/_macro/_serialization/__init__.py
--rw-rw-rw-   0        0        0      785 2019-08-15 16:57:23.000000 nanome-0.8.3/nanome/_internal/_macro/_serialization/_macro_serializer.py
-drwxrwxrwx   0        0        0        0 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome/_internal/_network/
--rw-rw-rw-   0        0        0      266 2019-02-22 07:08:10.000000 nanome-0.8.3/nanome/_internal/_network/__init__.py
-drwxrwxrwx   0        0        0        0 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome/_internal/_network/_commands/
--rw-rw-rw-   0        0        0       91 2019-02-22 07:08:10.000000 nanome-0.8.3/nanome/_internal/_network/_commands/__init__.py
-drwxrwxrwx   0        0        0        0 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_callbacks/
--rw-rw-rw-   0        0        0     1325 2019-09-26 17:02:56.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_callbacks/__init__.py
--rw-rw-rw-   0        0        0       90 2019-04-21 02:15:45.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_callbacks/_add_bonds_result.py
--rw-rw-rw-   0        0        0       89 2019-05-23 18:17:50.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_callbacks/_add_dssp_done.py
--rw-rw-rw-   0        0        0       86 2019-03-08 05:32:49.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_callbacks/_advanced_settings.py
--rw-rw-rw-   0        0        0     4228 2019-09-26 17:02:56.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_callbacks/_commands_enums.py
--rw-rw-rw-   0        0        0      270 2019-05-23 22:21:21.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_callbacks/_complex_list.py
--rw-rw-rw-   0        0        0       49 2019-03-08 05:32:50.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_callbacks/_connect.py
--rw-rw-rw-   0        0        0      576 2019-09-26 17:02:56.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_callbacks/_create_stream_result.py
--rw-rw-rw-   0        0        0      147 2019-09-26 17:02:56.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_callbacks/_feed_stream.py
--rw-rw-rw-   0        0        0       82 2019-04-21 02:15:45.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_callbacks/_feed_stream_done.py
--rw-rw-rw-   0        0        0      299 2019-03-08 05:32:50.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_callbacks/_file.py
--rw-rw-rw-   0        0        0      418 2019-04-21 02:15:45.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_callbacks/_interrupt_stream.py
--rw-rw-rw-   0        0        0       82 2019-08-15 16:57:23.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_callbacks/_macro_callbacks.py
--rw-rw-rw-   0        0        0     2050 2019-07-01 20:09:33.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_callbacks/_menu.py
--rw-rw-rw-   0        0        0       90 2019-05-23 18:17:50.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_callbacks/_position_structures_done.py
--rw-rw-rw-   0        0        0       84 2019-09-26 17:02:56.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_callbacks/_presenter_change.py
--rw-rw-rw-   0        0        0       90 2019-09-26 17:02:56.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_callbacks/_receive_presenter_info.py
--rw-rw-rw-   0        0        0       61 2019-03-08 05:32:50.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_callbacks/_run.py
--rw-rw-rw-   0        0        0     3416 2019-09-26 17:02:56.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_callbacks/_ui_callbacks.py
--rw-rw-rw-   0        0        0       93 2019-04-21 02:15:45.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_callbacks/_update_structures_deep_done.py
--rw-rw-rw-   0        0        0       85 2019-05-23 18:17:50.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_callbacks/_upload_cryo_em_done.py
--rw-rw-rw-   0        0        0      328 2019-04-21 02:15:45.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_callbacks/_workspace_callbacks.py
-drwxrwxrwx   0        0        0        0 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/
--rw-rw-rw-   0        0        0     2138 2019-09-26 17:02:56.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/__init__.py
--rw-rw-rw-   0        0        0     1245 2019-06-06 16:05:56.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_add_bonds.py
--rw-rw-rw-   0        0        0     1222 2019-06-06 16:05:56.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_add_dssp.py
--rw-rw-rw-   0        0        0     1216 2019-06-06 16:05:56.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_add_to_workspace.py
--rw-rw-rw-   0        0        0      389 2019-03-08 05:32:50.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_advanced_settings.py
--rw-rw-rw-   0        0        0      891 2019-09-26 17:02:56.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_button_callback.py
--rw-rw-rw-   0        0        0      395 2019-04-21 02:15:45.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_complex_added_removed.py
--rw-rw-rw-   0        0        0      751 2019-06-06 16:05:56.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_connect.py
--rw-rw-rw-   0        0        0      641 2019-09-26 17:02:56.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_create_stream.py
--rw-rw-rw-   0        0        0      872 2019-09-26 17:02:56.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_create_stream_result.py
--rw-rw-rw-   0        0        0      418 2019-04-21 02:15:45.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_destroy_stream.py
--rw-rw-rw-   0        0        0     1064 2019-03-08 05:32:50.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_directory_request.py
--rw-rw-rw-   0        0        0     1451 2019-09-26 17:02:56.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_feed_stream.py
--rw-rw-rw-   0        0        0      402 2019-04-21 02:15:45.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_feed_stream_done.py
--rw-rw-rw-   0        0        0      798 2019-03-08 05:32:50.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_file_request.py
--rw-rw-rw-   0        0        0      692 2019-03-08 05:32:50.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_file_save.py
--rw-rw-rw-   0        0        0      379 2019-09-26 17:02:56.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_get_presenter_info.py
--rw-rw-rw-   0        0        0      755 2019-09-26 17:02:56.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_get_presenter_info_response.py
--rw-rw-rw-   0        0        0      944 2019-08-15 16:57:23.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_image_callback.py
--rw-rw-rw-   0        0        0      478 2019-04-21 02:15:45.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_interrupt_stream.py
--rw-rw-rw-   0        0        0     3412 2019-08-15 16:57:23.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_macro_commands.py
--rw-rw-rw-   0        0        0      423 2019-03-08 05:32:50.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_menu_callback.py
--rw-rw-rw-   0        0        0      527 2019-08-29 18:22:25.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_open_url.py
--rw-rw-rw-   0        0        0     1378 2019-06-06 16:05:56.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_position_structures.py
--rw-rw-rw-   0        0        0      418 2019-05-23 18:17:50.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_position_structures_done.py
--rw-rw-rw-   0        0        0      377 2019-09-26 17:02:56.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_presenter_change.py
--rw-rw-rw-   0        0        0     1740 2019-04-21 02:15:45.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_receive_complex_list.py
--rw-rw-rw-   0        0        0     1056 2019-03-08 05:32:50.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_receive_menu.py
--rw-rw-rw-   0        0        0      971 2019-03-08 05:32:50.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_receive_workspace.py
--rw-rw-rw-   0        0        0      890 2019-06-06 16:05:56.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_request_complex_list.py
--rw-rw-rw-   0        0        0      379 2019-03-08 05:32:50.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_request_workspace.py
--rw-rw-rw-   0        0        0      353 2019-03-08 05:32:50.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_run.py
--rw-rw-rw-   0        0        0      865 2019-04-21 02:15:45.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_send_notification.py
--rw-rw-rw-   0        0        0      553 2019-03-08 05:32:50.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_set_plugin_list_button.py
--rw-rw-rw-   0        0        0      737 2019-08-15 16:57:23.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_slider_callback.py
--rw-rw-rw-   0        0        0      859 2019-08-15 16:57:23.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_text_input_callback.py
--rw-rw-rw-   0        0        0      525 2019-03-08 05:32:50.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_update_content.py
--rw-rw-rw-   0        0        0      988 2019-03-08 05:32:50.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_update_menu.py
--rw-rw-rw-   0        0        0     3236 2019-06-13 20:32:12.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_update_structures.py
--rw-rw-rw-   0        0        0      421 2019-04-21 02:15:45.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_update_structures_deep_done.py
--rw-rw-rw-   0        0        0     1190 2019-06-06 16:05:56.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_update_workspace.py
--rw-rw-rw-   0        0        0      781 2019-05-23 18:17:50.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_upload_cryo_em.py
--rw-rw-rw-   0        0        0      406 2019-05-23 18:17:50.000000 nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_upload_cryo_em_done.py
--rw-rw-rw-   0        0        0     8383 2019-09-26 17:02:56.000000 nanome-0.8.3/nanome/_internal/_network/_data.py
--rw-rw-rw-   0        0        0     3314 2019-08-15 16:57:23.000000 nanome-0.8.3/nanome/_internal/_network/_net_instance.py
--rw-rw-rw-   0        0        0     2739 2019-08-15 16:57:23.000000 nanome-0.8.3/nanome/_internal/_network/_packet.py
--rw-rw-rw-   0        0        0     3206 2019-09-26 17:02:56.000000 nanome-0.8.3/nanome/_internal/_network/_process_network.py
-drwxrwxrwx   0        0        0        0 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome/_internal/_network/_serialization/
--rw-rw-rw-   0        0        0      132 2019-02-22 07:08:10.000000 nanome-0.8.3/nanome/_internal/_network/_serialization/__init__.py
--rw-rw-rw-   0        0        0     8389 2019-09-26 17:02:56.000000 nanome-0.8.3/nanome/_internal/_network/_serialization/_context.py
--rw-rw-rw-   0        0        0    13062 2019-09-26 17:02:56.000000 nanome-0.8.3/nanome/_internal/_network/_serialization/_serializer.py
--rw-rw-rw-   0        0        0     2432 2019-09-26 17:02:56.000000 nanome-0.8.3/nanome/_internal/_network/_session.py
--rw-rw-rw-   0        0        0    10221 2019-10-16 22:16:06.000000 nanome-0.8.3/nanome/_internal/_plugin.py
--rw-rw-rw-   0        0        0     2442 2019-09-12 17:08:22.000000 nanome-0.8.3/nanome/_internal/_plugin_instance.py
-drwxrwxrwx   0        0        0        0 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome/_internal/_process/
--rw-rw-rw-   0        0        0      237 2019-08-15 16:57:23.000000 nanome-0.8.3/nanome/_internal/_process/__init__.py
--rw-rw-rw-   0        0        0     3782 2019-08-15 16:57:23.000000 nanome-0.8.3/nanome/_internal/_process/_bonding.py
--rw-rw-rw-   0        0        0     5735 2019-08-15 17:19:40.000000 nanome-0.8.3/nanome/_internal/_process/_dssp.py
-drwxrwxrwx   0        0        0        0 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome/_internal/_process/_external/
-drwxrwxrwx   0        0        0        0 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome/_internal/_process/_external/_dssp/
--rwxrwxrwx   0        0        0  1223168 2019-08-15 16:57:23.000000 nanome-0.8.3/nanome/_internal/_process/_external/_dssp/dssp-3.0.0-win32.exe
--rw-rw-rw-   0        0        0  4079000 2019-08-15 16:57:23.000000 nanome-0.8.3/nanome/_internal/_process/_external/_dssp/dssp-linux
--rw-rw-rw-   0        0        0      917 2019-08-15 16:57:23.000000 nanome-0.8.3/nanome/_internal/_process/_process_entry.py
--rw-rw-rw-   0        0        0     4554 2019-08-15 16:57:23.000000 nanome-0.8.3/nanome/_internal/_process/_process_manager.py
--rw-rw-rw-   0        0        0     1895 2019-09-12 17:08:22.000000 nanome-0.8.3/nanome/_internal/_process/_process_manager_instance.py
-drwxrwxrwx   0        0        0        0 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome/_internal/_structure/
--rw-rw-rw-   0        0        0      334 2019-10-16 22:16:06.000000 nanome-0.8.3/nanome/_internal/_structure/__init__.py
--rw-rw-rw-   0        0        0     5348 2019-10-16 22:16:06.000000 nanome-0.8.3/nanome/_internal/_structure/_atom.py
--rw-rw-rw-   0        0        0      122 2019-09-12 17:08:22.000000 nanome-0.8.3/nanome/_internal/_structure/_base.py
--rw-rw-rw-   0        0        0     3912 2019-10-16 22:16:06.000000 nanome-0.8.3/nanome/_internal/_structure/_bond.py
--rw-rw-rw-   0        0        0     1104 2019-10-16 22:16:06.000000 nanome-0.8.3/nanome/_internal/_structure/_chain.py
--rw-rw-rw-   0        0        0     3434 2019-10-16 22:16:07.000000 nanome-0.8.3/nanome/_internal/_structure/_complex.py
-drwxrwxrwx   0        0        0        0 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome/_internal/_structure/_helpers/
--rw-rw-rw-   0        0        0       52 2019-10-16 22:16:07.000000 nanome-0.8.3/nanome/_internal/_structure/_helpers/__init__.py
--rw-rw-rw-   0        0        0    11836 2019-10-16 22:16:07.000000 nanome-0.8.3/nanome/_internal/_structure/_helpers/_conformer_helper.py
--rw-rw-rw-   0        0        0     1726 2019-10-16 22:16:07.000000 nanome-0.8.3/nanome/_internal/_structure/_helpers/_copy.py
-drwxrwxrwx   0        0        0        0 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome/_internal/_structure/_io/
--rw-rw-rw-   0        0        0       77 2019-02-22 07:08:10.000000 nanome-0.8.3/nanome/_internal/_structure/_io/__init__.py
-drwxrwxrwx   0        0        0        0 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome/_internal/_structure/_io/_mmcif/
--rw-rw-rw-   0        0        0      108 2019-06-06 16:05:56.000000 nanome-0.8.3/nanome/_internal/_structure/_io/_mmcif/__init__.py
--rw-rw-rw-   0        0        0     1130 2019-06-13 20:32:12.000000 nanome-0.8.3/nanome/_internal/_structure/_io/_mmcif/content.py
--rw-rw-rw-   0        0        0    16719 2019-06-06 16:05:56.000000 nanome-0.8.3/nanome/_internal/_structure/_io/_mmcif/parse.py
--rw-rw-rw-   0        0        0     8281 2019-10-16 22:16:07.000000 nanome-0.8.3/nanome/_internal/_structure/_io/_mmcif/save.py
--rw-rw-rw-   0        0        0     4911 2019-10-16 22:16:07.000000 nanome-0.8.3/nanome/_internal/_structure/_io/_mmcif/structure.py
-drwxrwxrwx   0        0        0        0 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome/_internal/_structure/_io/_pdb/
--rw-rw-rw-   0        0        0      108 2019-06-06 16:05:56.000000 nanome-0.8.3/nanome/_internal/_structure/_io/_pdb/__init__.py
--rw-rw-rw-   0        0        0     3331 2019-03-08 05:32:50.000000 nanome-0.8.3/nanome/_internal/_structure/_io/_pdb/content.py
--rw-rw-rw-   0        0        0    12662 2019-09-12 17:08:22.000000 nanome-0.8.3/nanome/_internal/_structure/_io/_pdb/parse.py
--rw-rw-rw-   0        0        0     6143 2019-10-16 22:16:07.000000 nanome-0.8.3/nanome/_internal/_structure/_io/_pdb/save.py
--rw-rw-rw-   0        0        0     2865 2019-10-16 22:16:07.000000 nanome-0.8.3/nanome/_internal/_structure/_io/_pdb/structure.py
-drwxrwxrwx   0        0        0        0 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome/_internal/_structure/_io/_sdf/
--rw-rw-rw-   0        0        0      108 2019-06-06 16:05:56.000000 nanome-0.8.3/nanome/_internal/_structure/_io/_sdf/__init__.py
--rw-rw-rw-   0        0        0      814 2019-03-08 05:32:50.000000 nanome-0.8.3/nanome/_internal/_structure/_io/_sdf/content.py
--rw-rw-rw-   0        0        0     6103 2019-06-06 16:05:56.000000 nanome-0.8.3/nanome/_internal/_structure/_io/_sdf/parse.py
--rw-rw-rw-   0        0        0     5346 2019-10-16 22:16:07.000000 nanome-0.8.3/nanome/_internal/_structure/_io/_sdf/save.py
--rw-rw-rw-   0        0        0     1619 2019-10-16 22:16:07.000000 nanome-0.8.3/nanome/_internal/_structure/_io/_sdf/structure.py
--rw-rw-rw-   0        0        0     4560 2019-10-16 22:16:07.000000 nanome-0.8.3/nanome/_internal/_structure/_molecule.py
--rw-rw-rw-   0        0        0     2796 2019-10-16 22:16:07.000000 nanome-0.8.3/nanome/_internal/_structure/_residue.py
-drwxrwxrwx   0        0        0        0 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome/_internal/_structure/_serialization/
--rw-rw-rw-   0        0        0      411 2019-04-21 02:15:45.000000 nanome-0.8.3/nanome/_internal/_structure/_serialization/__init__.py
--rw-rw-rw-   0        0        0     4750 2019-10-16 22:16:07.000000 nanome-0.8.3/nanome/_internal/_structure/_serialization/_atom_serializer.py
--rw-rw-rw-   0        0        0      895 2019-06-20 19:01:39.000000 nanome-0.8.3/nanome/_internal/_structure/_serialization/_atom_serializer_id.py
--rw-rw-rw-   0        0        0     2477 2019-10-16 22:16:07.000000 nanome-0.8.3/nanome/_internal/_structure/_serialization/_bond_serializer.py
--rw-rw-rw-   0        0        0     1231 2019-09-12 17:08:22.000000 nanome-0.8.3/nanome/_internal/_structure/_serialization/_chain_serializer.py
--rw-rw-rw-   0        0        0     3689 2019-09-12 17:08:22.000000 nanome-0.8.3/nanome/_internal/_structure/_serialization/_complex_serializer.py
--rw-rw-rw-   0        0        0     3039 2019-09-12 17:08:22.000000 nanome-0.8.3/nanome/_internal/_structure/_serialization/_molecule_serializer.py
--rw-rw-rw-   0        0        0     2973 2019-09-12 17:08:22.000000 nanome-0.8.3/nanome/_internal/_structure/_serialization/_residue_serializer.py
--rw-rw-rw-   0        0        0     1341 2019-06-13 20:32:12.000000 nanome-0.8.3/nanome/_internal/_structure/_serialization/_workspace_serializer.py
--rw-rw-rw-   0        0        0     1258 2019-06-13 20:32:12.000000 nanome-0.8.3/nanome/_internal/_structure/_workspace.py
-drwxrwxrwx   0        0        0        0 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome/_internal/_ui/
--rw-rw-rw-   0        0        0      433 2019-04-21 02:15:45.000000 nanome-0.8.3/nanome/_internal/_ui/__init__.py
--rw-rw-rw-   0        0        0     4823 2019-09-26 17:02:56.000000 nanome-0.8.3/nanome/_internal/_ui/_button.py
--rw-rw-rw-   0        0        0     1447 2019-05-26 21:55:20.000000 nanome-0.8.3/nanome/_internal/_ui/_image.py
-drwxrwxrwx   0        0        0        0 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome/_internal/_ui/_io/
--rw-rw-rw-   0        0        0      304 2019-04-21 02:15:45.000000 nanome-0.8.3/nanome/_internal/_ui/_io/__init__.py
--rw-rw-rw-   0        0        0     6256 2019-10-16 22:16:07.000000 nanome-0.8.3/nanome/_internal/_ui/_io/_button_json.py
--rw-rw-rw-   0        0        0      644 2019-05-26 21:55:20.000000 nanome-0.8.3/nanome/_internal/_ui/_io/_image_json.py
--rw-rw-rw-   0        0        0     1724 2019-05-26 21:55:20.000000 nanome-0.8.3/nanome/_internal/_ui/_io/_label_json.py
--rw-rw-rw-   0        0        0     2161 2019-07-01 20:09:33.000000 nanome-0.8.3/nanome/_internal/_ui/_io/_layout_node_json.py
--rw-rw-rw-   0        0        0      702 2019-04-21 02:15:45.000000 nanome-0.8.3/nanome/_internal/_ui/_io/_loading_bar_json.py
--rw-rw-rw-   0        0        0      721 2019-04-21 02:15:45.000000 nanome-0.8.3/nanome/_internal/_ui/_io/_menu_json.py
--rw-rw-rw-   0        0        0      349 2019-02-22 07:08:10.000000 nanome-0.8.3/nanome/_internal/_ui/_io/_mesh_json.py
--rw-rw-rw-   0        0        0      526 2019-02-22 07:08:10.000000 nanome-0.8.3/nanome/_internal/_ui/_io/_slider_json.py
--rw-rw-rw-   0        0        0      589 2019-02-22 07:08:10.000000 nanome-0.8.3/nanome/_internal/_ui/_io/_text_input_json.py
--rw-rw-rw-   0        0        0     2473 2019-04-21 02:15:45.000000 nanome-0.8.3/nanome/_internal/_ui/_io/_ui_base_json.py
--rw-rw-rw-   0        0        0      696 2019-04-21 02:15:45.000000 nanome-0.8.3/nanome/_internal/_ui/_io/_ui_list_json.py
--rw-rw-rw-   0        0        0     1478 2019-05-26 21:55:20.000000 nanome-0.8.3/nanome/_internal/_ui/_label.py
--rw-rw-rw-   0        0        0     3988 2019-07-01 20:09:33.000000 nanome-0.8.3/nanome/_internal/_ui/_layout_node.py
--rw-rw-rw-   0        0        0      573 2019-04-21 02:15:45.000000 nanome-0.8.3/nanome/_internal/_ui/_loading_bar.py
--rw-rw-rw-   0        0        0     1385 2019-06-13 20:32:12.000000 nanome-0.8.3/nanome/_internal/_ui/_menu.py
--rw-rw-rw-   0        0        0      403 2019-03-08 05:32:50.000000 nanome-0.8.3/nanome/_internal/_ui/_mesh.py
-drwxrwxrwx   0        0        0        0 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome/_internal/_ui/_serialization/
--rw-rw-rw-   0        0        0      664 2019-04-21 02:15:45.000000 nanome-0.8.3/nanome/_internal/_ui/_serialization/__init__.py
--rw-rw-rw-   0        0        0     7212 2019-09-26 17:28:03.000000 nanome-0.8.3/nanome/_internal/_ui/_serialization/_button_serializer.py
--rw-rw-rw-   0        0        0     1838 2019-09-26 17:02:56.000000 nanome-0.8.3/nanome/_internal/_ui/_serialization/_image_serializer.py
--rw-rw-rw-   0        0        0     2427 2019-08-15 16:57:23.000000 nanome-0.8.3/nanome/_internal/_ui/_serialization/_label_serializer.py
--rw-rw-rw-   0        0        0     2728 2019-08-15 16:57:23.000000 nanome-0.8.3/nanome/_internal/_ui/_serialization/_layout_node_serializer.py
--rw-rw-rw-   0        0        0     2460 2019-07-01 20:21:41.000000 nanome-0.8.3/nanome/_internal/_ui/_serialization/_layout_node_serializer_deep.py
--rw-rw-rw-   0        0        0     1516 2019-08-15 16:57:23.000000 nanome-0.8.3/nanome/_internal/_ui/_serialization/_loading_bar_serializer.py
--rw-rw-rw-   0        0        0     1198 2019-06-13 20:32:12.000000 nanome-0.8.3/nanome/_internal/_ui/_serialization/_menu_serializer.py
--rw-rw-rw-   0        0        0     1145 2019-08-15 16:57:23.000000 nanome-0.8.3/nanome/_internal/_ui/_serialization/_mesh_serializer.py
--rw-rw-rw-   0        0        0     1280 2019-08-15 16:57:23.000000 nanome-0.8.3/nanome/_internal/_ui/_serialization/_slider_serializer.py
--rw-rw-rw-   0        0        0     1503 2019-08-15 16:57:23.000000 nanome-0.8.3/nanome/_internal/_ui/_serialization/_text_input_serializer.py
--rw-rw-rw-   0        0        0     1631 2019-04-21 02:15:45.000000 nanome-0.8.3/nanome/_internal/_ui/_serialization/_ui_base_serializer.py
--rw-rw-rw-   0        0        0     1691 2019-08-15 16:57:23.000000 nanome-0.8.3/nanome/_internal/_ui/_serialization/_ui_list_serializer.py
--rw-rw-rw-   0        0        0      808 2019-03-08 05:32:50.000000 nanome-0.8.3/nanome/_internal/_ui/_slider.py
--rw-rw-rw-   0        0        0      863 2019-03-08 05:32:50.000000 nanome-0.8.3/nanome/_internal/_ui/_text_input.py
--rw-rw-rw-   0        0        0      437 2019-04-21 02:15:45.000000 nanome-0.8.3/nanome/_internal/_ui/_ui_base.py
--rw-rw-rw-   0        0        0      757 2019-03-08 05:32:50.000000 nanome-0.8.3/nanome/_internal/_ui/_ui_list.py
-drwxrwxrwx   0        0        0        0 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome/_internal/_util/
--rw-rw-rw-   0        0        0       53 2019-02-22 07:08:10.000000 nanome-0.8.3/nanome/_internal/_util/__init__.py
-drwxrwxrwx   0        0        0        0 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome/_internal/_util/_serializers/
--rw-rw-rw-   0        0        0      820 2019-08-29 18:22:25.000000 nanome-0.8.3/nanome/_internal/_util/_serializers/__init__.py
--rw-rw-rw-   0        0        0     1079 2019-03-08 05:32:50.000000 nanome-0.8.3/nanome/_internal/_util/_serializers/_array_serializer.py
--rw-rw-rw-   0        0        0      407 2019-03-08 05:32:50.000000 nanome-0.8.3/nanome/_internal/_util/_serializers/_bool_serializer.py
--rw-rw-rw-   0        0        0      428 2019-03-08 05:32:50.000000 nanome-0.8.3/nanome/_internal/_util/_serializers/_byte_serializer.py
--rw-rw-rw-   0        0        0      465 2019-03-08 05:32:50.000000 nanome-0.8.3/nanome/_internal/_util/_serializers/_color_serializer.py
--rw-rw-rw-   0        0        0     1126 2019-03-08 05:32:50.000000 nanome-0.8.3/nanome/_internal/_util/_serializers/_dictionary_serializer.py
--rw-rw-rw-   0        0        0      663 2019-03-08 05:32:50.000000 nanome-0.8.3/nanome/_internal/_util/_serializers/_directory_entry_serializer.py
--rw-rw-rw-   0        0        0      686 2019-03-08 05:32:50.000000 nanome-0.8.3/nanome/_internal/_util/_serializers/_file_data_serializer.py
--rw-rw-rw-   0        0        0      854 2019-03-08 05:32:50.000000 nanome-0.8.3/nanome/_internal/_util/_serializers/_file_save_data_serializer.py
--rw-rw-rw-   0        0        0      403 2019-03-08 05:32:50.000000 nanome-0.8.3/nanome/_internal/_util/_serializers/_int_serializer.py
--rw-rw-rw-   0        0        0      415 2019-03-08 05:32:50.000000 nanome-0.8.3/nanome/_internal/_util/_serializers/_long_serializer.py
--rw-rw-rw-   0        0        0      778 2019-05-23 18:17:50.000000 nanome-0.8.3/nanome/_internal/_util/_serializers/_quaternion_serializer.py
--rw-rw-rw-   0        0        0      810 2019-03-08 05:32:50.000000 nanome-0.8.3/nanome/_internal/_util/_serializers/_string_serializer.py
--rw-rw-rw-   0        0        0     1232 2019-03-08 05:32:50.000000 nanome-0.8.3/nanome/_internal/_util/_serializers/_tuple_serializer.py
--rw-rw-rw-   0        0        0     1212 2019-05-23 18:17:50.000000 nanome-0.8.3/nanome/_internal/_util/_serializers/_type_serializer.py
--rw-rw-rw-   0        0        0      626 2019-03-08 05:32:50.000000 nanome-0.8.3/nanome/_internal/_util/_serializers/_vector3_serializer.py
-drwxrwxrwx   0        0        0        0 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome/_internal/_volumetric/
--rw-rw-rw-   0        0        0       98 2019-05-23 18:17:50.000000 nanome-0.8.3/nanome/_internal/_volumetric/__init__.py
-drwxrwxrwx   0        0        0        0 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome/_internal/_volumetric/_io/
--rw-rw-rw-   0        0        0       21 2019-05-23 18:17:50.000000 nanome-0.8.3/nanome/_internal/_volumetric/_io/__init__.py
-drwxrwxrwx   0        0        0        0 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome/_internal/_volumetric/_io/_em_map/
--rw-rw-rw-   0        0        0       20 2019-05-23 18:17:50.000000 nanome-0.8.3/nanome/_internal/_volumetric/_io/_em_map/__init__.py
--rw-rw-rw-   0        0        0     2600 2019-05-23 18:17:50.000000 nanome-0.8.3/nanome/_internal/_volumetric/_io/_em_map/_parse.py
-drwxrwxrwx   0        0        0        0 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome/_internal/_volumetric/_serialization/
--rw-rw-rw-   0        0        0       58 2019-05-23 18:17:50.000000 nanome-0.8.3/nanome/_internal/_volumetric/_serialization/__init__.py
--rw-rw-rw-   0        0        0     1402 2019-06-06 16:05:56.000000 nanome-0.8.3/nanome/_internal/_volumetric/_serialization/_volume_data_serializer.py
--rw-rw-rw-   0        0        0      613 2019-05-23 18:17:50.000000 nanome-0.8.3/nanome/_internal/_volumetric/_volume_data.py
-drwxrwxrwx   0        0        0        0 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome/api/
--rw-rw-rw-   0        0        0      211 2019-09-26 17:02:56.000000 nanome-0.8.3/nanome/api/__init__.py
-drwxrwxrwx   0        0        0        0 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome/api/macro/
--rw-rw-rw-   0        0        0       24 2019-08-15 16:57:23.000000 nanome-0.8.3/nanome/api/macro/__init__.py
--rw-rw-rw-   0        0        0     1120 2019-08-15 16:57:23.000000 nanome-0.8.3/nanome/api/macro/macro.py
--rw-rw-rw-   0        0        0     3040 2019-08-15 16:57:23.000000 nanome-0.8.3/nanome/api/plugin.py
--rw-rw-rw-   0        0        0    13490 2019-09-26 17:02:56.000000 nanome-0.8.3/nanome/api/plugin_instance.py
-drwxrwxrwx   0        0        0        0 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome/api/streams/
--rw-rw-rw-   0        0        0       43 2019-04-21 02:15:45.000000 nanome-0.8.3/nanome/api/streams/__init__.py
--rw-rw-rw-   0        0        0     2802 2019-09-26 17:02:56.000000 nanome-0.8.3/nanome/api/streams/stream.py
-drwxrwxrwx   0        0        0        0 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome/api/structure/
--rw-rw-rw-   0        0        0      263 2019-05-23 18:17:50.000000 nanome-0.8.3/nanome/api/structure/__init__.py
--rw-rw-rw-   0        0        0     8505 2019-10-16 22:16:07.000000 nanome-0.8.3/nanome/api/structure/atom.py
--rw-rw-rw-   0        0        0      306 2019-05-23 18:17:50.000000 nanome-0.8.3/nanome/api/structure/base.py
--rw-rw-rw-   0        0        0     2957 2019-10-16 22:16:07.000000 nanome-0.8.3/nanome/api/structure/bond.py
--rw-rw-rw-   0        0        0     1773 2019-09-12 17:08:22.000000 nanome-0.8.3/nanome/api/structure/chain.py
--rw-rw-rw-   0        0        0     8993 2019-10-16 22:16:07.000000 nanome-0.8.3/nanome/api/structure/complex.py
-drwxrwxrwx   0        0        0        0 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome/api/structure/io/
--rw-rw-rw-   0        0        0       54 2019-02-22 07:08:10.000000 nanome-0.8.3/nanome/api/structure/io/__init__.py
--rw-rw-rw-   0        0        0     4396 2019-06-13 20:32:12.000000 nanome-0.8.3/nanome/api/structure/io/complex_io.py
--rw-rw-rw-   0        0        0       64 2019-03-08 05:32:50.000000 nanome-0.8.3/nanome/api/structure/io/molecule_io.py
--rw-rw-rw-   0        0        0       65 2019-03-08 05:32:50.000000 nanome-0.8.3/nanome/api/structure/io/workspace_io.py
--rw-rw-rw-   0        0        0     3418 2019-10-16 22:16:07.000000 nanome-0.8.3/nanome/api/structure/molecule.py
--rw-rw-rw-   0        0        0     6469 2019-10-16 22:16:07.000000 nanome-0.8.3/nanome/api/structure/residue.py
--rw-rw-rw-   0        0        0     1744 2019-06-13 20:32:12.000000 nanome-0.8.3/nanome/api/structure/workspace.py
-drwxrwxrwx   0        0        0        0 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome/api/ui/
--rw-rw-rw-   0        0        0      382 2019-04-21 02:15:45.000000 nanome-0.8.3/nanome/api/ui/__init__.py
--rw-rw-rw-   0        0        0    10106 2019-09-26 17:02:56.000000 nanome-0.8.3/nanome/api/ui/button.py
--rw-rw-rw-   0        0        0     1190 2019-08-15 16:57:23.000000 nanome-0.8.3/nanome/api/ui/image.py
-drwxrwxrwx   0        0        0        0 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome/api/ui/io/
--rw-rw-rw-   0        0        0       86 2019-05-23 18:17:50.000000 nanome-0.8.3/nanome/api/ui/io/__init__.py
--rw-rw-rw-   0        0        0     1337 2019-04-21 02:15:45.000000 nanome-0.8.3/nanome/api/ui/io/layout_node_io.py
--rw-rw-rw-   0        0        0     1394 2019-05-23 18:17:50.000000 nanome-0.8.3/nanome/api/ui/io/menu_io.py
--rw-rw-rw-   0        0        0     3210 2019-09-12 17:08:22.000000 nanome-0.8.3/nanome/api/ui/label.py
--rw-rw-rw-   0        0        0     7791 2019-07-01 20:09:33.000000 nanome-0.8.3/nanome/api/ui/layout_node.py
--rw-rw-rw-   0        0        0     1074 2019-09-12 17:08:22.000000 nanome-0.8.3/nanome/api/ui/loading_bar.py
--rw-rw-rw-   0        0        0     1685 2019-09-12 17:08:22.000000 nanome-0.8.3/nanome/api/ui/menu.py
--rw-rw-rw-   0        0        0      487 2019-04-21 02:15:45.000000 nanome-0.8.3/nanome/api/ui/mesh.py
--rw-rw-rw-   0        0        0     1445 2019-04-21 02:15:45.000000 nanome-0.8.3/nanome/api/ui/slider.py
--rw-rw-rw-   0        0        0     1870 2019-09-12 17:08:22.000000 nanome-0.8.3/nanome/api/ui/text_input.py
--rw-rw-rw-   0        0        0      216 2019-04-21 02:15:45.000000 nanome-0.8.3/nanome/api/ui/ui_base.py
--rw-rw-rw-   0        0        0     1309 2019-04-21 02:15:45.000000 nanome-0.8.3/nanome/api/ui/ui_list.py
-drwxrwxrwx   0        0        0        0 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome/api/user/
--rw-rw-rw-   0        0        0       41 2019-09-26 17:02:56.000000 nanome-0.8.3/nanome/api/user/__init__.py
--rw-rw-rw-   0        0        0      677 2019-09-26 17:02:56.000000 nanome-0.8.3/nanome/api/user/presenter_info.py
--rw-rw-rw-   0        0        0     2961 2019-10-16 22:13:32.000000 nanome-0.8.3/nanome/setup_config.py
-drwxrwxrwx   0        0        0        0 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome/util/
--rw-rw-rw-   0        0        0      610 2019-10-16 22:16:07.000000 nanome-0.8.3/nanome/util/__init__.py
--rw-rw-rw-   0        0        0      310 2019-03-08 05:32:50.000000 nanome-0.8.3/nanome/util/_logs_2.py
--rw-rw-rw-   0        0        0      315 2019-03-08 05:32:51.000000 nanome-0.8.3/nanome/util/_logs_3.py
--rw-rw-rw-   0        0        0     3185 2019-10-16 22:16:07.000000 nanome-0.8.3/nanome/util/color.py
--rw-rw-rw-   0        0        0      509 2019-06-06 16:05:56.000000 nanome-0.8.3/nanome/util/complex_save_options.py
--rw-rw-rw-   0        0        0     1656 2019-09-12 17:08:22.000000 nanome-0.8.3/nanome/util/config.py
--rw-rw-rw-   0        0        0    37006 2019-09-12 17:08:22.000000 nanome-0.8.3/nanome/util/enum.py
--rw-rw-rw-   0        0        0     1341 2019-09-26 18:33:51.000000 nanome-0.8.3/nanome/util/enums.py
--rw-rw-rw-   0        0        0     1008 2019-03-08 05:32:51.000000 nanome-0.8.3/nanome/util/file.py
--rw-rw-rw-   0        0        0      521 2019-03-08 05:32:51.000000 nanome-0.8.3/nanome/util/import_utils.py
--rw-rw-rw-   0        0        0     2831 2019-06-13 20:32:12.000000 nanome-0.8.3/nanome/util/logs.py
--rw-rw-rw-   0        0        0     5896 2019-05-23 18:17:50.000000 nanome-0.8.3/nanome/util/matrix.py
--rw-rw-rw-   0        0        0     5444 2019-05-23 18:17:50.000000 nanome-0.8.3/nanome/util/octree.py
--rw-rw-rw-   0        0        0     1622 2019-08-15 16:57:23.000000 nanome-0.8.3/nanome/util/process.py
--rw-rw-rw-   0        0        0     3006 2019-10-16 22:16:07.000000 nanome-0.8.3/nanome/util/quaternion.py
--rw-rw-rw-   0        0        0      212 2019-09-26 17:02:56.000000 nanome-0.8.3/nanome/util/stream.py
--rw-rw-rw-   0        0        0      293 2019-10-16 22:16:07.000000 nanome-0.8.3/nanome/util/string_builder.py
--rw-rw-rw-   0        0        0     1986 2019-10-16 22:16:07.000000 nanome-0.8.3/nanome/util/vector3.py
-drwxrwxrwx   0        0        0        0 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome.egg-info/
--rw-rw-rw-   0        0        0     1510 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    12212 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2019-10-16 22:17:13.000000 nanome-0.8.3/nanome.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      227 2019-10-16 22:17:13.000000 nanome-0.8.3/setup.cfg
--rw-rw-rw-   0        0        0     1295 2019-10-16 22:17:11.000000 nanome-0.8.3/setup.py
+drwxrwxrwx   0        0        0        0 2019-11-06 18:07:52.000000 nanome-0.9.0/
+-rw-rw-rw-   0        0        0     1510 2019-11-06 18:07:52.000000 nanome-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0      588 2019-06-13 20:32:12.000000 nanome-0.9.0/README.md
+drwxrwxrwx   0        0        0        0 2019-11-06 18:07:51.000000 nanome-0.9.0/nanome/
+-rw-rw-rw-   0        0        0      107 2019-11-06 18:07:49.000000 nanome-0.9.0/nanome/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-06 18:07:51.000000 nanome-0.9.0/nanome/_internal/
+-rw-rw-rw-   0        0        0      279 2019-08-15 16:57:23.000000 nanome-0.9.0/nanome/_internal/__init__.py
+-rw-rw-rw-   0        0        0      271 2019-03-08 05:32:49.000000 nanome-0.9.0/nanome/_internal/_addon.py
+drwxrwxrwx   0        0        0        0 2019-11-06 18:07:51.000000 nanome-0.9.0/nanome/_internal/_macro/
+-rw-rw-rw-   0        0        0       58 2019-08-15 16:57:23.000000 nanome-0.9.0/nanome/_internal/_macro/__init__.py
+-rw-rw-rw-   0        0        0     1279 2019-08-15 16:57:23.000000 nanome-0.9.0/nanome/_internal/_macro/_macro.py
+drwxrwxrwx   0        0        0        0 2019-11-06 18:07:51.000000 nanome-0.9.0/nanome/_internal/_macro/_serialization/
+-rw-rw-rw-   0        0        0       64 2019-08-15 16:57:23.000000 nanome-0.9.0/nanome/_internal/_macro/_serialization/__init__.py
+-rw-rw-rw-   0        0        0      785 2019-08-15 16:57:23.000000 nanome-0.9.0/nanome/_internal/_macro/_serialization/_macro_serializer.py
+drwxrwxrwx   0        0        0        0 2019-11-06 18:07:51.000000 nanome-0.9.0/nanome/_internal/_network/
+-rw-rw-rw-   0        0        0      266 2019-02-22 07:08:10.000000 nanome-0.9.0/nanome/_internal/_network/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-06 18:07:51.000000 nanome-0.9.0/nanome/_internal/_network/_commands/
+-rw-rw-rw-   0        0        0       91 2019-02-22 07:08:10.000000 nanome-0.9.0/nanome/_internal/_network/_commands/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-06 18:07:51.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_callbacks/
+-rw-rw-rw-   0        0        0     1325 2019-09-26 17:02:56.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_callbacks/__init__.py
+-rw-rw-rw-   0        0        0       90 2019-04-21 02:15:45.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_callbacks/_add_bonds_result.py
+-rw-rw-rw-   0        0        0       89 2019-05-23 18:17:50.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_callbacks/_add_dssp_done.py
+-rw-rw-rw-   0        0        0       86 2019-03-08 05:32:49.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_callbacks/_advanced_settings.py
+-rw-rw-rw-   0        0        0     4254 2019-10-23 18:54:22.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_callbacks/_commands_enums.py
+-rw-rw-rw-   0        0        0      270 2019-05-23 22:21:21.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_callbacks/_complex_list.py
+-rw-rw-rw-   0        0        0       49 2019-03-08 05:32:50.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_callbacks/_connect.py
+-rw-rw-rw-   0        0        0      576 2019-09-26 17:02:56.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_callbacks/_create_stream_result.py
+-rw-rw-rw-   0        0        0      147 2019-09-26 17:02:56.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_callbacks/_feed_stream.py
+-rw-rw-rw-   0        0        0       82 2019-04-21 02:15:45.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_callbacks/_feed_stream_done.py
+-rw-rw-rw-   0        0        0      299 2019-03-08 05:32:50.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_callbacks/_file.py
+-rw-rw-rw-   0        0        0      418 2019-04-21 02:15:45.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_callbacks/_interrupt_stream.py
+-rw-rw-rw-   0        0        0       82 2019-08-15 16:57:23.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_callbacks/_macro_callbacks.py
+-rw-rw-rw-   0        0        0     2050 2019-07-01 20:09:33.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_callbacks/_menu.py
+-rw-rw-rw-   0        0        0       90 2019-05-23 18:17:50.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_callbacks/_position_structures_done.py
+-rw-rw-rw-   0        0        0       84 2019-09-26 17:02:56.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_callbacks/_presenter_change.py
+-rw-rw-rw-   0        0        0       90 2019-09-26 17:02:56.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_callbacks/_receive_presenter_info.py
+-rw-rw-rw-   0        0        0       61 2019-03-08 05:32:50.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_callbacks/_run.py
+-rw-rw-rw-   0        0        0     3416 2019-09-26 17:02:56.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_callbacks/_ui_callbacks.py
+-rw-rw-rw-   0        0        0       93 2019-04-21 02:15:45.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_callbacks/_update_structures_deep_done.py
+-rw-rw-rw-   0        0        0       85 2019-05-23 18:17:50.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_callbacks/_upload_cryo_em_done.py
+-rw-rw-rw-   0        0        0      328 2019-04-21 02:15:45.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_callbacks/_workspace_callbacks.py
+drwxrwxrwx   0        0        0        0 2019-11-06 18:07:51.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/
+-rw-rw-rw-   0        0        0     2177 2019-10-23 18:54:22.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/__init__.py
+-rw-rw-rw-   0        0        0     1245 2019-06-06 16:05:56.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_add_bonds.py
+-rw-rw-rw-   0        0        0     1222 2019-06-06 16:05:56.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_add_dssp.py
+-rw-rw-rw-   0        0        0     1216 2019-06-06 16:05:56.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_add_to_workspace.py
+-rw-rw-rw-   0        0        0      389 2019-03-08 05:32:50.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_advanced_settings.py
+-rw-rw-rw-   0        0        0      891 2019-09-26 17:02:56.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_button_callback.py
+-rw-rw-rw-   0        0        0      395 2019-04-21 02:15:45.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_complex_added_removed.py
+-rw-rw-rw-   0        0        0      751 2019-06-06 16:05:56.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_connect.py
+-rw-rw-rw-   0        0        0      641 2019-09-26 17:02:56.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_create_stream.py
+-rw-rw-rw-   0        0        0      872 2019-09-26 17:02:56.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_create_stream_result.py
+-rw-rw-rw-   0        0        0      418 2019-04-21 02:15:45.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_destroy_stream.py
+-rw-rw-rw-   0        0        0     1064 2019-03-08 05:32:50.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_directory_request.py
+-rw-rw-rw-   0        0        0     1451 2019-09-26 17:02:56.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_feed_stream.py
+-rw-rw-rw-   0        0        0      402 2019-04-21 02:15:45.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_feed_stream_done.py
+-rw-rw-rw-   0        0        0      798 2019-03-08 05:32:50.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_file_request.py
+-rw-rw-rw-   0        0        0      692 2019-03-08 05:32:50.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_file_save.py
+-rw-rw-rw-   0        0        0      379 2019-09-26 17:02:56.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_get_presenter_info.py
+-rw-rw-rw-   0        0        0      755 2019-09-26 17:02:56.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_get_presenter_info_response.py
+-rw-rw-rw-   0        0        0      944 2019-08-15 16:57:23.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_image_callback.py
+-rw-rw-rw-   0        0        0      478 2019-04-21 02:15:45.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_interrupt_stream.py
+-rw-rw-rw-   0        0        0     3412 2019-08-15 16:57:23.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_macro_commands.py
+-rw-rw-rw-   0        0        0      423 2019-03-08 05:32:50.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_menu_callback.py
+-rw-rw-rw-   0        0        0      527 2019-08-29 18:22:25.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_open_url.py
+-rw-rw-rw-   0        0        0     1378 2019-06-06 16:05:56.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_position_structures.py
+-rw-rw-rw-   0        0        0      418 2019-05-23 18:17:50.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_position_structures_done.py
+-rw-rw-rw-   0        0        0      377 2019-09-26 17:02:56.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_presenter_change.py
+-rw-rw-rw-   0        0        0     1740 2019-04-21 02:15:45.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_receive_complex_list.py
+-rw-rw-rw-   0        0        0     1056 2019-03-08 05:32:50.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_receive_menu.py
+-rw-rw-rw-   0        0        0      971 2019-03-08 05:32:50.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_receive_workspace.py
+-rw-rw-rw-   0        0        0      890 2019-06-06 16:05:56.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_request_complex_list.py
+-rw-rw-rw-   0        0        0      379 2019-03-08 05:32:50.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_request_workspace.py
+-rw-rw-rw-   0        0        0      353 2019-03-08 05:32:50.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_run.py
+-rw-rw-rw-   0        0        0      865 2019-04-21 02:15:45.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_send_notification.py
+-rw-rw-rw-   0        0        0      553 2019-03-08 05:32:50.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_set_plugin_list_button.py
+-rw-rw-rw-   0        0        0      737 2019-08-15 16:57:23.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_slider_callback.py
+-rw-rw-rw-   0        0        0      859 2019-08-15 16:57:23.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_text_input_callback.py
+-rw-rw-rw-   0        0        0      525 2019-03-08 05:32:50.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_update_content.py
+-rw-rw-rw-   0        0        0     1059 2019-10-25 21:45:48.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_update_menu.py
+-rw-rw-rw-   0        0        0      555 2019-10-23 18:54:22.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_update_node.py
+-rw-rw-rw-   0        0        0     3236 2019-06-13 20:32:12.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_update_structures.py
+-rw-rw-rw-   0        0        0      421 2019-04-21 02:15:45.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_update_structures_deep_done.py
+-rw-rw-rw-   0        0        0     1190 2019-06-06 16:05:56.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_update_workspace.py
+-rw-rw-rw-   0        0        0      781 2019-05-23 18:17:50.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_upload_cryo_em.py
+-rw-rw-rw-   0        0        0      406 2019-05-23 18:17:50.000000 nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_upload_cryo_em_done.py
+-rw-rw-rw-   0        0        0     8383 2019-09-26 17:02:56.000000 nanome-0.9.0/nanome/_internal/_network/_data.py
+-rw-rw-rw-   0        0        0     3314 2019-08-15 16:57:23.000000 nanome-0.9.0/nanome/_internal/_network/_net_instance.py
+-rw-rw-rw-   0        0        0     2739 2019-08-15 16:57:23.000000 nanome-0.9.0/nanome/_internal/_network/_packet.py
+-rw-rw-rw-   0        0        0     3206 2019-09-26 17:02:56.000000 nanome-0.9.0/nanome/_internal/_network/_process_network.py
+drwxrwxrwx   0        0        0        0 2019-11-06 18:07:51.000000 nanome-0.9.0/nanome/_internal/_network/_serialization/
+-rw-rw-rw-   0        0        0      132 2019-02-22 07:08:10.000000 nanome-0.9.0/nanome/_internal/_network/_serialization/__init__.py
+-rw-rw-rw-   0        0        0     8389 2019-09-26 17:02:56.000000 nanome-0.9.0/nanome/_internal/_network/_serialization/_context.py
+-rw-rw-rw-   0        0        0    13149 2019-10-23 18:54:22.000000 nanome-0.9.0/nanome/_internal/_network/_serialization/_serializer.py
+-rw-rw-rw-   0        0        0     2432 2019-09-26 17:02:56.000000 nanome-0.9.0/nanome/_internal/_network/_session.py
+-rw-rw-rw-   0        0        0    10320 2019-11-05 21:37:41.000000 nanome-0.9.0/nanome/_internal/_plugin.py
+-rw-rw-rw-   0        0        0     2496 2019-11-05 21:37:41.000000 nanome-0.9.0/nanome/_internal/_plugin_instance.py
+drwxrwxrwx   0        0        0        0 2019-11-06 18:07:51.000000 nanome-0.9.0/nanome/_internal/_process/
+-rw-rw-rw-   0        0        0      237 2019-08-15 16:57:23.000000 nanome-0.9.0/nanome/_internal/_process/__init__.py
+-rw-rw-rw-   0        0        0     3774 2019-11-05 21:37:41.000000 nanome-0.9.0/nanome/_internal/_process/_bonding.py
+-rw-rw-rw-   0        0        0     5731 2019-11-05 21:37:41.000000 nanome-0.9.0/nanome/_internal/_process/_dssp.py
+drwxrwxrwx   0        0        0        0 2019-11-06 18:07:51.000000 nanome-0.9.0/nanome/_internal/_process/_external/
+drwxrwxrwx   0        0        0        0 2019-11-06 18:07:51.000000 nanome-0.9.0/nanome/_internal/_process/_external/_dssp/
+-rwxrwxrwx   0        0        0  1223168 2019-08-15 16:57:23.000000 nanome-0.9.0/nanome/_internal/_process/_external/_dssp/dssp-3.0.0-win32.exe
+-rw-rw-rw-   0        0        0  4079000 2019-08-15 16:57:23.000000 nanome-0.9.0/nanome/_internal/_process/_external/_dssp/dssp-linux
+-rw-rw-rw-   0        0        0      917 2019-08-15 16:57:23.000000 nanome-0.9.0/nanome/_internal/_process/_process_entry.py
+-rw-rw-rw-   0        0        0     4554 2019-08-15 16:57:23.000000 nanome-0.9.0/nanome/_internal/_process/_process_manager.py
+-rw-rw-rw-   0        0        0     1895 2019-09-12 17:08:22.000000 nanome-0.9.0/nanome/_internal/_process/_process_manager_instance.py
+drwxrwxrwx   0        0        0        0 2019-11-06 18:07:51.000000 nanome-0.9.0/nanome/_internal/_structure/
+-rw-rw-rw-   0        0        0      334 2019-10-16 22:16:06.000000 nanome-0.9.0/nanome/_internal/_structure/__init__.py
+-rw-rw-rw-   0        0        0     5666 2019-11-05 21:37:41.000000 nanome-0.9.0/nanome/_internal/_structure/_atom.py
+-rw-rw-rw-   0        0        0      122 2019-09-12 17:08:22.000000 nanome-0.9.0/nanome/_internal/_structure/_base.py
+-rw-rw-rw-   0        0        0     4222 2019-11-05 21:37:42.000000 nanome-0.9.0/nanome/_internal/_structure/_bond.py
+-rw-rw-rw-   0        0        0     1276 2019-11-05 21:37:42.000000 nanome-0.9.0/nanome/_internal/_structure/_chain.py
+-rw-rw-rw-   0        0        0     3484 2019-11-05 21:37:42.000000 nanome-0.9.0/nanome/_internal/_structure/_complex.py
+drwxrwxrwx   0        0        0        0 2019-11-06 18:07:51.000000 nanome-0.9.0/nanome/_internal/_structure/_helpers/
+-rw-rw-rw-   0        0        0       52 2019-10-16 22:16:07.000000 nanome-0.9.0/nanome/_internal/_structure/_helpers/__init__.py
+-rw-rw-rw-   0        0        0     9178 2019-11-06 18:06:18.000000 nanome-0.9.0/nanome/_internal/_structure/_helpers/_conformer_helper.py
+-rw-rw-rw-   0        0        0     3635 2019-11-05 21:37:42.000000 nanome-0.9.0/nanome/_internal/_structure/_helpers/_copy.py
+drwxrwxrwx   0        0        0        0 2019-11-06 18:07:51.000000 nanome-0.9.0/nanome/_internal/_structure/_io/
+-rw-rw-rw-   0        0        0       77 2019-02-22 07:08:10.000000 nanome-0.9.0/nanome/_internal/_structure/_io/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-06 18:07:51.000000 nanome-0.9.0/nanome/_internal/_structure/_io/_mmcif/
+-rw-rw-rw-   0        0        0      108 2019-06-06 16:05:56.000000 nanome-0.9.0/nanome/_internal/_structure/_io/_mmcif/__init__.py
+-rw-rw-rw-   0        0        0     1130 2019-06-13 20:32:12.000000 nanome-0.9.0/nanome/_internal/_structure/_io/_mmcif/content.py
+-rw-rw-rw-   0        0        0    16719 2019-06-06 16:05:56.000000 nanome-0.9.0/nanome/_internal/_structure/_io/_mmcif/parse.py
+-rw-rw-rw-   0        0        0     8281 2019-10-16 22:16:07.000000 nanome-0.9.0/nanome/_internal/_structure/_io/_mmcif/save.py
+-rw-rw-rw-   0        0        0     4899 2019-11-05 21:37:42.000000 nanome-0.9.0/nanome/_internal/_structure/_io/_mmcif/structure.py
+drwxrwxrwx   0        0        0        0 2019-11-06 18:07:51.000000 nanome-0.9.0/nanome/_internal/_structure/_io/_pdb/
+-rw-rw-rw-   0        0        0      108 2019-06-06 16:05:56.000000 nanome-0.9.0/nanome/_internal/_structure/_io/_pdb/__init__.py
+-rw-rw-rw-   0        0        0     3331 2019-03-08 05:32:50.000000 nanome-0.9.0/nanome/_internal/_structure/_io/_pdb/content.py
+-rw-rw-rw-   0        0        0    12662 2019-09-12 17:08:22.000000 nanome-0.9.0/nanome/_internal/_structure/_io/_pdb/parse.py
+-rw-rw-rw-   0        0        0     6143 2019-10-16 22:16:07.000000 nanome-0.9.0/nanome/_internal/_structure/_io/_pdb/save.py
+-rw-rw-rw-   0        0        0     2853 2019-11-05 21:37:42.000000 nanome-0.9.0/nanome/_internal/_structure/_io/_pdb/structure.py
+drwxrwxrwx   0        0        0        0 2019-11-06 18:07:52.000000 nanome-0.9.0/nanome/_internal/_structure/_io/_sdf/
+-rw-rw-rw-   0        0        0      108 2019-06-06 16:05:56.000000 nanome-0.9.0/nanome/_internal/_structure/_io/_sdf/__init__.py
+-rw-rw-rw-   0        0        0      814 2019-03-08 05:32:50.000000 nanome-0.9.0/nanome/_internal/_structure/_io/_sdf/content.py
+-rw-rw-rw-   0        0        0     6103 2019-06-06 16:05:56.000000 nanome-0.9.0/nanome/_internal/_structure/_io/_sdf/parse.py
+-rw-rw-rw-   0        0        0     5346 2019-10-16 22:16:07.000000 nanome-0.9.0/nanome/_internal/_structure/_io/_sdf/save.py
+-rw-rw-rw-   0        0        0     1603 2019-11-05 21:37:42.000000 nanome-0.9.0/nanome/_internal/_structure/_io/_sdf/structure.py
+-rw-rw-rw-   0        0        0     5044 2019-11-05 21:37:42.000000 nanome-0.9.0/nanome/_internal/_structure/_molecule.py
+-rw-rw-rw-   0        0        0     2964 2019-11-05 21:37:42.000000 nanome-0.9.0/nanome/_internal/_structure/_residue.py
+drwxrwxrwx   0        0        0        0 2019-11-06 18:07:52.000000 nanome-0.9.0/nanome/_internal/_structure/_serialization/
+-rw-rw-rw-   0        0        0      411 2019-04-21 02:15:45.000000 nanome-0.9.0/nanome/_internal/_structure/_serialization/__init__.py
+-rw-rw-rw-   0        0        0     4750 2019-10-16 22:16:07.000000 nanome-0.9.0/nanome/_internal/_structure/_serialization/_atom_serializer.py
+-rw-rw-rw-   0        0        0      895 2019-06-20 19:01:39.000000 nanome-0.9.0/nanome/_internal/_structure/_serialization/_atom_serializer_id.py
+-rw-rw-rw-   0        0        0     2477 2019-10-16 22:16:07.000000 nanome-0.9.0/nanome/_internal/_structure/_serialization/_bond_serializer.py
+-rw-rw-rw-   0        0        0     1231 2019-09-12 17:08:22.000000 nanome-0.9.0/nanome/_internal/_structure/_serialization/_chain_serializer.py
+-rw-rw-rw-   0        0        0     3689 2019-09-12 17:08:22.000000 nanome-0.9.0/nanome/_internal/_structure/_serialization/_complex_serializer.py
+-rw-rw-rw-   0        0        0     3039 2019-09-12 17:08:22.000000 nanome-0.9.0/nanome/_internal/_structure/_serialization/_molecule_serializer.py
+-rw-rw-rw-   0        0        0     2973 2019-09-12 17:08:22.000000 nanome-0.9.0/nanome/_internal/_structure/_serialization/_residue_serializer.py
+-rw-rw-rw-   0        0        0     1341 2019-06-13 20:32:12.000000 nanome-0.9.0/nanome/_internal/_structure/_serialization/_workspace_serializer.py
+-rw-rw-rw-   0        0        0     1258 2019-06-13 20:32:12.000000 nanome-0.9.0/nanome/_internal/_structure/_workspace.py
+drwxrwxrwx   0        0        0        0 2019-11-06 18:07:52.000000 nanome-0.9.0/nanome/_internal/_ui/
+-rw-rw-rw-   0        0        0      433 2019-04-21 02:15:45.000000 nanome-0.9.0/nanome/_internal/_ui/__init__.py
+-rw-rw-rw-   0        0        0     4823 2019-09-26 17:02:56.000000 nanome-0.9.0/nanome/_internal/_ui/_button.py
+-rw-rw-rw-   0        0        0     1447 2019-05-26 21:55:20.000000 nanome-0.9.0/nanome/_internal/_ui/_image.py
+drwxrwxrwx   0        0        0        0 2019-11-06 18:07:52.000000 nanome-0.9.0/nanome/_internal/_ui/_io/
+-rw-rw-rw-   0        0        0      304 2019-04-21 02:15:45.000000 nanome-0.9.0/nanome/_internal/_ui/_io/__init__.py
+-rw-rw-rw-   0        0        0     6256 2019-10-16 22:16:07.000000 nanome-0.9.0/nanome/_internal/_ui/_io/_button_json.py
+-rw-rw-rw-   0        0        0      644 2019-05-26 21:55:20.000000 nanome-0.9.0/nanome/_internal/_ui/_io/_image_json.py
+-rw-rw-rw-   0        0        0     1724 2019-05-26 21:55:20.000000 nanome-0.9.0/nanome/_internal/_ui/_io/_label_json.py
+-rw-rw-rw-   0        0        0     2161 2019-07-01 20:09:33.000000 nanome-0.9.0/nanome/_internal/_ui/_io/_layout_node_json.py
+-rw-rw-rw-   0        0        0      702 2019-04-21 02:15:45.000000 nanome-0.9.0/nanome/_internal/_ui/_io/_loading_bar_json.py
+-rw-rw-rw-   0        0        0      721 2019-04-21 02:15:45.000000 nanome-0.9.0/nanome/_internal/_ui/_io/_menu_json.py
+-rw-rw-rw-   0        0        0      349 2019-02-22 07:08:10.000000 nanome-0.9.0/nanome/_internal/_ui/_io/_mesh_json.py
+-rw-rw-rw-   0        0        0      526 2019-02-22 07:08:10.000000 nanome-0.9.0/nanome/_internal/_ui/_io/_slider_json.py
+-rw-rw-rw-   0        0        0      589 2019-02-22 07:08:10.000000 nanome-0.9.0/nanome/_internal/_ui/_io/_text_input_json.py
+-rw-rw-rw-   0        0        0     2473 2019-04-21 02:15:45.000000 nanome-0.9.0/nanome/_internal/_ui/_io/_ui_base_json.py
+-rw-rw-rw-   0        0        0      696 2019-04-21 02:15:45.000000 nanome-0.9.0/nanome/_internal/_ui/_io/_ui_list_json.py
+-rw-rw-rw-   0        0        0     1478 2019-05-26 21:55:20.000000 nanome-0.9.0/nanome/_internal/_ui/_label.py
+-rw-rw-rw-   0        0        0     4038 2019-10-23 18:54:22.000000 nanome-0.9.0/nanome/_internal/_ui/_layout_node.py
+-rw-rw-rw-   0        0        0      573 2019-04-21 02:15:45.000000 nanome-0.9.0/nanome/_internal/_ui/_loading_bar.py
+-rw-rw-rw-   0        0        0     1461 2019-10-25 21:45:48.000000 nanome-0.9.0/nanome/_internal/_ui/_menu.py
+-rw-rw-rw-   0        0        0      403 2019-03-08 05:32:50.000000 nanome-0.9.0/nanome/_internal/_ui/_mesh.py
+drwxrwxrwx   0        0        0        0 2019-11-06 18:07:52.000000 nanome-0.9.0/nanome/_internal/_ui/_serialization/
+-rw-rw-rw-   0        0        0      664 2019-04-21 02:15:45.000000 nanome-0.9.0/nanome/_internal/_ui/_serialization/__init__.py
+-rw-rw-rw-   0        0        0     7212 2019-09-26 17:28:03.000000 nanome-0.9.0/nanome/_internal/_ui/_serialization/_button_serializer.py
+-rw-rw-rw-   0        0        0     1838 2019-09-26 17:02:56.000000 nanome-0.9.0/nanome/_internal/_ui/_serialization/_image_serializer.py
+-rw-rw-rw-   0        0        0     2427 2019-08-15 16:57:23.000000 nanome-0.9.0/nanome/_internal/_ui/_serialization/_label_serializer.py
+-rw-rw-rw-   0        0        0     2728 2019-08-15 16:57:23.000000 nanome-0.9.0/nanome/_internal/_ui/_serialization/_layout_node_serializer.py
+-rw-rw-rw-   0        0        0     2460 2019-07-01 20:21:41.000000 nanome-0.9.0/nanome/_internal/_ui/_serialization/_layout_node_serializer_deep.py
+-rw-rw-rw-   0        0        0     1516 2019-08-15 16:57:23.000000 nanome-0.9.0/nanome/_internal/_ui/_serialization/_loading_bar_serializer.py
+-rw-rw-rw-   0        0        0     1198 2019-06-13 20:32:12.000000 nanome-0.9.0/nanome/_internal/_ui/_serialization/_menu_serializer.py
+-rw-rw-rw-   0        0        0     1145 2019-08-15 16:57:23.000000 nanome-0.9.0/nanome/_internal/_ui/_serialization/_mesh_serializer.py
+-rw-rw-rw-   0        0        0     1280 2019-08-15 16:57:23.000000 nanome-0.9.0/nanome/_internal/_ui/_serialization/_slider_serializer.py
+-rw-rw-rw-   0        0        0     1503 2019-08-15 16:57:23.000000 nanome-0.9.0/nanome/_internal/_ui/_serialization/_text_input_serializer.py
+-rw-rw-rw-   0        0        0     1631 2019-04-21 02:15:45.000000 nanome-0.9.0/nanome/_internal/_ui/_serialization/_ui_base_serializer.py
+-rw-rw-rw-   0        0        0     1691 2019-08-15 16:57:23.000000 nanome-0.9.0/nanome/_internal/_ui/_serialization/_ui_list_serializer.py
+-rw-rw-rw-   0        0        0      808 2019-03-08 05:32:50.000000 nanome-0.9.0/nanome/_internal/_ui/_slider.py
+-rw-rw-rw-   0        0        0      863 2019-03-08 05:32:50.000000 nanome-0.9.0/nanome/_internal/_ui/_text_input.py
+-rw-rw-rw-   0        0        0      437 2019-04-21 02:15:45.000000 nanome-0.9.0/nanome/_internal/_ui/_ui_base.py
+-rw-rw-rw-   0        0        0      757 2019-03-08 05:32:50.000000 nanome-0.9.0/nanome/_internal/_ui/_ui_list.py
+drwxrwxrwx   0        0        0        0 2019-11-06 18:07:52.000000 nanome-0.9.0/nanome/_internal/_util/
+-rw-rw-rw-   0        0        0       53 2019-02-22 07:08:10.000000 nanome-0.9.0/nanome/_internal/_util/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-06 18:07:52.000000 nanome-0.9.0/nanome/_internal/_util/_serializers/
+-rw-rw-rw-   0        0        0      820 2019-08-29 18:22:25.000000 nanome-0.9.0/nanome/_internal/_util/_serializers/__init__.py
+-rw-rw-rw-   0        0        0     1079 2019-03-08 05:32:50.000000 nanome-0.9.0/nanome/_internal/_util/_serializers/_array_serializer.py
+-rw-rw-rw-   0        0        0      407 2019-03-08 05:32:50.000000 nanome-0.9.0/nanome/_internal/_util/_serializers/_bool_serializer.py
+-rw-rw-rw-   0        0        0      428 2019-03-08 05:32:50.000000 nanome-0.9.0/nanome/_internal/_util/_serializers/_byte_serializer.py
+-rw-rw-rw-   0        0        0      465 2019-03-08 05:32:50.000000 nanome-0.9.0/nanome/_internal/_util/_serializers/_color_serializer.py
+-rw-rw-rw-   0        0        0     1126 2019-03-08 05:32:50.000000 nanome-0.9.0/nanome/_internal/_util/_serializers/_dictionary_serializer.py
+-rw-rw-rw-   0        0        0      663 2019-03-08 05:32:50.000000 nanome-0.9.0/nanome/_internal/_util/_serializers/_directory_entry_serializer.py
+-rw-rw-rw-   0        0        0      686 2019-03-08 05:32:50.000000 nanome-0.9.0/nanome/_internal/_util/_serializers/_file_data_serializer.py
+-rw-rw-rw-   0        0        0      854 2019-03-08 05:32:50.000000 nanome-0.9.0/nanome/_internal/_util/_serializers/_file_save_data_serializer.py
+-rw-rw-rw-   0        0        0      403 2019-03-08 05:32:50.000000 nanome-0.9.0/nanome/_internal/_util/_serializers/_int_serializer.py
+-rw-rw-rw-   0        0        0      415 2019-03-08 05:32:50.000000 nanome-0.9.0/nanome/_internal/_util/_serializers/_long_serializer.py
+-rw-rw-rw-   0        0        0      778 2019-05-23 18:17:50.000000 nanome-0.9.0/nanome/_internal/_util/_serializers/_quaternion_serializer.py
+-rw-rw-rw-   0        0        0      810 2019-03-08 05:32:50.000000 nanome-0.9.0/nanome/_internal/_util/_serializers/_string_serializer.py
+-rw-rw-rw-   0        0        0     1232 2019-03-08 05:32:50.000000 nanome-0.9.0/nanome/_internal/_util/_serializers/_tuple_serializer.py
+-rw-rw-rw-   0        0        0     1212 2019-05-23 18:17:50.000000 nanome-0.9.0/nanome/_internal/_util/_serializers/_type_serializer.py
+-rw-rw-rw-   0        0        0      626 2019-03-08 05:32:50.000000 nanome-0.9.0/nanome/_internal/_util/_serializers/_vector3_serializer.py
+drwxrwxrwx   0        0        0        0 2019-11-06 18:07:52.000000 nanome-0.9.0/nanome/_internal/_volumetric/
+-rw-rw-rw-   0        0        0       98 2019-05-23 18:17:50.000000 nanome-0.9.0/nanome/_internal/_volumetric/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-06 18:07:52.000000 nanome-0.9.0/nanome/_internal/_volumetric/_io/
+-rw-rw-rw-   0        0        0       21 2019-05-23 18:17:50.000000 nanome-0.9.0/nanome/_internal/_volumetric/_io/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-06 18:07:52.000000 nanome-0.9.0/nanome/_internal/_volumetric/_io/_em_map/
+-rw-rw-rw-   0        0        0       20 2019-05-23 18:17:50.000000 nanome-0.9.0/nanome/_internal/_volumetric/_io/_em_map/__init__.py
+-rw-rw-rw-   0        0        0     2600 2019-05-23 18:17:50.000000 nanome-0.9.0/nanome/_internal/_volumetric/_io/_em_map/_parse.py
+drwxrwxrwx   0        0        0        0 2019-11-06 18:07:52.000000 nanome-0.9.0/nanome/_internal/_volumetric/_serialization/
+-rw-rw-rw-   0        0        0       58 2019-05-23 18:17:50.000000 nanome-0.9.0/nanome/_internal/_volumetric/_serialization/__init__.py
+-rw-rw-rw-   0        0        0     1402 2019-06-06 16:05:56.000000 nanome-0.9.0/nanome/_internal/_volumetric/_serialization/_volume_data_serializer.py
+-rw-rw-rw-   0        0        0      613 2019-05-23 18:17:50.000000 nanome-0.9.0/nanome/_internal/_volumetric/_volume_data.py
+drwxrwxrwx   0        0        0        0 2019-11-06 18:07:52.000000 nanome-0.9.0/nanome/api/
+-rw-rw-rw-   0        0        0      211 2019-09-26 17:02:56.000000 nanome-0.9.0/nanome/api/__init__.py
+drwxrwxrwx   0        0        0        0 2019-11-06 18:07:52.000000 nanome-0.9.0/nanome/api/macro/
+-rw-rw-rw-   0        0        0       24 2019-08-15 16:57:23.000000 nanome-0.9.0/nanome/api/macro/__init__.py
+-rw-rw-rw-   0        0        0     1120 2019-08-15 16:57:23.000000 nanome-0.9.0/nanome/api/macro/macro.py
+-rw-rw-rw-   0        0        0     3314 2019-11-05 21:37:42.000000 nanome-0.9.0/nanome/api/plugin.py
+-rw-rw-rw-   0        0        0    13991 2019-11-05 21:37:42.000000 nanome-0.9.0/nanome/api/plugin_instance.py
+drwxrwxrwx   0        0        0        0 2019-11-06 18:07:52.000000 nanome-0.9.0/nanome/api/streams/
+-rw-rw-rw-   0        0        0       43 2019-04-21 02:15:45.000000 nanome-0.9.0/nanome/api/streams/__init__.py
+-rw-rw-rw-   0        0        0     2802 2019-09-26 17:02:56.000000 nanome-0.9.0/nanome/api/streams/stream.py
+drwxrwxrwx   0        0        0        0 2019-11-06 18:07:52.000000 nanome-0.9.0/nanome/api/structure/
+-rw-rw-rw-   0        0        0      263 2019-05-23 18:17:50.000000 nanome-0.9.0/nanome/api/structure/__init__.py
+-rw-rw-rw-   0        0        0     8505 2019-10-16 22:16:07.000000 nanome-0.9.0/nanome/api/structure/atom.py
+-rw-rw-rw-   0        0        0      306 2019-05-23 18:17:50.000000 nanome-0.9.0/nanome/api/structure/base.py
+-rw-rw-rw-   0        0        0     2957 2019-10-16 22:16:07.000000 nanome-0.9.0/nanome/api/structure/bond.py
+-rw-rw-rw-   0        0        0     1773 2019-09-12 17:08:22.000000 nanome-0.9.0/nanome/api/structure/chain.py
+-rw-rw-rw-   0        0        0     8993 2019-10-16 22:16:07.000000 nanome-0.9.0/nanome/api/structure/complex.py
+drwxrwxrwx   0        0        0        0 2019-11-06 18:07:52.000000 nanome-0.9.0/nanome/api/structure/io/
+-rw-rw-rw-   0        0        0       54 2019-02-22 07:08:10.000000 nanome-0.9.0/nanome/api/structure/io/__init__.py
+-rw-rw-rw-   0        0        0     4396 2019-06-13 20:32:12.000000 nanome-0.9.0/nanome/api/structure/io/complex_io.py
+-rw-rw-rw-   0        0        0       64 2019-03-08 05:32:50.000000 nanome-0.9.0/nanome/api/structure/io/molecule_io.py
+-rw-rw-rw-   0        0        0       65 2019-03-08 05:32:50.000000 nanome-0.9.0/nanome/api/structure/io/workspace_io.py
+-rw-rw-rw-   0        0        0     3418 2019-10-16 22:16:07.000000 nanome-0.9.0/nanome/api/structure/molecule.py
+-rw-rw-rw-   0        0        0     6469 2019-10-16 22:16:07.000000 nanome-0.9.0/nanome/api/structure/residue.py
+-rw-rw-rw-   0        0        0     1744 2019-06-13 20:32:12.000000 nanome-0.9.0/nanome/api/structure/workspace.py
+drwxrwxrwx   0        0        0        0 2019-11-06 18:07:52.000000 nanome-0.9.0/nanome/api/ui/
+-rw-rw-rw-   0        0        0      382 2019-04-21 02:15:45.000000 nanome-0.9.0/nanome/api/ui/__init__.py
+-rw-rw-rw-   0        0        0    10106 2019-09-26 17:02:56.000000 nanome-0.9.0/nanome/api/ui/button.py
+-rw-rw-rw-   0        0        0     1190 2019-08-15 16:57:23.000000 nanome-0.9.0/nanome/api/ui/image.py
+drwxrwxrwx   0        0        0        0 2019-11-06 18:07:52.000000 nanome-0.9.0/nanome/api/ui/io/
+-rw-rw-rw-   0        0        0       86 2019-05-23 18:17:50.000000 nanome-0.9.0/nanome/api/ui/io/__init__.py
+-rw-rw-rw-   0        0        0     1337 2019-04-21 02:15:45.000000 nanome-0.9.0/nanome/api/ui/io/layout_node_io.py
+-rw-rw-rw-   0        0        0     1394 2019-05-23 18:17:50.000000 nanome-0.9.0/nanome/api/ui/io/menu_io.py
+-rw-rw-rw-   0        0        0     3210 2019-09-12 17:08:22.000000 nanome-0.9.0/nanome/api/ui/label.py
+-rw-rw-rw-   0        0        0     7791 2019-07-01 20:09:33.000000 nanome-0.9.0/nanome/api/ui/layout_node.py
+-rw-rw-rw-   0        0        0     1074 2019-09-12 17:08:22.000000 nanome-0.9.0/nanome/api/ui/loading_bar.py
+-rw-rw-rw-   0        0        0     1877 2019-10-25 21:45:48.000000 nanome-0.9.0/nanome/api/ui/menu.py
+-rw-rw-rw-   0        0        0      487 2019-04-21 02:15:45.000000 nanome-0.9.0/nanome/api/ui/mesh.py
+-rw-rw-rw-   0        0        0     1445 2019-04-21 02:15:45.000000 nanome-0.9.0/nanome/api/ui/slider.py
+-rw-rw-rw-   0        0        0     1870 2019-09-12 17:08:22.000000 nanome-0.9.0/nanome/api/ui/text_input.py
+-rw-rw-rw-   0        0        0      216 2019-04-21 02:15:45.000000 nanome-0.9.0/nanome/api/ui/ui_base.py
+-rw-rw-rw-   0        0        0     1309 2019-04-21 02:15:45.000000 nanome-0.9.0/nanome/api/ui/ui_list.py
+drwxrwxrwx   0        0        0        0 2019-11-06 18:07:52.000000 nanome-0.9.0/nanome/api/user/
+-rw-rw-rw-   0        0        0       41 2019-09-26 17:02:56.000000 nanome-0.9.0/nanome/api/user/__init__.py
+-rw-rw-rw-   0        0        0      677 2019-09-26 17:02:56.000000 nanome-0.9.0/nanome/api/user/presenter_info.py
+-rw-rw-rw-   0        0        0     2961 2019-10-23 18:54:26.000000 nanome-0.9.0/nanome/setup_config.py
+drwxrwxrwx   0        0        0        0 2019-11-06 18:07:52.000000 nanome-0.9.0/nanome/util/
+-rw-rw-rw-   0        0        0      610 2019-11-06 18:06:18.000000 nanome-0.9.0/nanome/util/__init__.py
+-rw-rw-rw-   0        0        0      310 2019-03-08 05:32:50.000000 nanome-0.9.0/nanome/util/_logs_2.py
+-rw-rw-rw-   0        0        0      315 2019-03-08 05:32:51.000000 nanome-0.9.0/nanome/util/_logs_3.py
+-rw-rw-rw-   0        0        0     3185 2019-10-16 22:16:07.000000 nanome-0.9.0/nanome/util/color.py
+-rw-rw-rw-   0        0        0      509 2019-06-06 16:05:56.000000 nanome-0.9.0/nanome/util/complex_save_options.py
+-rw-rw-rw-   0        0        0     1656 2019-09-12 17:08:22.000000 nanome-0.9.0/nanome/util/config.py
+-rw-rw-rw-   0        0        0    37034 2019-11-06 18:06:18.000000 nanome-0.9.0/nanome/util/enum.py
+-rw-rw-rw-   0        0        0     1358 2019-11-06 18:06:19.000000 nanome-0.9.0/nanome/util/enums.py
+-rw-rw-rw-   0        0        0     1008 2019-03-08 05:32:51.000000 nanome-0.9.0/nanome/util/file.py
+-rw-rw-rw-   0        0        0      521 2019-03-08 05:32:51.000000 nanome-0.9.0/nanome/util/import_utils.py
+-rw-rw-rw-   0        0        0     2831 2019-06-13 20:32:12.000000 nanome-0.9.0/nanome/util/logs.py
+-rw-rw-rw-   0        0        0     5896 2019-05-23 18:17:50.000000 nanome-0.9.0/nanome/util/matrix.py
+-rw-rw-rw-   0        0        0     5444 2019-05-23 18:17:50.000000 nanome-0.9.0/nanome/util/octree.py
+-rw-rw-rw-   0        0        0     1622 2019-08-15 16:57:23.000000 nanome-0.9.0/nanome/util/process.py
+-rw-rw-rw-   0        0        0     3006 2019-10-16 22:16:07.000000 nanome-0.9.0/nanome/util/quaternion.py
+-rw-rw-rw-   0        0        0      212 2019-09-26 17:02:56.000000 nanome-0.9.0/nanome/util/stream.py
+-rw-rw-rw-   0        0        0      373 2019-11-05 21:37:42.000000 nanome-0.9.0/nanome/util/string_builder.py
+-rw-rw-rw-   0        0        0     1986 2019-10-16 22:16:07.000000 nanome-0.9.0/nanome/util/vector3.py
+drwxrwxrwx   0        0        0        0 2019-11-06 18:07:51.000000 nanome-0.9.0/nanome.egg-info/
+-rw-rw-rw-   0        0        0     1510 2019-11-06 18:07:50.000000 nanome-0.9.0/nanome.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    12279 2019-11-06 18:07:51.000000 nanome-0.9.0/nanome.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2019-11-06 18:07:50.000000 nanome-0.9.0/nanome.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2019-11-06 18:07:50.000000 nanome-0.9.0/nanome.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2019-11-06 18:07:50.000000 nanome-0.9.0/nanome.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      227 2019-11-06 18:07:52.000000 nanome-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1295 2019-11-06 18:07:49.000000 nanome-0.9.0/setup.py
```

### Comparing `nanome-0.8.3/PKG-INFO` & `nanome-0.9.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanome
-Version: 0.8.3
+Version: 0.9.0
 Summary: Python API for Nanome Plugins
 Home-page: https://github.com/nanome-ai/nanome
 Author: Nanome
 Author-email: hello@nanome.ai
 License: MIT
 Description: # Nanome
```

### Comparing `nanome-0.8.3/README.md` & `nanome-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_macro/_macro.py` & `nanome-0.9.0/nanome/_internal/_macro/_macro.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_macro/_serialization/_macro_serializer.py` & `nanome-0.9.0/nanome/_internal/_macro/_serialization/_macro_serializer.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_network/_commands/_callbacks/__init__.py` & `nanome-0.9.0/nanome/_internal/_network/_commands/_callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_network/_commands/_callbacks/_commands_enums.py` & `nanome-0.9.0/nanome/_internal/_network/_commands/_callbacks/_commands_enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,14 +82,15 @@
     #Control
     connect = auto()
     plugin_list_button_set = auto()
 
     #UI
     menu_update = auto()
     content_update = auto()
+    node_update = auto()
     notification_send = auto()
 
     #Structure
     structures_deep_update = auto()
     structures_shallow_update = auto()
     structures_zoom = auto()
     structures_center = auto()
```

### Comparing `nanome-0.8.3/nanome/_internal/_network/_commands/_callbacks/_create_stream_result.py` & `nanome-0.9.0/nanome/_internal/_network/_commands/_callbacks/_create_stream_result.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_network/_commands/_callbacks/_menu.py` & `nanome-0.9.0/nanome/_internal/_network/_commands/_callbacks/_menu.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_network/_commands/_callbacks/_ui_callbacks.py` & `nanome-0.9.0/nanome/_internal/_network/_commands/_callbacks/_ui_callbacks.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/__init__.py` & `nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 from ._set_plugin_list_button import _SetPluginListButton
 from ._menu_callback import _MenuCallback
 from ._button_callback import _ButtonCallback
 from ._slider_callback import _SliderCallback
 from ._text_input_callback import _TextInputCallback
 from ._image_callback import _ImageCallback
 from ._update_content import _UpdateContent
+from ._update_node import _UpdateNode
 from ._update_menu import _UpdateMenu
 from ._update_workspace import _UpdateWorkspace
 from ._position_structures import _PositionStructures
 from ._position_structures_done import _PositionStructuresDone
 from ._send_notification import _SendNotification
 
 from ._macro_commands import _RunMacro, _SaveMacro, _DeleteMacro, _GetMacros, _GetMacrosResponse, _StopMacro
```

### Comparing `nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_add_bonds.py` & `nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_add_bonds.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_add_dssp.py` & `nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_add_dssp.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_add_to_workspace.py` & `nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_add_to_workspace.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_button_callback.py` & `nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_button_callback.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_connect.py` & `nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_connect.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_create_stream.py` & `nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_create_stream.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_create_stream_result.py` & `nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_create_stream_result.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_directory_request.py` & `nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_directory_request.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_feed_stream.py` & `nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_feed_stream.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_file_request.py` & `nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_file_request.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_file_save.py` & `nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_file_save.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_get_presenter_info_response.py` & `nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_get_presenter_info_response.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_image_callback.py` & `nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_image_callback.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_macro_commands.py` & `nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_macro_commands.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_open_url.py` & `nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_open_url.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_position_structures.py` & `nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_position_structures.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_receive_complex_list.py` & `nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_receive_complex_list.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_receive_menu.py` & `nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_receive_menu.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_receive_workspace.py` & `nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_receive_workspace.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_request_complex_list.py` & `nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_request_complex_list.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_send_notification.py` & `nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_send_notification.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_set_plugin_list_button.py` & `nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_set_plugin_list_button.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_slider_callback.py` & `nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_slider_callback.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_text_input_callback.py` & `nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_text_input_callback.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_update_content.py` & `nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_update_content.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_update_menu.py` & `nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_update_menu.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,20 +7,22 @@
     def __init__(self):
         self.menu = _MenuSerializer()
         self.array = _ArraySerializer()
         self.layout = _LayoutNodeSerializer()
         self.content = _UIBaseSerializer()
 
     def version(self):
-        return 0
+        return 1
 
     def name(self):
         return "UpdateMenu"
 
     def serialize(self, version, value, context):
+        if version >= 1:
+            context.write_byte(value.index)
         context.write_using_serializer(self.menu, value)
         self.array.set_type(self.layout)
         context.write_using_serializer(self.array, value._get_all_nodes())
         self.array.set_type(self.content)
         context.write_using_serializer(self.array, value._get_all_content())
 
     def deserialize(self, version, context):
```

### Comparing `nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_update_structures.py` & `nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_update_structures.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_update_workspace.py` & `nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_update_workspace.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_network/_commands/_serialization/_upload_cryo_em.py` & `nanome-0.9.0/nanome/_internal/_network/_commands/_serialization/_upload_cryo_em.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_network/_data.py` & `nanome-0.9.0/nanome/_internal/_network/_data.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_network/_net_instance.py` & `nanome-0.9.0/nanome/_internal/_network/_net_instance.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_network/_packet.py` & `nanome-0.9.0/nanome/_internal/_network/_packet.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_network/_process_network.py` & `nanome-0.9.0/nanome/_internal/_network/_process_network.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_network/_serialization/_context.py` & `nanome-0.9.0/nanome/_internal/_network/_serialization/_context.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_network/_serialization/_serializer.py` & `nanome-0.9.0/nanome/_internal/_network/_serialization/_serializer.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,14 +154,15 @@
 
 #volume
 add_message(CommandCallbacks._Messages.upload_cryo_em, CommandSerializers._UploadCryoEM())
 
 #ui
 add_message(CommandCallbacks._Messages.menu_update, CommandSerializers._UpdateMenu())
 add_message(CommandCallbacks._Messages.content_update, CommandSerializers._UpdateContent())
+add_message(CommandCallbacks._Messages.node_update, CommandSerializers._UpdateNode())
 add_message(CommandCallbacks._Messages.notification_send, CommandSerializers._SendNotification())
 
 #file
 add_message(CommandCallbacks._Messages.directory_request, CommandSerializers._DirectoryRequest())
 add_message(CommandCallbacks._Messages.file_request, CommandSerializers._FileRequest())
 add_message(CommandCallbacks._Messages.file_save, CommandSerializers._FileSave())
 add_message(CommandCallbacks._Messages.plugin_list_button_set, CommandSerializers._SetPluginListButton())
```

### Comparing `nanome-0.8.3/nanome/_internal/_network/_session.py` & `nanome-0.9.0/nanome/_internal/_network/_session.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_plugin.py` & `nanome-0.9.0/nanome/_internal/_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 try_reconnection_time = 20.0
 keep_alive_time_interval = 3600.0
 
 __metaclass__ = type
 class _Plugin(object):
     __serializer = Serializer()
     _plugin_id = -1
+    _custom_data = None
 
     def __parse_args(self):
         Logs._set_verbose(False)
         for i in range(1, len(sys.argv)):
             if sys.argv[i] == "-h":
                 Logs.message("Usage:", sys.argv[1],"[-h] [-a ADDRESS] [-p PORT]")
                 Logs.message(" -h  display this help")
@@ -193,32 +194,32 @@
             session.plugin_process.join()
         sys.exit(0)
 
     def __on_client_connection(self, session_id, version_table):
         main_conn_net, process_conn_net = Pipe()
         main_conn_proc, process_conn_proc = Pipe()
         session = Network._Session(session_id, self._network, self._process_manager, main_conn_net, main_conn_proc)
-        process = Process(target=_Plugin._launch_plugin, args=(self._plugin_class, session_id, process_conn_net, process_conn_proc, _Plugin.__serializer, _Plugin._plugin_id, version_table, _TypeSerializer.get_version_table(), Logs._is_verbose()))
+        process = Process(target=_Plugin._launch_plugin, args=(self._plugin_class, session_id, process_conn_net, process_conn_proc, _Plugin.__serializer, _Plugin._plugin_id, version_table, _TypeSerializer.get_version_table(), Logs._is_verbose(), _Plugin._custom_data))
         process.start()
         session.plugin_process = process
         self._sessions[session_id] = session
         Logs.debug("Registered new session:", session_id)
 
     @staticmethod
     def _is_process():
         return current_process().name != 'MainProcess'
 
     @classmethod
-    def _launch_plugin_profile(cls, plugin_class, session_id, pipe_net, pipe_proc, serializer, plugin_id, version_table, original_version_table, verbose):
-        cProfile.runctx('_Plugin._launch_plugin(plugin_class, session_id, pipe_net, pipe_proc, serializer, plugin_id, version_table, original_version_table, verbose)', globals(), locals(), 'profile.out')
+    def _launch_plugin_profile(cls, plugin_class, session_id, pipe_net, pipe_proc, serializer, plugin_id, version_table, original_version_table, verbose, custom_data):
+        cProfile.runctx('_Plugin._launch_plugin(plugin_class, session_id, pipe_net, pipe_proc, serializer, plugin_id, version_table, original_version_table, verbose, custom_data)', globals(), locals(), 'profile.out')
 
     @classmethod
-    def _launch_plugin(cls, plugin_class, session_id, pipe_net, pipe_proc, serializer, plugin_id, version_table, original_version_table, verbose):
+    def _launch_plugin(cls, plugin_class, session_id, pipe_net, pipe_proc, serializer, plugin_id, version_table, original_version_table, verbose, custom_data):
         plugin = plugin_class()
-        _PluginInstance.__init__(plugin, session_id, pipe_net, pipe_proc, serializer, plugin_id, version_table, original_version_table, verbose)
+        _PluginInstance.__init__(plugin, session_id, pipe_net, pipe_proc, serializer, plugin_id, version_table, original_version_table, verbose, custom_data)
         Logs.debug("Starting plugin")
         plugin._run()
 
     def __init__(self, name, description, category = "", has_advanced = False):
         self._sessions = dict()
         self._description = {
             'name': name,
```

### Comparing `nanome-0.8.3/nanome/_internal/_plugin_instance.py` & `nanome-0.9.0/nanome/_internal/_plugin_instance.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,18 +54,19 @@
         except:
             Logs.error(traceback.format_exc())
             self._on_stop()
             self._process_manager._close()
             self._network._close()
             return
 
-    def __init__(self, session_id, net_pipe, proc_pipe, serializer, plugin_id, version_table, original_version_table, verbose):
+    def __init__(self, session_id, net_pipe, proc_pipe, serializer, plugin_id, version_table, original_version_table, verbose, custom_data):
         Logs._set_verbose(verbose)
 
         self._network = _ProcessNetwork(self, session_id, net_pipe, serializer, plugin_id, version_table)
         self._process_manager = _ProcessManagerInstance(proc_pipe)
         Logs.debug("Plugin constructed for session", session_id)
         self._network._send(_Messages.connect, [_Packet._compression_type(), original_version_table])
         self._run_text = "Run"
         self._run_usable = True
         self._advanced_settings_text = "Advanced Settings"
-        self._advanced_settings_usable = True
+        self._advanced_settings_usable = True
+        self._custom_data = custom_data
```

### Comparing `nanome-0.8.3/nanome/_internal/_process/_bonding.py` & `nanome-0.9.0/nanome/_internal/_process/_bonding.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
                 self.__done()
                 return
             complex = self.__complexes[self.__complex_idx]
             self.__molecule_idx = 0
         molecule = complex._molecules[self.__molecule_idx]
 
         self.__saved_complex._molecules.clear()
-        self.__saved_complex._molecules.append(molecule)
+        self.__saved_complex._add_molecule(molecule)
         _pdb.to_file(self.__input.name, complex)
 
         self.__proc.start()
 
     def __on_error(self, msg):
         if not "molecule converted" in msg:
             Logs.warning("[Bond Generation]", msg)
@@ -87,15 +87,15 @@
                 if serial1 in atom_by_serial and serial2 in atom_by_serial:
                     atom1, residue1 = atom_by_serial[serial1]
                     atom2, residue2 = atom_by_serial[serial2]
                     new_bond = _Bond._create()
                     new_bond._kind = bond._kind
                     new_bond._atom1 = atom1
                     new_bond._atom2 = atom2
-                    residue1._bonds.append(new_bond)
+                    residue1._add_bond(new_bond)
 
     def __done(self):
         self.__input.close()
         self.__output.close()
         os.remove(self.__input.name)
         os.remove(self.__output.name)
         self.__callback(self.__complexes)
```

### Comparing `nanome-0.8.3/nanome/_internal/_process/_dssp.py` & `nanome-0.9.0/nanome/_internal/_process/_dssp.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
                 self.__done()
                 return
             complex = self.__complexes[self.__complex_idx]
             self.__molecule_idx = 0
         molecule = complex._molecules[self.__molecule_idx]
 
         self.__saved_complex._molecules.clear()
-        self.__saved_complex._molecules.append(molecule)
+        self.__saved_complex._add_molecule(molecule)
         _pdb.to_file(self.__input.name, complex)
 
         self.__proc.start()
 
     def __on_error(self, msg):
         Logs.warning("[DSSP]", msg)
```

### Comparing `nanome-0.8.3/nanome/_internal/_process/_external/_dssp/dssp-3.0.0-win32.exe` & `nanome-0.9.0/nanome/_internal/_process/_external/_dssp/dssp-3.0.0-win32.exe`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_process/_external/_dssp/dssp-linux` & `nanome-0.9.0/nanome/_internal/_process/_external/_dssp/dssp-linux`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_process/_process_entry.py` & `nanome-0.9.0/nanome/_internal/_process/_process_entry.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_process/_process_manager.py` & `nanome-0.9.0/nanome/_internal/_process/_process_manager.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_process/_process_manager_instance.py` & `nanome-0.9.0/nanome/_internal/_process/_process_manager_instance.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_structure/_atom.py` & `nanome-0.9.0/nanome/_internal/_structure/_atom.py`

 * *Files 4% similar despite different names*

```diff
@@ -135,15 +135,16 @@
             index = src
         value = self._in_conformer[src]
         self._in_conformer.insert(index, value)
         value = self._positions[src].get_copy()
         self._positions.insert(index, value)
     #endregion
 
-    def _shallow_copy(self):
+    #copies the structure. If conformer_number is not None it will only copy that conformer's data..
+    def _shallow_copy(self, conformer_number = None):
         atom = _Atom._create()
         atom._symbol = self._symbol
         atom._serial = self._serial
         atom._name = self._name
         atom._is_het = self._is_het
         #No API
         atom._occupancy = self._occupancy
@@ -164,10 +165,14 @@
         atom._surface_opacity = self._surface_opacity
         #No API
         atom._hydrogened = self._hydrogened
         atom._watered = self._watered
         atom._het_atomed = self._het_atomed
         atom._het_surfaced = self._het_surfaced
         #conformer
-        atom._positions = [position.get_copy() for position in self._positions]
-        atom._in_conformer = list(self._in_conformer)
+        if conformer_number == None:
+            atom._positions = [position.get_copy() for position in self._positions]
+            atom._in_conformer = list(self._in_conformer)
+        else:
+            atom._position = self._positions[conformer_number]
+            #atom._exists = self._in_conformer[conformer_number]
         return atom
```

### Comparing `nanome-0.8.3/nanome/_internal/_structure/_bond.py` & `nanome-0.9.0/nanome/_internal/_structure/_bond.py`

 * *Files 16% similar despite different names*

```diff
@@ -136,12 +136,17 @@
         return self._in_conformer[self._current_conformer]
     
     @_exists.setter
     def _exists(self, value):
         self._in_conformer[self._current_conformer] = value
     #endregion
 
-    def _shallow_copy(self):
+    #copies the structure. If conformer_number is not None it will only copy that conformer's data.
+    def _shallow_copy(self, conformer_number = None):
         bond = _Bond._create()
-        bond._in_conformer = list(self._in_conformer)
-        bond._kinds = list(self._kinds)
+        if conformer_number == None:
+            bond._in_conformer = list(self._in_conformer)
+            bond._kinds = list(self._kinds)
+        else:
+            bond._kind = self._kinds[conformer_number]
+            # bond._exists = self._in_conformer[conformer_number]
         return bond
```

### Comparing `nanome-0.8.3/nanome/_internal/_structure/_chain.py` & `nanome-0.9.0/nanome/_internal/_structure/_chain.py`

 * *Files 24% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     def _complex(self):
         if self._parent:
             return self._parent._complex
         else:
             return None
     #endregion
 
-    def _shallow_copy(self):
+        #copies the structure. If conformer_number is not None it will only copy that conformer's data
+    def _shallow_copy(self, conformer_number = None):
         chain = _Chain._create()
         chain._name = self._name
         return chain
 
-    def _deep_copy(self):
-        return _helpers._copy._deep_copy_chain(self)
+    def _deep_copy(self, conformer_number = None):
+        return _helpers._copy._deep_copy_chain(self, conformer_number)
```

### Comparing `nanome-0.8.3/nanome/_internal/_structure/_complex.py` & `nanome-0.9.0/nanome/_internal/_structure/_complex.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,11 +96,13 @@
         complex._rotation = self._rotation.get_copy()
         return complex
 
     def _deep_copy(self):
         return _helpers._copy._deep_copy_complex(self)
     
     def _convert_to_conformers(self, force_conformers = None):
-        return _helpers._conformer_helper.convert_to_conformers(self, None)
+        result = _helpers._conformer_helper.convert_to_conformers(self, None)
+        return result
 
     def _convert_to_frames(self):
-        return _helpers._conformer_helper.convert_to_frames(self)
+        result = _helpers._conformer_helper.convert_to_frames(self)
+        return result
```

### Comparing `nanome-0.8.3/nanome/_internal/_structure/_helpers/_conformer_helper.py` & `nanome-0.9.0/nanome/_internal/_structure/_helpers/_conformer_helper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,83 +1,21 @@
 import hashlib, copy
 from nanome.util import StringBuilder, Vector3, enums
 s_ConformersDisabled = False #Nanome.Core.Config.getBool("mol-conformers-disabled", "false")
 s_ConformersAlways = False #Nanome.Core.Config.getBool("mol-conformers-always", "false")
 
-def _delete_atoms(atoms):
-    for atom in atoms:
-        atom.name == "DELETED"
-        try:
-            atom._residue._remove_atom(atom)
-        except ValueError:
-            pass
-        _delete_bonds(atom._bonds)
-    del atoms[:]
-
-def _delete_bonds(bonds):
-    for bond in bonds:
-        bond._atom1 = None
-        bond._atom2 = None
-        try:
-            bond._residue.remove_bond(bond)
-        except ValueError:
-            pass
-    del bonds[:]
-
-def _delete_residues(residues):
-    for residue in residues:
-        residue._chain._remove_residue(residue)
-    del residues[:]
-
-def _delete_chains(chains):
-    for chain in chains:
-        chain._molecule._remove_chain(chain)
-    del chains[:]
-
-#disabled hashing until I can find a fast algorithm
-def _get_hash_code(str):
-    return str #int(hashlib.sha256(str.encode('utf-8')).hexdigest(), 16)
+def _get_hash_code(string):
+    return hash(string)
 
 def convert_to_frames(complex): #Data.Complex -> Data.Complex
-    deleted_atoms = []
-    deleted_bonds = []
-    deleted_residues = []
-    deleted_chains = []
     new_complex = complex._shallow_copy()
     for molecule in complex._molecules:
-        if molecule._conformer_count > 1:
-            count = molecule._conformer_count
-            for i in range(count):
-                new_molecule = molecule._deep_copy()
-                new_molecule._names = [molecule._names[i]]
-                new_molecule._associateds = [molecule._associateds[i]]
-                for new_chain in new_molecule._chains:
-                    for new_residue in new_chain._residues:
-                        for new_atom in new_residue._atoms:
-                            if not new_atom._in_conformer[i]:
-                                deleted_atoms.append(new_atom)
-                            new_atom._positions = [new_atom._positions[i]]
-                            new_atom._in_conformer = [True]
-                        _delete_atoms(deleted_atoms)
-                        for new_bond in new_residue._bonds:
-                            if not new_bond._in_conformer[i]:
-                                deleted_bonds.append(new_bond)
-                            new_bond._kinds = [new_bond._kinds[i]]
-                            new_bond._in_conformer = [True]
-                        _delete_bonds(deleted_bonds)
-                        if len(new_residue._atoms) == 0:
-                            deleted_residues.append(new_residue)
-                    _delete_residues(deleted_residues)
-                    if len(new_chain._residues) == 0:
-                        deleted_chains.append(new_chain)
-                _delete_chains(deleted_chains)
-                new_molecule._conformer_count = 1
-                new_complex._add_molecule(new_molecule)
-        else:
-            new_complex._add_molecule(molecule._deep_copy())
+        count = molecule._conformer_count
+        for i in range(count):
+            new_complex.add_molecule(molecule._deep_copy(i))
     return new_complex
 
 def convert_to_conformers(complex, force_conformer = None): #Data.Complex -> Data.Complex
     frame_count = len(complex._molecules)
     # Maybe conformers are disabled
     if frame_count <= 1 or s_ConformersDisabled:
         return complex._deep_copy()
@@ -135,14 +73,15 @@
                 names_dictionary.clear()
 
                 for atom in residue._atoms:
                     name_hash = _get_hash_code(atom.name)
                     off = 0
                     if name_hash in names_dictionary:
                         off = names_dictionary[name_hash]
+                    off +=1
                     names_dictionary[name_hash] = off
                     # Lookup or create atom with hash
                     hash_atom = _get_atom_hash(sb, atom, off)
                     new_atom = None
                     if hash_atom in new_atoms:
                         new_atom = new_atoms[hash_atom]
                     else:
@@ -185,15 +124,15 @@
             # Update current conformer
             new_bond._in_conformer[molecule_index] = True
             new_bond._kinds[molecule_index] = bond.kind
             # Count bonds
             bond_total_count+=1
 
         for atom in molecule.atoms:
-            for bond in molecule.bonds:
+            for bond in atom.bonds:
                 atom_info_1 = atoms_dictionary[bond._atom1._unique_identifier]
                 atom_info_2 = atoms_dictionary[bond._atom2._unique_identifier]
 
                 # Lookup the parent residue
                 residue = bond._parent
                 hash_residue = _get_residue_hash(sb, residue)
                 new_residue = new_residues[hash_residue]
@@ -238,42 +177,30 @@
 
 def _get_chain_hash(sb, chain): #StringBuilder, Data.Chain -> int
     return _get_hash_code(chain.name)
 
 def _get_residue_hash(sb, residue): #StringBuilder, Data.Residue -> int
     sb.clear()
     sb.append(residue._serial)
-    sb.append(":")
-    sb.append(residue._name)
-    sb.append(":")
-    sb.append(residue._chain._name)
-    return _get_hash_code(sb.to_string())
+    sb.append_string(residue._name)
+    sb.append_string(residue._chain._name)
+    return _get_hash_code(sb.to_string(":"))
 
 def _get_atom_hash(sb, atom, off): #StringBuilder, Data.Atom, int -> int
     sb.clear()
     sb.append(atom._symbol)
-    sb.append(":")
-    sb.append(atom._name)
-    sb.append(":")
+    sb.append_string(atom._name)
     sb.append(atom._is_het)
-    sb.append(":")
     sb.append(off)
-    sb.append(":")
     sb.append(atom._residue._serial)
-    sb.append(":")
-    sb.append(atom._residue._name)
-    sb.append(":")
-    sb.append(atom._residue._chain._name)
-    return _get_hash_code(sb.to_string())
+    sb.append_string(atom._residue._name)
+    sb.append_string(atom._residue._chain._name)
+    return _get_hash_code(sb.to_string(":"))
 
 def _get_bond_hash(sb, bond, atom1, atom2): #StringBuilder, Data.Bond, int, int -> int
     sb.clear()
     sb.append(atom1)
-    sb.append(":")
     sb.append(atom2)
-    sb.append(":")
     sb.append(bond._residue._serial)
-    sb.append(":")
-    sb.append(bond._residue._name)
-    sb.append(":")
-    sb.append(bond._chain._name)
-    return _get_hash_code(sb.to_string())
+    sb.append_string(bond._residue._name)
+    sb.append_string(bond._chain._name)
+    return _get_hash_code(sb.to_string(":"))
```

### Comparing `nanome-0.8.3/nanome/_internal/_structure/_io/_mmcif/content.py` & `nanome-0.9.0/nanome/_internal/_structure/_io/_mmcif/content.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_structure/_io/_mmcif/parse.py` & `nanome-0.9.0/nanome/_internal/_structure/_io/_mmcif/parse.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_structure/_io/_mmcif/save.py` & `nanome-0.9.0/nanome/_internal/_structure/_io/_mmcif/save.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_structure/_io/_mmcif/structure.py` & `nanome-0.9.0/nanome/_internal/_structure/_io/_mmcif/structure.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,30 +31,30 @@
         if not atom_id in all_atoms:
             if not residue_id in all_residues:
                 if not chain_id in all_chains:
                     if not molecule_id in all_molecules:
                         molecule = _Molecule._create()
                         molecule._name = str(c_atom.model)
                         all_molecules[molecule_id] = molecule
-                        complex._molecules.append(molecule)
+                        complex._add_molecule(molecule)
                     chain = _Chain._create()
                     chain._name = chain_name
                     all_chains[chain_id] = chain
-                    all_molecules[molecule_id]._chains.append(chain)
+                    all_molecules[molecule_id]._add_chain(chain)
                 residue = _Residue._create()
                 residue._name = c_atom.residue_name
                 residue._type = residue._name
                 residue.serial = c_atom.residue_serial
                 all_residues[residue_id] = residue
-                all_chains[chain_id]._residues.append(residue)
+                all_chains[chain_id]._add_residue(residue)
             atom = StructureAtom(c_atom, helper)
             all_atoms[atom_id] = None
-            all_residues[residue_id]._atoms.append(atom)
+            all_residues[residue_id]._add_atom(atom)
     # Done
-    return complex._convert_to_frames()
+    return complex._convert_to_conformers()
 
 def StructureAtom(c_atom, helper):
     atom = _Atom._create()
     atom._serial = c_atom.atom_serial
     atom._occupancy = c_atom.occupancy
     atom._bfactor = c_atom.bfactor
     atom._position = Vector3(c_atom.x, c_atom.y, c_atom.z)
```

### Comparing `nanome-0.8.3/nanome/_internal/_structure/_io/_pdb/content.py` & `nanome-0.9.0/nanome/_internal/_structure/_io/_pdb/content.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_structure/_io/_pdb/parse.py` & `nanome-0.9.0/nanome/_internal/_structure/_io/_pdb/parse.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_structure/_io/_pdb/save.py` & `nanome-0.9.0/nanome/_internal/_structure/_io/_pdb/save.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_structure/_io/_pdb/structure.py` & `nanome-0.9.0/nanome/_internal/_structure/_io/_pdb/structure.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
     for ratom in content.atoms:
         atoms_by_molecule[ratom.model_number - 1].append(ratom)
     complex = _Complex._create()
     complex._remarks = content._remarks
     for i in range(num_molecules):
         molecule = structure_molecule(atoms_by_molecule[i], content.compnds)
         molecule._name = str(i)
-        complex._molecules.append(molecule)
+        complex._add_molecule(molecule)
     # Done
-    return complex._convert_to_frames()
+    return complex._convert_to_conformers()
         
          
 def structure_molecule(atoms, compnds):
     # All structured infos
     all_residues = {} #<string, Residue>
     all_chains = {} #<string, Chain>
     all_atoms = {} #<string, Atom>
@@ -50,21 +50,21 @@
                 chain_id = ratom.chain_identifier
                 if ratom.is_het_atom:
                     chain_id = "H" + chain_id
                 if not chain_id in all_chains:
                     chain = _Chain._create()
                     chain._name = chain_id
                     all_chains[chain_id] = chain
-                all_chains[chain_id]._residues.append(residue)
-            all_residues[residue_id]._atoms.append(atom)
+                all_chains[chain_id]._add_residue(residue)
+            all_residues[residue_id]._add_atom(atom)
             all_atoms[atom_id] = atom
     # Final molecule
     molecule = _Molecule._create()
     # Assemble molecule contents
     for chain in all_chains:
-        molecule._chains.append(all_chains[chain])
+        molecule._add_chain(all_chains[chain])
     # Done
     return molecule
```

### Comparing `nanome-0.8.3/nanome/_internal/_structure/_io/_sdf/content.py` & `nanome-0.9.0/nanome/_internal/_structure/_io/_sdf/content.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_structure/_io/_sdf/parse.py` & `nanome-0.9.0/nanome/_internal/_structure/_io/_sdf/parse.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_structure/_io/_sdf/save.py` & `nanome-0.9.0/nanome/_internal/_structure/_io/_sdf/save.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_structure/_io/_sdf/structure.py` & `nanome-0.9.0/nanome/_internal/_structure/_io/_sdf/structure.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,45 +2,45 @@
 from nanome._internal._structure import _Complex, _Molecule, _Chain, _Residue, _Bond, _Atom
 from .content import Content
 
 def structure(content):
     # type: (Content) -> Complex
     complex = _Complex._create()
     for model in content.models:
-        complex._molecules.append(structure_molecule(model))
+        complex._add_molecule(structure_molecule(model))
     complex._remarks = {}
-    return complex._convert_to_frames()
+    return complex._convert_to_conformers()
 
 
 def structure_molecule(model):
     # type: (Content.Model) -> Molecule
     molecule = _Molecule._create()
     molecule._name = model.name
 
     chain = _Chain._create()
     chain._name = "S"
-    molecule._chains.append(chain)
+    molecule._add_chain(chain)
     residue = _Residue._create()
     residue._name = "SDF"
     residue._type = residue._name
     residue.serial = 1
-    chain._residues.append(residue)
+    chain._add_residue(residue)
     atoms_by_serial = {}
 
     for catom in model.atoms:
         atom = _Atom._create()
         atom._symbol = catom.symbol
         atom._serial = catom.serial
         atom._position = Vector3(catom.x, catom.y, catom.z)
         atom._name = catom.symbol
         atom._is_het = True
-        residue._atoms.append(atom)
+        residue._add_atom(atom)
         atoms_by_serial[atom._serial] = atom
     for cbond in model.bonds:
         if cbond.serial_atom1 in atoms_by_serial and cbond.serial_atom2 in atoms_by_serial:
             bond = _Bond._create()
             bond._atom1 = atoms_by_serial[cbond.serial_atom1]
             bond._atom2 = atoms_by_serial[cbond.serial_atom2]
             bond._kind = cbond.bond_order
-            residue._bonds.append(bond)
+            residue._add_bond(bond)
     molecule._associated = model._associated
     return molecule
```

### Comparing `nanome-0.8.3/nanome/_internal/_structure/_molecule.py` & `nanome-0.9.0/nanome/_internal/_structure/_molecule.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from . import _Base
 from . import _helpers
+import copy
 
 class _Molecule(_Base):
     @classmethod
     def _create(cls):
         return cls()
 
     def __init__(self):
@@ -134,17 +135,24 @@
             atom._copy_conformer(src, index)
         for bond in self._bonds:
             bond._copy_conformer(src, index)
         self.__conformer_count += 1
 
     #endregion
 
-    def _shallow_copy(self):
+        #copies the structure. If conformer_number is not None it will only copy that conformer's data
+    def _shallow_copy(self, conformer_number = None):
         molecule = _Molecule._create()
-        molecule._current_conformer = self._current_conformer
-        molecule.__conformer_count = self.__conformer_count
-        molecule._names = list(self._names)
-        molecule._associateds = list(self._associateds)
+        if conformer_number == None:
+            molecule._names = list(self._names)
+            molecule._associateds = copy.deepcopy(self._associateds)
+            molecule.__conformer_count = self.__conformer_count
+            molecule._current_conformer = self._current_conformer
+        else:
+            molecule._name = self._names[conformer_number]
+            molecule._associated = self._associateds[conformer_number]
+            molecule.__conformer_count = 1
+            molecule._current_conformer = 0
         return molecule
 
-    def _deep_copy(self):
-        return _helpers._copy._deep_copy_molecule(self)
+    def _deep_copy(self, conformer_number = None):
+        return _helpers._copy._deep_copy_molecule(self, conformer_number)
```

### Comparing `nanome-0.8.3/nanome/_internal/_structure/_residue.py` & `nanome-0.9.0/nanome/_internal/_structure/_residue.py`

 * *Files 11% similar despite different names*

```diff
@@ -77,15 +77,16 @@
         parent = self._parent
         if parent:
             return parent._complex
         else:
             return None
     #endregion
 
-    def _shallow_copy(self):
+    #copies the structure. If conformer_number is not None it will only copy that conformer's data
+    def _shallow_copy(self, conformer_number = None):
         residue = _Residue._create()
         #molecular
         residue._type = self._type 
         residue._serial = self._serial 
         residue._name = self._name 
         residue._secondary_structure = self._secondary_structure 
         #rendering
@@ -93,9 +94,9 @@
         residue._ribbon_size = self._ribbon_size 
         residue._ribbon_mode = self._ribbon_mode 
         residue._ribbon_color = self._ribbon_color.copy()
         residue._labeled = self._labeled 
         residue._label_text = self._label_text 
         return residue
 
-    def _deep_copy(self):
-        return _helpers._copy._deep_copy_residue(self)
+    def _deep_copy(self, conformer_number = None):
+        return _helpers._copy._deep_copy_residue(self, conformer_number)
```

### Comparing `nanome-0.8.3/nanome/_internal/_structure/_serialization/_atom_serializer.py` & `nanome-0.9.0/nanome/_internal/_structure/_serialization/_atom_serializer.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_structure/_serialization/_atom_serializer_id.py` & `nanome-0.9.0/nanome/_internal/_structure/_serialization/_atom_serializer_id.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_structure/_serialization/_bond_serializer.py` & `nanome-0.9.0/nanome/_internal/_structure/_serialization/_bond_serializer.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_structure/_serialization/_chain_serializer.py` & `nanome-0.9.0/nanome/_internal/_structure/_serialization/_chain_serializer.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_structure/_serialization/_complex_serializer.py` & `nanome-0.9.0/nanome/_internal/_structure/_serialization/_complex_serializer.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_structure/_serialization/_molecule_serializer.py` & `nanome-0.9.0/nanome/_internal/_structure/_serialization/_molecule_serializer.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_structure/_serialization/_residue_serializer.py` & `nanome-0.9.0/nanome/_internal/_structure/_serialization/_residue_serializer.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_structure/_serialization/_workspace_serializer.py` & `nanome-0.9.0/nanome/_internal/_structure/_serialization/_workspace_serializer.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_structure/_workspace.py` & `nanome-0.9.0/nanome/_internal/_structure/_workspace.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_ui/_button.py` & `nanome-0.9.0/nanome/_internal/_ui/_button.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_ui/_image.py` & `nanome-0.9.0/nanome/_internal/_ui/_image.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_ui/_io/_button_json.py` & `nanome-0.9.0/nanome/_internal/_ui/_io/_button_json.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_ui/_io/_image_json.py` & `nanome-0.9.0/nanome/_internal/_ui/_io/_image_json.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_ui/_io/_label_json.py` & `nanome-0.9.0/nanome/_internal/_ui/_io/_label_json.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_ui/_io/_layout_node_json.py` & `nanome-0.9.0/nanome/_internal/_ui/_io/_layout_node_json.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_ui/_io/_loading_bar_json.py` & `nanome-0.9.0/nanome/_internal/_ui/_io/_loading_bar_json.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_ui/_io/_menu_json.py` & `nanome-0.9.0/nanome/_internal/_ui/_io/_menu_json.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_ui/_io/_slider_json.py` & `nanome-0.9.0/nanome/_internal/_ui/_io/_slider_json.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_ui/_io/_text_input_json.py` & `nanome-0.9.0/nanome/_internal/_ui/_io/_text_input_json.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_ui/_io/_ui_base_json.py` & `nanome-0.9.0/nanome/_internal/_ui/_io/_ui_base_json.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_ui/_io/_ui_list_json.py` & `nanome-0.9.0/nanome/_internal/_ui/_io/_ui_list_json.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_ui/_label.py` & `nanome-0.9.0/nanome/_internal/_ui/_label.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_ui/_layout_node.py` & `nanome-0.9.0/nanome/_internal/_ui/_layout_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,16 +52,17 @@
             child_node._parent._remove_child(child_node)
         #add to curr parent
         self._children.append(child_node)
         child_node._parent = self
         self._save_changes()
 
     def _remove_child(self, child_node):
-        self._children.remove(child_node)
-        child_node._parent = None
+        if child_node in self._children:
+            self._children.remove(child_node)
+            child_node._parent = None
         self._save_changes()
 
     def _clear_children(self):
         for child in self._children:
             child._parent = None
         self._children = []
         self._save_changes()
```

### Comparing `nanome-0.8.3/nanome/_internal/_ui/_loading_bar.py` & `nanome-0.9.0/nanome/_internal/_ui/_loading_bar.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_ui/_menu.py` & `nanome-0.9.0/nanome/_internal/_ui/_menu.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 
 class _Menu(object):
 
     @classmethod
     def _create(cls):
         return cls()
 
-    def __init__(self, title = "title"):
+    def __init__(self, index = 0, title = "title"):
         #Protocol
         self._enabled = True
         self._id = 0
         self._title = title
         self._locked = False
         self._width = 0.7
         self._height = 0.6
+        self._index = index
         #self.all_layout_nodes[]
         #self.all_contents[]
 
         #API
         self._root = _LayoutNode._create()
         self._opened_callback = lambda self: None
         self._closed_callback = lambda self: None
@@ -47,8 +48,9 @@
 
     def _copy_data(self, other):
         self._enabled = other._enabled
         self._title = other._title
         self._locked = other._locked
         self._width = other._width
         self._height = other._height
+        self._index = other._index
```

### Comparing `nanome-0.8.3/nanome/_internal/_ui/_serialization/__init__.py` & `nanome-0.9.0/nanome/_internal/_ui/_serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_ui/_serialization/_button_serializer.py` & `nanome-0.9.0/nanome/_internal/_ui/_serialization/_button_serializer.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_ui/_serialization/_image_serializer.py` & `nanome-0.9.0/nanome/_internal/_ui/_serialization/_image_serializer.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_ui/_serialization/_label_serializer.py` & `nanome-0.9.0/nanome/_internal/_ui/_serialization/_label_serializer.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_ui/_serialization/_layout_node_serializer.py` & `nanome-0.9.0/nanome/_internal/_ui/_serialization/_layout_node_serializer.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_ui/_serialization/_layout_node_serializer_deep.py` & `nanome-0.9.0/nanome/_internal/_ui/_serialization/_layout_node_serializer_deep.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_ui/_serialization/_loading_bar_serializer.py` & `nanome-0.9.0/nanome/_internal/_ui/_serialization/_loading_bar_serializer.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_ui/_serialization/_menu_serializer.py` & `nanome-0.9.0/nanome/_internal/_ui/_serialization/_menu_serializer.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_ui/_serialization/_mesh_serializer.py` & `nanome-0.9.0/nanome/_internal/_ui/_serialization/_mesh_serializer.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_ui/_serialization/_slider_serializer.py` & `nanome-0.9.0/nanome/_internal/_ui/_serialization/_slider_serializer.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_ui/_serialization/_text_input_serializer.py` & `nanome-0.9.0/nanome/_internal/_ui/_serialization/_text_input_serializer.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_ui/_serialization/_ui_base_serializer.py` & `nanome-0.9.0/nanome/_internal/_ui/_serialization/_ui_base_serializer.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_ui/_serialization/_ui_list_serializer.py` & `nanome-0.9.0/nanome/_internal/_ui/_serialization/_ui_list_serializer.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_ui/_slider.py` & `nanome-0.9.0/nanome/_internal/_ui/_slider.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_ui/_text_input.py` & `nanome-0.9.0/nanome/_internal/_ui/_text_input.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_ui/_ui_list.py` & `nanome-0.9.0/nanome/_internal/_ui/_ui_list.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_util/_serializers/__init__.py` & `nanome-0.9.0/nanome/_internal/_util/_serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_util/_serializers/_array_serializer.py` & `nanome-0.9.0/nanome/_internal/_util/_serializers/_array_serializer.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_util/_serializers/_dictionary_serializer.py` & `nanome-0.9.0/nanome/_internal/_util/_serializers/_dictionary_serializer.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_util/_serializers/_directory_entry_serializer.py` & `nanome-0.9.0/nanome/_internal/_util/_serializers/_directory_entry_serializer.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_util/_serializers/_file_data_serializer.py` & `nanome-0.9.0/nanome/_internal/_util/_serializers/_file_data_serializer.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_util/_serializers/_file_save_data_serializer.py` & `nanome-0.9.0/nanome/_internal/_util/_serializers/_file_save_data_serializer.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_util/_serializers/_quaternion_serializer.py` & `nanome-0.9.0/nanome/_internal/_util/_serializers/_quaternion_serializer.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_util/_serializers/_string_serializer.py` & `nanome-0.9.0/nanome/_internal/_util/_serializers/_string_serializer.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_util/_serializers/_tuple_serializer.py` & `nanome-0.9.0/nanome/_internal/_util/_serializers/_tuple_serializer.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_util/_serializers/_type_serializer.py` & `nanome-0.9.0/nanome/_internal/_util/_serializers/_type_serializer.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_util/_serializers/_vector3_serializer.py` & `nanome-0.9.0/nanome/_internal/_util/_serializers/_vector3_serializer.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_volumetric/_io/_em_map/_parse.py` & `nanome-0.9.0/nanome/_internal/_volumetric/_io/_em_map/_parse.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_volumetric/_serialization/_volume_data_serializer.py` & `nanome-0.9.0/nanome/_internal/_volumetric/_serialization/_volume_data_serializer.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/_internal/_volumetric/_volume_data.py` & `nanome-0.9.0/nanome/_internal/_volumetric/_volume_data.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/api/macro/macro.py` & `nanome-0.9.0/nanome/api/macro/macro.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/api/plugin.py` & `nanome-0.9.0/nanome/api/plugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,14 +27,24 @@
     def setup(cls, name, description, category, has_advanced, plugin_class, host = "config", port = "config", key_file = "config"):
         if not _Plugin._is_process():
             plugin = cls(name, description, category, has_advanced)
             plugin.set_plugin_class(plugin_class)
             plugin.run(host, port, key_file)
 
     @staticmethod
+    def set_custom_data(*args):
+        """
+        | Store arbitrary data to send to plugin instances
+
+        :param args: Variable length argument list
+        :type args: Anything serializable
+        """
+        _Plugin._custom_data = args
+
+    @staticmethod
     def set_maximum_processes_count(max_process_nb):
         _ProcessManager._max_process_count = max_process_nb
 
     def run(self, host = "config", port = "config", key_file = "config"):
         """
         | Starts the plugin by connecting to the server specified.
         | If arguments (-a, -p) are given when starting plugin, host/port will be ignored.
```

### Comparing `nanome-0.8.3/nanome/api/plugin_instance.py` & `nanome-0.9.0/nanome/api/plugin_instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,14 +192,23 @@
         | Update a specific UI element (button, slider, list...)
 
         :param content: UI element to update
         :type content: :class:`~nanome.api.ui.ui_base`
         """
         self._network._send(_Messages.content_update, content)
 
+    def update_node(self, node):
+        """
+        | Update a layout node and its children
+
+        :param node: Layout node to update
+        :type node: :class:`~nanome.api.ui.layout_node`
+        """
+        self._network._send(_Messages.node_update, node)
+
     def request_directory(self, path, callback = None, pattern = "*"):
         """
         | Requests the content of a directory on the machine running Nanome
 
         :param path: Path to request. E.g. "." means Nanome's running directory
         :type path: str
         :param pattern: Pattern to match. E.g. "*.txt" will match all .txt files. Default value is "*" (match everything)
@@ -349,11 +358,20 @@
 
     @property
     def plugin_files_path(self):
         path = os.path.expanduser(config.fetch('plugin_files_path'))
         if not os.path.exists(path):
             os.makedirs(path)
         return path
+
+    @property
+    def custom_data(self):
+        """
+        Get custom data set with Plugin.set_custom_data
+
+        :type: tuple of objects or None if no data has been set
+        """
+        return self._custom_data
         
 class _DefaultPlugin(PluginInstance):
     def __init__(self):
         pass
```

### Comparing `nanome-0.8.3/nanome/api/streams/stream.py` & `nanome-0.9.0/nanome/api/streams/stream.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/api/structure/atom.py` & `nanome-0.9.0/nanome/api/structure/atom.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/api/structure/bond.py` & `nanome-0.9.0/nanome/api/structure/bond.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/api/structure/chain.py` & `nanome-0.9.0/nanome/api/structure/chain.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/api/structure/complex.py` & `nanome-0.9.0/nanome/api/structure/complex.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/api/structure/io/complex_io.py` & `nanome-0.9.0/nanome/api/structure/io/complex_io.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/api/structure/molecule.py` & `nanome-0.9.0/nanome/api/structure/molecule.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/api/structure/residue.py` & `nanome-0.9.0/nanome/api/structure/residue.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/api/structure/workspace.py` & `nanome-0.9.0/nanome/api/structure/workspace.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/api/ui/button.py` & `nanome-0.9.0/nanome/api/ui/button.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/api/ui/image.py` & `nanome-0.9.0/nanome/api/ui/image.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/api/ui/io/layout_node_io.py` & `nanome-0.9.0/nanome/api/ui/io/layout_node_io.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/api/ui/io/menu_io.py` & `nanome-0.9.0/nanome/api/ui/io/menu_io.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/api/ui/label.py` & `nanome-0.9.0/nanome/api/ui/label.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/api/ui/layout_node.py` & `nanome-0.9.0/nanome/api/ui/layout_node.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/api/ui/loading_bar.py` & `nanome-0.9.0/nanome/api/ui/loading_bar.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/api/ui/menu.py` & `nanome-0.9.0/nanome/api/ui/menu.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from nanome._internal._ui import _Menu
 from .io import MenuIO
 
 class Menu(_Menu):
     io = MenuIO()
-    def __init__(self):
-        _Menu.__init__(self)
+    def __init__(self, index = 0, title = "title"):
+        _Menu.__init__(self, index, title)
         self.io = MenuIO(self)
     
     def register_closed_callback(self, func):
         self._closed_callback = func
 
     def register_opened_callback(self, func):
         self._opened_callback = func
@@ -59,14 +59,22 @@
     @property
     def height(self):
         return self._height
     
     @height.setter
     def height(self, value):
         self._height = value
+
+    @property
+    def index(self):
+        return self._index
+    
+    @index.setter
+    def index(self, value):
+        self._index = value
     #endregion
 
     def find_content(self, content_id):
         return self._find_content(content_id)
 
     def get_all_content(self):
         return self._get_all_content()
```

### Comparing `nanome-0.8.3/nanome/api/ui/slider.py` & `nanome-0.9.0/nanome/api/ui/slider.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/api/ui/text_input.py` & `nanome-0.9.0/nanome/api/ui/text_input.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/api/ui/ui_list.py` & `nanome-0.9.0/nanome/api/ui/ui_list.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/api/user/presenter_info.py` & `nanome-0.9.0/nanome/api/user/presenter_info.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/setup_config.py` & `nanome-0.9.0/nanome/setup_config.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/util/__init__.py` & `nanome-0.9.0/nanome/util/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from . import *
 #classes
 from .string_builder import StringBuilder
 from .color import Color
+from .logs import Logs
 from .enum import Enum, IntEnum, auto
 try:
     from .enum import reset_auto
 except:
     pass
 
 from . import enums
 from . import complex_save_options
 
 from .import_utils import ImportUtils
-from .logs import Logs
 from .octree import Octree
 from .quaternion import Quaternion
 from .vector3 import Vector3
 from .matrix import Matrix
 from .file import DirectoryErrorCode, DirectoryRequestResult, DirectoryRequestOptions, FileErrorCode, FileData, FileSaveData, DirectoryEntry
 from .process import Process
```

### Comparing `nanome-0.8.3/nanome/util/color.py` & `nanome-0.9.0/nanome/util/color.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/util/config.py` & `nanome-0.9.0/nanome/util/config.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/util/enum.py` & `nanome-0.9.0/nanome/util/enum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+from . import Logs
 import sys
 
 @classmethod
 def safe_cast(cls, value):
     try:
         return cls(value)
     except ValueError:
         if cls.cast_failed_warning == False:
             cls.cast_failed_warning = True
             Logs.warning("Invalid value", value, "for enum", cls.__name__, ". Library might outdated.")
-        return cls(0)
+        return list(cls)[0]
 
 if sys.version_info >= (3, 4):
     from enum import Enum, IntEnum
 else:
 
 # Python 2 Enum Classes
 
@@ -893,8 +894,8 @@
         return result
 
     def reset_auto():
         global __enum_auto_value
         __enum_auto_value = 0
 
 Enum.safe_cast = safe_cast
-Enum.cast_failed_warning = False
+Enum.cast_failed_warning = False
```

### Comparing `nanome-0.8.3/nanome/util/enums.py` & `nanome-0.9.0/nanome/util/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     Wire = 2
     VanDerWaals = 3
     Point = 4
     BFactor = 5
     Adaptive = 6
 
 class Kind(IntEnum):
+    Unknown = 0
     CovalentSingle = 1
     CovalentDouble = 2
     CovalentTriple = 3
     Hydrogen = 4
     HydrogenWater = 5
 
 class RibbonMode(IntEnum):
```

### Comparing `nanome-0.8.3/nanome/util/file.py` & `nanome-0.9.0/nanome/util/file.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/util/import_utils.py` & `nanome-0.9.0/nanome/util/import_utils.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/util/logs.py` & `nanome-0.9.0/nanome/util/logs.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/util/matrix.py` & `nanome-0.9.0/nanome/util/matrix.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/util/octree.py` & `nanome-0.9.0/nanome/util/octree.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/util/process.py` & `nanome-0.9.0/nanome/util/process.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/util/quaternion.py` & `nanome-0.9.0/nanome/util/quaternion.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome/util/vector3.py` & `nanome-0.9.0/nanome/util/vector3.py`

 * *Files identical despite different names*

### Comparing `nanome-0.8.3/nanome.egg-info/PKG-INFO` & `nanome-0.9.0/nanome.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanome
-Version: 0.8.3
+Version: 0.9.0
 Summary: Python API for Nanome Plugins
 Home-page: https://github.com/nanome-ai/nanome
 Author: Nanome
 Author-email: hello@nanome.ai
 License: MIT
 Description: # Nanome
```

### Comparing `nanome-0.8.3/nanome.egg-info/SOURCES.txt` & `nanome-0.9.0/nanome.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -79,14 +79,15 @@
 nanome/_internal/_network/_commands/_serialization/_run.py
 nanome/_internal/_network/_commands/_serialization/_send_notification.py
 nanome/_internal/_network/_commands/_serialization/_set_plugin_list_button.py
 nanome/_internal/_network/_commands/_serialization/_slider_callback.py
 nanome/_internal/_network/_commands/_serialization/_text_input_callback.py
 nanome/_internal/_network/_commands/_serialization/_update_content.py
 nanome/_internal/_network/_commands/_serialization/_update_menu.py
+nanome/_internal/_network/_commands/_serialization/_update_node.py
 nanome/_internal/_network/_commands/_serialization/_update_structures.py
 nanome/_internal/_network/_commands/_serialization/_update_structures_deep_done.py
 nanome/_internal/_network/_commands/_serialization/_update_workspace.py
 nanome/_internal/_network/_commands/_serialization/_upload_cryo_em.py
 nanome/_internal/_network/_commands/_serialization/_upload_cryo_em_done.py
 nanome/_internal/_network/_serialization/__init__.py
 nanome/_internal/_network/_serialization/_context.py
```

### Comparing `nanome-0.8.3/setup.py` & `nanome-0.9.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages, setup
 
 README = (pathlib.Path(__file__).parent / "README.md").read_text()
 
 setup(
     name = 'nanome',
     packages=find_packages(exclude=["testing","doc","test_plugins"]),
-    version = '0.8.3',
+    version = '0.9.0',
     license='MIT',
     description = 'Python API for Nanome Plugins',
     long_description = README,
     long_description_content_type = "text/markdown",
     author = 'Nanome',
     author_email = 'hello@nanome.ai',
     url = 'https://github.com/nanome-ai/nanome',
```

